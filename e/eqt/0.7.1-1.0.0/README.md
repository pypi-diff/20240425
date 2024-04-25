# Comparing `tmp/eqt-0.7.1.tar.gz` & `tmp/eqt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eqt-0.7.1.tar", last modified: Mon Aug  7 14:29:00 2023, max compression
+gzip compressed data, was "eqt-1.0.0.tar", last modified: Thu Apr 25 13:43:42 2024, max compression
```

## Comparing `eqt-0.7.1.tar` & `eqt-1.0.0.tar`

### file list

```diff
@@ -1,54 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:00.403427 eqt-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-07 14:28:41.000000 eqt-0.7.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:00.395427 eqt-0.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:00.399428 eqt-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-08-07 14:28:41.000000 eqt-0.7.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-07 14:28:41.000000 eqt-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-07 14:28:41.000000 eqt-0.7.1/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-07 14:28:41.000000 eqt-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-07 14:28:41.000000 eqt-0.7.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-07 14:28:41.000000 eqt-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-08-07 14:29:00.403427 eqt-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-08-07 14:28:41.000000 eqt-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:00.399428 eqt-0.7.1/eqt/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-07 14:28:41.000000 eqt-0.7.1/eqt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 14:29:00.000000 eqt-0.7.1/eqt/_dist_ver.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-07 14:28:41.000000 eqt-0.7.1/eqt/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:00.399428 eqt-0.7.1/eqt/threading/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-08-07 14:28:41.000000 eqt-0.7.1/eqt/threading/QtThreading.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-07 14:28:41.000000 eqt-0.7.1/eqt/threading/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:00.403427 eqt-0.7.1/eqt/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-08-07 14:28:41.000000 eqt-0.7.1/eqt/ui/FormDialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-08-07 14:28:41.000000 eqt-0.7.1/eqt/ui/MainWindowWithProgressDialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23836 2023-08-07 14:28:41.000000 eqt-0.7.1/eqt/ui/MainWindowWithSessionManagement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-07 14:28:41.000000 eqt-0.7.1/eqt/ui/ProgressTimerDialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-08-07 14:28:41.000000 eqt-0.7.1/eqt/ui/ReOrderableListWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-08-07 14:28:41.000000 eqt-0.7.1/eqt/ui/SessionDialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16771 2023-08-07 14:28:41.000000 eqt-0.7.1/eqt/ui/UIFormWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-08-07 14:28:41.000000 eqt-0.7.1/eqt/ui/UIMultiStepWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-07 14:28:41.000000 eqt-0.7.1/eqt/ui/UISliderWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-08-07 14:28:41.000000 eqt-0.7.1/eqt/ui/UIStackedWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-07 14:28:41.000000 eqt-0.7.1/eqt/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:00.399428 eqt-0.7.1/eqt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-08-07 14:29:00.000000 eqt-0.7.1/eqt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-08-07 14:29:00.000000 eqt-0.7.1/eqt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:29:00.000000 eqt-0.7.1/eqt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-07 14:29:00.000000 eqt-0.7.1/eqt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 14:29:00.000000 eqt-0.7.1/eqt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:00.403427 eqt-0.7.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-08-07 14:28:41.000000 eqt-0.7.1/examples/MainWindowWithSessionManagement_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-07 14:28:41.000000 eqt-0.7.1/examples/dialog_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-07 14:28:41.000000 eqt-0.7.1/examples/dialog_example_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-08-07 14:28:41.000000 eqt-0.7.1/examples/dialog_multistep_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-08-07 14:28:41.000000 eqt-0.7.1/examples/dialog_save_state_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-08-07 14:28:41.000000 eqt-0.7.1/examples/progress_timer_dialog_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-07 14:28:41.000000 eqt-0.7.1/examples/reorderable_list_widget_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-08-07 14:28:41.000000 eqt-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 14:29:00.407427 eqt-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:29:00.403427 eqt-0.7.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-08-07 14:28:41.000000 eqt-0.7.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-08-07 14:28:41.000000 eqt-0.7.1/test/dialog_example_2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20428 2023-08-07 14:28:41.000000 eqt-0.7.1/test/test_MainWindowWithSessionManagement.py
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-08-07 14:28:41.000000 eqt-0.7.1/test/test_SessionDialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24245 2023-08-07 14:28:41.000000 eqt-0.7.1/test/test__formUI_status_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-07 14:28:41.000000 eqt-0.7.1/test/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:42.103487 eqt-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-25 13:43:32.000000 eqt-1.0.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:42.091487 eqt-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:42.095487 eqt-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-25 13:43:32.000000 eqt-1.0.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-25 13:43:32.000000 eqt-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-25 13:43:32.000000 eqt-1.0.0/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-25 13:43:32.000000 eqt-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-04-25 13:43:32.000000 eqt-1.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-25 13:43:32.000000 eqt-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-25 13:43:32.000000 eqt-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-04-25 13:43:42.099487 eqt-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-04-25 13:43:32.000000 eqt-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:42.095487 eqt-1.0.0/eqt/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-25 13:43:32.000000 eqt-1.0.0/eqt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 13:43:42.000000 eqt-1.0.0/eqt/_dist_ver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-25 13:43:32.000000 eqt-1.0.0/eqt/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:42.095487 eqt-1.0.0/eqt/threading/
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-25 13:43:32.000000 eqt-1.0.0/eqt/threading/QtThreading.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-25 13:43:32.000000 eqt-1.0.0/eqt/threading/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:42.099487 eqt-1.0.0/eqt/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)    18054 2024-04-25 13:43:32.000000 eqt-1.0.0/eqt/ui/FormDialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-04-25 13:43:32.000000 eqt-1.0.0/eqt/ui/MainWindowWithProgressDialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23840 2024-04-25 13:43:32.000000 eqt-1.0.0/eqt/ui/MainWindowWithSessionManagement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-25 13:43:32.000000 eqt-1.0.0/eqt/ui/ProgressTimerDialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-25 13:43:32.000000 eqt-1.0.0/eqt/ui/ReOrderableListWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-25 13:43:32.000000 eqt-1.0.0/eqt/ui/SessionDialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28630 2024-04-25 13:43:32.000000 eqt-1.0.0/eqt/ui/UIFormWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-25 13:43:32.000000 eqt-1.0.0/eqt/ui/UIMultiStepWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-25 13:43:32.000000 eqt-1.0.0/eqt/ui/UISliderWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-04-25 13:43:32.000000 eqt-1.0.0/eqt/ui/UIStackedWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-25 13:43:32.000000 eqt-1.0.0/eqt/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:42.099487 eqt-1.0.0/eqt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-04-25 13:43:42.000000 eqt-1.0.0/eqt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-25 13:43:42.000000 eqt-1.0.0/eqt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:43:42.000000 eqt-1.0.0/eqt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 13:43:42.000000 eqt-1.0.0/eqt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-25 13:43:42.000000 eqt-1.0.0/eqt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:42.099487 eqt-1.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-25 13:43:32.000000 eqt-1.0.0/examples/MainWindowWithSessionManagement_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-25 13:43:32.000000 eqt-1.0.0/examples/advanced_dialog_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-25 13:43:32.000000 eqt-1.0.0/examples/dialog_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-25 13:43:32.000000 eqt-1.0.0/examples/dialog_example_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-25 13:43:32.000000 eqt-1.0.0/examples/dialog_example_3_save_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-25 13:43:32.000000 eqt-1.0.0/examples/dialog_multistep_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-25 13:43:32.000000 eqt-1.0.0/examples/dialog_save_state_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-25 13:43:32.000000 eqt-1.0.0/examples/insert_widgets_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-25 13:43:32.000000 eqt-1.0.0/examples/progress_timer_dialog_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-25 13:43:32.000000 eqt-1.0.0/examples/remove_widgets_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-25 13:43:32.000000 eqt-1.0.0/examples/reorderable_list_widget_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-25 13:43:32.000000 eqt-1.0.0/examples/utilitiesForExamples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-25 13:43:32.000000 eqt-1.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:42.099487 eqt-1.0.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-25 13:43:32.000000 eqt-1.0.0/scripts/eqt_env.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 13:43:42.103487 eqt-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:42.099487 eqt-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-25 13:43:32.000000 eqt-1.0.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-25 13:43:32.000000 eqt-1.0.0/test/dialog_example_2_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18619 2024-04-25 13:43:32.000000 eqt-1.0.0/test/test_MainWindowWithSessionManagement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-25 13:43:32.000000 eqt-1.0.0/test/test_MainWindowWithSessionManagementDialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-25 13:43:32.000000 eqt-1.0.0/test/test_SessionDialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47047 2024-04-25 13:43:32.000000 eqt-1.0.0/test/test__formUI_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-25 13:43:32.000000 eqt-1.0.0/test/test_io.py
```

### Comparing `eqt-0.7.1/.github/workflows/test.yml` & `eqt-1.0.0/.github/workflows/test.yml`

 * *Files 7% similar despite different names*

```diff
@@ -7,31 +7,31 @@
     if: github.event_name != 'pull_request' || !contains('OWNER,MEMBER,COLLABORATOR', github.event.pull_request.author_association)
     name: py${{ matrix.python }}
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python: [3.7, 3.11]
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         fetch-depth: 0
-    - uses: actions/setup-python@v4
+    - uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python }}
     - run: pip install -U .[dev]
     - run: pytest
   deploy:
     needs: [test]
     name: PyPI Deploy
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         fetch-depth: 0
-    - uses: actions/setup-python@v4
+    - uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
       id: changes
       name: Check annotated tag
       run: |
         git fetch --tags -f
@@ -46,16 +46,19 @@
           echo "$DELIM" >> "$GITHUB_OUTPUT"
         else
           echo "::error title=Missing tag annotation::$tag"
           changelog=$(git log --pretty='format:%d%n- %s%n%b---' $(git tag --sort=v:refname | tail -n2 | head -n1)..HEAD)
           cat <<EOF >> "$GITHUB_STEP_SUMMARY"
         # Missing tag annotation
         ## Fix
-        See <https://github.com/TomographicImaging/eqt/tree/main/.github/workflows#releasing>.
+        See <https://github.com/TomographicImaging/eqt/tree/main/CONTRIBUTING.md#releasing>.
         ## Suggested body
+        See <https://github.com/TomographicImaging/eqt/tree/main/CHANGELOG.md>.
+        In particular, check that these commits are described:
+
         $changelog
         EOF
           exit 1
         fi
     - id: dist
       uses: casperdcl/deploy-pypi@v2
       with:
```

### Comparing `eqt-0.7.1/.pre-commit-config.yaml` & `eqt-1.0.0/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 default_language_version:
   python: python3
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.4.0
+  rev: v4.5.0
   hooks:
   - id: check-added-large-files
   - id: check-case-conflict
   - id: check-docstring-first
   - id: check-executables-have-shebangs
   - id: check-toml
   - id: check-merge-conflict
@@ -22,34 +22,36 @@
     name: Check TODO
     language: pygrep
     args: [-i]
     entry: TODO
     types: [text]
     exclude: ^(.pre-commit-config.yaml|.github/workflows/test.yml)$
 - repo: https://github.com/PyCQA/flake8
-  rev: 5.0.4
+  rev: 7.0.0
   hooks:
   - id: flake8
     args: [-j8]
     additional_dependencies:
     - flake8-broken-line
     - flake8-bugbear
     - flake8-comprehensions
     - flake8-debugger
     - flake8-isort
     - flake8-pyproject
     - flake8-string-format
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: v1.4.1
+  rev: v1.9.0
   hooks:
   - id: mypy
     additional_dependencies: [types-setuptools]
 - repo: https://github.com/google/yapf
-  rev: v0.40.0
+  rev: v0.40.2
   hooks:
   - id: yapf
     args: [-i]
     additional_dependencies: [toml]
 - repo: https://github.com/PyCQA/isort
-  rev: 5.12.0
+  rev: 5.13.2
   hooks:
   - id: isort
+ci:
+  autofix_prs: false
```

### Comparing `eqt-0.7.1/LICENSE` & `eqt-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eqt-0.7.1/PKG-INFO` & `eqt-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eqt
-Version: 0.7.1
+Version: 1.0.0
 Summary: A number of templates and tools to develop Qt GUIs with Python effectively
 Author-email: Edoardo Pasca <edoardo.pasca@stfc.ac.uk>, Laura Murgatroyd <laura.murgatroyd@stfc.ac.uk>
 Maintainer-email: Casper da Costa-Luis <casper.dcl@physics.org>
 License: Apache-2.0
 Project-URL: documentation, https://github.com/TomographicImaging/eqt#readme
 Project-URL: repository, https://github.com/TomographicImaging/eqt
 Project-URL: changelog, https://github.com/TomographicImaging/eqt/releases
@@ -17,47 +17,45 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: pyside2
+Requires-Dist: qdarkstyle
+Provides-Extra: dev
+Requires-Dist: pytest>=6; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-timeout; extra == "dev"
 
 # eqt: Qt Elements
 
-[![Tests](https://img.shields.io/github/actions/workflow/status/TomographicImaging/eqt/test.yml?branch=main&label=Tests&logo=GitHub)](https://github.com/casperdcl/cdcl/actions)
-
-A number of templates and tools to develop Qt GUI's with Python effectively.
+[![Tests](https://img.shields.io/github/actions/workflow/status/TomographicImaging/eqt/test.yml?branch=main&label=Tests&logo=GitHub)](https://github.com/TomographicImaging/eqt/actions?query=branch%3Amain) [![PyPI](https://img.shields.io/pypi/v/eqt.svg?logo=pypi&logoColor=white)](https://pypi.org/project/eqt) [![Conda](https://img.shields.io/conda/v/conda-forge/eqt.svg?label=conda-forge&logo=conda-forge)](https://anaconda.org/conda-forge/eqt)
 
-Developing GUIs I often find myself creating forms to pass some input and also
-running some task asynchronously so that the interface is still responsive.
+Templates & tools to develop Qt GUIs in Python.
 
-This little package tries to address both recurring requirements.
+One use case is accepting user input while running another task asynchronously (so that the UI is still responsive).
 
-1. `UIFormWidget`, a class to help creating Qt forms
-   programmatically, useable in `QDockWidgets` and `QWidget`
-2. `FormDialog`, a `QDialog` with a form inside with OK and Cancel button
-3. `Worker`, a class that defines a `QRunnable` to
-   handle worker thread setup, signals and wrap up
+1. `UIFormWidget`: a class to help creating Qt forms programmatically, useable in `QDockWidgets` and `QWidget`
+2. `FormDialog`: a `QDialog` with a form inside with <kbd>OK</kbd> and <kbd>Cancel</kbd> buttons
+3. `Worker`: a class that defines a `QRunnable` to handle worker thread setup, signals and wrap up
 
 ## Installation
 
-You may install via `pip` or `conda`
+Via `pip`/`conda`/`mamba`, i.e. any of the following:
 
-```bash
-python -m pip install eqt
-# or
-conda install eqt -c paskino
-```
+- `python -m pip install eqt`
+- `conda install -c conda-forge eqt`
+- `mamba install -c conda-forge eqt`
 
 ## Examples
 
-In the `example` directory there is an example on how to launch a `QDialog` with a form inside using `eqt`'s [`QWidget`](examples/dialog_example.py) or [`FormDialog`](examples/dialog_example_2.py).
+See the [`examples`](examples) directory, e.g. how to launch a `QDialog` with a form inside using `eqt`'s [`QWidget`](examples/dialog_example.py) or [`FormDialog`](examples/dialog_example_2.py).
 
 ### Running asynchronous tasks
 
 To run a function in a separate thread we use a `Worker` which is a subclass of a `QRunnable`.
 
 For the `Worker` to work one needs to define:
 
@@ -126,8 +124,11 @@
 result = QtCore.Signal(object)
 
 progress = QtCore.Signal(int)
 message = QtCore.Signal(str)
 status = QtCore.Signal(tuple)
 ```
 
-Read more on [Qt signals and slots](https://doc.qt.io/qt-5/signalsandslots.html) and on how to use them in [pyside2](https://wiki.qt.io/Qt_for_Python_Signals_and_Slots).
+Read more on [Qt signals and slots](https://doc.qt.io/qt-5/signalsandslots.html) and on how to use them in [PySide2](https://wiki.qt.io/Qt_for_Python_Signals_and_Slots).
+
+## Developer Contribution Guide
+See [CONTRIBUTING.md](./CONTRIBUTING.md).
```

### Comparing `eqt-0.7.1/README.md` & `eqt-1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 # eqt: Qt Elements
 
-[![Tests](https://img.shields.io/github/actions/workflow/status/TomographicImaging/eqt/test.yml?branch=main&label=Tests&logo=GitHub)](https://github.com/casperdcl/cdcl/actions)
+[![Tests](https://img.shields.io/github/actions/workflow/status/TomographicImaging/eqt/test.yml?branch=main&label=Tests&logo=GitHub)](https://github.com/TomographicImaging/eqt/actions?query=branch%3Amain) [![PyPI](https://img.shields.io/pypi/v/eqt.svg?logo=pypi&logoColor=white)](https://pypi.org/project/eqt) [![Conda](https://img.shields.io/conda/v/conda-forge/eqt.svg?label=conda-forge&logo=conda-forge)](https://anaconda.org/conda-forge/eqt)
 
-A number of templates and tools to develop Qt GUI's with Python effectively.
+Templates & tools to develop Qt GUIs in Python.
 
-Developing GUIs I often find myself creating forms to pass some input and also
-running some task asynchronously so that the interface is still responsive.
+One use case is accepting user input while running another task asynchronously (so that the UI is still responsive).
 
-This little package tries to address both recurring requirements.
-
-1. `UIFormWidget`, a class to help creating Qt forms
-   programmatically, useable in `QDockWidgets` and `QWidget`
-2. `FormDialog`, a `QDialog` with a form inside with OK and Cancel button
-3. `Worker`, a class that defines a `QRunnable` to
-   handle worker thread setup, signals and wrap up
+1. `UIFormWidget`: a class to help creating Qt forms programmatically, useable in `QDockWidgets` and `QWidget`
+2. `FormDialog`: a `QDialog` with a form inside with <kbd>OK</kbd> and <kbd>Cancel</kbd> buttons
+3. `Worker`: a class that defines a `QRunnable` to handle worker thread setup, signals and wrap up
 
 ## Installation
 
-You may install via `pip` or `conda`
+Via `pip`/`conda`/`mamba`, i.e. any of the following:
 
-```bash
-python -m pip install eqt
-# or
-conda install eqt -c paskino
-```
+- `python -m pip install eqt`
+- `conda install -c conda-forge eqt`
+- `mamba install -c conda-forge eqt`
 
 ## Examples
 
-In the `example` directory there is an example on how to launch a `QDialog` with a form inside using `eqt`'s [`QWidget`](examples/dialog_example.py) or [`FormDialog`](examples/dialog_example_2.py).
+See the [`examples`](examples) directory, e.g. how to launch a `QDialog` with a form inside using `eqt`'s [`QWidget`](examples/dialog_example.py) or [`FormDialog`](examples/dialog_example_2.py).
 
 ### Running asynchronous tasks
 
 To run a function in a separate thread we use a `Worker` which is a subclass of a `QRunnable`.
 
 For the `Worker` to work one needs to define:
 
@@ -100,8 +93,11 @@
 result = QtCore.Signal(object)
 
 progress = QtCore.Signal(int)
 message = QtCore.Signal(str)
 status = QtCore.Signal(tuple)
 ```
 
-Read more on [Qt signals and slots](https://doc.qt.io/qt-5/signalsandslots.html) and on how to use them in [pyside2](https://wiki.qt.io/Qt_for_Python_Signals_and_Slots).
+Read more on [Qt signals and slots](https://doc.qt.io/qt-5/signalsandslots.html) and on how to use them in [PySide2](https://wiki.qt.io/Qt_for_Python_Signals_and_Slots).
+
+## Developer Contribution Guide
+See [CONTRIBUTING.md](./CONTRIBUTING.md).
```

### Comparing `eqt-0.7.1/eqt/io.py` & `eqt-1.0.0/eqt/io.py`

 * *Files identical despite different names*

### Comparing `eqt-0.7.1/eqt/threading/QtThreading.py` & `eqt-1.0.0/eqt/threading/QtThreading.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         -------
         - Error: An exception is thrown in the workers function.
         - Result: Contains the return value of a function that has just completed successfully.
         - Finished: Worker thread has completed.
         """
         try:
             result = self.fn(*self.args, **self.kwargs)
-        except BaseException:
+        except BaseException: # NOQA: B036
             traceback.print_exc()
             exctype, value = sys.exc_info()[:2]
             self.signals.error.emit((exctype, value, traceback.format_exc()))
         else:
             self.signals.result.emit(result)
         finally:
             self.signals.finished.emit()
```

### Comparing `eqt-0.7.1/eqt/ui/MainWindowWithProgressDialogs.py` & `eqt-1.0.0/eqt/ui/MainWindowWithProgressDialogs.py`

 * *Files identical despite different names*

### Comparing `eqt-0.7.1/eqt/ui/MainWindowWithSessionManagement.py` & `eqt-1.0.0/eqt/ui/MainWindowWithSessionManagement.py`

 * *Files 0% similar despite different names*

```diff
@@ -495,15 +495,15 @@
         '''
         process_name = 'Save Session'
 
         self.process_finished = False
         self.createUnknownProgressWindow(process_name, "Saving", "Saving Session")
 
         saveSession_worker = Worker(self.saveSession, session_name, compress)
-        if type(event) == QCloseEvent:
+        if isinstance(event, QCloseEvent):
             saveSession_worker.signals.finished.connect(
                 lambda: self.removeTempAndClose(process_name))
         else:
             saveSession_worker.signals.finished.connect(lambda: self.closeSaveWindow(process_name))
         self.threadpool.start(saveSession_worker)
 
     def saveSession(self, session_name, compress, **kwargs):
```

### Comparing `eqt-0.7.1/eqt/ui/ProgressTimerDialog.py` & `eqt-1.0.0/eqt/ui/ProgressTimerDialog.py`

 * *Files identical despite different names*

### Comparing `eqt-0.7.1/eqt/ui/ReOrderableListWidget.py` & `eqt-1.0.0/eqt/ui/ReOrderableListWidget.py`

 * *Files identical despite different names*

### Comparing `eqt-0.7.1/eqt/ui/SessionDialogs.py` & `eqt-1.0.0/eqt/ui/SessionDialogs.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,16 +65,21 @@
             The selected directory, to be used as the directory in which all sessions are saved.
         '''
         FormDialog.__init__(self, parent, "Select Session Directory")
         self.parent = parent
 
         self.app_name = app_name
 
+        if app_name is not None:
+            app_name_label = ' ' + app_name
+        else:
+            app_name_label = ''
+
         label_text = ("Select a session directory to save and retrieve all"
-                      f" {app_name or ''} Sessions:")
+                      f"{app_name_label} Sessions:")
 
         self.addSpanningWidget(QLabel(label_text), 'select_session_directory')
 
         browse_button = QPushButton('Browse')
         browse_button.clicked.connect(self.browse_for_dir)
         self.addWidget(browse_button, QLabel('No directory selected'), 'selected_dir')
```

### Comparing `eqt-0.7.1/eqt/ui/UIFormWidget.py` & `eqt-1.0.0/eqt/ui/FormDialog.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,434 +1,443 @@
 from PySide2 import QtWidgets
 
-from .UISliderWidget import UISliderWidget
+from . import UIFormFactory
 
 
-class UIFormWidget:
-    '''
-             QWidget or QDockWidget
-    +----------------------------------------------------------+
-    |        QVBoxLayout                                       |
-    |   +---------------------------------------------------+  |
-    |   |    QGroupBox                                      |  |
-    |   |                                                   |  |
-    |   |    +------------------------------------------+   |  |
-    |   |    |   QFormLayout                            |   |  |
-    |   |    |                                          |   |  |
-    |   |    |                                          |   |  |
-    |   |    +------------------------------------------+   |  |
-    |   |                                                   |  |
-    |   +---------------------------------------------------+  |
-    |                                                          |
-    +----------------------------------------------------------+
-    '''
-    def createForm(self):
-        # Add vertical layout to dock contents
-        verticalLayout = QtWidgets.QVBoxLayout(self)
-        verticalLayout.setContentsMargins(10, 10, 10, 10)
-
-        # Add vertical layout to main widget (self)
-        # verticalLayout.addWidget(self)
-        self.setLayout(verticalLayout)
-
-        # Add group box
-        groupBox = QtWidgets.QGroupBox(self)
-
-        # Add form layout to group box
-        groupBoxFormLayout = QtWidgets.QFormLayout(groupBox)
-
-        # Add elements to layout
-        verticalLayout.addWidget(groupBox)
-
-        self.num_widgets = 0
-        self.uiElements = {
-            'verticalLayout': verticalLayout, 'groupBox': groupBox,
-            'groupBoxFormLayout': groupBoxFormLayout}
-        self.widgets = {}
+class FormDialog(QtWidgets.QDialog):
+    def __init__(self, parent=None, title=None):
+        super().__init__(parent)
 
-    @property
-    def groupBox(self):
-        return self.uiElements['groupBox']
+        self.buttonBox = QtWidgets.QDialogButtonBox(QtWidgets.QDialogButtonBox.Ok
+                                                    | QtWidgets.QDialogButtonBox.Cancel)
+        self.formWidget = UIFormFactory.getQWidget(parent=self)
+        # set the layout of the dialog
+        self.setLayout(self.formWidget.uiElements['verticalLayout'])
 
-    def addSpanningWidget(self, qwidget, name):
-        self._addWidget(name, qwidget)
+        if title is not None:
+            self.setWindowTitle(title)
+        # add button box to the UI
+        self.formWidget.uiElements['verticalLayout'].addWidget(self.buttonBox)
+        self.buttonBox.button(QtWidgets.QDialogButtonBox.Ok).clicked.connect(self._onOk)
+        self.buttonBox.button(QtWidgets.QDialogButtonBox.Cancel).clicked.connect(self._onCancel)
 
-    def addWidget(self, qwidget, qlabel, name):
-        self._addWidget(name, qwidget, qlabel)
+    @property
+    def Ok(self):
+        '''Returns a reference to the Dialog Ok button to connect its signals.'''
+        return self.buttonBox.button(QtWidgets.QDialogButtonBox.Ok)
 
-    def getWidget(self, name, role='field'):
-        '''returns the Widget by the name with which it has been added
+    @property
+    def Cancel(self):
+        '''Returns a reference to the Dialog Cancel button to connect its signals.'''
+        return self.buttonBox.button(QtWidgets.QDialogButtonBox.Cancel)
+
+    def _onOk(self):
+        '''Saves the widget states and calls `onOk`.'''
+        self.saveAllWidgetStates()
+        self.onOk()
+        self.close()
+
+    def _onCancel(self):
+        '''Calls `onCancel`, closes the FormDialog and restores the previously saved states
+        or the default states.'''
+        self.onCancel()
+        self.close()
+        self.restoreAllSavedWidgetStates()
+
+    def onOk(self):
+        '''Called when the dialog's "Ok" button is clicked.
+        Can be redefined to add additional functionality on "Ok".'''
+        pass
+
+    def onCancel(self):
+        '''Called when the dialog's "Cancel" button is clicked.
+        Can be redefined to add additional functionality on "Cancel"'''
+        pass
 
-        By default it returns the widget that is the field in the form.
-        The user can get the label by specifying the role to be label
+    @property
+    def widgets(self):
+        return self.formWidget.widgets
 
-        Raises ValueError if the role is not field or label.
-        '''
-        allowed_roles = 'field', 'label'
-        if role in allowed_roles:
-            return self.widgets[f'{name}_{role}']
-        raise ValueError(f'Unexpected role: expected any of {allowed_roles}, got {role}')
+    @property
+    def groupBox(self):
+        return self.formWidget.groupBox
 
-    def setWidgetVisible(self, name, visible):
+    def addWidget(self, qwidget, qlabel=None, name=None, layout='form'):
         '''
-        Sets the visibility of the widget and associated label with the given name.
+        Adds a widget to the layout. In particular, adds a qwidget and a qlabel widget
+        in the same row of the form layout if layout is 'form' and adds a spanning widget
+        to the vertical layout if layout is 'vertical'.
 
         Parameters
         ----------
-        name: str
-            The name of the widget to set visible/invisible
-        visible: bool
-            True to set the widget visible, False to hide it
-        '''
-        allowed_roles = ['field', 'label']
-        for role in allowed_roles:
-            try:
-                self.getWidget(name, role).setVisible(visible)
-            except Exception:
-                # We may not have a label for the widget
-                pass
-
-    def getWidgets(self):
-        '''returns a dictionary of all the widgets in the form'''
-        return self.widgets
-
-    def addTitle(self, qlabel, name):
-        if isinstance(qlabel, str):
-            txt = qlabel
-            qlabel = QtWidgets.QLabel(self.uiElements['groupBox'])
-            qlabel.setText(txt)
-        qlabel.setStyleSheet("font-weight: bold")
-        self._addWidget(name, qlabel)
-
-    def addSeparator(self, name):
-        # Adds horizontal separator to the form
-        frame = QtWidgets.QFrame()
-        frame.setFrameShape(QtWidgets.QFrame.HLine)
-        frame.setFrameShadow(QtWidgets.QFrame.Raised)
-        self._addWidget(name, frame)
-
-    def _addWidget(self, name, qwidget, qlabel=None):
-        formLayout = self.uiElements['groupBoxFormLayout']
-
-        # Create the widgets:
-
-        widgetno = self.num_widgets
-
-        # add the field
-        field = f'{name}_field'
-        self.widgets[field] = qwidget
-
-        if qlabel is not None:
-            # add the label
-            label = f'{name}_label'
-            if isinstance(qlabel, str):
-                txt = qlabel
-                qlabel = QtWidgets.QLabel(self.uiElements['groupBox'])
-                qlabel.setText(txt)
-            formLayout.setWidget(widgetno, QtWidgets.QFormLayout.LabelRole, qlabel)
-
-            # save a reference to label widgets in the dictionary
-            self.widgets[label] = qlabel
-
-            field_form_role = QtWidgets.QFormLayout.FieldRole
-
+        qwidget : QWidget
+        qlabel : qlabel widget or str
+            only supported when layout is 'form'
+        name : str
+            only supported when layout is 'form'
+        layout : 'form' or 'vertical'
+                'form' - adds to the `groupBoxFormLayout`,
+                'vertical' - adds to the `verticalLayout` below the form.
+        '''
+        if layout == 'vertical':
+            if name is not None or qlabel is not None:
+                raise ValueError('`qlabel` and `name` are unsupported when `layout=vertical`')
+            self.formWidget.uiElements['verticalLayout'].addWidget(qwidget)
+        elif layout == 'form':
+            if name is None:
+                raise ValueError('To add the widget to the form, please set name.')
+            if qlabel is None:
+                raise ValueError('To add the widget to the form, please set label.')
+            self.formWidget.addWidget(qwidget, qlabel, name)
         else:
-            # In the case we don't have a qlabel, set a spanning widget:
-            field_form_role = QtWidgets.QFormLayout.SpanningRole
+            raise ValueError(f"layout '{layout}' unrecognised: expected 'form' or 'vertical'")
 
-        formLayout.setWidget(widgetno, field_form_role, qwidget)
-        self.num_widgets += 1
-
-    def getAllWidgetStates(self):
+    def addSpanningWidget(self, qwidget, name=None, layout='form'):
         '''
-        Returns
-        -------
-        dict
-          Format: {'widget_name': {'value': str | bool | int, 'enabled': bool, 'visible': bool},
-                   ...},
-          e.g. {{'widget1': {'value': 1, 'enabled': True, 'visible': True},
-                 'widget2': {'value': 2, 'enabled': False, 'visible': False}}.
-        '''
-        all_widget_states = {}
-        for name, widget in self.widgets.items():
-            widget_state = self.getWidgetState(widget)
-            all_widget_states[name] = widget_state
-        return all_widget_states
+        Adds a spanning widget occupying the full row in the layout.
 
-    def getWidgetState(self, widget, role=None):
-        '''
         Parameters
         ----------
-        widget: QWidget or str
-            The (name of) widget to get the state of.
-        role: str, optional, default None, values: 'label', 'field', None.
-            The role of the widget to apply the state to (only if `widget` is a `str`).
-            If unspecified, the widget is chosen based on `name=widget`.
+        qwidget : QWidget
+        name : str
+            only supported when layout is 'form'
+        layout : 'form' or 'vertical'
+                'form' - adds to the `groupBoxFormLayout`,
+                'vertical' - adds to the `verticalLayout` below the form.
+        '''
+        if layout == 'vertical':
+            if name is not None:
+                raise ValueError(f"`name='{name}'` cannot be given if `layout='{layout}'`")
+            self.formWidget.uiElements['verticalLayout'].addWidget(qwidget)
+        elif layout == 'form':
+            if name is None:
+                raise ValueError('To add the widget to the form, please set name')
+            self.formWidget.addSpanningWidget(qwidget, name)
+        else:
+            raise ValueError(
+                f"layout {layout} is not recognised, must be set to 'form' or 'vertical'")
 
-        Returns
-        -------
-        state: dict
-            Format: {'value': str | bool | int, 'enabled': bool, 'visible': bool},
-            e.g. {'value': 1, 'enabled': True, 'visible': True}.
-            This can be used to restore the state of the widget using `setWidgetState()`.
+    def insertWidget(self, row, name, qwidget, qlabel=None):
         '''
-        if widget is None:
-            raise ValueError('The widget (or name of widget) must be given')
-
-        if isinstance(widget, str):
-            if role is not None:
-                if role not in ['label', 'field']:
-                    raise ValueError('role must be either "label", "field" or None')
-                name = widget + '_' + role
-            else:
-                name = widget
-
-            try:
-                widget = self.widgets[name]
-            except KeyError:
-                if role is None:
-                    try:
-                        widget = self.widgets[name + '_field']
-                    except KeyError:
-                        raise KeyError('No widget with name: ' + name + ' or ' + name + '_field')
-                else:
-                    raise KeyError('No widget with name: ' + name)
-
-        widget_state = {}
-        widget_state['enabled'] = widget.isEnabled()
-        widget_state['visible'] = widget.isVisible()
-
-        if isinstance(widget, QtWidgets.QLabel):
-            widget_state['value'] = widget.text()
-        elif isinstance(widget, (QtWidgets.QCheckBox, QtWidgets.QPushButton)):
-            widget_state['value'] = widget.isChecked()
-        elif isinstance(widget, QtWidgets.QComboBox):
-            widget_state['value'] = widget.currentIndex()
-        elif isinstance(widget, UISliderWidget) or isinstance(widget, QtWidgets.QSlider):
-            widget_state['value'] = widget.value()
-        elif isinstance(widget, (QtWidgets.QDoubleSpinBox, QtWidgets.QSpinBox)):
-            widget_state['value'] = widget.value()
-        elif isinstance(widget, QtWidgets.QLineEdit):
-            widget_state['value'] = widget.text()
-        elif isinstance(widget, QtWidgets.QRadioButton):
-            widget_state['value'] = widget.isChecked()
-        elif isinstance(widget, (QtWidgets.QTextEdit, QtWidgets.QPlainTextEdit)):
-            widget_state['value'] = widget.toPlainText()
+        Inserts a labelled widget, or a spanning widget, to the form layout.
+        The position in the form is specified by row. If row is out of bounds, the widget
+        is added at the end of the form. An error is raised if `name` is already in use
+        by another widget in the form. The entries associated with the widget are added
+        to the widget dictionary and the default-widget-states
+        dictionary.
 
-        return widget_state
+        Parameters
+        ----------
+        row : int
+            The position in the form where the widget is added.
+        name : str
+            The string associated to the qwidget and qlabel.
+        qwidget : QWidget
+            The widget to be added on the right hand side of the form or as a spanning widget.
+        qlabel : qlabel widget or str
+            The qlabel widget, or a str from which a qlabel widget is created, to be added
+            on the left hand side of the form. If qlabel is `None` the widget spans the full
+            width of the form.
+        '''
+        self.formWidget.insertWidget(row, name, qwidget, qlabel)
+
+    def insertWidgetToVerticalLayout(self, row, qwidget):
+        '''Inserts a widget to the vertical layout at position specified by row.'''
+        self.formWidget.uiElements['verticalLayout'].insertWidget(row, qwidget)
+
+    def getWidgetFromVerticalLayout(self, index):
+        '''Returns the widget in the vertical layout located at position index.'''
+        return self.formWidget.uiElements['verticalLayout'].itemAt(index).widget()
 
-    def applyWidgetState(self, name, state, role=None):
+    def getIndexFromVerticalLayout(self, widget):
         '''
-        Applies the given `state` to the widget with the given `name`.
+        Returns the index of the widget in the vertical layout.
 
         Parameters
-        ----------
-        name: str
-            The name of the widget to apply the state to.
-        role: str, optional, default None, values: 'label', 'field', None.
-            The role of the widget to apply the state to (only if `widget` is a `str`).
-            If unspecified, the widget is chosen based on `name`.
-        state: dict
-            Format: {'value': str | bool | int, 'enabled': bool, 'visible': bool},
-            e.g. {'value': 1, 'enabled': True, 'visible': True}.
-        '''
-        if role is not None:
-            if role not in ['label', 'field']:
-                raise ValueError('role must be either "label", "field" or None')
-            name = name + '_' + role
-
-        try:
-            widget = self.widgets[name]
-        except KeyError:
-            if role is None:
-                try:
-                    widget = self.widgets[name + '_field']
-                except KeyError:
-                    raise KeyError('No widget with name: ' + name + ' or ' + name + '_field')
-            else:
-                raise KeyError('No widget with name: ' + name)
-
-        for key, value in state.items():
-            if key == 'enabled':
-                widget.setEnabled(value)
-            elif key == 'visible':
-                widget.setVisible(value)
-            elif key == 'value':
-                if isinstance(widget, QtWidgets.QLabel):
-                    widget.setText(value)
-                elif isinstance(widget, QtWidgets.QCheckBox):
-                    widget.setChecked(value)
-                elif isinstance(widget, QtWidgets.QComboBox):
-                    widget.setCurrentIndex(value)
-                elif isinstance(widget, (UISliderWidget, QtWidgets.QSlider)):
-                    widget.setValue(value)
-                elif isinstance(widget, (QtWidgets.QDoubleSpinBox, QtWidgets.QSpinBox)):
-                    widget.setValue(value)
-                elif isinstance(widget, QtWidgets.QPushButton):
-                    widget.setChecked(value)
-                elif isinstance(widget, QtWidgets.QLineEdit):
-                    widget.setText(value)
-                elif isinstance(widget, QtWidgets.QRadioButton):
-                    widget.setChecked(value)
-                elif isinstance(widget, (QtWidgets.QTextEdit, QtWidgets.QPlainTextEdit)):
-                    widget.setPlainText(value)
-
-    def applyWidgetStates(self, state):
-        '''
-        Applies the given states to the form's widgets.
+        -------------
+        widget : QWidget
+            The widget in the layout.
+
+        Return
+        ------------
+        int
+            The index of the widget in the layout.
+        '''
+        return self.formWidget.uiElements['verticalLayout'].indexOf(widget)
+
+    def removeWidget(self, name):
+        '''
+        Removes the widget with the specified name from the form layout.
+        This method deletes the qwidget, and qlabel if present, from the widgets dictionary
+        and sets their parent to `None`.
 
         Parameters
         ----------
-        state: dict
-          Format: {'widget_name': {'value': str | bool | int, 'enabled': bool, 'visible': bool},
-                   ...},
-          e.g. {{'widget1': {'value': 1, 'enabled': True, 'visible': True},
-                 'widget2': {'value': 2, 'enabled': False, 'visible': False}}.
-        '''
-        for name, widget_state in state.items():
-            self.applyWidgetState(name, widget_state)
+        name : str
+            The name of the widget to be removed.
 
-    def saveAllWidgetStates(self):
-        '''
-        Saves the state of all widgets in the form.
-        To later restore the states, use `restoreAllSavedWidgetStates()`.
-        '''
-        self.widget_states = self.getAllWidgetStates()
-
-    def restoreAllSavedWidgetStates(self):
-        '''
-        Restore all widgets in the form to the state saved by `saveAllWidgetStates()`.
-        If `saveAllWidgetStates()` method was not previously invoked, do nothing.
+        Returns
+        -------
+        tuple or QWidget
+            If the widget has a corresponding label, a tuple containing the widget
+            and label is returned. Otherwise, only the widget is returned.
         '''
-        if hasattr(self, 'widget_states'):
-            self.applyWidgetStates(self.widget_states)
-
-
-class FormWidget(QtWidgets.QWidget, UIFormWidget):
-    def __init__(self, parent=None):
-        # dockWidgetContents = QtWidgets.QWidget()
-
-        QtWidgets.QWidget.__init__(self, parent)
-        self.createForm()
+        return self.formWidget.removeWidget(name)
 
+    def removeWidgetFromVerticalLayout(self, widget):
+        '''Removes a widget from the vertical layout.
 
-class FormDockWidget(QtWidgets.QDockWidget):
-    def __init__(self, parent=None, title=None):
-        QtWidgets.QDockWidget.__init__(self, parent)
-        widget = FormWidget(parent)
-        self.setWidget(widget)
-        if title is not None:
-            self.setObjectName(title)
-
-    def addWidget(self, qwidget, qlabel, name):
-        self.widget().addWidget(qwidget, qlabel, name)
+        Parameters
+        ----------
+        widget : QWidget
+            The widget to be removed.
+        '''
+        self.formWidget.uiElements['verticalLayout'].removeWidget(widget)
+        widget.setParent(None)
+        return widget
+
+    def getNumWidgets(self):
+        '''Returns the number of widgets in the form.'''
+        return self.formWidget.getNumWidgets()
 
     def getWidget(self, name, role='field'):
-        '''returns the Widget by the name with which it has been added
-
+        '''
+        Returns the widget by the name with which it has been added.
         By default it returns the widget that is the field in the form.
-        The user can get the label by specifying the role to be label
-
+        The user can get the label by specifying the role to be label.
         Raises ValueError if the role is not field or label.
         '''
-        return self.widget().getWidget(name, role)
+        return self.formWidget.getWidget(name, role)
 
     def getWidgets(self):
-        '''returns a dictionary of all the widgets in the form'''
-        return self.widget().getWidgets()
+        '''Returns a dictionary of the widgets currently present in the form.'''
+        return self.formWidget.getWidgets()
+
+    def getWidgetRow(self, name, role='field'):
+        '''
+        Returns the widget row in the form layout by the widget name.
+        This is the row of the widget in the form layout.
+        '''
+        return self.formWidget.getWidgetRow(name, role)
 
     def setWidgetVisible(self, name, visible):
-        '''Sets the visibility of the widget and associated label with the given name.'''
-        self.widget().setWidgetVisible(name, visible)
+        '''
+        Sets the visibility of the widget and associated label with the given name.
+
+        Parameters
+        ----------
+        name : str
+            The name of the widget to set visible/invisible
+        visible : bool
+            True to set the widget visible, False to hide it
+        '''
+        self.formWidget.setWidgetVisible(name, visible)
 
     def saveAllWidgetStates(self):
         '''
-        Saves the state of all widgets in the form.
+        Saves the state of all widgets currently present in the form.
         To later restore the states, use `restoreAllSavedWidgetStates()`.
         '''
-        self.widget().saveAllWidgetStates()
+        self.formWidget.saveAllWidgetStates()
+
+    def getWidgetStates(self):
+        '''Deprecated. Use `getSavedWidgetStates`.'''
+        return self.formWidget.getWidgetStates()
+
+    def getSavedWidgetStates(self):
+        '''Returns the saved widget states.'''
+        return self.formWidget.getSavedWidgetStates()
+
+    def getDefaultWidgetStates(self):
+        '''Returns the saved default widget states.'''
+        return self.formWidget.getDefaultWidgetStates()
 
     def restoreAllSavedWidgetStates(self):
         '''
         Restore all widgets in the form to the state saved by `saveAllWidgetStates()`.
         If `saveAllWidgetStates()` method was not previously invoked, do nothing.
         '''
-        self.widget().restoreAllSavedWidgetStates()
+        self.formWidget.restoreAllSavedWidgetStates()
 
     def getAllWidgetStates(self):
         '''
         Returns
         -------
-        states: dict
-          Format: {'widget_name': {'value': str | bool | int, 'enabled': bool, 'visible': bool},
-                   ...},
-          e.g. {{'widget1': {'value': 1, 'enabled': True, 'visible': True},
-                 'widget2': {'value': 2, 'enabled': False, 'visible': False}}.
+        dict
+            Format: {'widget_name': {'value': str | bool | int, 'enabled': bool, 'visible': bool,
+            'widget_row': int}, ...}.
+            e.g. {'widget1': {'value': 1, 'enabled': True, 'visible': True, 'widget_row': 0},
+            'widget2': {'value': 2, 'enabled': False, 'visible': False, 'widget_row': 1}}.
         '''
-        return self.widget().getAllWidgetStates()
+        return self.formWidget.getAllWidgetStates()
 
     def getWidgetState(self, widget, role=None):
         '''
+        Returns the current state of the widget in the form.
+
         Parameters
         ----------
-        widget: QWidget or str
-            The (name of) widget to get the state of.
-        role: str, optional, default None, values: 'label', 'field', None.
-            The role of the widget to get the state of (only if `widget` is a `str`).
-            If unspecified, the widget is chosen based on `name=widget`.
+        widget : QWidget or str
+            The widget or its name (or its name + '_field' or '_label', when role is None) to get
+            the state of.
+        role : str, optional, default None, values: 'label', 'field', None.
+            The role of the widget to apply the state to. This is used only if `widget` is the
+            widget name string.
 
         Returns
         -------
-        dict
-            Widget state, format: {'value': str | bool | int, 'enabled': bool, 'visible': bool},
-            e.g. {'value': 1, 'enabled': True, 'visible': True}.
+        state : dict
+            Format: {'value': str | bool | int, 'enabled': bool, 'visible': bool,
+            'widget_row' : int}.
+            e.g. {'value': 1, 'enabled': True, 'visible': True, 'widget_row' : 0}.
             This can be used to restore the state of the widget using `setWidgetState()`.
         '''
-        return self.widget().getWidgetState(widget, role)
+        return self.formWidget.getWidgetState(widget, role)
 
     def applyWidgetState(self, name, state, role=None):
         '''
-        Applies the given state to the widget with the given name.
+        Applies the given `state` to the widget associated with `name` and `role`.
+        If role is None, the role is assigned to be 'field'.
 
         Parameters
         ----------
-        name: str
+        name : str
             The name of the widget to apply the state to.
-        role: str, optional, default None, values: 'label', 'field', None.
+        role : str, optional, default None, values: 'label', 'field', None.
             The role of the widget to apply the state to.
-            If unspecified, the widget is chosen based on `name`.
-        state: dict
-            Format: {'value': str | bool | int, 'enabled': bool, 'visible': bool},
-            e.g. {'value': 1, 'enabled': True, 'visible': True}.
-        '''
-        return self.widget().applyWidgetState(name, state, role)
+        state : dict
+            Format: {'value': str | bool | int, 'enabled': bool, 'visible': bool,
+            'widget_row' : int}.
+            e.g. {'value': 1, 'enabled': True, 'visible': True, 'widget_row' : 0}.
+        '''
+        return self.formWidget.applyWidgetState(name, state, role)
+
+    def applyWidgetStates(self, states):
+        '''
+        Applies the given states to the form's widgets. It raises an error if the keys in the
+        dicitonary of states and the keys in the dictionary of widgets in the form are not the
+        same.
 
-    def applyWidgetStates(self, state):
-        '''
-        Applies the given states to the form's widgets.
+        Parameters
+        ----------
+        states : dict
+            Format: {'name_field': {'value': str | bool | int, 'enabled': bool, 'visible': bool,
+            'widget_row' : int}, 'name_label': {'value': str | bool | int, 'enabled': bool,
+            'visible': bool, 'widget_row' : int}, ...}.
+            e.g. {'widget1': {'value': 1, 'enabled': True, 'visible': True, 'widget_row': 0},
+                  'widget2': {'value': 2, 'enabled': False, 'visible': False, 'widget_row': 1}}.
+        '''
+        return self.formWidget.applyWidgetStates(states)
+
+
+class AdvancedFormDialog(FormDialog):
+    def __init__(self, parent=None, title=None, parent_button_name=None):
+        """
+        Constructs an advanced form dialog that adds widgets on its parent.
+
+        To add widgets to the parent, call `displayWidgetValueOnParent` after creating an instance
+        of the class. The advanced form dialog has a default button in its vertical layout, which
+        is located between the form layout and the buttons 'ok' and 'cancel'. This button sets the
+        widgets to their default values.
 
         Parameters
         ----------
-        state: dict
-          Format: {'widget_name': {'value': str | bool | int, 'enabled': bool, 'visible': bool},
-                   ...},
-          e.g. {{'widget1': {'value': 1, 'enabled': True, 'visible': True},
-                 'widget2': {'value': 2, 'enabled': False, 'visible': False}}.
-        '''
-        return self.widget().applyWidgetStates(state)
+        parent : UIFormWidget or None, optional
+            The parent widget of the advanced form dialog.
+            If None, the dialog is created without a parent.
+        title : str or None, optional
+            The title of the advanced form dialog.
+        parent_button_name : str or None, optional
+            The name of the button opening the advanced form dialog in the parent.
+            If passed, the extra widgets will be added under this button in the parent,
+            otherwise they are added at the end.
+        """
+        self.dialog_parent = parent
+        self.display_on_parent = []
+        if parent_button_name is None:
+            self.parent_button_row = -1
+        elif parent is None:
+            raise ValueError(
+                'The parent is None. Set the parent if you want to set the parent button name.')
+        else:
+            self.parent_button_row = self.dialog_parent.getWidgetRow(parent_button_name)
 
+        FormDialog.__init__(self, parent, title)
 
-class UIFormFactory(QtWidgets.QWidget):
-    # def generateUIFormView(QtWidgets.QWidget):
-    '''creates a widget with a form layout group to add things to
+        # add default button to vertical layout
+        self.default_button = QtWidgets.QPushButton("Set default values")
+        self.insertWidgetToVerticalLayout(1, self.default_button)
+        self.default_button.clicked.connect(lambda: self._setDefaultValues())
+
+    def _onOk(self):
+        """
+        Called when the "Ok" button is clicked in the advanced dialog.
+
+        Calls the super-class method `_onOk`, sets the default widgets
+        to visible, and adds/updates/removes widgets from the
+        parent depending on the the widgets in the advanced dialog.
+        """
+        super()._onOk()
+        self.formWidget.setDefaultWidgetStatesVisibleTrue()
+        if self.display_on_parent:
+            if self.getSavedWidgetStates() == self.getDefaultWidgetStates():
+                self._removeWidgetsFromParent()
+            else:
+                self._addOrUpdateWidgetsInParent()
+
+    def _addOrUpdateWidgetsInParent(self):
+        """
+        Adds or updates widgets in the parent form.
+
+        This method iterates over the display_on_parent and adds the widgets to the parent
+        form. If a widget already exists in the parent form, it is updated with the most current
+        value set in the advanced dialog.
+        """
+        for index, name in enumerate(self.display_on_parent, start=1):
+            widget_row = self.parent_button_row + index if self.parent_button_row != -1 else -1
+            value = self.getSavedWidgetStates()[f'{name}_field']['value']
+            qwidget = self.getWidget(name, 'field')
+            if isinstance(qwidget, QtWidgets.QComboBox):
+                value = qwidget.itemText(value)
+            if f'{name}_field' not in self.dialog_parent.getWidgets():
+                label = str(self.getSavedWidgetStates()[f'{name}_label']['value'])
+                self.dialog_parent.insertWidget(widget_row, name, QtWidgets.QLabel(str(value)),
+                                                label)
+            else:
+                self.dialog_parent.getWidget(name, 'field').setText(str(value))
 
-    basically you can add widget to the returned groupBoxFormLayout and paramsGroupBox
-    The returned dockWidget must be added with
-    main_window.addDockWidget(QtCore.Qt.RightDockWidgetArea, dockWidget)
-    '''
-    @staticmethod
-    def getQDockWidget(parent=None, title=None):
-        return FormDockWidget(parent, title)
+    def _removeWidgetsFromParent(self):
+        """
+        Removes widgets from the parent form.
+
+        This method iterates over the display_on_parent and removes
+        the widgets from the parent.
+        """
+        for name in self.display_on_parent:
+            if f'{name}_field' in self.dialog_parent.getWidgets():
+                self.dialog_parent.removeWidget(name)
+
+    def _setDefaultValues(self):
+        """
+        Sets the widgets in the advanced dialog to their default states.
+
+        Makes the default widget states visible, as often the default states are saved while the
+        widgets are not visible. Applies the widget states to the widgets in the form.
+        """
+        self.formWidget.setDefaultWidgetStatesVisibleTrue()
+        self.applyWidgetStates(self.formWidget.default_widget_states)
+
+    def displayWidgetValueOnParent(self, name):
+        """
+        Adds `name` in a list. The order in which names are added to this
+        list reflects the order in which the widgets are added to the parent.
+        Raises an error if the parent of the advanced dialog is `None`.
 
-    @staticmethod
-    def getQWidget(parent=None):
-        return FormWidget(parent)
+        Parameters
+        ----------
+        name : str
+            The name of the widget in the advanced dialog to be displayed in the parent.
+        """
+        if self.dialog_parent is None:
+            raise KeyError('''The advanced-dialog parent is None.
+                           Set the parent if you want to add widgets to it.''')
+        self.display_on_parent.append(name)
```

### Comparing `eqt-0.7.1/eqt/ui/UIMultiStepWidget.py` & `eqt-1.0.0/eqt/ui/UIMultiStepWidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,33 +47,26 @@
 
         self.current_step = -1
 
         self.uiElements = {'verticalLayout': verticalLayout, 'buttonGroupBox': horizontalGroupBox}
         self.widgets = {}
 
     def updateStep(self, go_to="next"):
-        steps = list(self.widgets.keys())
+        steps = list(self.widgets)
         step_widgets = list(self.widgets.values())
         current_step_index = steps.index(self.current_step)
 
         if go_to == 'next':
             self.prev_button.setEnabled(True)
             next_index = current_step_index + 1
-            if next_index == len(steps) - 1:
-                self.next_button.setEnabled(False)
-            else:
-                self.next_button.setEnabled(True)
-
-        if go_to == 'prev':
+            self.next_button.setEnabled(next_index == len(steps) - 1)
+        elif go_to == 'prev':
             self.next_button.setEnabled(True)
             next_index = current_step_index - 1
-            if next_index == 0:
-                self.prev_button.setEnabled(False)
-            else:
-                self.prev_button.setEnabled(True)
+            self.prev_button.setEnabled(next_index == 0)
 
         self.current_step = steps[next_index]
 
         widgets_to_show = step_widgets.pop(next_index)
         widgets_to_hide = step_widgets
         self.showHideWidgets(widgets_to_hide, show=False)
         self.showHideWidgets(widgets_to_show, show=True)
@@ -88,15 +81,15 @@
         self.uiElements['verticalLayout'].insertWidget(0, qwidget)
 
     def addStepWidgets(self, qwidgets, name):
         for qwidget in qwidgets:
             self.addStepWidget(qwidget, name)
 
     def showHideWidgets(self, widgets, show=True):
-        if type(widgets) != list:
+        if not isinstance(widgets, (list, tuple)):
             widgets = [widgets]
         for widget in widgets:
             widget.setVisible(show)
 
 
 class MultiStepWidget(QtWidgets.QWidget, UIMultiStepWidget):
     def __init__(self, parent=None):
```

### Comparing `eqt-0.7.1/eqt/ui/UISliderWidget.py` & `eqt-1.0.0/eqt/ui/UISliderWidget.py`

 * *Files identical despite different names*

### Comparing `eqt-0.7.1/eqt/ui/UIStackedWidget.py` & `eqt-1.0.0/eqt/ui/UIStackedWidget.py`

 * *Files identical despite different names*

### Comparing `eqt-0.7.1/eqt.egg-info/PKG-INFO` & `eqt-1.0.0/eqt.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eqt
-Version: 0.7.1
+Version: 1.0.0
 Summary: A number of templates and tools to develop Qt GUIs with Python effectively
 Author-email: Edoardo Pasca <edoardo.pasca@stfc.ac.uk>, Laura Murgatroyd <laura.murgatroyd@stfc.ac.uk>
 Maintainer-email: Casper da Costa-Luis <casper.dcl@physics.org>
 License: Apache-2.0
 Project-URL: documentation, https://github.com/TomographicImaging/eqt#readme
 Project-URL: repository, https://github.com/TomographicImaging/eqt
 Project-URL: changelog, https://github.com/TomographicImaging/eqt/releases
@@ -17,47 +17,45 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: pyside2
+Requires-Dist: qdarkstyle
+Provides-Extra: dev
+Requires-Dist: pytest>=6; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-timeout; extra == "dev"
 
 # eqt: Qt Elements
 
-[![Tests](https://img.shields.io/github/actions/workflow/status/TomographicImaging/eqt/test.yml?branch=main&label=Tests&logo=GitHub)](https://github.com/casperdcl/cdcl/actions)
-
-A number of templates and tools to develop Qt GUI's with Python effectively.
+[![Tests](https://img.shields.io/github/actions/workflow/status/TomographicImaging/eqt/test.yml?branch=main&label=Tests&logo=GitHub)](https://github.com/TomographicImaging/eqt/actions?query=branch%3Amain) [![PyPI](https://img.shields.io/pypi/v/eqt.svg?logo=pypi&logoColor=white)](https://pypi.org/project/eqt) [![Conda](https://img.shields.io/conda/v/conda-forge/eqt.svg?label=conda-forge&logo=conda-forge)](https://anaconda.org/conda-forge/eqt)
 
-Developing GUIs I often find myself creating forms to pass some input and also
-running some task asynchronously so that the interface is still responsive.
+Templates & tools to develop Qt GUIs in Python.
 
-This little package tries to address both recurring requirements.
+One use case is accepting user input while running another task asynchronously (so that the UI is still responsive).
 
-1. `UIFormWidget`, a class to help creating Qt forms
-   programmatically, useable in `QDockWidgets` and `QWidget`
-2. `FormDialog`, a `QDialog` with a form inside with OK and Cancel button
-3. `Worker`, a class that defines a `QRunnable` to
-   handle worker thread setup, signals and wrap up
+1. `UIFormWidget`: a class to help creating Qt forms programmatically, useable in `QDockWidgets` and `QWidget`
+2. `FormDialog`: a `QDialog` with a form inside with <kbd>OK</kbd> and <kbd>Cancel</kbd> buttons
+3. `Worker`: a class that defines a `QRunnable` to handle worker thread setup, signals and wrap up
 
 ## Installation
 
-You may install via `pip` or `conda`
+Via `pip`/`conda`/`mamba`, i.e. any of the following:
 
-```bash
-python -m pip install eqt
-# or
-conda install eqt -c paskino
-```
+- `python -m pip install eqt`
+- `conda install -c conda-forge eqt`
+- `mamba install -c conda-forge eqt`
 
 ## Examples
 
-In the `example` directory there is an example on how to launch a `QDialog` with a form inside using `eqt`'s [`QWidget`](examples/dialog_example.py) or [`FormDialog`](examples/dialog_example_2.py).
+See the [`examples`](examples) directory, e.g. how to launch a `QDialog` with a form inside using `eqt`'s [`QWidget`](examples/dialog_example.py) or [`FormDialog`](examples/dialog_example_2.py).
 
 ### Running asynchronous tasks
 
 To run a function in a separate thread we use a `Worker` which is a subclass of a `QRunnable`.
 
 For the `Worker` to work one needs to define:
 
@@ -126,8 +124,11 @@
 result = QtCore.Signal(object)
 
 progress = QtCore.Signal(int)
 message = QtCore.Signal(str)
 status = QtCore.Signal(tuple)
 ```
 
-Read more on [Qt signals and slots](https://doc.qt.io/qt-5/signalsandslots.html) and on how to use them in [pyside2](https://wiki.qt.io/Qt_for_Python_Signals_and_Slots).
+Read more on [Qt signals and slots](https://doc.qt.io/qt-5/signalsandslots.html) and on how to use them in [PySide2](https://wiki.qt.io/Qt_for_Python_Signals_and_Slots).
+
+## Developer Contribution Guide
+See [CONTRIBUTING.md](./CONTRIBUTING.md).
```

### Comparing `eqt-0.7.1/eqt.egg-info/SOURCES.txt` & `eqt-1.0.0/eqt.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .git-blame-ignore-revs
 .gitignore
 .mailmap
 .pre-commit-config.yaml
+CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
 README.md
 pyproject.toml
 .github/workflows/test.yml
 eqt/__init__.py
 eqt/_dist_ver.py
@@ -25,19 +26,26 @@
 eqt/ui/SessionDialogs.py
 eqt/ui/UIFormWidget.py
 eqt/ui/UIMultiStepWidget.py
 eqt/ui/UISliderWidget.py
 eqt/ui/UIStackedWidget.py
 eqt/ui/__init__.py
 examples/MainWindowWithSessionManagement_example.py
+examples/advanced_dialog_example.py
 examples/dialog_example.py
 examples/dialog_example_2.py
+examples/dialog_example_3_save_default.py
 examples/dialog_multistep_example.py
 examples/dialog_save_state_example.py
+examples/insert_widgets_example.py
 examples/progress_timer_dialog_example.py
+examples/remove_widgets_example.py
 examples/reorderable_list_widget_example.py
+examples/utilitiesForExamples.py
+scripts/eqt_env.yml
 test/__init__.py
 test/dialog_example_2_test.py
 test/test_MainWindowWithSessionManagement.py
+test/test_MainWindowWithSessionManagementDialogs.py
 test/test_SessionDialogs.py
 test/test__formUI_status_test.py
 test/test_io.py
```

### Comparing `eqt-0.7.1/examples/MainWindowWithSessionManagement_example.py` & `eqt-1.0.0/examples/MainWindowWithSessionManagement_example.py`

 * *Files identical despite different names*

### Comparing `eqt-0.7.1/examples/dialog_example.py` & `eqt-1.0.0/examples/dialog_example.py`

 * *Files identical despite different names*

### Comparing `eqt-0.7.1/examples/dialog_example_2.py` & `eqt-1.0.0/examples/dialog_example_2.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,17 +21,16 @@
         self.setCentralWidget(widg)
 
         self.show()
 
     def openFormDialog(self):
         dialog = FormDialog(parent=self, title='Example')
         dialog.Ok.clicked.connect(lambda: self.accepted())
-        dialog.Cancel.clicked.connect(lambda: self.rejected())
 
-        # ## Example on how to add elements to the
+        # Example on how to add elements to the FormDialog
         # add input 1 as QLineEdit
         qlabel = QtWidgets.QLabel(dialog.groupBox)
         qlabel.setText("Input 1: ")
         qwidget = QtWidgets.QLineEdit(dialog.groupBox)
         qwidget.setClearButtonEnabled(True)
         # finally add to the form widget
         dialog.addSpanningWidget(QtWidgets.QLabel("Input Values: "), 'input_title')
@@ -50,27 +49,25 @@
         dialog.addWidget(QtWidgets.QLabel("Example Vertical Layout Text"), layout="vertical")
 
         # Example of using 'getWidget':
         dialog.getWidget('input2').setCurrentIndex(1)
 
         # store a reference
         self.dialog = dialog
-
+        self.dialog.onCancel = self.rejected
         dialog.exec()
 
     def accepted(self):
         print("accepted")
         print(self.dialog.widgets['input1_field'].text())
         print(self.dialog.widgets['input2_field'].currentText())
-
         self.dialog.close()
 
     def rejected(self):
         print("rejected")
-        self.dialog.close()
 
 
 if __name__ == "__main__":
     app = QtWidgets.QApplication(sys.argv)
 
     window = MainUI()
```

### Comparing `eqt-0.7.1/examples/dialog_multistep_example.py` & `eqt-1.0.0/examples/dialog_multistep_example.py`

 * *Files identical despite different names*

### Comparing `eqt-0.7.1/examples/dialog_save_state_example.py` & `eqt-1.0.0/examples/dialog_save_state_example.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,16 +19,14 @@
         widg = QtWidgets.QWidget()
         widg.setLayout(layout)
 
         self.setCentralWidget(widg)
 
         # create dialog to be opened later:
         dialog = FormDialog(parent=self, title='Example')
-        dialog.Ok.clicked.connect(lambda: self.accepted())
-        dialog.Cancel.clicked.connect(lambda: self.rejected())
 
         # ## Example on how to add elements to the
         dialog.addWidget(QtWidgets.QLabel('test label'), 'Label: ', 'label')
         dialog.addWidget(QtWidgets.QCheckBox('test checkbox'), 'CheckBox: ', 'checkBox')
         combobox = QtWidgets.QComboBox()
         combobox.addItems(['test1', 'test2'])
         dialog.addWidget(combobox, 'ComboBox: ', 'comboBox')
@@ -47,24 +45,16 @@
 
         # store a reference
         self.dialog = dialog
 
         self.show()
 
     def openFormDialog(self):
-        self.dialog.restoreAllSavedWidgetStates()
         self.dialog.exec()
 
-    def accepted(self):
-        self.dialog.saveAllWidgetStates()
-        self.dialog.close()
-
-    def rejected(self):
-        self.dialog.close()
-
 
 if __name__ == "__main__":
     app = QtWidgets.QApplication(sys.argv)
 
     window = MainUI()
 
     sys.exit(app.exec_())
```

### Comparing `eqt-0.7.1/examples/progress_timer_dialog_example.py` & `eqt-1.0.0/examples/progress_timer_dialog_example.py`

 * *Files identical despite different names*

### Comparing `eqt-0.7.1/examples/reorderable_list_widget_example.py` & `eqt-1.0.0/examples/reorderable_list_widget_example.py`

 * *Files identical despite different names*

### Comparing `eqt-0.7.1/pyproject.toml` & `eqt-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "eqt/_dist_ver.py"
 write_to_template = "__version__ = '{version}'\n"
 
 [tool.setuptools.packages.find]
-exclude = ["test", "examples"]
+include = ["eqt", "eqt.*"]
 
 [project.urls]
 documentation = "https://github.com/TomographicImaging/eqt#readme"
 repository = "https://github.com/TomographicImaging/eqt"
 changelog = "https://github.com/TomographicImaging/eqt/releases"
 
 [project]
```

### Comparing `eqt-0.7.1/test/__init__.py` & `eqt-1.0.0/test/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 
 from PySide2 import QtWidgets
 from pytest import skip
 
 from eqt.ui import FormDialog
 
-if any(os.getenv(var, '0').lower() in ('1', 'true') for var in ('CONDA_BUILD', 'CI')):
+is_ci = any(os.getenv(var, '0').lower() in ('1', 'true') for var in ('CONDA_BUILD', 'CI'))
+
+if is_ci:
 
     def skip_ci(_):
         def inner(*_, **__):
             skip("Running in CI (no GUI)")
 
         return inner
 else:
```

### Comparing `eqt-0.7.1/test/dialog_example_2_test.py` & `eqt-1.0.0/test/dialog_example_2_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         qwidget.setEnabled(True)
         # finally add to the form widget
         dialog.addWidget(qwidget, qlabel, 'input2')
 
         # store a reference
         self.dialog = dialog
 
-        dialog.exec()
+        dialog.open()
 
     def accepted(self):
         print("accepted")
         print(self.dialog.widgets['input1_field'].text())
         print(self.dialog.widgets['input2_field'].currentText())
 
         self.dialog.close()
```

### Comparing `eqt-0.7.1/test/test_MainWindowWithSessionManagement.py` & `eqt-1.0.0/test/test_MainWindowWithSessionManagement.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,64 +225,20 @@
 
     def tearDown(self):
         os.chdir("..")
         shutil.rmtree("Test Folder")
 
 
 @skip_ci
-class TestMainWindowWithSessionManagementCreateLoadSessionDialog(unittest.TestCase):
-    '''
-    Tests the createLoadSessionDialog method of the MainWindowWithSessionManagement class
-
-    This method is responsible for creating the load session dialog
-    and populating it with the available sessions
-    '''
-    def setUp(self):
-        self.title = "title"
-        self.app_name = "app_name"
-        self.smw = MainWindowWithSessionManagement(self.title, self.app_name)
-        self.smw.sessions_directory = mock.MagicMock()
-        self.zip_folders = ["zip_folder_1", "zip_folder_2"]
-
-    def test_createLoadSessionDialog_populates_session_dropdown(self):
-        dialog = self.smw.createLoadSessionDialog(self.zip_folders)
-        assert dialog is not None
-        assert isinstance(dialog, eqt.ui.SessionDialogs.LoadSessionDialog)
-        select_session_combo = dialog.getWidget('select_session')
-        assert select_session_combo is not None
-        items_in_combo = [
-            select_session_combo.itemText(i) for i in range(select_session_combo.count())]
-        assert items_in_combo == self.zip_folders
-
-    def test_createLoadSessionDialog_connections(self):
-        dialog = self.smw.createLoadSessionDialog(self.zip_folders)
-
-        self.smw.loadSessionLoad = mock.MagicMock()
-        self.smw.selectLoadSessionsDirectorySelectedInSessionSelector = mock.MagicMock()
-        self.smw.loadSessionNew = mock.MagicMock()
-
-        dialog = self.smw.createLoadSessionDialog(self.zip_folders)
-
-        dialog.Ok.click()
-        self.smw.loadSessionLoad.assert_called_once()
-
-        dialog.Select.click()
-        self.smw.selectLoadSessionsDirectorySelectedInSessionSelector.assert_called_with(dialog)
-
-        dialog.Cancel.click()
-        self.smw.loadSessionNew.assert_called_once()
-
-
-@skip_ci
 class TestSelectLoadSessionsDirectorySelectedInSessionSelector(unittest.TestCase):
     '''
     Tests the `selectLoadSessionsDirectorySelectedInSessionSelector` method of the
     `MainWindowWithSessionManagement` class
 
-    This method sould close the passed dialog, and call
+    This method should close the passed dialog, and call
     `createSessionsDirectorySelectionDialog(new_session=True)`
     '''
     def setUp(self):
         self.title = "title"
         self.app_name = "app_name"
         self.smw = MainWindowWithSessionManagement(self.title, self.app_name)
         self.load_session_dialog = mock.MagicMock()
```

### Comparing `eqt-0.7.1/test/test_SessionDialogs.py` & `eqt-1.0.0/test/test_SessionDialogs.py`

 * *Files identical despite different names*

### Comparing `eqt-0.7.1/test/test_io.py` & `eqt-1.0.0/test/test_io.py`

 * *Files identical despite different names*


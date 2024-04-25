# Comparing `tmp/totolo-1.2.tar.gz` & `tmp/totolo-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "totolo-1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "totolo-1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `totolo-1.2.tar` & `totolo-1.4.tar`

### file list

```diff
@@ -1,52 +1,65 @@
--rw-r--r--   0        0        0      834 2023-12-07 11:11:22.844177 totolo-1.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2023-12-07 11:11:22.844177 totolo-1.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1096 2023-12-07 11:11:22.844177 totolo-1.2/.github/workflows/coverage-branch.yaml
--rw-r--r--   0        0        0     1143 2023-12-07 11:11:22.844177 totolo-1.2/.github/workflows/coverage.yaml
--rw-r--r--   0        0        0     1300 2023-12-07 11:11:22.844177 totolo-1.2/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      862 2023-12-07 11:11:22.844177 totolo-1.2/.github/workflows/test.yaml
--rw-r--r--   0        0        0     3088 2023-12-07 11:11:22.844177 totolo-1.2/.gitignore
--rw-r--r--   0        0        0     1528 2023-12-07 11:11:22.844177 totolo-1.2/.vscode/launch.json
--rw-r--r--   0        0        0      277 2023-12-07 11:11:22.844177 totolo-1.2/.vscode/settings.json
--rw-r--r--   0        0        0     1071 2023-12-07 11:11:22.844177 totolo-1.2/LICENSE
--rw-r--r--   0        0        0     3931 2023-12-07 11:11:22.844177 totolo-1.2/README.md
--rw-r--r--   0        0        0     1104 2023-12-07 11:11:22.844177 totolo-1.2/examples/basics.py
--rw-r--r--   0        0        0     1450 2023-12-07 11:11:22.844177 totolo-1.2/pyproject.toml
--rw-r--r--   0        0        0       46 2023-12-07 11:11:22.844177 totolo-1.2/requirements-dev.txt
--rw-r--r--   0        0        0        0 2023-12-07 11:11:22.844177 totolo-1.2/tests/__init__.py
--rw-r--r--   0        0        0       24 2023-12-07 11:11:22.844177 totolo-1.2/tests/data/cycles1.th.txt
--rw-r--r--   0        0        0       47 2023-12-07 11:11:22.844177 totolo-1.2/tests/data/cycles2.th.txt
--rw-r--r--   0        0        0       71 2023-12-07 11:11:22.844177 totolo-1.2/tests/data/cycles3.th.txt
--rw-r--r--   0        0        0   173716 2023-12-07 11:11:22.844177 totolo-1.2/tests/data/film-timeout-top100.st.txt
--rw-r--r--   0        0        0   332534 2023-12-07 11:11:22.844177 totolo-1.2/tests/data/flat.tar.gz
--rw-r--r--   0        0        0      166 2023-12-07 11:11:22.844177 totolo-1.2/tests/data/messy.st.txt
--rw-r--r--   0        0        0   332557 2023-12-07 11:11:22.848177 totolo-1.2/tests/data/sample-2023.07.23.tar.gz
--rw-r--r--   0        0        0    34632 2023-12-07 11:11:22.848177 totolo-1.2/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt
--rw-r--r--   0        0        0    28050 2023-12-07 11:11:22.848177 totolo-1.2/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt
--rw-r--r--   0        0        0    48760 2023-12-07 11:11:22.848177 totolo-1.2/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt
--rw-r--r--   0        0        0  1011578 2023-12-07 11:11:22.852177 totolo-1.2/tests/data/sample-2023.07.23/notes/themes/primary.th.txt
--rw-r--r--   0        0        0    14882 2023-12-07 11:11:22.852177 totolo-1.2/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt
--rw-r--r--   0        0        0      428 2023-12-07 11:11:22.852177 totolo-1.2/tests/data/storytree.st.txt
--rw-r--r--   0        0        0  1011579 2023-12-07 11:11:22.856177 totolo-1.2/tests/data/to-2023.07.09.th.txt
--rw-r--r--   0        0        0     2365 2023-12-07 11:11:22.856177 totolo-1.2/tests/data/to-sample-2023.07.09-copy.st.txt
--rw-r--r--   0        0        0     2365 2023-12-07 11:11:22.856177 totolo-1.2/tests/data/to-sample-2023.07.09.st.txt
--rw-r--r--   0        0        0     6170 2023-12-07 11:11:22.856177 totolo-1.2/tests/test_entries.py
--rw-r--r--   0        0        0     5663 2023-12-07 11:11:22.856177 totolo-1.2/tests/test_impl.py
--rw-r--r--   0        0        0     2219 2023-12-07 11:11:22.856177 totolo-1.2/tests/test_lib.py
--rw-r--r--   0        0        0     1909 2023-12-07 11:11:22.860177 totolo-1.2/tests/test_toset.py
--rw-r--r--   0        0        0    12624 2023-12-07 11:11:22.860177 totolo-1.2/tests/test_totolo.py
--rw-r--r--   0        0        0      189 2023-12-07 11:11:22.860177 totolo-1.2/totolo/__init__.py
--rw-r--r--   0        0        0     1201 2023-12-07 11:11:22.860177 totolo-1.2/totolo/api.py
--rw-r--r--   0        0        0     1893 2023-12-07 11:11:22.860177 totolo-1.2/totolo/collection.py
--rw-r--r--   0        0        0        0 2023-12-07 11:11:22.860177 totolo-1.2/totolo/impl/__init__.py
--rw-r--r--   0        0        0     3036 2023-12-07 11:11:22.860177 totolo-1.2/totolo/impl/core.py
--rw-r--r--   0        0        0     5933 2023-12-07 11:11:22.860177 totolo-1.2/totolo/impl/entry.py
--rw-r--r--   0        0        0     3300 2023-12-07 11:11:22.860177 totolo-1.2/totolo/impl/field.py
--rw-r--r--   0        0        0      666 2023-12-07 11:11:22.860177 totolo-1.2/totolo/impl/keyword.py
--rw-r--r--   0        0        0     8111 2023-12-07 11:11:22.860177 totolo-1.2/totolo/impl/parser.py
--rw-r--r--   0        0        0        0 2023-12-07 11:11:22.860177 totolo-1.2/totolo/lib/__init__.py
--rw-r--r--   0        0        0     1134 2023-12-07 11:11:22.860177 totolo-1.2/totolo/lib/files.py
--rw-r--r--   0        0        0     1283 2023-12-07 11:11:22.860177 totolo-1.2/totolo/lib/textformat.py
--rw-r--r--   0        0        0     3605 2023-12-07 11:11:22.860177 totolo-1.2/totolo/story.py
--rw-r--r--   0        0        0     2395 2023-12-07 11:11:22.860177 totolo-1.2/totolo/theme.py
--rw-r--r--   0        0        0     8726 2023-12-07 11:11:22.860177 totolo-1.2/totolo/themeontology.py
--rw-r--r--   0        0        0     4363 1970-01-01 00:00:00.000000 totolo-1.2/PKG-INFO
+-rw-r--r--   0        0        0      834 2024-04-25 15:57:15.349500 totolo-1.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2024-04-25 15:57:15.349500 totolo-1.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1096 2024-04-25 15:57:15.349500 totolo-1.4/.github/workflows/coverage-branch.yaml
+-rw-r--r--   0        0        0     1106 2024-04-25 15:57:15.349500 totolo-1.4/.github/workflows/coverage.yaml
+-rw-r--r--   0        0        0     4043 2024-04-25 15:57:15.349500 totolo-1.4/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      825 2024-04-25 15:57:15.349500 totolo-1.4/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     3088 2024-04-25 15:57:15.349500 totolo-1.4/.gitignore
+-rw-r--r--   0        0        0     1550 2024-04-25 15:57:15.349500 totolo-1.4/.vscode/launch.json
+-rw-r--r--   0        0        0      277 2024-04-25 15:57:15.349500 totolo-1.4/.vscode/settings.json
+-rw-r--r--   0        0        0     1071 2024-04-25 15:57:15.349500 totolo-1.4/LICENSE
+-rw-r--r--   0        0        0     4126 2024-04-25 15:57:15.349500 totolo-1.4/README.md
+-rw-r--r--   0        0        0     1104 2024-04-25 15:57:15.349500 totolo-1.4/examples/basics.py
+-rw-r--r--   0        0        0     1662 2024-04-25 15:57:15.349500 totolo-1.4/pyproject.toml
+-rw-r--r--   0        0        0       60 2024-04-25 15:57:15.349500 totolo-1.4/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2024-04-25 15:57:15.349500 totolo-1.4/tests/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-25 15:57:15.349500 totolo-1.4/tests/data/cycles1.th.txt
+-rw-r--r--   0        0        0       47 2024-04-25 15:57:15.349500 totolo-1.4/tests/data/cycles2.th.txt
+-rw-r--r--   0        0        0       71 2024-04-25 15:57:15.349500 totolo-1.4/tests/data/cycles3.th.txt
+-rw-r--r--   0        0        0   173716 2024-04-25 15:57:15.349500 totolo-1.4/tests/data/film-timeout-top100.st.txt
+-rw-r--r--   0        0        0   332534 2024-04-25 15:57:15.349500 totolo-1.4/tests/data/flat.tar.gz
+-rw-r--r--   0        0        0      166 2024-04-25 15:57:15.349500 totolo-1.4/tests/data/messy.st.txt
+-rw-r--r--   0        0        0   332557 2024-04-25 15:57:15.353500 totolo-1.4/tests/data/sample-2023.07.23.tar.gz
+-rw-r--r--   0        0        0    34632 2024-04-25 15:57:15.353500 totolo-1.4/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt
+-rw-r--r--   0        0        0    28050 2024-04-25 15:57:15.353500 totolo-1.4/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt
+-rw-r--r--   0        0        0    48760 2024-04-25 15:57:15.353500 totolo-1.4/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt
+-rw-r--r--   0        0        0  1011578 2024-04-25 15:57:15.357500 totolo-1.4/tests/data/sample-2023.07.23/notes/themes/primary.th.txt
+-rw-r--r--   0        0        0    14882 2024-04-25 15:57:15.357500 totolo-1.4/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt
+-rwxr-xr-x   0        0        0    10486 2024-04-25 15:57:15.357500 totolo-1.4/tests/data/scifi1920-mergelist.xlsx
+-rw-r--r--   0        0        0      428 2024-04-25 15:57:15.357500 totolo-1.4/tests/data/storytree.st.txt
+-rw-r--r--   0        0        0  1011579 2024-04-25 15:57:15.361500 totolo-1.4/tests/data/to-2023.07.09.th.txt
+-rw-r--r--   0        0        0     2365 2024-04-25 15:57:15.361500 totolo-1.4/tests/data/to-sample-2023.07.09-copy.st.txt
+-rw-r--r--   0        0        0     2365 2024-04-25 15:57:15.361500 totolo-1.4/tests/data/to-sample-2023.07.09.st.txt
+-rw-r--r--   0        0        0        0 2024-04-25 15:57:15.361500 totolo-1.4/tests/lib/__init__.py
+-rw-r--r--   0        0        0      745 2024-04-25 15:57:15.361500 totolo-1.4/tests/lib/test_excel.py
+-rw-r--r--   0        0        0      800 2024-04-25 15:57:15.361500 totolo-1.4/tests/lib/test_files.py
+-rw-r--r--   0        0        0      794 2024-04-25 15:57:15.361500 totolo-1.4/tests/lib/test_logging.py
+-rw-r--r--   0        0        0     1419 2024-04-25 15:57:15.361500 totolo-1.4/tests/lib/test_textformat.py
+-rw-r--r--   0        0        0     6170 2024-04-25 15:57:15.361500 totolo-1.4/tests/test_entries.py
+-rw-r--r--   0        0        0     6158 2024-04-25 15:57:15.365500 totolo-1.4/tests/test_impl.py
+-rw-r--r--   0        0        0     1909 2024-04-25 15:57:15.365500 totolo-1.4/tests/test_toset.py
+-rw-r--r--   0        0        0    15084 2024-04-25 15:57:15.365500 totolo-1.4/tests/test_totolo.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:57:15.365500 totolo-1.4/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1968 2024-04-25 15:57:15.365500 totolo-1.4/tests/utils/test_mergefiles.py
+-rw-r--r--   0        0        0     3191 2024-04-25 15:57:15.365500 totolo-1.4/tests/utils/test_mergelist.py
+-rw-r--r--   0        0        0      189 2024-04-25 15:57:15.365500 totolo-1.4/totolo/__init__.py
+-rw-r--r--   0        0        0     1201 2024-04-25 15:57:15.365500 totolo-1.4/totolo/api.py
+-rw-r--r--   0        0        0     1893 2024-04-25 15:57:15.365500 totolo-1.4/totolo/collection.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:57:15.365500 totolo-1.4/totolo/impl/__init__.py
+-rw-r--r--   0        0        0     3367 2024-04-25 15:57:15.365500 totolo-1.4/totolo/impl/core.py
+-rw-r--r--   0        0        0     6525 2024-04-25 15:57:15.365500 totolo-1.4/totolo/impl/entry.py
+-rw-r--r--   0        0        0     4595 2024-04-25 15:57:15.365500 totolo-1.4/totolo/impl/field.py
+-rw-r--r--   0        0        0      666 2024-04-25 15:57:15.365500 totolo-1.4/totolo/impl/keyword.py
+-rw-r--r--   0        0        0     8111 2024-04-25 15:57:15.365500 totolo-1.4/totolo/impl/parser.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:57:15.365500 totolo-1.4/totolo/lib/__init__.py
+-rw-r--r--   0        0        0     1690 2024-04-25 15:57:15.365500 totolo-1.4/totolo/lib/excel.py
+-rw-r--r--   0        0        0     1134 2024-04-25 15:57:15.365500 totolo-1.4/totolo/lib/files.py
+-rw-r--r--   0        0        0      248 2024-04-25 15:57:15.365500 totolo-1.4/totolo/lib/log.py
+-rw-r--r--   0        0        0     1283 2024-04-25 15:57:15.365500 totolo-1.4/totolo/lib/textformat.py
+-rw-r--r--   0        0        0     3605 2024-04-25 15:57:15.365500 totolo-1.4/totolo/story.py
+-rw-r--r--   0        0        0     2395 2024-04-25 15:57:15.365500 totolo-1.4/totolo/theme.py
+-rw-r--r--   0        0        0    11866 2024-04-25 15:57:15.365500 totolo-1.4/totolo/themeontology.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:57:15.365500 totolo-1.4/totolo/util/__init__.py
+-rw-r--r--   0        0        0     2221 2024-04-25 15:57:15.365500 totolo-1.4/totolo/util/mergefiles.py
+-rw-r--r--   0        0        0     7321 2024-04-25 15:57:15.365500 totolo-1.4/totolo/util/mergelist.py
+-rw-r--r--   0        0        0     4558 1970-01-01 00:00:00.000000 totolo-1.4/PKG-INFO
```

### Comparing `totolo-1.2/.github/ISSUE_TEMPLATE/bug_report.md` & `totolo-1.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `totolo-1.2/.github/ISSUE_TEMPLATE/feature_request.md` & `totolo-1.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `totolo-1.2/.github/workflows/coverage-branch.yaml` & `totolo-1.4/.github/workflows/coverage-branch.yaml`

 * *Files identical despite different names*

### Comparing `totolo-1.2/.github/workflows/coverage.yaml` & `totolo-1.4/.github/workflows/coverage.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 jobs:
   build-testcoverage:
     if: github.event.pull_request.merged == true || github.event_name == 'push'
 
     strategy:
       matrix:
-        python-version: ["3.8", "3.x"]
-        os: [ubuntu-latest, windows-latest, macos-latest]
+        python-version: ["3.x"]
+        os: [ubuntu-latest]
 
     runs-on: ${{ matrix.os }}
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
```

### Comparing `totolo-1.2/.github/workflows/test.yaml` & `totolo-1.4/.github/workflows/test.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     branches: [ main ]
     types: [ opened, synchronized, closed ]
 
 jobs:
   build-test:
     strategy:
       matrix:
-        python-version: ["3.8", "3.x"]
-        os: [ubuntu-latest, windows-latest, macos-latest]
+        python-version: ["3.x"]
+        os: [ubuntu-latest]
 
     runs-on: ${{ matrix.os }}
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
```

### Comparing `totolo-1.2/.gitignore` & `totolo-1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `totolo-1.2/.vscode/launch.json` & `totolo-1.4/.vscode/launch.json`

 * *Files 1% similar despite different names*

```diff
@@ -39,13 +39,14 @@
             "purpose": [
                 "debug-test"
             ],
             "console": "integratedTerminal",
             "justMyCode": false,
             "args": [
                 "-c",
+                "-v",
                 "pytest.ini"
             ],
             "internalConsoleOptions": "openOnSessionStart",
         }
     ]
 }
```

### Comparing `totolo-1.2/LICENSE` & `totolo-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `totolo-1.2/README.md` & `totolo-1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -83,29 +83,41 @@
 52454  videogame: Final Fantasy VI (1994)  Final Fantasy VI  1994-04-02             father and son  Minor Themes
 
 [52455 rows x 5 columns]
 ```
 
 ## Snippets
 
+List official versioned releases of the ontology:
+
+```python
+    list(totolo.remote.versions())
+```
+
+Load the v2023.06 release:
+
+```python
+    ontology = totolo.remote.version('v2023.06')
+```
+
 Create an excel sheet with all the usages of the theme "loyalty" as well as any child theme of the same:
 
 ```python
     df = ontology.theme['loyalty'].descendants().dataframe(motivation=True, descriptions=True)
     df.to_excel("/mnt/d/repos/themelist-loyalty.xlsx", "loyalty")
 ```
 
 Find theme entries in stories according to some criteria. For example, find empty motivations:
 
 ```python
     empty_motivations = [
         (story, weight, part)
         for story in ontology.stories()
         for weight, part in story.iter_theme_entries()
-        if part.motivation.strip()==""
+        if part.motivation.strip() == ""
     ]
 ```
 
 ## Getting Help
 
 If you encounter a bug, please file a minimal reproducible example on
 [GitHub issues](https://github.com/theme-ontology/python-totolo/issues/). For
```

### Comparing `totolo-1.2/examples/basics.py` & `totolo-1.4/examples/basics.py`

 * *Files identical despite different names*

### Comparing `totolo-1.2/pyproject.toml` & `totolo-1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -20,18 +20,25 @@
 
 [tool.pylint."MESSAGES CONTROL"]
 disable = [
     "missing-module-docstring",         # don't want it
     "missing-class-docstring",          # don't want it
     "missing-function-docstring",       # don't want it
     "too-few-public-methods",           # don't want it
+    "logging-fstring-interpolation",    # don't want it
     "too-many-arguments",               # borderline acceptable
     "super-init-not-called",            # borderline acceptable
     "import-outside-toplevel",          # borderline acceptable
     "no-member",                        # pylint gets it wrong
     "unsupported-membership-test",      # pylint gets it wrong
     "not-callable",                     # pylint gets it wrong
     "unsubscriptable-object",           # pylint gets it wrong
     "unsupported-assignment-operation", # pylint gets it wrong
     "unsupported-delete-operation",     # pylint gets it wrong
     "super-with-arguments",             # pylint gets it wrong
+    "abstract-class-instantiated",      # pylint gets it wrong with ExcelWriter
 ]
+
+[tool.coverage.report]
+exclude_also = [
+    "if __name__ == .__main__.:",
+]
```

### Comparing `totolo-1.2/tests/data/film-timeout-top100.st.txt` & `totolo-1.4/tests/data/film-timeout-top100.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.2/tests/data/flat.tar.gz` & `totolo-1.4/tests/data/flat.tar.gz`

 * *Files identical despite different names*

### Comparing `totolo-1.2/tests/data/sample-2023.07.23.tar.gz` & `totolo-1.4/tests/data/sample-2023.07.23.tar.gz`

 * *Files identical despite different names*

### Comparing `totolo-1.2/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt` & `totolo-1.4/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.2/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt` & `totolo-1.4/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.2/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt` & `totolo-1.4/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.2/tests/data/sample-2023.07.23/notes/themes/primary.th.txt` & `totolo-1.4/tests/data/sample-2023.07.23/notes/themes/primary.th.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.2/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt` & `totolo-1.4/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.2/tests/data/to-2023.07.09.th.txt` & `totolo-1.4/tests/data/to-2023.07.09.th.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.2/tests/data/to-sample-2023.07.09-copy.st.txt` & `totolo-1.4/tests/data/to-sample-2023.07.09-copy.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.2/tests/data/to-sample-2023.07.09.st.txt` & `totolo-1.4/tests/data/to-sample-2023.07.09.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.2/tests/test_entries.py` & `totolo-1.4/tests/test_entries.py`

 * *Files identical despite different names*

### Comparing `totolo-1.2/tests/test_impl.py` & `totolo-1.4/tests/test_impl.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import pytest
 
 import totolo
 from totolo.impl.core import TOObject, a, sa
 from totolo.impl.field import TOField
 from totolo.impl.parser import TOParser
 from totolo.story import TOStory
@@ -13,14 +14,19 @@
     a3 = a(private=True)
     bb = sa("txt", default="baz: b", required=True)
     cc = sa("txt", default="baz: c")
     aa = sa("txt", default="baz: a")
 
 
 class TestTOObject:
+    def test_equality(self):
+        assert TOTest1() == TOTest1()
+        assert TOTest1() != TOObject()
+        assert TOTest1() != TOTest1(a1="bar")
+
     def test_object_attributes(self):
         a = TOTest1(a2="fox")
         assert a.a1 == "foo"
         assert a.a2 == "fox"
         attrs = [k for k, _ in a.iter_attrs()]
         sattrs = [k for k, _ in a.iter_stored()]
         assert attrs == ["a1", "a2", "a3", "bb", "cc", "aa"]
@@ -52,14 +58,25 @@
         ]
         for strobj in strs:
             assert isinstance(strobj, str)
             assert len(strobj) > 5
 
 
 class TestField:
+    def test_equality(self):
+        f1 = TOField(name="foo", fieldtype="text", source=["source line"]).setup()
+        assert f1 != "bogus"
+        f2 = copy.deepcopy(f1)
+        assert f1 == f2
+        f2.name = "bar"
+        assert f1 != f2
+        f2 = copy.deepcopy(f1)
+        f2.fieldtype = "blob"
+        assert f1 != f2
+
     def make_field(self, fieldtype="text"):
         field = TOField(name="foo", fieldtype=fieldtype, source=["source line"]).setup()
         if fieldtype == "kwlist":
             field.insert_kw(
                 keyword="foo",
                 motivation="bar",
                 capacity="baz",
```

### Comparing `totolo-1.2/tests/test_toset.py` & `totolo-1.4/tests/test_toset.py`

 * *Files identical despite different names*

### Comparing `totolo-1.2/tests/test_totolo.py` & `totolo-1.4/tests/test_totolo.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import difflib
 import io
 import json
 import os.path
 import tempfile
 import urllib.request
 from unittest.mock import patch
+import copy
 
 import pandas as pd
 import pytest
 
 import totolo
 from totolo.story import TOStory
 from totolo.theme import TOTheme
@@ -321,7 +322,82 @@
     def test_multiple_entries(self):
         ontology = totolo.files([
             "tests/data/to-sample-2023.07.09.st.txt",
             "tests/data/to-sample-2023.07.09-copy.st.txt",
         ])
         warnings = list(ontology.validate_entries())
         assert any("Multiple TOStory with name" in x for x in warnings)
+
+
+class TestOperations:
+    def test_equality(self):
+        o1 = totolo.files("tests/data/sample-2023.07.23")
+        o2 = totolo.files("tests/data/sample-2023.07.23")
+        assert o1 == o2
+        s1 = o1.story["movie: Dr. Jekyll and Mr. Hyde (1920 I)"]
+        s1["Major Themes"].delete_kw("mad scientist stereotype")
+        assert o1 != o2
+        del o1.story["movie: Dr. Jekyll and Mr. Hyde (1920 I)"]
+        assert o1 != o2
+
+        o1 = copy.deepcopy(o2)
+        assert o1 == o2
+        o1["bar theme"] = TOTheme()
+        assert o1 != o2
+
+
+    def test_addition(self):
+        o1 = totolo.files("tests/data/sample-2023.07.23")
+        o2 = totolo.files("tests/data/sample-2023.07.23")
+
+        del o1["movie: Dr. Jekyll and Mr. Hyde (1920 II)"]
+        s1 = o1.story["movie: Dr. Jekyll and Mr. Hyde (1920 I)"]
+        s1["Major Themes"].delete_kw("mad scientist stereotype")
+        o3 = o1 + o2
+        o1 += o2
+        assert o1 == o2
+        assert o3 == o2
+        o2["foo story"] = TOStory()
+        o2["bar theme"] = TOTheme()
+        o1 += o2
+        assert o1 == o2
+
+    def test_get(self):
+        o1 = totolo.files("tests/data/sample-2023.07.23")
+        o1["foo"] = TOTheme()
+        assert o1["foo"].name == "foo"
+        o1.story["foo"] = TOStory()  # invalid usage
+        with pytest.raises(KeyError):
+            o1["foo"]
+
+    def test_del(self):
+        o1 = totolo.files("tests/data/sample-2023.07.23")
+        o1["foo"] = TOTheme()
+        del o1["foo"]
+        assert o1 == totolo.files("tests/data/sample-2023.07.23")
+        o1["foo"] = TOStory()
+        del o1["foo"]
+        assert o1 == totolo.files("tests/data/sample-2023.07.23")
+
+    def test_set(self):
+        o1 = totolo.files("tests/data/sample-2023.07.23")
+        with pytest.raises(ValueError):
+            o1["foo"] = "bar"
+        o1["bar"] = TOTheme()
+        o1["foo"] = TOTheme()
+        o1["foo"] = TOStory()
+        assert "foo" not in o1.theme
+        assert "foo" in o1.story
+        assert "bar" in o1.theme
+
+    def test_contains(self):
+        o1 = totolo.files("tests/data/sample-2023.07.23")
+        o1["foo"] = TOStory()
+        o1["bar"] = TOTheme()
+        assert "foo" in o1
+        assert "bar" in o1
+        assert TOStory(name="foo") in o1
+        assert TOTheme(name="bar") in o1
+        assert TOTheme(name="foo") not in o1
+        assert TOStory(name="bar") not in o1
+        assert 42 not in o1
+        assert ... not in o1
```

### Comparing `totolo-1.2/totolo/api.py` & `totolo-1.4/totolo/api.py`

 * *Files identical despite different names*

### Comparing `totolo-1.2/totolo/collection.py` & `totolo-1.4/totolo/collection.py`

 * *Files identical despite different names*

### Comparing `totolo-1.2/totolo/impl/core.py` & `totolo-1.4/totolo/impl/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,14 +70,23 @@
 
 
 class TOObject(metaclass=TOObjectMeta):
     def __init__(self, **kwargs):
         super().__init__()
         self.__dict__.update(kwargs)
 
+    def __eq__(self, other):
+        if {k for k, _ in self.iter_attrs()} != {k for k, _ in other.iter_attrs()}:
+            return False
+        for key, attr in self.iter_attrs():
+            if not attr.private:
+                if getattr(self, key) != getattr(other, key):
+                    return False
+        return True
+
     def get_attr(self, key):
         return self._to_attrs.get(key)
 
     def iter_attrs(self):
         for key, value in self._to_attrs.items():
             yield key, value
```

### Comparing `totolo-1.2/totolo/impl/entry.py` & `totolo-1.4/totolo/impl/entry.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,17 +9,36 @@
     fields = a(OrderedDict)
     parents = a(set)
     children = a(set)
     source = a(list)
     source_location = a("<api>)")
     ontology = a(lambda: (lambda: None))
 
+    def __iadd__(self, other):
+        assert isinstance(other, TOEntry)
+        assert self.name == other.name
+        for key, other_field in other.fields.items():
+            self_field = self.setdefault(key)
+            self_field += other_field
+        self.parents |= other.parents
+        self.children |= other.children
+        return self
+
     def __lt__(self, other):
         return str(self) < str(other)
 
+    def __eq__(self, other):
+        if type(self) is not type(other):
+            return False
+        if self.name != other.name:
+            return False
+        if self.fields != other.fields:
+            return False
+        return True
+
     def __hash__(self):
         return hash(self.name)
 
     def __str__(self):
         name = self.name.encode("ascii", "ignore")
         return f"{name}[{len(self.fields)}]"
```

### Comparing `totolo-1.2/totolo/impl/keyword.py` & `totolo-1.4/totolo/impl/keyword.py`

 * *Files identical despite different names*

### Comparing `totolo-1.2/totolo/impl/parser.py` & `totolo-1.4/totolo/impl/parser.py`

 * *Files identical despite different names*

### Comparing `totolo-1.2/totolo/lib/files.py` & `totolo-1.4/totolo/lib/files.py`

 * *Files identical despite different names*

### Comparing `totolo-1.2/totolo/lib/textformat.py` & `totolo-1.4/totolo/lib/textformat.py`

 * *Files identical despite different names*

### Comparing `totolo-1.2/totolo/story.py` & `totolo-1.4/totolo/story.py`

 * *Files identical despite different names*

### Comparing `totolo-1.2/totolo/theme.py` & `totolo-1.4/totolo/theme.py`

 * *Files identical despite different names*

### Comparing `totolo-1.2/totolo/themeontology.py` & `totolo-1.4/totolo/themeontology.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,116 @@
 import copy
 import os.path
 import random
 from collections import defaultdict
+import weakref
 
 from .impl.core import TOObject, a
 from .collection import TODict
+from .story import TOStory
+from .theme import TOTheme
 
 
 class ThemeOntology(TOObject):
     theme = a(TODict)
     story = a(TODict)
     entries = a(dict)
     basepaths = a(set)
 
     def __len__(self):
         return sum(len(v) for v in self.entries.values())
 
     def __str__(self):
-        return f"<{len(self.theme)} themes, {len(self.story)} stories>"
+        return f"ThemeOntology<{len(self.theme)} themes, {len(self.story)} stories>"
+
+    def __iadd__(self, other):
+        assert isinstance(other, ThemeOntology)
+        other_prefix = os.path.commonpath(other.basepaths)
+        self_prefix = os.path.commonpath(self.basepaths)
+        for other_path, other_entries in other.entries.items():
+            if os.path.commonprefix([other_prefix, other_path]) != other_prefix:
+                new_path = other_path  # probably not a path, e.g. '<api>'
+            else:
+                new_path = os.path.join(self_prefix, os.path.relpath(other_path, other_prefix))
+            self_entries = self.entries.setdefault(new_path, [])
+            entry_lu = {e.name: e for e in self_entries}
+            for other_entry in other_entries:
+                if other_entry.name  in entry_lu:
+                    entry_lu[other_entry.name] += other_entry
+                else:
+                    new_entry = copy.deepcopy(other_entry)
+                    new_entry.ontology = weakref.ref(self)
+                    self_entries.append(new_entry)
+                    if isinstance(new_entry, TOStory):
+                        self.story[new_entry.name] = new_entry
+                    elif isinstance(new_entry, TOTheme):
+                        self.theme[new_entry.name] = new_entry
+        self.refresh_relations()
+        return self
+
+    def __add__(self, other):
+        result = copy.deepcopy(self)
+        result += other
+        return result
+
+    def __eq__(self, other):
+        if self.theme != other.theme:
+            return False
+        if self.story != other.story:
+            return False
+        return True
+
+    def __contains__(self, obj):
+        if isinstance(obj, str):
+            return obj in self.story or obj in self.theme
+        if isinstance(obj, TOTheme):
+            return self.theme.get(obj.name, None) == obj
+        if isinstance(obj, TOStory):
+            return self.story.get(obj.name, None) == obj
+        return False
+
+    def __getitem__(self, key):
+        if key in self.theme:
+            if key in self.story:
+                raise KeyError(f"Ambiguous Key: '{key}' is both a theme and a story.")
+            return self.theme[key]
+        return self.story[key]
+
+    def __setitem__(self, key, value):
+        if not isinstance(value, (TOStory, TOTheme)):
+            raise ValueError(
+                f"Can only insert TOTheme or TOStory into ontology, not {type(value)}."
+            )
+        if not value.name:
+            value.name = key
+        assert value.name == key
+        try:
+            del self[key]
+        except KeyError:
+            pass
+        if isinstance(value, TOStory):
+            self.story[key] = value
+        elif isinstance(value, TOTheme):
+            self.theme[key] = value
+        self.entries.setdefault(value.source_location, []).append(value)
+        value.ontology = weakref.ref(self)
+
+    def __delitem__(self, key):
+        item = self[key]
+        self.entries[item.source_location].remove(item)
+        if key in self.theme:
+            del self.theme[key]
+        if key in self.story:
+            del self.story[key]
 
     def stories(self):
-        for story in self.story.values():
-            yield story
+        yield from self.story.values()
 
     def themes(self):
-        for theme in self.theme.values():
-            yield theme
+        yield from self.theme.values()
 
     def astory(self):
         return random.sample(list(self.story.values()), 1)[0]
 
     def atheme(self):
         return random.sample(list(self.theme.values()), 1)[0]
 
@@ -88,30 +169,30 @@
         descriptions=False,
     ):
         data = []
         for weight, part in story.iter_theme_entries():
             themes = [part.keyword]
             if implied_themes and part.keyword in self.theme:
                 theme = self.theme[part.keyword]
-                themes.extend(theme.ancestors())
-            for theme in themes:
+                themes.extend(t.name for t in theme.ancestors())
+            for themename in themes:
                 record = [
                     story.name,
                     story["Title"],
                     story["Date"],
-                    theme,
+                    themename,
                     weight,
                 ]
                 if motivation:
                     record.append(part.motivation)
                 if descriptions:
                     record.append(story.verbose_description())
                     record.append(
-                        self.theme[theme].verbose_description()
-                        if theme in self.theme else ""
+                        self.theme[themename].verbose_description()
+                        if themename in self.theme else ""
                     )
                 data.append(record)
         return data
 
     def validate(self):
         yield from self.validate_entries()
         yield from self.validate_storythemes()
@@ -219,15 +300,15 @@
                     story.children.add(cstory_name)
                     self.story[cstory_name].parents.add(story.name)
         return self
 
     def _writefile(self, path, entries, cleaned):
         cskey = "Component Stories"
         dirname = os.path.dirname(path)
-        if not os.path.exists(dirname):
+        if dirname and not os.path.exists(dirname):
             os.makedirs(dirname)
         with open(path, "w", encoding='utf-8') as fhandle:
             sids = set(e.name for e in entries)
             for idx, entry in enumerate(entries):
                 if idx == 0 and entry.name in entry["Collections"]:
                     field = entry.get(cskey)
                     all_parts = list(field)
```

### Comparing `totolo-1.2/PKG-INFO` & `totolo-1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: totolo
-Version: 1.2
+Version: 1.4
 Summary: The Python interface to themeontology.org.
 Author-email: Mikael Onsjö <mikael@odinlake.net>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Documentation, https://github.com/theme-ontology/theming
 Project-URL: Home, https://www.themeontology.org/
 Project-URL: Source, https://github.com/theme-ontology/python-totolo
@@ -94,29 +94,41 @@
 52454  videogame: Final Fantasy VI (1994)  Final Fantasy VI  1994-04-02             father and son  Minor Themes
 
 [52455 rows x 5 columns]
 ```
 
 ## Snippets
 
+List official versioned releases of the ontology:
+
+```python
+    list(totolo.remote.versions())
+```
+
+Load the v2023.06 release:
+
+```python
+    ontology = totolo.remote.version('v2023.06')
+```
+
 Create an excel sheet with all the usages of the theme "loyalty" as well as any child theme of the same:
 
 ```python
     df = ontology.theme['loyalty'].descendants().dataframe(motivation=True, descriptions=True)
     df.to_excel("/mnt/d/repos/themelist-loyalty.xlsx", "loyalty")
 ```
 
 Find theme entries in stories according to some criteria. For example, find empty motivations:
 
 ```python
     empty_motivations = [
         (story, weight, part)
         for story in ontology.stories()
         for weight, part in story.iter_theme_entries()
-        if part.motivation.strip()==""
+        if part.motivation.strip() == ""
     ]
 ```
 
 ## Getting Help
 
 If you encounter a bug, please file a minimal reproducible example on
 [GitHub issues](https://github.com/theme-ontology/python-totolo/issues/). For
```


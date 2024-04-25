# Comparing `tmp/tables-io-0.9.5.tar.gz` & `tmp/tables_io-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tables-io-0.9.5.tar", last modified: Wed Mar  6 23:40:32 2024, max compression
+gzip compressed data, was "tables_io-0.9.6.tar", last modified: Thu Apr 25 03:06:23 2024, max compression
```

## Comparing `tables-io-0.9.5.tar` & `tables_io-0.9.6.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 23:40:32.093639 tables-io-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-06 23:40:25.000000 tables-io-0.9.5/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-06 23:40:25.000000 tables-io-0.9.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 23:40:32.081639 tables-io-0.9.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 23:40:32.081639 tables-io-0.9.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-06 23:40:25.000000 tables-io-0.9.5/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-06 23:40:25.000000 tables-io-0.9.5/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-06 23:40:25.000000 tables-io-0.9.5/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-06 23:40:25.000000 tables-io-0.9.5/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 23:40:32.081639 tables-io-0.9.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-06 23:40:25.000000 tables-io-0.9.5/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-06 23:40:25.000000 tables-io-0.9.5/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-06 23:40:25.000000 tables-io-0.9.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-06 23:40:25.000000 tables-io-0.9.5/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-03-06 23:40:25.000000 tables-io-0.9.5/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-03-06 23:40:25.000000 tables-io-0.9.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-03-06 23:40:25.000000 tables-io-0.9.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-06 23:40:25.000000 tables-io-0.9.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-06 23:40:25.000000 tables-io-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-03-06 23:40:32.093639 tables-io-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-06 23:40:25.000000 tables-io-0.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 23:40:32.085639 tables-io-0.9.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-03-06 23:40:25.000000 tables-io-0.9.5/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-06 23:40:25.000000 tables-io-0.9.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-03-06 23:40:25.000000 tables-io-0.9.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-03-06 23:40:25.000000 tables-io-0.9.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-06 23:40:25.000000 tables-io-0.9.5/docs/install.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 23:40:32.085639 tables-io-0.9.5/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-06 23:40:25.000000 tables-io-0.9.5/docs/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 23:40:25.000000 tables-io-0.9.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-06 23:40:25.000000 tables-io-0.9.5/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 23:40:32.085639 tables-io-0.9.5/nb/
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-06 23:40:25.000000 tables-io-0.9.5/nb/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-03-06 23:40:25.000000 tables-io-0.9.5/nb/hdf5_iter_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-03-06 23:40:25.000000 tables-io-0.9.5/nb/multipleWriteHdf5_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-03-06 23:40:25.000000 tables-io-0.9.5/nb/singleTable_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-03-06 23:40:25.000000 tables-io-0.9.5/nb/tableDict_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-03-06 23:40:25.000000 tables-io-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 23:40:32.093639 tables-io-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-06 23:40:25.000000 tables-io-0.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 23:40:32.081639 tables-io-0.9.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 23:40:32.085639 tables-io-0.9.5/src/tables_io/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-06 23:40:25.000000 tables-io-0.9.5/src/tables_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-06 23:40:31.000000 tables-io-0.9.5/src/tables_io/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-03-06 23:40:25.000000 tables-io-0.9.5/src/tables_io/arrayUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-03-06 23:40:25.000000 tables-io-0.9.5/src/tables_io/convUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    37461 2024-03-06 23:40:25.000000 tables-io-0.9.5/src/tables_io/ioUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-03-06 23:40:25.000000 tables-io-0.9.5/src/tables_io/lazy_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-03-06 23:40:25.000000 tables-io-0.9.5/src/tables_io/tableDict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-03-06 23:40:25.000000 tables-io-0.9.5/src/tables_io/testUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-03-06 23:40:25.000000 tables-io-0.9.5/src/tables_io/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 23:40:32.089639 tables-io-0.9.5/src/tables_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-03-06 23:40:32.000000 tables-io-0.9.5/src/tables_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-06 23:40:32.000000 tables-io-0.9.5/src/tables_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 23:40:32.000000 tables-io-0.9.5/src/tables_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-06 23:40:32.000000 tables-io-0.9.5/src/tables_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-06 23:40:32.000000 tables-io-0.9.5/src/tables_io.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 23:40:32.089639 tables-io-0.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-06 23:40:25.000000 tables-io-0.9.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 23:40:32.089639 tables-io-0.9.5/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-03-06 23:40:25.000000 tables-io-0.9.5/tests/data/no_groupname_test.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)     9104 2024-03-06 23:40:25.000000 tables-io-0.9.5/tests/data/pandas_test_hdf5.h5
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-03-06 23:40:25.000000 tables-io-0.9.5/tests/data/parquet_test.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-03-06 23:40:25.000000 tables-io-0.9.5/tests/test_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-03-06 23:40:25.000000 tables-io-0.9.5/tests/test_fileIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-03-06 23:40:25.000000 tables-io-0.9.5/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-03-06 23:40:25.000000 tables-io-0.9.5/tests/test_table_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-03-06 23:40:25.000000 tables-io-0.9.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:06:23.233872 tables_io-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-25 03:06:14.000000 tables_io-0.9.6/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 03:06:14.000000 tables_io-0.9.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:06:23.221871 tables_io-0.9.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:06:23.221871 tables_io-0.9.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 03:06:14.000000 tables_io-0.9.6/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-25 03:06:14.000000 tables_io-0.9.6/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-25 03:06:14.000000 tables_io-0.9.6/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-25 03:06:14.000000 tables_io-0.9.6/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:06:23.221871 tables_io-0.9.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-25 03:06:14.000000 tables_io-0.9.6/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-25 03:06:14.000000 tables_io-0.9.6/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-25 03:06:14.000000 tables_io-0.9.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-25 03:06:14.000000 tables_io-0.9.6/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-25 03:06:14.000000 tables_io-0.9.6/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-25 03:06:14.000000 tables_io-0.9.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-25 03:06:14.000000 tables_io-0.9.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-25 03:06:14.000000 tables_io-0.9.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-25 03:06:14.000000 tables_io-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-25 03:06:23.233872 tables_io-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-25 03:06:14.000000 tables_io-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:06:23.225872 tables_io-0.9.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-25 03:06:14.000000 tables_io-0.9.6/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-25 03:06:14.000000 tables_io-0.9.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-25 03:06:14.000000 tables_io-0.9.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-25 03:06:14.000000 tables_io-0.9.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-25 03:06:14.000000 tables_io-0.9.6/docs/install.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:06:23.225872 tables_io-0.9.6/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 03:06:14.000000 tables_io-0.9.6/docs/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 03:06:14.000000 tables_io-0.9.6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-25 03:06:14.000000 tables_io-0.9.6/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:06:23.225872 tables_io-0.9.6/nb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-25 03:06:14.000000 tables_io-0.9.6/nb/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-25 03:06:14.000000 tables_io-0.9.6/nb/hdf5_iter_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-04-25 03:06:14.000000 tables_io-0.9.6/nb/multipleWriteHdf5_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-04-25 03:06:14.000000 tables_io-0.9.6/nb/singleTable_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-25 03:06:14.000000 tables_io-0.9.6/nb/tableDict_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-25 03:06:14.000000 tables_io-0.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 03:06:23.233872 tables_io-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-25 03:06:14.000000 tables_io-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:06:23.217872 tables_io-0.9.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:06:23.225872 tables_io-0.9.6/src/tables_io/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-25 03:06:14.000000 tables_io-0.9.6/src/tables_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 03:06:22.000000 tables_io-0.9.6/src/tables_io/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-25 03:06:14.000000 tables_io-0.9.6/src/tables_io/arrayUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-25 03:06:14.000000 tables_io-0.9.6/src/tables_io/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-04-25 03:06:14.000000 tables_io-0.9.6/src/tables_io/convUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37461 2024-04-25 03:06:14.000000 tables_io-0.9.6/src/tables_io/ioUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-25 03:06:14.000000 tables_io-0.9.6/src/tables_io/lazy_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-25 03:06:14.000000 tables_io-0.9.6/src/tables_io/tableDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-25 03:06:14.000000 tables_io-0.9.6/src/tables_io/testUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-04-25 03:06:14.000000 tables_io-0.9.6/src/tables_io/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:06:23.229872 tables_io-0.9.6/src/tables_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-25 03:06:23.000000 tables_io-0.9.6/src/tables_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-25 03:06:23.000000 tables_io-0.9.6/src/tables_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 03:06:23.000000 tables_io-0.9.6/src/tables_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 03:06:23.000000 tables_io-0.9.6/src/tables_io.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-25 03:06:23.000000 tables_io-0.9.6/src/tables_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 03:06:23.000000 tables_io-0.9.6/src/tables_io.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:06:23.229872 tables_io-0.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-25 03:06:14.000000 tables_io-0.9.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:06:23.229872 tables_io-0.9.6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-04-25 03:06:14.000000 tables_io-0.9.6/tests/data/no_groupname_test.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     9104 2024-04-25 03:06:14.000000 tables_io-0.9.6/tests/data/pandas_test_hdf5.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-04-25 03:06:14.000000 tables_io-0.9.6/tests/data/parquet_test.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-25 03:06:14.000000 tables_io-0.9.6/tests/test_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-04-25 03:06:14.000000 tables_io-0.9.6/tests/test_fileIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-04-25 03:06:14.000000 tables_io-0.9.6/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-25 03:06:14.000000 tables_io-0.9.6/tests/test_table_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-25 03:06:14.000000 tables_io-0.9.6/tests/test_utils.py
```

### Comparing `tables-io-0.9.5/.github/ISSUE_TEMPLATE/1-bug_report.md` & `tables_io-0.9.6/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/.github/ISSUE_TEMPLATE/2-feature_request.md` & `tables_io-0.9.6/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/.github/pull_request_template.md` & `tables_io-0.9.6/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/.github/workflows/linting.yml` & `tables_io-0.9.6/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/.github/workflows/publish-to-pypi.yml` & `tables_io-0.9.6/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/.github/workflows/smoke-test.yml` & `tables_io-0.9.6/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/.github/workflows/testing-and-coverage.yml` & `tables_io-0.9.6/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/.gitignore` & `tables_io-0.9.6/.gitignore`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/.pre-commit-config.yaml` & `tables_io-0.9.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/LICENSE` & `tables_io-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/PKG-INFO` & `tables_io-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tables-io
-Version: 0.9.5
+Version: 0.9.6
 Summary: Input/output and conversion functions for tabular data
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <echarles@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2023 Eric Charles
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tables-io-0.9.5/README.md` & `tables_io-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/docs/.gitignore` & `tables_io-0.9.6/docs/.gitignore`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/docs/Makefile` & `tables_io-0.9.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/docs/conf.py` & `tables_io-0.9.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/docs/index.rst` & `tables_io-0.9.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/nb/.gitignore` & `tables_io-0.9.6/nb/.gitignore`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/nb/hdf5_iter_example.ipynb` & `tables_io-0.9.6/nb/hdf5_iter_example.ipynb`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/nb/multipleWriteHdf5_example.ipynb` & `tables_io-0.9.6/nb/multipleWriteHdf5_example.ipynb`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/nb/singleTable_example.ipynb` & `tables_io-0.9.6/nb/singleTable_example.ipynb`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/nb/tableDict_example.ipynb` & `tables_io-0.9.6/nb/tableDict_example.ipynb`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/pyproject.toml` & `tables_io-0.9.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,17 @@
     "jaxlib",
     "pre-commit", # Used to run checks before finalizing a git commit
     "sphinx", # Used to automatically generate documentation
     "sphinx_rtd_theme", # Used to render documentation
     "sphinx-autoapi", # Used to automatically generate api documentation
 ]
 
+[project.scripts]
+convert-table = "tables_io.cli:main"
+
 [build-system]
 requires = [
     "setuptools>=62", # Used to build and package the Python project
     "setuptools_scm>=6.2", # Gets release version from git. Makes it available programmatically
 ]
 build-backend = "setuptools.build_meta"
```

### Comparing `tables-io-0.9.5/src/tables_io/__init__.py` & `tables_io-0.9.6/src/tables_io/__init__.py`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/src/tables_io/arrayUtils.py` & `tables_io-0.9.6/src/tables_io/arrayUtils.py`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/src/tables_io/convUtils.py` & `tables_io-0.9.6/src/tables_io/convUtils.py`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/src/tables_io/ioUtils.py` & `tables_io-0.9.6/src/tables_io/ioUtils.py`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/src/tables_io/lazy_modules.py` & `tables_io-0.9.6/src/tables_io/lazy_modules.py`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/src/tables_io/tableDict.py` & `tables_io-0.9.6/src/tables_io/tableDict.py`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/src/tables_io/testUtils.py` & `tables_io-0.9.6/src/tables_io/testUtils.py`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/src/tables_io/types.py` & `tables_io-0.9.6/src/tables_io/types.py`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/src/tables_io.egg-info/PKG-INFO` & `tables_io-0.9.6/src/tables_io.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tables-io
-Version: 0.9.5
+Version: 0.9.6
 Summary: Input/output and conversion functions for tabular data
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <echarles@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2023 Eric Charles
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tables-io-0.9.5/src/tables_io.egg-info/SOURCES.txt` & `tables_io-0.9.6/src/tables_io.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -28,23 +28,25 @@
 nb/hdf5_iter_example.ipynb
 nb/multipleWriteHdf5_example.ipynb
 nb/singleTable_example.ipynb
 nb/tableDict_example.ipynb
 src/tables_io/__init__.py
 src/tables_io/_version.py
 src/tables_io/arrayUtils.py
+src/tables_io/cli.py
 src/tables_io/convUtils.py
 src/tables_io/ioUtils.py
 src/tables_io/lazy_modules.py
 src/tables_io/tableDict.py
 src/tables_io/testUtils.py
 src/tables_io/types.py
 src/tables_io.egg-info/PKG-INFO
 src/tables_io.egg-info/SOURCES.txt
 src/tables_io.egg-info/dependency_links.txt
+src/tables_io.egg-info/entry_points.txt
 src/tables_io.egg-info/requires.txt
 src/tables_io.egg-info/top_level.txt
 tests/conftest.py
 tests/test_conv.py
 tests/test_fileIO.py
 tests/test_io.py
 tests/test_table_dict.py
```

### Comparing `tables-io-0.9.5/tests/conftest.py` & `tables_io-0.9.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/tests/data/no_groupname_test.hdf5` & `tables_io-0.9.6/tests/data/no_groupname_test.hdf5`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/tests/data/pandas_test_hdf5.h5` & `tables_io-0.9.6/tests/data/pandas_test_hdf5.h5`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/tests/data/parquet_test.parquet` & `tables_io-0.9.6/tests/data/parquet_test.parquet`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/tests/test_conv.py` & `tables_io-0.9.6/tests/test_conv.py`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/tests/test_fileIO.py` & `tables_io-0.9.6/tests/test_fileIO.py`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/tests/test_io.py` & `tables_io-0.9.6/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/tests/test_table_dict.py` & `tables_io-0.9.6/tests/test_table_dict.py`

 * *Files identical despite different names*

### Comparing `tables-io-0.9.5/tests/test_utils.py` & `tables_io-0.9.6/tests/test_utils.py`

 * *Files identical despite different names*


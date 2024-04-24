# Comparing `tmp/aind_exaspim_pipeline_utils-0.8.0.tar.gz` & `tmp/aind_exaspim_pipeline_utils-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_exaspim_pipeline_utils-0.8.0.tar", last modified: Tue Apr  2 18:15:48 2024, max compression
+gzip compressed data, was "aind_exaspim_pipeline_utils-0.8.1.tar", last modified: Wed Apr 24 23:09:30 2024, max compression
```

## Comparing `aind_exaspim_pipeline_utils-0.8.0.tar` & `aind_exaspim_pipeline_utils-0.8.1.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.677715 aind_exaspim_pipeline_utils-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.661715 aind_exaspim_pipeline_utils-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.665715 aind_exaspim_pipeline_utils-0.8.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.665715 aind_exaspim_pipeline_utils-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/.github/workflows/lint_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-02 18:15:48.677715 aind_exaspim_pipeline_utils-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.669715 aind_exaspim_pipeline_utils-0.8.0/capsule_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/capsule_scripts/imagej_postInstall
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/capsule_scripts/imagej_run.sh
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/capsule_scripts/n5tozarr_postInstall
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/capsule_scripts/n5tozarr_run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.669715 aind_exaspim_pipeline_utils-0.8.0/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.669715 aind_exaspim_pipeline_utils-0.8.0/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.669715 aind_exaspim_pipeline_utils-0.8.0/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/doc/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/doc/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/doc/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 18:15:48.677715 aind_exaspim_pipeline_utils-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.665715 aind_exaspim_pipeline_utils-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.669715 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14493 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/exaspim_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/imagej_macros.py
--rw-r--r--   0 runner    (1001) docker     (127)    24042 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/imagej_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.673715 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/n5tozarr/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/n5tozarr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18825 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.673715 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/qc/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/qc/create_ng_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/qc/ng_ip_visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.673715 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/trigger/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27230 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/trigger/capsule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.673715 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-02 18:15:48.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-02 18:15:48.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:15:48.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-02 18:15:48.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-02 18:15:48.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 18:15:48.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.673715 aind_exaspim_pipeline_utils-0.8.0/src/aind_trigger_codeocean/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_trigger_codeocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51638 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_trigger_codeocean/pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.673715 aind_exaspim_pipeline_utils-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/tests/test_capsule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/tests/test_imagej_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/tests/test_n5tozarr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.106714 aind_exaspim_pipeline_utils-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.090714 aind_exaspim_pipeline_utils-0.8.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.094714 aind_exaspim_pipeline_utils-0.8.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.094714 aind_exaspim_pipeline_utils-0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/.github/workflows/lint_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-24 23:09:30.106714 aind_exaspim_pipeline_utils-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.098713 aind_exaspim_pipeline_utils-0.8.1/capsule_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/capsule_scripts/imagej_postInstall
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/capsule_scripts/imagej_run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/capsule_scripts/n5tozarr_postInstall
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/capsule_scripts/n5tozarr_run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.098713 aind_exaspim_pipeline_utils-0.8.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.098713 aind_exaspim_pipeline_utils-0.8.1/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.098713 aind_exaspim_pipeline_utils-0.8.1/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/doc/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/doc/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/doc/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 23:09:30.106714 aind_exaspim_pipeline_utils-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.094714 aind_exaspim_pipeline_utils-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.098713 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-24 23:09:20.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23467 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/exaspim_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/imagej_macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24042 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/imagej_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/java_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.102714 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/n5tozarr/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/n5tozarr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18825 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.102714 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/qc/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/qc/create_ng_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9689 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/qc/ng_ip_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.102714 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/trigger/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28034 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/trigger/capsule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.102714 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-24 23:09:30.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-24 23:09:30.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 23:09:30.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-24 23:09:30.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-24 23:09:30.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 23:09:30.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.102714 aind_exaspim_pipeline_utils-0.8.1/src/aind_trigger_codeocean/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_trigger_codeocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51638 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/src/aind_trigger_codeocean/pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:09:30.102714 aind_exaspim_pipeline_utils-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/tests/test_capsule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/tests/test_imagej_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-24 23:09:19.000000 aind_exaspim_pipeline_utils-0.8.1/tests/test_n5tozarr.py
```

### Comparing `aind_exaspim_pipeline_utils-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_exaspim_pipeline_utils-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_exaspim_pipeline_utils-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/.github/ISSUE_TEMPLATE/user-story.md` & `aind_exaspim_pipeline_utils-0.8.1/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/.github/workflows/lint_and_test.yml` & `aind_exaspim_pipeline_utils-0.8.1/.github/workflows/lint_and_test.yml`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/.github/workflows/tag_and_publish.yml` & `aind_exaspim_pipeline_utils-0.8.1/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/.gitignore` & `aind_exaspim_pipeline_utils-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/LICENSE` & `aind_exaspim_pipeline_utils-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/PKG-INFO` & `aind_exaspim_pipeline_utils-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_exaspim_pipeline_utils
-Version: 0.8.0
+Version: 0.8.1
 Summary: AIND exaSPIM pipeline utilities.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_exaspim_pipeline_utils-0.8.0/README.md` & `aind_exaspim_pipeline_utils-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/doc/Makefile` & `aind_exaspim_pipeline_utils-0.8.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/doc/make.bat` & `aind_exaspim_pipeline_utils-0.8.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/doc/source/_static/dark-logo.svg` & `aind_exaspim_pipeline_utils-0.8.1/doc/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/doc/source/_static/favicon.ico` & `aind_exaspim_pipeline_utils-0.8.1/doc/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/doc/source/_static/light-logo.svg` & `aind_exaspim_pipeline_utils-0.8.1/doc/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/doc/source/conf.py` & `aind_exaspim_pipeline_utils-0.8.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/pyproject.toml` & `aind_exaspim_pipeline_utils-0.8.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 imagej_wrapper = "aind_exaspim_pipeline_utils.imagej_wrapper:main"
 imagej_wrapper_manifest = "aind_exaspim_pipeline_utils.imagej_wrapper:imagej_wrapper_main"
 n5tozarr_da_converter = "aind_exaspim_pipeline_utils.n5tozarr.n5tozarr_da:n5tozarr_da_converter"
 zarr_multiscale_converter = "aind_exaspim_pipeline_utils.n5tozarr.n5tozarr_da:zarr_multiscale_converter"
 create_example_manifest = "aind_exaspim_pipeline_utils.exaspim_manifest:create_example_manifest"
 bigstitcher_log_edge_analysis = "aind_exaspim_pipeline_utils.qc.bigstitcher_log_edge_analysis:main"
 run_trigger_capsule = "aind_exaspim_pipeline_utils.trigger.capsule:capsule_main"
+java_detreg_postprocess = "aind_exaspim_pipeline_utils.java_utils:java_detreg_postprocess_main"
 
 [tool.setuptools.dynamic]
 version = {attr = "aind_exaspim_pipeline_utils.__version__"}
 
 [tool.black]
 line-length = 110
 target_version = ['py38']
```

### Comparing `aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/imagej_macros.py` & `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/imagej_macros.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/imagej_wrapper.py` & `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/imagej_wrapper.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py` & `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py` & `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/qc/create_ng_link.py` & `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/qc/create_ng_link.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/qc/ng_ip_visualization.py` & `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/qc/ng_ip_visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         translation = np.round(translation, 4)
 
         tile_positions[tile_path.name] = translation
 
     return tile_positions
 
 
-def read_in_n5_ips(tile_setupId, transform_3x4=None):
+def read_in_n5_ips(tile_setupId, transform_3x4=None):  # pragma: no cover
     """Read in intereset point coordinates from the n5 binary files.
     Interest points are not sorted.
     """
     n5s = zarr.n5.N5FSStore("../results/interestpoints.n5/")
     zg = zarr.open(store=n5s, mode="r")
 
     id = zg[f"tpId_0_viewSetupId_{tile_setupId}/beads/interestpoints/id"]
```

### Comparing `aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/trigger/capsule.py` & `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils/trigger/capsule.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,17 @@
     XMLCreationParameters,
     IJWrapperParameters,
     IPDetectionParameters,
     IPRegistrationParameters,
     ExaspimProcessingPipeline,
     N5toZarrParameters,
     ZarrMultiscaleParameters,
+    SparkInterestPointDetections,
+    SparkGeometricDescriptorMatching,
+    Solver,
 )
 
 logging.basicConfig(format="%(asctime)s %(message)s", datefmt="%Y-%m-%d %H:%M")
 logger = logging.getLogger("exaspim_trigger")
 logger.setLevel(logging.INFO)
 
 
@@ -56,32 +59,34 @@
         "--exaspim_data_uri",
         help="S3 URI Top-level location of input exaSPIM " "dataset in aind-open-data",
         required=True,
     )
     parser.add_argument(
         "--raw_data_uri",
         help="S3 URI Top-level location of input exaSPIM"
-             "dataset in aind-open-data if different from exaspim_data_uri "
-             "(ie. flat-fielded)",
+        "dataset in aind-open-data if different from exaspim_data_uri "
+        "(ie. flat-fielded)",
     )
     parser.add_argument(
         "--manifest_output_prefix_uri", help="S3 prefix URI for processing manifest upload", required=True
     )
     parser.add_argument(
         "--pipeline_timestamp",
         help="Pipeline timestamp to be appended to folder names. "
-             "Defaults to current local time as YYYY-MM-DD_HH-MM-SS",
+        "Defaults to current local time as YYYY-MM-DD_HH-MM-SS",
     )
     parser.add_argument("--template_manifest", help="Template manifest json file to override defaults.")
 
     parser.add_argument("--xml_capsule_id", help="XML converter capsule id. Runs it if present.")
     parser.add_argument("--ij_capsule_id", help="ImageJ wrapper capsule id. Starts it if present.")
-    parser.add_argument("--channel",
-                        help="Channel name to process. Must be one of the wavelengths in the metadata. "
-                             "Without the 'ch' prefix.")
+    parser.add_argument(
+        "--channel",
+        help="Channel name to process. Must be one of the wavelengths in the metadata. "
+        "Without the 'ch' prefix.",
+    )
     args = parser.parse_args()
     return args
 
 
 def get_s3_file(bucket_name: str, object_name: str, local_file: str):  # pragma: no cover
     """Download a file from S3.
 
@@ -146,16 +151,17 @@
         del metadata["exaSPIM_acquisition"]
 
     # Validate subject_id
     m = re.match(r".*exaSPIM_(\w+)_\d{4}-\d{2}-\d{2}", args.input_dataset_prefix)
     if m:
         fname_subject_id = m.group(1)
     else:
-        raise ValueError("Cannot extract subject id from the input dataset prefix {}".format(
-            args.input_dataset_prefix))
+        raise ValueError(
+            "Cannot extract subject id from the input dataset prefix {}".format(args.input_dataset_prefix)
+        )
 
     if not metadata["subject"]:
         logger.warning("No subject metadata. Using file path pattern.")
         metadata["subject"] = {"subject_id": fname_subject_id}
     else:
         meta_subject_id = metadata["subject"].get("subject_id")
         if not meta_subject_id:
@@ -181,29 +187,30 @@
 #     if meta_url.netloc != args.input_dataset_bucket_name or \
 #     meta_url.path.strip("/") != args.input_dataset_prefix:
 #         raise ValueError(
 #         "Output location of last DataProcess does not match with current dataset location")
 
 
 def register_or_get_dataset_as_CO_data_asset(
-        dataset_name, dataset_bucket, dataset_prefix, co_client
+    dataset_name, dataset_bucket, dataset_prefix, co_client
 ):  # pragma: no cover
     """Query the input dataset for existence and register it if not found.
 
     At the moment the dataset_name and dataset_prefix are the same in aind-open-data.
     """
+    logger.info(f"Query for dataset {dataset_name} in CO.")
     query_response = co_client.search_data_assets(query=f"name:{dataset_name}")
     if query_response.status_code != 200:
         raise RuntimeError("Cannot query data assets")
     query_response = query_response.json()
     results = query_response["results"]
     for r in results:
         if r["name"] == dataset_name:
             # Check that it points to the same bucket and prefix
-            sourceBucket = r.get("sourceBucket", {})
+            sourceBucket = r.get("source_bucket", {})
             if sourceBucket.get("prefix") == dataset_prefix and sourceBucket.get("bucket") == dataset_bucket:
                 logger.info(f"Found dataset {dataset_name} in CO as {r['id']}")
                 return r["id"]
     # Not found, register
     logger.info(f"Register dataset as a data asset in CO. {dataset_bucket}:{dataset_name}")
     # Register data asset
     data_configs = {"prefix": dataset_prefix, "bucket": dataset_bucket}
@@ -371,28 +378,26 @@
     if "acquisition" in metadata:
         acq = metadata["acquisition"]
         for t in acq["tiles"]:
             ch_names.append(t["channel"]["channel_name"])
     logger.info(f"Found channels in acquisition metadata: {set(ch_names)}")
     if args.channel:
         if args.channel not in ch_names:
-            raise ValueError(
-                f"Channel name {args.channel} not found in the metadata: {set(ch_names)}."
-            )
+            raise ValueError(f"Channel name {args.channel} not found in the metadata: {set(ch_names)}.")
     else:
         args.channel = ch_names[0]
     logger.info(f"Processing selected channel: {args.channel}")
     return args.channel
 
 
 def recursive_assign_items(
-        dst: Union[collections.abc.Mapping, list],
-        key_dst: Union[str, int],
-        src: Union[collections.abc.Mapping, list],
-        key_src: Union[str, int],
+    dst: Union[collections.abc.Mapping, list],
+    key_dst: Union[str, int],
+    src: Union[collections.abc.Mapping, list],
+    key_src: Union[str, int],
 ) -> None:
     """Recursively assign items between dictionaries or lists.
 
 
     If src[key_src] is a dictionary, recursively assign items from src[key_src] to dst[key_dst].
     dst[key_dst] must exist.
 
@@ -411,15 +416,15 @@
         for i in range(len(slist)):
             recursive_assign_items(dlist, i, slist, i)
     else:
         dst[key_dst] = src[key_src]
 
 
 def recursive_update_mapping(
-        dst: collections.abc.Mapping, src: collections.abc.Mapping
+    dst: collections.abc.Mapping, src: collections.abc.Mapping
 ) -> collections.abc.Mapping:
     """Recursively update a dictionary-like object.
 
     Use to override items in a parameter configuration dictionary (manifest). The overriding dictionary
     shall have the same hierarchy as the original one but only contains the entries to override.
 
     If a list item is to be updated, the overriding dictionary shall contain a list of the same length and
@@ -452,14 +457,15 @@
         find_maxima=True,
         set_minimum_maximum=True,
         minimal_intensity=0,
         maximal_intensity=2000,
         ip_limitation_choice="brightest",
         maximum_number_of_detections=150000,
     )
+
     ip_reg_translation: IPRegistrationParameters = IPRegistrationParameters(
         # dataset_xml=capsule_xml_path,
         IJwrap=def_ij_wrapper_parameters,
         transformation_choice="translation",
         compare_views_choice="overlapping_views",
         interest_point_inclusion_choice="overlapping_ips",
         fix_views_choice="select_fixed",
@@ -489,24 +495,46 @@
     )
 
     zarr_multiscale: ZarrMultiscaleParameters = ZarrMultiscaleParameters(
         voxel_size_zyx=(1.0, 0.748, 0.748),
         input_uri=f"s3://{args.fusion_output_bucket}/{args.fusion_output_prefix}/fused.zarr/",
     )
 
-    xml_creation: XMLCreationParameters = XMLCreationParameters(ch_name=ch_name,
-                                                                input_uri=args.exaspim_data_uri)
+    xml_creation: XMLCreationParameters = XMLCreationParameters(
+        ch_name=ch_name, input_uri=args.exaspim_data_uri
+    )
 
     processing_manifest: ExaspimProcessingPipeline = ExaspimProcessingPipeline(
         creation_time=args.pipeline_timestamp,
         pipeline_suffix=args.fname_timestamp,
         subject_id=metadata["subject"].get("subject_id"),
         name=metadata["data_description"].get("name"),
         xml_creation=xml_creation,
         ip_detection=def_ip_detection_parameters,
+        spark_ip_detections=SparkInterestPointDetections(overlappingOnly=True),
+        spark_geometric_descriptor_matching_tr=SparkGeometricDescriptorMatching(
+            clearCorrespondences=True,
+            transformationModel="TRANSLATION",
+            regularizationModel="NONE",
+        ),
+        solver_tr=Solver(
+            transformationModel="TRANSLATION",
+            regularizationModel="NONE",
+            fixedViews=["0,7"],
+        ),
+        spark_geometric_descriptor_matching_aff=SparkGeometricDescriptorMatching(
+            clearCorrespondences=True,
+            transformationModel="AFFINE",
+            regularizationModel="RIGID",
+        ),
+        solver_aff=Solver(
+            transformationModel="AFFINE",
+            regularizationModel="RIGID",
+            fixedViews=["0,7"],
+        ),
         ip_registrations=[ip_reg_translation, ip_reg_affine],
         n5_to_zarr=n5_to_zarr,
         zarr_multiscale=zarr_multiscale,
     )
     if args.template_manifest:
         logger.info(f"Overriding manifest entries from {args.template_manifest}")
         with open(args.template_manifest, "r") as f:
@@ -517,22 +545,22 @@
 
     return processing_manifest
 
 
 def create_and_upload_emr_config(args, manifest: ExaspimProcessingPipeline):  # pragma: no cover
     """Create EMR command line parameters for the fusion of the present alignment run."""
     config = (
-        f"[\"-x\", \"{args.alignment_output_uri}"
-        f"bigstitcher_emr_{manifest.subject_id}_{manifest.pipeline_suffix}_0.xml\",\n"
-        f"\"--outS3Bucket\", \"{args.fusion_output_bucket}\", "
-        f"\"-o\", \"/{args.fusion_output_prefix}/fused.n5\",\n"
-        f"\"--bdv\", \"0,0\", "
-        f"\"--xmlout\", \"s3://{args.fusion_output_bucket}/{args.fusion_output_prefix}/fused.xml\", "
-        "\"--storage\", \"N5\", \"--UINT16\", \"--minIntensity=0\", "
-        "\"--maxIntensity=65535\", \"--preserveAnisotropy\" ]\n"
+        f'["-x", "{args.alignment_output_uri}'
+        f'bigstitcher_emr_{manifest.subject_id}_{manifest.pipeline_suffix}_0.xml",\n'
+        f'"--outS3Bucket", "{args.fusion_output_bucket}", '
+        f'"-o", "/{args.fusion_output_prefix}/fused.n5",\n'
+        f'"--bdv", "0,0", '
+        f'"--xmlout", "s3://{args.fusion_output_bucket}/{args.fusion_output_prefix}/fused.xml", '
+        '"--storage", "N5", "--UINT16", "--minIntensity=0", '
+        '"--maxIntensity=65535", "--preserveAnisotropy" ]\n'
     )
     with open("../results/emr_fusion_config.txt", "w") as f:
         f.write(config)
     logger.info("Uploading emr_fusion_config.txt to bucket {}".format(args.manifest_bucket_name))
     s3 = boto3.client("s3")  # Authentication should be available in the environment
     object_name = "/".join((args.manifest_path, "emr_fusion_config.txt"))
     s3.upload_file("../results/emr_fusion_config.txt", args.manifest_bucket_name, object_name)
```

### Comparing `aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO` & `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_exaspim_pipeline_utils
-Version: 0.8.0
+Version: 0.8.1
 Summary: AIND exaSPIM pipeline utilities.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt` & `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 doc/source/_static/dark-logo.svg
 doc/source/_static/favicon.ico
 doc/source/_static/light-logo.svg
 src/aind_exaspim_pipeline_utils/__init__.py
 src/aind_exaspim_pipeline_utils/exaspim_manifest.py
 src/aind_exaspim_pipeline_utils/imagej_macros.py
 src/aind_exaspim_pipeline_utils/imagej_wrapper.py
+src/aind_exaspim_pipeline_utils/java_utils.py
 src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO
 src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt
 src/aind_exaspim_pipeline_utils.egg-info/dependency_links.txt
 src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt
 src/aind_exaspim_pipeline_utils.egg-info/requires.txt
 src/aind_exaspim_pipeline_utils.egg-info/top_level.txt
 src/aind_exaspim_pipeline_utils/n5tozarr/__init__.py
```

### Comparing `aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt` & `aind_exaspim_pipeline_utils-0.8.1/src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 [console_scripts]
 bigstitcher_log_edge_analysis = aind_exaspim_pipeline_utils.qc.bigstitcher_log_edge_analysis:main
 create_example_manifest = aind_exaspim_pipeline_utils.exaspim_manifest:create_example_manifest
 imagej_wrapper = aind_exaspim_pipeline_utils.imagej_wrapper:main
 imagej_wrapper_manifest = aind_exaspim_pipeline_utils.imagej_wrapper:imagej_wrapper_main
+java_detreg_postprocess = aind_exaspim_pipeline_utils.java_utils:java_detreg_postprocess_main
 n5tozarr_da_converter = aind_exaspim_pipeline_utils.n5tozarr.n5tozarr_da:n5tozarr_da_converter
 run_trigger_capsule = aind_exaspim_pipeline_utils.trigger.capsule:capsule_main
 zarr_multiscale_converter = aind_exaspim_pipeline_utils.n5tozarr.n5tozarr_da:zarr_multiscale_converter
```

### Comparing `aind_exaspim_pipeline_utils-0.8.0/src/aind_trigger_codeocean/pipelines.py` & `aind_exaspim_pipeline_utils-0.8.1/src/aind_trigger_codeocean/pipelines.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/tests/test_capsule.py` & `aind_exaspim_pipeline_utils-0.8.1/tests/test_capsule.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/tests/test_imagej_wrapper.py` & `aind_exaspim_pipeline_utils-0.8.1/tests/test_imagej_wrapper.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.0/tests/test_n5tozarr.py` & `aind_exaspim_pipeline_utils-0.8.1/tests/test_n5tozarr.py`

 * *Files identical despite different names*


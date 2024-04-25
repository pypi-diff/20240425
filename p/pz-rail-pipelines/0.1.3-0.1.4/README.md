# Comparing `tmp/pz-rail-pipelines-0.1.3.tar.gz` & `tmp/pz_rail_pipelines-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-pipelines-0.1.3.tar", last modified: Tue Oct 31 22:23:52 2023, max compression
+gzip compressed data, was "pz_rail_pipelines-0.1.4.tar", last modified: Thu Apr 25 01:55:57 2024, max compression
```

## Comparing `pz-rail-pipelines-0.1.3.tar` & `pz_rail_pipelines-0.1.4.tar`

### file list

```diff
@@ -1,56 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:23:52.950015 pz-rail-pipelines-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:23:52.938015 pz-rail-pipelines-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:23:52.938015 pz-rail-pipelines-0.1.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:23:52.938015 pz-rail-pipelines-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      957 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/.prepare_project.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2023-10-31 22:23:52.946015 pz-rail-pipelines-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:23:52.934014 pz-rail-pipelines-0.1.3/nb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:23:52.942015 pz-rail-pipelines-0.1.3/nb/estimation/
--rw-r--r--   0 runner    (1001) docker     (127)    14274 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/nb/estimation/estimate_all.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12116 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/nb/estimation/estimate_all_hsc.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8190 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/nb/estimation/inform_all.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/nb/estimation/inform_all_hsc.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:23:52.934014 pz-rail-pipelines-0.1.3/nb/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:23:52.942015 pz-rail-pipelines-0.1.3/nb/examples/goldenspike/
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/nb/examples/goldenspike/goldenspike.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-31 22:23:52.950015 pz-rail-pipelines-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:23:52.934014 pz-rail-pipelines-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:23:52.942015 pz-rail-pipelines-0.1.3/src/pz_rail_pipelines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2023-10-31 22:23:52.000000 pz-rail-pipelines-0.1.3/src/pz_rail_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2023-10-31 22:23:52.000000 pz-rail-pipelines-0.1.3/src/pz_rail_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 22:23:52.000000 pz-rail-pipelines-0.1.3/src/pz_rail_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      384 2023-10-31 22:23:52.000000 pz-rail-pipelines-0.1.3/src/pz_rail_pipelines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-31 22:23:52.000000 pz-rail-pipelines-0.1.3/src/pz_rail_pipelines.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:23:52.934014 pz-rail-pipelines-0.1.3/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:23:52.942015 pz-rail-pipelines-0.1.3/src/rail/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/src/rail/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-31 22:23:52.000000 pz-rail-pipelines-0.1.3/src/rail/pipelines/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:23:52.942015 pz-rail-pipelines-0.1.3/src/rail/pipelines/estimation/
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/src/rail/pipelines/estimation/estimate_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/src/rail/pipelines/estimation/inform_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:23:52.934014 pz-rail-pipelines-0.1.3/src/rail/pipelines/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:23:52.942015 pz-rail-pipelines-0.1.3/src/rail/pipelines/examples/goldenspike/
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/src/rail/pipelines/examples/goldenspike/goldenspike.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:23:52.942015 pz-rail-pipelines-0.1.3/src/rail/pipelines/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/src/rail/pipelines/utils/name_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:23:52.942015 pz-rail-pipelines-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2023-10-31 22:23:35.000000 pz-rail-pipelines-0.1.3/tests/test_pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.225616 pz_rail_pipelines-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.217615 pz_rail_pipelines-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.217615 pz_rail_pipelines-0.1.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.217615 pz_rail_pipelines-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.prepare_project.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-25 01:55:57.225616 pz_rail_pipelines-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.213616 pz_rail_pipelines-0.1.4/nb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.221615 pz_rail_pipelines-0.1.4/nb/estimation/
+-rw-r--r--   0 runner    (1001) docker     (127)    14274 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/nb/estimation/estimate_all.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12116 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/nb/estimation/estimate_all_hsc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/nb/estimation/inform_all.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/nb/estimation/inform_all_hsc.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.213616 pz_rail_pipelines-0.1.4/nb/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.221615 pz_rail_pipelines-0.1.4/nb/examples/goldenspike/
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/nb/examples/goldenspike/goldenspike.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.221615 pz_rail_pipelines-0.1.4/nb/examples/survey_nonuniformity/
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/nb/examples/survey_nonuniformity/survey_nonuniform.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 01:55:57.225616 pz_rail_pipelines-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.213616 pz_rail_pipelines-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.221615 pz_rail_pipelines-0.1.4/src/pz_rail_pipelines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-25 01:55:57.000000 pz_rail_pipelines-0.1.4/src/pz_rail_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-25 01:55:57.000000 pz_rail_pipelines-0.1.4/src/pz_rail_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 01:55:57.000000 pz_rail_pipelines-0.1.4/src/pz_rail_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-25 01:55:57.000000 pz_rail_pipelines-0.1.4/src/pz_rail_pipelines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 01:55:57.000000 pz_rail_pipelines-0.1.4/src/pz_rail_pipelines.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.213616 pz_rail_pipelines-0.1.4/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.221615 pz_rail_pipelines-0.1.4/src/rail/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/src/rail/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 01:55:56.000000 pz_rail_pipelines-0.1.4/src/rail/pipelines/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.221615 pz_rail_pipelines-0.1.4/src/rail/pipelines/estimation/
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/src/rail/pipelines/estimation/estimate_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/src/rail/pipelines/estimation/inform_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.217615 pz_rail_pipelines-0.1.4/src/rail/pipelines/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.221615 pz_rail_pipelines-0.1.4/src/rail/pipelines/examples/goldenspike/
+-rw-r--r--   0 runner    (1001) docker     (127)     7686 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/src/rail/pipelines/examples/goldenspike/goldenspike.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.221615 pz_rail_pipelines-0.1.4/src/rail/pipelines/examples/survey_nonuniformity/
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/src/rail/pipelines/examples/survey_nonuniformity/survey_nonuniformity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.221615 pz_rail_pipelines-0.1.4/src/rail/pipelines/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/src/rail/pipelines/utils/name_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.221615 pz_rail_pipelines-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/tests/test_pipelines.py
```

### Comparing `pz-rail-pipelines-0.1.3/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_pipelines-0.1.4/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.1.3/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_pipelines-0.1.4/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.1.3/.github/pull_request_template.md` & `pz_rail_pipelines-0.1.4/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.1.3/.github/workflows/linting.yml` & `pz_rail_pipelines-0.1.4/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.1.3/.github/workflows/publish-to-pypi.yml` & `pz_rail_pipelines-0.1.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.1.3/.github/workflows/testing-and-coverage.yml` & `pz_rail_pipelines-0.1.4/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.1.3/.gitignore` & `pz_rail_pipelines-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.1.3/.pre-commit-config.yaml` & `pz_rail_pipelines-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.1.3/.prepare_project.sh` & `pz_rail_pipelines-0.1.4/.prepare_project.sh`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.1.3/LICENSE` & `pz_rail_pipelines-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.1.3/README.md` & `pz_rail_pipelines-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.1.3/nb/estimation/estimate_all.ipynb` & `pz_rail_pipelines-0.1.4/nb/estimation/estimate_all.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.1.3/nb/estimation/estimate_all_hsc.ipynb` & `pz_rail_pipelines-0.1.4/nb/estimation/estimate_all_hsc.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.1.3/nb/estimation/inform_all.ipynb` & `pz_rail_pipelines-0.1.4/nb/estimation/inform_all.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.1.3/nb/estimation/inform_all_hsc.ipynb` & `pz_rail_pipelines-0.1.4/nb/estimation/inform_all_hsc.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.1.3/nb/examples/goldenspike/goldenspike.ipynb` & `pz_rail_pipelines-0.1.4/nb/examples/goldenspike/goldenspike.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.1.3/pyproject.toml` & `pz_rail_pipelines-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -19,38 +19,19 @@
 dependencies = [
     "pz-rail-base",
 ]
 
 # On a mac, install optional dependencies with `pip install '.[dev]'` (include the single quotes)
 [project.optional-dependencies]
 full = [
-    "pz-rail-astro-tools",
-    "pz-rail-bpz",
-    "pz-rail-cmnn",
-    "pz-rail-dsps",
-    "pz-rail-flexzboost",
-    "pz-rail-fsps",
-    "pz-rail-gpz-v1",
-    "pz-rail-pzflow",
-    "pz-rail-sklearn",
-    "pz-rail-som",
-    "qp-prob[full]",
+    "pz-rail[algos]",
 ]
 
 dev = [
-    "pz-rail-astro-tools",
-    "pz-rail-bpz",
-    "pz-rail-dsps",
-    "pz-rail-flexzboost",
-    "pz-rail-fsps",
-    "pz-rail-gpz-v1",
-    "pz-rail-pzflow",
-    "pz-rail-sklearn",
-    "pz-rail-som",
-    "qp-prob[full]",
+    "pz-rail[algos]",
     "coverage",
     "pytest",
     "pytest-cov", # Used to report total code coverage
     "pre-commit", # Used to run checks before finalizing a git commit
     "pylint", # Used for static linting of files
 ]
```

### Comparing `pz-rail-pipelines-0.1.3/src/pz_rail_pipelines.egg-info/SOURCES.txt` & `pz_rail_pipelines-0.1.4/src/pz_rail_pipelines.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,19 +19,21 @@
 .github/workflows/smoke-test.yml
 .github/workflows/testing-and-coverage.yml
 nb/estimation/estimate_all.ipynb
 nb/estimation/estimate_all_hsc.ipynb
 nb/estimation/inform_all.ipynb
 nb/estimation/inform_all_hsc.ipynb
 nb/examples/goldenspike/goldenspike.ipynb
+nb/examples/survey_nonuniformity/survey_nonuniform.ipynb
 src/pz_rail_pipelines.egg-info/PKG-INFO
 src/pz_rail_pipelines.egg-info/SOURCES.txt
 src/pz_rail_pipelines.egg-info/dependency_links.txt
 src/pz_rail_pipelines.egg-info/requires.txt
 src/pz_rail_pipelines.egg-info/top_level.txt
 src/rail/pipelines/__init__.py
 src/rail/pipelines/_version.py
 src/rail/pipelines/estimation/estimate_all.py
 src/rail/pipelines/estimation/inform_all.py
 src/rail/pipelines/examples/goldenspike/goldenspike.py
+src/rail/pipelines/examples/survey_nonuniformity/survey_nonuniformity.py
 src/rail/pipelines/utils/name_factory.py
 tests/test_pipelines.py
```

### Comparing `pz-rail-pipelines-0.1.3/src/rail/pipelines/estimation/estimate_all.py` & `pz_rail_pipelines-0.1.4/src/rail/pipelines/estimation/estimate_all.py`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.1.3/src/rail/pipelines/estimation/inform_all.py` & `pz_rail_pipelines-0.1.4/src/rail/pipelines/estimation/inform_all.py`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.1.3/src/rail/pipelines/examples/goldenspike/goldenspike.py` & `pz_rail_pipelines-0.1.4/src/rail/pipelines/examples/goldenspike/goldenspike.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             n_samples=50,
             seed=1235,
             output=os.path.join(namer.get_data_dir(DataType.catalog, CatalogType.created), "output_flow_engine_train.pq"),
         )
 
         self.lsst_error_model_train = LSSTErrorModel.build(
             connections=dict(input=self.flow_engine_train.io.output),    
-            bandNames=band_dict, seed=29,
+            renameDict=band_dict, seed=29,
             output=os.path.join(namer.get_data_dir(DataType.catalog, CatalogType.degraded), "output_lsst_error_model_train.pq"),
         )
 
         self.inv_redshift = InvRedshiftIncompleteness.build(
             connections=dict(input=self.lsst_error_model_train.io.output),
             pivot_redshift=1.0,
             output=os.path.join(namer.get_data_dir(DataType.catalog, CatalogType.degraded), "output_inv_redshift.pq"),
@@ -148,21 +148,22 @@
             nondetect_val=np.nan,
             hdf5_groupname='',
             output=os.path.join(namer.get_data_dir(DataType.pdf, PdfType.pz), "output_estimate_FZBoost.hdf5"),
         )
 
         eval_dict = dict(bpz=self.estimate_bpz, fzboost=self.estimate_fzboost, knn=self.estimate_knn)
         for key, val in eval_dict.items():
-            the_eval = Evaluator.make_and_connect(
-                name=f'{key}_eval',
+            the_eval = DistToPointEvaluator.make_and_connect(
+                name=f'{key}_dist_to_point',
                 connections=dict(
                     input=val.io.output,
                     truth=self.flow_engine_train.io.output,
                 ),
                 output=os.path.join(namer.get_data_dir(DataType.pdf, PdfType.pz), f"output_{key}_eval.pq"),
+                force_exact=True,
             )
             self.add_stage(the_eval)
 
         self.point_estimate_test = PointEstHistSummarizer.build(
             connections=dict(input=self.estimate_bpz.io.output),
             output=os.path.join(namer.get_data_dir(DataType.pdf, PdfType.nz), "output_point_estimate_test.hdf5"),
             single_NZ=os.path.join(namer.get_data_dir(DataType.pdf, PdfType.nz), "single_NZ_point_estimate_test.hdf5"),
```

### Comparing `pz-rail-pipelines-0.1.3/src/rail/pipelines/utils/name_factory.py` & `pz_rail_pipelines-0.1.4/src/rail/pipelines/utils/name_factory.py`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.1.3/tests/test_pipelines.py` & `pz_rail_pipelines-0.1.4/tests/test_pipelines.py`

 * *Files identical despite different names*


# Comparing `tmp/ppx-1.4.2.tar.gz` & `tmp/ppx-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppx-1.4.2.tar", last modified: Tue Apr 16 17:45:46 2024, max compression
+gzip compressed data, was "ppx-1.4.4.tar", last modified: Thu Apr 25 07:08:17 2024, max compression
```

## Comparing `ppx-1.4.2.tar` & `ppx-1.4.4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.650948 ppx-1.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.638948 ppx-1.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.642948 ppx-1.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-16 17:45:31.000000 ppx-1.4.2/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-16 17:45:31.000000 ppx-1.4.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-16 17:45:31.000000 ppx-1.4.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-16 17:45:31.000000 ppx-1.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-16 17:45:31.000000 ppx-1.4.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-16 17:45:31.000000 ppx-1.4.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-16 17:45:31.000000 ppx-1.4.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-16 17:45:31.000000 ppx-1.4.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-16 17:45:31.000000 ppx-1.4.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-16 17:45:31.000000 ppx-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-16 17:45:46.650948 ppx-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-16 17:45:31.000000 ppx-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.642948 ppx-1.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.642948 ppx-1.4.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    28123 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/_static/ppx_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    14258 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/ann_solo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.646948 ppx-1.4.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/api/functions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/api/massive.rst
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/api/pride.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-16 17:45:31.000000 ppx-1.4.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.646948 ppx-1.4.2/ppx/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-16 17:45:31.000000 ppx-1.4.2/ppx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-16 17:45:31.000000 ppx-1.4.2/ppx/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-16 17:45:31.000000 ppx-1.4.2/ppx/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-04-16 17:45:31.000000 ppx-1.4.2/ppx/ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-16 17:45:31.000000 ppx-1.4.2/ppx/massive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-16 17:45:31.000000 ppx-1.4.2/ppx/ppx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-16 17:45:31.000000 ppx-1.4.2/ppx/pride.py
--rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-04-16 17:45:31.000000 ppx-1.4.2/ppx/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-16 17:45:31.000000 ppx-1.4.2/ppx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.650948 ppx-1.4.2/ppx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-16 17:45:46.000000 ppx-1.4.2/ppx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-16 17:45:46.000000 ppx-1.4.2/ppx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:45:46.000000 ppx-1.4.2/ppx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 17:45:46.000000 ppx-1.4.2/ppx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-16 17:45:46.000000 ppx-1.4.2/ppx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 17:45:46.000000 ppx-1.4.2/ppx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-16 17:45:31.000000 ppx-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:45:46.650948 ppx-1.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.646948 ppx-1.4.2/static/
--rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-16 17:45:31.000000 ppx-1.4.2/static/ppx_light.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.646948 ppx-1.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.646948 ppx-1.4.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/data/params.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11126 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/data/pride_files_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/data/pride_project_response.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.646948 ppx-1.4.2/tests/system_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/system_tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:46.650948 ppx-1.4.2/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/unit_tests/test_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/unit_tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/unit_tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/unit_tests/test_find_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/unit_tests/test_list_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/unit_tests/test_massive.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/unit_tests/test_pride.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/unit_tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-16 17:45:31.000000 ppx-1.4.2/tests/unit_tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:17.066643 ppx-1.4.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:17.054643 ppx-1.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:17.058643 ppx-1.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-25 07:08:06.000000 ppx-1.4.4/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-25 07:08:06.000000 ppx-1.4.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-25 07:08:06.000000 ppx-1.4.4/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-25 07:08:06.000000 ppx-1.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-25 07:08:06.000000 ppx-1.4.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-25 07:08:06.000000 ppx-1.4.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-25 07:08:06.000000 ppx-1.4.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-25 07:08:06.000000 ppx-1.4.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-25 07:08:06.000000 ppx-1.4.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-25 07:08:06.000000 ppx-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-25 07:08:17.066643 ppx-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-25 07:08:06.000000 ppx-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:17.058643 ppx-1.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-25 07:08:06.000000 ppx-1.4.4/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-25 07:08:06.000000 ppx-1.4.4/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-25 07:08:06.000000 ppx-1.4.4/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-25 07:08:06.000000 ppx-1.4.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:17.058643 ppx-1.4.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-25 07:08:06.000000 ppx-1.4.4/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    28123 2024-04-25 07:08:06.000000 ppx-1.4.4/docs/_static/ppx_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14258 2024-04-25 07:08:06.000000 ppx-1.4.4/docs/ann_solo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:17.062643 ppx-1.4.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-25 07:08:06.000000 ppx-1.4.4/docs/api/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-25 07:08:06.000000 ppx-1.4.4/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-25 07:08:06.000000 ppx-1.4.4/docs/api/massive.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-25 07:08:06.000000 ppx-1.4.4/docs/api/pride.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-25 07:08:06.000000 ppx-1.4.4/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-25 07:08:06.000000 ppx-1.4.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-25 07:08:06.000000 ppx-1.4.4/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-25 07:08:06.000000 ppx-1.4.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-25 07:08:06.000000 ppx-1.4.4/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:17.062643 ppx-1.4.4/ppx/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-25 07:08:06.000000 ppx-1.4.4/ppx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-25 07:08:06.000000 ppx-1.4.4/ppx/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-25 07:08:06.000000 ppx-1.4.4/ppx/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-04-25 07:08:06.000000 ppx-1.4.4/ppx/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-25 07:08:06.000000 ppx-1.4.4/ppx/massive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-25 07:08:06.000000 ppx-1.4.4/ppx/ppx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-25 07:08:06.000000 ppx-1.4.4/ppx/pride.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-04-25 07:08:06.000000 ppx-1.4.4/ppx/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-25 07:08:06.000000 ppx-1.4.4/ppx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:17.066643 ppx-1.4.4/ppx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-25 07:08:17.000000 ppx-1.4.4/ppx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-25 07:08:17.000000 ppx-1.4.4/ppx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:08:17.000000 ppx-1.4.4/ppx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-25 07:08:17.000000 ppx-1.4.4/ppx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-25 07:08:17.000000 ppx-1.4.4/ppx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 07:08:17.000000 ppx-1.4.4/ppx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-25 07:08:06.000000 ppx-1.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 07:08:17.066643 ppx-1.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:17.062643 ppx-1.4.4/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-25 07:08:06.000000 ppx-1.4.4/static/ppx_light.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:17.062643 ppx-1.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:06.000000 ppx-1.4.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-04-25 07:08:06.000000 ppx-1.4.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:17.062643 ppx-1.4.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-25 07:08:06.000000 ppx-1.4.4/tests/data/params.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11126 2024-04-25 07:08:06.000000 ppx-1.4.4/tests/data/pride_files_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-25 07:08:06.000000 ppx-1.4.4/tests/data/pride_project_response.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:17.066643 ppx-1.4.4/tests/system_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-25 07:08:06.000000 ppx-1.4.4/tests/system_tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:17.066643 ppx-1.4.4/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:06.000000 ppx-1.4.4/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-25 07:08:06.000000 ppx-1.4.4/tests/unit_tests/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-25 07:08:06.000000 ppx-1.4.4/tests/unit_tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-25 07:08:06.000000 ppx-1.4.4/tests/unit_tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-25 07:08:06.000000 ppx-1.4.4/tests/unit_tests/test_find_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-25 07:08:06.000000 ppx-1.4.4/tests/unit_tests/test_list_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-25 07:08:06.000000 ppx-1.4.4/tests/unit_tests/test_massive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-25 07:08:06.000000 ppx-1.4.4/tests/unit_tests/test_pride.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-25 07:08:06.000000 ppx-1.4.4/tests/unit_tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-25 07:08:06.000000 ppx-1.4.4/tests/unit_tests/utils.py
```

### Comparing `ppx-1.4.2/.github/workflows/lint.yml` & `ppx-1.4.4/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/.github/workflows/publish.yml` & `ppx-1.4.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/.github/workflows/tests.yml` & `ppx-1.4.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/.gitignore` & `ppx-1.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/CHANGELOG.md` & `ppx-1.4.4/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog for ppx
 
 ## [Unreleased]
 
+## [1.4.4]
+- Fix links to MassIVE `ccms_peak` files. See [this issue](https://github.com/CCMS-UCSD/MassIVEDocumentation/issues/30#issue) for details.
+
+## [1.4.3]
+### Fixed
+- MassIVE and PRIDE links...again
+
 ## [1.4.2]
 ### Fixed
 - Fix Test status badge.
 
 ## [1.4.1]
 ### Fixed
 - Updated the ReadTheDocs configuration.
```

### Comparing `ppx-1.4.2/CODE_OF_CONDUCT.md` & `ppx-1.4.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/CONTRIBUTING.md` & `ppx-1.4.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/LICENSE` & `ppx-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/PKG-INFO` & `ppx-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppx
-Version: 1.4.2
+Version: 1.4.4
 Summary: A Python interface to proteomics data repostitories.
 Author-email: "William E. Fondrie" <fondriew@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/wfondrie/ppx
 Project-URL: Documentation, https://ppx.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ppx-1.4.2/README.md` & `ppx-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/docs/CHANGELOG.md` & `ppx-1.4.4/docs/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog for ppx
 
 ## [Unreleased]
 
+## [1.4.4]
+- Fix links to MassIVE `ccms_peak` files. See [this issue](https://github.com/CCMS-UCSD/MassIVEDocumentation/issues/30#issue) for details.
+
+## [1.4.3]
+### Fixed
+- MassIVE and PRIDE links...again
+
 ## [1.4.2]
 ### Fixed
 - Fix Test status badge.
 
 ## [1.4.1]
 ### Fixed
 - Updated the ReadTheDocs configuration.
```

### Comparing `ppx-1.4.2/docs/CODE_OF_CONDUCT.md` & `ppx-1.4.4/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/docs/CONTRIBUTING.md` & `ppx-1.4.4/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/docs/Makefile` & `ppx-1.4.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/docs/_static/custom.css` & `ppx-1.4.4/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/docs/_static/ppx_dark.png` & `ppx-1.4.4/docs/_static/ppx_dark.png`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/docs/ann_solo.ipynb` & `ppx-1.4.4/docs/ann_solo.ipynb`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/docs/api/index.rst` & `ppx-1.4.4/docs/api/index.rst`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/docs/conf.py` & `ppx-1.4.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/docs/examples.rst` & `ppx-1.4.4/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/docs/index.rst` & `ppx-1.4.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/docs/usage.rst` & `ppx-1.4.4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/ppx/__init__.py` & `ppx-1.4.4/ppx/__init__.py`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/ppx/config.py` & `ppx-1.4.4/ppx/config.py`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/ppx/factory.py` & `ppx-1.4.4/ppx/factory.py`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/ppx/ftp.py` & `ppx-1.4.4/ppx/ftp.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,41 +65,42 @@
         self.max_depth = max_depth
         self.max_reconnects = max_reconnects
         self.timeout = timeout
         self._files = None
         self._dirs = None
         self._depth = 0
 
-    def _connect(self):
+    def _connect(self, path=None):
         """Connect to the FTP server"""
         if self.connection is not None and self.connection.file is None:
             self.connection.close()
             self.connection = None
 
         if self.connection is None:
             self.connection = FTP(timeout=self.timeout)
             self.connection.connect(self.server)
             self.connection.login()
-            self.connection.cwd(self.path)
+            self.connection.cwd(self.path if path is None else path)
 
-    def connect(self):
+    def connect(self, path=None):
         """Connect to the FTP server, with reconnects on failure."""
-        self._with_reconnects(self._connect)
+        self._with_reconnects(self._connect, path=path)
 
     def quit(self):
         """Close the connection."""
         if self.connection is not None:
             self.connection.close()
             self.connection = None
 
     def _with_reconnects(self, func, *args, **kwargs):
         """Try and execute a function, reconnecting on failure."""
+        path = kwargs.get("path", None)
         for _ in range(self.max_reconnects):
             try:
-                self._connect()
+                self._connect(path)
                 return func(*args, **kwargs)
 
             except (
                 TimeoutError,
                 ConnectionRefusedError,
                 ConnectionResetError,
                 socket.gaierror,
@@ -131,15 +132,22 @@
             The local file.
         silent : bool
             Disable the progress bar?
         force_ : bool
             Force the file to be redownloaded, even if it exists.
 
         """
-        self.connect()
+        if remote_file.startswith("ccms_peak"):
+            # Special case for: https://github.com/CCMS-UCSD/MassIVEDocumentation/issues/30#issue
+            path = "z01/" + self.path.split("/", 1)[1]
+        else:
+            path = None
+
+        self.connect(path)
+
         size = self.connection.size(remote_file)
         pbar = tqdm(
             desc=str(remote_file),
             total=size,
             position=1,
             unit="b",
             unit_divisor=1024,
```

### Comparing `ppx-1.4.2/ppx/massive.py` & `ppx-1.4.4/ppx/massive.py`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/ppx/ppx.py` & `ppx-1.4.4/ppx/ppx.py`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/ppx/pride.py` & `ppx-1.4.4/ppx/pride.py`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/ppx/project.py` & `ppx-1.4.4/ppx/project.py`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/ppx/utils.py` & `ppx-1.4.4/ppx/utils.py`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/ppx.egg-info/PKG-INFO` & `ppx-1.4.4/ppx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppx
-Version: 1.4.2
+Version: 1.4.4
 Summary: A Python interface to proteomics data repostitories.
 Author-email: "William E. Fondrie" <fondriew@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/wfondrie/ppx
 Project-URL: Documentation, https://ppx.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ppx-1.4.2/ppx.egg-info/SOURCES.txt` & `ppx-1.4.4/ppx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/pyproject.toml` & `ppx-1.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/static/ppx_light.svg` & `ppx-1.4.4/static/ppx_light.svg`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/tests/conftest.py` & `ppx-1.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/tests/data/params.xml` & `ppx-1.4.4/tests/data/params.xml`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/tests/data/pride_files_response.json` & `ppx-1.4.4/tests/data/pride_files_response.json`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/tests/data/pride_project_response.json` & `ppx-1.4.4/tests/data/pride_project_response.json`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/tests/system_tests/test_cli.py` & `ppx-1.4.4/tests/system_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/tests/unit_tests/test_cloud.py` & `ppx-1.4.4/tests/unit_tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/tests/unit_tests/test_config.py` & `ppx-1.4.4/tests/unit_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/tests/unit_tests/test_download.py` & `ppx-1.4.4/tests/unit_tests/test_download.py`

 * *Files 10% similar despite different names*

```diff
@@ -108,7 +108,20 @@
     txt = proj.download(fname, force_=True)
     new_size, new_mtime = utils.sig(local_txt)
     assert orig_sig[0] == new_size
     assert orig_sig[1] != new_mtime
 
     proj.timeout = 10
     assert proj._parser_state is None
+
+
+def test_massive_ccms_peak(tmp_path):
+    """Test a ccms_peak file."""
+    # TODO: Find a smaller file.
+    proj = ppx.MassiveProject("MSV000080544")
+    files = proj.local_files()
+    assert files == []
+
+    fname = "ccms_peak/RAW/01709a_GA9-TUM_second_pool_1_01_01-ETD-1h-R2.mzXML"
+    proj.download(fname)
+    files = proj.local_files()
+    assert len(files) > 0
```

### Comparing `ppx-1.4.2/tests/unit_tests/test_find_project.py` & `ppx-1.4.4/tests/unit_tests/test_find_project.py`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/tests/unit_tests/test_list_projects.py` & `ppx-1.4.4/tests/unit_tests/test_list_projects.py`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/tests/unit_tests/test_massive.py` & `ppx-1.4.4/tests/unit_tests/test_massive.py`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/tests/unit_tests/test_pride.py` & `ppx-1.4.4/tests/unit_tests/test_pride.py`

 * *Files identical despite different names*

### Comparing `ppx-1.4.2/tests/unit_tests/test_utils.py` & `ppx-1.4.4/tests/unit_tests/test_utils.py`

 * *Files identical despite different names*


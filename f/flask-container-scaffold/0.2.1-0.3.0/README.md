# Comparing `tmp/flask-container-scaffold-0.2.1.tar.gz` & `tmp/flask_container_scaffold-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-container-scaffold-0.2.1.tar", last modified: Thu Feb  8 13:46:22 2024, max compression
+gzip compressed data, was "flask_container_scaffold-0.3.0.tar", last modified: Thu Apr 25 11:04:53 2024, max compression
```

## Comparing `flask-container-scaffold-0.2.1.tar` & `flask_container_scaffold-0.3.0.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:46:22.522551 flask-container-scaffold-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:46:22.514551 flask-container-scaffold-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:46:22.518551 flask-container-scaffold-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/.mergify.yml
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-02-08 13:46:22.522551 flask-container-scaffold-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/dist-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:46:22.518551 flask-container-scaffold-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/docs/flask_container_scaffold.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/docs-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-02-08 13:46:22.526551 flask-container-scaffold-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:46:22.514551 flask-container-scaffold-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:46:22.518551 flask-container-scaffold-0.2.1/src/flask_container_scaffold/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/src/flask_container_scaffold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/src/flask_container_scaffold/app_configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/src/flask_container_scaffold/app_scaffold.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/src/flask_container_scaffold/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/src/flask_container_scaffold/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/src/flask_container_scaffold/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/src/flask_container_scaffold/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:46:22.522551 flask-container-scaffold-0.2.1/src/flask_container_scaffold.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-02-08 13:46:22.000000 flask-container-scaffold-0.2.1/src/flask_container_scaffold.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-08 13:46:22.000000 flask-container-scaffold-0.2.1/src/flask_container_scaffold.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 13:46:22.000000 flask-container-scaffold-0.2.1/src/flask_container_scaffold.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-02-08 13:46:22.000000 flask-container-scaffold-0.2.1/src/flask_container_scaffold.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-08 13:46:22.000000 flask-container-scaffold-0.2.1/src/flask_container_scaffold.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:46:22.518551 flask-container-scaffold-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:46:22.522551 flask-container-scaffold-0.2.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/tests/data/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:46:22.522551 flask-container-scaffold-0.2.1/tests/data/custom/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/tests/data/custom/bad_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/tests/data/custom/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/tests/data/custom/extra.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/tests/data/custom/has_includes.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/tests/data/extra.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/tests/data/settings.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:46:22.522551 flask-container-scaffold-0.2.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/tests/unit/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/tests/unit/test_scaffold.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/tests/unit/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 13:46:22.522551 flask-container-scaffold-0.2.1/tooling/
--rwxr-xr-x   0 runner    (1001) docker     (127)      342 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/tooling/build_changelog
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-02-08 13:45:43.000000 flask-container-scaffold-0.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:53.402754 flask_container_scaffold-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:53.390754 flask_container_scaffold-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:53.394754 flask_container_scaffold-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-04-25 11:04:53.402754 flask_container_scaffold-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)     9173 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/dist-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:53.394754 flask_container_scaffold-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/docs/flask_container_scaffold.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-25 11:04:53.402754 flask_container_scaffold-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:53.390754 flask_container_scaffold-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:53.394754 flask_container_scaffold-0.3.0/src/flask_container_scaffold/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/src/flask_container_scaffold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/src/flask_container_scaffold/app_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/src/flask_container_scaffold/app_scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/src/flask_container_scaffold/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/src/flask_container_scaffold/base_scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/src/flask_container_scaffold/celery_scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/src/flask_container_scaffold/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/src/flask_container_scaffold/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/src/flask_container_scaffold/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:53.398754 flask_container_scaffold-0.3.0/src/flask_container_scaffold.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-04-25 11:04:53.000000 flask_container_scaffold-0.3.0/src/flask_container_scaffold.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-25 11:04:53.000000 flask_container_scaffold-0.3.0/src/flask_container_scaffold.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 11:04:53.000000 flask_container_scaffold-0.3.0/src/flask_container_scaffold.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-25 11:04:53.000000 flask_container_scaffold-0.3.0/src/flask_container_scaffold.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 11:04:53.000000 flask_container_scaffold-0.3.0/src/flask_container_scaffold.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:53.398754 flask_container_scaffold-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:53.398754 flask_container_scaffold-0.3.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/tests/data/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:53.398754 flask_container_scaffold-0.3.0/tests/data/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/tests/data/custom/bad_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/tests/data/custom/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/tests/data/custom/extra.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/tests/data/custom/has_includes.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/tests/data/extra.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/tests/data/settings.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:53.398754 flask_container_scaffold-0.3.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/tests/unit/test_celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/tests/unit/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/tests/unit/test_scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/tests/unit/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:04:53.398754 flask_container_scaffold-0.3.0/tooling/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      342 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/tooling/build_changelog
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-25 11:04:09.000000 flask_container_scaffold-0.3.0/tox.ini
```

### Comparing `flask-container-scaffold-0.2.1/.github/workflows/publish.yml` & `flask_container_scaffold-0.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `flask-container-scaffold-0.2.1/.github/workflows/test.yml` & `flask_container_scaffold-0.3.0/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   pull_request:
     branches: [ main ]
 jobs:
     test:
       runs-on: ubuntu-latest
       strategy:
         matrix:
-          python: ['3.7', '3.8', '3.9', '3.10', '3.11']
+          python: ['3.8', '3.9', '3.10', '3.11', '3.12']
       steps:
         - uses: actions/checkout@v3
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
             python-version: ${{ matrix.python }}
         - name: Install Tox and any other packages
@@ -25,15 +25,15 @@
     flake8:
       runs-on: ubuntu-latest
       steps:
         - uses: actions/checkout@v3
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-            python-version: 3.11
+            python-version: 3.12
         - name: Install Tox and any other packages
           run: |
             python -m pip install --upgrade pip
             pip install tox tox-gh-actions
         - name: Lint with flake8
           run: tox -eflake8
     twine:
@@ -41,14 +41,14 @@
       steps:
         - uses: actions/checkout@v3
           with:
             fetch-depth: 0
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-            python-version: 3.11
+            python-version: 3.12
         - name: Install Tox and any other packages
           run: |
             python -m pip install --upgrade pip
             pip install tox tox-gh-actions
         - name: Run twine-check
           run: tox -etwine
```

### Comparing `flask-container-scaffold-0.2.1/.gitignore` & `flask_container_scaffold-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `flask-container-scaffold-0.2.1/LICENSE` & `flask_container_scaffold-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-container-scaffold-0.2.1/PKG-INFO` & `flask_container_scaffold-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,7 @@
-Metadata-Version: 2.1
-Name: flask-container-scaffold
-Version: 0.2.1
-Summary: Configuration layer to aid in deployment of Flask apps
-Home-page: https://github.com/release-depot/flask-container-scaffold
-Author: Jason Guiditta
-Author-email: jason.guiditta@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/release-depot/flask-container-scaffold/issues
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: flask
-Requires-Dist: pydantic
-Requires-Dist: toolchest
-Provides-Extra: devbase
-Requires-Dist: tox; extra == "devbase"
-Provides-Extra: test
-Requires-Dist: flake8; extra == "test"
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
-Provides-Extra: docs
-Requires-Dist: sphinx==4.3.1; extra == "docs"
-Requires-Dist: sphinx-autobuild==2021.3.14; extra == "docs"
-Requires-Dist: sphinx-rtd-theme==0.5.2; extra == "docs"
-Requires-Dist: myst-parser==0.15.2; extra == "docs"
-Provides-Extra: dist
-Requires-Dist: build; extra == "dist"
-Requires-Dist: setuptools_scm; extra == "dist"
-Requires-Dist: twine; extra == "dist"
-
 ## flask-container-scaffold
 
 [![pypi](https://img.shields.io/pypi/v/flask-container-scaffold.svg)](https://pypi.python.org/pypi/flask-container-scaffold)
 [![tests](https://github.com/release-depot/flask-container-scaffold/actions/workflows/test.yml/badge.svg)](https://github.com/release-depot/flask-container-scaffold/actions/workflows/test.yml)
 [![documentation](https://readthedocs.org/projects/flask-container-scaffold/badge/?version=latest)](https://flask-container-scaffold.readthedocs.io/en/latest/?badge=latest)
 
 A common base layer for Flask applications that are deployed in containers.
@@ -161,14 +125,59 @@
         },
         'root': {
             'level': 'WARNING',
             'handlers': ['wsgi', 'file'],
         },
     })
 
+### CeleryScaffold
+
+This class has all of the same support as the above AppScaffold and takes
+the same parameters. Each CeleryScaffold instance has a flask_app and celery_app
+attribute that can be used in your project. More information about celery can
+be found [here](https://docs.celeryq.dev/en/stable/getting-started/introduction.html).
+Information on integrating celery with flask can be found in flask's
+[documentation](https://flask.palletsprojects.com/en/2.3.x/patterns/celery/).
+
+
+#### Installation
+
+    pip install flask-container-scaffold['celery']
+
+or
+
+    pipenv install --categories celery
+
+#### Basic Usage
+
+    celery_scaffold = CeleryScaffold(name=__name__, config=config)
+    flask_app = celery_scaffold.flask_app
+    celery_app = celery_scaffold.celery_app
+
+#### Basic Configuration
+
+All configuration is done via a 'CELERY' key in a configuration dictionary. The
+'CELERY' element itself is a dictionary of configuration items. More details on the 
+available configuration items for celery can be found [here](https://docs.celeryq.dev/en/stable/userguide/configuration.html).
+Below is a basic example in yaml format that uses a local rabbitmq broker, json serialization, and no result backend.
+
+```
+---
+
+CELERY:
+  broker: "pyamqp://guest@127.0.0.1//"
+  result_persistent: False
+  task_serializer: "json"
+  accept_content:
+    - "json"  # Ignore other content
+  result_serializer: "json"
+  result_expires: "300"
+  broker_connection_retry_on_startup: 'False'
+```
+
 ### Using the parse_input method
 
 This method is used to validate incoming data against a pydantic model. A
 custom return type can be specifed in the case of validation failure, but
 it must extend flask_container_scaffold.BaseApiView, or minimally implement a
 field 'errors' of type dict, so that the parse_input method can properly
 populate it on a failure.
```

### Comparing `flask-container-scaffold-0.2.1/README.md` & `flask_container_scaffold-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,45 @@
+Metadata-Version: 2.1
+Name: flask-container-scaffold
+Version: 0.3.0
+Summary: Configuration layer to aid in deployment of Flask apps
+Home-page: https://github.com/release-depot/flask-container-scaffold
+Author: Jason Guiditta
+Author-email: jason.guiditta@gmail.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/release-depot/flask-container-scaffold/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: flask
+Requires-Dist: pydantic
+Requires-Dist: toolchest
+Provides-Extra: celery
+Requires-Dist: celery; extra == "celery"
+Provides-Extra: devbase
+Requires-Dist: tox; extra == "devbase"
+Provides-Extra: test
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-autobuild; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: myst-parser; extra == "docs"
+Provides-Extra: dist
+Requires-Dist: build; extra == "dist"
+Requires-Dist: setuptools_scm; extra == "dist"
+Requires-Dist: twine; extra == "dist"
+
 ## flask-container-scaffold
 
 [![pypi](https://img.shields.io/pypi/v/flask-container-scaffold.svg)](https://pypi.python.org/pypi/flask-container-scaffold)
 [![tests](https://github.com/release-depot/flask-container-scaffold/actions/workflows/test.yml/badge.svg)](https://github.com/release-depot/flask-container-scaffold/actions/workflows/test.yml)
 [![documentation](https://readthedocs.org/projects/flask-container-scaffold/badge/?version=latest)](https://flask-container-scaffold.readthedocs.io/en/latest/?badge=latest)
 
 A common base layer for Flask applications that are deployed in containers.
@@ -125,14 +163,59 @@
         },
         'root': {
             'level': 'WARNING',
             'handlers': ['wsgi', 'file'],
         },
     })
 
+### CeleryScaffold
+
+This class has all of the same support as the above AppScaffold and takes
+the same parameters. Each CeleryScaffold instance has a flask_app and celery_app
+attribute that can be used in your project. More information about celery can
+be found [here](https://docs.celeryq.dev/en/stable/getting-started/introduction.html).
+Information on integrating celery with flask can be found in flask's
+[documentation](https://flask.palletsprojects.com/en/2.3.x/patterns/celery/).
+
+
+#### Installation
+
+    pip install flask-container-scaffold['celery']
+
+or
+
+    pipenv install --categories celery
+
+#### Basic Usage
+
+    celery_scaffold = CeleryScaffold(name=__name__, config=config)
+    flask_app = celery_scaffold.flask_app
+    celery_app = celery_scaffold.celery_app
+
+#### Basic Configuration
+
+All configuration is done via a 'CELERY' key in a configuration dictionary. The
+'CELERY' element itself is a dictionary of configuration items. More details on the 
+available configuration items for celery can be found [here](https://docs.celeryq.dev/en/stable/userguide/configuration.html).
+Below is a basic example in yaml format that uses a local rabbitmq broker, json serialization, and no result backend.
+
+```
+---
+
+CELERY:
+  broker: "pyamqp://guest@127.0.0.1//"
+  result_persistent: False
+  task_serializer: "json"
+  accept_content:
+    - "json"  # Ignore other content
+  result_serializer: "json"
+  result_expires: "300"
+  broker_connection_retry_on_startup: 'False'
+```
+
 ### Using the parse_input method
 
 This method is used to validate incoming data against a pydantic model. A
 custom return type can be specifed in the case of validation failure, but
 it must extend flask_container_scaffold.BaseApiView, or minimally implement a
 field 'errors' of type dict, so that the parse_input method can properly
 populate it on a failure.
```

### Comparing `flask-container-scaffold-0.2.1/docs/Makefile` & `flask_container_scaffold-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flask-container-scaffold-0.2.1/docs/conf.py` & `flask_container_scaffold-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `flask-container-scaffold-0.2.1/docs/flask_container_scaffold.rst` & `flask_container_scaffold-0.3.0/docs/flask_container_scaffold.rst`

 * *Files 20% similar despite different names*

```diff
@@ -3,23 +3,41 @@
 
 .. automodule:: flask_container_scaffold.app_configurator
    :members:
    :special-members: __init__
    :undoc-members:
    :show-inheritance:
 
+BaseScaffold
+------------
+
+.. automodule:: flask_container_scaffold.base_scaffold
+   :members:
+   :special-members: __init__
+   :undoc-members:
+   :show-inheritance:
+
 AppScaffold
 -----------
 
 .. automodule:: flask_container_scaffold.app_scaffold
    :members:
    :special-members: __init__
    :undoc-members:
    :show-inheritance:
 
+CeleryScaffold
+--------------
+
+.. automodule:: flask_container_scaffold.celery_scaffold
+   :members:
+   :special-members: __init__
+   :undoc-members:
+   :show-inheritance:
+
 FlaskRequestFormatter
 ---------------------
 
 .. automodule:: flask_container_scaffold.logging
    :members:
    :special-members: __init__
    :undoc-members:
```

### Comparing `flask-container-scaffold-0.2.1/docs/make.bat` & `flask_container_scaffold-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flask-container-scaffold-0.2.1/setup.cfg` & `flask_container_scaffold-0.3.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -24,25 +24,27 @@
 packages = find:
 install_requires = 
 	flask
 	pydantic
 	toolchest
 
 [options.extras_require]
+celery = 
+	celery
 devbase = 
 	tox
 test = 
 	flake8
 	pytest
 	pytest-cov
 docs = 
-	sphinx==4.3.1
-	sphinx-autobuild==2021.3.14
-	sphinx-rtd-theme==0.5.2
-	myst-parser==0.15.2
+	sphinx
+	sphinx-autobuild
+	sphinx-rtd-theme
+	myst-parser
 dist = 
 	build
 	setuptools_scm
 	twine
 
 [options.packages.find]
 where = src
```

### Comparing `flask-container-scaffold-0.2.1/src/flask_container_scaffold/app_configurator.py` & `flask_container_scaffold-0.3.0/src/flask_container_scaffold/app_configurator.py`

 * *Files identical despite different names*

### Comparing `flask-container-scaffold-0.2.1/src/flask_container_scaffold/app_scaffold.py` & `flask_container_scaffold-0.3.0/src/flask_container_scaffold/base_scaffold.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import os
 
 from flask import Flask
 
 from flask_container_scaffold.app_configurator import AppConfigurator
 
 
-class AppScaffold(object):
+class BaseScaffold(object):
 
     def __init__(self, app=None,
                  name=__name__, config=None,
                  settings_required=False,
                  instance_path=None,
                  instance_relative_config=True):
         """
-        This class provides a way to dynamically configure a Flask application.
+        This base class provides a way to dynamically configure a Flask
+        application.
 
         :param obj app: An existing Flask application, if passed, otherwise we
             will create a new one
         :param str name: The name of the application, defaults to __name__.
         :param dict config: A dict of configuration details. This can include
             standard Flask configuration keys, like 'TESTING', or
-            'CUSTOM_SETTINGS' (which can be a string referencing a file with custom
-            configuration, or a dictionary containing any values your application
-            may need) to make them available to the application during runtime
+            'CUSTOM_SETTINGS' (which can be a string referencing a file with
+            custom configuration, or a dictionary containing any values your
+            application may need) to make them available to the application
+            during runtime
         :param bool settings_required: Whether your app requires certain
             settings be specified in a settings.cfg file
         :param str instance_path: Passthrough parameter to flask. An
             alternative instance path for the application. By default
             the folder 'instance' next to the package or module is
             assumed to be the instance path.
         :param bool instance_relative_config: Passthrough parameter to flask.
@@ -37,18 +39,19 @@
         """
         # TODO: Consider taking **kwargs here, so we can automatically support
         # all params the flask object takes, and just pass them through.  Keep
         # the ones we already have, as they are needed for the current code to
         # work.
         Flask.jinja_options = dict(Flask.jinja_options, trim_blocks=True,
                                    lstrip_blocks=True)
-        self.app = (app or
-                    Flask(name,
-                          instance_relative_config=instance_relative_config,
-                          instance_path=instance_path))
+        self.flask_app = app or Flask(
+            name,
+            instance_relative_config=instance_relative_config,
+            instance_path=instance_path,
+        )
         self.config = config
         self.silent = not settings_required
         self.relative = instance_relative_config
         self._init_app()
 
     def _init_app(self):
         self._load_flask_settings()
@@ -62,37 +65,38 @@
         - via config mapping
         - via Flask settings.cfg file
         - via environment variable 'FLASK_SETTINGS'
         """
         config_not_loaded = True
         if self.config is not None:
             # load the config if passed in
-            self.app.config.from_mapping(self.config)
+            self.flask_app.config.from_mapping(self.config)
             config_not_loaded = False
         # load the instance config, if it exists and/or is required
         try:
-            self.app.config.from_pyfile('settings.cfg', silent=self.silent)
+            self.flask_app.config.from_pyfile('settings.cfg',
+                                              silent=self.silent)
             config_not_loaded = False
         except Exception:
             config_not_loaded = True
         # Load any additional config specified in the FLASK_SETTINGS file,
         # if it exists. We only want to fail in the case where settings are
         # required by the app.
         if ((config_not_loaded and not self.silent) or
                 os.environ.get('FLASK_SETTINGS')):
-            self.app.config.from_envvar('FLASK_SETTINGS')
+            self.flask_app.config.from_envvar('FLASK_SETTINGS')
 
     def _load_custom_settings(self):
         """
         Load any custom configuration for the app from:
         - app.config['CUSTOM_SETTINGS']
         - environment variable 'CUSTOM_SETTINGS'
         """
-        configurator = AppConfigurator(self.app, self.relative)
-        if self.app.config.get('CUSTOM_SETTINGS') is not None:
+        configurator = AppConfigurator(self.flask_app, self.relative)
+        if self.flask_app.config.get('CUSTOM_SETTINGS') is not None:
             # load the config if passed in
-            custom = self.app.config.get('CUSTOM_SETTINGS')
+            custom = self.flask_app.config.get('CUSTOM_SETTINGS')
             configurator.parse(custom)
         # Next, load from override file, if specified
         if os.environ.get('CUSTOM_SETTINGS') is not None:
             custom = os.environ.get('CUSTOM_SETTINGS')
             configurator.parse(custom)
```

### Comparing `flask-container-scaffold-0.2.1/src/flask_container_scaffold/base.py` & `flask_container_scaffold-0.3.0/src/flask_container_scaffold/base.py`

 * *Files identical despite different names*

### Comparing `flask-container-scaffold-0.2.1/src/flask_container_scaffold/logging.py` & `flask_container_scaffold-0.3.0/src/flask_container_scaffold/logging.py`

 * *Files identical despite different names*

### Comparing `flask-container-scaffold-0.2.1/src/flask_container_scaffold/network.py` & `flask_container_scaffold-0.3.0/src/flask_container_scaffold/network.py`

 * *Files identical despite different names*

### Comparing `flask-container-scaffold-0.2.1/src/flask_container_scaffold/util.py` & `flask_container_scaffold-0.3.0/src/flask_container_scaffold/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
 
 def parse_input(logger, obj, default_return=BaseApiView):
     """
     Parses incoming request, returns a serializable object to return
     to the client in all cases. When there is a failure, the
     object contains error information.
+
     :param Logger logger: Instantiated logger object
     :param BaseModel obj: An object type based on a pydantic BaseModel to
                           attempt to parse.
     :param BaseApiView default_return: An object type that will be returned if
                                        validation of obj fails. This object
                                        must descend from BaseApiView or
                                        implement an errors field of type dict.
```

### Comparing `flask-container-scaffold-0.2.1/src/flask_container_scaffold.egg-info/PKG-INFO` & `flask_container_scaffold-0.3.0/src/flask_container_scaffold.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-container-scaffold
-Version: 0.2.1
+Version: 0.3.0
 Summary: Configuration layer to aid in deployment of Flask apps
 Home-page: https://github.com/release-depot/flask-container-scaffold
 Author: Jason Guiditta
 Author-email: jason.guiditta@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/release-depot/flask-container-scaffold/issues
 Classifier: Development Status :: 3 - Alpha
@@ -14,25 +14,27 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: flask
 Requires-Dist: pydantic
 Requires-Dist: toolchest
+Provides-Extra: celery
+Requires-Dist: celery; extra == "celery"
 Provides-Extra: devbase
 Requires-Dist: tox; extra == "devbase"
 Provides-Extra: test
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: docs
-Requires-Dist: sphinx==4.3.1; extra == "docs"
-Requires-Dist: sphinx-autobuild==2021.3.14; extra == "docs"
-Requires-Dist: sphinx-rtd-theme==0.5.2; extra == "docs"
-Requires-Dist: myst-parser==0.15.2; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-autobuild; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: myst-parser; extra == "docs"
 Provides-Extra: dist
 Requires-Dist: build; extra == "dist"
 Requires-Dist: setuptools_scm; extra == "dist"
 Requires-Dist: twine; extra == "dist"
 
 ## flask-container-scaffold
 
@@ -161,14 +163,59 @@
         },
         'root': {
             'level': 'WARNING',
             'handlers': ['wsgi', 'file'],
         },
     })
 
+### CeleryScaffold
+
+This class has all of the same support as the above AppScaffold and takes
+the same parameters. Each CeleryScaffold instance has a flask_app and celery_app
+attribute that can be used in your project. More information about celery can
+be found [here](https://docs.celeryq.dev/en/stable/getting-started/introduction.html).
+Information on integrating celery with flask can be found in flask's
+[documentation](https://flask.palletsprojects.com/en/2.3.x/patterns/celery/).
+
+
+#### Installation
+
+    pip install flask-container-scaffold['celery']
+
+or
+
+    pipenv install --categories celery
+
+#### Basic Usage
+
+    celery_scaffold = CeleryScaffold(name=__name__, config=config)
+    flask_app = celery_scaffold.flask_app
+    celery_app = celery_scaffold.celery_app
+
+#### Basic Configuration
+
+All configuration is done via a 'CELERY' key in a configuration dictionary. The
+'CELERY' element itself is a dictionary of configuration items. More details on the 
+available configuration items for celery can be found [here](https://docs.celeryq.dev/en/stable/userguide/configuration.html).
+Below is a basic example in yaml format that uses a local rabbitmq broker, json serialization, and no result backend.
+
+```
+---
+
+CELERY:
+  broker: "pyamqp://guest@127.0.0.1//"
+  result_persistent: False
+  task_serializer: "json"
+  accept_content:
+    - "json"  # Ignore other content
+  result_serializer: "json"
+  result_expires: "300"
+  broker_connection_retry_on_startup: 'False'
+```
+
 ### Using the parse_input method
 
 This method is used to validate incoming data against a pydantic model. A
 custom return type can be specifed in the case of validation failure, but
 it must extend flask_container_scaffold.BaseApiView, or minimally implement a
 field 'errors' of type dict, so that the parse_input method can properly
 populate it on a failure.
```

### Comparing `flask-container-scaffold-0.2.1/tests/conftest.py` & `flask_container_scaffold-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flask-container-scaffold-0.2.1/tests/unit/test_logging.py` & `flask_container_scaffold-0.3.0/tests/unit/test_logging.py`

 * *Files identical despite different names*

### Comparing `flask-container-scaffold-0.2.1/tests/unit/test_scaffold.py` & `flask_container_scaffold-0.3.0/tests/unit/test_scaffold.py`

 * *Files identical despite different names*

### Comparing `flask-container-scaffold-0.2.1/tests/unit/test_util.py` & `flask_container_scaffold-0.3.0/tests/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `flask-container-scaffold-0.2.1/tox.ini` & `flask_container_scaffold-0.3.0/tox.ini`

 * *Files identical despite different names*


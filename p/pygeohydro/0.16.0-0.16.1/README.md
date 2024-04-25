# Comparing `tmp/pygeohydro-0.16.0.tar.gz` & `tmp/pygeohydro-0.16.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeohydro-0.16.0.tar", last modified: Wed Jan  3 23:00:44 2024, max compression
+gzip compressed data, was "pygeohydro-0.16.1.tar", last modified: Thu Apr 25 03:22:07 2024, max compression
```

## Comparing `pygeohydro-0.16.0.tar` & `pygeohydro-0.16.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 23:00:44.566000 pygeohydro-0.16.0/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/.deepsource.toml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 23:00:44.558000 pygeohydro-0.16.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 23:00:44.562000 pygeohydro-0.16.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/.github/ISSUE_TEMPLATE/bugreport.yml
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/.github/ISSUE_TEMPLATE/newfeature.yml
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 23:00:44.562000 pygeohydro-0.16.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/.sonarcloud.properties
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34948 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    22915 2024-01-03 23:00:44.566000 pygeohydro-0.16.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20737 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 23:00:44.554000 pygeohydro-0.16.0/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 23:00:44.562000 pygeohydro-0.16.0/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/ci/requirements/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/ci/requirements/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 23:00:44.566000 pygeohydro-0.16.0/pygeohydro/
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/pygeohydro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/pygeohydro/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/pygeohydro/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/pygeohydro/nfhl.py
--rw-r--r--   0 runner    (1001) docker     (127)    16497 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/pygeohydro/nlcd.py
--rw-r--r--   0 runner    (1001) docker     (127)    26929 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/pygeohydro/nwis.py
--rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/pygeohydro/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/pygeohydro/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/pygeohydro/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    35192 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/pygeohydro/pygeohydro.py
--rw-r--r--   0 runner    (1001) docker     (127)    24754 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/pygeohydro/stnfloodevents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/pygeohydro/us_abbrs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/pygeohydro/waterdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/pygeohydro/watershed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 23:00:44.566000 pygeohydro-0.16.0/pygeohydro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22915 2024-01-03 23:00:44.000000 pygeohydro-0.16.0/pygeohydro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-01-03 23:00:44.000000 pygeohydro-0.16.0/pygeohydro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 23:00:44.000000 pygeohydro-0.16.0/pygeohydro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 23:00:44.000000 pygeohydro-0.16.0/pygeohydro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-01-03 23:00:44.000000 pygeohydro-0.16.0/pygeohydro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-03 23:00:44.000000 pygeohydro-0.16.0/pygeohydro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-03 23:00:44.566000 pygeohydro-0.16.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 23:00:44.566000 pygeohydro-0.16.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    33690 2024-01-03 23:00:31.000000 pygeohydro-0.16.0/tests/test_pygeohydro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:07.670975 pygeohydro-0.16.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/.deepsource.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:07.662975 pygeohydro-0.16.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:07.662975 pygeohydro-0.16.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/.github/ISSUE_TEMPLATE/bugreport.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/.github/ISSUE_TEMPLATE/newfeature.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:07.662975 pygeohydro-0.16.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/.sonarcloud.properties
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35646 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    22915 2024-04-25 03:22:07.670975 pygeohydro-0.16.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20737 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:07.658975 pygeohydro-0.16.1/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:07.662975 pygeohydro-0.16.1/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/ci/requirements/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/ci/requirements/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:07.666975 pygeohydro-0.16.1/pygeohydro/
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/pygeohydro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/pygeohydro/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/pygeohydro/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/pygeohydro/nfhl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16436 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/pygeohydro/nlcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27551 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/pygeohydro/nwis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/pygeohydro/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/pygeohydro/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/pygeohydro/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    36316 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/pygeohydro/pygeohydro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24697 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/pygeohydro/stnfloodevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/pygeohydro/us_abbrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14950 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/pygeohydro/waterdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/pygeohydro/watershed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:07.670975 pygeohydro-0.16.1/pygeohydro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22915 2024-04-25 03:22:07.000000 pygeohydro-0.16.1/pygeohydro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-25 03:22:07.000000 pygeohydro-0.16.1/pygeohydro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 03:22:07.000000 pygeohydro-0.16.1/pygeohydro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 03:22:07.000000 pygeohydro-0.16.1/pygeohydro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-25 03:22:07.000000 pygeohydro-0.16.1/pygeohydro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 03:22:07.000000 pygeohydro-0.16.1/pygeohydro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 03:22:07.670975 pygeohydro-0.16.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:07.666975 pygeohydro-0.16.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33731 2024-04-25 03:21:55.000000 pygeohydro-0.16.1/tests/test_pygeohydro.py
```

### Comparing `pygeohydro-0.16.0/.github/ISSUE_TEMPLATE/bugreport.yml` & `pygeohydro-0.16.1/.github/ISSUE_TEMPLATE/bugreport.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.0/.github/ISSUE_TEMPLATE/newfeature.yml` & `pygeohydro-0.16.1/.github/ISSUE_TEMPLATE/newfeature.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.0/.github/workflows/codeql-analysis.yml` & `pygeohydro-0.16.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.0/.github/workflows/release.yml` & `pygeohydro-0.16.1/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
           --wrap=none
           -t markdown
           -o ${{ github.workflow }}-CHANGELOG.md
     - name: Remove extra spaces
       run: |-
         sed -i 's/-   /- /g' ${{ github.workflow }}-CHANGELOG.md
     - name: Github Release
-      uses: softprops/action-gh-release@v1
+      uses: softprops/action-gh-release@v2
       if: startsWith(github.ref, 'refs/tags/')
       with:
         body_path: ${{ github.workflow }}-CHANGELOG.md
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
   build:
@@ -81,8 +81,8 @@
           echo "❌ INVALID VERSION NUMBER"
           exit 1
         else
           echo "✅ Looks good"
         fi
 
     - name: Publish to PyPI
-      uses: pypa/gh-action-pypi-publish@v1.8.11
+      uses: pypa/gh-action-pypi-publish@v1.8.14
```

### Comparing `pygeohydro-0.16.0/.github/workflows/test.yml` & `pygeohydro-0.16.1/.github/workflows/test.yml`

 * *Files 5% similar despite different names*

```diff
@@ -42,28 +42,29 @@
         environment-file: ${{ env.CONDA_ENV_FILE }}
         environment-name: ${{ env.REPO_NAME }}-tests
         create-args: >-
           python=${{ env.PYTHON_VERSION }}
         cache-environment: true
         cache-environment-key: ${{runner.os}}-${{runner.arch}}-py${{env.PYTHON_VERSION}}-${{env.TODAY}}-${{hashFiles(env.CONDA_ENV_FILE)}}
     - name: Install error reporter
-      if: ${{ matrix.os }} == 'ubuntu-latest' and ${{ matrix.python-version }} == '3.11'
+      if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.11'
       run: |
         python -m pip install pytest-github-actions-annotate-failures
     - name: Install the package
       run: |-
         python -m pip install --no-deps .
     - name: Version info
       run: |-
         NAME="$(echo ${REPO_NAME} | tr - _)"
         python -c "import ${NAME}; ${NAME}.show_versions()"
     - name: Run pytest
       run: |-
         pytest
     - name: Run codecov and upload the report
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
       with:
         file: ./coverage.xml
         flags: unittests
         env_vars: RUNNER_OS,PYTHON_VERSION
         name: codecov-umbrella
         fail_ci_if_error: false
+        token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `pygeohydro-0.16.0/.gitignore` & `pygeohydro-0.16.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.0/.pre-commit-config.yaml` & `pygeohydro-0.16.1/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,39 @@
 repos:
-- repo: https://github.com/hadialqattan/pycln
-  rev: v2.4.0
-  hooks:
-  - id: pycln
-    name: Find and remove unused import statements with pycln
-    args: [--config=pyproject.toml]
-
 - repo: https://github.com/bwhmather/ssort
-  rev: v0.12.0
+  rev: 0.12.4
   hooks:
   - id: ssort
     name: Sort top level statements with ssort
 
-- repo: https://github.com/MarcoGorelli/absolufy-imports
-  rev: v0.3.1
-  hooks:
-  - id: absolufy-imports
-    name: Convert relative imports to absolute with absolufy-imports
-
 - repo: https://github.com/Instagram/Fixit
   rev: v2.1.0
   hooks:
   - id: fixit-fix
-
-- repo: https://github.com/psf/black
-  rev: 23.12.1
-  hooks:
-  - id: black
-    name: Autoformat with black
+    additional_dependencies:
+    - ufmt
 
 - repo: https://github.com/asottile/blacken-docs
   rev: 1.16.0
   hooks:
   - id: blacken-docs
     name: Autoformat codes in docstrings with blacken-docs
     additional_dependencies: [black]
     args: [-t, py38, -l, '100']
 
-- repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: v0.1.11
+- repo: https://github.com/astral-sh/ruff-pre-commit
+  rev: v0.3.5
   hooks:
   - id: ruff
     name: Linting with Ruff
-    args: [--fix, --exit-non-zero-on-fix]
+    types_or: [python]
+    args: [--fix]
+  - id: ruff-format
+    name: Formatting with Ruff
+    types_or: [python]
 
 - repo: https://github.com/PyCQA/doc8
   rev: v1.1.1
   hooks:
   - id: doc8
     name: Check documentation formats with doc8
     args: [--max-line-length, '100']
@@ -56,23 +43,23 @@
   hooks:
   - id: codespell
     name: Check common misspellings in text files with codespell.
     additional_dependencies:
     - tomli
 
 - repo: https://github.com/dosisod/refurb
-  rev: v1.26.0
+  rev: v2.0.0
   hooks:
   - id: refurb
     name: Modernizing Python codebases using Refurb
     additional_dependencies:
     - numpy
 
 - repo: https://github.com/tox-dev/pyproject-fmt
-  rev: 1.5.3
+  rev: 1.7.0
   hooks:
   - id: pyproject-fmt
     name: Apply a consistent format to pyproject.toml
 
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.5.0
   hooks:
@@ -98,19 +85,26 @@
   - id: pretty-format-json
     args: [--autofix, --no-ensure-ascii, --no-sort-keys]
   - id: trailing-whitespace
     args: [--markdown-linebreak-ext=md]
     exclude: \.(html|svg)$
 
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.12.0
+  rev: v2.13.0
   hooks:
   - id: pretty-format-yaml
     args: [--autofix, --indent, '2']
 
+- repo: https://github.com/rhysd/actionlint
+  rev: v1.6.27
+  hooks:
+  - id: actionlint
+    files: .github/workflows/
+    args: [-ignore, SC1090, -ignore, SC2046, -ignore, SC2086, -ignore, SC2129, -ignore, SC2155]
+
 - repo: local
   hooks:
   - id: future-annotations
     name: import annotations from __future__
     entry: from __future__ import annotations
     language: pygrep
     args: [--negate]
```

### Comparing `pygeohydro-0.16.0/CITATION.cff` & `pygeohydro-0.16.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.0/CODE_OF_CONDUCT.rst` & `pygeohydro-0.16.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.0/CONTRIBUTING.rst` & `pygeohydro-0.16.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.0/HISTORY.rst` & `pygeohydro-0.16.1/HISTORY.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,28 @@
 =======
 History
 =======
 
+0.16.1 (2024-04-24)
+-------------------
+
+Bug Fixes
+~~~~~~~~~
+- In ``nlcd_helper`` function the roughness value for class 82 was set to 0.16
+  instead of 0.037.
+
+New Features
+~~~~~~~~~~~~
+- Converted all methods of ``NWIS`` class to ``classmethod`` so the class can be used
+  without instantiating it. This change makes the class more flexible and easier to use.
+- In ``NID`` class, the ``stage_nid_inventory`` method now checks if the remote NID
+  database has been modified since the last download and only downloads the new data
+  if it has been modified. This change makes the method more efficient and reduces the
+  network traffic while ensuring that the local database is always up-to-date.
+
 0.16.0 (2024-01-03)
 -------------------
 
 Breaking Changes
 ~~~~~~~~~~~~~~~~
 - Bump the minimum supported version of ``shapely`` to 2.
```

### Comparing `pygeohydro-0.16.0/LICENSE` & `pygeohydro-0.16.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.0/PKG-INFO` & `pygeohydro-0.16.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeohydro
-Version: 0.16.0
+Version: 0.16.1
 Summary: Access geospatial web services that offer hydrological data
 Author-email: Taher Chegini <cheginit@gmail.com>
 License: MIT
 Project-URL: CI, https://github.com/hyriver/pygeohydro/actions
 Project-URL: Changelog, https://docs.hyriver.io/changelogs/pygeohydro.html
 Project-URL: Homepage, https://docs.hyriver.io/readme/pygeohydro.html
 Project-URL: Issues, https://github.com/hyriver/pygeohydro/issues
```

### Comparing `pygeohydro-0.16.0/README.rst` & `pygeohydro-0.16.1/README.rst`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.0/ci/requirements/environment-dev.yml` & `pygeohydro-0.16.1/ci/requirements/environment-dev.yml`

 * *Files 22% similar despite different names*

```diff
@@ -10,130 +10,149 @@
 - aiohttp-client-cache >=0.8.1
 - brotli
 - cytoolz
 - nest-asyncio
 - ujson
 
 # pygeoogc deps
-# - async-retriever>=0.15,<0.16
+# - async-retriever
 - cytoolz
 - defusedxml
 - joblib
 - multidict
-- owslib>=0.27.2
-- pyproj>=3.0.1
+- owslib >=0.27.2
+- pyproj >=3.0.1
 - requests
-- requests-cache>=0.9.6
-- shapely>=2.0.0
+- requests-cache >=0.9.6
+- shapely >=2
+- typing_extensions
 - ujson
-- url-normalize>=1.4
+- url-normalize >=1.4
 - urllib3
 - yarl
 
 # pygeoutils deps
 - cytoolz
-- geopandas-base >=0.7
+- geopandas-base >=0.10
 - fiona
 - netcdf4
 - numpy >=1.21
-- pyproj >=2.2
+- pyproj >=3.0.1
 - rasterio >=1.2
 - rioxarray >=0.11
 - scipy
 - shapely >=2.0
 - ujson
-- xarray >=2023.01.0
+- xarray >=2023.01
 
 # hydrosignatures deps
-- numpy
-- pandas
+- numpy >=1.21
+- pandas >=1
 - scipy
-- xarray
+- xarray >=2023.01
 # optional deps
 - numba
+- numbagg
 
 # py3dep
-# - async-retriever >=0.3.6
+# - async-retriever
+- click >=0.7
 - cytoolz
+- geopandas-base >=0.10
 - numpy >=1.21
-# - pygeoogc >=0.13.7
-# - pygeoutils >=0.13.7
+# - pygeoogc
+# - pygeoutils
 - rasterio >=1.2
 - rioxarray >=0.11
 - scipy
-- shapely >=2.0
-- xarray >=2023.01.0
-# optional dep
-- pyflwdir >=0.5.6
+- shapely >=2
+- xarray >=2023.01
+# optional deps
+- pyflwdir >=0.5.8
 
 # pynhd deps
-# - async-retriever >=0.3.6
+# - async-retriever
 - cytoolz
 - geopandas-base >=0.9
 - networkx
 - numpy >=1.21
 - pandas >=1.0
 - pyarrow >=1.0.1
-# - pygeoogc >=0.13.7
-# - pygeoutils >=0.13.7
+# - pygeoogc
+# - pygeoutils
 - shapely >=2.0
 # optional deps
 - pyogrio
 - py7zr
 
 # pydaymet deps
-# - async-retriever >=0.3.6
-- lxml
-- numpy >=1.21
-- pandas >=1.0
-# - py3dep >=0.13.7
-# - pygeoogc >=0.13.7
-# - pygeoutils >=0.13.9
-- rasterio >=1.2
+# - async-retriever
+- click >=0.7
+- geopandas-base >=0.10
+- numpy >=1.21
+- pandas >=1
+# - py3dep
+# - pygeoogc
+# - pygeoutils
+- pyproj >=3.0.1
 - scipy
-- shapely >=2.0
-- xarray >=2023.01.0
+- shapely >=2
+- xarray >=2023.01
 # optional deps
 - numba
 
+# pygridmet deps
+# - async-retriever
+- click >=0.7
+- geopandas-base >=0.10
+- numpy >=1.21
+- pandas >=1
+# - pygeoogc
+# - pygeoutils
+- pyproj >=3.0.1
+- shapely >=2
+- xarray >=2023.01
+
 # pygeohydro deps
+# - async-retriever
 - cytoolz
 - defusedxml
 - folium
-- geopandas-base >=0.7
+- geopandas-base >=0.10
 - h5netcdf
-# - hydrosignatures >=0.1.1
-- lxml
-- matplotlib-base >=3.5
+# - hydrosignatures
+- matplotlib >=3.5
 - numpy >=1.21
-- pandas >=1.0
-# - pygeoogc >=0.13.7
-# - pygeoutils >=0.13.9
-# - pynhd >=0.13.7
-- rasterio >=1.2
-- rioxarray >=0.11.0
+- pandas >=1
+# - pygeoogc
+# - pygeoutils
+# - pynhd
+- pyproj >=3.0.1
+- rioxarray >=0.11
 - scipy
-- shapely >=2.0
-- xarray >=2023.01.0
+- shapely >=2
+- ujson
+- xarray >=2023.01
 # optional deps
 - planetary-computer
 - pystac-client
+- pyogrio
 
 # pynldas2
-# - async-retriever >=0.3.6
+# - async-retriever
 - h5netcdf
 - numpy >=1.21
 - pandas >=1.0
-# - pygeoutils >=0.13.10
-- pyproj >=2.2
+# - pygeoutils
+- pyproj >=3.0.1
 - rioxarray >=0.11
 - xarray >=2023.01.0
 
 # optional deps for speeding up some operations
-- bottleneck
+- flox
 
 # Other deps required by example notebooks
 - mapclassify
 - contextily
 - hvplot
 - osmnx
 - tqdm
@@ -159,9 +178,10 @@
   - git+https://github.com/hyriver/async-retriever.git
   - git+https://github.com/hyriver/hydrosignatures.git
   - git+https://github.com/hyriver/pygeoogc.git
   - git+https://github.com/hyriver/pygeoutils.git
   - git+https://github.com/hyriver/pynhd.git
   - git+https://github.com/hyriver/py3dep.git
   - git+https://github.com/hyriver/pydaymet.git
+  - git+https://github.com/hyriver/pygridmet.git
   - git+https://github.com/hyriver/pynldas2.git
   - git+https://github.com/hyriver/pygeohydro.git
```

### Comparing `pygeohydro-0.16.0/ci/requirements/environment.yml` & `pygeohydro-0.16.1/ci/requirements/environment.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.0/noxfile.py` & `pygeohydro-0.16.1/noxfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nox sessions."""
+
 from __future__ import annotations
 
 import shutil
 from pathlib import Path
 
 import nox
 
@@ -109,14 +110,15 @@
     session.notify("cover")
     if speedup_dep:
         session.notify("speedup")
 
 
 @nox.session(python=python_versions)
 def speedup(session: nox.Session) -> None:
+    """Run tests that require speedup deps."""
     extras = get_extras()
     install_deps(session, ",".join(["test", *extras]))
     session.run("pytest", "--doctest-modules", "-m", "speedup", *session.posargs)
 
 
 @nox.session
 def cover(session: nox.Session) -> None:
```

### Comparing `pygeohydro-0.16.0/pygeohydro/__init__.py` & `pygeohydro-0.16.1/pygeohydro/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 """Top-level package for PyGeoHydro."""
+
+from __future__ import annotations
+
 from importlib.metadata import PackageNotFoundError, version
 
 from pygeohydro import helpers, plot
 from pygeohydro.exceptions import (
     DataNotAvailableError,
     DependencyError,
     InputRangeError,
```

### Comparing `pygeohydro-0.16.0/pygeohydro/exceptions.py` & `pygeohydro-0.16.1/pygeohydro/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Customized PyGeoHydro exceptions."""
+
 from __future__ import annotations
 
 from typing import Generator, Sequence
 
 import async_retriever as ar
 import pygeoogc as ogc
 
@@ -27,25 +28,27 @@
     """
 
     def __init__(self, missing: list[str]) -> None:
         self.message = f"The following columns are missing:\n{', '.join(missing)}"
         super().__init__(self.message)
 
     def __str__(self) -> str:
+        """Return the error message."""
         return self.message
 
 
 class MissingCRSError(Exception):
     """Exception raised when input GeoDataFrame is missing CRS."""
 
     def __init__(self) -> None:
         self.message = "The input GeoDataFrame is missing CRS."
         super().__init__(self.message)
 
     def __str__(self) -> str:
+        """Return the error message."""
         return self.message
 
 
 class ServiceUnavailableError(ogc.ServiceUnavailableError):
     """Exception raised when the service is not available.
 
     Parameters
@@ -65,14 +68,15 @@
     """
 
     def __init__(self, data_name: str) -> None:
         self.message = f"{data_name.capitalize()} is not available for the requested query."
         super().__init__(self.message)
 
     def __str__(self) -> str:
+        """Return the error message."""
         return self.message
 
 
 class InputValueError(Exception):
     """Exception raised for invalid input.
 
     Parameters
@@ -95,14 +99,15 @@
             self.message = f"Given {inp} is invalid. Valid options are:\n"
         else:
             self.message = f"Given {inp} ({given}) is invalid. Valid options are:\n"
         self.message += "\n".join(str(i) for i in valid_inputs)
         super().__init__(self.message)
 
     def __str__(self) -> str:
+        """Return the error message."""
         return self.message
 
 
 class InputRangeError(Exception):
     """Exception raised when a function argument is not in the valid range.
 
     Parameters
@@ -114,14 +119,15 @@
     """
 
     def __init__(self, database: str, rng: tuple[str, str]) -> None:
         self.message = f"{database.capitalize()} is available from {rng[0]} to {rng[1]}."
         super().__init__(self.message)
 
     def __str__(self) -> str:
+        """Return the error message."""
         return self.message
 
 
 class InputTypeError(Exception):
     """Exception raised when a function argument type is invalid.
 
     Parameters
@@ -137,14 +143,15 @@
     def __init__(self, arg: str, valid_type: str, example: str | None = None) -> None:
         self.message = f"The {arg} argument should be of type {valid_type}"
         if example is not None:
             self.message += f":\n{example}"
         super().__init__(self.message)
 
     def __str__(self) -> str:
+        """Return the error message."""
         return self.message
 
 
 class ZeroMatchedError(ValueError):
     """Exception raised when a function argument is missing.
 
     Parameters
@@ -157,14 +164,15 @@
         if msg is None:
             self.message = "Service returned no features."
         else:
             self.message = f"Service returned no features with the following error message:\n{msg}"
         super().__init__(self.message)
 
     def __str__(self) -> str:
+        """Return the error message."""
         return self.message
 
 
 class DependencyError(Exception):
     """Exception raised when a dependencies are not met.
 
     Parameters
@@ -176,8 +184,9 @@
     def __init__(self, func: str, libraries: str | list[str] | Generator[str, None, None]) -> None:
         libraries = [libraries] if isinstance(libraries, str) else libraries
         self.message = f"The following dependencies are missing for running {func}:\n"
         self.message += ", ".join(libraries)
         super().__init__(self.message)
 
     def __str__(self) -> str:
+        """Return the error message."""
         return self.message
```

### Comparing `pygeohydro-0.16.0/pygeohydro/helpers.py` & `pygeohydro-0.16.1/pygeohydro/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 """Some helper function for PyGeoHydro."""
+
 # pyright: reportGeneralTypeIssues=false
 from __future__ import annotations
 
 import io
+from dataclasses import dataclass
 from datetime import datetime
-from typing import TYPE_CHECKING, Any, NamedTuple, Tuple, Union, cast
+from typing import TYPE_CHECKING, Any, Tuple, Union, cast
 
 import cytoolz.curried as tlz
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import ujson as json
 from defusedxml import ElementTree
 
 import async_retriever as ar
 from pygeohydro import us_abbrs
-from pygeohydro.exceptions import (
-    InputRangeError,
-    InputTypeError,
-    InputValueError,
-)
+from pygeohydro.exceptions import InputRangeError, InputTypeError, InputValueError
 from pygeoogc import ServiceURL
 
 if TYPE_CHECKING:
     import pyproj
     from shapely import MultiPolygon, Polygon
 
     GTYPE = Union[Polygon, MultiPolygon, Tuple[float, float, float, float]]
@@ -41,39 +39,39 @@
         - https://www.mrlc.gov/data-services-page
         - https://www.mrlc.gov/data/legends/national-land-cover-database-2016-nlcd2016-legend
         - https://doi.org/10.1111/jfr3.12347
 
     Returns
     -------
     dict
-        Years where data is available and cover classes and categories, and roughness estimations.
+        Years when data is available and cover classes and categories, and roughness estimations.
     """
     base_url = "https://www.mrlc.gov/downloads/sciweb1/shared/mrlc/metadata"
     base_path = "eainfo/detailed/attr/attrdomv/edom"
 
     def _get_xml(
         layer: str,
     ) -> tuple[Any, Any, Any]:
-        root = ElementTree.fromstring(ar.retrieve_text([f"{base_url}/{layer}.xml"], ssl=False)[0])
+        et = ElementTree.fromstring(ar.retrieve_text([f"{base_url}/{layer}.xml"], ssl=False)[0])
         return (
-            root,
-            root.findall(f"{base_path}/edomv"),
-            root.findall(f"{base_path}/edomvd"),
+            et,
+            et.findall(f"{base_path}/edomv"),
+            et.findall(f"{base_path}/edomvd"),
         )
 
     root, edomv, edomvd = _get_xml("NLCD_2019_Land_Cover_Science_Product_L48_20210604")
     cover_classes = {}
     for t, v in zip(edomv, edomvd):
         cover_classes[t.text] = v.text
 
     clist = [i.split() for i in root.find("eainfo/overview/eadetcit").text.split("\n")[2:]]
     colors = {
         int(c): (float(r) / 255.0, float(g) / 255.0, float(b) / 255.0, 1.0) for c, r, g, b in clist
     }
-    colors[0] = (*colors[0][:3], 0.0)
+    colors[0] = (colors[0][0], colors[0][1], colors[0][2], 0.0)
 
     _, edomv, edomvd = _get_xml("nlcd_2019_impervious_descriptor_l48_20210604")
     descriptors = {}
     for t, v in zip(edomv, edomvd):
         tag = t.text.split(" - ")
         descriptors[tag[0]] = v.text if tag[-1].isnumeric() else f"{tag[-1]}: {v.text}"
 
@@ -108,17 +106,16 @@
             "42": 0.32,
             "43": 0.4,
             "45": 0.4,
             "46": 0.24,
             "51": 0.24,
             "52": 0.4,
             "71": 0.368,
-            "72": np.nan,
             "81": 0.325,
-            "82": 0.16,
+            "82": 0.037,
             "90": 0.086,
             "95": 0.1825,
         },
         "colors": colors,
     }
 
     return nlcd_meta
@@ -164,15 +161,16 @@
     f_list = [
         (d, f"{base_url}/det{d.strftime('%Y%j')}.modisSSEBopETactual.zip") for d in date_range
     ]
 
     return f_list
 
 
-class Stats(NamedTuple):
+@dataclass(frozen=True)
+class Stats:
     """Statistics for NLCD."""
 
     classes: dict[str, float]
     categories: dict[str, float]
 
 
 def _get_state_codes(subset_key: str | list[str]) -> list[str]:
@@ -196,15 +194,15 @@
         raise InputValueError("subset_key", [*valid_keys, "conus"])
     if other_keys:
         state_cd += tlz.concat(getattr(us_abbrs, k.upper()) for k in other_keys)
     return state_cd
 
 
 def get_us_states(subset_key: str | list[str] | None = None) -> gpd.GeoDataFrame:
-    """Get US states as a GeoDataFrame from Census' TIGERLine 2022 database.
+    """Get US states as a GeoDataFrame from Census' TIGERLine 2023 database.
 
     Parameters
     ----------
     subset_key : str or list of str, optional
         Key to subset the geometries instead of returning all states, by default
         all states are returned. Valid keys are:
 
@@ -215,23 +213,24 @@
         - Two letter state codes, e.g., ``["TX", "CA", "FL", ...]``
 
     Returns
     -------
     geopandas.GeoDataFrame
         GeoDataFrame of requested US states.
     """
-    url = "https://www2.census.gov/geo/tiger/TIGER2022/STATE/tl_2022_us_state.zip"
+    url = "https://www2.census.gov/geo/tiger/TIGER2023/STATE/tl_2023_us_state.zip"
     us_states = gpd.read_file(io.BytesIO(ar.retrieve_binary([url])[0]))
     if subset_key is not None:
         state_cd = _get_state_codes(subset_key)
-        return us_states[us_states.STUSPS.isin(state_cd)].copy()
-    return us_states
+        return us_states[us_states.STUSPS.isin(state_cd)].copy()  # pyright: ignore[reportReturnType]
+    return us_states  # pyright: ignore[reportReturnType]
 
 
-class StateCounties(NamedTuple):
+@dataclass(frozen=True)
+class StateCounties:
     """State and county codes and names."""
 
     name: str
     code: str | None
     counties: pd.Series
 
 
@@ -260,15 +259,15 @@
     resp = ar.retrieve_text(urls)
 
     codes = pd.read_csv(io.StringIO(resp[0]), sep="|")
     codes["STATE"] = codes["STATE"].astype(str).str.zfill(2)
     codes = codes.set_index("STATE")
 
     def _county2series(cd: dict[str, dict[str, str]]) -> pd.Series:
-        return pd.DataFrame.from_dict(cd, orient="index")["name"]
+        return pd.DataFrame.from_dict(cd, orient="index")["name"]  # pyright: ignore[reportReturnType]
 
     def _state_cd(state: str) -> str | None:
         try:
             return codes.loc[state, "STUSAB"]
         except KeyError:
             return None
```

### Comparing `pygeohydro-0.16.0/pygeohydro/nfhl.py` & `pygeohydro-0.16.1/pygeohydro/nfhl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Accessing National Flood Hazard Layers (NFHL) through web services."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Union
 
 from pygeohydro.exceptions import InputValueError
 from pygeoogc import ServiceURL
 from pynhd import AGRBase
```

### Comparing `pygeohydro-0.16.0/pygeohydro/nlcd.py` & `pygeohydro-0.16.1/pygeohydro/nlcd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Accessing data from the supported databases through their APIs."""
+
 from __future__ import annotations
 
 import warnings
 from typing import TYPE_CHECKING, Mapping, Tuple, Union, cast
 
 import cytoolz.curried as tlz
 import geopandas as gpd
@@ -97,15 +98,15 @@
             crs=self.crs,
             validation=False,
             ssl=ssl,
         )
 
     def get_layers(self) -> dict[str, str]:
         """Get NLCD layers for the provided years dictionary."""
-        valid_regions = ["L48", "HI", "PR", "AK"]
+        valid_regions = ("L48", "HI", "PR", "AK")
         if self.region not in valid_regions:
             raise InputValueError("region", valid_regions)
 
         nlcd_meta = helpers.nlcd_helper()
 
         names = ["impervious", "cover", "canopy", "descriptor"]
         avail_years = {n: nlcd_meta[f"{n}_years"] for n in names}
@@ -124,15 +125,15 @@
                     return f"nlcd_tcc_conus_{yr}_v2021-4"
                 return f"NLCD_{yr}_Tree_Canopy_{self.region}"
             if lyr == "cover":
                 return f"NLCD_{yr}_Land_Cover_Science_Product_{self.region}"
             if lyr == "impervious":
                 return f"NLCD_{yr}_Impervious_{self.region}"
             if self.region in ("HI", "PR"):
-                raise InputValueError("region (descriptor)", ("L48, AK"))  # noqa: TRY003
+                raise InputValueError("region (descriptor)", ("L48", "AK"))  # noqa: TRY003
             service_lyr = (
                 "Impervious_Descriptor" if self.region == "AK" else "Impervious_descriptor"
             )
             return f"NLCD_{yr}_{service_lyr}_{self.region}"
 
         return {f"{lyr}_{yr}": layer_name(lyr, yr) for lyr, yrs in self.years.items() for yr in yrs}
 
@@ -255,15 +256,14 @@
 
     Returns
     -------
     geopandas.GeoDataFrame
         A GeoDataFrame with the NLCD data and the coordinates.
     """
     nlcd_wms = NLCD(years=years, region=region, crs=3857, ssl=ssl)
-    coords = geoutils.geometry_reproject(coords, 4326, 4326)
     points = gpd.GeoSeries(gpd.points_from_xy(*zip(*coords), crs=4326))
     points_proj = points.to_crs(nlcd_wms.crs)
     geoms = points_proj.buffer(50, cap_style=3)
     ds_list = [nlcd_wms.get_map(g, 30) for g in geoms]
 
     def get_value(da: xr.DataArray, x: float, y: float) -> Number:
         nodata = da.attrs["nodatavals"][0]
@@ -388,15 +388,15 @@
     It considers land cover classes of 21 to 24 as urban and the rest as natural.
     Then, uses imperviousness percentage to partition the urban area into developed
     and impervious areas. So, ``urban = developed + impervious`` and always
     ``natural + urban = natural + developed + impervious = 100``.
 
     Parameters
     ----------
-    geometry : geopandas.GeoDataFrame or geopandas.GeoSeries
+    geo_df : geopandas.GeoDataFrame or geopandas.GeoSeries
         A GeoDataFrame or GeoSeries with the geometry to query. The indices are used
         as keys in the output dictionary.
     year : int, optional
         Year of the NLCD data, defaults to 2019. Available years are 2021, 2019, 2016,
         2013, 2011, 2008, 2006, 2004, and 2001.
     region : str, optional
         Region in the US that the input geometries are located, defaults to ``L48``.
@@ -405,15 +405,15 @@
 
     Returns
     -------
     pandas.DataFrame
         A dataframe with the same index as input ``geo_df`` and columns are the area
         percentages of the natural, developed, impervious, and urban
         (sum of developed and impervious) areas. Sum of urban and natural percentages
-        is always 100, as well as the sume of natural, developed, and impervious
+        is always 100, as well as the sum of natural, developed, and impervious
         percentages.
     """
     valid_year = (2021, 2019, 2016, 2013, 2011, 2008, 2006, 2004, 2001)
     if year not in valid_year:
         raise InputValueError("year", valid_year)
 
     if not isinstance(geo_df, (gpd.GeoDataFrame, gpd.GeoSeries)):
```

### Comparing `pygeohydro-0.16.0/pygeohydro/nwis.py` & `pygeohydro-0.16.1/pygeohydro/nwis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Accessing NWIS."""
-# pyright: reportGeneralTypeIssues=false
+
+# pyright: reportArgumentType=false,reportCallIssue=false,reportReturnType=false
 from __future__ import annotations
 
 import contextlib
 import itertools
 import re
 import warnings
 from typing import (
@@ -36,14 +37,15 @@
 from pynhd import NLDI
 
 try:
     from pandas.errors import IntCastingNaNError
 except ImportError:
     IntCastingNaNError = ValueError
 
+YEAR_END = "Y" if int(pd.__version__.split(".")[0]) < 2 else "YE"
 T_FMT = "%Y-%m-%d"
 __all__ = ["NWIS", "streamflow_fillna"]
 
 if TYPE_CHECKING:
     ArrayLike = TypeVar("ArrayLike", pd.Series, pd.DataFrame, xr.DataArray)
 
 
@@ -52,15 +54,15 @@
 
     It drops stations with more than ``missing_max`` days missing data
     per year. Missing data in the remaining stations, are filled with
     day-of-year average over the entire dataset.
 
     Parameters
     ----------
-    discharge : xarray.DataArray or pandas.DataFrame or pandas.Series
+    streamflow : xarray.DataArray or pandas.DataFrame or pandas.Series
         Daily streamflow observations with at least 10 years of daily data.
     missing_max : int
         Maximum allowed number of missing daily data per year for filling,
         defaults to 5.
 
     Returns
     -------
@@ -82,15 +84,15 @@
     df.columns = df.columns.astype(str)
     df.index = pd.DatetimeIndex(pd.to_datetime(df.index).date)
     if df.index.year.unique().size < 10:
         raise InputTypeError("streamflow", "array with at least 10 years of daily data")
 
     df[df < 0] = np.nan
     s_nan = pd.DataFrame.from_dict(
-        {yr: q.isna().sum() for yr, q in df.resample("Y")}, orient="index"
+        {yr: q.isna().sum() for yr, q in df.resample(YEAR_END)}, orient="index"
     )
     if np.all(s_nan == 0):
         return streamflow
 
     s_fill = s_nan[s_nan <= missing_max].dropna(axis=1).columns.tolist()
     if not s_fill:
         msg = f"Found no column with less than {missing_max} days of missing data."
@@ -125,16 +127,15 @@
     Notes
     -----
     More information about query parameters and codes that NWIS accepts
     can be found at its help
     `webpage <https://help.waterdata.usgs.gov/codes-and-parameters>`__.
     """
 
-    def __init__(self) -> None:
-        self.url = ServiceURL().restful.nwis
+    url: str = ServiceURL().restful.nwis
 
     @staticmethod
     def retrieve_rdb(url: str, payloads: list[dict[str, str]]) -> pd.DataFrame:
         """Retrieve and process requests with RDB format.
 
         Parameters
         ----------
@@ -171,15 +172,15 @@
 
         data = [
             line.split("\t") for r in resp for line in r.splitlines() if not line.startswith("#")
         ]
         if not data:
             raise ZeroMatchedError
 
-        rdb_df = pd.DataFrame.from_dict(dict(zip(data[0], d)) for d in data[2:])
+        rdb_df = pd.DataFrame.from_dict(dict(zip(data[0], d)) for d in data[2:])  # pyright: ignore[reportArgumentType]
         if "agency_cd" in rdb_df:
             rdb_df = rdb_df[~rdb_df["agency_cd"].str.contains("agency_cd|5s")].copy()
         return rdb_df
 
     @staticmethod
     def _validate_usgs_queries(
         queries: list[dict[str, str]], expanded: bool = False
@@ -274,15 +275,18 @@
         if not_valid:
             invalid_keys = f"query keys ({', '.join(not_valid)})"
             raise InputValueError(invalid_keys, valid_query_keys)
 
         _queries = queries.copy()
         if expanded:
             _ = [
-                q.pop(k) for k in ("outputDataTypeCd", "outputDataType") for q in _queries if k in q
+                q.pop(k)
+                for k in ("outputDataTypeCd", "outputDataType", "seriesCatalogOutput")
+                for q in _queries
+                if k in q
             ]
             output_type = {"siteOutput": "expanded"}
         else:
             output_type = {"siteOutput": "basic"}
 
         return [{**query, **output_type, "format": "rdb"} for query in _queries]
 
@@ -310,16 +314,17 @@
                     "reachcode": "nhd_reachcode",
                     "measure": "nhd_measure",
                     "WSAREASQKM": "nhd_areasqkm",
                 }
             )
         )
 
+    @classmethod
     def get_info(
-        self,
+        cls,
         queries: dict[str, str] | list[dict[str, str]],
         expanded: bool = False,
         fix_names: bool = True,
         nhd_info: bool = False,
     ) -> gpd.GeoDataFrame:
         """Send multiple queries to USGS Site Web Service.
 
@@ -344,16 +349,16 @@
         Returns
         -------
         geopandas.GeoDataFrame
             A correctly typed ``GeoDataFrame`` containing site(s) information.
         """
         queries = [queries] if isinstance(queries, dict) else queries
 
-        payloads = self._validate_usgs_queries(queries, False)
-        sites = self.retrieve_rdb(f"{self.url}/site", payloads)
+        payloads = cls._validate_usgs_queries(queries, False)
+        sites = cls.retrieve_rdb(f"{cls.url}/site", payloads)
 
         def fix_station_nm(station_nm: str) -> str:
             name = station_nm.title().rsplit(" ", 1)
             if len(name) == 1:
                 return name[0]
 
             name[0] = name[0] if name[0][-1] == "," else f"{name[0]},"
@@ -365,30 +370,34 @@
 
         for c in sites.select_dtypes("object"):
             sites[c] = sites[c].str.strip().astype(str)
 
         numeric_cols = ["dec_lat_va", "dec_long_va", "alt_va", "alt_acy_va"]
 
         if expanded:
-            payloads = self._validate_usgs_queries(queries, True)
+            payloads = cls._validate_usgs_queries(queries, True)
             sites = sites.merge(
-                self.retrieve_rdb(f"{self.url}/site", payloads),
+                cls.retrieve_rdb(f"{cls.url}/site", payloads),
                 on="site_no",
                 how="outer",
                 suffixes=("", "_overlap"),
             )
             sites = sites.filter(regex="^(?!.*_overlap)")
             numeric_cols += ["drain_area_va", "contrib_drain_area_va"]
 
         with contextlib.suppress(KeyError):
-            sites["begin_date"] = pd.to_datetime(sites["begin_date"])
-            sites["end_date"] = pd.to_datetime(sites["end_date"])
+            sites["begin_date"] = pd.to_datetime(
+                sites["begin_date"], errors="coerce", yearfirst=True
+            ).fillna(sites["begin_date"])
+            sites["end_date"] = pd.to_datetime(
+                sites["end_date"], errors="coerce", yearfirst=True
+            ).fillna(sites["end_date"])
 
         if nhd_info:
-            nhd = self._nhd_info(sites["site_no"].to_list())
+            nhd = cls._nhd_info(sites["site_no"].to_list())
             sites = pd.merge(sites, nhd, left_on="site_no", right_on="site_no", how="left")
 
         urls = [
             "/".join(
                 (
                     "https://gist.githubusercontent.com/cheginit",
                     "2dbc4b9c096f19089dbadb522821e8f3/raw/hcdn_2009_station_ids.txt",
@@ -404,15 +413,16 @@
 
         return gpd.GeoDataFrame(
             sites,
             geometry=gpd.points_from_xy(sites["dec_long_va"], sites["dec_lat_va"]),
             crs=4326,
         )
 
-    def get_parameter_codes(self, keyword: str) -> pd.DataFrame:
+    @classmethod
+    def get_parameter_codes(cls, keyword: str) -> pd.DataFrame:
         """Search for parameter codes by name or number.
 
         Notes
         -----
         NWIS guideline for keywords is as follows:
 
             By default an exact search is made. To make a partial search the term
@@ -437,15 +447,15 @@
         >>> nwis = NWIS()
         >>> codes = nwis.get_parameter_codes("%discharge%")
         >>> codes.loc[codes.parameter_cd == "00060", "parm_nm"].iloc[0]
         'Discharge, cubic feet per second'
         """
         url = "https://help.waterdata.usgs.gov/code/parameter_cd_nm_query"
         kwds = [{"parm_nm_cd": keyword, "fmt": "rdb"}]
-        return self.retrieve_rdb(url, kwds)
+        return cls.retrieve_rdb(url, kwds)
 
     @staticmethod
     def _to_xarray(qobs: pd.DataFrame, long_names: dict[str, str], mmd: bool) -> xr.Dataset:
         """Convert a pandas.DataFrame to an xarray.Dataset."""
         ds = xr.Dataset(
             data_vars={
                 "discharge": (["time", "station_id"], qobs),
@@ -517,51 +527,53 @@
         if not isinstance(dates, tuple) or len(dates) != 2:
             raise InputTypeError("dates", "tuple", "(start, end)")
 
         start = pd.to_datetime(dates[0], utc=utc)
         end = pd.to_datetime(dates[1], utc=utc)
         return sids_df.to_list(), start, end
 
-    def _drainage_area_sqm(self, siteinfo: pd.DataFrame, freq: str) -> pd.Series:
+    @classmethod
+    def _drainage_area_sqm(cls, siteinfo: pd.DataFrame, freq: str) -> pd.Series:
         """Get drainage area of the stations."""
         if "nhd_areasqkm" not in siteinfo:
-            area = self._nhd_info(siteinfo["site_no"].to_list())
+            area = cls._nhd_info(siteinfo["site_no"].to_list())
             area = area[["site_no", "nhd_areasqkm"]].copy()
         else:
-            area = siteinfo[["site_no", "nhd_areasqkm"]].copy()
-        if area["nhd_areasqkm"].isna().any():
+            area = siteinfo[["site_no", "nhd_areasqkm"]].copy()  # pyright: ignore[reportGeneralTypeIssues]
+        if area["nhd_areasqkm"].isna().any():  # pyright: ignore[reportGeneralTypeIssues]
             sids = area[area["nhd_areasqkm"].isna()].site_no
             queries = [
                 {
                     "parameterCd": "00060",
                     "siteStatus": "all",
                     "outputDataTypeCd": freq,
                     "sites": ",".join(s),
                 }
                 for s in tlz.partition_all(1500, sids)
             ]
-            info = self.get_info(queries, expanded=True)
+            info = cls.get_info(queries, expanded=True)
 
             def get_idx(ids: list[str]) -> tuple[pd.Index, pd.Index]:
                 return info.site_no.isin(ids), area.site_no.isin(ids)
 
             i_idx, a_idx = get_idx(sids)
             # Drainage areas in info are in sq mi and should be converted to sq km
             area.loc[a_idx, "nhd_areasqkm"] = info.loc[i_idx, "contrib_drain_area_va"] * 0.38610
-            if area["nhd_areasqkm"].isna().any():
+            if area["nhd_areasqkm"].isna().any():  # pyright: ignore[reportGeneralTypeIssues]
                 sids = area[area["nhd_areasqkm"].isna()].site_no
                 i_idx, a_idx = get_idx(sids)
                 area.loc[a_idx, "nhd_areasqkm"] = info.loc[i_idx, "drain_area_va"] * 0.38610
 
-        if area["nhd_areasqkm"].isna().all():
+        if area["nhd_areasqkm"].isna().all():  # pyright: ignore[reportGeneralTypeIssues]
             raise DataNotAvailableError("drainage")
         return area.set_index("site_no").nhd_areasqkm * 1e6
 
+    @classmethod
     def _get_streamflow(
-        self,
+        cls,
         sids: Sequence[str],
         start_dt: str,
         end_dt: str,
         freq: str,
         kwargs: dict[str, str],
     ) -> pd.DataFrame:
         """Convert json to dataframe."""
@@ -571,15 +583,15 @@
                 "startDT": start_dt,
                 "endDT": end_dt,
                 **kwargs,
             }
             for s in tlz.partition_all(1500, sids)
         ]
         resp = ar.retrieve_json(
-            [f"{self.url}/{freq}"] * len(payloads), [{"params": p} for p in payloads]
+            [f"{cls.url}/{freq}"] * len(payloads), [{"params": p} for p in payloads]
         )
         resp = cast("list[dict[str, Any]]", resp)
 
         def get_site_id(site_cd: dict[str, str]) -> str:
             """Get site id."""
             return f"{site_cd['agencyCode']}-{site_cd['value']}"
 
@@ -618,38 +630,39 @@
         qobs = pd.concat(itertools.starmap(to_df, r_ts.items()), axis=1)
         if len(qobs) == 0:
             raise DataNotAvailableError("discharge")
         qobs[qobs.le(0)] = np.nan
         # Convert cfs to cms
         return qobs * np.float_power(0.3048, 3)
 
+    @classmethod
     @overload
     def get_streamflow(
-        self,
+        cls,
         station_ids: Sequence[str] | str,
         dates: tuple[str, str],
         freq: str = "dv",
         mmd: bool = False,
         to_xarray: Literal[False] = ...,
-    ) -> pd.DataFrame:
-        ...
+    ) -> pd.DataFrame: ...
 
+    @classmethod
     @overload
     def get_streamflow(
-        self,
+        cls,
         station_ids: Sequence[str] | str,
         dates: tuple[str, str],
         freq: str = "dv",
         mmd: bool = False,
         to_xarray: Literal[True] = ...,
-    ) -> xr.Dataset:
-        ...
+    ) -> xr.Dataset: ...
 
+    @classmethod
     def get_streamflow(
-        self,
+        cls,
         station_ids: Sequence[str] | str,
         dates: tuple[str, str],
         freq: str = "dv",
         mmd: bool = False,
         to_xarray: bool = False,
     ) -> pd.DataFrame | xr.Dataset:
         """Get mean daily streamflow observations from USGS.
@@ -678,30 +691,30 @@
             Note that when frequency is set to ``iv`` the time zone is converted to UTC.
         """
         valid_freqs = ["dv", "iv"]
         if freq not in valid_freqs:
             raise InputValueError("freq", valid_freqs)
         utc = True if freq == "iv" else None
 
-        sids, start, end = self._check_inputs(station_ids, dates, utc)
+        sids, start, end = cls._check_inputs(station_ids, dates, utc)
 
         queries = [
             {
                 "parameterCd": "00060",
                 "siteStatus": "all",
                 "outputDataTypeCd": freq,
                 "sites": ",".join(s),
                 "startDt": start.strftime("%Y-%m-%d"),
                 "endDt": end.strftime("%Y-%m-%d"),
             }
             for s in tlz.partition_all(1500, sids)
         ]
 
         try:
-            siteinfo = self.get_info(queries)
+            siteinfo = cls.get_info(queries)
         except ZeroMatchedError as ex:
             raise DataNotAvailableError("discharge") from ex
 
         params = {
             "format": "json",
             "parameterCd": "00060",
             "siteStatus": "all",
@@ -723,35 +736,35 @@
         sids = list(siteinfo.site_no.unique())
         if not sids:
             raise DataNotAvailableError("discharge")
 
         time_fmt = T_FMT if utc is None else "%Y-%m-%dT%H:%M%z"
         start_dt = start.strftime(time_fmt)
         end_dt = end.strftime(time_fmt)
-        qobs = self._get_streamflow(sids, start_dt, end_dt, freq, params)
+        qobs = cls._get_streamflow(sids, start_dt, end_dt, freq, params)
 
         n_orig = len(sids)
         sids = [s.split("-")[1] for s in qobs]
         if len(sids) != n_orig:
             warnings.warn(
                 (
                     f"Dropped {n_orig - len(sids)} stations since they don't have discharge data"
                     f" from {start_dt} to {end_dt}."
                 ),
                 UserWarning,
                 stacklevel=2,
             )
         siteinfo = siteinfo[siteinfo.site_no.isin(sids)]
         if mmd:
-            area_sqm = self._drainage_area_sqm(siteinfo, freq)
+            area_sqm = cls._drainage_area_sqm(siteinfo, freq)
             ms2mmd = 1000.0 * 24.0 * 3600.0
             try:
                 qobs = pd.DataFrame(
                     {c: q / area_sqm.loc[c.split("-")[-1]] * ms2mmd for c, q in qobs.items()}
                 )
             except KeyError as ex:
                 raise DataNotAvailableError("drainage") from ex
 
-        qobs.attrs, long_names = self._get_attrs(siteinfo, mmd)
+        qobs.attrs, long_names = cls._get_attrs(siteinfo, mmd)
         if to_xarray:
-            return self._to_xarray(qobs, long_names, mmd)
+            return cls._to_xarray(qobs, long_names, mmd)
         return qobs
```

### Comparing `pygeohydro-0.16.0/pygeohydro/plot.py` & `pygeohydro-0.16.1/pygeohydro/plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Plot hydrological signatures.
 
 Plots include daily, monthly and annual hydrograph as well as regime
 curve (monthly mean) and flow duration curve.
 """
+
 # pyright: reportGeneralTypeIssues=false
 from __future__ import annotations
 
 import contextlib
+from dataclasses import dataclass, fields
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, NamedTuple, TypeVar, Union
+from typing import TYPE_CHECKING, Any, TypeVar, Union
 
 import folium
 import matplotlib.pyplot as plt
 import pandas as pd
 from matplotlib.colors import BoundaryNorm, ListedColormap
 
 import hydrosignatures as hs
@@ -26,23 +28,29 @@
 
     DF = TypeVar("DF", pd.DataFrame, pd.Series)
     CRSTYPE = Union[int, str, pyproj.CRS]
 
 __all__ = ["signatures", "prepare_plot_data"]
 
 
-class PlotDataType(NamedTuple):
+@dataclass(frozen=True)
+class PlotDataType:
     """Data structure for plotting hydrologic signatures."""
 
     daily: pd.DataFrame
     mean_monthly: pd.DataFrame
     ranked: pd.DataFrame
     titles: dict[str, str]
     units: dict[str, str]
 
+    @classmethod
+    def fields(cls) -> tuple[str, ...]:
+        """Return the field names of the dataclass."""
+        return tuple(field.name for field in fields(cls))
+
 
 def prepare_plot_data(daily: pd.DataFrame | pd.Series) -> PlotDataType:
     """Generate a structured data for plotting hydrologic signatures.
 
     Parameters
     ----------
     daily : pandas.Series or pandas.DataFrame
@@ -65,31 +73,31 @@
         "Flow Duration Curve",
     ]
     _units = [
         "mm/day",
         "mm/month",
         "mm/day",
     ]
-    fields = PlotDataType._fields
-    titles = dict(zip(fields[:-1], _titles))
-    units = dict(zip(fields[:-1], _units))
+    _fields = PlotDataType.fields()
+    titles = dict(zip(_fields[:-1], _titles))
+    units = dict(zip(_fields[:-1], _units))
     return PlotDataType(daily, mean_month, ranked, titles, units)
 
 
 def _prepare_plot_data(
     daily: pd.DataFrame | pd.Series,
     precipitation: pd.DataFrame | pd.Series | None = None,
 ) -> tuple[PlotDataType, PlotDataType | None]:
     if not isinstance(daily, (pd.DataFrame, pd.Series)):
         raise InputTypeError("daily", "pandas.DataFrame or pandas.Series")
 
     discharge = prepare_plot_data(daily)
     if precipitation is not None:
         if isinstance(precipitation, pd.DataFrame) and precipitation.shape[1] == 1:
-            prcp = prepare_plot_data(precipitation.squeeze())
+            prcp = prepare_plot_data(precipitation.squeeze())  # pyright: ignore[reportArgumentType]
         elif isinstance(precipitation, pd.Series):
             prcp = prepare_plot_data(precipitation)
         else:
             raise InputTypeError(
                 "precipitation", "pandas.Series or pandas.DataFrame with one column"
             )
     else:
@@ -147,15 +155,20 @@
     if prcp is not None:
         _prcp = prcp.daily.squeeze()
         _prcp = _prcp.loc[daily.index[0] : daily.index[-1]]
         label = "$P$ (mm/day)"
         ax_p = ax.twinx()
         ax_p.grid(False)
         if _prcp.shape[0] > 1000:
-            ax_p.plot(_prcp, alpha=0.7, color="g", label=label)
+            ax_p.plot(
+                _prcp,
+                alpha=0.7,
+                color="g",
+                label=label,
+            )
         else:
             ax_p.bar(
                 _prcp.index,
                 _prcp.to_numpy().ravel(),
                 alpha=0.7,
                 width=1,
                 color="g",
@@ -243,15 +256,15 @@
     Parameters
     ----------
     bbox : tuple
         List of corners in this order (west, south, east, north)
     crs : str, int, or pyproj.CRS, optional
         CRS of the input bounding box, defaults to EPSG:4326.
     nwis_kwds : dict, optional
-        Optional keywords to include in the NWIS request as a dictionary like so:
+        Additional keywords to include in the NWIS request as a dictionary like so:
         ``{"hasDataTypeCd": "dv,iv", "outputDataTypeCd": "dv,iv", "parameterCd": "06000"}``.
         Default to None.
 
     Returns
     -------
     folium.Map
         Interactive map within a bounding box.
```

### Comparing `pygeohydro-0.16.0/pygeohydro/print_versions.py` & `pygeohydro-0.16.1/pygeohydro/print_versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Utility functions for printing version information.
 
 The original script is from
 `xarray <https://github.com/pydata/xarray/blob/main/xarray/util/print_versions.py>`__
 """
+
 # pyright: reportMissingImports=false
 from __future__ import annotations
 
 import contextlib
 import importlib
 import importlib.util
 import locale
```

### Comparing `pygeohydro-0.16.0/pygeohydro/pygeohydro.py` & `pygeohydro-0.16.1/pygeohydro/pygeohydro.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """Accessing data from the supported databases through their APIs."""
+
 from __future__ import annotations
 
 import contextlib
 import functools
 import importlib.util
 import io
 import itertools
 import warnings
-import zipfile
+from datetime import datetime, timezone
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Iterable, Iterator, Literal, Sequence, Tuple, Union, cast
 from unittest.mock import patch
+from zipfile import ZipFile
 
 import cytoolz.curried as tlz
 import geopandas as gpd
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import pyproj
 import rasterio as rio
+import requests
 import xarray as xr
+from rasterio.io import MemoryFile
 from rioxarray import _io as rxr
 from shapely.errors import GEOSException
 
 import async_retriever as ar
 import pygeoogc as ogc
 import pygeoutils as geoutils
 from pygeohydro import helpers
@@ -141,17 +145,15 @@
     f_list = helpers.get_ssebopeta_urls(dates)
     session = RetrySession()
 
     with patch("socket.has_ipv6", False), RetrySession() as session:
 
         def _ssebop(url: str) -> list[npt.NDArray[np.float64]]:
             r = session.get(url)
-            z = zipfile.ZipFile(io.BytesIO(r.content))
-
-            with rio.MemoryFile() as memfile:
+            with ZipFile(io.BytesIO(r.content)) as z, MemoryFile() as memfile:
                 memfile.write(z.read(z.filelist[0].filename))
                 with memfile.open() as src:
                     return list(src.sample(co_list))
 
         time, eta = zip(*[(t, _ssebop(url)) for t, url in f_list])
     eta_arr = np.array(eta).reshape(len(time), -1)
     ds = xr.Dataset(
@@ -188,15 +190,15 @@
     Since there's still no web service available for subsetting SSEBop, the data first
     needs to be downloaded for the requested period then it is masked by the
     region of interest locally. Therefore, it's not as fast as other functions and
     the bottleneck could be the download speed.
 
     Parameters
     ----------
-    geometry : shapely.geometry.Polygon or tuple
+    geometry : shapely.Polygon or tuple
         The geometry for downloading clipping the data. For a tuple bbox,
         the order should be (west, south, east, north).
     dates : tuple or list, optional
         Start and end dates as a tuple (start, end) or a list of years [2001, 2010, ...].
     geo_crs : str, int, or pyproj.CRS, optional
         The CRS of the input geometry, defaults to ``epsg:4326``.
 
@@ -213,17 +215,17 @@
         raise InputTypeError("geometry", "(Multi)Polygon or tuple of length 4") from ex
 
     gtiff2xarray = functools.partial(geoutils.gtiff2xarray, geometry=geometry, geo_crs=geo_crs)
     with patch("socket.has_ipv6", False), RetrySession() as session:
 
         def _ssebop(t: pd.Timestamp, url: str) -> xr.DataArray | xr.Dataset:
             resp = session.get(url)
-            zfile = zipfile.ZipFile(io.BytesIO(resp.content))
-            content = zfile.read(zfile.filelist[0].filename)
-            return gtiff2xarray(r_dict={"eta": content}).expand_dims({"time": [t]})
+            with ZipFile(io.BytesIO(resp.content)) as zfile:
+                content = zfile.read(zfile.filelist[0].filename)
+                return gtiff2xarray(r_dict={"eta": content}).expand_dims({"time": [t]})
 
         data = xr.merge(itertools.starmap(_ssebop, f_list))
     eta = data.eta.where(data.eta < data.eta.rio.nodata) * 1e-3
     eta = cast("xr.DataArray", eta)
     eta.attrs.update(
         {
             "units": "mm/day",
@@ -231,14 +233,34 @@
             "crs": 4326,
             "long_name": "Actual ET",
         }
     )
     return eta
 
 
+def _remote_file_modified(file_path: Path) -> bool:
+    """Check if the file is older than the last modification date of the NID web service."""
+    url = "https://nid.sec.usace.army.mil/api/nation/gpkg"
+    # we need to get the redirect URL so that we can get the last modified date, so
+    # we need to send a request with the Range header set to 0-0 to avoid downloading
+    # the entire file.
+    response = requests.get(url, headers={"Range": "bytes=0-0"}, allow_redirects=True, timeout=50)
+    if response.status_code != 200:
+        raise ServiceError(response.reason, url)
+    response = requests.head(response.url, timeout=50)
+    if response.status_code != 200:
+        raise ServiceError(response.reason, url)
+
+    remote_last_modified = datetime.strptime(
+        response.headers["Last-Modified"], "%a, %d %b %Y %H:%M:%S GMT"
+    )
+    local_last_modified = datetime.fromtimestamp(file_path.stat().st_mtime, tz=timezone.utc)
+    return local_last_modified < remote_last_modified
+
+
 class NID:
     """Retrieve data from the National Inventory of Dams web service."""
 
     def __init__(self) -> None:
         self.base_url = ServiceURL().restful.nid
         self.suggest_url = f"{self.base_url}/suggestions"
         resp = ar.retrieve_json([f"{self.base_url}/advanced-fields"])
@@ -320,14 +342,16 @@
         """
         fname = self.nid_inventory_path if fname is None else Path(fname)
         if fname.suffix != ".feather":
             fname = fname.with_suffix(".feather")
 
         self.nid_inventory_path = fname
         if not self.nid_inventory_path.exists():
+            if _remote_file_modified(fname.with_suffix(".gpkg")):
+                fname.with_suffix(".gpkg").unlink()
             url = "https://nid.sec.usace.army.mil/api/nation/gpkg"
             _ = ogc.streaming_download(url, fnames=fname.with_suffix(".gpkg"))
             dams = (
                 gpd.read_file(fname.with_suffix(".gpkg"), engine="pyogrio", use_arrow=True)
                 if importlib.util.find_spec("pyogrio")
                 else gpd.read_file(fname.with_suffix(".gpkg"))
             )
@@ -601,15 +625,15 @@
         --------
         >>> from pygeohydro import NID
         >>> nid = NID()
         >>> dams = nid.inventory_byid(['KY01232', 'GA02400', 'NE04081', 'IL55070', 'TN05345'])
         """
         if not isinstance(federal_ids, Iterable) or isinstance(federal_ids, (str, int)):
             raise InputTypeError("federal_ids", "list of str (Federal IDs)")
-        
+
         if not all(isinstance(i, str) for i in federal_ids):
             raise InputTypeError("federal_ids", "list of str (Federal IDs)")
 
         urls = [f"{self.base_url}/dams/{i.upper()}/inventory" for i in set(federal_ids)]
         return self._to_geodf(pd.DataFrame(self._get_json(urls)).set_index("id"))
 
     def get_suggestions(
@@ -699,27 +723,27 @@
     if properties == "*":
         prop = list(valid_props)
     else:
         prop = [properties] if isinstance(properties, str) else properties
         if not all(p in valid_props for p in prop):
             raise InputValueError("properties", list(valid_props))
 
-    soil = ScienceBase().get_file_urls("5fd7c19cd34e30b9123cb51f")
+    soil = ScienceBase.get_file_urls("5fd7c19cd34e30b9123cb51f")
     pat = "|".join(prop)
     _files, urls = zip(*soil[soil.index.str.contains(f"{pat}.*zip")].url.to_dict().items())
     urls = list(urls)
 
     root = Path(soil_dir)
     root.mkdir(exist_ok=True, parents=True)
     files = [root.joinpath(f) for f in _files]
     _ = ogc.streaming_download(urls, fnames=files)
 
     def get_tif(file: Path) -> xr.DataArray:
         """Get the .tif file from a zip file."""
-        with zipfile.ZipFile(file) as z:
+        with ZipFile(file) as z:
             try:
                 fname = next(f.filename for f in z.filelist if f.filename.endswith(".tif"))
             except StopIteration as ex:
                 raise ZeroMatchedError from ex
             ds = rxr.open_rasterio(io.BytesIO(z.read(fname)))
             ds = cast("xr.DataArray", ds)
             ds = ds.squeeze("band", drop=True)
@@ -793,21 +817,21 @@
         with rio.open(fpaths[0]) as src:
             ds_crs = src.crs
         ds = ds.rio.write_transform(affine)
         ds = ds.rio.write_crs(ds_crs)
         ds = ds.rio.write_coordinate_system()
         return ds
 
-    ds = xr.merge((get_layer(lyr) for lyr in lyrs), combine_attrs="drop_conflicts")
-    poly = geoutils.geo2polygon(geometry, crs, ds.rio.crs)
-    ds = geoutils.xarray_geomask(ds, poly, ds.rio.crs)
-    _ = ds.attrs.pop("_FillValue", None)
-    _ = ds.attrs.pop("units", None)
-    _ = ds.attrs.pop("long_name", None)
-    return ds
+    soil = xr.merge((get_layer(lyr) for lyr in lyrs), combine_attrs="drop_conflicts")
+    poly = geoutils.geo2polygon(geometry, crs, soil.rio.crs)
+    soil = geoutils.xarray_geomask(soil, poly, soil.rio.crs)
+    _ = soil.attrs.pop("_FillValue", None)
+    _ = soil.attrs.pop("units", None)
+    _ = soil.attrs.pop("long_name", None)
+    return soil
 
 
 class EHydro(AGRBase):
     """Access USACE Hydrographic Surveys (eHydro).
 
     Notes
     -----
@@ -885,15 +909,15 @@
 
     def __post_process(self, survey: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
         urls = survey["sourcedatalocation"].to_list()
         fnames = [Path("cache", Path(u).name) for u in urls]
         _ = ogc.streaming_download(urls, fnames=fnames)
 
         def get_depth(fname: Path) -> gpd.GeoDataFrame:
-            with zipfile.ZipFile(fname, "r") as zip_ref:
+            with ZipFile(fname, "r") as zip_ref:
                 gdb = next(
                     (
                         f"zip://{fname}!{n.filename}"
                         for n in zip_ref.filelist
                         if n.filename.endswith(".gdb/")
                     ),
                     None,
@@ -902,18 +926,16 @@
                     raise ZeroMatchedError(self._error_msg)
 
             if self._layer == "SurveyPoint" and "SurveyPointHD" in self._get_layers(gdb):
                 self._layer = "SurveyPointHD"
 
             if self._engine == "pyogrio":
                 with contextlib.suppress(GEOSException):
-                    return gpd.read_file(
-                        gdb, layer=self._layer, engine="pyogrio", use_arrow=True
-                    )  # pyright: ignore[reportGeneralTypeIssues]
-            return gpd.read_file(gdb, layer=self._layer)  # pyright: ignore[reportGeneralTypeIssues]
+                    return gpd.read_file(gdb, layer=self._layer, engine="pyogrio", use_arrow=True)  # pyright: ignore[reportReturnType]
+            return gpd.read_file(gdb, layer=self._layer)  # pyright: ignore[reportReturnType]
 
         return gpd.GeoDataFrame(pd.concat((get_depth(f) for f in fnames), ignore_index=True))
 
     def _getfeatures(
         self, oids: Iterator[tuple[str, ...]], return_m: bool = False, return_geom: bool = True
     ) -> gpd.GeoDataFrame:
         """Send a request for getting data based on object IDs.
```

### Comparing `pygeohydro-0.16.0/pygeohydro/stnfloodevents.py` & `pygeohydro-0.16.1/pygeohydro/stnfloodevents.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Access USGS Short-Term Network (STN) via Restful API."""
+
 from __future__ import annotations
 
 from io import BytesIO
 from typing import TYPE_CHECKING, Any, ClassVar, Literal, Union, cast, overload
 
 import geopandas as gpd
 import numpy as np
@@ -176,33 +177,31 @@
                 return x
             if len(x) == 1:
                 return x[0]
             return np.nan
 
         return {k: delist(v) for k, v in d.items()}
 
-    @overload
     @classmethod
+    @overload
     def data_dictionary(
         cls,
         data_type: str,
         as_dict: Literal[False] = False,
         async_retriever_kwargs: dict[str, Any] | None = ...,
-    ) -> pd.DataFrame:
-        ...
+    ) -> pd.DataFrame: ...
 
-    @overload
     @classmethod
+    @overload
     def data_dictionary(
         cls,
         data_type: str,
         as_dict: Literal[True] = True,
         async_retriever_kwargs: dict[str, Any] | None = ...,
-    ) -> dict[str, Any]:
-        ...
+    ) -> dict[str, Any]: ...
 
     @classmethod
     def data_dictionary(
         cls,
         data_type: str,
         as_dict: bool = False,
         async_retriever_kwargs: dict[str, Any] | None = None,
@@ -280,35 +279,33 @@
                 data_dict["Field"].append(f)
                 data_dict["Definition"].append(d)
 
         if as_dict:
             return data_dict
         return pd.DataFrame(data_dict)
 
-    @overload
     @classmethod
+    @overload
     def get_all_data(
         cls,
         data_type: str,
         as_list: Literal[False] = False,
         crs: CRSTYPE = ...,
         async_retriever_kwargs: dict[str, Any] | None = ...,
-    ) -> gpd.GeoDataFrame | pd.DataFrame:
-        ...
+    ) -> gpd.GeoDataFrame | pd.DataFrame: ...
 
-    @overload
     @classmethod
+    @overload
     def get_all_data(
         cls,
         data_type: str,
         as_list: Literal[True] = True,
         crs: CRSTYPE = ...,
         async_retriever_kwargs: dict[str, Any] | None = ...,
-    ) -> list[dict[str, Any]]:
-        ...
+    ) -> list[dict[str, Any]]: ...
 
     @classmethod
     def get_all_data(
         cls,
         data_type: str,
         as_list: bool = False,
         crs: CRSTYPE = 4326,
@@ -381,15 +378,15 @@
 
         if async_retriever_kwargs is None:
             async_retriever_kwargs = {}
         else:
             _ = async_retriever_kwargs.pop("url", None)
 
         resp = ar.retrieve_json([f"{cls.service_url}{endpoint}"], **async_retriever_kwargs)
-        data = [cls._delist_dict(d) for d in resp[0]]  # pyright: ignore[reportGeneralTypeIssues]
+        data = [cls._delist_dict(d) for d in resp[0]]  # pyright: ignore[reportArgumentType]
 
         if as_list:
             return data
 
         _xy_cols = {
             "instruments": None,
             "peaks": None,
@@ -399,37 +396,35 @@
         xy_cols = _xy_cols[data_type]
         if xy_cols is None:
             return pd.DataFrame(data)
 
         x_col, y_col = xy_cols
         return cls._geopandify(data, x_col, y_col, crs, cls.service_crs)
 
-    @overload
     @classmethod
+    @overload
     def get_filtered_data(
         cls,
         data_type: str,
         query_params: dict[str, Any] | None = ...,
         as_list: Literal[False] = False,
         crs: CRSTYPE = ...,
         async_retriever_kwargs: dict[str, Any] | None = ...,
-    ) -> gpd.GeoDataFrame | pd.DataFrame:
-        ...
+    ) -> gpd.GeoDataFrame | pd.DataFrame: ...
 
-    @overload
     @classmethod
+    @overload
     def get_filtered_data(
         cls,
         data_type: str,
         query_params: dict[str, Any] | None = ...,
         as_list: Literal[True] = True,
         crs: CRSTYPE = ...,
         async_retriever_kwargs: dict[str, Any] | None = ...,
-    ) -> list[dict[str, Any]]:
-        ...
+    ) -> list[dict[str, Any]]: ...
 
     @classmethod
     def get_filtered_data(
         cls,
         data_type: str,
         query_params: dict[str, Any] | None = None,
         as_list: bool = False,
@@ -545,15 +540,15 @@
             async_retriever_kwargs.pop("request_kwds", None)
 
         resp = ar.retrieve_json(
             [f"{cls.service_url}{endpoint}"],
             request_kwds=[{"params": query_params}],
             **async_retriever_kwargs,
         )
-        data = [cls._delist_dict(d) for d in resp[0]]  # pyright: ignore[reportGeneralTypeIssues]
+        data = [cls._delist_dict(d) for d in resp[0]]  # pyright: ignore[reportArgumentType]
         if as_list:
             return data
 
         xy_cols = {
             "instruments": ("longitude", "latitude"),
             "peaks": ("longitude_dd", "latitude_dd"),
             "hwms": ("longitude", "latitude"),
```

### Comparing `pygeohydro-0.16.0/pygeohydro/us_abbrs.py` & `pygeohydro-0.16.1/pygeohydro/us_abbrs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """US states and territories Abbreviations from ``us`` package."""
+
 from __future__ import annotations
 
 CONTIGUOUS = [
     "AL",
     "AZ",
     "AR",
     "CA",
```

### Comparing `pygeohydro-0.16.0/pygeohydro/waterdata.py` & `pygeohydro-0.16.1/pygeohydro/waterdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Accessing WaterData related APIs."""
+
 from __future__ import annotations
 
 import io
 from typing import TYPE_CHECKING, Any, Literal, cast, overload
 
 import cytoolz.curried as tlz
 import pandas as pd
@@ -239,21 +240,21 @@
     """Class for interacting with SensorThings API."""
 
     def __init__(self) -> None:
         self.base_url = "https://labs.waterdata.usgs.gov/sta/v1.1/Things"
 
     @overload
     @staticmethod
-    def _get_urls(url: str, kwd: dict[str, Any] | None = ...) -> dict[str, Any]:
-        ...
+    def _get_urls(url: str, kwd: dict[str, Any] | None = ...) -> dict[str, Any]: ...
 
     @overload
     @staticmethod
-    def _get_urls(url: list[str], kwd: list[dict[str, Any]] | None = ...) -> list[dict[str, Any]]:
-        ...
+    def _get_urls(
+        url: list[str], kwd: list[dict[str, Any]] | None = ...
+    ) -> list[dict[str, Any]]: ...
 
     @staticmethod
     def _get_urls(
         url: str | list[str], kwd: dict[str, Any] | list[dict[str, Any]] | None = None
     ) -> dict[str, Any] | list[dict[str, Any]]:
         urls = url if isinstance(url, list) else [url]
         if kwd:
@@ -286,15 +287,15 @@
             Conditionals to be applied to the database, defaults to ``None``.
             Note that the conditionals should have the form of
             ``cond1 operator 'value' and/or cond2 operator 'value``.
             For example:
             ``properties/monitoringLocationType eq 'Stream' and ...``
         expand : dict of dict, optional
             Expand the properties of the selected columns, defaults to ``None``.
-            Note that the expand should have the form of
+            Note that the ``expand`` should have the form of
             ``{Property: {func: value, ...}}``. For example: ``{"Locations":
             {"select": "location", "filter": "ObservedProperty/@iot.id eq '00060'"}}``
         max_count : int, optional
             Maximum number of items to be returned, defaults to ``None``.
         extra_params : dict, optional
             Extra parameters to be added to the Odata filter, defaults to ``None``.
 
@@ -377,15 +378,15 @@
         pandas.DataFrame
             Requested sensor data.
         """
         sensor_ids = [sensor_ids] if isinstance(sensor_ids, str) else sensor_ids
         urls = [f"{self.base_url}('{i}')" for i in sensor_ids]
         data = pd.json_normalize(self._get_urls(urls))
         columns = data.columns[data.columns.str.endswith("Link")]
-        return data.drop(columns=columns)  # pyright: ignore[reportGeneralTypeIssues]
+        return data.drop(columns=columns)  # pyright: ignore[reportCallIssue,reportArgumentType]
 
     def sensor_property(self, sensor_property: str, sensor_ids: str | list[str]) -> pd.DataFrame:
         """Query a sensor property.
 
         Parameters
         ----------
         sensor_property : str or list of str
```

### Comparing `pygeohydro-0.16.0/pygeohydro/watershed.py` & `pygeohydro-0.16.1/pygeohydro/watershed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Accessing watershed boundary-level data through web services."""
+
 from __future__ import annotations
 
 import importlib.util
 import io
 from pathlib import Path
 from typing import TYPE_CHECKING, Union, cast
 
@@ -126,20 +127,23 @@
 def irrigation_withdrawals() -> xr.Dataset:
     """Get monthly water use for irrigation at HUC12-level for CONUS.
 
     Notes
     -----
     Dataset is retrieved from https://doi.org/10.5066/P9FDLY8P.
     """
-    item = ScienceBase().get_file_urls("5ff7acf4d34ea5387df03d73")
+    item = ScienceBase.get_file_urls("5ff7acf4d34ea5387df03d73")
     urls = item.loc[item.index.str.contains(".csv"), "url"]
     resp = ar.retrieve_text(urls.tolist())
     irr = {}
     for name, r in zip(urls.index, resp):
-        df = pd.read_csv(io.StringIO(r), usecols=lambda x: "m3" in x or "huc12t" in x)  # pyright: ignore[reportGeneralTypeIssues]
+        df = pd.read_csv(
+            io.StringIO(r),
+            usecols=lambda s: "m3" in s or "huc12t" in s,  # type: ignore
+        )
         df["huc12t"] = df["huc12t"].str.strip("'")
         df = df.rename(columns={"huc12t": "huc12"}).set_index("huc12")
         df = df.rename(columns={c: str(c)[:3].capitalize() for c in df})
         irr[name[-6:-4]] = df.copy()
     ds = xr.Dataset(irr).rename({"dim_1": "month"})
     long_names = {
         "GW": "groundwater_withdrawal",
```

### Comparing `pygeohydro-0.16.0/pygeohydro.egg-info/PKG-INFO` & `pygeohydro-0.16.1/pygeohydro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeohydro
-Version: 0.16.0
+Version: 0.16.1
 Summary: Access geospatial web services that offer hydrological data
 Author-email: Taher Chegini <cheginit@gmail.com>
 License: MIT
 Project-URL: CI, https://github.com/hyriver/pygeohydro/actions
 Project-URL: Changelog, https://docs.hyriver.io/changelogs/pygeohydro.html
 Project-URL: Homepage, https://docs.hyriver.io/readme/pygeohydro.html
 Project-URL: Issues, https://github.com/hyriver/pygeohydro/issues
```

### Comparing `pygeohydro-0.16.0/pygeohydro.egg-info/SOURCES.txt` & `pygeohydro-0.16.1/pygeohydro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.0/pyproject.toml` & `pygeohydro-0.16.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -83,20 +83,17 @@
 
 [tool.setuptools.packages]
 find = {namespaces = false}
 
 [tool.setuptools_scm]
 fallback_version = "999"
 
-[tool.black]
-line-length = 100
-
 [tool.ruff]
 target-version = "py38"
-select = [
+lint.select = [
     # flake8-bugbear
     "B",
     # flake8-comprehensions
     "C4",
     # pydocstyle
     "D",
     # Error
@@ -146,41 +143,50 @@
     "PYI",
     # tidy imports
     "TID",
     # type-checking imports
     "TCH",
     # Ruff-specific rules
     "RUF",
+    # compatibility with numpy 2.0
+    "NPY201",
 ]
 
 exclude = [
     "__pycache__",
     ".nox",
 ]
 
-ignore = [
+lint.ignore = [
     "D103",
     "D105",
     "E501",
     "PLR2004",
     "PLR0913",
+    "PGH003",
+    # conflict with ruff-formatter
+    "ISC001",
+]
+lint.extend-safe-fixes = [
+  # absolute imports
+  "TID252",
 ]
 line-length = 100
 
-[tool.ruff.flake8-bugbear]
+[tool.ruff.lint.flake8-bugbear]
 extend-immutable-calls = [
     "chr",
     "typer.Argument",
     "typer.Option",
 ]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/*.py" = [
     "D100",
     "D101",
     "D102",
     "D103",
     "D104",
     "D105",
@@ -194,33 +200,29 @@
     "S106",
     # use of "eval"
     "PGH001",
     # Mutable class attributes
     "RUF012",
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
+required-imports = ["from __future__ import annotations"]
 known-first-party = [
   "async_retriever",
   "pygeoogc",
   "pygeoutils",
   "pynhd",
   "py3dep",
   "hydrosignatures",
   "pygeohydro",
   "pydaymet",
+  "pygridmet",
   "pynldas2",
 ]
 
-[tool.pycln]
-all = true
-expand_stars = true
-no_gitignore = false
-verbose = true
-
 [tool.codespell]
 skip = "__pycache__,_build,.mypy_cache,.git,./htmlcov,.nox,**/us_abbrs.py,cache"
 ignore-words-list = "gage,gages,paramss,trough"
 
 [tool.pytest.ini_options]
 addopts = "--ignore=noxfile.py -n=auto -v --cov=pygeohydro --cov-report xml --durations=5"
 doctest_optionflags = 'NORMALIZE_WHITESPACE IGNORE_EXCEPTION_DETAIL NUMBER'
@@ -265,14 +267,15 @@
 reportUnknownArgumentType = false
 reportUnknownLambdaType = false
 reportUnknownMemberType = false
 reportUnknownParameterType = false
 reportUnknownVariableType = false
 reportUnnecessaryIsInstance = false
 reportUntypedFunctionDecorator = false
+reportAttributeAccessIssue = false
 typeCheckingMode = "strict"
 
 [tool.fixit]
 formatter = "ufmt"
 
 [tool.refurb]
 python_version = "3.8"
```

### Comparing `pygeohydro-0.16.0/tests/test_exceptions.py` & `pygeohydro-0.16.1/tests/test_exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import geopandas as gpd
 import pandas as pd
 import pytest
 from shapely import Polygon
 
 import pygeohydro as gh
 from pygeohydro import (
```

### Comparing `pygeohydro-0.16.0/tests/test_pygeohydro.py` & `pygeohydro-0.16.1/tests/test_pygeohydro.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 """Tests for PyGeoHydro package."""
+
+from __future__ import annotations
+
 import io
 import shutil
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import pytest
@@ -30,15 +33,15 @@
         [-69.77, 45.45],
         [-69.77, 45.07],
     ]
 )
 
 
 def assert_close(a: float, b: float) -> None:
-    assert np.isclose(a, b, rtol=1e-3).all()
+    np.testing.assert_allclose(a, b, rtol=1e-3)
 
 
 class TestNWIS:
     nwis: NWIS = NWIS()
 
     def test_qobs_dv(self):
         df = self.nwis.get_streamflow(SID_NATURAL, DATES)
@@ -297,15 +300,15 @@
 def test_irrigation():
     irr = gh.irrigation_withdrawals()
     assert_close(irr.TW.mean(), 419996.4992)
 
 
 def test_soil():
     soil = gh.soil_properties("por")
-    assert soil.dims["x"] == 266301
+    assert soil.sizes["x"] == 266301
 
 
 def test_gnatsgo():
     layers = ["Tk0_100a", "Soc20_50"]
     geometry = (-95.624515, 30.121598, -95.448253, 30.264074)
     soil = gh.soil_gnatsgo(layers, geometry, 4326)
     assert_close(soil.tk0_100a.mean().compute().item(), 89.848)
```


# Comparing `tmp/earthkit-meteo-0.0.1.tar.gz` & `tmp/earthkit_meteo-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthkit-meteo-0.0.1.tar", last modified: Wed Sep  6 14:57:16 2023, max compression
+gzip compressed data, was "earthkit_meteo-0.1.0.tar", last modified: Thu Apr 25 09:11:15 2024, max compression
```

## Comparing `earthkit-meteo-0.0.1.tar` & `earthkit_meteo-0.1.0.tar`

### file list

```diff
@@ -1,51 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-06 14:57:16.104051 earthkit-meteo-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-06 14:57:16.100051 earthkit-meteo-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-06 14:57:16.100051 earthkit-meteo-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5807 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/.github/workflows/label-public-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/.github/workflows/notify-new-issue.yml
--rw-r--r--   0 runner    (1001) docker     (127)      279 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/.github/workflows/notify-new-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      755 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2023-09-06 14:57:16.104051 earthkit-meteo-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-06 14:57:16.104051 earthkit-meteo-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-06 14:57:16.104051 earthkit-meteo-0.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/docs/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)    65385 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/docs/_static/earthkit-meteo.png
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/docs/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-06 14:57:16.104051 earthkit-meteo-0.0.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/docs/licence.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/docs/references.rst
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-06 14:57:16.100051 earthkit-meteo-0.0.1/earthkit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-06 14:57:16.104051 earthkit-meteo-0.0.1/earthkit/meteo/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/earthkit/meteo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-06 14:57:16.104051 earthkit-meteo-0.0.1/earthkit/meteo/solar/
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/earthkit/meteo/solar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-09-06 14:57:16.000000 earthkit-meteo-0.0.1/earthkit/meteo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-06 14:57:16.104051 earthkit-meteo-0.0.1/earthkit_meteo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2023-09-06 14:57:16.000000 earthkit-meteo-0.0.1/earthkit_meteo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      891 2023-09-06 14:57:16.000000 earthkit-meteo-0.0.1/earthkit_meteo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-06 14:57:16.000000 earthkit-meteo-0.0.1/earthkit_meteo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-09-06 14:57:16.000000 earthkit-meteo-0.0.1/earthkit_meteo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-06 14:57:16.000000 earthkit-meteo-0.0.1/earthkit_meteo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      890 2023-09-06 14:57:16.104051 earthkit-meteo-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-06 14:57:16.104051 earthkit-meteo-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/tests/environment-unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/tests/test_solar.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2023-09-06 14:56:58.000000 earthkit-meteo-0.0.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.210790 earthkit_meteo-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.194790 earthkit_meteo-0.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/.github/ci-hpc-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.194790 earthkit_meteo-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/.github/workflows/label-public-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/.github/workflows/legacy-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/.github/workflows/notify-new-issue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/.github/workflows/notify-new-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-25 09:11:15.210790 earthkit_meteo-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.198790 earthkit_meteo-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.198790 earthkit_meteo-0.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/docs/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)    65385 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/docs/_static/earthkit-meteo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/docs/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)    35591 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/docs/_static/wind_direction.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35424 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/docs/_static/wind_sector.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.198790 earthkit_meteo-0.1.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/docs/licence.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/docs/references.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/docs/skip_api_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.190790 earthkit_meteo-0.1.0/earthkit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.198790 earthkit_meteo-0.1.0/earthkit/meteo/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.198790 earthkit_meteo-0.1.0/earthkit/meteo/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/constants/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.202790 earthkit_meteo-0.1.0/earthkit/meteo/extreme/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/extreme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.202790 earthkit_meteo-0.1.0/earthkit/meteo/extreme/array/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/extreme/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/extreme/array/cpf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/extreme/array/efi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/extreme/array/sot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/extreme/cpf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/extreme/efi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/extreme/sot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.202790 earthkit_meteo-0.1.0/earthkit/meteo/score/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/score/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.202790 earthkit_meteo-0.1.0/earthkit/meteo/score/array/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/score/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/score/array/crps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/score/crps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.202790 earthkit_meteo-0.1.0/earthkit/meteo/solar/
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/solar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.202790 earthkit_meteo-0.1.0/earthkit/meteo/solar/array/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/solar/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/solar/array/solar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/solar/solar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.202790 earthkit_meteo-0.1.0/earthkit/meteo/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/stats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.202790 earthkit_meteo-0.1.0/earthkit/meteo/stats/array/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/stats/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/stats/array/numpy_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/stats/array/quantiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/stats/numpy_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/stats/quantiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.202790 earthkit_meteo-0.1.0/earthkit/meteo/thermo/
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/thermo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.202790 earthkit_meteo-0.1.0/earthkit/meteo/thermo/array/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/thermo/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51773 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/thermo/array/thermo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/thermo/thermo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-25 09:11:15.000000 earthkit_meteo-0.1.0/earthkit/meteo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.206790 earthkit_meteo-0.1.0/earthkit/meteo/wind/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/wind/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.206790 earthkit_meteo-0.1.0/earthkit/meteo/wind/array/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/wind/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/wind/array/wind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/earthkit/meteo/wind/wind.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.210790 earthkit_meteo-0.1.0/earthkit_meteo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-25 09:11:15.000000 earthkit_meteo-0.1.0/earthkit_meteo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-25 09:11:15.000000 earthkit_meteo-0.1.0/earthkit_meteo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:11:15.000000 earthkit_meteo-0.1.0/earthkit_meteo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-25 09:11:15.000000 earthkit_meteo-0.1.0/earthkit_meteo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 09:11:15.000000 earthkit_meteo-0.1.0/earthkit_meteo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-25 09:11:15.210790 earthkit_meteo-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.206790 earthkit_meteo-0.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.210790 earthkit_meteo-0.1.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    72061 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/data/eqpt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/data/sat_mr.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/data/sat_mr_slope.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/data/sat_q.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/data/sat_q_slope.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/data/sat_vp.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/data/sat_vp_slope.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    36024 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/data/seqpt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    60013 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/data/t_hum_p_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    16705 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/data/t_on_most_adiabat.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   142545 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/data/t_wet.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   214331 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/data/t_wetpt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/downstream-ci-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/environment-unit-tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.210790 earthkit_meteo-0.1.0/tests/extreme/
+-rw-r--r--   0 runner    (1001) docker     (127)    23954 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/extreme/test_extreme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.210790 earthkit_meteo-0.1.0/tests/score/
+-rw-r--r--   0 runner    (1001) docker     (127)    21959 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/score/test_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.210790 earthkit_meteo-0.1.0/tests/solar/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/solar/test_solar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.210790 earthkit_meteo-0.1.0/tests/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/stats/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.210790 earthkit_meteo-0.1.0/tests/thermo/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/thermo/test_thermo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23563 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/thermo/test_thermo_array.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:11:15.210790 earthkit_meteo-0.1.0/tests/wind/
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-25 09:11:04.000000 earthkit_meteo-0.1.0/tests/wind/test_wind.py
```

### Comparing `earthkit-meteo-0.0.1/.github/workflows/ci.yml` & `earthkit_meteo-0.1.0/.github/workflows/legacy-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: ci
+name: legacy-ci
 
 on:
   push:
     branches:
     - main
     - develop
     tags:
```

### Comparing `earthkit-meteo-0.0.1/.gitignore` & `earthkit_meteo-0.1.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -353,11 +353,14 @@
 *.rej
 
 # mac
 .DS_Store
 
 # local code
 _dev
+_util
 ?
 ?.*
 tempCodeRunnerFile*
 dev/
+_util
+docs/experimental
```

### Comparing `earthkit-meteo-0.0.1/.pre-commit-config.yaml` & `earthkit_meteo-0.1.0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -11,38 +11,37 @@
   - id: debug-statements
   - id: mixed-line-ending
 - repo: https://github.com/PyCQA/isort
   rev: 5.12.0
   hooks:
   - id: isort
 - repo: https://github.com/psf/black
-  rev: 23.3.0
+  rev: 23.9.1
   hooks:
   - id: black
 - repo: https://github.com/keewis/blackdoc
   rev: v0.3.8
   hooks:
   - id: blackdoc
     additional_dependencies: [black==23.3.0]
 - repo: https://github.com/PyCQA/flake8
-  rev: 4.0.1
+  rev: 6.1.0
   hooks:
   - id: flake8
 - repo: https://github.com/executablebooks/mdformat
   rev: 0.7.14
   hooks:
   - id: mdformat
     exclude: cruft-update-template.md
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.4.0
+  rev: v2.11.0
   hooks:
   - id: pretty-format-yaml
     args: [--autofix, --preserve-quotes]
   - id: pretty-format-toml
     args: [--autofix]
-    additional_dependencies: [toml-sort<0.22.0]
 - repo: https://github.com/PyCQA/pydocstyle.git
   rev: 6.1.1
   hooks:
   - id: pydocstyle
     additional_dependencies: [toml]
     exclude: tests|docs
```

### Comparing `earthkit-meteo-0.0.1/LICENSE` & `earthkit_meteo-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `earthkit-meteo-0.0.1/Makefile` & `earthkit_meteo-0.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `earthkit-meteo-0.0.1/PKG-INFO` & `earthkit_meteo-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-Metadata-Version: 2.1
-Name: earthkit-meteo
-Version: 0.0.1
-Summary: Meteorological computations
-License: Apache License 2.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # earthkit-meteo
 
-Meteorological computations.
+<!--
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/earthkit-meteo.svg)](https://pypi.python.org/pypi/earthkit-meteo/) -->
 
 **DISCLAIMER**
 This project is **BETA** and will be **Experimental** for the foreseeable future.
 Interfaces and functionality are likely to change, and the project itself may be scrapped.
 **DO NOT** use this software in any project/software that is operational.
 
+**earthkit-meteo** is a Python package providing meteorological computations using **numpy** input and output.
+
+```python
+from earthkit.meteo import thermo
+import numpy as np
+
+t = np.array([264.12, 261.45]) # Kelvins
+p = np.array([850, 850]) * 100. # Pascals
+
+theta = thermo.potential_temperature(t, p)
+```
+
 ## Documentation
 
 The documentation can be found at https://earthkit-meteo.readthedocs.io/.
 
 ## Install
 
 Install via `pip` with:
```

### Comparing `earthkit-meteo-0.0.1/docs/Makefile` & `earthkit_meteo-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `earthkit-meteo-0.0.1/docs/_static/earthkit-meteo.png` & `earthkit_meteo-0.1.0/docs/_static/earthkit-meteo.png`

 * *Files identical despite different names*

### Comparing `earthkit-meteo-0.0.1/docs/_static/style.css` & `earthkit_meteo-0.1.0/docs/_static/style.css`

 * *Files identical despite different names*

### Comparing `earthkit-meteo-0.0.1/docs/conf.py` & `earthkit_meteo-0.1.0/docs/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     "show-module-summary",
     "imported-members",
     "inherited-members",
 ]
 autoapi_root = "_api"
 autoapi_member_order = "alphabetical"
 autoapi_add_toctree_entry = False
+autoapi_own_page_level = "function"
 
 # napoleon configuration
 napoleon_google_docstring = False
 napoleon_numpy_docstring = True
 napoleon_preprocess_types = True
 
 # Add any paths that contain templates here, relative to this directory.
@@ -82,7 +83,13 @@
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 html_css_files = ["style.css"]
 
 html_logo = "_static/earthkit-meteo.png"
+
+
+def setup(app):
+    from skip_api_rules import _skip_api_items
+
+    app.connect("autoapi-skip-member", _skip_api_items)
```

### Comparing `earthkit-meteo-0.0.1/docs/development.rst` & `earthkit_meteo-0.1.0/docs/development.rst`

 * *Files identical despite different names*

### Comparing `earthkit-meteo-0.0.1/docs/licence.rst` & `earthkit_meteo-0.1.0/docs/licence.rst`

 * *Files identical despite different names*

### Comparing `earthkit-meteo-0.0.1/docs/make.bat` & `earthkit_meteo-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `earthkit-meteo-0.0.1/earthkit/meteo/__init__.py` & `earthkit_meteo-0.1.0/earthkit/meteo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# (C) Copyright 2023 ECMWF.
+# (C) Copyright 2021 ECMWF.
 #
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
-
+#
 
 try:
     # NOTE: the `version.py` file must not be present in the git repository
     #   as it is generated by setuptools at install time
     from .version import __version__
 except ImportError:  # pragma: no cover
     # Local copy or not installed with setuptools
```

### Comparing `earthkit-meteo-0.0.1/earthkit/meteo/solar/__init__.py` & `earthkit_meteo-0.1.0/earthkit/meteo/solar/array/solar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# (C) Copyright 2023 ECMWF.
+# (C) Copyright 2021 ECMWF.
 #
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
+#
 
 import datetime
 
 import numpy as np
 
 DAYS_PER_YEAR = 365.25
```

### Comparing `earthkit-meteo-0.0.1/setup.cfg` & `earthkit_meteo-0.1.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -21,14 +21,19 @@
 packages = find_namespace:
 install_requires = 
 	numpy
 
 [options.packages.find]
 include = earthkit.*
 
+[options.extras_require]
+test = 
+	pytest
+	pytest-cov
+
 [flake8]
 max-line-length = 110
 extend-ignore = E203, W503
 
 [mypy]
 strict = False
 ignore_missing_imports = True
```


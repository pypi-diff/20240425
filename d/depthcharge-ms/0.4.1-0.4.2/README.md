# Comparing `tmp/depthcharge_ms-0.4.1.tar.gz` & `tmp/depthcharge_ms-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depthcharge_ms-0.4.1.tar", last modified: Fri Apr 19 22:23:28 2024, max compression
+gzip compressed data, was "depthcharge_ms-0.4.2.tar", last modified: Thu Apr 25 06:27:56 2024, max compression
```

## Comparing `depthcharge_ms-0.4.1.tar` & `depthcharge_ms-0.4.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.142728 depthcharge_ms-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.126728 depthcharge_ms-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.130728 depthcharge_ms-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-19 22:23:28.142728 depthcharge_ms-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.130728 depthcharge_ms-0.4.1/data/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/data/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/data/TMT10-Trial-8.mgf
--rw-r--r--   0 runner    (1001) docker     (127)   333839 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/data/TMT10-Trial-8.mzML
--rw-r--r--   0 runner    (1001) docker     (127)    67798 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/data/TMT10-Trial-8.mzXML
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.130728 depthcharge_ms-0.4.1/depthcharge/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.134728 depthcharge_ms-0.4.1/depthcharge/data/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/data/analyte_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12035 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/data/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/data/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    18919 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/data/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/data/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    18401 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/data/spectrum_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.134728 depthcharge_ms-0.4.1/depthcharge/encoders/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/encoders/sinusoidal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/feedforward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.134728 depthcharge_ms-0.4.1/depthcharge/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/tokenizers/molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/tokenizers/peptides.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/tokenizers/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.134728 depthcharge_ms-0.4.1/depthcharge/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/transformers/analytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/transformers/spectra.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/depthcharge/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.138728 depthcharge_ms-0.4.1/depthcharge_ms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-19 22:23:28.000000 depthcharge_ms-0.4.1/depthcharge_ms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-19 22:23:28.000000 depthcharge_ms-0.4.1/depthcharge_ms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 22:23:28.000000 depthcharge_ms-0.4.1/depthcharge_ms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-19 22:23:28.000000 depthcharge_ms-0.4.1/depthcharge_ms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 22:23:28.000000 depthcharge_ms-0.4.1/depthcharge_ms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.134728 depthcharge_ms-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.134728 depthcharge_ms-0.4.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/api/datasets.md
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/api/encoders.md
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/api/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/api/primitives.md
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/api/tokenizers.md
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/api/transformers.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.138728 depthcharge_ms-0.4.1/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/getting-started/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     9968 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/getting-started/spectra.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.138728 depthcharge_ms-0.4.1/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 22:23:28.142728 depthcharge_ms-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.138728 depthcharge_ms-0.4.1/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/static/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    50058 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/static/logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    46385 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/static/logo-light.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.138728 depthcharge_ms-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.138728 depthcharge_ms-0.4.1/tests/unit_tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.138728 depthcharge_ms-0.4.1/tests/unit_tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_data/test_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_data/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_data/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_data/test_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.138728 depthcharge_ms-0.4.1/tests/unit_tests/test_encoders/
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_encoders/test_sinusoidal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_feedforward.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.138728 depthcharge_ms-0.4.1/tests/unit_tests/test_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_tokenizers/test_molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_tokenizers/test_peptides.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:23:28.138728 depthcharge_ms-0.4.1/tests/unit_tests/test_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_transformers/test_analyte_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_transformers/test_spectrum_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-19 22:23:17.000000 depthcharge_ms-0.4.1/tests/unit_tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.333618 depthcharge_ms-0.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.317618 depthcharge_ms-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.321618 depthcharge_ms-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-25 06:27:56.333618 depthcharge_ms-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.321618 depthcharge_ms-0.4.2/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/data/TMT10-Trial-8.mgf
+-rw-r--r--   0 runner    (1001) docker     (127)   333839 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/data/TMT10-Trial-8.mzML
+-rw-r--r--   0 runner    (1001) docker     (127)    67798 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/data/TMT10-Trial-8.mzXML
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.325618 depthcharge_ms-0.4.2/depthcharge/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.325618 depthcharge_ms-0.4.2/depthcharge/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/data/analyte_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12035 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/data/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/data/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18919 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/data/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/data/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18603 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/data/spectrum_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.325618 depthcharge_ms-0.4.2/depthcharge/encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/encoders/sinusoidal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.325618 depthcharge_ms-0.4.2/depthcharge/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/tokenizers/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/tokenizers/peptides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/tokenizers/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.325618 depthcharge_ms-0.4.2/depthcharge/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/transformers/analytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/transformers/spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/depthcharge/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.333618 depthcharge_ms-0.4.2/depthcharge_ms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-25 06:27:56.000000 depthcharge_ms-0.4.2/depthcharge_ms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-25 06:27:56.000000 depthcharge_ms-0.4.2/depthcharge_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 06:27:56.000000 depthcharge_ms-0.4.2/depthcharge_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-25 06:27:56.000000 depthcharge_ms-0.4.2/depthcharge_ms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 06:27:56.000000 depthcharge_ms-0.4.2/depthcharge_ms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.329618 depthcharge_ms-0.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/docs/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.329618 depthcharge_ms-0.4.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/docs/api/datasets.md
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/docs/api/encoders.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/docs/api/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/docs/api/primitives.md
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/docs/api/tokenizers.md
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/docs/api/transformers.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.329618 depthcharge_ms-0.4.2/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/docs/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9968 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/docs/getting-started/spectra.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.329618 depthcharge_ms-0.4.2/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 06:27:56.333618 depthcharge_ms-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.329618 depthcharge_ms-0.4.2/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    50058 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/static/logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46385 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/static/logo-light.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.329618 depthcharge_ms-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.329618 depthcharge_ms-0.4.2/tests/unit_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.329618 depthcharge_ms-0.4.2/tests/unit_tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/tests/unit_tests/test_data/test_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/tests/unit_tests/test_data/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/tests/unit_tests/test_data/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/tests/unit_tests/test_data/test_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.329618 depthcharge_ms-0.4.2/tests/unit_tests/test_encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/tests/unit_tests/test_encoders/test_sinusoidal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/tests/unit_tests/test_feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/tests/unit_tests/test_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/tests/unit_tests/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.329618 depthcharge_ms-0.4.2/tests/unit_tests/test_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/tests/unit_tests/test_tokenizers/test_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/tests/unit_tests/test_tokenizers/test_peptides.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:27:56.333618 depthcharge_ms-0.4.2/tests/unit_tests/test_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/tests/unit_tests/test_transformers/test_analyte_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/tests/unit_tests/test_transformers/test_spectrum_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-25 06:27:45.000000 depthcharge_ms-0.4.2/tests/unit_tests/test_version.py
```

### Comparing `depthcharge_ms-0.4.1/.github/workflows/docs.yml` & `depthcharge_ms-0.4.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/.github/workflows/lint.yml` & `depthcharge_ms-0.4.2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/.github/workflows/publish.yml` & `depthcharge_ms-0.4.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/.github/workflows/tests.yml` & `depthcharge_ms-0.4.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/CHANGELOG.md` & `depthcharge_ms-0.4.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v0.4.2]
+
+### Changed
+- The length of `SpectrumDataset` and `AnnotatedSpectrumDataset` is now the number of batches, not the number of spectra. This let's tools like PyTorch Lighting create their progress bars properly.
+- Parsing a dataset now no longer requires reading essentially the whole first file. Now the schema is inferred from the first 128 spectra.
+
 ## [v0.4.1]
 
 ### Added
 - Significant updates to documentation. Add how to model mass spectra.
 - Reading and writing from cloud storage on everything!
 
 ### Changed
```

### Comparing `depthcharge_ms-0.4.1/CODE_OF_CONDUCT.md` & `depthcharge_ms-0.4.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/CONTRIBUTING.md` & `depthcharge_ms-0.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/LICENSE` & `depthcharge_ms-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/PKG-INFO` & `depthcharge_ms-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthcharge-ms
-Version: 0.4.1
+Version: 0.4.2
 Summary: A mass spectrometry toolkit for deep learning with Transformer models.
 Author-email: "William E. Fondrie" <fondriew@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/wfondrie/depthcharge
 Project-URL: Documentation, https://wfondrie.github.io/depthcharge
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `depthcharge_ms-0.4.1/README.md` & `depthcharge_ms-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/data/TMT10-Trial-8.mgf` & `depthcharge_ms-0.4.2/data/TMT10-Trial-8.mgf`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/data/TMT10-Trial-8.mzML` & `depthcharge_ms-0.4.2/data/TMT10-Trial-8.mzML`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/data/TMT10-Trial-8.mzXML` & `depthcharge_ms-0.4.2/data/TMT10-Trial-8.mzXML`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/depthcharge/__init__.py` & `depthcharge_ms-0.4.2/depthcharge/__init__.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/depthcharge/data/analyte_datasets.py` & `depthcharge_ms-0.4.2/depthcharge/data/analyte_datasets.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/depthcharge/data/arrow.py` & `depthcharge_ms-0.4.2/depthcharge/data/arrow.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/depthcharge/data/fields.py` & `depthcharge_ms-0.4.2/depthcharge/data/fields.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/depthcharge/data/parsers.py` & `depthcharge_ms-0.4.2/depthcharge/data/parsers.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/depthcharge/data/preprocessing.py` & `depthcharge_ms-0.4.2/depthcharge/data/preprocessing.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/depthcharge/data/spectrum_datasets.py` & `depthcharge_ms-0.4.2/depthcharge/data/spectrum_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Serve mass spectra to neural networks."""
 
 from __future__ import annotations
 
+import copy
 import logging
+import math
 import uuid
 from collections.abc import Generator, Iterable
 from os import PathLike
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Any
 
@@ -84,28 +86,32 @@
         batch_size: int,
         path: PathLike | None = None,
         parse_kwargs: dict | None = None,
         **kwargs: dict,
     ) -> None:
         """Initialize a SpectrumDataset."""
         self._parse_kwargs = {} if parse_kwargs is None else parse_kwargs
+        self._init_kwargs = copy.copy(self._parse_kwargs)
+        self._init_kwargs["batch_size"] = 128
+        self._init_kwargs["progress"] = False
+
         self._tmpdir = None
         if path is None:
             # Create a random temporary file:
             self._tmpdir = TemporaryDirectory()
             path = Path(self._tmpdir.name) / f"{uuid.uuid4()}.lance"
 
         self._path = AnyPath(path)
         if self._path.suffix != ".lance":
             self._path = self._path.with_suffix(".lance")
 
         # Now parse spectra.
         if spectra is not None:
             spectra = utils.listify(spectra)
-            batch = next(_get_records(spectra, **self._parse_kwargs))
+            batch = next(_get_records(spectra, **self._init_kwargs))
             lance.write_dataset(
                 _get_records(spectra, **self._parse_kwargs),
                 str(self._path),
                 mode="overwrite" if self._path.exists() else "create",
                 schema=batch.schema,
             )
 
@@ -133,15 +139,15 @@
             Spectra to add to this collection. These may be a DataFrame parsed
             with `depthcharge.spectra_to_df()`, parquet files created with
             `depthcharge.spectra_to_parquet()`, or a peak file in the mzML,
             mzXML, or MGF format.
 
         """
         spectra = utils.listify(spectra)
-        batch = next(_get_records(spectra, **self._parse_kwargs))
+        batch = next(_get_records(spectra, **self._init_kwargs))
         self._dataset = lance.write_dataset(
             _get_records(spectra, **self._parse_kwargs),
             self._path,
             mode="append",
             schema=batch.schema,
         )
 
@@ -163,16 +169,16 @@
             row. List columns are automatically converted to
             PyTorch tensors if the nested data type is compatible.
 
         """
         return self._to_tensor(self._dataset.take(utils.listify(idx)))
 
     def __len__(self) -> int:
-        """The number of spectra in the lance dataset."""
-        return self._dataset.count_rows()
+        """The number of batches in the lance dataset."""
+        return math.ceil(self._dataset.count_rows() / self.batch_size)
 
     def __del__(self) -> None:
         """Cleanup the temporary directory."""
         if self._tmpdir is not None:
             self._tmpdir.cleanup()
 
     @property
```

### Comparing `depthcharge_ms-0.4.1/depthcharge/encoders/sinusoidal.py` & `depthcharge_ms-0.4.2/depthcharge/encoders/sinusoidal.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/depthcharge/feedforward.py` & `depthcharge_ms-0.4.2/depthcharge/feedforward.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/depthcharge/mixins.py` & `depthcharge_ms-0.4.2/depthcharge/mixins.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/depthcharge/primitives.py` & `depthcharge_ms-0.4.2/depthcharge/primitives.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/depthcharge/testing.py` & `depthcharge_ms-0.4.2/depthcharge/testing.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/depthcharge/tokenizers/molecules.py` & `depthcharge_ms-0.4.2/depthcharge/tokenizers/molecules.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/depthcharge/tokenizers/peptides.py` & `depthcharge_ms-0.4.2/depthcharge/tokenizers/peptides.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/depthcharge/tokenizers/tokenizer.py` & `depthcharge_ms-0.4.2/depthcharge/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/depthcharge/transformers/analytes.py` & `depthcharge_ms-0.4.2/depthcharge/transformers/analytes.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/depthcharge/transformers/spectra.py` & `depthcharge_ms-0.4.2/depthcharge/transformers/spectra.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/depthcharge/utils.py` & `depthcharge_ms-0.4.2/depthcharge/utils.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/depthcharge_ms.egg-info/PKG-INFO` & `depthcharge_ms-0.4.2/depthcharge_ms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthcharge-ms
-Version: 0.4.1
+Version: 0.4.2
 Summary: A mass spectrometry toolkit for deep learning with Transformer models.
 Author-email: "William E. Fondrie" <fondriew@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/wfondrie/depthcharge
 Project-URL: Documentation, https://wfondrie.github.io/depthcharge
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `depthcharge_ms-0.4.1/depthcharge_ms.egg-info/SOURCES.txt` & `depthcharge_ms-0.4.2/depthcharge_ms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/docs/CHANGELOG.md` & `depthcharge_ms-0.4.2/docs/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v0.4.2]
+
+### Changed
+- The length of `SpectrumDataset` and `AnnotatedSpectrumDataset` is now the number of batches, not the number of spectra. This let's tools like PyTorch Lighting create their progress bars properly.
+- Parsing a dataset now no longer requires reading essentially the whole first file. Now the schema is inferred from the first 128 spectra.
+
 ## [v0.4.1]
 
 ### Added
 - Significant updates to documentation. Add how to model mass spectra.
 - Reading and writing from cloud storage on everything!
 
 ### Changed
```

### Comparing `depthcharge_ms-0.4.1/docs/CODE_OF_CONDUCT.md` & `depthcharge_ms-0.4.2/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/docs/CONTRIBUTING.md` & `depthcharge_ms-0.4.2/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/docs/api/index.md` & `depthcharge_ms-0.4.2/docs/api/index.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/docs/getting-started/installation.md` & `depthcharge_ms-0.4.2/docs/getting-started/installation.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/docs/getting-started/spectra.qmd` & `depthcharge_ms-0.4.2/docs/getting-started/spectra.qmd`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/docs/index.md` & `depthcharge_ms-0.4.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/docs/stylesheets/extra.css` & `depthcharge_ms-0.4.2/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/mkdocs.yml` & `depthcharge_ms-0.4.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/pyproject.toml` & `depthcharge_ms-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/static/icon.svg` & `depthcharge_ms-0.4.2/static/icon.svg`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/static/logo-dark.png` & `depthcharge_ms-0.4.2/static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/static/logo-light.png` & `depthcharge_ms-0.4.2/static/logo-light.png`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/tests/conftest.py` & `depthcharge_ms-0.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/tests/unit_tests/test_data/test_arrow.py` & `depthcharge_ms-0.4.2/tests/unit_tests/test_data/test_arrow.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/tests/unit_tests/test_data/test_datasets.py` & `depthcharge_ms-0.4.2/tests/unit_tests/test_data/test_datasets.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/tests/unit_tests/test_data/test_loaders.py` & `depthcharge_ms-0.4.2/tests/unit_tests/test_data/test_loaders.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/tests/unit_tests/test_data/test_parsers.py` & `depthcharge_ms-0.4.2/tests/unit_tests/test_data/test_parsers.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/tests/unit_tests/test_encoders/test_sinusoidal.py` & `depthcharge_ms-0.4.2/tests/unit_tests/test_encoders/test_sinusoidal.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/tests/unit_tests/test_feedforward.py` & `depthcharge_ms-0.4.2/tests/unit_tests/test_feedforward.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/tests/unit_tests/test_primitives.py` & `depthcharge_ms-0.4.2/tests/unit_tests/test_primitives.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/tests/unit_tests/test_testing.py` & `depthcharge_ms-0.4.2/tests/unit_tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/tests/unit_tests/test_tokenizers/test_molecules.py` & `depthcharge_ms-0.4.2/tests/unit_tests/test_tokenizers/test_molecules.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/tests/unit_tests/test_tokenizers/test_peptides.py` & `depthcharge_ms-0.4.2/tests/unit_tests/test_tokenizers/test_peptides.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/tests/unit_tests/test_transformers/test_analyte_transformers.py` & `depthcharge_ms-0.4.2/tests/unit_tests/test_transformers/test_analyte_transformers.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/tests/unit_tests/test_transformers/test_spectrum_transformers.py` & `depthcharge_ms-0.4.2/tests/unit_tests/test_transformers/test_spectrum_transformers.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.1/tests/unit_tests/test_version.py` & `depthcharge_ms-0.4.2/tests/unit_tests/test_version.py`

 * *Files identical despite different names*


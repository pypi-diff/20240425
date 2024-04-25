# Comparing `tmp/ansible_dev_tools-24.4.0.tar.gz` & `tmp/ansible_dev_tools-24.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_dev_tools-24.4.0.tar", last modified: Mon Apr 22 14:46:00 2024, max compression
+gzip compressed data, was "ansible_dev_tools-24.4.1.tar", last modified: Thu Apr 25 15:52:43 2024, max compression
```

## Comparing `ansible_dev_tools-24.4.0.tar` & `ansible_dev_tools-24.4.1.tar`

### file list

```diff
@@ -1,72 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:46:00.930931 ansible_dev_tools-24.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:46:00.922931 ansible_dev_tools-24.4.0/.config/
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/.config/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/.config/requirements-docs.in
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/.config/requirements-lock.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/.config/requirements-test.in
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/.config/requirements.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:46:00.922931 ansible_dev_tools-24.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:46:00.922931 ansible_dev_tools-24.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:46:00.922931 ansible_dev_tools-24.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-22 14:46:00.930931 ansible_dev_tools-24.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:46:00.922931 ansible_dev_tools-24.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/docs/contributor-guide.md
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:46:00.926931 ansible_dev_tools-24.4.0/docs/media/
--rw-r--r--   0 runner    (1001) docker     (127)   351712 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/docs/media/ansible-lint.mp4
--rw-r--r--   0 runner    (1001) docker     (127)   185365 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/docs/media/ansible-navigator-run.mp4
--rwxr-xr-x   0 runner    (1001) docker     (127)      136 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/docs/media/compress.sh
--rw-r--r--   0 runner    (1001) docker     (127)   325589 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/docs/media/create-collection.mp4
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:46:00.926931 ansible_dev_tools-24.4.0/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/docs/user-guide/building-collection.md
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/docs/user-guide/ci-setup.md
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/docs/user-guide/content-best-practices.md
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/docs/user-guide/content-release.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:46:00.926931 ansible_dev_tools-24.4.0/docs/user-guide/images/
--rw-r--r--   0 runner    (1001) docker     (127)    75270 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/docs/user-guide/images/ci.png
--rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/docs/user-guide/images/release.png
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/docs/user-guide/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/docs/user-guide/testing.md
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11119 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 14:46:00.930931 ansible_dev_tools-24.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:46:00.918931 ansible_dev_tools-24.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:46:00.926931 ansible_dev_tools-24.4.0/src/ansible_dev_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/src/ansible_dev_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/src/ansible_dev_tools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-22 14:46:00.000000 ansible_dev_tools-24.4.0/src/ansible_dev_tools/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/src/ansible_dev_tools/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/src/ansible_dev_tools/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/src/ansible_dev_tools/version_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:46:00.930931 ansible_dev_tools-24.4.0/src/ansible_dev_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-22 14:46:00.000000 ansible_dev_tools-24.4.0/src/ansible_dev_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-22 14:46:00.000000 ansible_dev_tools-24.4.0/src/ansible_dev_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 14:46:00.000000 ansible_dev_tools-24.4.0/src/ansible_dev_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-22 14:46:00.000000 ansible_dev_tools-24.4.0/src/ansible_dev_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-22 14:46:00.000000 ansible_dev_tools-24.4.0/src/ansible_dev_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 14:46:00.000000 ansible_dev_tools-24.4.0/src/ansible_dev_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:46:00.930931 ansible_dev_tools-24.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:46:00.930931 ansible_dev_tools-24.4.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/tests/integration/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-22 14:45:51.000000 ansible_dev_tools-24.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.906848 ansible_dev_tools-24.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.894848 ansible_dev_tools-24.4.1/.config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.config/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.config/requirements-docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.config/requirements-server.in
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.config/requirements-test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.config/requirements.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.894848 ansible_dev_tools-24.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.894848 ansible_dev_tools-24.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.894848 ansible_dev_tools-24.4.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-25 15:52:43.906848 ansible_dev_tools-24.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.894848 ansible_dev_tools-24.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/contributor-guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.898848 ansible_dev_tools-24.4.1/docs/media/
+-rw-r--r--   0 runner    (1001) docker     (127)   351712 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/media/ansible-lint.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)   185365 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/media/ansible-navigator-run.mp4
+-rwxr-xr-x   0 runner    (1001) docker     (127)      136 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/media/compress.sh
+-rw-r--r--   0 runner    (1001) docker     (127)   325589 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/media/create-collection.mp4
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.898848 ansible_dev_tools-24.4.1/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/user-guide/building-collection.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/user-guide/ci-setup.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/user-guide/content-best-practices.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/user-guide/content-release.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.898848 ansible_dev_tools-24.4.1/docs/user-guide/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    75270 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/user-guide/images/ci.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/user-guide/images/release.png
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/user-guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/docs/user-guide/testing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:52:43.906848 ansible_dev_tools-24.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.890848 ansible_dev_tools-24.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.902848 ansible_dev_tools-24.4.1/src/ansible_dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-25 15:52:43.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.890848 ansible_dev_tools-24.4.1/src/ansible_dev_tools/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.902848 ansible_dev_tools-24.4.1/src/ansible_dev_tools/resources/server/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/resources/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/resources/server/creator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.902848 ansible_dev_tools-24.4.1/src/ansible_dev_tools/resources/server/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/resources/server/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/resources/server/data/openapi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/server_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.902848 ansible_dev_tools-24.4.1/src/ansible_dev_tools/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/subcommands/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools/version_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.906848 ansible_dev_tools-24.4.1/src/ansible_dev_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-25 15:52:43.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-25 15:52:43.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:52:43.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 15:52:43.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-25 15:52:43.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 15:52:43.000000 ansible_dev_tools-24.4.1/src/ansible_dev_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.902848 ansible_dev_tools-24.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:52:43.906848 ansible_dev_tools-24.4.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/tests/integration/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/tests/integration/test_server_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-25 15:52:34.000000 ansible_dev_tools-24.4.1/tox.ini
```

### Comparing `ansible_dev_tools-24.4.0/.config/constraints.txt` & `ansible_dev_tools-24.4.1/.config/constraints.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.12
 # by the following command:
 #
 #    pip-compile --all-extras --no-annotate --output-file=.config/constraints.txt --strip-extras pyproject.toml
 #
 ansible-builder==3.0.1
 ansible-compat==4.1.11
 ansible-core==2.16.6
-ansible-creator==24.4.2
-ansible-dev-environment==24.1.1
+ansible-creator==24.4.3
+ansible-dev-environment==24.4.0
 ansible-lint==24.2.2
 ansible-navigator==24.2.0
 ansible-runner==2.3.6
 ansible-sign==0.1.1
+asgiref==3.8.1
 attrs==23.2.0
 babel==2.14.0
 beautifulsoup4==4.12.3
 bindep==2.11.0
 black==24.4.0
 bracex==2.4
 build==1.2.1
@@ -27,118 +28,137 @@
 cffi==1.16.0
 cfgv==3.4.0
 chardet==5.2.0
 charset-normalizer==3.3.2
 click==8.1.7
 click-help-colors==0.9.4
 colorama==0.4.6
-coverage==7.4.4
+coverage==7.5.0
 cryptography==42.0.5
 csscompressor==0.9.5
 cssselect2==0.7.0
 defusedxml==0.7.1
 distlib==0.3.8
 distro==1.9.0
+django==4.2.11
+django-stubs==4.2.7
+django-stubs-ext==4.2.7
 dnspython==2.6.1
 docstring-parser-fork==0.0.5
 docutils==0.21.1
 enrich==1.2.7
-exceptiongroup==1.2.0
 execnet==2.1.1
 filelock==3.13.4
 ghp-import==2.1.0
-griffe==0.42.2
+griffe==0.44.0
+gunicorn==22.0.0
 htmlmin2==0.1.13
-identify==2.5.35
+identify==2.5.36
 idna==3.7
 iniconfig==2.0.0
+isodate==0.6.1
 jinja2==3.1.3
 jsmin==3.0.1
 jsonschema==4.21.1
+jsonschema-path==0.3.2
 jsonschema-specifications==2023.12.1
+lazy-object-proxy==1.10.0
 linkchecker==10.4.0
 lockfile==0.12.2
 markdown==3.6
 markdown-exec==1.8.1
 markdown-include==0.8.1
 markdown-it-py==3.0.0
 markupsafe==2.1.5
 mdurl==0.1.2
 mergedeep==1.3.4
 mkdocs==1.5.3
 mkdocs-ansible==24.3.0
 mkdocs-autorefs==1.0.1
 mkdocs-gen-files==0.5.0
 mkdocs-htmlproofer-plugin==1.2.1
+mkdocs-macros-plugin==1.0.5
 mkdocs-material==9.5.18
 mkdocs-material-extensions==1.3.1
 mkdocs-minify-plugin==0.8.0
 mkdocs-monorepo-plugin==1.1.0
 mkdocstrings==0.24.3
-mkdocstrings-python==1.9.2
+mkdocstrings-python==1.10.0
 molecule==24.2.1
-mypy==1.9.0
+more-itertools==10.2.0
+mypy==1.7.1
 mypy-extensions==1.0.0
 nodeenv==1.8.0
 onigurumacffi==1.3.0
+openapi-core==0.19.1
+openapi-schema-validator==0.6.2
+openapi-spec-validator==0.7.1
 packaging==24.0
 paginate==0.5.6
+parse==1.20.1
 parsley==1.3
+pathable==0.4.3
 pathspec==0.12.1
 pbr==6.0.0
 pexpect==4.9.0
 pillow==10.3.0
 pip-tools==7.4.1
 pipdeptree==2.18.1
 platformdirs==4.2.0
 pluggy==1.4.0
 pre-commit==3.7.0
 ptyprocess==0.7.0
 pycparser==2.22
 pydoclint==0.4.1
 pygments==2.17.2
-pymdown-extensions==10.7.1
+pymdown-extensions==10.8
 pyproject-api==1.6.1
 pyproject-hooks==1.0.0
 pytest==8.1.1
 pytest-ansible==24.1.3
 pytest-xdist==3.5.0
 python-daemon==3.0.1
 python-dateutil==2.9.0.post0
 python-gnupg==0.5.2
 python-slugify==8.0.4
 pyyaml==6.0.1
 pyyaml-env-tag==0.1
-referencing==0.34.0
+referencing==0.31.1
 regex==2024.4.16
 requests==2.31.0
 requirements-parser==0.9.0
 resolvelib==1.0.1
+rfc3339-validator==0.1.4
 rich==13.7.1
 rpds-py==0.18.0
 ruamel-yaml==0.18.6
 ruamel-yaml-clib==0.2.8
-ruff==0.3.7
+ruff==0.4.1
 six==1.16.0
 soupsieve==2.5
+sqlparse==0.5.0
 subprocess-tee==0.4.1
+termcolor==2.4.0
 text-unidecode==1.3
-tinycss2==1.2.1
+tinycss2==1.3.0
 toml-sort==0.23.1
-tomli==2.0.1
 tomlkit==0.12.4
 tox==4.14.2
 tox-ansible==24.2.0
+types-pytz==2024.1.0.20240417
+types-pyyaml==6.0.12.20240311
+types-requests==2.31.0.20240406
 types-setuptools==69.5.0.20240415
 typing-extensions==4.11.0
 tzdata==2024.1
 urllib3==2.2.1
 virtualenv==20.25.2
 watchdog==4.0.0
 wcmatch==8.5.1
 webencodings==0.5.1
+werkzeug==3.0.2
 wheel==0.43.0
 yamllint==1.35.1
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `ansible_dev_tools-24.4.0/.github/dependabot.yml` & `ansible_dev_tools-24.4.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/.github/workflows/release.yml` & `ansible_dev_tools-24.4.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/.github/workflows/tox.yml` & `ansible_dev_tools-24.4.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/.gitignore` & `ansible_dev_tools-24.4.1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+/src/ansible_dev_tools/_version.py
+
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `ansible_dev_tools-24.4.0/.pre-commit-config.yaml` & `ansible_dev_tools-24.4.1/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -85,27 +85,38 @@
     hooks:
       - id: pylint
         args:
           - --output-format=colorized
         additional_dependencies:
           - pytest
           - tox
+          - PyYAML
+          - ansible-creator
+          - django
+          - openapi_core
+          - pytest
+          - gunicorn
 
   - repo: https://github.com/pre-commit/mirrors-mypy.git
     rev: v1.9.0
     hooks:
       - id: mypy
         additional_dependencies:
+          - django-stubs[compatible-mypy]
+          - jinja2
           - pytest
           - tox
+          - types-pyyaml
+          - types-requests
           - types-setuptools
         args:
           - src
           - tests
         pass_filenames: false
+        language_version: "3.10"
 
   - repo: https://github.com/jazzband/pip-tools
     rev: 7.4.1
     hooks:
       - id: pip-compile
         name: deps
         alias: deps
```

### Comparing `ansible_dev_tools-24.4.0/LICENSE` & `ansible_dev_tools-24.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/PKG-INFO` & `ansible_dev_tools-24.4.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-dev-tools
-Version: 24.4.0
+Version: 24.4.1
 Summary: Ansible Developtment Tools kit bundles all tools needed for content creation and testing.
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: GPL-3.0-only
 Project-URL: changelog, https://github.com/ansible/ansible-dev-tools/releases
 Project-URL: documentation, https://ansible.readthedocs.io/projects/dev-tools/
 Project-URL: homepage, https://github.com/ansible/ansible-dev-tools
@@ -42,16 +42,24 @@
 Requires-Dist: black; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pip-tools; extra == "test"
 Requires-Dist: pre-commit; extra == "test"
 Requires-Dist: pydoclint; extra == "test"
 Requires-Dist: pytest; extra == "test"
+Requires-Dist: requests; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: toml-sort; extra == "test"
+Requires-Dist: types-pyyaml; extra == "test"
+Requires-Dist: types-requests; extra == "test"
+Requires-Dist: django-stubs[compatible-mypy]; extra == "test"
+Provides-Extra: server
+Requires-Dist: django<4.3,>4.1; extra == "server"
+Requires-Dist: gunicorn; extra == "server"
+Requires-Dist: openapi-core>=0.19.1; extra == "server"
 
 <!-- cspell:disable-next-line -->
 
 # Ansible Development Tools (ADT)
 
 The `ansible-dev-tools` python package provides an easy way to install and discover the best tools available to create and test ansible content.
 
@@ -96,10 +104,18 @@
 ansible-navigator                        <version>
 ansible-sign                             <version>
 molecule                                 <version>
 pytest-ansible                           <version>
 tox-ansible                              <version>
 ```
 
+## Developer Notes
+
+The `ansible-dev-tools` package also offers an Ansible Devtools server which can be launched with `adt server`. Currently, this server only supports REST APIs for `ansible-creator`.
+
+Refer to the [server](https://github.com/ansible/ansible-dev-tools/blob/main/src/ansible_dev_tools/subcommands/server.py) code for available endpoints.
+
+**Note:** This is primarily for backend integrations and is not intended to be an user-facing functionality.
+
 ## Documentation
 
 For more information, please visit our [documentation](https://ansible.readthedocs.io/projects/dev-tools/) page.
```

### Comparing `ansible_dev_tools-24.4.0/README.md` & `ansible_dev_tools-24.4.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -45,10 +45,18 @@
 ansible-navigator                        <version>
 ansible-sign                             <version>
 molecule                                 <version>
 pytest-ansible                           <version>
 tox-ansible                              <version>
 ```
 
+## Developer Notes
+
+The `ansible-dev-tools` package also offers an Ansible Devtools server which can be launched with `adt server`. Currently, this server only supports REST APIs for `ansible-creator`.
+
+Refer to the [server](https://github.com/ansible/ansible-dev-tools/blob/main/src/ansible_dev_tools/subcommands/server.py) code for available endpoints.
+
+**Note:** This is primarily for backend integrations and is not intended to be an user-facing functionality.
+
 ## Documentation
 
 For more information, please visit our [documentation](https://ansible.readthedocs.io/projects/dev-tools/) page.
```

### Comparing `ansible_dev_tools-24.4.0/cspell.config.yaml` & `ansible_dev_tools-24.4.1/cspell.config.yaml`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/docs/contributor-guide.md` & `ansible_dev_tools-24.4.1/docs/contributor-guide.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/docs/index.md` & `ansible_dev_tools-24.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/docs/installation.md` & `ansible_dev_tools-24.4.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/docs/media/ansible-lint.mp4` & `ansible_dev_tools-24.4.1/docs/media/ansible-lint.mp4`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/docs/media/ansible-navigator-run.mp4` & `ansible_dev_tools-24.4.1/docs/media/ansible-navigator-run.mp4`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/docs/media/create-collection.mp4` & `ansible_dev_tools-24.4.1/docs/media/create-collection.mp4`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/docs/user-guide/building-collection.md` & `ansible_dev_tools-24.4.1/docs/user-guide/building-collection.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/docs/user-guide/ci-setup.md` & `ansible_dev_tools-24.4.1/docs/user-guide/ci-setup.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/docs/user-guide/content-best-practices.md` & `ansible_dev_tools-24.4.1/docs/user-guide/content-best-practices.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/docs/user-guide/content-release.md` & `ansible_dev_tools-24.4.1/docs/user-guide/content-release.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/docs/user-guide/images/ci.png` & `ansible_dev_tools-24.4.1/docs/user-guide/images/ci.png`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/docs/user-guide/images/release.png` & `ansible_dev_tools-24.4.1/docs/user-guide/images/release.png`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/docs/user-guide/index.md` & `ansible_dev_tools-24.4.1/docs/user-guide/index.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/docs/user-guide/testing.md` & `ansible_dev_tools-24.4.1/docs/user-guide/testing.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/mkdocs.yml` & `ansible_dev_tools-24.4.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/pyproject.toml` & `ansible_dev_tools-24.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,18 @@
 homepage = "https://github.com/ansible/ansible-dev-tools"
 repository = "https://github.com/ansible/ansible-dev-tools"
 
 [tool.mypy]
 files = ["src", "tests"]
 strict = true
 
+[[tool.mypy.overrides]]
+ignore_missing_imports = true
+module = ["gunicorn.*", "openapi_core.*", "ansible_creator.*"]
+
 [tool.pydoclint]
 allow-init-docstring = true
 arg-type-hints-in-docstring = false
 check-return-types = false
 style = 'google'
 
 [tool.pylint]
@@ -228,14 +232,17 @@
   "W3301", # nested-min-max / ruff PLW3301
   "duplicate-code",
   "fixme",
   "too-few-public-methods",
   "unsubscriptable-object"
 ]
 
+[tool.pytest.ini_options]
+addopts = "-p no:pytest-ansible"
+
 [tool.ruff]
 builtins = ["__"]
 fix = true
 line-length = 100
 select = ["ALL"]
 target-version = "py310"
 
@@ -255,14 +262,15 @@
 [tool.ruff.pydocstyle]
 convention = "pep257"
 
 [tool.setuptools.dynamic]
 dependencies = {file = [".config/requirements.in"]}
 optional-dependencies.docs = {file = [".config/requirements-docs.in"]}
 optional-dependencies.test = {file = [".config/requirements-test.in"]}
+optional-dependencies.server = {file = [".config/requirements-server.in"]}
 
 [tool.setuptools_scm]
 # To prevent accidental pick of mobile version tags such 'v6'
 git_describe_command = [
   "git",
   "describe",
   "--dirty",
```

### Comparing `ansible_dev_tools-24.4.0/src/ansible_dev_tools/version_builder.py` & `ansible_dev_tools-24.4.1/src/ansible_dev_tools/version_builder.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.0/src/ansible_dev_tools.egg-info/PKG-INFO` & `ansible_dev_tools-24.4.1/src/ansible_dev_tools.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-dev-tools
-Version: 24.4.0
+Version: 24.4.1
 Summary: Ansible Developtment Tools kit bundles all tools needed for content creation and testing.
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: GPL-3.0-only
 Project-URL: changelog, https://github.com/ansible/ansible-dev-tools/releases
 Project-URL: documentation, https://ansible.readthedocs.io/projects/dev-tools/
 Project-URL: homepage, https://github.com/ansible/ansible-dev-tools
@@ -42,16 +42,24 @@
 Requires-Dist: black; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pip-tools; extra == "test"
 Requires-Dist: pre-commit; extra == "test"
 Requires-Dist: pydoclint; extra == "test"
 Requires-Dist: pytest; extra == "test"
+Requires-Dist: requests; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: toml-sort; extra == "test"
+Requires-Dist: types-pyyaml; extra == "test"
+Requires-Dist: types-requests; extra == "test"
+Requires-Dist: django-stubs[compatible-mypy]; extra == "test"
+Provides-Extra: server
+Requires-Dist: django<4.3,>4.1; extra == "server"
+Requires-Dist: gunicorn; extra == "server"
+Requires-Dist: openapi-core>=0.19.1; extra == "server"
 
 <!-- cspell:disable-next-line -->
 
 # Ansible Development Tools (ADT)
 
 The `ansible-dev-tools` python package provides an easy way to install and discover the best tools available to create and test ansible content.
 
@@ -96,10 +104,18 @@
 ansible-navigator                        <version>
 ansible-sign                             <version>
 molecule                                 <version>
 pytest-ansible                           <version>
 tox-ansible                              <version>
 ```
 
+## Developer Notes
+
+The `ansible-dev-tools` package also offers an Ansible Devtools server which can be launched with `adt server`. Currently, this server only supports REST APIs for `ansible-creator`.
+
+Refer to the [server](https://github.com/ansible/ansible-dev-tools/blob/main/src/ansible_dev_tools/subcommands/server.py) code for available endpoints.
+
+**Note:** This is primarily for backend integrations and is not intended to be an user-facing functionality.
+
 ## Documentation
 
 For more information, please visit our [documentation](https://ansible.readthedocs.io/projects/dev-tools/) page.
```

### Comparing `ansible_dev_tools-24.4.0/src/ansible_dev_tools.egg-info/SOURCES.txt` & `ansible_dev_tools-24.4.1/src/ansible_dev_tools.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 cspell.config.yaml
 mkdocs.yml
 pyproject.toml
 tox.ini
 .config/constraints.txt
 .config/dictionary.txt
 .config/requirements-docs.in
-.config/requirements-lock.txt
+.config/requirements-server.in
 .config/requirements-test.in
 .config/requirements.in
 .github/CODEOWNERS
 .github/CODE_OF_CONDUCT.md
 .github/dependabot.yml
 .github/release-drafter.yml
 .github/workflows/ack.yml
@@ -40,17 +40,27 @@
 docs/user-guide/images/ci.png
 docs/user-guide/images/release.png
 src/ansible_dev_tools/__init__.py
 src/ansible_dev_tools/__main__.py
 src/ansible_dev_tools/_version.py
 src/ansible_dev_tools/arg_parser.py
 src/ansible_dev_tools/cli.py
+src/ansible_dev_tools/server_utils.py
+src/ansible_dev_tools/utils.py
 src/ansible_dev_tools/version_builder.py
 src/ansible_dev_tools.egg-info/PKG-INFO
 src/ansible_dev_tools.egg-info/SOURCES.txt
 src/ansible_dev_tools.egg-info/dependency_links.txt
 src/ansible_dev_tools.egg-info/entry_points.txt
 src/ansible_dev_tools.egg-info/requires.txt
 src/ansible_dev_tools.egg-info/top_level.txt
+src/ansible_dev_tools/resources/server/__init__.py
+src/ansible_dev_tools/resources/server/creator.py
+src/ansible_dev_tools/resources/server/data/__init__.py
+src/ansible_dev_tools/resources/server/data/openapi.yaml
+src/ansible_dev_tools/subcommands/__init__.py
+src/ansible_dev_tools/subcommands/server.py
 tests/__init__.py
 tests/integration/__init__.py
-tests/integration/test_basic.py
+tests/integration/conftest.py
+tests/integration/test_cli.py
+tests/integration/test_server_creator.py
```

### Comparing `ansible_dev_tools-24.4.0/tox.ini` & `ansible_dev_tools-24.4.1/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 skip_missing_interpreters = true
 work_dir = {env:TOX_WORK_DIR:.tox}
 
 [testenv]
 description = Run pytest under {basepython} ({envpython})
 package = editable
 extras =
+    server
     test
 pass_env =
     CI
     CONTAINER_*
     DOCKER_*
     GITHUB_*
     HOME
```


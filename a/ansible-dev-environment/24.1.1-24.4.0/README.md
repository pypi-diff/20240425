# Comparing `tmp/ansible-dev-environment-24.1.1.tar.gz` & `tmp/ansible_dev_environment-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-dev-environment-24.1.1.tar", last modified: Wed Apr 10 10:43:25 2024, max compression
+gzip compressed data, was "ansible_dev_environment-24.4.0.tar", last modified: Thu Apr 25 15:20:14 2024, max compression
```

## Comparing `ansible-dev-environment-24.1.1.tar` & `ansible_dev_environment-24.4.0.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:43:25.059182 ansible-dev-environment-24.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:43:25.047181 ansible-dev-environment-24.1.1/.config/
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/.config/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/.config/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/.config/requirements-docs.in
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/.config/requirements-test.in
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/.config/requirements.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:43:25.047181 ansible-dev-environment-24.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:43:25.051182 ansible-dev-environment-24.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:43:25.051182 ansible-dev-environment-24.1.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-10 10:43:25.059182 ansible-dev-environment-24.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:43:25.051182 ansible-dev-environment-24.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:43:25.059182 ansible-dev-environment-24.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:43:25.043182 ansible-dev-environment-24.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:43:25.051182 ansible-dev-environment-24.1.1/src/ansible_dev_environment/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-10 10:43:24.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment/output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:43:25.055182 ansible-dev-environment-24.1.1/src/ansible_dev_environment/subcommands/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8161 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment/subcommands/checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment/subcommands/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)    18224 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment/subcommands/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment/subcommands/lister.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment/subcommands/treemaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment/subcommands/uninstaller.py
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    14630 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:43:25.055182 ansible-dev-environment-24.1.1/src/ansible_dev_environment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-10 10:43:25.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-10 10:43:25.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:43:25.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-10 10:43:25.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-10 10:43:25.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-10 10:43:25.000000 ansible-dev-environment-24.1.1/src/ansible_dev_environment.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:43:25.055182 ansible-dev-environment-24.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:43:25.055182 ansible-dev-environment-24.1.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/tests/fixtures/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/tests/fixtures/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:43:25.055182 ansible-dev-environment-24.1.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/tests/integration/test_basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:43:25.055182 ansible-dev-environment-24.1.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/tests/unit/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-10 10:43:12.000000 ansible-dev-environment-24.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.656499 ansible_dev_environment-24.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.644500 ansible_dev_environment-24.4.0/.config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.config/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.config/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.config/requirements-docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.config/requirements-test.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.config/requirements.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.644500 ansible_dev_environment-24.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.648500 ansible_dev_environment-24.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.648500 ansible_dev_environment-24.4.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-25 15:20:14.656499 ansible_dev_environment-24.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.648500 ansible_dev_environment-24.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:20:14.656499 ansible_dev_environment-24.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.640500 ansible_dev_environment-24.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.648500 ansible_dev_environment-24.4.0/src/ansible_dev_environment/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-25 15:20:14.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.652500 ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8161 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18224 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/lister.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/treemaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/uninstaller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14630 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.656499 ansible_dev_environment-24.4.0/src/ansible_dev_environment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-25 15:20:14.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-25 15:20:14.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:20:14.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-25 15:20:14.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-25 15:20:14.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 15:20:14.000000 ansible_dev_environment-24.4.0/src/ansible_dev_environment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.652500 ansible_dev_environment-24.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.652500 ansible_dev_environment-24.4.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/tests/fixtures/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/tests/fixtures/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.652500 ansible_dev_environment-24.4.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/tests/integration/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:20:14.652500 ansible_dev_environment-24.4.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/tests/unit/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-25 15:20:00.000000 ansible_dev_environment-24.4.0/tox.ini
```

### Comparing `ansible-dev-environment-24.1.1/.config/constraints.txt` & `ansible_dev_environment-24.4.0/.config/constraints.txt`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/.github/workflows/ack.yml` & `ansible_dev_environment-24.4.0/.github/workflows/ack.yml`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/.github/workflows/release.yml` & `ansible_dev_environment-24.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/.github/workflows/tox.yml` & `ansible_dev_environment-24.4.0/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/.gitignore` & `ansible_dev_environment-24.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/.pre-commit-config.yaml` & `ansible_dev_environment-24.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/.vscode/launch.json` & `ansible_dev_environment-24.4.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/.vscode/settings.json` & `ansible_dev_environment-24.4.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/LICENSE` & `ansible_dev_environment-24.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/PKG-INFO` & `ansible_dev_environment-24.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-dev-environment
-Version: 24.1.1
+Version: 24.4.0
 Summary: A pip-like ansible collection installer.
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Bradley Thornton <bthornto@redhat.com>
 License: GPL-3.0-only
 Project-URL: changelog, https://github.com/ansible/ansible-dev-environment/releases
 Project-URL: documentation, https://ansible.readthedocs.io/projects/dev-environment/
 Project-URL: homepage, https://github.com/ansible/ansible-dev-environment
```

### Comparing `ansible-dev-environment-24.1.1/README.md` & `ansible_dev_environment-24.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/cspell.config.yaml` & `ansible_dev_environment-24.4.0/cspell.config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/docs/index.md` & `ansible_dev_environment-24.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/mkdocs.yml` & `ansible_dev_environment-24.4.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/pyproject.toml` & `ansible_dev_environment-24.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/src/ansible_dev_environment/arg_parser.py` & `ansible_dev_environment-24.4.0/src/ansible_dev_environment/arg_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,14 +111,23 @@
         "--no-ansi",
         action="store_true",
         default=False,
         dest="no_ansi",
         help="Disable the use of ANSI codes for terminal hyperlink generation and color.",
     )
 
+    level1.add_argument(
+        "--ssp",
+        "--system-site-packages",
+        help="When building a virtual environment, give access to the system site-packages dir.",
+        default=False,
+        dest="system_site_packages",
+        action="store_true",
+    )
+
     common_args(level1)
 
     _check = subparsers.add_parser(
         "check",
         formatter_class=CustomHelpFormatter,
         parents=[level1],
         help="Check installed collections",
```

### Comparing `ansible-dev-environment-24.1.1/src/ansible_dev_environment/cli.py` & `ansible_dev_environment-24.4.0/src/ansible_dev_environment/cli.py`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/src/ansible_dev_environment/collection.py` & `ansible_dev_environment-24.4.0/src/ansible_dev_environment/collection.py`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/src/ansible_dev_environment/config.py` & `ansible_dev_environment-24.4.0/src/ansible_dev_environment/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -106,20 +106,23 @@
     ) -> None:
         """Set the interpreter."""
         if not self.venv.exists():
             if self._create_venv:
                 msg = f"Creating virtual environment: {self.venv}"
                 self._output.debug(msg)
                 command = f"python -m venv {self.venv}"
-                work = "Creating virtual environment"
+                msg = f"Creating virtual environment: {self.venv}"
+                if self.args.system_site_packages:
+                    command = f"{command} --system-site-packages"
+                    msg = f"Creating virtual environment with system site packages: {self.venv}"
                 try:
                     subprocess_run(
                         command=command,
                         verbose=self.args.verbose,
-                        msg=work,
+                        msg=msg,
                         output=self._output,
                     )
                     msg = f"Created virtual environment: {self.venv}"
                     self._output.info(msg)
                 except subprocess.CalledProcessError as exc:
                     err = f"Failed to create virtual environment: {exc}"
                     self._output.critical(err)
@@ -134,38 +137,42 @@
             self._output.critical(err)
 
         msg = f"Virtual environment interpreter: {venv_interpreter}"
         self._output.debug(msg)
         self.venv_interpreter = venv_interpreter
 
     def _set_site_pkg_path(self: Config) -> None:
-        """USe the interpreter to find the site packages path."""
+        """Use the interpreter to find the site packages path."""
         command = (
             f"{self.venv_interpreter} -c"
-            " 'import json,site; print(json.dumps(site.getsitepackages()))'"
+            "'import json,sysconfig; print(json.dumps(sysconfig.get_paths()))'"
         )
         work = "Locating site packages directory"
         try:
             proc = subprocess_run(
                 command=command,
                 verbose=self.args.verbose,
                 msg=work,
                 output=self._output,
             )
         except subprocess.CalledProcessError as exc:
             err = f"Failed to find site packages path: {exc}"
             self._output.critical(err)
 
         try:
-            site_pkg_dirs = json.loads(proc.stdout)
+            sysconfig_paths = json.loads(proc.stdout)
         except json.JSONDecodeError as exc:
             err = f"Failed to decode json: {exc}"
             self._output.critical(err)
 
-        if not site_pkg_dirs:
+        if not sysconfig_paths:
             err = "Failed to find site packages path."
             self._output.critical(err)
 
-        msg = f"Found site packages path: {site_pkg_dirs[0]}"
-        self._output.debug(msg)
+        purelib = sysconfig_paths.get("purelib")
+        if not purelib:
+            err = "Failed to find purelib in sysconfig paths."
+            self._output.critical(err)
 
-        self.site_pkg_path = Path(site_pkg_dirs[0])
+        self.site_pkg_path = Path(purelib)
+        msg = f"Found site packages path: {self.site_pkg_path}"
+        self._output.debug(msg)
```

### Comparing `ansible-dev-environment-24.1.1/src/ansible_dev_environment/output.py` & `ansible_dev_environment-24.4.0/src/ansible_dev_environment/output.py`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/src/ansible_dev_environment/subcommands/checker.py` & `ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/checker.py`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/src/ansible_dev_environment/subcommands/inspector.py` & `ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/inspector.py`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/src/ansible_dev_environment/subcommands/installer.py` & `ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/installer.py`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/src/ansible_dev_environment/subcommands/lister.py` & `ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/lister.py`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/src/ansible_dev_environment/subcommands/treemaker.py` & `ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/treemaker.py`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/src/ansible_dev_environment/subcommands/uninstaller.py` & `ansible_dev_environment-24.4.0/src/ansible_dev_environment/subcommands/uninstaller.py`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/src/ansible_dev_environment/tree.py` & `ansible_dev_environment-24.4.0/src/ansible_dev_environment/tree.py`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/src/ansible_dev_environment/utils.py` & `ansible_dev_environment-24.4.0/src/ansible_dev_environment/utils.py`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/src/ansible_dev_environment.egg-info/PKG-INFO` & `ansible_dev_environment-24.4.0/src/ansible_dev_environment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-dev-environment
-Version: 24.1.1
+Version: 24.4.0
 Summary: A pip-like ansible collection installer.
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Bradley Thornton <bthornto@redhat.com>
 License: GPL-3.0-only
 Project-URL: changelog, https://github.com/ansible/ansible-dev-environment/releases
 Project-URL: documentation, https://ansible.readthedocs.io/projects/dev-environment/
 Project-URL: homepage, https://github.com/ansible/ansible-dev-environment
```

### Comparing `ansible-dev-environment-24.1.1/src/ansible_dev_environment.egg-info/SOURCES.txt` & `ansible_dev_environment-24.4.0/src/ansible_dev_environment.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -51,9 +51,10 @@
 src/ansible_dev_environment/subcommands/uninstaller.py
 tests/__init__.py
 tests/fixtures/galaxy.yml
 tests/fixtures/requirements.yml
 tests/integration/__init__.py
 tests/integration/test_basic.py
 tests/unit/__init__.py
+tests/unit/test_config.py
 tests/unit/test_tree.py
 tests/unit/test_utils.py
```

### Comparing `ansible-dev-environment-24.1.1/tests/integration/test_basic.py` & `ansible_dev_environment-24.4.0/tests/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/tests/unit/test_tree.py` & `ansible_dev_environment-24.4.0/tests/unit/test_tree.py`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/tests/unit/test_utils.py` & `ansible_dev_environment-24.4.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-dev-environment-24.1.1/tox.ini` & `ansible_dev_environment-24.4.0/tox.ini`

 * *Files identical despite different names*


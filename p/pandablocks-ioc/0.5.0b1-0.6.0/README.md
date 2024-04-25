# Comparing `tmp/pandablocks-ioc-0.5.0b1.tar.gz` & `tmp/pandablocks_ioc-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandablocks-ioc-0.5.0b1.tar", last modified: Mon Mar  4 10:03:30 2024, max compression
+gzip compressed data, was "pandablocks_ioc-0.6.0.tar", last modified: Thu Apr 25 08:27:42 2024, max compression
```

## Comparing `pandablocks-ioc-0.5.0b1.tar` & `pandablocks_ioc-0.6.0.tar`

### file list

```diff
@@ -1,111 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.054273 pandablocks-ioc-0.5.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.038272 pandablocks-ioc-0.5.0b1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.devcontainer/.bashrc
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.devcontainer/initializeCommand
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.devcontainer/postCreateCommand
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.038272 pandablocks-ioc-0.5.0b1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.034273 pandablocks-ioc-0.5.0b1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.038272 pandablocks-ioc-0.5.0b1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.038272 pandablocks-ioc-0.5.0b1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     2759 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.042273 pandablocks-ioc-0.5.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.github/workflows/_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.github/workflows/_container.yml
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.github/workflows/_dist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.github/workflows/_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.github/workflows/_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.github/workflows/_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.github/workflows/_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.github/workflows/_tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.github/workflows/periodic.yml
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.042273 pandablocks-ioc-0.5.0b1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16559 2024-03-04 10:03:30.054273 pandablocks-ioc-0.5.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/catalog-info.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.042273 pandablocks-ioc-0.5.0b1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.042273 pandablocks-ioc-0.5.0b1/docs/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.042273 pandablocks-ioc-0.5.0b1/docs/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/explanations/decisions/0001-record-architecture-decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/explanations/decisions/0002-switched-to-python-copier-template.md
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/explanations/decisions/COPYME
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/explanations/decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/explanations.md
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/genindex.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.042273 pandablocks-ioc-0.5.0b1/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/how-to/capture-hdf.md
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/how-to/contribute.md
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/how-to/run-container.md
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/how-to.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.046273 pandablocks-ioc-0.5.0b1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    41547 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/images/data_bobfile.png
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    52271 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/images/phoebus_calc1.png
--rw-r--r--   0 runner    (1001) docker     (127)   215910 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/images/screen_index.png
--rw-r--r--   0 runner    (1001) docker     (127)    31121 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/images/webui_calc1.png
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.046273 pandablocks-ioc-0.5.0b1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/reference.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.046273 pandablocks-ioc-0.5.0b1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/tutorials/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 10:03:30.054273 pandablocks-ioc-0.5.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.034273 pandablocks-ioc-0.5.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.046273 pandablocks-ioc-0.5.0b1/src/pandablocks_ioc/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/src/pandablocks_ioc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/src/pandablocks_ioc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23725 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/src/pandablocks_ioc/_hdf_ioc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/src/pandablocks_ioc/_pvi.py
--rw-r--r--   0 runner    (1001) docker     (127)    16331 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/src/pandablocks_ioc/_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/src/pandablocks_ioc/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-04 10:03:29.000000 pandablocks-ioc-0.5.0b1/src/pandablocks_ioc/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    71699 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/src/pandablocks_ioc/ioc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.050273 pandablocks-ioc-0.5.0b1/src/pandablocks_ioc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16559 2024-03-04 10:03:30.000000 pandablocks-ioc-0.5.0b1/src/pandablocks_ioc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-03-04 10:03:30.000000 pandablocks-ioc-0.5.0b1/src/pandablocks_ioc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 10:03:30.000000 pandablocks-ioc-0.5.0b1/src/pandablocks_ioc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-04 10:03:30.000000 pandablocks-ioc-0.5.0b1/src/pandablocks_ioc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-04 10:03:30.000000 pandablocks-ioc-0.5.0b1/src/pandablocks_ioc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-04 10:03:30.000000 pandablocks-ioc-0.5.0b1/src/pandablocks_ioc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.050273 pandablocks-ioc-0.5.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.050273 pandablocks-ioc-0.5.0b1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29717 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/tests/fixtures/mocked_panda.py
--rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/tests/fixtures/panda_data.py
--rw-r--r--   0 runner    (1001) docker     (127)   440785 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/tests/raw_dump.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/tests/regenerate_test_bobfiles.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:03:30.050273 pandablocks-ioc-0.5.0b1/tests/test-bobfiles/
--rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/tests/test-bobfiles/DATA.bob
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/tests/test-bobfiles/PCAP.bob
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/tests/test-bobfiles/PULSE.bob
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/tests/test-bobfiles/PandA.bob
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/tests/test-bobfiles/SEQ.bob
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/tests/test-bobfiles/index.bob
--rwxr-xr-x   0 runner    (1001) docker     (127)     1325 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/tests/test-bobfiles/regenerate_test_bobfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    40938 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/tests/test_hdf_ioc.py
--rw-r--r--   0 runner    (1001) docker     (127)    24306 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/tests/test_ioc.py
--rw-r--r--   0 runner    (1001) docker     (127)    23489 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/tests/test_ioc_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/tests/test_pvaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)    16803 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/tests/test_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-04 10:03:25.000000 pandablocks-ioc-0.5.0b1/tests/test_unit_testing_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.618284 pandablocks_ioc-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.602284 pandablocks_ioc-0.6.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.devcontainer/.bashrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.devcontainer/initializeCommand
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.devcontainer/postCreateCommand
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.602284 pandablocks_ioc-0.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.598284 pandablocks_ioc-0.6.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.602284 pandablocks_ioc-0.6.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.606284 pandablocks_ioc-0.6.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2759 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.606284 pandablocks_ioc-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.github/workflows/_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.github/workflows/_container.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.github/workflows/_dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.github/workflows/_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.github/workflows/_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.github/workflows/_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.github/workflows/_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.github/workflows/_tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.github/workflows/periodic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.606284 pandablocks_ioc-0.6.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16557 2024-04-25 08:27:42.618284 pandablocks_ioc-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/catalog-info.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.606284 pandablocks_ioc-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.606284 pandablocks_ioc-0.6.0/docs/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.610283 pandablocks_ioc-0.6.0/docs/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/explanations/decisions/0001-record-architecture-decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/explanations/decisions/0002-switched-to-python-copier-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/explanations/decisions/COPYME
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/explanations/decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/explanations.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/genindex.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.610283 pandablocks_ioc-0.6.0/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/how-to/capture-hdf.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/how-to/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/how-to/run-container.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/how-to.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.610283 pandablocks_ioc-0.6.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    41547 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/images/data_bobfile.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    52271 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/images/phoebus_calc1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   215910 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/images/screen_index.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31121 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/images/webui_calc1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.610283 pandablocks_ioc-0.6.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/reference.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.610283 pandablocks_ioc-0.6.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/tutorials/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:27:42.618284 pandablocks_ioc-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.602284 pandablocks_ioc-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.610283 pandablocks_ioc-0.6.0/src/pandablocks_ioc/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/src/pandablocks_ioc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/src/pandablocks_ioc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/src/pandablocks_ioc/_connection_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23778 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/src/pandablocks_ioc/_hdf_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/src/pandablocks_ioc/_pvi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16331 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/src/pandablocks_ioc/_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/src/pandablocks_ioc/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 08:27:42.000000 pandablocks_ioc-0.6.0/src/pandablocks_ioc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72126 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/src/pandablocks_ioc/ioc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.618284 pandablocks_ioc-0.6.0/src/pandablocks_ioc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16557 2024-04-25 08:27:42.000000 pandablocks_ioc-0.6.0/src/pandablocks_ioc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-25 08:27:42.000000 pandablocks_ioc-0.6.0/src/pandablocks_ioc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:27:42.000000 pandablocks_ioc-0.6.0/src/pandablocks_ioc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-25 08:27:42.000000 pandablocks_ioc-0.6.0/src/pandablocks_ioc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-25 08:27:42.000000 pandablocks_ioc-0.6.0/src/pandablocks_ioc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-25 08:27:42.000000 pandablocks_ioc-0.6.0/src/pandablocks_ioc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.614283 pandablocks_ioc-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.614283 pandablocks_ioc-0.6.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29909 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/fixtures/mocked_panda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/fixtures/panda_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)   440785 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/raw_dump.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/regenerate_test_bobfiles.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:27:42.618284 pandablocks_ioc-0.6.0/tests/test-bobfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/test-bobfiles/DATA.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/test-bobfiles/PCAP.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/test-bobfiles/PULSE.bob
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/test-bobfiles/PandA.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/test-bobfiles/SEQ.bob
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/test-bobfiles/index.bob
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1325 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/test-bobfiles/regenerate_test_bobfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41151 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/test_hdf_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24882 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/test_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23489 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/test_ioc_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/test_pvaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16803 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-25 08:27:37.000000 pandablocks_ioc-0.6.0/tests/test_unit_testing_structure.py
```

### Comparing `pandablocks-ioc-0.5.0b1/.devcontainer/.bashrc` & `pandablocks_ioc-0.6.0/.devcontainer/.bashrc`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/.devcontainer/devcontainer.json` & `pandablocks_ioc-0.6.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/.dockerignore` & `pandablocks_ioc-0.6.0/.dockerignore`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/.github/CONTRIBUTING.md` & `pandablocks_ioc-0.6.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/.github/actions/install_requirements/action.yml` & `pandablocks_ioc-0.6.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/.github/dependabot.yml` & `pandablocks_ioc-0.6.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/.github/pages/make_switcher.py` & `pandablocks_ioc-0.6.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/.github/workflows/_check.yml` & `pandablocks_ioc-0.6.0/.github/workflows/_check.yml`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/.github/workflows/_container.yml` & `pandablocks_ioc-0.6.0/.github/workflows/_container.yml`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/.github/workflows/_dist.yml` & `pandablocks_ioc-0.6.0/.github/workflows/_dist.yml`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/.github/workflows/_docs.yml` & `pandablocks_ioc-0.6.0/.github/workflows/_docs.yml`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/.github/workflows/_release.yml` & `pandablocks_ioc-0.6.0/.github/workflows/_release.yml`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/.github/workflows/_test.yml` & `pandablocks_ioc-0.6.0/.github/workflows/_test.yml`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/.github/workflows/ci.yml` & `pandablocks_ioc-0.6.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/.gitignore` & `pandablocks_ioc-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/.pre-commit-config.yaml` & `pandablocks_ioc-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/.vscode/launch.json` & `pandablocks_ioc-0.6.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/Dockerfile` & `pandablocks_ioc-0.6.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/LICENSE` & `pandablocks_ioc-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/PKG-INFO` & `pandablocks_ioc-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandablocks-ioc
-Version: 0.5.0b1
+Version: 0.6.0
 Summary: Create an IOC from a PandA
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>, Alex Wells <alex.wells@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -214,15 +214,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools>=64
 Requires-Dist: numpy
 Requires-Dist: click
 Requires-Dist: h5py
 Requires-Dist: softioc>=4.4.0
-Requires-Dist: pandablocks~=0.7.0
+Requires-Dist: pandablocks~=0.8.0
 Requires-Dist: pvi~=0.7.0
 Requires-Dist: typing-extensions; python_version < "3.8"
 Provides-Extra: dev
 Requires-Dist: aioca; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mock; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
```

### Comparing `pandablocks-ioc-0.5.0b1/README.md` & `pandablocks_ioc-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/docs/conf.py` & `pandablocks_ioc-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/docs/explanations/decisions/0002-switched-to-python-copier-template.md` & `pandablocks_ioc-0.6.0/docs/explanations/decisions/0002-switched-to-python-copier-template.md`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/docs/how-to/capture-hdf.md` & `pandablocks_ioc-0.6.0/docs/how-to/capture-hdf.md`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/docs/images/data_bobfile.png` & `pandablocks_ioc-0.6.0/docs/images/data_bobfile.png`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/docs/images/dls-logo.svg` & `pandablocks_ioc-0.6.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/docs/images/phoebus_calc1.png` & `pandablocks_ioc-0.6.0/docs/images/phoebus_calc1.png`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/docs/images/screen_index.png` & `pandablocks_ioc-0.6.0/docs/images/screen_index.png`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/docs/images/webui_calc1.png` & `pandablocks_ioc-0.6.0/docs/images/webui_calc1.png`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/docs/index.md` & `pandablocks_ioc-0.6.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/docs/tutorials/installation.md` & `pandablocks_ioc-0.6.0/docs/tutorials/installation.md`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/pyproject.toml` & `pandablocks_ioc-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 description = "Create an IOC from a PandA"
 dependencies = [
     "setuptools>=64",
     "numpy",
     "click",
     "h5py",
     "softioc>=4.4.0",
-    "pandablocks~=0.7.0",
+    "pandablocks~=0.8.0",
     "pvi~=0.7.0",
     "typing-extensions;python_version<'3.8'",
 ] # Add project dependencies here, e.g. ["click", "numpy"]
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `pandablocks-ioc-0.5.0b1/src/pandablocks_ioc/__main__.py` & `pandablocks_ioc-0.6.0/src/pandablocks_ioc/__main__.py`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/src/pandablocks_ioc/_hdf_ioc.py` & `pandablocks_ioc-0.6.0/src/pandablocks_ioc/_hdf_ioc.py`

 * *Files 7% similar despite different names*

```diff
@@ -330,67 +330,69 @@
         self._client = client
 
         path_length = os.pathconf("/", "PC_PATH_MAX")
         filename_length = os.pathconf("/", "PC_NAME_MAX")
 
         # Create the records, including an uppercase alias for each
         # Naming convention and settings (mostly) copied from FSCN2 HDF5 records
-        directory_record_name = EpicsName(self._DATA_PREFIX + ":HDFDirectory")
+        directory_record_name = EpicsName(self._DATA_PREFIX + ":HDF_DIRECTORY")
         self._directory_record = builder.longStringOut(
             directory_record_name,
             length=path_length,
             DESC="File path for HDF5 files",
             validate=self._parameter_validate,
             on_update=self._update_full_file_path,
         )
         add_automatic_pvi_info(
             PviGroup.HDF,
             self._directory_record,
             directory_record_name,
             builder.longStringOut,
         )
         self._directory_record.add_alias(
-            record_prefix + ":" + directory_record_name.upper()
+            record_prefix + ":" + self._DATA_PREFIX + ":HDFDirectory"
         )
 
-        file_name_record_name = EpicsName(self._DATA_PREFIX + ":HDFFileName")
+        file_name_record_name = EpicsName(self._DATA_PREFIX + ":HDF_FILE_NAME")
         self._file_name_record = builder.longStringOut(
             file_name_record_name,
             length=filename_length,
             DESC="File name prefix for HDF5 files",
             validate=self._parameter_validate,
             on_update=self._update_full_file_path,
         )
         add_automatic_pvi_info(
             PviGroup.HDF,
             self._file_name_record,
             file_name_record_name,
             builder.longStringOut,
         )
         self._file_name_record.add_alias(
-            record_prefix + ":" + file_name_record_name.upper()
+            record_prefix + ":" + self._DATA_PREFIX + ":HDFFileName"
         )
 
-        full_file_path_record_name = EpicsName(self._DATA_PREFIX + ":HDFFullFilePath")
+        full_file_path_record_name = EpicsName(
+            self._DATA_PREFIX + ":HDF_FULL_FILE_PATH"
+        )
         self._full_file_path_record = builder.longStringIn(
             full_file_path_record_name,
             length=path_length + 1 + filename_length,
             DESC="Full HDF5 file name with directory",
         )
         add_automatic_pvi_info(
             PviGroup.HDF,
             self._full_file_path_record,
             full_file_path_record_name,
             builder.longStringIn,
         )
-        self._file_name_record.add_alias(
-            record_prefix + ":" + full_file_path_record_name.upper()
+        self._full_file_path_record.add_alias(
+            record_prefix + ":" + self._DATA_PREFIX + ":HDFFullFilePath"
         )
 
-        num_capture_record_name = EpicsName(self._DATA_PREFIX + ":NumCapture")
+        num_capture_record_name = EpicsName(self._DATA_PREFIX + ":NUM_CAPTURE")
         self._num_capture_record = builder.longOut(
             num_capture_record_name,
             initial_value=0,  # Infinite capture
             DESC="Number of frames to capture. 0=infinite",
             DRVL=0,
         )
 
@@ -398,118 +400,118 @@
             PviGroup.CAPTURE,
             self._num_capture_record,
             num_capture_record_name,
             builder.longOut,
         )
         # No validate - users are allowed to change this at any time
         self._num_capture_record.add_alias(
-            record_prefix + ":" + num_capture_record_name.upper()
+            record_prefix + ":" + self._DATA_PREFIX + ":NumCapture"
         )
 
-        num_captured_record_name = EpicsName(self._DATA_PREFIX + ":NumCaptured")
+        num_captured_record_name = EpicsName(self._DATA_PREFIX + ":NUM_CAPTURED")
         self._num_captured_record = builder.longIn(
             num_captured_record_name,
             initial_value=0,
             DESC="Number of frames written to file.",
         )
 
         add_automatic_pvi_info(
             PviGroup.CAPTURE,
             self._num_captured_record,
             num_captured_record_name,
             builder.longIn,
         )
         self._num_captured_record.add_alias(
-            record_prefix + ":" + num_captured_record_name.upper()
+            record_prefix + ":" + self._DATA_PREFIX + ":NumCaptured"
         )
 
-        num_received_record_name = EpicsName(self._DATA_PREFIX + ":NumReceived")
+        num_received_record_name = EpicsName(self._DATA_PREFIX + ":NUM_RECEIVED")
         self._num_received_record = builder.longIn(
             num_received_record_name,
             initial_value=0,
             DESC="Number of frames received from panda.",
         )
 
         add_automatic_pvi_info(
             PviGroup.CAPTURE,
             self._num_received_record,
             num_received_record_name,
             builder.longIn,
         )
         self._num_received_record.add_alias(
-            record_prefix + ":" + num_received_record_name.upper()
+            record_prefix + ":" + self._DATA_PREFIX + ":NumReceived"
         )
 
-        flush_period_record_name = EpicsName(self._DATA_PREFIX + ":FlushPeriod")
+        flush_period_record_name = EpicsName(self._DATA_PREFIX + ":FLUSH_PERIOD")
         self._flush_period_record = builder.aOut(
             flush_period_record_name,
             initial_value=1.0,
             DESC="Frequency that data is flushed (seconds)",
             EGU="s",
         )
         add_automatic_pvi_info(
             PviGroup.CAPTURE,
             self._flush_period_record,
             flush_period_record_name,
             builder.aOut,
         )
         self._flush_period_record.add_alias(
-            record_prefix + ":" + flush_period_record_name.upper()
+            record_prefix + ":" + self._DATA_PREFIX + ":FlushPeriod"
         )
 
-        capture_control_record_name = EpicsName(self._DATA_PREFIX + ":Capture")
+        capture_control_record_name = EpicsName(self._DATA_PREFIX + ":CAPTURE")
         self._capture_control_record = builder.boolOut(
             capture_control_record_name,
             ZNAM=ZNAM_STR,
             ONAM=ONAM_STR,
             on_update=self._capture_on_update,
             validate=self._capture_validate,
             DESC="Start/stop HDF5 capture",
         )
         add_data_capture_pvi_info(
             PviGroup.CAPTURE,
             capture_control_record_name,
             self._capture_control_record,
         )
         self._capture_control_record.add_alias(
-            record_prefix + ":" + capture_control_record_name.upper()
+            record_prefix + ":" + self._DATA_PREFIX + ":Capture"
         )
 
-        capture_mode_record_name = EpicsName(self._DATA_PREFIX + ":CaptureMode")
+        capture_mode_record_name = EpicsName(self._DATA_PREFIX + ":CAPTURE_MODE")
         self._capture_mode_record = builder.mbbOut(
             capture_mode_record_name,
             *[capture_mode.name for capture_mode in CaptureMode],
             initial_value=0,
             DESC="Choose how to hdf writer flushes",
         )
         add_automatic_pvi_info(
             PviGroup.CAPTURE,
             self._capture_mode_record,
             capture_mode_record_name,
             builder.mbbOut,
         )
         self._capture_mode_record.add_alias(
-            record_prefix + ":" + capture_mode_record_name.upper()
+            record_prefix + ":" + self._DATA_PREFIX + ":CaptureMode"
         )
 
-        status_message_record_name = EpicsName(self._DATA_PREFIX + ":Status")
+        status_message_record_name = EpicsName(self._DATA_PREFIX + ":STATUS")
         self._status_message_record = builder.longStringIn(
             status_message_record_name,
             initial_value="OK",
             length=200,
             DESC="Reports current status of HDF5 capture",
         )
         add_automatic_pvi_info(
             PviGroup.OUTPUTS,
             self._status_message_record,
             status_message_record_name,
             builder.stringIn,
         )
         self._status_message_record.add_alias(
-            record_prefix + ":" + status_message_record_name.upper()
+            record_prefix + ":" + self._DATA_PREFIX + ":Status"
         )
 
     def _parameter_validate(self, record: RecordWrapper, new_val) -> bool:
         """Control when values can be written to parameter records
         (file name etc.) based on capturing record's value"""
         logging.debug(f"Validating record {record.name} value {new_val}")
         if self._capture_control_record.get():
```

### Comparing `pandablocks-ioc-0.5.0b1/src/pandablocks_ioc/_pvi.py` & `pandablocks_ioc-0.6.0/src/pandablocks_ioc/_pvi.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             builder.longStringIn,
             builder.stringIn,
         ):
             widget = TextRead(format=TextFormat.string)
         else:
             widget = TextRead(format=None)
 
-        component = SignalR(name=pvi_name, pv=record_name, widget=TextRead())
+        component = SignalR(name=pvi_name, pv=record_name, widget=widget)
         access = "r"
 
     add_pvi_info_to_record(record, record_name, access)
     Pvi.add_pvi_info(record_name=record_name, group=group, component=component)
 
 
 _positions_table_group = Group(
```

### Comparing `pandablocks-ioc-0.5.0b1/src/pandablocks_ioc/_tables.py` & `pandablocks_ioc-0.6.0/src/pandablocks_ioc/_tables.py`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/src/pandablocks_ioc/_types.py` & `pandablocks_ioc-0.6.0/src/pandablocks_ioc/_types.py`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/src/pandablocks_ioc/ioc.py` & `pandablocks_ioc-0.6.0/src/pandablocks_ioc/ioc.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     TimeFieldInfo,
     UintFieldInfo,
 )
 from softioc import alarm, asyncio_dispatcher, builder, fields, softioc
 from softioc.imports import db_put_field
 from softioc.pythonSoftIoc import RecordWrapper
 
+from ._connection_status import ConnectionStatus, Statuses
 from ._hdf_ioc import HDF5RecordController
 from ._pvi import (
     Pvi,
     PviGroup,
     add_automatic_pvi_info,
     add_pcap_arm_pvi_info,
     add_positions_table_row,
@@ -90,14 +91,15 @@
     global create_softioc_task
     create_softioc_task = None
 
 
 async def _create_softioc(
     client: AsyncioClient,
     record_prefix: str,
+    connection_status: ConnectionStatus,
     dispatcher: asyncio_dispatcher.AsyncioDispatcher,
 ):
     """Asynchronous wrapper for IOC creation"""
     try:
         await client.connect()
     except OSError:
         logging.exception("Unable to connect to PandA")
@@ -107,15 +109,22 @@
     )
 
     global create_softioc_task
     if create_softioc_task:
         raise RuntimeError("Unexpected state - softioc task already exists")
 
     create_softioc_task = asyncio.create_task(
-        update(client, all_records, 0.1, all_values_dict, block_info_dict)
+        update(
+            client,
+            connection_status,
+            all_records,
+            0.1,
+            all_values_dict,
+            block_info_dict,
+        )
     )
 
     create_softioc_task.add_done_callback(_when_finished)
 
 
 def create_softioc(
     client: AsyncioClient,
@@ -142,23 +151,29 @@
         raise ValueError("recieved clear_bobfiles=True with no screens_dir")
 
     if screens_dir:
         Pvi.configure_pvi(screens_dir, clear_bobfiles)
 
     try:
         dispatcher = asyncio_dispatcher.AsyncioDispatcher()
+        connection_status = ConnectionStatus(record_prefix)
+        connection_status.set_status(Statuses.CONNECTING)
         asyncio.run_coroutine_threadsafe(
-            _create_softioc(client, record_prefix, dispatcher), dispatcher.loop
+            _create_softioc(client, record_prefix, connection_status, dispatcher),
+            dispatcher.loop,
         ).result()
+        connection_status.set_status(Statuses.CONNECTED)
 
         # Must leave this blocking line here, in the main thread, not in the
         # dispatcher's loop or it'll block every async process in this module
         softioc.interactive_ioc(globals())
-    except Exception:
+    except OSError as exc:
         logging.exception("Exception while initializing softioc")
+        connection_status.set_status(Statuses.DISCONNECTED)
+        raise exc
     finally:
         # Client was connected in the _create_softioc method
         if client.is_connected():
             asyncio.run_coroutine_threadsafe(client.close(), dispatcher.loop).result()
 
 
 async def introspect_panda(
@@ -1847,14 +1862,15 @@
 
     block_info_dict = {key: value.block_info for key, value in panda_dict.items()}
     return (all_records, all_values_dict, block_info_dict)
 
 
 async def update(
     client: AsyncioClient,
+    connection_status: ConnectionStatus,
     all_records: Dict[EpicsName, RecordInfo],
     poll_period: float,
     all_values_dict: Dict[EpicsName, RecordValue],
     block_info_dict: Dict[str, BlockInfo],
 ):
     """Query the PandA at regular intervals for any changed fields, and update
     the records accordingly
@@ -1883,23 +1899,22 @@
 
             try:
                 changes = await client.send(GetChanges(ChangeGroup.ALL, True), timeout)
             except asyncio.TimeoutError:
                 # Indicates PandA did not reply within the timeout
                 logging.error(
                     f"PandA did not respond to GetChanges within {timeout} seconds. "
-                    "Setting all records to major alarm state."
+                    "Setting all records to major alarm state and disconnecting."
                 )
+                connection_status.set_status(Statuses.DISCONNECTED)
                 set_all_records_severity(
                     all_records, alarm.MAJOR_ALARM, alarm.READ_ACCESS_ALARM
                 )
-                continue
-
-            # Clear any alarm state as we've received a new update from PandA
-            set_all_records_severity(all_records, alarm.NO_ALARM, alarm.UDF_ALARM)
+                await client.close()
+                break
 
             _, new_all_values_dict = _create_dicts_from_changes(
                 changes, block_info_dict
             )
 
             # Apply the new values to the existing dict, so various updater classes
             # will have access to the latest values.
@@ -2012,10 +2027,9 @@
 
 def set_all_records_severity(
     all_records: Dict[EpicsName, RecordInfo], severity: int, alarm: int
 ):
     """Set the severity of all possible records to the given state"""
     logging.debug(f"Setting all record to severity {severity} alarm {alarm}")
     for record_info in all_records.values():
-        # TODO: Update this if PythonSoftIOC issue #53 is fixed
         if record_info.is_in_record:
             record_info.record.set_alarm(severity, alarm)
```

### Comparing `pandablocks-ioc-0.5.0b1/src/pandablocks_ioc.egg-info/PKG-INFO` & `pandablocks_ioc-0.6.0/src/pandablocks_ioc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandablocks-ioc
-Version: 0.5.0b1
+Version: 0.6.0
 Summary: Create an IOC from a PandA
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>, Alex Wells <alex.wells@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -214,15 +214,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools>=64
 Requires-Dist: numpy
 Requires-Dist: click
 Requires-Dist: h5py
 Requires-Dist: softioc>=4.4.0
-Requires-Dist: pandablocks~=0.7.0
+Requires-Dist: pandablocks~=0.8.0
 Requires-Dist: pvi~=0.7.0
 Requires-Dist: typing-extensions; python_version < "3.8"
 Provides-Extra: dev
 Requires-Dist: aioca; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mock; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
```

### Comparing `pandablocks-ioc-0.5.0b1/src/pandablocks_ioc.egg-info/SOURCES.txt` & `pandablocks_ioc-0.6.0/src/pandablocks_ioc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 docs/images/phoebus_calc1.png
 docs/images/screen_index.png
 docs/images/webui_calc1.png
 docs/reference/api.md
 docs/tutorials/installation.md
 src/pandablocks_ioc/__init__.py
 src/pandablocks_ioc/__main__.py
+src/pandablocks_ioc/_connection_status.py
 src/pandablocks_ioc/_hdf_ioc.py
 src/pandablocks_ioc/_pvi.py
 src/pandablocks_ioc/_tables.py
 src/pandablocks_ioc/_types.py
 src/pandablocks_ioc/_version.py
 src/pandablocks_ioc/ioc.py
 src/pandablocks_ioc.egg-info/PKG-INFO
@@ -65,14 +66,15 @@
 src/pandablocks_ioc.egg-info/dependency_links.txt
 src/pandablocks_ioc.egg-info/entry_points.txt
 src/pandablocks_ioc.egg-info/requires.txt
 src/pandablocks_ioc.egg-info/top_level.txt
 tests/conftest.py
 tests/raw_dump.txt
 tests/regenerate_test_bobfiles.sh
+tests/test_connection.py
 tests/test_hdf_ioc.py
 tests/test_ioc.py
 tests/test_ioc_system.py
 tests/test_pvaccess.py
 tests/test_tables.py
 tests/test_types.py
 tests/test_unit_testing_structure.py
```

### Comparing `pandablocks-ioc-0.5.0b1/tests/fixtures/mocked_panda.py` & `pandablocks_ioc-0.6.0/tests/fixtures/mocked_panda.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,21 @@
 
         if key not in self.responses:
             raise RuntimeError(
                 f"Error in mocked panda, command {command} was passed in, "
                 f"the mocked responses defined for are: {[self.responses.keys()]}"
             )
 
+        try:
+            response = next(self.responses[key])
+        except StopIteration as err:  # Only happens if the client has disconnected
+            raise asyncio.TimeoutError from err
+
+        return response
+
         return next(self.responses[key])
 
 
 class Rows:
     def __init__(self, *rows):
         self.rows = rows
 
@@ -205,16 +212,15 @@
             and isinstance(command, GetChanges)
         ):
             self.introspect_panda_ran_already = True
 
             # Now the panda has set up, tell the test to start
             self.child_conn.send("R")
 
-        response = self.response_handler(command)
-        return response
+        return self.response_handler(command)
 
     def is_connected(self):
         return False
 
     async def close(self):
         pass
```

### Comparing `pandablocks-ioc-0.5.0b1/tests/fixtures/panda_data.py` & `pandablocks_ioc-0.6.0/tests/fixtures/panda_data.py`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/tests/raw_dump.txt` & `pandablocks_ioc-0.6.0/tests/raw_dump.txt`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/tests/test-bobfiles/DATA.bob` & `pandablocks_ioc-0.6.0/tests/test-bobfiles/DATA.bob`

 * *Files 4% similar despite different names*

```diff
@@ -30,147 +30,148 @@
     <x>5</x>
     <y>30</y>
     <width>496</width>
     <height>106</height>
     <transparent>true</transparent>
     <widget type="label" version="2.0.0">
       <name>Label</name>
-      <text>Hdfdirectory</text>
+      <text>Hdf Directory</text>
       <x>0</x>
       <y>0</y>
       <width>250</width>
       <height>20</height>
     </widget>
     <widget type="textentry" version="3.0.0">
       <name>TextEntry</name>
-      <pv_name>TEST_PREFIX:DATA:HDFDirectory</pv_name>
+      <pv_name>TEST_PREFIX:DATA:HDF_DIRECTORY</pv_name>
       <x>255</x>
       <y>0</y>
       <width>205</width>
       <height>20</height>
       <horizontal_alignment>1</horizontal_alignment>
       <format>6</format>
     </widget>
     <widget type="label" version="2.0.0">
       <name>Label</name>
-      <text>Hdffilename</text>
+      <text>Hdf File Name</text>
       <x>0</x>
       <y>25</y>
       <width>250</width>
       <height>20</height>
     </widget>
     <widget type="textentry" version="3.0.0">
       <name>TextEntry</name>
-      <pv_name>TEST_PREFIX:DATA:HDFFileName</pv_name>
+      <pv_name>TEST_PREFIX:DATA:HDF_FILE_NAME</pv_name>
       <x>255</x>
       <y>25</y>
       <width>205</width>
       <height>20</height>
       <horizontal_alignment>1</horizontal_alignment>
       <format>6</format>
     </widget>
     <widget type="label" version="2.0.0">
       <name>Label</name>
-      <text>Hdffullfilepath</text>
+      <text>Hdf Full File Path</text>
       <x>0</x>
       <y>50</y>
       <width>250</width>
       <height>20</height>
     </widget>
     <widget type="textupdate" version="2.0.0">
       <name>TextUpdate</name>
-      <pv_name>TEST_PREFIX:DATA:HDFFullFilePath</pv_name>
+      <pv_name>TEST_PREFIX:DATA:HDF_FULL_FILE_PATH</pv_name>
       <x>255</x>
       <y>50</y>
       <width>205</width>
       <height>20</height>
       <font>
         <font name="Default Bold" family="Liberation Sans" style="BOLD" size="14.0">
       </font>
       </font>
       <horizontal_alignment>1</horizontal_alignment>
+      <format>6</format>
     </widget>
   </widget>
   <widget type="group" version="2.0.0">
     <name>CAPTURE</name>
     <x>5</x>
     <y>141</y>
     <width>496</width>
     <height>206</height>
     <transparent>true</transparent>
     <widget type="label" version="2.0.0">
       <name>Label</name>
-      <text>Numcapture</text>
+      <text>Num Capture</text>
       <x>0</x>
       <y>0</y>
       <width>250</width>
       <height>20</height>
     </widget>
     <widget type="textentry" version="3.0.0">
       <name>TextEntry</name>
-      <pv_name>TEST_PREFIX:DATA:NumCapture</pv_name>
+      <pv_name>TEST_PREFIX:DATA:NUM_CAPTURE</pv_name>
       <x>255</x>
       <y>0</y>
       <width>205</width>
       <height>20</height>
       <horizontal_alignment>1</horizontal_alignment>
     </widget>
     <widget type="label" version="2.0.0">
       <name>Label</name>
-      <text>Numcaptured</text>
+      <text>Num Captured</text>
       <x>0</x>
       <y>25</y>
       <width>250</width>
       <height>20</height>
     </widget>
     <widget type="textupdate" version="2.0.0">
       <name>TextUpdate</name>
-      <pv_name>TEST_PREFIX:DATA:NumCaptured</pv_name>
+      <pv_name>TEST_PREFIX:DATA:NUM_CAPTURED</pv_name>
       <x>255</x>
       <y>25</y>
       <width>205</width>
       <height>20</height>
       <font>
         <font name="Default Bold" family="Liberation Sans" style="BOLD" size="14.0">
       </font>
       </font>
       <horizontal_alignment>1</horizontal_alignment>
     </widget>
     <widget type="label" version="2.0.0">
       <name>Label</name>
-      <text>Numreceived</text>
+      <text>Num Received</text>
       <x>0</x>
       <y>50</y>
       <width>250</width>
       <height>20</height>
     </widget>
     <widget type="textupdate" version="2.0.0">
       <name>TextUpdate</name>
-      <pv_name>TEST_PREFIX:DATA:NumReceived</pv_name>
+      <pv_name>TEST_PREFIX:DATA:NUM_RECEIVED</pv_name>
       <x>255</x>
       <y>50</y>
       <width>205</width>
       <height>20</height>
       <font>
         <font name="Default Bold" family="Liberation Sans" style="BOLD" size="14.0">
       </font>
       </font>
       <horizontal_alignment>1</horizontal_alignment>
     </widget>
     <widget type="label" version="2.0.0">
       <name>Label</name>
-      <text>Flushperiod</text>
+      <text>Flush Period</text>
       <x>0</x>
       <y>75</y>
       <width>250</width>
       <height>20</height>
     </widget>
     <widget type="textentry" version="3.0.0">
       <name>TextEntry</name>
-      <pv_name>TEST_PREFIX:DATA:FlushPeriod</pv_name>
+      <pv_name>TEST_PREFIX:DATA:FLUSH_PERIOD</pv_name>
       <x>255</x>
       <y>75</y>
       <width>205</width>
       <height>20</height>
       <horizontal_alignment>1</horizontal_alignment>
     </widget>
     <widget type="label" version="2.0.0">
@@ -179,15 +180,15 @@
       <x>0</x>
       <y>100</y>
       <width>250</width>
       <height>20</height>
     </widget>
     <widget type="action_button" version="3.0.0">
       <name>WritePV</name>
-      <pv_name>TEST_PREFIX:DATA:Capture</pv_name>
+      <pv_name>TEST_PREFIX:DATA:CAPTURE</pv_name>
       <actions>
         <action type="write_pv">
           <pv_name>$(pv_name)</pv_name>
           <value>1</value>
           <description>$(name)</description>
         </action>
       </actions>
@@ -196,15 +197,15 @@
       <y>100</y>
       <width>65</width>
       <height>20</height>
       <tooltip>$(actions)</tooltip>
     </widget>
     <widget type="action_button" version="3.0.0">
       <name>WritePV</name>
-      <pv_name>TEST_PREFIX:DATA:Capture</pv_name>
+      <pv_name>TEST_PREFIX:DATA:CAPTURE</pv_name>
       <actions>
         <action type="write_pv">
           <pv_name>$(pv_name)</pv_name>
           <value>0</value>
           <description>$(name)</description>
         </action>
       </actions>
@@ -213,31 +214,31 @@
       <y>100</y>
       <width>65</width>
       <height>20</height>
       <tooltip>$(actions)</tooltip>
     </widget>
     <widget type="led" version="2.0.0">
       <name>LED</name>
-      <pv_name>TEST_PREFIX:DATA:Capture</pv_name>
+      <pv_name>TEST_PREFIX:DATA:CAPTURE</pv_name>
       <x>417</x>
       <y>100</y>
       <width>20</width>
       <height>20</height>
     </widget>
     <widget type="label" version="2.0.0">
       <name>Label</name>
-      <text>Capturemode</text>
+      <text>Capture Mode</text>
       <x>0</x>
       <y>125</y>
       <width>250</width>
       <height>20</height>
     </widget>
     <widget type="combo" version="2.0.0">
       <name>ComboBox</name>
-      <pv_name>TEST_PREFIX:DATA:CaptureMode</pv_name>
+      <pv_name>TEST_PREFIX:DATA:CAPTURE_MODE</pv_name>
       <x>255</x>
       <y>125</y>
       <width>205</width>
       <height>20</height>
     </widget>
     <widget type="label" version="2.0.0">
       <name>Label</name>
@@ -277,20 +278,21 @@
       <x>0</x>
       <y>0</y>
       <width>250</width>
       <height>20</height>
     </widget>
     <widget type="textupdate" version="2.0.0">
       <name>TextUpdate</name>
-      <pv_name>TEST_PREFIX:DATA:Status</pv_name>
+      <pv_name>TEST_PREFIX:DATA:STATUS</pv_name>
       <x>255</x>
       <y>0</y>
       <width>205</width>
       <height>20</height>
       <font>
         <font name="Default Bold" family="Liberation Sans" style="BOLD" size="14.0">
       </font>
       </font>
       <horizontal_alignment>1</horizontal_alignment>
+      <format>6</format>
     </widget>
   </widget>
 </display>
```

### Comparing `pandablocks-ioc-0.5.0b1/tests/test-bobfiles/PCAP.bob` & `pandablocks_ioc-0.6.0/tests/test-bobfiles/PCAP.bob`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/tests/test-bobfiles/PULSE.bob` & `pandablocks_ioc-0.6.0/tests/test-bobfiles/PULSE.bob`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/tests/test-bobfiles/PandA.bob` & `pandablocks_ioc-0.6.0/tests/test-bobfiles/PandA.bob`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/tests/test-bobfiles/SEQ.bob` & `pandablocks_ioc-0.6.0/tests/test-bobfiles/SEQ.bob`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/tests/test-bobfiles/index.bob` & `pandablocks_ioc-0.6.0/tests/test-bobfiles/index.bob`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/tests/test-bobfiles/regenerate_test_bobfiles.py` & `pandablocks_ioc-0.6.0/tests/test-bobfiles/regenerate_test_bobfiles.py`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/tests/test_hdf_ioc.py` & `pandablocks_ioc-0.6.0/tests/test_hdf_ioc.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,29 +112,29 @@
 ]
 
 
 @pytest_asyncio.fixture
 def slow_dump_expected():
     yield [
         ReadyData(),
-        StartData(DUMP_FIELDS, 0, "Scaled", "Framed", 52),
+        StartData(DUMP_FIELDS, 0, "Scaled", "Framed", 52, None, None, None),
         FrameData(Rows([0, 1, 1, 3, 5.6e-08, 1, 2])),
         FrameData(Rows([8, 2, 2, 6, 1.000000056, 2, 4])),
         FrameData(Rows([0, 3, 3, 9, 2.000000056, 3, 6])),
         FrameData(Rows([8, 4, 4, 12, 3.000000056, 4, 8])),
         FrameData(Rows([0, 5, 5, 15, 4.000000056, 5, 10])),
         EndData(5, EndReason.DISARMED),
     ]
 
 
 @pytest_asyncio.fixture
 def fast_dump_expected():
     yield [
         ReadyData(),
-        StartData(DUMP_FIELDS, 0, "Scaled", "Framed", 52),
+        StartData(DUMP_FIELDS, 0, "Scaled", "Framed", 52, None, None, None),
         FrameData(
             Rows(
                 [0, 1, 1, 3, 5.6e-08, 1, 2],
                 [0, 2, 2, 6, 0.010000056, 2, 4],
                 [8, 3, 3, 9, 0.020000056, 3, 6],
                 [8, 4, 4, 12, 0.030000056, 4, 8],
                 [8, 5, 5, 15, 0.040000056, 5, 10],
@@ -326,15 +326,15 @@
 
     val = await caget(hdf5_test_prefix + ":HDFDirectory", datatype=DBR_CHAR_STR)
 
     # Default value of longStringOut is an array of a single NULL byte
     assert val == ""
 
     # Mix and match between CamelCase and UPPERCASE to check aliases work
-    val = await caget(hdf5_test_prefix + ":HDFFILENAME", datatype=DBR_CHAR_STR)
+    val = await caget(hdf5_test_prefix + ":HDF_FILE_NAME", datatype=DBR_CHAR_STR)
     assert val == ""
 
     val = await caget(hdf5_test_prefix + ":NumCapture")
     assert val == 0
 
     val = await caget(hdf5_test_prefix + ":FlushPeriod")
     assert val == 1.0
@@ -540,15 +540,15 @@
     assert not (tmp_path / test_filename).exists()
 
 
 @pytest_asyncio.fixture
 def differently_sized_framedata():
     yield [
         ReadyData(),
-        StartData(DUMP_FIELDS, 0, "Scaled", "Framed", 52),
+        StartData(DUMP_FIELDS, 0, "Scaled", "Framed", 52, None, None, None),
         FrameData(
             numpy.array(
                 [
                     [0, 1, 1, 3, 5.6e-08, 1, 2],
                     [0, 2, 2, 6, 0.010000056, 2, 4],
                     [8, 3, 3, 9, 0.020000056, 3, 6],
                     [8, 4, 4, 12, 0.030000056, 4, 8],
@@ -778,15 +778,15 @@
         num_received_output.append,
         num_captured_setter_pipeline,
     )
     buffer.put_data_to_file = frames_written_to_file.append
 
     large_data = [
         ReadyData(),
-        StartData([], 0, "Scaled", "Framed", 52),
+        StartData([], 0, "Scaled", "Framed", 52, None, None, None),
         FrameData(numpy.zeros(25000)),
         FrameData(numpy.zeros(25000)),
         FrameData(numpy.zeros(25000)),
         FrameData(numpy.zeros(25000)),
         FrameData(numpy.zeros(25000)),
         FrameData(numpy.append(numpy.zeros(15000), numpy.arange(1, 10001))),
         EndData(150000, EndReason.OK),
@@ -795,15 +795,15 @@
     for data in large_data:
         buffer.handle_data(data)
 
     assert buffer.number_of_received_rows == 150000
     assert buffer.number_of_rows_in_circular_buffer == 25000
 
     expected_output = [
-        StartData([], 0, "Scaled", "Framed", 52),
+        StartData([], 0, "Scaled", "Framed", 52, None, None, None),
         FrameData(numpy.append(numpy.zeros(15000), numpy.arange(1, 10001))),
         EndData(150000, EndReason.OK),
     ]
 
     output_frames = [
         frame_data
         for frame_data in frames_written_to_file
@@ -937,25 +937,22 @@
                         units="",
                     )
                 ],
                 0,
                 "Scaled",
                 "Framed",
                 52,
+                None,
+                None,
+                None,
             ),
             FrameData(Rows([0, 1, 1, 3, 5.6e-08, 1, 2])),
             # Implicit end of first data here
             ReadyData(),
-            StartData(
-                [],
-                0,
-                "Different",
-                "Also Different",
-                52,
-            ),
+            StartData([], 0, "Different", "Also Different", 52, None, None, None),
         ]
         for item in list:
             yield item
 
     # Set up all the mocks
     hdf5_controller._get_filepath = MagicMock(  # type: ignore
         return_value="Some/Filepath"
@@ -1006,14 +1003,17 @@
                         units="",
                     )
                 ],
                 0,
                 "Scaled",
                 "Framed",
                 52,
+                None,
+                None,
+                None,
             ),
         ]
         for item in list:
             yield item
         raise CancelledError
 
     # Set up all the mocks
@@ -1061,14 +1061,17 @@
                         units="",
                     )
                 ],
                 0,
                 "Scaled",
                 "Framed",
                 52,
+                None,
+                None,
+                None,
             ),
         ]
         for item in list:
             yield item
         raise Exception("Test exception")
 
     # Set up all the mocks
```

### Comparing `pandablocks-ioc-0.5.0b1/tests/test_ioc.py` & `pandablocks_ioc-0.6.0/tests/test_ioc.py`

 * *Files 5% similar despite different names*

```diff
@@ -784,17 +784,30 @@
     record_info.record = MagicMock()
 
     all_records = {EpicsName("ABC:DEF"): record_info}
     poll_period = 0.1
     all_values_dict = {}
     block_info = {}
 
+    class MockConnectionStatus:
+        statuses_set = []
+        set_status = statuses_set.append
+
+    mock_connection_status = MockConnectionStatus()
+
     try:
         await asyncio.wait_for(
-            update(client, all_records, poll_period, all_values_dict, block_info),
+            update(
+                client,
+                mock_connection_status,
+                all_records,
+                poll_period,
+                all_values_dict,
+                block_info,
+            ),
             timeout=0.3,
         )
     except asyncio.TimeoutError:
         pass
 
     record_info.record.set_alarm.assert_called_with(3, 17)
     assert "PandA reports field in error" in caplog.text
@@ -820,17 +833,30 @@
     record_info._field_info = FieldInfo("bit_out", None, None)
 
     all_records = {EpicsName("ABC:DEF"): record_info}
     poll_period = 0.1
     all_values_dict = {}
     block_info = {}
 
+    class MockConnectionStatus:
+        statuses_set = []
+        set_status = statuses_set.append
+
+    mock_connection_status = MockConnectionStatus()
+
     try:
         await asyncio.wait_for(
-            update(client, all_records, poll_period, all_values_dict, block_info),
+            update(
+                client,
+                mock_connection_status,
+                all_records,
+                poll_period,
+                all_values_dict,
+                block_info,
+            ),
             timeout=0.5,
         )
     except asyncio.TimeoutError:
         pass
 
     # Note that the update() method may run more than once, so we'll get an
     # unreliable number of calls to the set method.
```

### Comparing `pandablocks-ioc-0.5.0b1/tests/test_ioc_system.py` & `pandablocks_ioc-0.6.0/tests/test_ioc_system.py`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/tests/test_pvaccess.py` & `pandablocks_ioc-0.6.0/tests/test_pvaccess.py`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/tests/test_tables.py` & `pandablocks_ioc-0.6.0/tests/test_tables.py`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/tests/test_types.py` & `pandablocks_ioc-0.6.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pandablocks-ioc-0.5.0b1/tests/test_unit_testing_structure.py` & `pandablocks_ioc-0.6.0/tests/test_unit_testing_structure.py`

 * *Files identical despite different names*


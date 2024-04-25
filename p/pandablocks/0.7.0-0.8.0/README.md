# Comparing `tmp/pandablocks-0.7.0.tar.gz` & `tmp/pandablocks-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandablocks-0.7.0.tar", last modified: Mon Jan 29 09:10:19 2024, max compression
+gzip compressed data, was "pandablocks-0.8.0.tar", last modified: Thu Apr 25 08:08:21 2024, max compression
```

## Comparing `pandablocks-0.7.0.tar` & `pandablocks-0.8.0.tar`

### file list

```diff
@@ -1,129 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.495820 pandablocks-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.479820 pandablocks-0.7.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-01-29 09:10:11.000000 pandablocks-0.7.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.479820 pandablocks-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.475820 pandablocks-0.7.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.479820 pandablocks-0.7.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-01-29 09:10:11.000000 pandablocks-0.7.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-01-29 09:10:11.000000 pandablocks-0.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.479820 pandablocks-0.7.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-01-29 09:10:11.000000 pandablocks-0.7.0/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     3043 2024-01-29 09:10:11.000000 pandablocks-0.7.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.479820 pandablocks-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-01-29 09:10:11.000000 pandablocks-0.7.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-01-29 09:10:11.000000 pandablocks-0.7.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-01-29 09:10:11.000000 pandablocks-0.7.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-01-29 09:10:11.000000 pandablocks-0.7.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-01-29 09:10:11.000000 pandablocks-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-01-29 09:10:11.000000 pandablocks-0.7.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.483820 pandablocks-0.7.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-01-29 09:10:11.000000 pandablocks-0.7.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-01-29 09:10:11.000000 pandablocks-0.7.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-01-29 09:10:11.000000 pandablocks-0.7.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-01-29 09:10:11.000000 pandablocks-0.7.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-01-29 09:10:11.000000 pandablocks-0.7.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-29 09:10:11.000000 pandablocks-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-01-29 09:10:19.495820 pandablocks-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-01-29 09:10:11.000000 pandablocks-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.483820 pandablocks-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.483820 pandablocks-0.7.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.483820 pandablocks-0.7.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.483820 pandablocks-0.7.0/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.483820 pandablocks-0.7.0/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.483820 pandablocks-0.7.0/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/developer/explanations/decisions/0003-make-library-sans-io.rst
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/developer/explanations/decisions.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.483820 pandablocks-0.7.0/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.483820 pandablocks-0.7.0/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.487820 pandablocks-0.7.0/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.487820 pandablocks-0.7.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    16088 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/images/PandA-logo-for-black-background.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/images/PandA-logo.ico
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.487820 pandablocks-0.7.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.487820 pandablocks-0.7.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/user/explanations/docs-structure.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/user/explanations/performance.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/user/explanations/sans-io.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.487820 pandablocks-0.7.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/user/how-to/introspect-panda.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/user/how-to/library-hdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/user/how-to/poll-changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.487820 pandablocks-0.7.0/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/user/reference/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/user/reference/appendix.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/user/reference/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/user/reference/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.487820 pandablocks-0.7.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/user/tutorials/commandline-hdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/user/tutorials/control.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/user/tutorials/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/user/tutorials/load-save.rst
--rw-r--r--   0 runner    (1001) docker     (127)   139735 2024-01-29 09:10:11.000000 pandablocks-0.7.0/docs/user/tutorials/tutorial_layout.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.487820 pandablocks-0.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-29 09:10:11.000000 pandablocks-0.7.0/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-01-29 09:10:11.000000 pandablocks-0.7.0/examples/arm_and_hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-01-29 09:10:11.000000 pandablocks-0.7.0/examples/hdf_queue_reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-29 09:10:11.000000 pandablocks-0.7.0/examples/introspect_panda.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-01-29 09:10:11.000000 pandablocks-0.7.0/examples/plot_counter_hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-01-29 09:10:11.000000 pandablocks-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 09:10:19.495820 pandablocks-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.479820 pandablocks-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.491820 pandablocks-0.7.0/src/pandablocks/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-01-29 09:10:11.000000 pandablocks-0.7.0/src/pandablocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-01-29 09:10:11.000000 pandablocks-0.7.0/src/pandablocks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-01-29 09:10:11.000000 pandablocks-0.7.0/src/pandablocks/_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-01-29 09:10:11.000000 pandablocks-0.7.0/src/pandablocks/_exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-29 09:10:19.000000 pandablocks-0.7.0/src/pandablocks/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-01-29 09:10:11.000000 pandablocks-0.7.0/src/pandablocks/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-01-29 09:10:11.000000 pandablocks-0.7.0/src/pandablocks/blocking.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-01-29 09:10:11.000000 pandablocks-0.7.0/src/pandablocks/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    30732 2024-01-29 09:10:11.000000 pandablocks-0.7.0/src/pandablocks/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    16010 2024-01-29 09:10:11.000000 pandablocks-0.7.0/src/pandablocks/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-01-29 09:10:11.000000 pandablocks-0.7.0/src/pandablocks/hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-01-29 09:10:11.000000 pandablocks-0.7.0/src/pandablocks/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.491820 pandablocks-0.7.0/src/pandablocks/saves/
--rw-r--r--   0 runner    (1001) docker     (127)    15831 2024-01-29 09:10:11.000000 pandablocks-0.7.0/src/pandablocks/saves/tutorial.sav
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-01-29 09:10:11.000000 pandablocks-0.7.0/src/pandablocks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.495820 pandablocks-0.7.0/src/pandablocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-01-29 09:10:19.000000 pandablocks-0.7.0/src/pandablocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-01-29 09:10:19.000000 pandablocks-0.7.0/src/pandablocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 09:10:19.000000 pandablocks-0.7.0/src/pandablocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-29 09:10:19.000000 pandablocks-0.7.0/src/pandablocks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-01-29 09:10:19.000000 pandablocks-0.7.0/src/pandablocks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-29 09:10:19.000000 pandablocks-0.7.0/src/pandablocks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:19.495820 pandablocks-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 09:10:11.000000 pandablocks-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10809 2024-01-29 09:10:11.000000 pandablocks-0.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-01-29 09:10:11.000000 pandablocks-0.7.0/tests/fast_dump.txt
--rw-r--r--   0 runner    (1001) docker     (127)   440785 2024-01-29 09:10:11.000000 pandablocks-0.7.0/tests/raw_dump.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-01-29 09:10:11.000000 pandablocks-0.7.0/tests/slow_dump.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-01-29 09:10:11.000000 pandablocks-0.7.0/tests/test_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-01-29 09:10:11.000000 pandablocks-0.7.0/tests/test_blocking.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-01-29 09:10:11.000000 pandablocks-0.7.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-01-29 09:10:11.000000 pandablocks-0.7.0/tests/test_completer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-01-29 09:10:11.000000 pandablocks-0.7.0/tests/test_hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    38660 2024-01-29 09:10:11.000000 pandablocks-0.7.0/tests/test_pandablocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-01-29 09:10:11.000000 pandablocks-0.7.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.798611 pandablocks-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.782611 pandablocks-0.8.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.782611 pandablocks-0.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.778611 pandablocks-0.8.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.782611 pandablocks-0.8.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.782611 pandablocks-0.8.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2759 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.786611 pandablocks-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.github/workflows/_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.github/workflows/_container.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.github/workflows/_dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.github/workflows/_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.github/workflows/_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.github/workflows/_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.github/workflows/_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.github/workflows/_tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.github/workflows/periodic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.786611 pandablocks-0.8.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-25 08:08:18.000000 pandablocks-0.8.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-25 08:08:18.000000 pandablocks-0.8.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 08:08:18.000000 pandablocks-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-04-25 08:08:21.798611 pandablocks-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-25 08:08:18.000000 pandablocks-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-25 08:08:18.000000 pandablocks-0.8.0/catalog-info.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.786611 pandablocks-0.8.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.786611 pandablocks-0.8.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.786611 pandablocks-0.8.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.786611 pandablocks-0.8.0/docs/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.786611 pandablocks-0.8.0/docs/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/explanations/decisions/0001-record-architecture-decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/explanations/decisions/0002-switched-to-python-copier-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/explanations/decisions/0003-make-library-sans-io.md
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/explanations/decisions/COPYME
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/explanations/decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/explanations/performance.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/explanations/sans-io.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/explanations.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/genindex.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.790611 pandablocks-0.8.0/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/how-to/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/how-to/introspect-panda.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/how-to/library-hdf.md
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/how-to/poll-changes.md
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/how-to/run-container.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/how-to.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.790611 pandablocks-0.8.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    16088 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/images/PandA-logo-for-black-background.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/images/PandA-logo.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.790611 pandablocks-0.8.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/reference/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/reference.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.790611 pandablocks-0.8.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/tutorials/commandline-hdf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/tutorials/control.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/tutorials/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/tutorials/load-save.md
+-rw-r--r--   0 runner    (1001) docker     (127)   139735 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/tutorials/tutorial_layout.png
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-25 08:08:18.000000 pandablocks-0.8.0/docs/tutorials.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.790611 pandablocks-0.8.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-25 08:08:18.000000 pandablocks-0.8.0/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-25 08:08:18.000000 pandablocks-0.8.0/examples/arm_and_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-25 08:08:18.000000 pandablocks-0.8.0/examples/hdf_queue_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-25 08:08:18.000000 pandablocks-0.8.0/examples/introspect_panda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-25 08:08:18.000000 pandablocks-0.8.0/examples/load_abs_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-25 08:08:18.000000 pandablocks-0.8.0/examples/plot_counter_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-25 08:08:18.000000 pandablocks-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:08:21.798611 pandablocks-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.782611 pandablocks-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.794611 pandablocks-0.8.0/src/pandablocks/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-25 08:08:18.000000 pandablocks-0.8.0/src/pandablocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-25 08:08:18.000000 pandablocks-0.8.0/src/pandablocks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-04-25 08:08:18.000000 pandablocks-0.8.0/src/pandablocks/_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-25 08:08:18.000000 pandablocks-0.8.0/src/pandablocks/_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 08:08:21.000000 pandablocks-0.8.0/src/pandablocks/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-04-25 08:08:18.000000 pandablocks-0.8.0/src/pandablocks/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-25 08:08:18.000000 pandablocks-0.8.0/src/pandablocks/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-25 08:08:18.000000 pandablocks-0.8.0/src/pandablocks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30732 2024-04-25 08:08:18.000000 pandablocks-0.8.0/src/pandablocks/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16499 2024-04-25 08:08:18.000000 pandablocks-0.8.0/src/pandablocks/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9407 2024-04-25 08:08:18.000000 pandablocks-0.8.0/src/pandablocks/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-04-25 08:08:18.000000 pandablocks-0.8.0/src/pandablocks/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.794611 pandablocks-0.8.0/src/pandablocks/saves/
+-rw-r--r--   0 runner    (1001) docker     (127)    15831 2024-04-25 08:08:18.000000 pandablocks-0.8.0/src/pandablocks/saves/tutorial.sav
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-25 08:08:18.000000 pandablocks-0.8.0/src/pandablocks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.798611 pandablocks-0.8.0/src/pandablocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-04-25 08:08:21.000000 pandablocks-0.8.0/src/pandablocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-25 08:08:21.000000 pandablocks-0.8.0/src/pandablocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:08:21.000000 pandablocks-0.8.0/src/pandablocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 08:08:21.000000 pandablocks-0.8.0/src/pandablocks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-25 08:08:21.000000 pandablocks-0.8.0/src/pandablocks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 08:08:21.000000 pandablocks-0.8.0/src/pandablocks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.794611 pandablocks-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:18.000000 pandablocks-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12575 2024-04-25 08:08:18.000000 pandablocks-0.8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:08:21.798611 pandablocks-0.8.0/tests/data_dumps/
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-25 08:08:18.000000 pandablocks-0.8.0/tests/data_dumps/fast_dump.bin
+-rw-r--r--   0 runner    (1001) docker     (127)   440881 2024-04-25 08:08:18.000000 pandablocks-0.8.0/tests/data_dumps/raw_dump.bin
+-rw-r--r--   0 runner    (1001) docker     (127)   440785 2024-04-25 08:08:18.000000 pandablocks-0.8.0/tests/data_dumps/raw_dump_no_duration.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-25 08:08:18.000000 pandablocks-0.8.0/tests/data_dumps/slow_dump.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-04-25 08:08:18.000000 pandablocks-0.8.0/tests/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-25 08:08:18.000000 pandablocks-0.8.0/tests/test_blocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-25 08:08:18.000000 pandablocks-0.8.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-25 08:08:18.000000 pandablocks-0.8.0/tests/test_completer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-25 08:08:18.000000 pandablocks-0.8.0/tests/test_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38896 2024-04-25 08:08:18.000000 pandablocks-0.8.0/tests/test_pandablocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-04-25 08:08:18.000000 pandablocks-0.8.0/tests/test_utils.py
```

### Comparing `pandablocks-0.7.0/.devcontainer/devcontainer.json` & `pandablocks-0.8.0/.devcontainer/devcontainer.json`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,46 @@
 // For format details, see https://containers.dev/implementors/json_reference/
 {
     "name": "Python 3 Developer Container",
     "build": {
         "dockerfile": "../Dockerfile",
-        "target": "build",
-        // Only upgrade pip, we will install the project below
-        "args": {
-            "PIP_OPTIONS": "--upgrade pip"
-        }
+        "target": "developer"
     },
     "remoteEnv": {
+        // Allow X11 apps to run inside the container
         "DISPLAY": "${localEnv:DISPLAY}"
     },
-    // Add the URLs of features you want added when the container is built.
-    "features": {
-        "ghcr.io/devcontainers/features/common-utils:1": {
-            "username": "none",
-            "upgradePackages": false
-        }
-    },
-    // Set *default* container specific settings.json values on container create.
-    "settings": {
-        "python.defaultInterpreterPath": "/venv/bin/python"
-    },
     "customizations": {
         "vscode": {
+            // Set *default* container specific settings.json values on container create.
+            "settings": {
+                "python.defaultInterpreterPath": "/venv/bin/python"
+            },
             // Add the IDs of extensions you want installed when the container is created.
             "extensions": [
                 "ms-python.python",
+                "github.vscode-github-actions",
                 "tamasfe.even-better-toml",
                 "redhat.vscode-yaml",
-                "ryanluker.vscode-coverage-gutters"
+                "ryanluker.vscode-coverage-gutters",
+                "charliermarsh.ruff",
+                "ms-azuretools.vscode-docker"
             ]
         }
     },
-    // Make sure the files we are mapping into the container exist on the host
-    "initializeCommand": "bash -c 'for i in $HOME/.inputrc; do [ -f $i ] || touch $i; done'",
+    "features": {
+        // Some default things like git config
+        "ghcr.io/devcontainers/features/common-utils:2": {
+            "upgradePackages": false
+        }
+    },
     "runArgs": [
+        // Allow the container to access the host X11 display and EPICS CA
         "--net=host",
-        "--security-opt=label=type:container_runtime_t"
-    ],
-    "mounts": [
-        "source=${localEnv:HOME}/.ssh,target=/root/.ssh,type=bind",
-        "source=${localEnv:HOME}/.inputrc,target=/root/.inputrc,type=bind",
-        // map in home directory - not strictly necessary but useful
-        "source=${localEnv:HOME},target=${localEnv:HOME},type=bind,consistency=cached"
+        // Make sure SELinux does not disable with access to host filesystems like tmp
+        "--security-opt=label=disable"
     ],
-    // make the workspace folder the same inside and outside of the container
-    "workspaceMount": "source=${localWorkspaceFolder},target=${localWorkspaceFolder},type=bind",
-    "workspaceFolder": "${localWorkspaceFolder}",
+    // Mount the parent as /workspaces so we can pip install peers as editable
+    "workspaceMount": "source=${localWorkspaceFolder}/..,target=/workspaces,type=bind",
     // After the container is created, install the python project in editable form
-    "postCreateCommand": "pip install -e '.[dev]'"
-}
+    "postCreateCommand": "pip install $([ -f dev-requirements.txt ] && echo '-c dev-requirements.txt') -e '.[dev]' && pre-commit install"
+}
```

### Comparing `pandablocks-0.7.0/.github/pages/make_switcher.py` & `pandablocks-0.8.0/.github/pages/make_switcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,29 +20,26 @@
 
 def get_sorted_tags_list() -> List[str]:
     """Get a list of sorted tags in descending order from the repository."""
     stdout = check_output(["git", "tag", "-l", "--sort=-v:refname"])
     return report_output(stdout, "Tags list")
 
 
-def get_versions(ref: str, add: Optional[str], remove: Optional[str]) -> List[str]:
+def get_versions(ref: str, add: Optional[str]) -> List[str]:
     """Generate the file containing the list of all GitHub Pages builds."""
     # Get the directories (i.e. builds) from the GitHub Pages branch
     try:
         builds = set(get_branch_contents(ref))
     except CalledProcessError:
         builds = set()
         logging.warning(f"Cannot get {ref} contents")
 
     # Add and remove from the list of builds
     if add:
         builds.add(add)
-    if remove:
-        assert remove in builds, f"Build '{remove}' not in {sorted(builds)}"
-        builds.remove(remove)
 
     # Get a sorted list of tags
     tags = get_sorted_tags_list()
 
     # Make the sorted versions list from main branches and tags
     versions: List[str] = []
     for version in ["master", "main"] + tags:
@@ -65,35 +62,31 @@
     text = json.dumps(struct, indent=2)
     print(f"JSON switcher:\n{text}")
     path.write_text(text, encoding="utf-8")
 
 
 def main(args=None):
     parser = ArgumentParser(
-        description="Make a versions.txt file from gh-pages directories"
+        description="Make a versions.json file from gh-pages directories"
     )
     parser.add_argument(
         "--add",
         help="Add this directory to the list of existing directories",
     )
     parser.add_argument(
-        "--remove",
-        help="Remove this directory from the list of existing directories",
-    )
-    parser.add_argument(
         "repository",
         help="The GitHub org and repository name: ORG/REPO",
     )
     parser.add_argument(
         "output",
         type=Path,
         help="Path of write switcher.json to",
     )
     args = parser.parse_args(args)
 
     # Write the versions file
-    versions = get_versions("origin/gh-pages", args.add, args.remove)
+    versions = get_versions("origin/gh-pages", args.add)
     write_json(args.output, args.repository, versions)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pandablocks-0.7.0/.gitignore` & `pandablocks-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/LICENSE` & `pandablocks-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/README.rst` & `pandablocks-0.8.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,72 +1,51 @@
-PandABlocks Python Client
-=========================
-
-|code_ci| |docs_ci| |coverage| |pypi_version| |license|
-
-A Python client which connects to the control and data ports of the PandABlocks TCP server.
-
-============== ==============================================================
-PyPI           ``pip install pandablocks``
-Source code    https://github.com/PandABlocks/PandABlocks-client
-Documentation  https://pandablocks.github.io/PandABlocks-client
-============== ==============================================================
-
-Command line tool features an interactive console, load/save control, and HDF5
-writing:
-
-.. code::
-
-    $ pip install pandablocks
-
-    $ pandablocks control <panda-hostname>
-    < PCAP.     # Hit TAB key...
-    PCAP.ACTIVE     PCAP.BITS1      PCAP.BITS3      PCAP.GATE       PCAP.SAMPLES    PCAP.TRIG       PCAP.TS_END     PCAP.TS_TRIG
-    PCAP.BITS0      PCAP.BITS2      PCAP.ENABLE     PCAP.HEALTH     PCAP.SHIFT_SUM  PCAP.TRIG_EDGE  PCAP.TS_START
-    < PCAP.ACTIVE?
-    OK =1
-
-    $ pandablocks hdf <panda-hostname> /tmp/panda-%d.h5
-    INFO:Opened '/tmp/panda-1.h5' with 60 byte samples stored in 11 datasets
-    INFO:Closed '/tmp/panda-1.h5' after writing 50000000 samples. End reason is 'Disarmed'
+[![CI](https://github.com/PandABlocks/PandABlocks-client/actions/workflows/ci.yml/badge.svg)](https://github.com/PandABlocks/PandABlocks-client/actions/workflows/ci.yml)
+[![Coverage](https://codecov.io/gh/PandABlocks/PandABlocks-client/branch/main/graph/badge.svg)](https://codecov.io/gh/PandABlocks/PandABlocks-client)
+[![PyPI](https://img.shields.io/pypi/v/pandablocks.svg)](https://pypi.org/project/pandablocks)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+
+# pandablocks
+
+A Python client to control and data ports of the PandABlocks TCP server
+
+Source          | <https://github.com/PandABlocks/PandABlocks-client>
+:---:           | :---:
+PyPI            | `pip install pandablocks`
+Docker          | `docker run ghcr.io/pandablocks/PandABlocks-client:latest`
+Documentation   | <https://pandablocks.github.io/PandABlocks-client>
+Releases        | <https://github.com/PandABlocks/PandABlocks-client/releases>
+
+Command line tool features an interactive console, load/save control, and HDF5 writing:
+
+```shell
+$ pip install pandablocks
+
+$ pandablocks control <panda-hostname>
+< PCAP.     # Hit TAB key...
+PCAP.ACTIVE     PCAP.BITS1      PCAP.BITS3      PCAP.GATE       PCAP.SAMPLES    PCAP.TRIG       PCAP.TS_END     PCAP.TS_TRIG
+PCAP.BITS0      PCAP.BITS2      PCAP.ENABLE     PCAP.HEALTH     PCAP.SHIFT_SUM  PCAP.TRIG_EDGE  PCAP.TS_START
+< PCAP.ACTIVE?
+OK =1
+
+$ pandablocks hdf <panda-hostname> /tmp/panda-%d.h5
+INFO:Opened '/tmp/panda-1.h5' with 60 byte samples stored in 11 datasets
+INFO:Closed '/tmp/panda-1.h5' after writing 50000000 samples. End reason is 'Disarmed'
+```
 
 Library features a Sans-IO core with both asyncio and blocking wrappers:
 
-.. code:: python
-
-    from pandablocks.blocking import BlockingClient
-    from pandablocks.commands import Get
+```python
+from pandablocks.blocking import BlockingClient
+from pandablocks.commands import Get
+
+with BlockingClient("hostname-or-ip") as client:
+    # Commands sent to Control port
+    idn = client.send(Get("*IDN"))
+    print(f"Hello {idn}")
+    for data in client.data():
+        # Data captured from Data port
+        print(f"I got some PCAP data {data}")
+```
 
-    with BlockingClient("hostname-or-ip") as client:
-        # Commands sent to Control port
-        idn = client.send(Get("*IDN"))
-        print(f"Hello {idn}")
-        for data in client.data():
-            # Data captured from Data port
-            print(f"I got some PCAP data {data}")
-
-
-.. |code_ci| image:: https://github.com/PandABlocks/PandABlocks-client/workflows/Code%20CI/badge.svg?branch=master
-    :target: https://github.com/PandABlocks/PandABlocks-client/actions?query=workflow%3A%22Code+CI%22
-    :alt: Code CI
-
-.. |docs_ci| image:: https://github.com/PandABlocks/PandABlocks-client/workflows/Docs%20CI/badge.svg?branch=master
-    :target: https://github.com/PandABlocks/PandABlocks-client/actions?query=workflow%3A%22Docs+CI%22
-    :alt: Docs CI
-
-.. |coverage| image:: https://codecov.io/gh/PandABlocks/PandABlocks-client/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/PandABlocks/PandABlocks-client
-    :alt: Test Coverage
-
-.. |pypi_version| image:: https://badge.fury.io/py/pandablocks.svg
-    :target: https://badge.fury.io/py/pandablocks
-    :alt: Latest PyPI version
-
-.. |license| image:: https://img.shields.io/badge/License-Apache%202.0-blue.svg
-    :target: https://opensource.org/licenses/Apache-2.0
-    :alt: Apache License
-
-..
-    These definitions are used when viewing README.rst and will be replaced
-    when included in index.rst
+<!-- README only content. Anything below this line won't be included in index.md -->
 
 See https://pandablocks.github.io/PandABlocks-client for more detailed documentation.
```

### Comparing `pandablocks-0.7.0/docs/_static/theme_overrides.css` & `pandablocks-0.8.0/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/docs/_templates/layout.html` & `pandablocks-0.8.0/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/docs/conf.py` & `pandablocks-0.8.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,16 +44,21 @@
     "matplotlib.sphinxext.plot_directive",
     # Adds the inheritance-diagram generation directive
     "sphinx.ext.inheritance_diagram",
     # Add a copy button to each code block
     "sphinx_copybutton",
     # For the card element
     "sphinx_design",
+    # So we can write markdown files
+    "myst_parser",
 ]
 
+# So we can use the ::: syntax
+myst_enable_extensions = ["colon_fence"]
+
 # If true, Sphinx will warn about all references where the target cannot
 # be found.
 nitpicky = True
 
 # A list of (type, target) tuples (by default empty) that should be ignored when
 # generating warnings in "nitpicky mode". Note that type should include the
 # domain name if present. Example entries would be ('py:func', 'int') or
@@ -64,14 +69,15 @@
     ("py:class", "'float'"),
     ("py:class", "'int'"),
     ("py:class", "'bool'"),
     ("py:class", "'object'"),
     ("py:class", "'id'"),
     ("py:class", "typing_extensions.Literal"),
     ("py:func", "int"),
+    ("py:class", "pandablocks.commands.T"),
 ]
 
 # Both the class’ and the __init__ method’s docstring are concatenated and
 # inserted into the main body of the autoclass directive
 autoclass_content = "both"
 
 # Order the members by the order they appear in the source code
@@ -83,17 +89,14 @@
 # Output graphviz directive produced images in a scalable format
 graphviz_output_format = "svg"
 
 # The name of a reST role (builtin or Sphinx extension) to use as the default
 # role, that is, for text marked up `like this`
 default_role = "any"
 
-# The suffix of source filenames.
-source_suffix = ".rst"
-
 # The master toctree document.
 master_doc = "index"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # These patterns also affect html_static_path and html_extra_path
 exclude_patterns = ["_build"]
@@ -133,15 +136,15 @@
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "pydata_sphinx_theme"
-github_repo = project
+github_repo = "PandABlocks-client"
 github_user = "PandABlocks"
 switcher_json = f"https://{github_user}.github.io/{github_repo}/switcher.json"
 switcher_exists = requests.get(switcher_json).ok
 if not switcher_exists:
     print(
         "*** Can't read version switcher, is GitHub pages enabled? \n"
         "    Once Docs CI job has successfully run once, set the "
@@ -153,16 +156,16 @@
 # Theme options for pydata_sphinx_theme
 # We don't check switcher because there are 3 possible states for a repo:
 # 1. New project, docs are not published so there is no switcher
 # 2. Existing project with latest skeleton, switcher exists and works
 # 3. Existing project with old skeleton that makes broken switcher,
 #    switcher exists but is broken
 # Point 3 makes checking switcher difficult, because the updated skeleton
-# will fix the switcher at the end of the docs workflow, but never gets a chance
-# to complete as the docs build warns and fails.
+# will fix the switcher at the end of the docs workflow, but never gets a
+# chance to complete as the docs build warns and fails.
 html_theme_options = {
     "logo": {
         "text": project,
     },
     "use_edit_page_button": True,
     "github_url": f"https://github.com/{github_user}/{github_repo}",
     "icon_links": [
@@ -174,20 +177,15 @@
     ],
     "switcher": {
         "json_url": switcher_json,
         "version_match": version,
     },
     "check_switcher": False,
     "navbar_end": ["theme-switcher", "icon-links", "version-switcher"],
-    "external_links": [
-        {
-            "name": "Release Notes",
-            "url": f"https://github.com/{github_user}/{github_repo}/releases",
-        }
-    ],
+    "navigation_with_keys": False,
 }
 
 # A dictionary of values to pass into the template engine’s context for all pages
 html_context = {
     "github_user": github_user,
     "github_repo": project,
     "github_version": version,
```

### Comparing `pandablocks-0.7.0/docs/images/PandA-logo-for-black-background.svg` & `pandablocks-0.8.0/docs/images/PandA-logo-for-black-background.svg`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/docs/images/PandA-logo.ico` & `pandablocks-0.8.0/docs/images/PandA-logo.ico`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/docs/user/explanations/performance.rst` & `pandablocks-0.8.0/docs/explanations/performance.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-.. _performance:
+(performance)=
 
-How fast can we write HDF files?
-================================
+# How fast can we write HDF files?
 
 There are many factors that affect the speed we can write HDF files. This article
 discusses how this library addresses them and what the maximum data rate of a PandA is.
 
-Factors to consider
--------------------
+## Factors to consider
 
+```{eval-rst}
 .. list-table::
     :widths: 10 50
 
     * - Trigger frequency
       - Each trigger will send all the captured fields, so the higher the trigger
         frequency the more data is sent
     * - Fields captured
@@ -28,58 +27,52 @@
       - Some local disks and NFS mounts may not be fast enough to sustain
         maximum data rate.
     * - CPU load on the PandA
       - Excessive CPU load on the PandA, generated by extra TCP server clients
         or panda-webcontrol will reduce throughput
     * - Flush rate
       - Flushing data to disk to often will slow write speed
+```
 
-Strategies to help
-------------------
+## Strategies to help
 
 There are a number of strategies that help increase performance. These can be
 combined to give the greatest benefit
 
-Average the data
-~~~~~~~~~~~~~~~~
+### Average the data
 
-Selecting the ``Mean`` capture mode will activate on-FPGA averaging of the
-captured value. ``Min`` and ``Max`` can also be captured at the same time.
-Capturing these rather than ``Value`` may allow you to lower the trigger
+Selecting the `Mean` capture mode will activate on-FPGA averaging of the
+captured value. `Min` and `Max` can also be captured at the same time.
+Capturing these rather than `Value` may allow you to lower the trigger
 frequency while still providing enough information for data analysis
 
-Scale the data on the client
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### Scale the data on the client
 
-`AsyncioClient.data` and `BlockingClient.data` accept a ``scaled`` argument.
+`AsyncioClient.data` and `BlockingClient.data` accept a `scaled` argument.
 Setting this to False will transfer the raw unscaled data, allowing for up to
 50% more data to be sent depending on the datatype of the field. You can
 use the `StartData.fields` information to scale the data on the client.
 The `write_hdf_files` function uses this approach.
 
-Remove the panda-webcontrol package
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### Remove the panda-webcontrol package
 
 The measures above should get you to about 50MBytes/s, but if more clients
 connect to the web GUI then this will drop. To increase the data rate to
 60MBytes/s and improve stability you may want to remove the panda-webcontrol
 zpkg.
 
-Flush about 1Hz
-~~~~~~~~~~~~~~~
+### Flush about 1Hz
 
-`AsyncioClient.data` accepts a ``flush_period`` argument. If given, it will
+`AsyncioClient.data` accepts a `flush_period` argument. If given, it will
 squash intermediate data frames together until this period expires, and only
 then produce them. This means the numpy data blocks are larger and can be more
 efficiently written to disk then flushed. The `write_hdf_files` function uses
 this approach.
 
-
-Performance Achieved
---------------------
+## Performance Achieved
 
 Tests were run with the following conditions:
 
 - 8-core Intel i7 machine as client
 - Version 2.1 of panda-server installed on PandA
 - PandA and client machine connected to same Gigabit ethernet switch
 - 60 byte sample payload
@@ -96,19 +89,18 @@
 
 - 60MBytes/s throughput
 - PandA CPU usage about 65% (of both cores)
 - local client CPU usage about 60% (of a single core)
 
 Increasing above these throughputs failed most scans with `DATA_OVERRUN`.
 
-Data overruns
--------------
+## Data overruns
 
 If there is a `DATA_OVERRUN`, the server will stop sending data. The most recently
 received `FrameData` from either `AsyncioClient.data` or `BlockingClient.data` may
-be corrupt. This is the case if the ``scaled`` argument is set to False. The mechanism
+be corrupt. This is the case if the `scaled` argument is set to False. The mechanism
 the server uses to send raw unscaled data is only able to detect the corrupt frame after
 it has already been sent. Conversely, the mechanism used to send scaled data aborts prior
 to sending a corrupt frame.
 
-The `write_hdf_files` function uses ``scaled=False``, so your HDF file may include some
+The `write_hdf_files` function uses `scaled=False`, so your HDF file may include some
 corrupt data in the event of an overrun.
```

### Comparing `pandablocks-0.7.0/docs/user/explanations/sans-io.rst` & `pandablocks-0.8.0/docs/explanations/sans-io.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,71 @@
-.. _sans-io:
+(sans-io)=
 
-Why write a Sans-IO library?
-============================
+# Why write a Sans-IO library?
 
-As the reference_ says: *Reusability*. The protocol can be coded in a separate
+As the [reference] says: *Reusability*. The protocol can be coded in a separate
 class to the I/O allowing integration into a number of different concurrency
 frameworks.
 
 For instance, we need both a `BlockingClient` and an `AsyncioClient`. If we had
 coded the protocol in either of them it would not be usable in the other. Much
 better to put it in a separate class and feed it bytes off the wire. We call
 this protocol encapsulation a Connection.
 
-Connections
------------
+## Connections
 
 The PandA TCP server exposes a Control port and a Data port, so there are
-corresponding `ControlConnection` and `DataConnection` objects:
+corresponding [](ControlConnection) and objects:
 
-.. currentmodule:: pandablocks.connections
+The [](ControlConnection) class has the following methods:
 
-.. autoclass:: ControlConnection
-    :noindex:
-
-    The :meth:`~ControlConnection.send` method takes a `Command` subclass and
+- The [`send()`](ControlConnection.send) method takes a `Command` subclass and
     returns the bytes that should be sent to the PandA. Whenever bytes are
-    received from the socket they can be passed to
-    :meth:`~ControlConnection.receive_bytes` which will return any subsequent
-    bytes that should be send back. The :meth:`~ControlConnection.responses`
-    method returns an iterator of ``(command, response)`` tuples that have now
+    received from the socket they can be passed to this method which will return any subsequent
+    bytes that should be send back. 
+- The [`responses()`](ControlConnection.responses) method returns an iterator of ``(command, response)`` tuples that have now
     completed. The response type will depend on the command. For instance `Get`
     returns `bytes` or a `list` of `bytes` of the field value, and `GetFieldInfo`
     returns a `dict` mapping `str` field name to `FieldInfo`.
 
-.. autoclass:: DataConnection
-    :noindex:
+The [](DataConnection) class has the following methods:
 
-    The :meth:`~DataConnection.connect` method takes any connection arguments
+- The [`connect()`](DataConnection.connect) method takes any connection arguments
     and returns the bytes that should be sent to the PandA to make the initial
     connection. Whenever bytes are received from the socket they can be passed
-    to :meth:`~DataConnection.receive_bytes` which will return an iterator of
-    `Data` objects. Intermediate `FrameData` can be squashed together by passing
+    to this method which will return an iterator of
+    `Data` objects. 
+- Intermediate `FrameData` can be squashed together by passing
     ``flush_every_frame=False``, then explicitly calling
-    :meth:`~DataConnection.flush` when they are required.
+    [`flush()`](DataConnection.flush) when they are required.
 
-Wrappers
---------
+## Wrappers
 
 Of course, these Connections are useless without connecting some I/O. To aid with
 this, wrappers are included for use in `asyncio <asyncio>` and blocking programs. They expose
 slightly different APIs to make best use of the features of their respective concurrency frameworks.
 
-For example, to send multiple commands in fields with the `blocking` wrapper::
-
-    with BlockingClient("hostname") as client:
-        resp1, resp2 = client.send([cmd1, cmd2])
-
-while with the `asyncio` wrapper we would::
+For example, to send multiple commands in fields with the `blocking` wrapper:
 
-    async with AsyncioClient("hostname") as client:
-        resp1, resp2 = await asyncio.gather(
-            client.send(cmd1),
-            client.send(cmd2)
-        )
+```
+with BlockingClient("hostname") as client:
+    resp1, resp2 = client.send([cmd1, cmd2])
+```
+
+while with the `asyncio` wrapper we would:
+
+```
+async with AsyncioClient("hostname") as client:
+    resp1, resp2 = await asyncio.gather(
+        client.send(cmd1),
+        client.send(cmd2)
+    )
+```
 
 The first has the advantage of simplicity, but blocks while waiting for data.
 The second allows multiple co-routines to use the client at the same time at the
 expense of a more verbose API.
 
-The wrappers do not guarantee feature parity, for instance the ``flush_period``
+The wrappers do not guarantee feature parity, for instance the `flush_period`
 option is only available in the asyncio wrapper.
 
-
-
-
-
-
-
-.. _reference: https://sans-io.readthedocs.io/
+[reference]: https://sans-io.readthedocs.io/
```

### Comparing `pandablocks-0.7.0/docs/user/how-to/introspect-panda.rst` & `pandablocks-0.8.0/docs/how-to/introspect-panda.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-How to introspect a PandA
-===========================
+# How to introspect a PandA
 
 Using a combination of `commands <pandablocks.commands>` it is straightforward to query the PandA
-to list all blocks, and all fields inside each block, that exist. 
+to list all blocks, and all fields inside each block, that exist.
 
 Call the following script, with the address of the PandA as the first and only command line argument:
 
+```{literalinclude} ../../examples/introspect_panda.py
+```
 
-.. literalinclude:: ../../../examples/introspect_panda.py
-
-This script can be found in ``examples/introspect_panda.py``.
+This script can be found in `examples/introspect_panda.py`.
 
 By examining the `BlockInfo` structure returned from `GetBlockInfo` for each Block the number
 and description may be acquired for every block.
 
-By examining the `FieldInfo` structure (which is fully printed in this example) the ``type``, 
-``sub-type``, ``description`` and ``label`` may all be found for every field. 
+By examining the `FieldInfo` structure (which is fully printed in this example) the `type`,
+`sub-type`, `description` and `label` may all be found for every field.
 
-Lastly the complete list of every ``BITS`` field in the ``PCAP`` block are gathered and
-printed. See the documentation in the `Field Types <https://pandablocks-server.readthedocs.io/en/latest/fields.html?#field-types>`_
+Lastly the complete list of every `BITS` field in the `PCAP` block are gathered and
+printed. See the documentation in the [Field Types](https://pandablocks-server.readthedocs.io/en/latest/fields.html?#field-types)
 section of the PandA Server documentation.
```

### Comparing `pandablocks-0.7.0/docs/user/how-to/library-hdf.rst` & `pandablocks-0.8.0/docs/how-to/library-hdf.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-.. _library-hdf:
+(library-hdf)=
 
-How to use the library to capture HDF files
-===========================================
+# How to use the library to capture HDF files
 
 The `commandline-hdf` introduced how to use the commandline to capture HDF files.
 The `write_hdf_files` function that is called to do this can also be integrated
 into custom Python applications. This guide shows how to do this.
 
-Approach 1: Call the function directly
---------------------------------------
+## Approach 1: Call the function directly
 
 If you need a one-shot configure and run application, you can use the
 function directly:
 
-.. literalinclude:: ../../../examples/arm_and_hdf.py
+```{literalinclude} ../../examples/arm_and_hdf.py
+```
 
 With the `AsyncioClient` as a `Context Manager <typecontextmanager>`, this code
 sets up some fields of a PandA before taking a single acquisition. The code in
 `write_hdf_files` is responsible for arming the PandA.
 
-.. note::
+:::{note}
+There are no log messages emitted like in `commandline-hdf`. This is because
+we have not configured the logging framework in this example. You can get
+these messages by adding a call to `logging.basicConfig` like this:
+
+```
+logging.basicConfig(level=logging.INFO)
+```
+:::
 
-    There are no log messages emitted like in `commandline-hdf`. This is because
-    we have not configured the logging framework in this example. You can get
-    these messages by adding a call to `logging.basicConfig` like this::
-
-        logging.basicConfig(level=logging.INFO)
-
-Approach 2: Create the pipeline yourself
-----------------------------------------
+## Approach 2: Create the pipeline yourself
 
 If you need more control over the pipeline, for instance to display progress,
 you can create the pipeline yourself, and feed it data from the PandA. This
 means you can make decisions about when to start and stop acquisitions based on
 the `Data` objects that go past. For example, if we want to make a progress bar
 we could:
 
-.. literalinclude:: ../../../examples/hdf_queue_reporting.py
+```{literalinclude} ../../examples/hdf_queue_reporting.py
+```
 
 This time, after setting up the PandA, we create the `AsyncioClient.data`
 iterator ourselves. Each `Data` object we get is queued on the first `Pipeline`
 element, then inspected. The type of object tells us if we should Arm the PandA,
 update a progress bar, or return as acquisition is complete.
 
 In a `finally <finally>` block we stop the pipeline, which will wait for all data
 to flow through the pipeline and close the HDF file.
 
-Performance
------------
+## Performance
 
 The commandline client and both these approaches use the same core code, so will
 give the same performance. The steps to consider in optimising performance are
-outlined in `performance`
+outlined in `performance`
```

### Comparing `pandablocks-0.7.0/docs/user/reference/api.rst` & `pandablocks-0.8.0/docs/reference/api.rst`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -85,8 +85,8 @@
     .. seealso:: `library-hdf`, `performance`
 
 .. automodule:: pandablocks.utils    
     
     Utilities
     ---------
 
-    This package contains general methods for working with pandablocks.
+    This package contains general methods for working with pandablocks.
```

### Comparing `pandablocks-0.7.0/docs/user/tutorials/control.rst` & `pandablocks-0.8.0/docs/tutorials/control.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,68 @@
-Interactive Control Tutorial
-============================
+# Interactive Control Tutorial
 
 This tutorial shows how to use the commandline tool to open an interactive terminal
 to control a PandA.
 
-Connect
--------
+## Connect
 
-Open a terminal, and type::
+Open a terminal, and type:
 
-    pandablocks control <hostname>
+```
+pandablocks control <hostname>
+```
 
-Where ``<hostname>`` is the hostname or ip address of your PandA.
+Where `<hostname>` is the hostname or ip address of your PandA.
 
-Type Commands
--------------
+## Type Commands
 
 You should be presented with a prompt where you can type PandABlocks-server
-commands_. If you are on Linux you can tab complete commands with the TAB key::
+[commands]. If you are on Linux you can tab complete commands with the TAB key:
 
-    < PCAP.     # Hit TAB key...
-    PCAP.ACTIVE     PCAP.BITS1      PCAP.BITS3      PCAP.GATE       PCAP.SAMPLES    PCAP.TRIG       PCAP.TS_END     PCAP.TS_TRIG
-    PCAP.BITS0      PCAP.BITS2      PCAP.ENABLE     PCAP.HEALTH     PCAP.SHIFT_SUM  PCAP.TRIG_EDGE  PCAP.TS_START
+```
+< PCAP.     # Hit TAB key...
+PCAP.ACTIVE     PCAP.BITS1      PCAP.BITS3      PCAP.GATE       PCAP.SAMPLES    PCAP.TRIG       PCAP.TS_END     PCAP.TS_TRIG
+PCAP.BITS0      PCAP.BITS2      PCAP.ENABLE     PCAP.HEALTH     PCAP.SHIFT_SUM  PCAP.TRIG_EDGE  PCAP.TS_START
+```
 
 Pressing return will send the command to the server and display the response.
 
-Control an acquisition
-----------------------
+## Control an acquisition
 
 You can check if an acquisition is currently in progress by getting the value of the
-``PCAP.ACTIVE`` field::
+`PCAP.ACTIVE` field:
 
-    < PCAP.ACTIVE?
-    OK =0
+```
+< PCAP.ACTIVE?
+OK =0
+```
 
-You can start and stop acquisitions with special "star" commands. To start an acquisition::
+You can start and stop acquisitions with special "star" commands. To start an acquisition:
 
-    < *PCAP.ARM=
-    OK
+```
+< *PCAP.ARM=
+OK
+```
 
-You can now use the up arrow to recall the previous command, then press return::
+You can now use the up arrow to recall the previous command, then press return:
 
-    < PCAP.ACTIVE?
-    OK =1
+```
+< PCAP.ACTIVE?
+OK =1
+```
 
-This means that acquisition is in progress. You can stop it by disarming::
+This means that acquisition is in progress. You can stop it by disarming:
 
-    < *PCAP.DISARM=
-    OK
-    < PCAP.ACTIVE?
-    OK =0
+```
+< *PCAP.DISARM=
+OK
+< PCAP.ACTIVE?
+OK =0
+```
 
-Conclusion
-----------
+## Conclusion
 
 This tutorial has shown how to start and stop an acquisition from the commandline
-client. It can also be used to send any other control commands_ to query and set
+client. It can also be used to send any other control [commands] to query and set
 variables on the PandA.
 
-.. _commands: https://pandablocks-server.readthedocs.io/en/latest/commands.html
+[commands]: https://pandablocks-server.readthedocs.io/en/latest/commands.html
```

### Comparing `pandablocks-0.7.0/docs/user/tutorials/load-save.rst` & `pandablocks-0.8.0/docs/tutorials/load-save.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,61 @@
-.. _tutorial-load-save:
+(tutorial-load-save)=
 
-Commandline Load/Save Tutorial
-==============================
+# Commandline Load/Save Tutorial
 
 This tutorial shows how to use the commandline tool to save the state of all the
 Blocks and Fields in a PandA, and load a new state from file. It assumes that
 you know the basic concepts of a PandA as outlined in the PandABlocks-FPGA
-blinking LEDs tutorial_.
+blinking LEDs [tutorial].
 
-Save
-----
+## Save
 
-You can save the current state using the save command as follows::
+You can save the current state using the save command as follows:
 
-    $ pandablocks save <hostname> <save_file>
+```
+$ pandablocks save <hostname> <save_file>
+```
 
 The save file is a text file containing the sequence of pandablocks control
 commands that will set up the PandA to match its state at the time of the save.
 This is a human readable file and may be edited if you want to modify a few
 fields.
 
 e.g. the first few lines of the tutorial save file look like this:
 
-.. literalinclude:: ../../../src/pandablocks/saves/tutorial.sav
-   :lines: 1-12
+```{literalinclude} ../../src/pandablocks/saves/tutorial.sav
+:lines: 1-12
+```
 
-Load
-----
+## Load
 
-To restore a PandA to a previously saved state use the load command as follows::
+To restore a PandA to a previously saved state use the load command as follows:
 
-    $ pandablocks load <hostname> <save_file>
+```
+$ pandablocks load <hostname> <save_file>
+```
 
-This is equivalent to typing the sequence of commands in <save_file> into the
+This is equivalent to typing the sequence of commands in \<save_file> into the
 pandablocks control command line.
 
-To load the preconfigured tutorial state::
+To load the preconfigured tutorial state:
 
-    $ pandablocks load <hostname> --tutorial
+```
+$ pandablocks load <hostname> --tutorial
+```
 
 The tutorial sets up a Seqencer block driving 3 Counter blocks and a Position
 Capture block. This configuration is the starting point for the next tutorial:
-:ref:`commandline-hdf`
+{ref}`commandline-hdf`
 
-.. note::
-
-    The Web UI will not change the Blocks visible on the screen when you use
-    ``pandablocks load``. If you want all the connected Blocks to appear in the
-    UI then restart the services on the PandA (Admin > System > Reboot/Restart)
+:::{note}
+The Web UI will not change the Blocks visible on the screen when you use
+`pandablocks load`. If you want all the connected Blocks to appear in the
+UI then restart the services on the PandA (Admin > System > Reboot/Restart)
+:::
 
 The tutorial blocks are wired up as shown in the following Web UI layout.
 
-.. image:: tutorial_layout.png
+```{image} tutorial_layout.png
+```
 
-.. _tutorial: https://pandablocks-fpga.readthedocs.io/en/latest/tutorials/tutorial1_blinking_leds.html
+[tutorial]: https://pandablocks-fpga.readthedocs.io/en/latest/tutorials/tutorial1_blinking_leds.html
```

### Comparing `pandablocks-0.7.0/docs/user/tutorials/tutorial_layout.png` & `pandablocks-0.8.0/docs/tutorials/tutorial_layout.png`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/examples/arm_and_hdf.py` & `pandablocks-0.8.0/examples/arm_and_hdf.py`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/examples/hdf_queue_reporting.py` & `pandablocks-0.8.0/examples/hdf_queue_reporting.py`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/examples/introspect_panda.py` & `pandablocks-0.8.0/examples/introspect_panda.py`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/pyproject.toml` & `pandablocks-0.8.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 [build-system]
-requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2", "wheel"]
+requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
-description = "A Python client to control and data ports of the PandABlocks TCP server"
 name = "pandablocks"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
+description = "A Python client to control and data ports of the PandABlocks TCP server"
 dependencies = ["typing-extensions;python_version<'3.8'", "numpy", "click"]
 dynamic = ["version"]
-license.file = "Apache License 2.0"
-readme = "README.rst"
+license.file = "LICENSE"
+readme = "README.md"
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 h5py = ["h5py", "matplotlib"]
 dev = [
     # A dev install will require [h5py] packages too
     "pandablocks[h5py]",
-    "black",
     "mypy",
     "mock",
     "types-mock",
     "atomicwrites",
     "typed-ast",
+    "copier",
+    "myst-parser",
     "pipdeptree",
     "pre-commit",
     "pydata-sphinx-theme>=0.12",
+    "pytest",
     "pytest-cov",
     "pytest-asyncio",
     "ruff",
     "sphinx-autobuild",
     "sphinx-copybutton",
     "sphinx-design",
     "tox-direct",
     "types-mock",
 ]
 
 [project.scripts]
 pandablocks = "pandablocks.cli:cli"
 
 [project.urls]
-GitHub = "https://github.com/PandABlocks/Pandablocks-client"
+GitHub = "https://github.com/PandABlocks/PandABlocks-client"
 
 [[project.authors]] # Further authors may be added by duplicating this section
 email = "tom.cobb@diamond.ac.uk"
 name = "Tom Cobb"
 
 
 [tool.setuptools_scm]
@@ -61,15 +63,14 @@
 [tool.mypy]
 ignore_missing_imports = true # Ignore missing stubs in imported modules
 
 [tool.pytest.ini_options]
 # Run pytest with all our checkers, and don't spam us with massive tracebacks on error
 addopts = """
     --tb=native -vv --doctest-modules --doctest-glob="*.rst"
-    --cov=src/pandablocks --cov-report term --cov-report xml:cov.xml 
     """
 asyncio_mode = "auto"
 # Doctest python code in docs, python code in src docstrings, test functions in tests
 testpaths = "docs src tests"
 
 [tool.coverage.run]
 data_file = "/tmp/pandablocks.coverage"
@@ -81,35 +82,38 @@
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 skipsdist=True
 
-[testenv:{pre-commit,mypy,pytest,docs}]
+[testenv:{pre-commit,type-checking,tests,docs}]
 # Don't create a virtualenv for the command, requires tox-direct plugin
 direct = True
 passenv = *
 allowlist_externals =
     pytest
     pre-commit
     mypy
     sphinx-build
     sphinx-autobuild
 commands =
-    pytest: pytest {posargs}
+    pytest: pytest --cov=src/pandablocks --cov-report term --cov-report xml:cov.xml {posargs}
     mypy: mypy src tests {posargs}
-    pre-commit: pre-commit run --all-files {posargs}
+    pre-commit: pre-commit run --all-files --show-diff-on-failure {posargs}
+    type-checking: mypy src tests {posargs}
+    tests: pytest --cov=pandablocks --cov-report term --cov-report xml:cov.xml {posargs}
     docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html
 """
 
-
 [tool.ruff]
 src = ["src", "tests"]
 line-length = 88
-select = [
-    "C4",   # flake8-comprehensions - https://beta.ruff.rs/docs/rules/#flake8-comprehensions-c4
-    "E",    # pycodestyle errors - https://beta.ruff.rs/docs/rules/#error-e
-    "F",    # pyflakes rules - https://beta.ruff.rs/docs/rules/#pyflakes-f
-    "W",    # pycodestyle warnings - https://beta.ruff.rs/docs/rules/#warning-w
-    "I001", # isort
+lint.select = [
+    "B",  # flake8-bugbear - https://docs.astral.sh/ruff/rules/#flake8-bugbear-b
+    "C4", # flake8-comprehensions - https://docs.astral.sh/ruff/rules/#flake8-comprehensions-c4
+    "E",  # pycodestyle errors - https://docs.astral.sh/ruff/rules/#error-e
+    "F",  # pyflakes rules - https://docs.astral.sh/ruff/rules/#pyflakes-f
+    "W",  # pycodestyle warnings - https://docs.astral.sh/ruff/rules/#warning-w
+    "I",  # isort - https://docs.astral.sh/ruff/rules/#isort-i
+    "UP", # pyupgrade - https://docs.astral.sh/ruff/rules/#pyupgrade-up
 ]
```

### Comparing `pandablocks-0.7.0/src/pandablocks/_control.py` & `pandablocks-0.8.0/src/pandablocks/_control.py`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/src/pandablocks/_exchange.py` & `pandablocks-0.8.0/src/pandablocks/_exchange.py`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/src/pandablocks/asyncio.py` & `pandablocks-0.8.0/src/pandablocks/asyncio.py`

 * *Files 8% similar despite different names*

```diff
@@ -95,16 +95,29 @@
         await self.connect()
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self.close()
 
     async def _ctrl_read_forever(self, reader: asyncio.StreamReader):
+        """Continually read data from the stream reader and add to the data queue.
+
+        Args:
+            reader: The `StreamReader` to read from
+        """
         while True:
             received = await reader.read(4096)
+            if received == b"":
+                error_str = (
+                    "Received an empty packet. Closing connection. "
+                    "Has the PandA disconnected?"
+                )
+                logging.error(error_str)
+                raise ConnectionError(error_str)
+
             try:
                 to_send = self._ctrl_connection.receive_bytes(received)
                 await self._ctrl_stream.write_and_drain(to_send)
                 for command, response in self._ctrl_connection.responses():
                     queue = self._ctrl_queues.pop(id(command))
                     queue.put_nowait(response)
             except Exception:
```

### Comparing `pandablocks-0.7.0/src/pandablocks/blocking.py` & `pandablocks-0.8.0/src/pandablocks/blocking.py`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/src/pandablocks/cli.py` & `pandablocks-0.8.0/src/pandablocks/cli.py`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/src/pandablocks/commands.py` & `pandablocks-0.8.0/src/pandablocks/commands.py`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/src/pandablocks/connections.py` & `pandablocks-0.8.0/src/pandablocks/connections.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,18 @@
     "NeedMoreData",
     "NoContextAvailable",
     "Buffer",
     "ControlConnection",
     "DataConnection",
 ]
 
-# The name of the samples field used for averaging unscaled fields
+# The names of the samples field used for averaging unscaled fields
+# In newer versions it's GATE_DURATION but we keep SAMPLES for backwards
+# compatibility
+GATE_DURATION_FIELD = "PCAP.GATE_DURATION.Value"
 SAMPLES_FIELD = "PCAP.SAMPLES.Value"
 
 
 class NeedMoreData(Exception):
     """Raised if the `Buffer` isn't full enough to return the requested bytes"""
 
 
@@ -98,16 +101,16 @@
 
     def __iter__(self):
         return self
 
     def __next__(self) -> bytes:
         try:
             return self.read_line()
-        except NeedMoreData:
-            raise StopIteration()
+        except NeedMoreData as err:
+            raise StopIteration() from err
 
 
 @dataclass
 class _ExchangeContext:
     #: The exchange we should be filling
     exchange: Exchange
     #: The command that produced it
@@ -321,20 +324,29 @@
                 fields.insert(
                     0,
                     FieldCapture(name, np.dtype("uint32"), capture),
                 )
             self._frame_dtype = np.dtype(
                 [(f"{f.name}.{f.capture}", f.type) for f in fields]
             )
+
+            try:
+                hw_time_offset_ns = np.int64(data.get("hw_time_offset_ns", ""))
+            except ValueError:
+                hw_time_offset_ns = None
+
             yield StartData(
                 fields=fields,
                 missed=int(data.get("missed")),
                 process=str(data.get("process")),
                 format=str(data.get("format")),
                 sample_bytes=sample_bytes,
+                arm_time=data.get("arm_time", None),
+                start_time=data.get("start_time", None),
+                hw_time_offset_ns=hw_time_offset_ns,
             )
             self._next_handler = self._handle_header_end
 
     def _handle_header_end(self):
         # Discard the newline at the end of the header
         assert self._buf.read_bytes(1) == b"\n", "Expected newline at end of header"
         self._next_handler = self._handle_data_start
```

### Comparing `pandablocks-0.7.0/src/pandablocks/hdf.py` & `pandablocks-0.8.0/src/pandablocks/hdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import h5py
 import numpy as np
 
 from pandablocks.commands import Arm
 
 from .asyncio import AsyncioClient
-from .connections import SAMPLES_FIELD
+from .connections import GATE_DURATION_FIELD, SAMPLES_FIELD
 from .responses import EndData, EndReason, FieldCapture, FrameData, ReadyData, StartData
 
 # Define the public API of this module
 __all__ = [
     "Pipeline",
     "HDFWriter",
     "FrameProcessor",
@@ -115,14 +115,23 @@
                 "Not enough file names available when opening new HDF5 file"
             )
             raise
         self.hdf_file = h5py.File(self.file_path, "w", libver="latest")
         raw = data.process == "Raw"
         self.datasets = [self.create_dataset(field, raw) for field in data.fields]
         self.hdf_file.swmr_mode = True
+
+        # Save parameters
+        if data.arm_time is not None:
+            self.hdf_file.attrs["arm_time"] = data.arm_time
+        if data.start_time is not None:
+            self.hdf_file.attrs["start_time"] = data.start_time
+        if data.hw_time_offset_ns is not None:
+            self.hdf_file.attrs["hw_time_offset_ns"] = data.hw_time_offset_ns
+
         logging.info(
             f"Opened '{self.file_path}' with {data.sample_bytes} byte samples "
             f"stored in {len(self.datasets)} datasets"
         )
 
     def write_frame(self, data: List[np.ndarray]):
         for dataset, column in zip(self.datasets, data):
@@ -155,19 +164,26 @@
         self.what_to_do = {
             StartData: self.create_processors,
             FrameData: self.scale_data,
         }
 
     def create_processor(self, field: FieldCapture, raw: bool):
         column_name = f"{field.name}.{field.capture}"
+
         if raw and field.capture == "Mean":
-            return (
-                lambda data: data[column_name] * field.scale / data[SAMPLES_FIELD]
-                + field.offset
-            )
+
+            def mean_callable(data):
+                if GATE_DURATION_FIELD in data.dtype.names:
+                    gate_duration = data[GATE_DURATION_FIELD]
+                else:
+                    gate_duration = data[SAMPLES_FIELD]
+
+                return (data[column_name] * field.scale / gate_duration) + field.offset
+
+            return mean_callable
         elif raw and (field.scale != 1 or field.offset != 0):
             return lambda data: data[column_name] * field.scale + field.offset
         else:
             return lambda data: data[column_name]
 
     def create_processors(self, data: StartData) -> StartData:
         raw = data.process == "Raw"
```

### Comparing `pandablocks-0.7.0/src/pandablocks/responses.py` & `pandablocks-0.8.0/src/pandablocks/responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,14 +262,17 @@
     """
 
     fields: List[FieldCapture]
     missed: int
     process: str
     format: str
     sample_bytes: int
+    arm_time: Optional[str]
+    start_time: Optional[str]
+    hw_time_offset_ns: Optional[int]
 
 
 @dataclass
 class FrameData(Data):
     """Yielded when a new data frame is flushed.
 
     Attributes:
```

### Comparing `pandablocks-0.7.0/src/pandablocks/saves/tutorial.sav` & `pandablocks-0.8.0/src/pandablocks/saves/tutorial.sav`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/src/pandablocks/utils.py` & `pandablocks-0.8.0/src/pandablocks/utils.py`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/src/pandablocks.egg-info/SOURCES.txt` & `pandablocks-0.8.0/src/pandablocks.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,69 @@
+.copier-answers.yml
 .gitignore
 .pre-commit-config.yaml
 Dockerfile
 LICENSE
-README.rst
+README.md
+catalog-info.yaml
 pyproject.toml
 .devcontainer/devcontainer.json
+.github/CONTRIBUTING.md
 .github/dependabot.yml
 .github/actions/install_requirements/action.yml
 .github/pages/index.html
 .github/pages/make_switcher.py
-.github/workflows/code.yml
-.github/workflows/docs.yml
-.github/workflows/docs_clean.yml
-.github/workflows/linkcheck.yml
+.github/workflows/_check.yml
+.github/workflows/_container.yml
+.github/workflows/_dist.yml
+.github/workflows/_docs.yml
+.github/workflows/_pypi.yml
+.github/workflows/_release.yml
+.github/workflows/_test.yml
+.github/workflows/_tox.yml
+.github/workflows/ci.yml
+.github/workflows/periodic.yml
 .vscode/extensions.json
 .vscode/launch.json
 .vscode/settings.json
 .vscode/tasks.json
-docs/CHANGELOG.rst
-docs/CONTRIBUTING.rst
 docs/conf.py
-docs/genindex.rst
-docs/index.rst
+docs/explanations.md
+docs/genindex.md
+docs/how-to.md
+docs/index.md
+docs/reference.md
+docs/tutorials.md
 docs/_static/theme_overrides.css
 docs/_templates/layout.html
-docs/developer/index.rst
-docs/developer/explanations/decisions.rst
-docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
-docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
-docs/developer/explanations/decisions/0003-make-library-sans-io.rst
-docs/developer/how-to/build-docs.rst
-docs/developer/how-to/contribute.rst
-docs/developer/how-to/lint.rst
-docs/developer/how-to/make-release.rst
-docs/developer/how-to/pin-requirements.rst
-docs/developer/how-to/run-tests.rst
-docs/developer/how-to/static-analysis.rst
-docs/developer/how-to/test-container.rst
-docs/developer/how-to/update-tools.rst
-docs/developer/reference/standards.rst
-docs/developer/tutorials/dev-install.rst
+docs/explanations/decisions.md
+docs/explanations/performance.md
+docs/explanations/sans-io.md
+docs/explanations/decisions/0001-record-architecture-decisions.md
+docs/explanations/decisions/0002-switched-to-python-copier-template.md
+docs/explanations/decisions/0003-make-library-sans-io.md
+docs/explanations/decisions/COPYME
+docs/how-to/contribute.md
+docs/how-to/introspect-panda.md
+docs/how-to/library-hdf.md
+docs/how-to/poll-changes.md
+docs/how-to/run-container.md
 docs/images/PandA-logo-for-black-background.svg
 docs/images/PandA-logo.ico
-docs/user/index.rst
-docs/user/explanations/docs-structure.rst
-docs/user/explanations/performance.rst
-docs/user/explanations/sans-io.rst
-docs/user/how-to/introspect-panda.rst
-docs/user/how-to/library-hdf.rst
-docs/user/how-to/poll-changes.rst
-docs/user/how-to/run-container.rst
-docs/user/reference/api.rst
-docs/user/reference/appendix.rst
-docs/user/reference/changelog.rst
-docs/user/reference/contributing.rst
-docs/user/tutorials/commandline-hdf.rst
-docs/user/tutorials/control.rst
-docs/user/tutorials/installation.rst
-docs/user/tutorials/load-save.rst
-docs/user/tutorials/tutorial_layout.png
+docs/reference/api.rst
+docs/tutorials/commandline-hdf.md
+docs/tutorials/control.md
+docs/tutorials/installation.md
+docs/tutorials/load-save.md
+docs/tutorials/tutorial_layout.png
 examples/README.rst
 examples/arm_and_hdf.py
 examples/hdf_queue_reporting.py
 examples/introspect_panda.py
+examples/load_abs_timestamps.py
 examples/plot_counter_hdf.py
 src/pandablocks/__init__.py
 src/pandablocks/__main__.py
 src/pandablocks/_control.py
 src/pandablocks/_exchange.py
 src/pandablocks/_version.py
 src/pandablocks/asyncio.py
@@ -82,17 +79,18 @@
 src/pandablocks.egg-info/dependency_links.txt
 src/pandablocks.egg-info/entry_points.txt
 src/pandablocks.egg-info/requires.txt
 src/pandablocks.egg-info/top_level.txt
 src/pandablocks/saves/tutorial.sav
 tests/__init__.py
 tests/conftest.py
-tests/fast_dump.txt
-tests/raw_dump.txt
-tests/slow_dump.txt
 tests/test_asyncio.py
 tests/test_blocking.py
 tests/test_cli.py
 tests/test_completer.py
 tests/test_hdf.py
 tests/test_pandablocks.py
-tests/test_utils.py
+tests/test_utils.py
+tests/data_dumps/fast_dump.bin
+tests/data_dumps/raw_dump.bin
+tests/data_dumps/raw_dump_no_duration.bin
+tests/data_dumps/slow_dump.bin
```

### Comparing `pandablocks-0.7.0/tests/fast_dump.txt` & `pandablocks-0.8.0/tests/data_dumps/fast_dump.bin`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/tests/raw_dump.txt` & `pandablocks-0.8.0/tests/data_dumps/raw_dump_no_duration.bin`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/tests/slow_dump.txt` & `pandablocks-0.8.0/tests/data_dumps/slow_dump.bin`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/tests/test_blocking.py` & `pandablocks-0.8.0/tests/test_blocking.py`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/tests/test_cli.py` & `pandablocks-0.8.0/tests/test_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,83 +1,84 @@
 from collections import deque
 from pathlib import Path
 from unittest.mock import patch
 
 import h5py
-import numpy as np
 import pytest
 from click.testing import CliRunner
 
 from pandablocks import cli
-from pandablocks.hdf import HDFDataOverrunException
-from tests.conftest import STATE_RESPONSES, STATE_SAVEFILE, DummyServer
-
-
-def test_writing_fast_hdf(dummy_server_in_thread: DummyServer, raw_dump, tmp_path):
+from pandablocks.hdf import GATE_DURATION_FIELD, SAMPLES_FIELD, HDFDataOverrunException
+from tests.conftest import (
+    STATE_RESPONSES,
+    STATE_SAVEFILE,
+    DummyServer,
+    assert_all_data_in_hdf_file,
+)
+
+
+@pytest.mark.parametrize("samples_name", [GATE_DURATION_FIELD, SAMPLES_FIELD])
+def test_writing_fast_hdf(
+    samples_name,
+    dummy_server_in_thread: DummyServer,
+    raw_dump,
+    raw_dump_no_duration,
+    tmp_path,
+):
     dummy_server_in_thread.send.append("OK")
-    dummy_server_in_thread.data = raw_dump
+    if samples_name == GATE_DURATION_FIELD:
+        dummy_server_in_thread.data = raw_dump
+    else:
+        dummy_server_in_thread.data = raw_dump_no_duration
+
     runner = CliRunner()
     result = runner.invoke(
         cli.cli, ["hdf", "localhost", str(tmp_path / "%d.h5"), "--arm"]
     )
     assert result.exit_code == 0
     hdf_file = h5py.File(tmp_path / "1.h5", "r")
     assert list(hdf_file) == [
         "COUNTER1.OUT.Max",
         "COUNTER1.OUT.Mean",
         "COUNTER1.OUT.Min",
         "COUNTER2.OUT.Mean",
         "COUNTER3.OUT.Value",
         "PCAP.BITS2.Value",
-        "PCAP.SAMPLES.Value",
+        samples_name,
         "PCAP.TS_START.Value",
     ]
     assert dummy_server_in_thread.received == ["*PCAP.ARM="]
-    assert_all_data_in_hdf_file(hdf_file)
+    assert_all_data_in_hdf_file(hdf_file, samples_name)
 
 
 def test_writing_overrun_hdf(
     dummy_server_in_thread: DummyServer, overrun_dump, tmp_path
 ):
     dummy_server_in_thread.send.append("OK")
     dummy_server_in_thread.data = [overrun_dump]
     runner = CliRunner()
     result = runner.invoke(
         cli.cli, ["hdf", "localhost", str(tmp_path / "%d.h5"), "--arm"]
     )
     assert result.exit_code == 1
     assert isinstance(result.exception, HDFDataOverrunException)
     hdf_file = h5py.File(tmp_path / "1.h5", "r")
-    assert_all_data_in_hdf_file(hdf_file)
-
-
-def assert_all_data_in_hdf_file(hdf_file):
-    def multiples(num, offset=0):
-        return pytest.approx(np.arange(1, 10001) * num + offset)
-
-    assert hdf_file["/COUNTER1.OUT.Max"][:] == multiples(1)
-    assert hdf_file["/COUNTER1.OUT.Mean"][:] == multiples(1)
-    assert hdf_file["/COUNTER1.OUT.Min"][:] == multiples(1)
-    assert hdf_file["/COUNTER2.OUT.Mean"][:] == multiples(2)
-    assert hdf_file["/COUNTER3.OUT.Value"][:] == multiples(3)
-    assert hdf_file["/PCAP.BITS2.Value"][:] == multiples(0)
-    assert hdf_file["/PCAP.SAMPLES.Value"][:] == multiples(0, offset=125)
-    assert hdf_file["/PCAP.TS_START.Value"][:] == multiples(2e-6, offset=7.2e-8 - 2e-6)
+    assert_all_data_in_hdf_file(hdf_file, "PCAP.GATE_DURATION.Value")
 
 
 class MockInput:
     def __init__(self, *commands: str):
         self._commands = deque(commands)
 
     def __call__(self, prompt):
         assert prompt == cli.PROMPT
         try:
             return self._commands.popleft()
-        except IndexError:
-            raise EOFError()
+        except IndexError as err:
+            raise EOFError() from err
 
 
 def test_interactive_simple(dummy_server_in_thread, capsys):
     mock_input = MockInput("PCAP.ACTIVE?", "SEQ1.TABLE?")
     dummy_server_in_thread.send += ["OK =0", "!1\n!2\n!3\n!4\n."]
     with patch("pandablocks._control.input", side_effect=mock_input):
         runner = CliRunner()
```

### Comparing `pandablocks-0.7.0/tests/test_completer.py` & `pandablocks-0.8.0/tests/test_completer.py`

 * *Files identical despite different names*

### Comparing `pandablocks-0.7.0/tests/test_hdf.py` & `pandablocks-0.8.0/tests/test_hdf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import queue
 from pathlib import Path
 
 import numpy as np
 
-from pandablocks.hdf import (
-    Pipeline,
-    create_default_pipeline,
-    stop_pipeline,
-)
+from pandablocks.hdf import Pipeline, create_default_pipeline, stop_pipeline
 from pandablocks.responses import EndData, EndReason, FieldCapture, FrameData, StartData
 
 
 def test_pipeline_returns_number_written(tmp_path):
     NUMBER_OF_FRAMES_WRITTEN = 10000
 
     num_written_queue = queue.Queue()
@@ -40,14 +36,17 @@
                         units="",
                     )
                 ],
                 0,
                 "Scaled",
                 "Framed",
                 52,
+                "2024-03-05T20:27:12.607841574Z",
+                "2024-03-05T20:27:12.608875498Z",
+                100555,
             ),
         )
         pipeline[0].queue.put_nowait(
             FrameData(
                 np.array(
                     NUMBER_OF_FRAMES_WRITTEN * [(1,)],
                     dtype=[("COUNTER1.OUT.Value", "<f8")],
```

### Comparing `pandablocks-0.7.0/tests/test_pandablocks.py` & `pandablocks-0.8.0/tests/test_pandablocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,26 +340,29 @@
                     labels=["Input-Level", "Pulse-On-Rising-Edge"],
                 ),
             },
         )
     ]
 
 
-def test_get_fields_type_ext_out():
+@pytest.mark.parametrize("gate_duration_name", ["GATE_DURATION", "SAMPLES"])
+def test_get_fields_type_ext_out(gate_duration_name):
     """Test for field type == ext_out, ensuring we add .CAPTURE to the end of the
     *ENUMS command"""
     conn = ControlConnection()
     cmd = GetFieldInfo("PCAP")
     assert conn.send(cmd) == b"PCAP.*?\n"
 
     # First yield, the response to "PCAP.*?"
-    assert (
-        conn.receive_bytes(b"!SAMPLES 9 ext_out samples\n.\n")
-        == b"*DESC.PCAP.SAMPLES?\n*ENUMS.PCAP.SAMPLES.CAPTURE?\n"
+    request_str = bytes(f"!{gate_duration_name} 9 ext_out samples\n.\n", "utf-8")
+    response_str = bytes(
+        f"*DESC.PCAP.{gate_duration_name}?\n*ENUMS.PCAP.{gate_duration_name}.CAPTURE?\n",
+        "utf-8",
     )
+    assert conn.receive_bytes(request_str) == response_str
 
     # Responses to the *DESC and *ENUM commands
     responses = [
         b"OK =Number of gated samples in the current capture\n",
         b"!No\n!Value\n.\n",
     ]
     for response in responses:
@@ -367,15 +370,15 @@
             conn.receive_bytes(response) == b""
         )  # Expect no bytes back as none of these trigger further commands
 
     assert get_responses(conn) == [
         (
             cmd,
             {
-                "SAMPLES": ExtOutFieldInfo(
+                gate_duration_name: ExtOutFieldInfo(
                     type="ext_out",
                     subtype="samples",
                     description="Number of gated samples in the current capture",
                     capture_labels=["No", "Value"],
                 )
             },
         )
```

### Comparing `pandablocks-0.7.0/tests/test_utils.py` & `pandablocks-0.8.0/tests/test_utils.py`

 * *Files identical despite different names*


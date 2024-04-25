# Comparing `tmp/ethpm-types-0.6.8.tar.gz` & `tmp/ethpm-types-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethpm-types-0.6.8.tar", last modified: Tue Apr  2 15:32:14 2024, max compression
+gzip compressed data, was "ethpm-types-0.6.9.tar", last modified: Tue Apr  9 17:17:06 2024, max compression
```

## Comparing `ethpm-types-0.6.8.tar` & `ethpm-types-0.6.9.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:14.010696 ethpm-types-0.6.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.986696 ethpm-types-0.6.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.986696 ethpm-types-0.6.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.986696 ethpm-types-0.6.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-02 15:32:14.010696 ethpm-types-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/build_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/cz-requirement.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.986696 ethpm-types-0.6.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.986696 ethpm-types-0.6.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.986696 ethpm-types-0.6.8/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.986696 ethpm-types-0.6.8/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/methoddocs/abi.md
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/methoddocs/contract_type.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/methoddocs/manifest.md
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/methoddocs/source.md
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/methoddocs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.986696 ethpm-types-0.6.8/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/userguides/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.990696 ethpm-types-0.6.8/ethpm_types/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/ethpm_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11035 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/ethpm_types/abi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/ethpm_types/ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/ethpm_types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16573 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/ethpm_types/contract_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    12491 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/ethpm_types/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/ethpm_types/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    26564 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/ethpm_types/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/ethpm_types/sourcemap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/ethpm_types/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-02 15:32:13.000000 ethpm-types-0.6.8/ethpm_types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.990696 ethpm-types-0.6.8/ethpm_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-02 15:32:13.000000 ethpm-types-0.6.8/ethpm_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-02 15:32:13.000000 ethpm-types-0.6.8/ethpm_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:32:13.000000 ethpm-types-0.6.8/ethpm_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:32:13.000000 ethpm-types-0.6.8/ethpm_types.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-02 15:32:13.000000 ethpm-types-0.6.8/ethpm_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 15:32:13.000000 ethpm-types-0.6.8/ethpm_types.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-02 15:32:14.010696 ethpm-types-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.990696 ethpm-types-0.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.982696 ethpm-types-0.6.8/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:14.006696 ethpm-types-0.6.8/tests/data/Compiled/
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Compiled/HasError.json
--rw-r--r--   0 runner    (1001) docker     (127) 12327472 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Compiled/OpenZeppelinContracts.json
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Compiled/SolFallbackAndReceive.json
--rw-r--r--   0 runner    (1001) docker     (127)   227889 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Compiled/SolidityContract.json
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Compiled/TestStrategy.srcmap
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Compiled/VyDefault.json
--rw-r--r--   0 runner    (1001) docker     (127)   230644 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Compiled/VyperContract.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:14.010696 ethpm-types-0.6.8/tests/data/Sources/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Sources/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Sources/SolFallbackAndReceive.sol
--rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Sources/SolidityContract.sol
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Sources/VyDefault.vy
--rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Sources/VyperContract.vy
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/test_cairo.py
--rw-r--r--   0 runner    (1001) docker     (127)    13640 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/test_contract_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/test_package_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/test_pc_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/test_schema_fuzzing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10539 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/test_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/test_sourcemap.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:17:06.836190 ethpm-types-0.6.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:17:06.812190 ethpm-types-0.6.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:17:06.812190 ethpm-types-0.6.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:17:06.812190 ethpm-types-0.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-09 17:17:06.836190 ethpm-types-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/build_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/cz-requirement.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:17:06.812190 ethpm-types-0.6.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:17:06.812190 ethpm-types-0.6.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:17:06.812190 ethpm-types-0.6.9/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:17:06.812190 ethpm-types-0.6.9/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/docs/methoddocs/abi.md
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/docs/methoddocs/contract_type.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/docs/methoddocs/manifest.md
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/docs/methoddocs/source.md
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/docs/methoddocs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:17:06.812190 ethpm-types-0.6.9/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/docs/userguides/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:17:06.816190 ethpm-types-0.6.9/ethpm_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/ethpm_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11035 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/ethpm_types/abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/ethpm_types/ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/ethpm_types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16573 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/ethpm_types/contract_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12491 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/ethpm_types/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/ethpm_types/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    26564 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/ethpm_types/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/ethpm_types/sourcemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/ethpm_types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 17:17:06.000000 ethpm-types-0.6.9/ethpm_types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:17:06.816190 ethpm-types-0.6.9/ethpm_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-09 17:17:06.000000 ethpm-types-0.6.9/ethpm_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-09 17:17:06.000000 ethpm-types-0.6.9/ethpm_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:17:06.000000 ethpm-types-0.6.9/ethpm_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:17:06.000000 ethpm-types-0.6.9/ethpm_types.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-09 17:17:06.000000 ethpm-types-0.6.9/ethpm_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 17:17:06.000000 ethpm-types-0.6.9/ethpm_types.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 17:17:06.836190 ethpm-types-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:17:06.816190 ethpm-types-0.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:17:06.808190 ethpm-types-0.6.9/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:17:06.832190 ethpm-types-0.6.9/tests/data/Compiled/
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/data/Compiled/HasError.json
+-rw-r--r--   0 runner    (1001) docker     (127) 12327472 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/data/Compiled/OpenZeppelinContracts.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/data/Compiled/SolFallbackAndReceive.json
+-rw-r--r--   0 runner    (1001) docker     (127)   227889 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/data/Compiled/SolidityContract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/data/Compiled/TestStrategy.srcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/data/Compiled/VyDefault.json
+-rw-r--r--   0 runner    (1001) docker     (127)   230644 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/data/Compiled/VyperContract.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:17:06.832190 ethpm-types-0.6.9/tests/data/Sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/data/Sources/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/data/Sources/SolFallbackAndReceive.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/data/Sources/SolidityContract.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/data/Sources/VyDefault.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/data/Sources/VyperContract.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/test_cairo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13640 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/test_contract_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/test_package_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/test_pc_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/test_schema_fuzzing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10539 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/test_sourcemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 17:16:44.000000 ethpm-types-0.6.9/tests/test_utils.py
```

### Comparing `ethpm-types-0.6.8/.github/ISSUE_TEMPLATE/bug.md` & `ethpm-types-0.6.9/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/.github/ISSUE_TEMPLATE/feature.md` & `ethpm-types-0.6.9/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/.github/ISSUE_TEMPLATE/work-item.md` & `ethpm-types-0.6.9/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/.github/release-drafter.yml` & `ethpm-types-0.6.9/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/.github/workflows/commitlint.yaml` & `ethpm-types-0.6.9/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/.github/workflows/docs.yaml` & `ethpm-types-0.6.9/.github/workflows/docs.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,17 @@
     pull_request:
         types: [opened, synchronize]
 
 jobs:
     docs:
         runs-on: ubuntu-latest
 
+        permissions:
+          contents: write
+
         steps:
         - uses: actions/checkout@v4
 
         - name: Setup Python
           uses: actions/setup-python@v5
           with:
               python-version: "3.10"
```

### Comparing `ethpm-types-0.6.8/.github/workflows/prtitle.yaml` & `ethpm-types-0.6.9/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/.github/workflows/publish.yaml` & `ethpm-types-0.6.9/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/.github/workflows/test.yaml` & `ethpm-types-0.6.9/.github/workflows/test.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10"]  # eventually add 3.11
+                python-version: [3.8, 3.9, "3.10", "3.11", "3.12"]
 
         steps:
         - uses: actions/checkout@v4
 
         - name: Setup Python
           uses: actions/setup-python@v5
           with:
```

### Comparing `ethpm-types-0.6.8/.gitignore` & `ethpm-types-0.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/.pre-commit-config.yaml` & `ethpm-types-0.6.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/CONTRIBUTING.md` & `ethpm-types-0.6.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/LICENSE` & `ethpm-types-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/PKG-INFO` & `ethpm-types-0.6.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethpm-types
-Version: 0.6.8
+Version: 0.6.9
 Summary: ethpm_types: Implementation of EIP-2678
 Home-page: https://github.com/ApeWorX/ethpm-types
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
@@ -30,15 +31,15 @@
 # Quick Start
 
 EthPM is an Ethereum package manifest containing data types for contracts, deployments, and source code using [EIP-2678](https://eips.ethereum.org/EIPS/eip-2678).
 The library validates and serializes contract related data and provides JSON schemas.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ethpm-types-0.6.8/README.md` & `ethpm-types-0.6.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Quick Start
 
 EthPM is an Ethereum package manifest containing data types for contracts, deployments, and source code using [EIP-2678](https://eips.ethereum.org/EIPS/eip-2678).
 The library validates and serializes contract related data and provides JSON schemas.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ethpm-types-0.6.8/build_docs.py` & `ethpm-types-0.6.9/build_docs.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/docs/_static/custom.css` & `ethpm-types-0.6.9/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/docs/_static/custom.js` & `ethpm-types-0.6.9/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/docs/_templates/layout.html` & `ethpm-types-0.6.9/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/docs/conf.py` & `ethpm-types-0.6.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/docs/favicon.ico` & `ethpm-types-0.6.9/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/docs/logo.gif` & `ethpm-types-0.6.9/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/ethpm_types/__init__.py` & `ethpm-types-0.6.9/ethpm_types/__init__.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/ethpm_types/abi.py` & `ethpm-types-0.6.9/ethpm_types/abi.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/ethpm_types/ast.py` & `ethpm-types-0.6.9/ethpm_types/ast.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/ethpm_types/base.py` & `ethpm-types-0.6.9/ethpm_types/base.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/ethpm_types/contract_type.py` & `ethpm-types-0.6.9/ethpm_types/contract_type.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/ethpm_types/manifest.py` & `ethpm-types-0.6.9/ethpm_types/manifest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/ethpm_types/source.py` & `ethpm-types-0.6.9/ethpm_types/source.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/ethpm_types/sourcemap.py` & `ethpm-types-0.6.9/ethpm_types/sourcemap.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/ethpm_types/utils.py` & `ethpm-types-0.6.9/ethpm_types/utils.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/ethpm_types.egg-info/PKG-INFO` & `ethpm-types-0.6.9/ethpm_types.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethpm-types
-Version: 0.6.8
+Version: 0.6.9
 Summary: ethpm_types: Implementation of EIP-2678
 Home-page: https://github.com/ApeWorX/ethpm-types
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
@@ -30,15 +31,15 @@
 # Quick Start
 
 EthPM is an Ethereum package manifest containing data types for contracts, deployments, and source code using [EIP-2678](https://eips.ethereum.org/EIPS/eip-2678).
 The library validates and serializes contract related data and provides JSON schemas.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ethpm-types-0.6.8/ethpm_types.egg-info/SOURCES.txt` & `ethpm-types-0.6.9/ethpm_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/ethpm_types.egg-info/requires.txt` & `ethpm-types-0.6.9/ethpm_types.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/pyproject.toml` & `ethpm-types-0.6.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310', 'py311']
+target-version = ['py38', 'py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:ape_test
     --cov-branch
     --cov-report term
```

### Comparing `ethpm-types-0.6.8/setup.py` & `ethpm-types-0.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,9 +99,10 @@
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `ethpm-types-0.6.8/tests/conftest.py` & `ethpm-types-0.6.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/tests/data/Compiled/HasError.json` & `ethpm-types-0.6.9/tests/data/Compiled/HasError.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/tests/data/Compiled/OpenZeppelinContracts.json` & `ethpm-types-0.6.9/tests/data/Compiled/OpenZeppelinContracts.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/tests/data/Compiled/SolFallbackAndReceive.json` & `ethpm-types-0.6.9/tests/data/Compiled/SolFallbackAndReceive.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/tests/data/Compiled/SolidityContract.json` & `ethpm-types-0.6.9/tests/data/Compiled/SolidityContract.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/tests/data/Compiled/TestStrategy.srcmap` & `ethpm-types-0.6.9/tests/data/Compiled/TestStrategy.srcmap`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/tests/data/Compiled/VyDefault.json` & `ethpm-types-0.6.9/tests/data/Compiled/VyDefault.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/tests/data/Compiled/VyperContract.json` & `ethpm-types-0.6.9/tests/data/Compiled/VyperContract.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/tests/data/Sources/SolidityContract.sol` & `ethpm-types-0.6.9/tests/data/Sources/SolidityContract.sol`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/tests/data/Sources/VyperContract.vy` & `ethpm-types-0.6.9/tests/data/Sources/VyperContract.vy`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/tests/test_abi.py` & `ethpm-types-0.6.9/tests/test_abi.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/tests/test_ast.py` & `ethpm-types-0.6.9/tests/test_ast.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/tests/test_cairo.py` & `ethpm-types-0.6.9/tests/test_cairo.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/tests/test_contract_type.py` & `ethpm-types-0.6.9/tests/test_contract_type.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/tests/test_package_manifest.py` & `ethpm-types-0.6.9/tests/test_package_manifest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/tests/test_pc_map.py` & `ethpm-types-0.6.9/tests/test_pc_map.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/tests/test_schema_fuzzing.py` & `ethpm-types-0.6.9/tests/test_schema_fuzzing.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/tests/test_source.py` & `ethpm-types-0.6.9/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.8/tests/test_sourcemap.py` & `ethpm-types-0.6.9/tests/test_sourcemap.py`

 * *Files identical despite different names*


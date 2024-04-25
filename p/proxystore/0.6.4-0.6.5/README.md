# Comparing `tmp/proxystore-0.6.4.tar.gz` & `tmp/proxystore-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxystore-0.6.4.tar", last modified: Mon Apr  8 15:58:54 2024, max compression
+gzip compressed data, was "proxystore-0.6.5.tar", last modified: Thu Apr 25 14:22:07 2024, max compression
```

## Comparing `proxystore-0.6.4.tar` & `proxystore-0.6.5.tar`

### file list

```diff
@@ -1,301 +1,315 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.514128 proxystore-0.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.470128 proxystore-0.6.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.470128 proxystore-0.6.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/ISSUE_TEMPLATE/01_bug.yml
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/ISSUE_TEMPLATE/02_feature.yml
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/ISSUE_TEMPLATE/03_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.470128 proxystore-0.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/workflows/cache.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/workflows/check-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-08 15:58:48.000000 proxystore-0.6.4/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-08 15:58:48.000000 proxystore-0.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-08 15:58:48.000000 proxystore-0.6.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-08 15:58:48.000000 proxystore-0.6.4/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-08 15:58:48.000000 proxystore-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-04-08 15:58:54.514128 proxystore-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-04-08 15:58:48.000000 proxystore-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.470128 proxystore-0.6.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.470128 proxystore-0.6.4/docs/_overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/_overrides/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.462128 proxystore-0.6.4/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.462128 proxystore-0.6.4/docs/_templates/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.474128 proxystore-0.6.4/docs/_templates/python/material/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.474128 proxystore-0.6.4/docs/_templates/python/material/docstring/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/_templates/python/material/docstring/admonition.html
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/_templates/python/material/function.html
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/_templates/python/material/module.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.474128 proxystore-0.6.4/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/api/cli.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.474128 proxystore-0.6.4/docs/concepts/
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/concepts/connector.md
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/concepts/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/concepts/proxy.md
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/concepts/store.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.474128 proxystore-0.6.4/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/contributing/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/contributing/issues-pull-requests.md
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/contributing/releases.md
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/contributing/style-guide.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.474128 proxystore-0.6.4/docs/css/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/css/mkdocstrings.css
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/generate_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/get-started.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.474128 proxystore-0.6.4/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/guides/endpoints-debugging.md
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/guides/endpoints.md
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/guides/globus-compute.md
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/guides/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/guides/object-lifetimes.md
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/guides/performance.md
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/guides/proxy-futures.md
--rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/guides/relay-serving.md
--rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/guides/streaming.md
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/known-issues.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.474128 proxystore-0.6.4/docs/publications/
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/publications/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.478128 proxystore-0.6.4/docs/static/
--rw-r--r--   0 runner    (1001) docker     (127)   134472 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/static/endpoint-overview.svg
--rw-r--r--   0 runner    (1001) docker     (127)   149176 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/static/endpoint-peering.svg
--rw-r--r--   0 runner    (1001) docker     (127)    46990 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)    45464 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/static/icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    31401 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/static/logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    31236 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/static/logo-light.png
--rw-r--r--   0 runner    (1001) docker     (127)   106893 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/static/proxystore-overview.svg
--rw-r--r--   0 runner    (1001) docker     (127)   106939 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/static/proxystore-schematic.svg
--rw-r--r--   0 runner    (1001) docker     (127)   176467 2024-04-08 15:58:48.000000 proxystore-0.6.4/docs/static/proxystore-streaming.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.478128 proxystore-0.6.4/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 15:58:48.000000 proxystore-0.6.4/examples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 15:58:48.000000 proxystore-0.6.4/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.478128 proxystore-0.6.4/examples/globus-compute/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 15:58:48.000000 proxystore-0.6.4/examples/globus-compute/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-08 15:58:48.000000 proxystore-0.6.4/examples/globus-compute/mapreduce_globus_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-08 15:58:48.000000 proxystore-0.6.4/examples/globus-compute/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.478128 proxystore-0.6.4/examples/parsl/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 15:58:48.000000 proxystore-0.6.4/examples/parsl/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-08 15:58:48.000000 proxystore-0.6.4/examples/parsl/mapreduce_parsl.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-08 15:58:48.000000 proxystore-0.6.4/examples/parsl/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-08 15:58:48.000000 proxystore-0.6.4/examples/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-08 15:58:48.000000 proxystore-0.6.4/examples/store_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-08 15:58:48.000000 proxystore-0.6.4/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.482128 proxystore-0.6.4/proxystore/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.482128 proxystore-0.6.4/proxystore/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/connectors/dim.py
--rw-r--r--   0 runner    (1001) docker     (127)    11150 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/connectors/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/connectors/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    23452 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/connectors/globus.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/connectors/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    15939 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/connectors/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/connectors/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/connectors/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.486127 proxystore-0.6.4/proxystore/endpoint/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8875 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13921 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    18441 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)    14893 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/endpoint/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/ex.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.486127 proxystore-0.6.4/proxystore/globus/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/globus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/globus/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/globus/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/globus/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/globus/scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/globus/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/globus/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.486127 proxystore-0.6.4/proxystore/p2p/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/chunks.py
--rw-r--r--   0 runner    (1001) docker     (127)    15261 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/nat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.490128 proxystore-0.6.4/proxystore/p2p/relay/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/relay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/relay/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)    13466 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/relay/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/relay/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/relay/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/relay/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/relay/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/relay/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    13593 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/p2p/relay/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.490128 proxystore-0.6.4/proxystore/store/
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43757 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/future.py
--rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/lifetimes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    19018 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.490128 proxystore-0.6.4/proxystore/stream/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    24393 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.494128 proxystore-0.6.4/proxystore/stream/shims/
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/shims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/shims/kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/shims/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/shims/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/stream/shims/zmq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.494128 proxystore-0.6.4/proxystore/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/utils/counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/utils/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/utils/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-08 15:58:48.000000 proxystore-0.6.4/proxystore/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.510128 proxystore-0.6.4/proxystore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-04-08 15:58:54.000000 proxystore-0.6.4/proxystore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-08 15:58:54.000000 proxystore-0.6.4/proxystore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:58:54.000000 proxystore-0.6.4/proxystore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-08 15:58:54.000000 proxystore-0.6.4/proxystore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-08 15:58:54.000000 proxystore-0.6.4/proxystore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 15:58:54.000000 proxystore-0.6.4/proxystore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-04-08 15:58:48.000000 proxystore-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 15:58:54.514128 proxystore-0.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.494128 proxystore-0.6.4/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/connectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.498128 proxystore-0.6.4/testing/mocked/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/mocked/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/mocked/globus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/mocked/kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/mocked/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/mocking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/relay_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.498128 proxystore-0.6.4/testing/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/scripts/kafka_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/scripts/peer_connection_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/scripts/peer_endpoint_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/scripts/peer_manager_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/scripts/redis_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/stores.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-08 15:58:48.000000 proxystore-0.6.4/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.498128 proxystore-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.502128 proxystore-0.6.4/tests/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/connectors/connector_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/connectors/dim_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/connectors/endpoint_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/connectors/file_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8834 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/connectors/globus_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/connectors/local_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/connectors/multi_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/connectors/redis_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.502128 proxystore-0.6.4/tests/endpoint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/endpoint/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/endpoint/client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    15221 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/endpoint/commands_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/endpoint/config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/endpoint/endpoint_peering_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/endpoint/endpoint_solo_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/endpoint/serve_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/endpoint/storage_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/ex_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/factory_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.502128 proxystore-0.6.4/tests/globus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/globus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/globus/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/globus/client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/globus/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/globus/manager_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/globus/scopes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/globus/storage_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/globus/transfer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.502128 proxystore-0.6.4/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/integration/endpoints_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.502128 proxystore-0.6.4/tests/p2p/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/chunks_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/manager_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/nat_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.506127 proxystore-0.6.4/tests/p2p/relay/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/relay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/relay/authenticate_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/relay/client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/relay/config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/relay/manager_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/relay/messages_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/relay/run_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/p2p/relay/server_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/proxy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/serialization_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.506127 proxystore-0.6.4/tests/store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/cache_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/factory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/init_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/lifetimes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/ref_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/scopes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/store_basics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/store_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/store_proxy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/store/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.506127 proxystore-0.6.4/tests/stream/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/stream/events_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/stream/filters_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10108 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/stream/interface_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.510128 proxystore-0.6.4/tests/stream/shims/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/stream/shims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/stream/shims/kafka_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/stream/shims/queue_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/stream/shims/redis_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/stream/shims/zmq_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:54.510128 proxystore-0.6.4/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/utils/config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/utils/counter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/utils/data_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/utils/environment_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/utils/imports_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/utils/tasks_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-08 15:58:48.000000 proxystore-0.6.4/tests/utils/timer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-08 15:58:48.000000 proxystore-0.6.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.510959 proxystore-0.6.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.466958 proxystore-0.6.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-25 14:22:03.000000 proxystore-0.6.5/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-25 14:22:03.000000 proxystore-0.6.5/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.466958 proxystore-0.6.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-25 14:22:03.000000 proxystore-0.6.5/.github/ISSUE_TEMPLATE/01_bug.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-25 14:22:03.000000 proxystore-0.6.5/.github/ISSUE_TEMPLATE/02_feature.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-25 14:22:03.000000 proxystore-0.6.5/.github/ISSUE_TEMPLATE/03_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-25 14:22:03.000000 proxystore-0.6.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-25 14:22:03.000000 proxystore-0.6.5/.github/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-25 14:22:03.000000 proxystore-0.6.5/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-25 14:22:03.000000 proxystore-0.6.5/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-25 14:22:03.000000 proxystore-0.6.5/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.470959 proxystore-0.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-25 14:22:03.000000 proxystore-0.6.5/.github/workflows/cache.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-25 14:22:03.000000 proxystore-0.6.5/.github/workflows/check-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-25 14:22:03.000000 proxystore-0.6.5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-25 14:22:03.000000 proxystore-0.6.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-25 14:22:03.000000 proxystore-0.6.5/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-25 14:22:03.000000 proxystore-0.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-25 14:22:03.000000 proxystore-0.6.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-25 14:22:03.000000 proxystore-0.6.5/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-25 14:22:03.000000 proxystore-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8875 2024-04-25 14:22:07.510959 proxystore-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-25 14:22:03.000000 proxystore-0.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-25 14:22:03.000000 proxystore-0.6.5/THIRD_PARTY_LICENSES
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.470959 proxystore-0.6.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.470959 proxystore-0.6.5/docs/_overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/_overrides/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.462958 proxystore-0.6.5/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.462958 proxystore-0.6.5/docs/_templates/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.470959 proxystore-0.6.5/docs/_templates/python/material/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.470959 proxystore-0.6.5/docs/_templates/python/material/docstring/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/_templates/python/material/docstring/admonition.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/_templates/python/material/function.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/_templates/python/material/module.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.470959 proxystore-0.6.5/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/api/cli.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.470959 proxystore-0.6.5/docs/concepts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/concepts/connector.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/concepts/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/concepts/proxy.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/concepts/store.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.470959 proxystore-0.6.5/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/contributing/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/contributing/issues-pull-requests.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/contributing/releases.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/contributing/style-guide.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.470959 proxystore-0.6.5/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/generate_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/get-started.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.474959 proxystore-0.6.5/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/guides/dask-distributed.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/guides/endpoints-debugging.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/guides/endpoints.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/guides/globus-compute.md
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/guides/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11663 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/guides/object-lifetimes.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/guides/performance.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/guides/proxy-futures.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/guides/relay-serving.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/guides/streaming.md
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.474959 proxystore-0.6.5/docs/publications/
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/publications/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.474959 proxystore-0.6.5/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   134472 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/static/endpoint-overview.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   149176 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/static/endpoint-peering.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    46990 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45464 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/static/icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31401 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/static/logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31236 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/static/logo-light.png
+-rw-r--r--   0 runner    (1001) docker     (127)   106893 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/static/proxystore-overview.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   106939 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/static/proxystore-schematic.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   176467 2024-04-25 14:22:03.000000 proxystore-0.6.5/docs/static/proxystore-streaming.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.478959 proxystore-0.6.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-25 14:22:03.000000 proxystore-0.6.5/examples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-25 14:22:03.000000 proxystore-0.6.5/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.478959 proxystore-0.6.5/examples/globus-compute/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-25 14:22:03.000000 proxystore-0.6.5/examples/globus-compute/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-25 14:22:03.000000 proxystore-0.6.5/examples/globus-compute/mapreduce_globus_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-25 14:22:03.000000 proxystore-0.6.5/examples/globus-compute/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.478959 proxystore-0.6.5/examples/parsl/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-25 14:22:03.000000 proxystore-0.6.5/examples/parsl/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-25 14:22:03.000000 proxystore-0.6.5/examples/parsl/mapreduce_parsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-25 14:22:03.000000 proxystore-0.6.5/examples/parsl/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-25 14:22:03.000000 proxystore-0.6.5/examples/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-25 14:22:03.000000 proxystore-0.6.5/examples/store_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-04-25 14:22:03.000000 proxystore-0.6.5/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.478959 proxystore-0.6.5/proxystore/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.482959 proxystore-0.6.5/proxystore/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/connectors/dim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11150 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/connectors/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/connectors/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23452 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/connectors/globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/connectors/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15939 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/connectors/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/connectors/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/connectors/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.482959 proxystore-0.6.5/proxystore/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8875 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/endpoint/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/endpoint/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13921 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/endpoint/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7610 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/endpoint/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/endpoint/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18441 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/endpoint/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/endpoint/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/endpoint/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14893 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/endpoint/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/endpoint/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.482959 proxystore-0.6.5/proxystore/globus/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/globus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/globus/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/globus/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/globus/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/globus/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/globus/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/globus/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/mypy_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.482959 proxystore-0.6.5/proxystore/p2p/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/p2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/p2p/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15261 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/p2p/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/p2p/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/p2p/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/p2p/nat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.486959 proxystore-0.6.5/proxystore/p2p/relay/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/p2p/relay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/p2p/relay/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13466 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/p2p/relay/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/p2p/relay/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/p2p/relay/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/p2p/relay/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/p2p/relay/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/p2p/relay/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13593 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/p2p/relay/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.486959 proxystore-0.6.5/proxystore/proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)    25479 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/proxy/_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/proxy/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.486959 proxystore-0.6.5/proxystore/store/
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47184 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/store/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/store/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/store/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/store/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/store/future.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18940 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/store/lifetimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/store/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22475 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/store/ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/store/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/store/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.490959 proxystore-0.6.5/proxystore/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/stream/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/stream/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/stream/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24437 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/stream/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/stream/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.490959 proxystore-0.6.5/proxystore/stream/shims/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/stream/shims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/stream/shims/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/stream/shims/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/stream/shims/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/stream/shims/zmq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.490959 proxystore-0.6.5/proxystore/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/utils/counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/utils/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/utils/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-25 14:22:03.000000 proxystore-0.6.5/proxystore/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.506959 proxystore-0.6.5/proxystore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8875 2024-04-25 14:22:07.000000 proxystore-0.6.5/proxystore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-25 14:22:07.000000 proxystore-0.6.5/proxystore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:22:07.000000 proxystore-0.6.5/proxystore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-25 14:22:07.000000 proxystore-0.6.5/proxystore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-25 14:22:07.000000 proxystore-0.6.5/proxystore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 14:22:07.000000 proxystore-0.6.5/proxystore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-04-25 14:22:03.000000 proxystore-0.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 14:22:07.510959 proxystore-0.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.490959 proxystore-0.6.5/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-25 14:22:03.000000 proxystore-0.6.5/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-25 14:22:03.000000 proxystore-0.6.5/testing/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-25 14:22:03.000000 proxystore-0.6.5/testing/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-25 14:22:03.000000 proxystore-0.6.5/testing/endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.494959 proxystore-0.6.5/testing/mocked/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-25 14:22:03.000000 proxystore-0.6.5/testing/mocked/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-25 14:22:03.000000 proxystore-0.6.5/testing/mocked/globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-25 14:22:03.000000 proxystore-0.6.5/testing/mocked/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-25 14:22:03.000000 proxystore-0.6.5/testing/mocked/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-25 14:22:03.000000 proxystore-0.6.5/testing/mocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-25 14:22:03.000000 proxystore-0.6.5/testing/relay_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.494959 proxystore-0.6.5/testing/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-25 14:22:03.000000 proxystore-0.6.5/testing/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-25 14:22:03.000000 proxystore-0.6.5/testing/scripts/kafka_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-25 14:22:03.000000 proxystore-0.6.5/testing/scripts/peer_connection_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-25 14:22:03.000000 proxystore-0.6.5/testing/scripts/peer_endpoint_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-25 14:22:03.000000 proxystore-0.6.5/testing/scripts/peer_manager_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-25 14:22:03.000000 proxystore-0.6.5/testing/scripts/redis_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-25 14:22:03.000000 proxystore-0.6.5/testing/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-25 14:22:03.000000 proxystore-0.6.5/testing/stores.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-25 14:22:03.000000 proxystore-0.6.5/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.494959 proxystore-0.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.494959 proxystore-0.6.5/tests/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/connectors/connector_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/connectors/dim_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/connectors/endpoint_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/connectors/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8834 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/connectors/globus_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/connectors/local_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/connectors/multi_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/connectors/redis_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.498959 proxystore-0.6.5/tests/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/endpoint/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/endpoint/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15221 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/endpoint/commands_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/endpoint/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/endpoint/endpoint_peering_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/endpoint/endpoint_solo_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/endpoint/serve_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/endpoint/storage_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/ex_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/factory_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.498959 proxystore-0.6.5/tests/globus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/globus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/globus/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/globus/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/globus/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/globus/manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/globus/scopes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/globus/storage_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/globus/transfer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.498959 proxystore-0.6.5/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/integration/endpoints_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/mypy_plugin_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.498959 proxystore-0.6.5/tests/p2p/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/p2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/p2p/chunks_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/p2p/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/p2p/manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/p2p/nat_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.498959 proxystore-0.6.5/tests/p2p/relay/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/p2p/relay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/p2p/relay/authenticate_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/p2p/relay/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/p2p/relay/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/p2p/relay/manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/p2p/relay/messages_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/p2p/relay/run_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/p2p/relay/server_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.502959 proxystore-0.6.5/tests/proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/proxy/property_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/proxy/proxy_async_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/proxy/proxy_container_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/proxy/proxy_numeric_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24269 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/proxy/proxy_type_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/proxy/proxy_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/serialize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.502959 proxystore-0.6.5/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/store/cache_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/store/factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/store/init_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/store/lifetimes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/store/metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/store/ref_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/store/scopes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/store/store_basics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/store/store_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/store/store_proxy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/store/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.502959 proxystore-0.6.5/tests/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/stream/events_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/stream/filters_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10108 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/stream/interface_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.502959 proxystore-0.6.5/tests/stream/shims/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/stream/shims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/stream/shims/kafka_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/stream/shims/queue_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/stream/shims/redis_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/stream/shims/zmq_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:07.506959 proxystore-0.6.5/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/utils/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/utils/counter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/utils/data_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/utils/environment_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/utils/imports_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/utils/tasks_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-25 14:22:03.000000 proxystore-0.6.5/tests/utils/timer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-25 14:22:03.000000 proxystore-0.6.5/tox.ini
```

### Comparing `proxystore-0.6.4/.github/CODE_OF_CONDUCT.md` & `proxystore-0.6.5/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/.github/ISSUE_TEMPLATE/01_bug.yml` & `proxystore-0.6.5/.github/ISSUE_TEMPLATE/01_bug.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/.github/ISSUE_TEMPLATE/02_feature.yml` & `proxystore-0.6.5/.github/ISSUE_TEMPLATE/02_feature.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/.github/SECURITY.md` & `proxystore-0.6.5/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/.github/pull_request_template.md` & `proxystore-0.6.5/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/.github/release.yml` & `proxystore-0.6.5/.github/release.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/.github/workflows/cache.yml` & `proxystore-0.6.5/.github/workflows/cache.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/.github/workflows/check-docs.yml` & `proxystore-0.6.5/.github/workflows/check-docs.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/.github/workflows/docs.yml` & `proxystore-0.6.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/.github/workflows/publish.yml` & `proxystore-0.6.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/.github/workflows/tests.yml` & `proxystore-0.6.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/.gitignore` & `proxystore-0.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/LICENSE` & `proxystore-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/PKG-INFO` & `proxystore-0.6.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: proxystore
-Version: 0.6.4
+Version: 0.6.5
 Summary: Lazy object proxy interface for distributed stores.
 Author: Globus Labs
 Author-email: Greg Pauloski <jgpauloski@uchicago.edu>
 Maintainer-email: Greg Pauloski <jgpauloski@uchicago.edu>, Valerie Hayot-Sasson <vhayot@uchicago.edu>
-License: FILE
-Project-URL: homepage, https://proxystore.dev
-Project-URL: documentation, https://docs.proxystore.dev
-Project-URL: repository, https://github.com/proxystore/proxystore
+License: MIT
+Project-URL: Homepage, https://proxystore.dev
+Project-URL: Documentation, https://docs.proxystore.dev
+Project-URL: Source, https://github.com/proxystore/proxystore
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -20,15 +20,14 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click!=8.1.4
 Requires-Dist: cloudpickle>=1.6.0
 Requires-Dist: cryptography>=39.0.1
 Requires-Dist: globus-sdk>=3.3.0
-Requires-Dist: lazy-object-proxy>=1.6.0
 Requires-Dist: typing-extensions>=4.3.0
 Provides-Extra: all
 Requires-Dist: proxystore[endpoints,extensions,kafka,redis,zmq]; extra == "all"
 Provides-Extra: endpoints
 Requires-Dist: aiortc>=1.3.2; extra == "endpoints"
 Requires-Dist: aiosqlite; extra == "endpoints"
 Requires-Dist: uvicorn[standard]; extra == "endpoints"
@@ -56,14 +55,15 @@
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio>=0.23.2; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-timeout; extra == "dev"
 Requires-Dist: ruff>=0.2.0; extra == "dev"
 Requires-Dist: tox; extra == "dev"
+Requires-Dist: types-psutil; extra == "dev"
 Requires-Dist: types-redis; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: virtualenv; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: black; extra == "docs"
 Requires-Dist: mkdocs-click; extra == "docs"
 Requires-Dist: mkdocs-gen-files; extra == "docs"
@@ -76,31 +76,32 @@
 Requires-Dist: proxystore[all]; extra == "docs"
 
 # ProxyStore
 
 ![PyPI - Version](https://img.shields.io/pypi/v/proxystore)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/proxystore)
 ![GitHub License](https://img.shields.io/github/license/proxystore/proxystore)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8077899.svg)](https://doi.org/10.5281/zenodo.8077899)
 
 [![docs](https://github.com/proxystore/proxystore/actions/workflows/docs.yml/badge.svg)](https://github.com/proxystore/proxystore/actions/workflows/docs.yml)
 [![tests](https://github.com/proxystore/proxystore/actions/workflows/tests.yml/badge.svg?label=tests)](https://github.com/proxystore/proxystore/actions)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/proxystore/proxystore/main.svg)](https://results.pre-commit.ci/latest/github/proxystore/proxystore/main)
 
 ProxyStore is a library that facilitates efficient data management in distributed Python applications.
-At the core of ProxyStore is the [*proxy*](https://docs.proxystore.dev/main/concepts/proxy/) object which acts as a transparent reference to an object living in a global object store.
+At the core of ProxyStore is the [*proxy*](https://docs.proxystore.dev/latest/concepts/proxy/) object which acts as a transparent reference to an object living in a global object store.
 This pass-by-reference interface with just-in-time object resolution works across processes, machines, and sites, and enables data producers to change the low-level communication method dynamically without altering application code or behavior.
 
 ProxyStore accelerates the development of dynamic task-based workflows, serverless applications, and more by (1) decoupling control flow from data flow, (2) abstracting low-level communication mechanisms, and (3) eliminating the need for shims, wrapper functions, and boilerplate code.
 
 ProxyStore supports a diverse set of programming paradigms:
 
 * [Task-based Workflows](https://arxiv.org/abs/2303.08803)
-* [Function-as-a-Service/Serverless Applications](https://docs.proxystore.dev/main/guides/globus-compute/)
-* [Distributed Futures](https://docs.proxystore.dev/main/guides/proxy-futures/)
-* [Bulk Data Streaming](https://docs.proxystore.dev/main/guides/streaming/)
+* [Function-as-a-Service/Serverless Applications](https://docs.proxystore.dev/latest/guides/globus-compute/)
+* [Distributed Futures](https://docs.proxystore.dev/latest/guides/proxy-futures/)
+* [Bulk Data Streaming](https://docs.proxystore.dev/latest/guides/streaming/)
 * and more!
 
 ProxyStore provides support for many third-party mediated communication methods
 out-of-the-box including
 [DAOS](https://docs.daos.io/v2.4/),
 [Globus Transfer](https://www.globus.org/data-transfer),
 [Kafka](https://kafka.apache.org/),
@@ -109,15 +110,15 @@
 Custom communication methods built on
 [Mochi](https://mochi.readthedocs.io/en/latest/margo.html),
 [UCX](https://openucx.org/),
 [WebRTC](https://webrtc.org/), and
 [ZeroMQ](https://zeromq.org/)
 are provided for high-performance and peer-to-peer applications.
 
-Read more about ProxyStore's concepts [here](https://docs.proxystore.dev/main/concepts/).
+Read more about ProxyStore's concepts [here](https://docs.proxystore.dev/latest/concepts/).
 Complete documentation for ProxyStore is available at
 [docs.proxystore.dev](https://docs.proxystore.dev).
 
 ## Installation
 
 The base ProxyStore package can be installed with [`pip`](https://pip.pypa.io/en/stable/).
 ```bash
@@ -131,17 +132,17 @@
 pip install proxystore[all]
 ```
 This will also install the [`proxystore-ex`](https://extensions.proxystore.dev/)
 package which contains extension and experimental features.
 The extensions package can also be installed with `pip` using
 `proxystore[extensions]` or `proxystore-ex`.
 
-See the [Installation](https://docs.proxystore.dev/main/installation) guide
+See the [Installation](https://docs.proxystore.dev/latest/installation) guide
 for more information about the available extras installation options.
-See the [Contributing](https://docs.proxystore.dev/main/contributing) guide
+See the [Contributing](https://docs.proxystore.dev/latest/contributing) guide
 to get started for local development.
 
 ## Example
 
 Getting started with ProxyStore requires a few lines of code.
 
 ```python
@@ -162,20 +163,20 @@
     # x is resolved my-store on first use transparently to the
     # function. Then x behaves as an instance of MyDataType.
     assert isinstance(x, MyDataType)
 
 my_function(proxy)  # Succeeds
 ```
 
-Check out the [Get Started](https://docs.proxystore.dev/main/get-started)
+Check out the [Get Started](https://docs.proxystore.dev/latest/get-started)
 guide to learn more!
 
 ## Citation
 
-[![DOI](https://zenodo.org/badge/357984234.svg)](https://zenodo.org/badge/latestdoi/357984234)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8077899.svg)](https://doi.org/10.5281/zenodo.8077899)
 
 If you use ProxyStore or any of this code in your work, please cite our [SC '23 paper](https://dl.acm.org/doi/10.1145/3581784.3607047).
 ```bibtex
 @inproceedings{pauloski2023proxystore,
     author = {Pauloski, J. Gregory and Hayot-Sasson, Valerie and Ward, Logan and Hudson, Nathaniel and Sabino, Charlie and Baughman, Matt and Chard, Kyle and Foster, Ian},
     title = {{Accelerating Communications in Federated Applications with Transparent Object Proxies}},
     address = {New York, NY, USA},
```

### Comparing `proxystore-0.6.4/README.md` & `proxystore-0.6.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # ProxyStore
 
 ![PyPI - Version](https://img.shields.io/pypi/v/proxystore)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/proxystore)
 ![GitHub License](https://img.shields.io/github/license/proxystore/proxystore)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8077899.svg)](https://doi.org/10.5281/zenodo.8077899)
 
 [![docs](https://github.com/proxystore/proxystore/actions/workflows/docs.yml/badge.svg)](https://github.com/proxystore/proxystore/actions/workflows/docs.yml)
 [![tests](https://github.com/proxystore/proxystore/actions/workflows/tests.yml/badge.svg?label=tests)](https://github.com/proxystore/proxystore/actions)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/proxystore/proxystore/main.svg)](https://results.pre-commit.ci/latest/github/proxystore/proxystore/main)
 
 ProxyStore is a library that facilitates efficient data management in distributed Python applications.
-At the core of ProxyStore is the [*proxy*](https://docs.proxystore.dev/main/concepts/proxy/) object which acts as a transparent reference to an object living in a global object store.
+At the core of ProxyStore is the [*proxy*](https://docs.proxystore.dev/latest/concepts/proxy/) object which acts as a transparent reference to an object living in a global object store.
 This pass-by-reference interface with just-in-time object resolution works across processes, machines, and sites, and enables data producers to change the low-level communication method dynamically without altering application code or behavior.
 
 ProxyStore accelerates the development of dynamic task-based workflows, serverless applications, and more by (1) decoupling control flow from data flow, (2) abstracting low-level communication mechanisms, and (3) eliminating the need for shims, wrapper functions, and boilerplate code.
 
 ProxyStore supports a diverse set of programming paradigms:
 
 * [Task-based Workflows](https://arxiv.org/abs/2303.08803)
-* [Function-as-a-Service/Serverless Applications](https://docs.proxystore.dev/main/guides/globus-compute/)
-* [Distributed Futures](https://docs.proxystore.dev/main/guides/proxy-futures/)
-* [Bulk Data Streaming](https://docs.proxystore.dev/main/guides/streaming/)
+* [Function-as-a-Service/Serverless Applications](https://docs.proxystore.dev/latest/guides/globus-compute/)
+* [Distributed Futures](https://docs.proxystore.dev/latest/guides/proxy-futures/)
+* [Bulk Data Streaming](https://docs.proxystore.dev/latest/guides/streaming/)
 * and more!
 
 ProxyStore provides support for many third-party mediated communication methods
 out-of-the-box including
 [DAOS](https://docs.daos.io/v2.4/),
 [Globus Transfer](https://www.globus.org/data-transfer),
 [Kafka](https://kafka.apache.org/),
@@ -32,15 +33,15 @@
 Custom communication methods built on
 [Mochi](https://mochi.readthedocs.io/en/latest/margo.html),
 [UCX](https://openucx.org/),
 [WebRTC](https://webrtc.org/), and
 [ZeroMQ](https://zeromq.org/)
 are provided for high-performance and peer-to-peer applications.
 
-Read more about ProxyStore's concepts [here](https://docs.proxystore.dev/main/concepts/).
+Read more about ProxyStore's concepts [here](https://docs.proxystore.dev/latest/concepts/).
 Complete documentation for ProxyStore is available at
 [docs.proxystore.dev](https://docs.proxystore.dev).
 
 ## Installation
 
 The base ProxyStore package can be installed with [`pip`](https://pip.pypa.io/en/stable/).
 ```bash
@@ -54,17 +55,17 @@
 pip install proxystore[all]
 ```
 This will also install the [`proxystore-ex`](https://extensions.proxystore.dev/)
 package which contains extension and experimental features.
 The extensions package can also be installed with `pip` using
 `proxystore[extensions]` or `proxystore-ex`.
 
-See the [Installation](https://docs.proxystore.dev/main/installation) guide
+See the [Installation](https://docs.proxystore.dev/latest/installation) guide
 for more information about the available extras installation options.
-See the [Contributing](https://docs.proxystore.dev/main/contributing) guide
+See the [Contributing](https://docs.proxystore.dev/latest/contributing) guide
 to get started for local development.
 
 ## Example
 
 Getting started with ProxyStore requires a few lines of code.
 
 ```python
@@ -85,20 +86,20 @@
     # x is resolved my-store on first use transparently to the
     # function. Then x behaves as an instance of MyDataType.
     assert isinstance(x, MyDataType)
 
 my_function(proxy)  # Succeeds
 ```
 
-Check out the [Get Started](https://docs.proxystore.dev/main/get-started)
+Check out the [Get Started](https://docs.proxystore.dev/latest/get-started)
 guide to learn more!
 
 ## Citation
 
-[![DOI](https://zenodo.org/badge/357984234.svg)](https://zenodo.org/badge/latestdoi/357984234)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8077899.svg)](https://doi.org/10.5281/zenodo.8077899)
 
 If you use ProxyStore or any of this code in your work, please cite our [SC '23 paper](https://dl.acm.org/doi/10.1145/3581784.3607047).
 ```bibtex
 @inproceedings{pauloski2023proxystore,
     author = {Pauloski, J. Gregory and Hayot-Sasson, Valerie and Ward, Logan and Hudson, Nathaniel and Sabino, Charlie and Baughman, Matt and Chard, Kyle and Foster, Ian},
     title = {{Accelerating Communications in Federated Applications with Transparent Object Proxies}},
     address = {New York, NY, USA},
```

### Comparing `proxystore-0.6.4/docs/_templates/python/material/function.html` & `proxystore-0.6.5/docs/_templates/python/material/function.html`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/_templates/python/material/module.html` & `proxystore-0.6.5/docs/_templates/python/material/module.html`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/api/cli.md` & `proxystore-0.6.5/docs/api/cli.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/concepts/connector.md` & `proxystore-0.6.5/docs/concepts/connector.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/concepts/index.md` & `proxystore-0.6.5/docs/concepts/index.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/concepts/proxy.md` & `proxystore-0.6.5/docs/concepts/proxy.md`

 * *Files 4% similar despite different names*

```diff
@@ -81,21 +81,24 @@
 ## Interacting with Proxies
 
 While a proxy can be used just as one would normally use the proxy's target
 object, additional functions are provided for interacting with the proxy
 directly.
 
 ```python
-from proxystore import proxy
+from proxystore.proxy import Proxy
+from proxystore.proxy import extract
+from proxystore.proxy import is_resolved
+from proxystore.proxy import resolve
 
-p = proxy.Proxy(...)
+p = Proxy(...)
 
 # Check if a proxy has been resolved yet
-proxy.is_resolved(p)
+is_resolved(p)
 
 # Force a proxy to resolve itself
-proxy.resolve(p)
+resolve(p)
 
 # Extract the wrapped object from the proxy
-x = proxy.extract(p)
-assert not isinstance(x, proxy.Proxy)
+x = extract(p)
+assert not isinstance(x, Proxy)
 ```
```

### Comparing `proxystore-0.6.4/docs/concepts/store.md` & `proxystore-0.6.5/docs/concepts/store.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,34 +21,33 @@
 other information necessary to retrieve the object from the mediated channel
 is generated, and then a new proxy, internalized with the factory, is returned.
 
 ```python title="Base Store Usage" linenums="1"
 from proxystore.connectors.redis import RedisConnector
 from proxystore.proxy import Proxy
 from proxystore.store import Store
-from proxystore.store import register_store
 
 def my_function(x: MyDataType) -> ...:
     assert isinstance(x, MyDataType)  # (1)!
     # More computation...
 
-store = Store('my-store', RedisConnector(...)) # (2)!
-register_store(store)  # (3)!
+connector = RedisConnector()  # (2)!
+store = Store('my-store', connector, register=True)  # (3)!
 
 my_object = MyDataType(...) # (4)!
 p = store.proxy(my_object)
 isinstance(p, Proxy)
 
 my_function(p) # (5)!
 ```
 
 1. `x` is resolved from "my-store" on the first use of `x`.
 2. The `Connector` defines the low-level communication method used by the `Store`.
-3. Registering `store` globally enables proxies to reuse the same instance
-   to improve performance.
+3. Passing the `register=True` will call [`register_store()`][proxystore.store.register_store] automatically to register the instance globally by name.
+   This enables proxies to reuse the same store instance to improve performance.
 4. Store the object and get a proxy.
 5. Always succeeds regardless of if `p` is the true object or a proxy.
 
 ## Asynchronous Resolving
 
 It is common in distributed computation for inputs to functions executed
 remotely to not be needed immediately upon execution.
```

### Comparing `proxystore-0.6.4/docs/contributing/index.md` & `proxystore-0.6.5/docs/contributing/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 to setup the development environment. This will create a new virtual
 environment with all of the required packages installed
 and ProxyStore installed in editable mode with the necessary extras options.
 
 ```bash
 $ git clone https://github.com/proxystore/proxystore
 $ cd proxystore
-$ tox --devenv venv -e py310
+$ tox --devenv venv -e py311
 $ . venv/bin/activate
 ```
 
 !!! warning
 
     Running Tox in a Conda environment is possible but it may conflict with
     Tox's ability to find the correct Python versions. E.g., if your
-    Conda environment is Python 3.9, running `#!bash $ tox -e p38` may still use
-    Python 3.9.
+    Conda environment is Python 3.12, running `#!bash $ tox -e p311` may still
+    use Python 3.12.
 
 To install manually:
 ```bash
 $ git clone https://github.com/proxystore/proxystore
 $ cd proxystore
 $ python -m venv venv
 $ . venv/bin/activate
@@ -57,17 +57,17 @@
 the code, and tests should not be dependent on the order in which they are run.
 
 Code that is useful for building tests but is not a test itself belongs in the
 `testing/` directory.
 
 ```bash
 # Run all tests in tests/
-$ tox -e py39
+$ tox -e py311
 # Run a specific test
-$ tox -e py39 -- tests/factory_test.py::test_lambda_factory
+$ tox -e py311 -- tests/factory_test.py::test_lambda_factory
 ```
 
 Many of the tests are asyncio tests.
 The asyncio default event loop is used by default, but uvloop can be used
 instead by passing `--use-uvloop` to pytest.
 
 ## Docs
```

### Comparing `proxystore-0.6.4/docs/contributing/issues-pull-requests.md` & `proxystore-0.6.5/docs/contributing/issues-pull-requests.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
         * limit subject line to 50 characters,
         * capitalize first word of subject line,
         * do not end the subject line with a period,
         * use the imperative mood for subject lines,
         * include related issue numbers at end of subject line,
         * wrap body at 72 characters, and
         * use the body to explain what/why rather than how.
-      Example: `Fix concurrency bug in Store (#42)`
+        * *Example*: `Fix concurrency bug in Store (#42)`
+
 3. Push commits to your fork.
     - Please squash commits fixing mistakes to keep the git history clean.
       For example, if commit "b" follows commit "a" and only fixes a small typo
       from "a", please squash "a" and "b" into a single, correct commit.
       This keeps the commit history readable and easier to search through when
       debugging (e.g., git blame/bisect).
 4. Open a pull request in this repository.
```

### Comparing `proxystore-0.6.4/docs/contributing/releases.md` & `proxystore-0.6.5/docs/contributing/releases.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/contributing/style-guide.md` & `proxystore-0.6.5/docs/contributing/style-guide.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/css/extra.css` & `proxystore-0.6.5/docs/css/extra.css`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/css/mkdocstrings.css` & `proxystore-0.6.5/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/examples.md` & `proxystore-0.6.5/docs/examples.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/generate_api.py` & `proxystore-0.6.5/docs/generate_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,18 @@
     if parts[-1].endswith('__init__'):
         parts = parts[:-1]
         doc_path = doc_path.with_name('index.md')
         full_doc_path = full_doc_path.with_name('index.md')
     elif parts[-1].endswith('__main__'):
         continue
 
+    mod_name = parts[-1].split('.')[-1]
+    if mod_name.startswith('_'):
+        continue
+
     nav_parts: tuple[str, ...]
     if len(parts) == 1:
         nav_parts = parts
     elif len(parts) == 2:
         nav_parts = (parts[1],)
     else:
         nav_parts = tuple([parts[1]] + [p.split('.')[-1] for p in parts[2:]])
```

### Comparing `proxystore-0.6.4/docs/get-started.md` & `proxystore-0.6.5/docs/get-started.md`

 * *Files 6% similar despite different names*

```diff
@@ -59,31 +59,33 @@
 The following example uses the
 [`RedisConnector`][proxystore.connectors.redis.RedisConnector] to interface
 with an already running Redis server using proxies.
 
 ```python title="Basic ProxyStore Usage" linenums="1"
 from proxystore.connectors.redis import RedisConnector
 from proxystore.store import get_store
-from proxystore.store import register_store
 from proxystore.store import Store
 
-store = Store('my-store', RedisConnector(hostname='localhost', port=1234))
-register_store(store)
+store = Store(
+    'my-store',
+    RedisConnector(hostname='localhost', port=1234),
+    register=True,
+)
 
 store = get_store('my-store')  # (1)!
 
 key = store.put(my_object)  # (2)!
 assert my_object == store.get(key)
 
 p = store.proxy(my_object)  # (3)!
 
 assert isinstance(p, type(my_object))  # (4)!
 ```
 
-1. A registered store can be retrieved by name.
+1. Passing `register=True` adds the store by name to a global registry, and registered store can be retrieved by name.
 2. Stores have basic get/put functionality.
 3. Place an object in the store and return a proxy.
 4. The proxy, when used, will behave as the target.
 
 This proxy, `p`, can be cheaply serialized and communicated to any
 arbitrary Python process as if it were the target object itself. Once the
 proxy is used on the remote process, the underlying factory function will
@@ -141,8 +143,16 @@
 2. Object communication always takes place between the producer, the store, and
    the consumer meaning communication is not wasted on intermediate processes
    which have a proxy but do not use it.
 3. Different backends can be used that are optimized for specific usage
    patterns.
 4. Proxies have built-in caching for frequently used objects.
 
-See the [Concepts](concepts/index.md) to learn more!
+## Learn More
+
+See the [Concepts](concepts/index.md) to learn more about ProxyStore's core concepts.
+
+ProxyStore provides many higher level interfaces for advanced application design patterns.
+
+* [Distributed Futures](guides/proxy-futures.md)
+* [Distributed Memory Management](guides/object-lifetimes.md)
+* [Stream by Proxy](guides/streaming.md)
```

### Comparing `proxystore-0.6.4/docs/guides/endpoints-debugging.md` & `proxystore-0.6.5/docs/guides/endpoints-debugging.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/guides/endpoints.md` & `proxystore-0.6.5/docs/guides/endpoints.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/guides/globus-compute.md` & `proxystore-0.6.5/docs/guides/globus-compute.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Globus Compute with ProxyStore
 
-*Last updated 2 May 2023*
+*Last updated 20 April 2024*
 
 This guide walks through integrating ProxyStore into a
 [Globus Compute](https://www.globus.org/compute){target=_blank} application.
 A more complete example of using ProxyStore with Globus Compute can be found
 in the [`examples/`](https://github.com/proxystore/proxystore/blob/main/examples){target=_blank}.
 
 !!! note
@@ -25,15 +25,15 @@
     The below versions represent the latest versions of these packages
     available when this guide was written. These instructions should generally
     work with newer versions as well.
 
 ```bash
 $ python -m venv venv
 $ . venv/bin/activate
-$ pip install globus-compute-sdk==2.0.1 globus-compute-endpoint==2.0.1 proxystore==0.5.*
+$ pip install globus-compute-sdk==2.18.1 globus-compute-endpoint==2.18.1 proxystore==0.6.5
 ```
 
 ## Using Globus Compute
 
 We will first configure and start a Globus Compute endpoint.
 
 ```bash
@@ -84,42 +84,40 @@
    is the high-level interface provided by ProxyStore.
 2. Register the `Store` instance globally. This is not strictly necessary, but
    is an optimization which enables proxies to share the same original `Store`
    instance, because the `Store` and `Connector` can have state (e.g., caches,
    open connections, etc.).
 3. Proxy the function inputs.
 
-```python linenums="1" title="example.py" hl_lines="2 3 4 11 12 16 21"
+```python linenums="1" title="example.py" hl_lines="2 3 10 14 19"
 from globus_compute_sdk import Executor
 from proxystore.connectors.file import FileConnector
-from proxystore.store import register_store
 from proxystore.store import Store
 
 ENDPOINT_UUID = '5b994a7d-8d7c-48d1-baa1-0fda09ea1687'
 
 def average(x: list[float]) -> float:
     return sum(x) / len(x)
 
-store = Store('my-store', FileConnector('./proxystore-cache'))  # (1)!
-register_store(store) # (2)!
+store = Store('my-store', FileConnector('./proxystore-cache'), register=True)  # (1)!
 
 with Executor(endpoint_id=ENDPOINT_UUID) as gce:
     x = list(range(1, 100000))
-    p = store.proxy(x) # (3)!
+    p = store.proxy(x) # (2)!
     future = gce.submit(average, p)
 
     print(future.result())
 
-store.close() # (4)!
+store.close() # (3)!
 ```
 
 1. Create a new store using the file system for mediated communication.
-2. Register the store instance so states (e.g., caches, etc.) can be shared.
-3. Proxy the input data.
-4. Close the `Store` to cleanup any resources.
+   Register the store instance so states (e.g., caches, etc.) can be shared.
+2. Proxy the input data.
+3. Close the `Store` to cleanup any resources.
 
 !!! tip
 
     The [`Store`][proxystore.store.base.Store] can also be used as a context
     manager that will automatically clean up resources.
 
     ```python
```

### Comparing `proxystore-0.6.4/docs/guides/object-lifetimes.md` & `proxystore-0.6.5/docs/guides/object-lifetimes.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Object Lifetimes
 
-*Last updated 20 March 2024*
+*Last updated 20 April 2024*
 
 The [`Store`][proxystore.store.base.Store], by default, leaves the responsibility of managing shared objects to the application.
 For example, a object put into a [`Store`][proxystore.store.base.Store] will persist there until the key is manually evicted.
 Some [`Connectors`][proxystore.connectors.protocols.Connector], and therefore [`Stores`][proxystore.store.base.Store], delete all of their objects when closed but this is not a specified requirement of the protocol.
 
 ProxyStore, however, provides optional mechanisms for more automated management of shared objects.
 
@@ -39,14 +39,15 @@
 If you run into these errors, try:
 
 * Enabling `DEBUG` level logging to determine where unintentional proxy resolution is occurring.
   The [`Store`][proxystore.store.base.Store] will log every `GET` and `EVICT` operation on a key.
 * Avoid use of datastructures or functions which unnecessarily resolve proxies.
 * If avoiding use of the datastructures or functions causing the problem is not possible, consider using the `populate_target=True` flag when creating the proxy.
   The `populate_target` flag will return a proxy that is already resolved so the factory, which would evict the target object, does not need to be called until the proxy is serialized and then deserialized and resolved on a different process.
+  The flag will also cache the class type and hash value of the target such that the proxy can be used in datastructures which rely on [`hash()`][hash] or in [`isinstance`][isinstance] checks without needing to resolve the proxy.
 
 ## Lifetimes
 
 Shared objects in a [`Store`][proxystore.store.base.Store] can be associated with a [`Lifetime`][proxystore.store.lifetimes.Lifetime].
 Lifetimes provide a management mechanism for keeping track of objects and cleaning them up when appropriate.
 
 ### Contextual Lifetime
@@ -88,15 +89,15 @@
 
 with ContextLifetime(store) as lifetime:
     key = store.put('value', lifetime=lifetime)
     proxy = store.proxy('value', lifetime=lifetime)
 
 assert not store.exists(key)
 
-store.close()  # (5)!
+store.close()
 ```
 
 ### Leased Lifetime
 
 The [`LeaseLifetime`][proxystore.store.lifetimes.LeaseLifetime] provides time-based object lifetimes.
 Each [`LeaseLifetime`][proxystore.store.lifetimes.LeaseLifetime] has an associated expiration time after which any associated objects will be evicted.
 The lease can be extended as needed with [`extend()`][proxystore.store.lifetimes.LeaseLifetime.extend] or ended early [`close()`][proxystore.store.lifetimes.LeaseLifetime.close].
@@ -124,41 +125,43 @@
 2. Extend the lease by another five seconds.
 3. Sleep for longer than our current lease.
 4. Lease has expired so the lifetime has ended and associated objects have been evicted.
 
 ### Static Lifetime
 
 A static lifetime indicates that the associated objects should live for the remainder of the lifetime of the running process which created the object.
-ProxyStore does not yet support a `StaticLifetime` class, but static lifetimes can be achieved with the use of a [`ContextLifetime`][proxystore.store.lifetimes.ContextLifetime] and an [atexit][atexit] handler.
+The [`StaticLifetime`][proxystore.store.lifetimes.StaticLifetime], a singleton class, will evict all associated objects at the end of the program via an [atexit][atexit] handler.
 
 ```python linenums="1" title="Static Lifetime"
-from proxystore.store.base import Store
-from proxystore.store.lifetimes import ContextLifetime
-from proxystore.store.lifetimes import register_lifetime_atexit
+from proxystore.connectors.local import LocalConnector
+from proxystore.store import Store
+from proxystore.store.lifetimes import StaticLifetime
 
-store = Store(...)
-
-lifetime = ContextLifetime(store)  # (1)!
-register_lifetime_atexit(lifetime, close_store=True)  # (2)!
+store = Store('default', LocalConnector(), register=True)  # (1)!
 
-key = store.put('value', lifetime=lifetime)  # (3)!
-proxy = store.proxy('value', lifetime=lifetime)
+key = store.put('value', lifetime=StaticLifetime())  # (2)!
+proxy = store.proxy('value', lifetime=StaticLifetime())  # (3)!
 ```
 
-1. Create and use a [`ContextLifetime`][proxystore.store.lifetimes.ContextLifetime] as normal.
-2. Register an [atexit][atexit] handler with [`register_lifetime_atexit`][proxystore.store.lifetimes.register_lifetime_atexit].
-   The `close_store` flag is `True` by default and will close the [`Store`][proxystore.store.base.Store] after the lifetime has been cleaned up.
-3. Objects associated with the lifetime will be cleaned up when the program exits.
+1. The atexit handler will call `store.close()` at the end of the program.
+   Setting `register=True` is recommended to prevent another instance being created internally when a proxy is resolved.
+2. The object associated with `key` will be evicted at the end of
+   the program.
+3. The object associated with `proxy` will be evicted at the end of
+   the program.
 
 Additional tips:
 
-1. The lifetime can be closed early if needed.
-2. Closing the [`Store`][proxystore.store.base.Store] at the end of the program but before the [atexit][atexit] handler has executed can cause undefined behaviour.
+1. Closing the [`Store`][proxystore.store.base.Store] at the end of the program but before the [atexit][atexit] handler has executed can cause undefined behaviour.
    Let the handler perform all cleanup.
+2. The [`StaticLifetime`][proxystore.store.lifetimes.StaticLifetime] can be closed manually, but only once.
+   This may be useful if the the associated stores need to be closed manually or outside of the atexit handler.
+   (Close the lifetime before the stores.)
 3. [atexit][atexit] does not guarantee that the handler will be called in some unexpected process shutdown cases.
+   This can lead to a memory leak in the connector(s).
 
 ## Ownership
 
 An [`OwnedProxy`][proxystore.store.ref.OwnedProxy], created by [`Store.owned_proxy()`][proxystore.store.base.Store.owned_proxy], provides an alternative to the default [`Proxy`][proxystore.proxy.Proxy] which enforces Rust-like ownership and borrowing rules for objects in a [`Store`][proxystore.store.base.Store].
 
 1. Each *target* object of type `T` in the global store has an associated [`OwnedProxy[T]`][proxystore.store.ref.OwnedProxy].
 2. There can only be one [`OwnedProxy[T]`][proxystore.store.ref.OwnedProxy] for any *target* in the global store.
```

### Comparing `proxystore-0.6.4/docs/guides/performance.md` & `proxystore-0.6.5/docs/guides/performance.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # Performance Tracking
 
-*Last updated 2 May 2023*
+*Last updated 20 April 2024*
 
 The [`Store`][proxystore.store.base.Store] can record metrics on executed operations (e.g., `get` and `put`).
 Metric collection is disabled by default and can be enabled by passing `#!python metrics=True` to a [`Store`][proxystore.store.base.Store] constructor.
 
 ## Enabling Metrics
 
 ```python linenums="1"
 import dataclasses
 from proxystore.connectors.file import FileConnector
-from proxystore.store import register_store
 from proxystore.store.base import Store
 
 store = Store(
    name='example-store',
    connector=FileConnector('/tmp/proxystore-dump'),
    metrics=True,  # (1)!
+   register=True,
 )
-register_store(store)
 assert store.metrics is not None
 ```
 
 1. Metric tracking is not enabled by default.
 
 Metrics are accessed via the
 [`Store.metrics`][proxystore.store.base.Store.metrics] property. This property
@@ -31,14 +30,21 @@
 !!! warning
     Metrics are local to each [`Store`][proxystore.store.base.Store] instance.
     In multi-process applications or applications that instantiate multiple
     [`Store`][proxystore.store.base.Store] instances,
     [`Store.metrics`][proxystore.store.base.Store.metrics] will only represent
     a partial view of the overall performance.
 
+!!! warning
+    ProxyStore v0.6.4 and older have a bug that causes the conversion from
+    nanoseconds to milliseconds in the
+    [`Metrics`][proxystore.store.metrics.Metrics] class to be incorrect.
+    This was fixed in v0.6.5 (see
+    [PR #538](https://github.com/proxystore/proxystore/pull/538){target=_blank}).
+
 Three types of metrics are collected.
 
 * Attributes: arbitrary attributes associated with an operation.
 * Counters: scalar counters that represent the number of times an event occurs.
 * Times: durations of events.
 
 ## A Simple Example
@@ -148,14 +154,15 @@
 proxy internally resolved the factory so we also see metrics about the
 `factory` and `store.get`.
 
 !!! warning
 
     For metrics to appropriately be tracked when a proxy is resolved, the
     [`Store`][proxystore.store.base.Store] needs to be registered globally
+    by setting `register=True` in the constructor or by manually registering
     with [`register_store()`][proxystore.store.register_store]. Otherwise,
     the factory will initialize a second [`Store`][proxystore.store.base.Store]
     to register and record its metrics to the second instance.
 
 ## Metrics for Batch Operations
 
 For batch [`Store`][proxystore.store.base.Store] operations, metrics are
```

### Comparing `proxystore-0.6.4/docs/guides/proxy-futures.md` & `proxystore-0.6.5/docs/guides/proxy-futures.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/guides/relay-serving.md` & `proxystore-0.6.5/docs/guides/relay-serving.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ```
 
 This relay server would be accessible at `ws://localhost:8700`. For example,
 an endpoint can be configure with this URI and will connect this instance
 when started.
 
 ```bash
-$ proxystore-endpoint configure my-endpoint --relay-server ws://localhost:8700`
+$ proxystore-endpoint configure my-endpoint --relay-server ws://localhost:8700
 $ proxystore-endpoint start my-endpoint --no-detach
 ```
 
 Here you would see the endpoint register with the relay server instance. See
 the [Endpoints Overview](endpoints.md) for more on how endpoints interact
 with a relay server.
 
@@ -78,15 +78,15 @@
 current_client_interval = 60
 current_client_limit = 32
 ```
 
 ## User Authentication
 
 A relay provides no user authentication by default. This means that any client
-can connect to any other client as long as they know the clients UUID. This
+can connect to any other client as long as they know the client's UUID. This
 may be suitable for internal or development purposes, but users should take
 extra precautions to ensure sensitive data is not exposed.
 
 The relay implementation supports serving with
 [Globus Auth](https://www.globus.org/globus-auth-service){target=_blank}.
 The following describes the steps required to create a Globus developer
 application and serve the relay with Globus Auth.
```

### Comparing `proxystore-0.6.4/docs/guides/streaming.md` & `proxystore-0.6.5/docs/guides/streaming.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/installation.md` & `proxystore-0.6.5/docs/installation.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 ProxyStore provides many features with extra dependencies that can be installed with the appropriate extras option.
 
 | Install | Purpose |
 | :------ | :------ |
 | `#!bash pip install proxystore[all]` | Install all extras except `dev` and `docs` |
 | `#!bash pip install proxystore[endpoints]` | Use [ProxyStore Endpoints](guides/endpoints.md) |
 | `#!bash pip install proxystore[extensions]` | Install the [`proxystore-ex`](https://github.com/proxystore/extensions){target=_blank} package |
-| `#!bash pip install proxystore[redis]` | Use the [`RedisConnector`][proxystore.connectors.redis.RedisConnector] |
+| `#!bash pip install proxystore[kafka]` | Use [Kafka stream shims][proxystore.stream.shims.kafka] |
+| `#!bash pip install proxystore[redis]` | Use [Redis stream shims][proxystore.stream.shims.redis] or the [`RedisConnector`][proxystore.connectors.redis.RedisConnector] |
+| `#!bash pip install proxystore[zmq]` | Use [ZeroMQ stream shims][proxystore.stream.shims.zmq] |
 | `#!bash pip install proxystore[dev]` | Development dependencies |
 | `#!bash pip install proxystore[docs]` | Documentation dependencies |
 
 Multiple extras options can be install at the same time.
 
 ```bash
 $ pip install proxystore[endpoints,redis]
```

### Comparing `proxystore-0.6.4/docs/publications/index.md` & `proxystore-0.6.5/docs/publications/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 }
 ```
 
 ## Featured Papers
 
 *If you use ProxyStore in your work and would like to be featured on this page, open an [issue](https://github.com/proxystore/proxystore/issues){target=_blank} or propose a [pull request](https://github.com/proxystore/proxystore/pulls){target=_blank} on GitHub.*
 
+* Devaraj, Harish, Shaleeza Sohail, Boyang Li, Nathaniel Hudson, Matt Baughman, Kyle Chard, Ryan Chard, Enrico Casella, Ian Foster, and Omer Rana. ["RuralAI in Tomato Farming: Integrated Sensor System, Distributed Computing and Hierarchical Federated Learning for Crop Health Monitoring."](https://doi.org/10.1109/LSENS.2024.3384935){target=_blank} *IEEE Sensors Letters*. IEEE, 2024.
 * Gautham Dharuman, Logan Ward, Heng Ma, Priyanka V. Setty, Ozan Gokdemir, Sam Foreman, Murali Emani, Kyle Hippe, Alexander Brace, Kristopher Keipert, Thomas Gibbs, Ian Foster, Anima Anandkumar, Venkatram Vishwanath, and Arvind Ramanathan. ["Protein Generation via Genome-scale Language Models with Bio-physical Scoring."](https://dl.acm.org/doi/abs/10.1145/3624062.3626087){target=_blank} *In Proceedings of the SC '23 Workshops of The International Conference on High Performance Computing, Network, Storage, and Analysis*. ACM, 2023.
 * Alok Kamatar, Mansi Sakarvadia, Valerie Hayot-Sasson, Kyle Chard, and Ian Foster. ["Lazy Python Dependency Management in Large-Scale Systems."](https://ieeexplore.ieee.org/document/10254910){target=_blank} *In Proceedings of IEEE 19th International Conference on e-Science.* IEEE, 2023.
 * Hassan Harb, Sarah N. Elliot, Logan Ward, Ian T. Foster, Stephen J. Klippenstein, Larry A. Curtiss, and Rajeev Surendran Assary. ["Uncovering novel liquid organic hydrogen carriers: a systematic exploration of chemical compound space using cheminformatics and quantum chemical methods."](https://doi.org/10.1039/D3DD00123G){target=_blank} *In Digital Discovery.* Royal Society of Chemistry, 2023.
 * Nicholson Collier, Justin M. Wozniak, Abby Stevens, Yadu Babuji, Mickaël Binois, Arindam Fadikar, Alexandra Würth, Kyle Chard, and Jonathan Ozik. ["Developing Distributed High-performance Computing Capabilities of an Open Science Platform for Robust Epidemic Analysis."](https://arxiv.org/abs/2304.14244){target=_blank} arXiv, 2023.
 * Logan Ward, J. Gregory Pauloski, Valerie Hayot-Sasson, Ryan Chard, Yadu Babuji, Ganesh Sivaraman, Sutanay Choudhury, Kyle Chard, Rajeev Thakur, and Ian Foster. ["Cloud Services Enable Efficient AI-Guided Simulation Workflows across Heterogeneous Resources."](https://arxiv.org/abs/2303.08803){target=_blank} *In Proceedings of Heterogeneity in Computing Workshop of the International Parallel and Distributed Processing Symposium.* IEEE, 2023.
 * Maxim Zvyagin et al. ["GenSLMs: Genome-scale language models reveal SARS-CoV-2 evolutionary dynamics."](https://www.biorxiv.org/content/10.1101/2022.10.10.511571v2){target=_blank} bioRxiv, 2022.
 * Logan Ward, Ganesh Sivaraman, J. Gregory Pauloski, Yadu Babuji, Ryan Chard, Naveen Dandu, Paul C. Redfern, Rajeev S. Assary, Kyle Chard, Larry A. Curtiss, Rajeev Thakur, and Ian Foster. ["Colmena: Scalable machine-learning-based steering of ensemble simulations for high performance computing."](https://arxiv.org/abs/2110.02827){target=_blank} *In IEEE/ACM Workshop on Machine Learning in High Performance Computing Environments.* IEEE, 2021.
```

### Comparing `proxystore-0.6.4/docs/static/endpoint-overview.svg` & `proxystore-0.6.5/docs/static/endpoint-overview.svg`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/static/endpoint-peering.svg` & `proxystore-0.6.5/docs/static/endpoint-peering.svg`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/static/favicon.png` & `proxystore-0.6.5/docs/static/favicon.png`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/static/icon.png` & `proxystore-0.6.5/docs/static/icon.png`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/static/logo-dark.png` & `proxystore-0.6.5/docs/static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/static/logo-light.png` & `proxystore-0.6.5/docs/static/logo-light.png`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/static/proxystore-overview.svg` & `proxystore-0.6.5/docs/static/proxystore-overview.svg`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/static/proxystore-schematic.svg` & `proxystore-0.6.5/docs/static/proxystore-schematic.svg`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/docs/static/proxystore-streaming.svg` & `proxystore-0.6.5/docs/static/proxystore-streaming.svg`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/examples/README.md` & `proxystore-0.6.5/examples/README.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/examples/globus-compute/README.md` & `proxystore-0.6.5/examples/globus-compute/README.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/examples/globus-compute/mapreduce_globus_compute.py` & `proxystore-0.6.5/examples/globus-compute/mapreduce_globus_compute.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/examples/globus-compute/run.sh` & `proxystore-0.6.5/examples/globus-compute/run.sh`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/examples/parsl/mapreduce_parsl.py` & `proxystore-0.6.5/examples/parsl/mapreduce_parsl.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/examples/parsl/run.sh` & `proxystore-0.6.5/examples/parsl/run.sh`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/bin/bash
 
 PORT=59465
 redis-server --save "" --appendonly no --port $PORT &> /dev/null &
 REDIS=$!
 
-ARRAY_COUNT=100
-ARRAY_SIZE=100
+ARRAY_COUNT=10
+ARRAY_SIZE=1000
 
 echo "Started Redis on localhost:$PORT"
 
 echo "Running mapreduce_parsl.py without ProxyStore"
-python mapreduce_parsl.py -n $ARRAY_SIZE -s $ARRAY_SIZE
+python mapreduce_parsl.py -n $ARRAY_COUNT -s $ARRAY_SIZE
 
 echo "Running mapreduce_parsl.py with ProxyStore (Local)"
-python mapreduce_parsl.py -n $ARRAY_SIZE -s $ARRAY_SIZE --proxy
+python mapreduce_parsl.py -n $ARRAY_COUNT -s $ARRAY_SIZE --proxy
 
 echo "Running mapreduce_parsl.py with ProxyStore (Redis)"
-python mapreduce_parsl.py -n $ARRAY_SIZE -s $ARRAY_SIZE --proxy --redis-port $PORT
+python mapreduce_parsl.py -n $ARRAY_COUNT -s $ARRAY_SIZE --proxy --redis-port $PORT
 
 kill $REDIS
```

### Comparing `proxystore-0.6.4/examples/store_metrics.py` & `proxystore-0.6.5/examples/store_metrics.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/mkdocs.yml` & `proxystore-0.6.5/mkdocs.yml`

 * *Files 3% similar despite different names*

```diff
@@ -107,23 +107,25 @@
 
 nav:
   - Home:
       - Overview: index.md
       - Installation: installation.md
       - Get Started: get-started.md
       - Examples: examples.md
-      - Known Issues: known-issues.md
+      - FAQ: faq.md
+      - Issues (GitHub): https://github.com/proxystore/proxystore/issues
       - Changelog (GitHub): https://github.com/proxystore/proxystore/releases
   - Concepts:
       - concepts/index.md
       - Proxy: concepts/proxy.md
       - Connector: concepts/connector.md
       - Store: concepts/store.md
   - Guides:
       - guides/index.md
+      - Dask Distributed: guides/dask-distributed.md
       - Globus Compute: guides/globus-compute.md
       - Endpoints Overview: guides/endpoints.md
       - Endpoints Debugging: guides/endpoints-debugging.md
       - Object Lifetimes: guides/object-lifetimes.md
       - Performance Tracking: guides/performance.md
       - Proxy Futures: guides/proxy-futures.md
       - Relay Serving: guides/relay-serving.md
@@ -162,14 +164,15 @@
             - https://aiortc.readthedocs.io/en/latest/objects.inv
             - https://globus-sdk-python.readthedocs.io/en/stable/objects.inv
             - https://websockets.readthedocs.io/en/stable/objects.inv
             - https://requests.readthedocs.io/en/latest/objects.inv
             - https://extensions.proxystore.dev/main/objects.inv
             - https://redis-py.readthedocs.io/en/stable/objects.inv
             - https://kafka-python.readthedocs.io/en/master/objects.inv
+            - https://distributed.dask.org/en/latest/objects.inv
           options:
             annotations_path: brief
             docstring_section_style: list
             docstring_style: google
             inherited_members: yes
             line_length: 60
             members_order: source
```

### Comparing `proxystore-0.6.4/proxystore/connectors/__init__.py` & `proxystore-0.6.5/proxystore/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/connectors/dim.py` & `proxystore-0.6.5/proxystore/connectors/dim.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/connectors/endpoint.py` & `proxystore-0.6.5/proxystore/connectors/endpoint.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/connectors/file.py` & `proxystore-0.6.5/proxystore/connectors/file.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/connectors/globus.py` & `proxystore-0.6.5/proxystore/connectors/globus.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/connectors/local.py` & `proxystore-0.6.5/proxystore/connectors/local.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/connectors/multi.py` & `proxystore-0.6.5/proxystore/connectors/multi.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/connectors/protocols.py` & `proxystore-0.6.5/proxystore/connectors/protocols.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/connectors/redis.py` & `proxystore-0.6.5/proxystore/connectors/redis.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/endpoint/__init__.py` & `proxystore-0.6.5/proxystore/endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/endpoint/cli.py` & `proxystore-0.6.5/proxystore/endpoint/cli.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/endpoint/client.py` & `proxystore-0.6.5/proxystore/endpoint/client.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/endpoint/commands.py` & `proxystore-0.6.5/proxystore/endpoint/commands.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/endpoint/config.py` & `proxystore-0.6.5/proxystore/endpoint/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 import uuid
 from typing import Any
 from typing import Dict
 from typing import Literal
 from typing import Optional
 
 from pydantic import BaseModel
+from pydantic import ConfigDict
 from pydantic import Field
 
 try:
     from pydantic import field_validator
 except ImportError:  # pragma: no cover
     # Pydantic v1 compatibility
-    from pydantic import validator as field_validator
+    from pydantic import validator as field_validator  # type: ignore[no-redef]
 
 from proxystore.endpoint.constants import MAX_OBJECT_SIZE_DEFAULT
 from proxystore.utils.config import dump
 from proxystore.utils.config import load
 
 ENDPOINT_CONFIG_FILE = 'config.toml'
 ENDPOINT_DATABASE_FILE = 'blobs.db'
@@ -33,14 +34,16 @@
     """Endpoint relay server authentication configuration.
 
     Attributes:
         method: Relay server authentication method.
         kwargs: Arbitrary options used by the authentication method.
     """
 
+    model_config = ConfigDict(extra='forbid')
+
     method: Optional[Literal['globus']] = None  # noqa: UP007
     kwargs: Dict[str, Any] = Field(default_factory=dict)  # noqa: UP006
 
 
 class EndpointRelayConfig(BaseModel):
     """Endpoint relay server configuration.
```

### Comparing `proxystore-0.6.4/proxystore/endpoint/endpoint.py` & `proxystore-0.6.5/proxystore/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/endpoint/exceptions.py` & `proxystore-0.6.5/proxystore/endpoint/exceptions.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/endpoint/messages.py` & `proxystore-0.6.5/proxystore/endpoint/messages.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/endpoint/serve.py` & `proxystore-0.6.5/proxystore/endpoint/serve.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/endpoint/storage.py` & `proxystore-0.6.5/proxystore/endpoint/storage.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/ex.py` & `proxystore-0.6.5/proxystore/ex.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/factory.py` & `proxystore-0.6.5/proxystore/factory.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/globus/cli.py` & `proxystore-0.6.5/proxystore/globus/cli.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/globus/client.py` & `proxystore-0.6.5/proxystore/globus/client.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/globus/manager.py` & `proxystore-0.6.5/proxystore/globus/manager.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/globus/scopes.py` & `proxystore-0.6.5/proxystore/globus/scopes.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/globus/storage.py` & `proxystore-0.6.5/proxystore/globus/storage.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/globus/transfer.py` & `proxystore-0.6.5/proxystore/globus/transfer.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/p2p/__init__.py` & `proxystore-0.6.5/proxystore/p2p/__init__.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/p2p/chunks.py` & `proxystore-0.6.5/proxystore/p2p/chunks.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/p2p/connection.py` & `proxystore-0.6.5/proxystore/p2p/connection.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/p2p/manager.py` & `proxystore-0.6.5/proxystore/p2p/manager.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/p2p/nat.py` & `proxystore-0.6.5/proxystore/p2p/nat.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/p2p/relay/authenticate.py` & `proxystore-0.6.5/proxystore/p2p/relay/authenticate.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/p2p/relay/client.py` & `proxystore-0.6.5/proxystore/p2p/relay/client.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/p2p/relay/config.py` & `proxystore-0.6.5/proxystore/p2p/relay/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 if sys.version_info >= (3, 11):  # pragma: >=3.11 cover
     from typing import Self
 else:  # pragma: <3.11 cover
     from typing_extensions import Self
 
 from pydantic import BaseModel
+from pydantic import ConfigDict
 from pydantic import Field
 
 from proxystore.utils.config import load
 
 
 class RelayAuthConfig(BaseModel):
     """Relay authentication configuration.
@@ -28,14 +29,16 @@
     Attributes:
         method: Authentication method.
         kwargs: Arbitrary keyword arguments to pass to the authenticator.
             The kwargs are excluded from the [`repr()`][repr] of this
             class because they often contain secrets.
     """
 
+    model_config = ConfigDict(extra='forbid')
+
     method: Optional[Literal['globus']] = None  # noqa: UP007
     kwargs: Dict[str, Any] = Field(  # noqa: UP006
         default_factory=dict,
         repr=False,
     )
```

### Comparing `proxystore-0.6.4/proxystore/p2p/relay/exceptions.py` & `proxystore-0.6.5/proxystore/p2p/relay/exceptions.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/p2p/relay/manager.py` & `proxystore-0.6.5/proxystore/p2p/relay/manager.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/p2p/relay/messages.py` & `proxystore-0.6.5/proxystore/p2p/relay/messages.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/p2p/relay/run.py` & `proxystore-0.6.5/proxystore/p2p/relay/run.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/p2p/relay/server.py` & `proxystore-0.6.5/proxystore/p2p/relay/server.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/serialize.py` & `proxystore-0.6.5/proxystore/serialize.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/store/__init__.py` & `proxystore-0.6.5/proxystore/store/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 """The ProxyStore [`Store`][proxystore.store.base.Store] interface."""
 
 from __future__ import annotations
 
 import contextlib
 import logging
+import threading
 from typing import Any
 from typing import Generator
 from typing import Sequence
 from typing import TypeVar
 
 from proxystore.connectors.protocols import Connector
+from proxystore.proxy import get_factory
 from proxystore.proxy import Proxy
 from proxystore.store.base import Store
 from proxystore.store.exceptions import ProxyStoreFactoryError
 from proxystore.store.exceptions import StoreExistsError
 from proxystore.store.factory import StoreFactory
 from proxystore.store.types import ConnectorT
+from proxystore.store.types import StoreConfig
 
 __all__ = [
     'Store',
     'StoreFactory',
     'get_store',
     'register_store',
     'store_registration',
     'unregister_store',
 ]
 
 T = TypeVar('T')
 
 _stores: dict[str, Store[Any]] = {}
+_stores_lock = threading.RLock()
 logger = logging.getLogger(__name__)
 
 
 def get_store(val: str | Proxy[T]) -> Store[Any] | None:
-    """Get the backend store with name.
+    """Get a registered store by name.
 
     Args:
         val: name of the store to get or a [`Proxy`][proxystore.proxy.Proxy]
             instance.
 
     Returns:
         [`Store`][proxystore.store.base.Store] if a store matching the \
@@ -47,29 +51,57 @@
     Raises:
         ProxyStoreFactoryError: If the value is a proxy but does not contain a
             factory of type
             [`StoreFactory`][proxystore.store.base.StoreFactory].
     """
     if isinstance(val, Proxy):
         # If the object is a proxy, get the factory that will access the store
-        factory = val.__factory__
+        factory = get_factory(val)
         if isinstance(factory, StoreFactory):
             return factory.get_store()
         else:
             raise ProxyStoreFactoryError(
                 'The proxy must contain a factory with type '
                 f'{type(StoreFactory).__name__}. {type(factory).__name__} '
                 'is not supported.',
             )
     else:
         name = val
 
-    if name in _stores:
-        return _stores[name]
-    return None
+    with _stores_lock:
+        if name in _stores:
+            return _stores[name]
+        return None
+
+
+def get_or_create_store(
+    store_config: StoreConfig,
+    *,
+    register: bool = True,
+) -> Store[Any]:
+    """Get a registered store or initialize a new instance from the config.
+
+    Args:
+        store_config: Store configuration used to reinitialize the store if
+            needed.
+        register: Optionally register the store if a new instance was
+            initialized.
+
+    Returns:
+        [`Store`][proxystore.store.base.Store] instance.
+    """
+    with _stores_lock:
+        store = get_store(store_config['name'])
+        if store is None:
+            store = Store.from_config(store_config)
+            if register:
+                # Set exists_ok here because the store may have initialized
+                # itself if register=True.
+                register_store(store, exist_ok=True)
+        return store
 
 
 def register_store(store: Store[Any], exist_ok: bool = False) -> None:
     """Register the store instance to the global registry.
 
     Note:
         Global means globally accessible within the Python process.
@@ -82,19 +114,22 @@
         store: Store instance to register.
         exist_ok: If a store with the same name exists, overwrite it.
 
     Raises:
         StoreExistsError: If a store with the same name is already registered
             and `exist_ok` is false.
     """
-    if store.name in _stores and not exist_ok:
-        raise StoreExistsError(f'A store named {store.name} already exists.')
+    with _stores_lock:
+        if store.name in _stores and not exist_ok:
+            raise StoreExistsError(
+                f'A store named "{store.name}" already exists.',
+            )
 
-    _stores[store.name] = store
-    logger.info(f'Registered a store named {store.name}')
+        _stores[store.name] = store
+        logger.info(f'Registered a store named "{store.name}"')
 
 
 @contextlib.contextmanager
 def store_registration(
     *stores: Store[Any],
     exist_ok: bool = False,
 ) -> Generator[None, None, None]:
@@ -145,10 +180,11 @@
 
     Args:
         name_or_store: Name of the store to unregister or a store itself.
     """
     name = (
         name_or_store if isinstance(name_or_store, str) else name_or_store.name
     )
-    if name in _stores:
-        del _stores[name]
-        logger.info(f'Unregistered a store named {name}')
+    with _stores_lock:
+        if name in _stores:
+            del _stores[name]
+            logger.info(f'Unregistered a store named {name}')
```

### Comparing `proxystore-0.6.4/proxystore/store/base.py` & `proxystore-0.6.5/proxystore/store/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,25 +25,27 @@
 import proxystore.serialize
 from proxystore.connectors.protocols import DeferrableConnector
 from proxystore.proxy import Proxy
 from proxystore.proxy import ProxyLocker
 from proxystore.serialize import SerializationError
 from proxystore.store.cache import LRUCache
 from proxystore.store.exceptions import NonProxiableTypeError
+from proxystore.store.exceptions import StoreExistsError
 from proxystore.store.factory import PollingStoreFactory
 from proxystore.store.factory import StoreFactory
 from proxystore.store.future import Future
 from proxystore.store.lifetimes import Lifetime
 from proxystore.store.metrics import StoreMetrics
 from proxystore.store.ref import into_owned
 from proxystore.store.ref import OwnedProxy
 from proxystore.store.types import ConnectorKeyT
 from proxystore.store.types import ConnectorT
 from proxystore.store.types import DeserializerT
 from proxystore.store.types import SerializerT
+from proxystore.store.types import StoreConfig
 from proxystore.utils.imports import get_object_path
 from proxystore.utils.imports import import_from_path
 from proxystore.utils.timer import Timer
 from proxystore.warnings import ExperimentalWarning
 
 logger = logging.getLogger(__name__)
 
@@ -77,41 +79,63 @@
         deserializer: Optional callable used by the factory to deserialize the
             byte string. If `None`, the default deserializer
             ([`deserialize()`][proxystore.serialize.deserialize]) will be
             used.
         cache_size: Size of LRU cache (in # of objects). If 0,
             the cache is disabled. The cache is local to the Python process.
         metrics: Enable recording operation metrics.
+        populate_target: Set the default value of `populate_target` for
+            proxy methods of the store.
+        register: Register the store instance after initialization.
 
     Raises:
         ValueError: If `cache_size` is less than zero.
+        StoreExistsError: If `register=True` and a store with `name` already
+            exists.
     """
 
     def __init__(
         self,
         name: str,
         connector: ConnectorT,
         *,
         serializer: SerializerT | None = None,
         deserializer: DeserializerT | None = None,
         cache_size: int = 16,
         metrics: bool = False,
+        populate_target: bool = False,
+        register: bool = False,
     ) -> None:
         if cache_size < 0:
             raise ValueError(
                 f'Cache size cannot be negative. Got {cache_size}.',
             )
 
         self.connector = connector
         self.cache: LRUCache[ConnectorKeyT, Any] = LRUCache(cache_size)
         self._name = name
         self._metrics = StoreMetrics() if metrics else None
         self._cache_size = cache_size
         self._serializer = serializer
         self._deserializer = deserializer
+        self._populate_target = populate_target
+        self._register = register
+
+        if self._register:
+            try:
+                proxystore.store.register_store(self)
+            except StoreExistsError as e:
+                if sys.version_info >= (3, 11):  # pragma: >=3.11 cover
+                    e.add_note(
+                        'Consider using get_store(name) rather than '
+                        'initializing a new instance with register=True.',
+                    )
+                else:  # pragma: <3.11 cover
+                    pass
+                raise
 
         logger.info(f'Initialized {self}')
 
     def __enter__(self) -> Self:
         return self
 
     def __exit__(
@@ -119,22 +143,30 @@
         exc_type: type[BaseException] | None,
         exc_value: BaseException | None,
         exc_traceback: TracebackType | None,
     ) -> None:
         self.close()
 
     def __repr__(self) -> str:
-        serializer = 'default' if self._serializer is None else 'custom'
-        deserializer = 'default' if self._deserializer is None else 'custom'
-        return (
-            f'Store("{self.name}", connector={self.connector}, '
-            f'serializer={serializer}, deserializer={deserializer}, '
-            f'cache_size={self.cache.maxsize}, '
-            f'metrics={self.metrics is not None})'
+        config = dict(**self.config())
+
+        del config['name']
+        del config['connector_type']
+        del config['connector_config']
+
+        config['serializer'] = (
+            'default' if config['serializer'] is None else 'custom'
+        )
+        config['deserializer'] = (
+            'default' if config['deserializer'] is None else 'custom'
         )
+        config['metrics'] = self.metrics is not None
+
+        params = ', '.join(f'{k}={v}' for k, v in config.items())
+        return f'Store(name={self.name}, connector={self.connector}, {params})'
 
     @property
     def name(self) -> str:
         """Name of this [`Store`][proxystore.store.base.Store] instance."""
         return self._name
 
     @property
@@ -159,66 +191,75 @@
             if self._deserializer is not None
             else proxystore.serialize.deserialize
         )
 
     def close(self, *args: Any, **kwargs: Any) -> None:
         """Close the connector associated with the store.
 
+        This will (1) close the connector and (2) unregister the store if
+        `register=True` was set during initialization.
+
         Warning:
             This method should only be called at the end of the program
             when the store will no longer be used, for example once all
             proxies have been resolved.
 
         Args:
             args: Positional arguments to pass to
                 [`Connector.close()`][proxystore.connectors.protocols.Connector.close].
             kwargs: Keyword arguments to pass to
                 [`Connector.close()`][proxystore.connectors.protocols.Connector.close].
         """
+        if self._register:
+            proxystore.store.unregister_store(self.name)
         self.connector.close(*args, **kwargs)
 
-    def config(self) -> dict[str, Any]:
+    def config(self) -> StoreConfig:
         """Get the store configuration.
 
         Example:
             ```python
             >>> store = Store(...)
             >>> config = store.config()
             >>> store = Store.from_config(config)
             ```
 
         Returns:
             Store configuration.
         """
-        return {
-            'name': self.name,
-            'connector_type': get_object_path(type(self.connector)),
-            'connector_config': self.connector.config(),
-            'serializer': self._serializer,
-            'deserializer': self._deserializer,
-            'cache_size': self._cache_size,
-            'metrics': self.metrics is not None,
-        }
+        return StoreConfig(
+            name=self.name,
+            connector_type=get_object_path(type(self.connector)),
+            connector_config=self.connector.config(),
+            serializer=self._serializer,
+            deserializer=self._deserializer,
+            cache_size=self._cache_size,
+            metrics=self.metrics is not None,
+            populate_target=self._populate_target,
+            register=self._register,
+        )
 
     @classmethod
-    def from_config(cls, config: dict[str, Any]) -> Store[Any]:
+    def from_config(cls, config: StoreConfig) -> Store[Any]:
         """Create a new store instance from a configuration.
 
         Args:
             config: Configuration returned by `#!python .config()`.
 
         Returns:
             Store instance.
         """
-        config = config.copy()  # Avoid messing with callers version
-        connector_type = config.pop('connector_type')
-        connector_config = config.pop('connector_config')
+        # Avoid messing with callers version and splat into new dict otherwise
+        # mypy will error that we are popping required keys from a TypedDict.
+        mut_config: dict[str, Any] = dict(**config.copy())
+        connector_type = mut_config.pop('connector_type')
+        connector_config = mut_config.pop('connector_config')
         connector = import_from_path(connector_type)
-        config['connector'] = connector.from_config(connector_config)
-        return cls(**config)
+        mut_config['connector'] = connector.from_config(connector_config)
+        return cls(**mut_config)
 
     def future(
         self,
         *,
         evict: bool = False,
         serializer: SerializerT | None = None,
         deserializer: DeserializerT | None = None,
@@ -311,15 +352,15 @@
             stacklevel=2,
         )
 
         with Timer() as connector_timer:
             key = self.connector.new_key()
 
         if self.metrics is not None:
-            ctime = connector_timer.elapsed_ns
+            ctime = connector_timer.elapsed_ms
             self.metrics.add_time('store.future.connector', key, ctime)
 
         factory: PollingStoreFactory[ConnectorT, T] = PollingStoreFactory(
             key,
             store_config=self.config(),
             deserializer=deserializer,
             evict=evict,
@@ -328,15 +369,15 @@
             polling_interval_limit=polling_interval_limit,
             polling_timeout=polling_timeout,
         )
         future = Future(factory, serializer=serializer)
 
         timer.stop()
         if self.metrics is not None:
-            self.metrics.add_time('store.future', key, timer.elapsed_ns)
+            self.metrics.add_time('store.future', key, timer.elapsed_ms)
 
         logger.debug(
             f'Store(name="{self.name}"): FUTURE {key} in '
             f'{timer.elapsed_ms:.3f} ms',
         )
         return future
 
@@ -347,21 +388,21 @@
             key: Key associated with object to evict.
         """
         with Timer() as timer:
             with Timer() as connector_timer:
                 self.connector.evict(key)
 
             if self.metrics is not None:
-                ctime = connector_timer.elapsed_ns
+                ctime = connector_timer.elapsed_ms
                 self.metrics.add_time('store.evict.connector', key, ctime)
 
             self.cache.evict(key)
 
         if self.metrics is not None:
-            self.metrics.add_time('store.evict', key, timer.elapsed_ns)
+            self.metrics.add_time('store.evict', key, timer.elapsed_ms)
 
         logger.debug(
             f'Store(name="{self.name}"): EVICT {key} in '
             f'{timer.elapsed_ms:.3f} ms',
         )
 
     def exists(self, key: ConnectorKeyT) -> bool:
@@ -376,19 +417,19 @@
         with Timer() as timer:
             res = self.cache.exists(key)
             if not res:
                 with Timer() as connector_timer:
                     res = self.connector.exists(key)
 
                 if self.metrics is not None:
-                    ctime = connector_timer.elapsed_ns
+                    ctime = connector_timer.elapsed_ms
                     self.metrics.add_time('store.exists.connector', key, ctime)
 
         if self.metrics is not None:
-            self.metrics.add_time('store.exists', key, timer.elapsed_ns)
+            self.metrics.add_time('store.exists', key, timer.elapsed_ms)
 
         logger.debug(
             f'Store(name="{self.name}"): EXISTS {key} in '
             f'{timer.elapsed_ms:.3f} ms',
         )
         return res
 
@@ -420,27 +461,27 @@
 
         if self.is_cached(key):
             value = self.cache.get(key)
 
             timer.stop()
             if self.metrics is not None:
                 self.metrics.add_counter('store.get.cache_hits', key, 1)
-                self.metrics.add_time('store.get', key, timer.elapsed_ns)
+                self.metrics.add_time('store.get', key, timer.elapsed_ms)
 
             logger.debug(
                 f'Store(name="{self.name}"): GET {key} in '
                 f'{timer.elapsed_ms:.3f} ms (cached=True)',
             )
             return value
 
         with Timer() as connector_timer:
             value = self.connector.get(key)
 
         if self.metrics is not None:
-            ctime = connector_timer.elapsed_ns
+            ctime = connector_timer.elapsed_ms
             self.metrics.add_counter('store.get.cache_misses', key, 1)
             self.metrics.add_time('store.get.connector', key, ctime)
 
         if value is not None:
             with Timer() as deserializer_timer:
                 deserializer = (
                     deserializer
@@ -453,30 +494,30 @@
                     name = get_object_path(deserializer)
                     raise SerializationError(
                         'Failed to deserialize object '
                         f'(deserializer={name}, key={key}).',
                     ) from e
 
             if self.metrics is not None:
-                dtime = deserializer_timer.elapsed_ns
+                dtime = deserializer_timer.elapsed_ms
                 obj_size = len(value)
                 self.metrics.add_time('store.get.deserialize', key, dtime)
                 self.metrics.add_attribute(
                     'store.get.object_size',
                     key,
                     obj_size,
                 )
 
             self.cache.set(key, result)
         else:
             result = default
 
         timer.stop()
         if self.metrics is not None:
-            self.metrics.add_time('store.get', key, timer.elapsed_ns)
+            self.metrics.add_time('store.get', key, timer.elapsed_ms)
 
         logger.debug(
             f'Store(name="{self.name}"): GET {key} in '
             f'{timer.elapsed_ms:.3f} ms (cached=False)',
         )
         return result
 
@@ -500,42 +541,42 @@
         self,
         obj: NonProxiableT,
         *,
         evict: bool = ...,
         lifetime: Lifetime | None = ...,
         serializer: SerializerT | None = ...,
         deserializer: DeserializerT | None = ...,
-        populate_target: bool = ...,
+        populate_target: bool | None = ...,
         skip_nonproxiable: Literal[True] = ...,
         **kwargs: Any,
     ) -> NonProxiableT: ...
 
     @overload
     def proxy(
         self,
         obj: T,
         *,
         evict: bool = ...,
         lifetime: Lifetime | None = ...,
         serializer: SerializerT | None = ...,
         deserializer: DeserializerT | None = ...,
-        populate_target: bool = ...,
+        populate_target: bool | None = ...,
         skip_nonproxiable: bool = ...,
         **kwargs: Any,
     ) -> Proxy[T]: ...
 
     def proxy(
         self,
         obj: T | NonProxiableT,
         *,
         evict: bool = False,
         lifetime: Lifetime | None = None,
         serializer: SerializerT | None = None,
         deserializer: DeserializerT | None = None,
-        populate_target: bool = False,
+        populate_target: bool | None = None,
         skip_nonproxiable: bool = False,
         **kwargs: Any,
     ) -> Proxy[T] | NonProxiableT:
         """Create a proxy that will resolve to an object in the store.
 
         Args:
             obj: The object to place in store and return a proxy for.
@@ -544,20 +585,23 @@
             lifetime: Attach the proxy to this lifetime. The object associated
                 with the proxy will be evicted when the lifetime ends.
                 Mutually exclusive with the `evict` parameter.
             serializer: Optionally override the default serializer for the
                 store instance.
             deserializer: Optionally override the default deserializer for the
                 store instance.
-            populate_target: Set the returned proxy to point at `obj`. I.e.,
-                return an already resolved proxy. This is `False` by default
-                because the returned proxy will hold a reference to `obj`
-                which will prevent garbage collecting `obj`. Setting this flag
-                is helpful when serializing the returned proxy on this process
-                will incidentally resolve the proxy.
+            populate_target: Pass `cache_defaults=True` and `target=obj` to
+                the [`Proxy`][proxystore.proxy.Proxy] constructor. I.e.,
+                return a proxy that (1) is already resolved, (2) can be used
+                in [`isinstance`][isinstance] checks without resolving, and (3)
+                is hashable without resolving if `obj` is a hashable type.
+                This is `False` by default because the returned proxy will
+                hold a reference to `obj` which will prevent garbage
+                collecting `obj`. If `None`, defaults to the store-wide
+                setting.
             skip_nonproxiable: Return non-proxiable types (e.g., built-in
                 constants like `bool` or `None`) rather than raising a
                 [`NonProxiableTypeError`][proxystore.store.exceptions.NonProxiableTypeError].
             kwargs: Additional keyword arguments to pass to
                 [`Connector.put()`][proxystore.connectors.protocols.Connector.put].
 
         Returns:
@@ -593,24 +637,32 @@
             key = self.put(obj, serializer=serializer, **kwargs)
             factory: StoreFactory[ConnectorT, T] = StoreFactory(
                 key,
                 store_config=self.config(),
                 deserializer=deserializer,
                 evict=evict,
             )
-            proxy = Proxy(factory)
+            populate_target = (
+                self._populate_target
+                if populate_target is None
+                else populate_target
+            )
+            if populate_target:
+                # If obj were None, we would have escaped early when
+                # checking _NON_PROXIABLE_TYPES.
+                assert obj is not None
+                proxy = Proxy(factory, cache_defaults=True, target=obj)
+            else:
+                proxy = Proxy(factory)
 
             if lifetime is not None:
                 lifetime.add_proxy(proxy)
 
-            if populate_target:
-                proxy.__wrapped__ = obj
-
         if self.metrics is not None:
-            self.metrics.add_time('store.proxy', key, timer.elapsed_ns)
+            self.metrics.add_time('store.proxy', key, timer.elapsed_ms)
 
         logger.debug(
             f'Store(name="{self.name}"): PROXY {key} in '
             f'{timer.elapsed_ms:.3f} ms',
         )
         return proxy
 
@@ -620,29 +672,29 @@
         self,
         objs: Sequence[NonProxiableT],
         *,
         evict: bool = ...,
         lifetime: Lifetime | None = ...,
         serializer: SerializerT | None = ...,
         deserializer: DeserializerT | None = ...,
-        populate_target: bool = ...,
+        populate_target: bool | None = ...,
         skip_nonproxiable: Literal[True] = ...,
         **kwargs: Any,
     ) -> list[NonProxiableT]: ...
 
     @overload
     def proxy_batch(
         self,
         objs: Sequence[T],
         *,
         evict: bool = ...,
         lifetime: Lifetime | None = ...,
         serializer: SerializerT | None = ...,
         deserializer: DeserializerT | None = ...,
-        populate_target: bool = ...,
+        populate_target: bool | None = ...,
         skip_nonproxiable: bool = ...,
         **kwargs: Any,
     ) -> list[Proxy[T]]: ...
 
     # MyPy raises the following:
     #    Overloaded function implementation cannot produce return type of
     #    signature 1
@@ -650,15 +702,15 @@
         self,
         objs: Sequence[T | NonProxiableT],
         *,
         evict: bool = False,
         lifetime: Lifetime | None = None,
         serializer: SerializerT | None = None,
         deserializer: DeserializerT | None = None,
-        populate_target: bool = False,
+        populate_target: bool | None = None,
         skip_nonproxiable: bool = False,
         **kwargs: Any,
     ) -> list[Proxy[T] | NonProxiableT]:
         """Create proxies that will resolve to an object in the store.
 
         Args:
             objs: The objects to place in store and return a proxies for.
@@ -667,21 +719,23 @@
             lifetime: Attach the proxies to this lifetime. The objects
                 associated with each proxy will be evicted when the lifetime
                 ends. Mutually exclusive with the `evict` parameter.
             serializer: Optionally override the default serializer for the
                 store instance.
             deserializer: Optionally override the default deserializer for the
                 store instance.
-            populate_target: Set each returned proxy to point at its
-                corresponding `obj`. I.e., return an already resolved proxy.
+            populate_target: Pass `cache_defaults=True` and `target=obj` to
+                the [`Proxy`][proxystore.proxy.Proxy] constructor. I.e.,
+                return a proxy that (1) is already resolved, (2) can be used
+                in [`isinstance`][isinstance] checks without resolving, and (3)
+                is hashable without resolving if `obj` is a hashable type.
                 This is `False` by default because the returned proxy will
-                hold a reference to `obj` which will prevent garbage collecting
-                `obj`. Setting this flag is helpful when serializing a
-                returned proxy on this process will incidentally resolve the
-                proxy.
+                hold a reference to `obj` which will prevent garbage
+                collecting `obj`. If `None`, defaults to the store-wide
+                setting.
             skip_nonproxiable: Return non-proxiable types (e.g., built-in
                 constants like `bool` or `None`) rather than raising a
                 [`NonProxiableTypeError`][proxystore.store.exceptions.NonProxiableTypeError].
             kwargs: Additional keyword arguments to pass to
                 [`Connector.put_batch()`][proxystore.connectors.protocols.Connector.put_batch].
 
         Returns:
@@ -723,36 +777,48 @@
             ]
 
             keys = self.put_batch(
                 proxiable_objs,
                 serializer=serializer,
                 **kwargs,
             )
-            proxies: list[Proxy[T]] = [
-                self.proxy_from_key(
+            factories: list[StoreFactory[ConnectorT, T]] = [
+                StoreFactory(
                     key,
+                    store_config=self.config(),
                     evict=evict,
-                    lifetime=lifetime,
                     deserializer=deserializer,
                 )
                 for key in keys
             ]
 
+            populate_target = (
+                self._populate_target
+                if populate_target is None
+                else populate_target
+            )
+
+            proxies: list[Proxy[T]] = []
+            for factory, obj in zip(factories, proxiable_objs):
+                if populate_target:
+                    proxy = Proxy(factory, cache_defaults=True, target=obj)
+                else:
+                    proxy = Proxy(factory)
+                proxies.append(proxy)
+
+            if lifetime is not None:
+                lifetime.add_proxy(*proxies)
+
             # Put non-proxiable objects back in their original positions.
             # The indices of non_proxiable must still be sorted
             for original_index, original_object in non_proxiable:
                 proxies.insert(original_index, original_object)
 
-            if populate_target:
-                for proxy, obj in zip(proxies, objs):
-                    if isinstance(proxy, Proxy):
-                        proxy.__wrapped__ = obj
-
         if self.metrics is not None:
-            self.metrics.add_time('store.proxy_batch', keys, timer.elapsed_ns)
+            self.metrics.add_time('store.proxy_batch', keys, timer.elapsed_ms)
 
         logger.debug(
             f'Store(name="{self.name}"): PROXY_BATCH ({len(proxies)} items) '
             f'in {timer.elapsed_ms:.3f} ms',
         )
         return cast(List[Union[Proxy[T], NonProxiableT]], proxies)
 
@@ -810,42 +876,42 @@
         self,
         obj: NonProxiableT,
         *,
         evict: bool = ...,
         lifetime: Lifetime | None = ...,
         serializer: SerializerT | None = ...,
         deserializer: DeserializerT | None = ...,
-        populate_target: bool = ...,
+        populate_target: bool | None = ...,
         skip_nonproxiable: Literal[True] = ...,
         **kwargs: Any,
     ) -> NonProxiableT: ...
 
     @overload
     def locked_proxy(
         self,
         obj: T,
         *,
         evict: bool = ...,
         lifetime: Lifetime | None = ...,
         serializer: SerializerT | None = ...,
         deserializer: DeserializerT | None = ...,
-        populate_target: bool = ...,
+        populate_target: bool | None = ...,
         skip_nonproxiable: bool = ...,
         **kwargs: Any,
     ) -> ProxyLocker[T]: ...
 
     def locked_proxy(
         self,
         obj: T | NonProxiableT,
         *,
         evict: bool = False,
         lifetime: Lifetime | None = None,
         serializer: SerializerT | None = None,
         deserializer: DeserializerT | None = None,
-        populate_target: bool = False,
+        populate_target: bool | None = None,
         skip_nonproxiable: bool = True,
         **kwargs: Any,
     ) -> ProxyLocker[T] | NonProxiableT:
         """Proxy an object and return [`ProxyLocker`][proxystore.proxy.ProxyLocker].
 
         Args:
             obj: The object to place in store and return a proxy for.
@@ -854,20 +920,23 @@
             lifetime: Attach the proxy to this lifetime. The object associated
                 with the proxy will be evicted when the lifetime ends.
                 Mutually exclusive with the `evict` parameter.
             serializer: Optionally override the default serializer for the
                 store instance.
             deserializer: Optionally override the default deserializer for the
                 store instance.
-            populate_target: Set the returned proxy to point at `obj`. I.e.,
-                return an already resolved proxy. This is `False` by default
-                because the returned proxy will hold a reference to `obj`
-                which will prevent garbage collecting `obj`. Setting this flag
-                is helpful when serializing the returned proxy on this process
-                will incidentally resolve the proxy.
+            populate_target: Pass `cache_defaults=True` and `target=obj` to
+                the [`Proxy`][proxystore.proxy.Proxy] constructor. I.e.,
+                return a proxy that (1) is already resolved, (2) can be used
+                in [`isinstance`][isinstance] checks without resolving, and (3)
+                is hashable without resolving if `obj` is a hashable type.
+                This is `False` by default because the returned proxy will
+                hold a reference to `obj` which will prevent garbage
+                collecting `obj`. If `None`, defaults to the store-wide
+                setting.
             skip_nonproxiable: Return non-proxiable types (e.g., built-in
                 constants like `bool` or `None`) rather than raising a
                 [`NonProxiableTypeError`][proxystore.store.exceptions.NonProxiableTypeError].
             kwargs: Additional keyword arguments to pass to
                 [`Connector.put()`][proxystore.connectors.protocols.Connector.put].
 
         Returns:
@@ -902,38 +971,38 @@
     @overload
     def owned_proxy(  # type: ignore[overload-overlap]
         self,
         obj: NonProxiableT,
         *,
         serializer: SerializerT | None = ...,
         deserializer: DeserializerT | None = ...,
-        populate_target: bool = ...,
+        populate_target: bool | None = ...,
         skip_nonproxiable: Literal[True] = ...,
         **kwargs: Any,
     ) -> NonProxiableT: ...
 
     @overload
     def owned_proxy(
         self,
         obj: T,
         *,
         serializer: SerializerT | None = ...,
         deserializer: DeserializerT | None = ...,
-        populate_target: bool = ...,
+        populate_target: bool | None = ...,
         skip_nonproxiable: bool = ...,
         **kwargs: Any,
     ) -> OwnedProxy[T]: ...
 
     def owned_proxy(
         self,
         obj: T | NonProxiableT,
         *,
         serializer: SerializerT | None = None,
         deserializer: DeserializerT | None = None,
-        populate_target: bool = False,
+        populate_target: bool | None = None,
         skip_nonproxiable: bool = True,
         **kwargs: Any,
     ) -> OwnedProxy[T] | NonProxiableT:
         """Create a proxy that will enforce ownership rules over the object.
 
         An [`OwnedProxy`][proxystore.store.ref.OwnedProxy] will auto-evict
         the object once it goes out of scope. This proxy type can also
@@ -941,20 +1010,23 @@
 
         Args:
             obj: The object to place in store and return a proxy for.
             serializer: Optionally override the default serializer for the
                 store instance.
             deserializer: Optionally override the default deserializer for the
                 store instance.
-            populate_target: Set the returned proxy to point at `obj`. I.e.,
-                return an already resolved proxy. This is `False` by default
-                because the returned proxy will hold a reference to `obj`
-                which will prevent garbage collecting `obj`. Setting this flag
-                is helpful when serializing the returned proxy on this process
-                will incidentally resolve the proxy.
+            populate_target: Pass `cache_defaults=True` and `target=obj` to
+                the [`Proxy`][proxystore.proxy.Proxy] constructor. I.e.,
+                return a proxy that (1) is already resolved, (2) can be used
+                in [`isinstance`][isinstance] checks without resolving, and (3)
+                is hashable without resolving if `obj` is a hashable type.
+                This is `False` by default because the returned proxy will
+                hold a reference to `obj` which will prevent garbage
+                collecting `obj`. If `None`, defaults to the store-wide
+                setting.
             skip_nonproxiable: Return non-proxiable types (e.g., built-in
                 constants like `bool` or `None`) rather than raising a
                 [`NonProxiableTypeError`][proxystore.store.exceptions.NonProxiableTypeError].
             kwargs: Additional keyword arguments to pass to
                 [`Connector.put()`][proxystore.connectors.protocols.Connector.put].
 
         Returns:
@@ -974,15 +1046,20 @@
             deserializer=deserializer,
             populate_target=populate_target,
             skip_nonproxiable=skip_nonproxiable,
             **kwargs,
         )
 
         if isinstance(possible_proxy, Proxy):
-            return into_owned(possible_proxy)
+            populate_target = (
+                self._populate_target
+                if populate_target is None
+                else populate_target
+            )
+            return into_owned(possible_proxy, populate_target=populate_target)
         return possible_proxy
 
     def put(
         self,
         obj: Any,
         *,
         lifetime: Lifetime | None = None,
@@ -1018,24 +1095,24 @@
         if not isinstance(obj, bytes):
             raise TypeError('Serializer must produce bytes.')
 
         with Timer() as connector_timer:
             key = self.connector.put(obj, **kwargs)
 
         if lifetime is not None:
-            lifetime.add_key(key)
+            lifetime.add_key(key, store=self)
 
         timer.stop()
         if self.metrics is not None:
-            ctime = connector_timer.elapsed_ns
-            stime = serialize_timer.elapsed_ns
+            ctime = connector_timer.elapsed_ms
+            stime = serialize_timer.elapsed_ms
             self.metrics.add_attribute('store.put.object_size', key, len(obj))
             self.metrics.add_time('store.put.serialize', key, stime)
             self.metrics.add_time('store.put.connector', key, ctime)
-            self.metrics.add_time('store.put', key, timer.elapsed_ns)
+            self.metrics.add_time('store.put', key, timer.elapsed_ms)
 
         logger.debug(
             f'Store(name="{self.name}"): PUT {key} in '
             f'{timer.elapsed_ms:.3f} ms',
         )
         return key
 
@@ -1081,29 +1158,29 @@
         with Timer() as serialize_timer:
             _objs = list(map(_serialize, objs))
 
         with Timer() as connector_timer:
             keys = self.connector.put_batch(_objs, **kwargs)
 
         if lifetime is not None:
-            lifetime.add_key(*keys)
+            lifetime.add_key(*keys, store=self)
 
         timer.stop()
         if self.metrics is not None:
-            ctime = connector_timer.elapsed_ns
-            stime = serialize_timer.elapsed_ns
+            ctime = connector_timer.elapsed_ms
+            stime = serialize_timer.elapsed_ms
             sizes = sum(len(obj) for obj in _objs)
             self.metrics.add_attribute(
                 'store.put_batch.object_sizes',
                 keys,
                 sizes,
             )
             self.metrics.add_time('store.put_batch.serialize', keys, stime)
             self.metrics.add_time('store.put_batch.connector', keys, ctime)
-            self.metrics.add_time('store.put_batch', keys, timer.elapsed_ns)
+            self.metrics.add_time('store.put_batch', keys, timer.elapsed_ms)
 
         logger.debug(
             f'Store(name="{self.name}"): PUT_BATCH ({len(keys)} items) in '
             f'{timer.elapsed_ms:.3f} ms',
         )
         return keys
 
@@ -1166,18 +1243,18 @@
         with Timer() as connector_timer:
             self.connector.set(key, obj, **kwargs)
 
         self.cache.evict(key)
 
         timer.stop()
         if self.metrics is not None:
-            ctime = connector_timer.elapsed_ns
-            stime = serialize_timer.elapsed_ns
+            ctime = connector_timer.elapsed_ms
+            stime = serialize_timer.elapsed_ms
             self.metrics.add_attribute('store.set.object_size', key, len(obj))
             self.metrics.add_time('store.set.serialize', key, stime)
             self.metrics.add_time('store.set.connector', key, ctime)
-            self.metrics.add_time('store.set', key, timer.elapsed_ns)
+            self.metrics.add_time('store.set', key, timer.elapsed_ms)
 
         logger.debug(
             f'Store(name="{self.name}"): SET {key} in '
             f'{timer.elapsed_ms:.3f} ms',
         )
```

### Comparing `proxystore-0.6.4/proxystore/store/cache.py` & `proxystore-0.6.5/proxystore/store/cache.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/store/exceptions.py` & `proxystore-0.6.5/proxystore/store/exceptions.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/store/factory.py` & `proxystore-0.6.5/proxystore/store/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 """Factory implementations."""
 
 from __future__ import annotations
 
 import logging
-import threading
 import time
 from concurrent.futures import Future
 from concurrent.futures import ThreadPoolExecutor
 from typing import Any
 from typing import cast
 from typing import Generic
 from typing import TYPE_CHECKING
 from typing import TypeVar
 
 import proxystore
 from proxystore.store.exceptions import ProxyResolveMissingKeyError
 from proxystore.store.types import ConnectorKeyT
 from proxystore.store.types import ConnectorT
 from proxystore.store.types import DeserializerT
+from proxystore.store.types import StoreConfig
 from proxystore.utils.timer import Timer
 
 if TYPE_CHECKING:
     from proxystore.store.base import Store
 
 logger = logging.getLogger(__name__)
 
 _default_pool = ThreadPoolExecutor()
-_factory_get_store_lock = threading.Lock()
 _MISSING_OBJECT = object()
 
 T = TypeVar('T')
 
 
 class StoreFactory(Generic[ConnectorT, T]):
     """Factory that resolves an object from a store.
@@ -53,15 +52,15 @@
             If `None`, the default deserializer
             ([`deserialize()`][proxystore.serialize.deserialize]) will be used.
     """
 
     def __init__(
         self,
         key: ConnectorKeyT,
-        store_config: dict[str, Any],
+        store_config: StoreConfig,
         *,
         evict: bool = False,
         deserializer: DeserializerT | None = None,
     ) -> None:
         self.key = key
         self.store_config = store_config
         self.evict = evict
@@ -91,26 +90,19 @@
         state['_obj_future'] = None
         return state
 
     def __setstate__(self, state: dict[str, Any]) -> None:
         self.__dict__.update(state)
 
     def get_store(self) -> Store[ConnectorT]:
-        """Get store and reinitialize if necessary.
-
-        Raises:
-            ValueError: If the type of the returned store does not match the
-                expected store type passed to the factory constructor.
-        """
-        with _factory_get_store_lock:
-            store = proxystore.store.get_store(self.store_config['name'])
-            if store is None:
-                store = proxystore.store.Store.from_config(self.store_config)
-                proxystore.store.register_store(store)
-            return store
+        """Get store and reinitialize if necessary."""
+        return proxystore.store.get_or_create_store(
+            self.store_config,
+            register=True,
+        )
 
     def resolve(self) -> T:
         """Get object associated with key from store.
 
         Raises:
             ProxyResolveMissingKeyError: If the key associated with this
                 factory does not exist in the store.
@@ -173,15 +165,15 @@
         polling_timeout: Optional maximum number of seconds to poll for. If
             the timeout is reached an error is raised.
     """
 
     def __init__(
         self,
         key: ConnectorKeyT,
-        store_config: dict[str, Any],
+        store_config: StoreConfig,
         *,
         deserializer: DeserializerT | None = None,
         evict: bool = False,
         polling_interval: float = 1,
         polling_backoff_factor: float = 1,
         polling_interval_limit: float | None = None,
         polling_timeout: float | None = None,
```

### Comparing `proxystore-0.6.4/proxystore/store/future.py` & `proxystore-0.6.5/proxystore/store/future.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/store/lifetimes.py` & `proxystore-0.6.5/proxystore/store/lifetimes.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import atexit
 import functools
 import logging
 import sys
 import threading
 import time
 import uuid
+from collections import defaultdict
 from datetime import datetime
 from datetime import timedelta
 from types import TracebackType
 from typing import Any
 from typing import Callable
 from typing import Protocol
 from typing import runtime_checkable
@@ -31,48 +32,46 @@
     from typing_extensions import ParamSpec
 
 if sys.version_info >= (3, 11):  # pragma: >=3.11 cover
     from typing import Self
 else:  # pragma: <3.11 cover
     from typing_extensions import Self
 
+from proxystore.proxy import get_factory
 from proxystore.proxy import Proxy
 from proxystore.store.exceptions import ProxyStoreFactoryError
 from proxystore.store.factory import StoreFactory
 from proxystore.store.types import ConnectorKeyT
 
 if TYPE_CHECKING:
     from proxystore.store.base import Store
 
 logger = logging.getLogger(__name__)
 
 
 @runtime_checkable
 class Lifetime(Protocol):
-    """Lifetime protocol.
+    """Lifetime protocol."""
 
-    Attributes:
-        store: [`Store`][proxystore.store.base.Store] instance use to create
-            the objects associated with this lifetime and that will be used
-            to evict them when the lifetime has ended.
-    """
-
-    name: str
-    store: Store[Any]
-
-    def add_key(self, *keys: ConnectorKeyT) -> None:
+    def add_key(
+        self,
+        *keys: ConnectorKeyT,
+        store: Store[Any] | None = None,
+    ) -> None:
         """Associate a new object with the lifetime.
 
         Warning:
             All keys should have been created by the same
             [`Store`][proxystore.store.base.Store] that this lifetime was
             initialized with.
 
         Args:
             keys: One or more keys of objects to associate with this lifetime.
+            store: Optional [`Store`][proxystore.store.base.Store] that `keys`
+                belongs to.
         """
         ...
 
     def add_proxy(self, *proxies: Proxy[Any]) -> None:
         """Associate a new object with the lifetime.
 
         Warning:
@@ -86,16 +85,21 @@
 
         Raises:
             ProxyStoreFactoryError: If the proxy's factory is not an instance
                 of [`StoreFactory`][proxystore.store.base.StoreFactory].
         """
         ...
 
-    def close(self) -> None:
-        """End the lifetime and evict all associated objects."""
+    def close(self, *, close_stores: bool = False) -> None:
+        """End the lifetime and evict all associated objects.
+
+        Args:
+            close_stores: Close any [`Store`][proxystore.store.base.Store]
+                store instances associated with the lifetime.
+        """
         ...
 
     def done(self) -> bool:
         """Check if lifetime has ended."""
         ...
 
 
@@ -168,25 +172,34 @@
         self,
         exc_type: type[BaseException] | None,
         exc_value: BaseException | None,
         exc_traceback: TracebackType | None,
     ) -> None:
         self.close()
 
+    def __repr__(self) -> str:
+        return f'Lifetime(name={self.name}, store={self.store!r})'
+
     @_error_if_done
-    def add_key(self, *keys: ConnectorKeyT) -> None:
+    def add_key(
+        self,
+        *keys: ConnectorKeyT,
+        store: Store[Any] | None = None,
+    ) -> None:
         """Associate a new object with the lifetime.
 
         Warning:
             All keys should have been created by the same
             [`Store`][proxystore.store.base.Store] that this lifetime was
             initialized with.
 
         Args:
             keys: One or more keys of objects to associate with this lifetime.
+            store: Optional [`Store`][proxystore.store.base.Store] that `keys`
+                belongs to. Ignored by this implementation.
 
         Raises:
             RuntimeError: If this lifetime has ended.
         """
         self._keys.update(keys)
         logger.debug(
             f'Added keys to lifetime manager (name={self.name}): '
@@ -209,39 +222,47 @@
         Raises:
             ProxyStoreFactoryError: If the proxy's factory is not an instance
                 of [`StoreFactory`][proxystore.store.base.StoreFactory].
             RuntimeError: If this lifetime has ended.
         """
         keys: list[ConnectorKeyT] = []
         for proxy in proxies:
-            factory = proxy.__factory__
+            factory = get_factory(proxy)
             if isinstance(factory, StoreFactory):
                 keys.append(factory.key)
             else:
                 raise ProxyStoreFactoryError(
                     'The proxy must contain a factory with type '
                     f'{type(StoreFactory).__name__}. {type(factory).__name__} '
                     'is not supported.',
                 )
         self.add_key(*keys)
 
-    def close(self) -> None:
-        """End the lifetime and evict all associated objects."""
+    def close(self, *, close_stores: bool = False) -> None:
+        """End the lifetime and evict all associated objects.
+
+        Args:
+            close_stores: Close any [`Store`][proxystore.store.base.Store]
+                store instances associated with the lifetime.
+        """
         if self.done():
             return
 
         for key in self._keys:
             self.store.evict(key)
         self._done = True
         logger.info(
             f'Closed lifetime manager and evicted {len(self._keys)} '
             f'associated objects (name={self.name})',
         )
         self._keys.clear()
 
+        if close_stores:
+            self.store.close()
+
     def done(self) -> bool:
         """Check if lifetime has ended."""
         return self._done
 
 
 class LeaseLifetime(ContextLifetime):
     """Time-based lease lifetime manager.
@@ -316,25 +337,29 @@
             # Excluded from coverage for the same reason as in
             # _timer_callback().
             self._timer.cancel()
         interval = max(0, self._expiry - time.time())
         self._timer = threading.Timer(interval, self._timer_callback)
         self._timer.start()
 
-    def close(self) -> None:
+    def close(self, *, close_stores: bool = False) -> None:
         """End the lifetime and evict all associated objects.
 
         This can be called before the specified expiry time to end the
         lifetime early.
+
+        Args:
+            close_stores: Close any [`Store`][proxystore.store.base.Store]
+                store instances associated with the lifetime.
         """
         if self._timer is not None:
             self._timer.cancel()
             self._timer = None
 
-        super().close()
+        super().close(close_stores=close_stores)
 
     @_error_if_done
     def extend(self, expiry: datetime | timedelta | float) -> None:
         """Extend the expiry of the lifetime lease.
 
         Args:
             expiry: Extends the current expiry if the value is
@@ -349,17 +374,166 @@
             self._expiry += expiry.total_seconds()
         elif isinstance(expiry, (int, float)):
             self._expiry += expiry
         else:
             raise AssertionError('Unreachable.')
 
 
+class StaticLifetime:
+    """Static lifetime manager.
+
+    Keeps associated objects alive for the remainder of the program.
+
+    Note:
+        This is a singleton class.
+
+    Warning:
+        This class registers an [atexit][atexit] handler which will close
+        the lifetime at the end of the program, evicting all objects associated
+        with the lifetime. Therefore, [`Store`][proxystore.store.base.Store]
+        instances used to created objects associated with the static lifetime
+        **should not** be closed prior to program exit. The handler will close
+        all of these stores. It is possible to call `StaticLifetime().close()`
+        manually, after which it is safe to also close the stores.
+
+    Example:
+        ```python linenums="1" title="Static Lifetime"
+        from proxystore.connectors.local import LocalConnector
+        from proxystore.store import Store
+        from proxystore.store.lifetimes import StaticLifetime
+
+        store = Store('default', LocalConnector(), register=True)  # (1)!
+
+        key = store.put('value', lifetime=StaticLifetime())  # (2)!
+        proxy = store.proxy('value', lifetime=StaticLifetime())  # (3)!
+        ```
+
+        1. The atexit handler will call `store.close()` at the end of the
+           program. Setting `register=True` is recommended to prevent another
+           instance being created internally when a proxy is resolved.
+        3. The object associated with `key` will be evicted at the end of
+           the program.
+        4. The object associated with `proxy` will be evicted at the end of
+           the program.
+    """
+
+    _instance: StaticLifetime | None = None
+    name = 'static'
+
+    def __new__(cls) -> StaticLifetime:
+        if cls._instance is None:
+            cls._instance = super().__new__(cls)
+            cls._initialized = False
+        return cls._instance
+
+    def __init__(self) -> None:
+        if not self._initialized:
+            self._done = False
+            self._keys: dict[Store[Any], set[ConnectorKeyT]] = defaultdict(set)
+            self._callback = register_lifetime_atexit(self, close_stores=True)
+            self._initialized = True
+
+    @_error_if_done
+    def add_key(
+        self,
+        *keys: ConnectorKeyT,
+        store: Store[Any] | None = None,
+    ) -> None:
+        """Associate a new object with the lifetime.
+
+        Args:
+            keys: One or more keys of objects to associate with this lifetime.
+            store: [`Store`][proxystore.store.base.Store] that `keys`
+                belongs to. Required by this implementation.
+
+        Raises:
+            RuntimeError: If this lifetime has ended.
+            ValueError: If `store` is `None`.
+        """
+        if store is None:
+            raise ValueError(
+                f'The {self.__class__.__name__} requires the store parameter.',
+            )
+        self._keys[store].update(keys)
+        logger.debug(
+            f'Added keys to lifetime manager (name={self.name}): '
+            f'{", ".join(repr(key) for key in keys)}',
+        )
+
+    @_error_if_done
+    def add_proxy(self, *proxies: Proxy[Any]) -> None:
+        """Associate a new object with the lifetime.
+
+        Warning:
+            This method will initialized new
+            [`Store`][proxystore.store.base.Store] instances if the stores
+            which were used to create the input proxies have not been
+            registered by setting the `register` flag or by calling
+            [`register_store()`][proxystore.store.register_store].
+
+        Args:
+            proxies: One or more proxies of objects to associate with this
+                lifetime.
+
+        Raises:
+            ProxyStoreFactoryError: If the proxy's factory is not an instance
+                of [`StoreFactory`][proxystore.store.base.StoreFactory].
+            RuntimeError: If this lifetime has ended.
+        """
+        for proxy in proxies:
+            factory = get_factory(proxy)
+            if isinstance(factory, StoreFactory):
+                self.add_key(factory.key, store=factory.get_store())
+            else:
+                raise ProxyStoreFactoryError(
+                    'The proxy must contain a factory with type '
+                    f'{type(StoreFactory).__name__}. {type(factory).__name__} '
+                    'is not supported.',
+                )
+
+    def close(self, *, close_stores: bool = False) -> None:
+        """End the lifetime and evict all associated objects.
+
+        Warning:
+            Because this class is a singleton this operation can only
+            be performed once.
+
+        Args:
+            close_stores: Close any [`Store`][proxystore.store.base.Store]
+                store instances associated with the lifetime.
+        """
+        if self.done():
+            return
+
+        count = 0
+        for store, keys in self._keys.items():
+            for key in keys:
+                store.evict(key)
+                count += 1
+
+            if close_stores:
+                store.close()
+
+        atexit.unregister(self._callback)
+
+        self._done = True
+        logger.info(
+            f'Closed lifetime manager and evicted {count} '
+            f'associated objects (name={self.name})',
+        )
+        self._keys.clear()
+
+    def done(self) -> bool:
+        """Check if lifetime has ended."""
+        return self._done
+
+
 def register_lifetime_atexit(
     lifetime: Lifetime,
-    close_store: bool = True,
+    close_stores: bool = True,
 ) -> Callable[[], None]:
     """Register atexit callback to cleanup the lifetime.
 
     Registers an atexit callback which will close the lifetime on normal
     program exit and optionally close the associated store as well.
 
     Tip:
@@ -371,26 +545,23 @@
 
     Warning:
         Callbacks are not guaranteed to be called in all cases. See the
         [`atexit`][atexit] docs for more details.
 
     Args:
         lifetime: Lifetime to be closed at exit.
-        close_store: Close the [`Store`][proxystore.store.base.Store] after
-            the lifetime.
+        close_stores: Close any [`Store`][proxystore.store.base.Store]
+            instances associated with the lifetime.
 
     Returns:
         The registered callback function which can be used with \
         [`atexit.unregister()`][atexit.unregister] if needed.
     """
 
     def _lifetime_atexit_callback() -> None:
-        lifetime.close()
-        if close_store:
-            lifetime.store.close()
+        lifetime.close(close_stores=close_stores)
 
     atexit.register(_lifetime_atexit_callback)
     logger.debug(
-        'Registered atexit callback for lifetime '
-        f'(lifetime: {lifetime.name}, store: {lifetime.store.name})',
+        f'Registered atexit callback for {lifetime!r}',
     )
     return _lifetime_atexit_callback
```

### Comparing `proxystore-0.6.4/proxystore/store/metrics.py` & `proxystore-0.6.5/proxystore/store/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,26 +144,26 @@
         """
         counters = self._metrics[_hash_key(key)].counters
         if name in counters:
             counters[name] += value
         else:
             counters[name] = value
 
-    def add_time(self, name: str, key: KeyT, time_ns: int) -> None:
+    def add_time(self, name: str, key: KeyT, time_ms: float) -> None:
         """Record a new time for an event.
 
         Args:
             name: Event or operation the time is for.
             key: Key associated with the event.
-            time_ns: The time in nanoseconds of the event.
+            time_ms: The time in milliseconds of the event.
         """
         times = self._metrics[_hash_key(key)].times
         if name not in times:
             times[name] = TimeStats()
-        times[name].add_time(time_ns / 1000)
+        times[name].add_time(time_ms)
 
     def aggregate_times(self) -> dict[str, TimeStats]:
         """Aggregate time statistics over all keys.
 
         Returns:
             Dictionary mapping event names to the time statistics aggregated \
             for that event.
```

### Comparing `proxystore-0.6.4/proxystore/store/ref.py` & `proxystore-0.6.5/proxystore/store/ref.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 of `T`, forwarding operations on themselves to a locally cached instance of
 `T`.
 """
 
 from __future__ import annotations
 
 import atexit
+import copy
 import sys
 import weakref
 from typing import Any
 from typing import Callable
 from typing import NoReturn
 from typing import SupportsIndex
 from typing import TypeVar
@@ -55,14 +56,15 @@
 if sys.version_info >= (3, 10):  # pragma: >=3.10 cover
     from typing import TypeAlias
 else:  # pragma: <3.10 cover
     from typing_extensions import TypeAlias
 
 from proxystore.proxy import is_resolved
 from proxystore.proxy import Proxy
+from proxystore.store.exceptions import ProxyStoreFactoryError
 from proxystore.store.factory import StoreFactory
 from proxystore.store.types import SerializerT
 
 T = TypeVar('T')
 FactoryType: TypeAlias = StoreFactory[Any, T]
 
 
@@ -112,34 +114,45 @@
        when accessing the wrapped target object.
     2. Disable [`copy()`][copy.copy] and [`deepcopy()`][copy.deepcopy]
        support to prevent misuse of the API. Generally,
        [`borrow()`][proxystore.store.ref.borrow] or
        [`clone()`][proxystore.store.ref.clone] should be used instead.
     """
 
-    def __init__(self, factory: FactoryType[T]) -> None:
-        object.__setattr__(self, '__valid__', True)
-        super().__init__(factory)
+    __slots__ = '__proxy_valid__'
+
+    __proxy_factory__: FactoryType[T]
+    __proxy_valid__: bool
+
+    def __init__(
+        self,
+        factory: FactoryType[T],
+        *,
+        cache_defaults: bool = False,
+        target: T | None = None,
+    ) -> None:
+        object.__setattr__(self, '__proxy_valid__', True)
+        super().__init__(factory, cache_defaults=cache_defaults, target=target)
 
     @property
-    def __wrapped__(self) -> T:
-        if not object.__getattribute__(self, '__valid__'):
+    def __proxy_wrapped__(self) -> T:
+        if not object.__getattribute__(self, '__proxy_valid__'):
             raise ReferenceInvalidError(
                 'Reference has been invalidated. This is likely because it '
                 'was pickled and transferred to a different process.',
             )
-        return super().__wrapped__
+        return super().__proxy_wrapped__
 
-    @__wrapped__.deleter
-    def __wrapped__(self) -> None:
-        object.__delattr__(self, '__target__')
-
-    @__wrapped__.setter
-    def __wrapped__(self, target: T) -> None:
-        object.__setattr__(self, '__target__', target)
+    @__proxy_wrapped__.deleter
+    def __proxy_wrapped__(self) -> None:
+        object.__delattr__(self, '__proxy_target__')
+
+    @__proxy_wrapped__.setter
+    def __proxy_wrapped__(self, target: T) -> None:
+        object.__setattr__(self, '__proxy_target__', target)
 
     def __copy__(self) -> NoReturn:
         raise NotImplementedError(
             'Copy is not implemented for reference proxy types to avoid '
             'incidental misuse of the API. Use clone() instead.',
         )
 
@@ -162,51 +175,74 @@
     mutable borrows of this proxy. The target object will be evicted from
     the store once this proxy goes out of scope (this is handled via
     `__del__` and an [atexit][atexit] handler).
 
     Args:
         factory: [`StoreFactory`][proxystore.store.factory.StoreFactory] used
             to resolve the target object from the store.
+        cache_defaults: Precompute and cache the `__proxy_default_class__` and
+            `__proxy_default_hash__` attributes of the proxy instance from
+            `target`. Ignored if `target` is not provided.
+        target: Optionally preset the target object.
     """
 
-    def __init__(self, factory: FactoryType[T]) -> None:
-        object.__setattr__(self, '__ref_count__', 0)
-        object.__setattr__(self, '__ref_mut_count__', 0)
+    __slots__ = (
+        '__proxy_ref_count__',
+        '__proxy_ref_mut_count__',
+        '__proxy_finalizer__',
+    )
+
+    __proxy_ref_count__: int
+    __proxy_ref_mut_count__: int
+    __proxy_finalizer__: Any
+
+    def __init__(
+        self,
+        factory: FactoryType[T],
+        *,
+        cache_defaults: bool = False,
+        target: T | None = None,
+    ) -> None:
+        object.__setattr__(self, '__proxy_ref_count__', 0)
+        object.__setattr__(self, '__proxy_ref_mut_count__', 0)
         object.__setattr__(
             self,
-            '__finalizer__',
+            '__proxy_finalizer__',
             atexit.register(_WeakRefFinalizer(self, '__del__')),
         )
-        super().__init__(factory)
+        super().__init__(factory, cache_defaults=cache_defaults, target=target)
 
     def __del__(self) -> None:
-        atexit.unregister(object.__getattribute__(self, '__finalizer__'))
-        if object.__getattribute__(self, '__valid__'):
-            ref_count = object.__getattribute__(self, '__ref_count__')
-            ref_mut_count = object.__getattribute__(self, '__ref_mut_count__')
+        atexit.unregister(object.__getattribute__(self, '__proxy_finalizer__'))
+        if object.__getattribute__(self, '__proxy_valid__'):
+            ref_count = object.__getattribute__(self, '__proxy_ref_count__')
+            ref_mut_count = object.__getattribute__(
+                self,
+                '__proxy_ref_mut_count__',
+            )
             if ref_count > 0 or ref_mut_count > 0:
                 raise RuntimeError(
                     'Cannot safely delete OwnedProxy because there still '
                     f'exists {ref_count} RefProxy and {ref_mut_count} '
                     'RefMutProxy.',
                 )
-            factory = object.__getattribute__(self, '__factory__')
+            factory = object.__getattribute__(self, '__proxy_factory__')
             store = factory.get_store()
             store.evict(factory.key)
-            object.__setattr__(self, '__valid__', False)
+            object.__setattr__(self, '__proxy_valid__', False)
 
     def __reduce__(  # type: ignore[override]
         self,
     ) -> tuple[
         Callable[[FactoryType[T]], OwnedProxy[T]],
         tuple[FactoryType[T]],
     ]:
-        object.__setattr__(self, '__valid__', False)
+        object.__setattr__(self, '__proxy_valid__', False)
         return _owned_proxy_trampoline, (
-            object.__getattribute__(self, '__factory__'),
+            object.__getattribute__(self, '__proxy_factory__'),
         )
 
     def __reduce_ex__(  # type: ignore[override]
         self,
         protocol: SupportsIndex,
     ) -> tuple[
         Callable[[FactoryType[T]], OwnedProxy[T]],
@@ -222,54 +258,65 @@
 
 class RefProxy(BaseRefProxy[T]):
     """Represents a borrowed reference to an object in the global store.
 
     Args:
         factory: [`StoreFactory`][proxystore.store.factory.StoreFactory] used
             to resolve the target object from the store.
+        cache_defaults: Precompute and cache the `__proxy_default_class__` and
+            `__proxy_default_hash__` attributes of the proxy instance from
+            `target`. Ignored if `target` is not provided.
         owner: Proxy which has ownership over the target object. This reference
             will keep the owner alive while this borrowed reference is alive.
             In the event this borrowed reference was initialized in a different
             address space from the proxy with ownership, then `owner` will
             be `None`.
+        target: Optionally preset the target object.
     """
 
+    __slots__ = ('__proxy_finalizer__', '__proxy_owner__')
+
+    __proxy_finalizer__: Any
+    __proxy_owner__: OwnedProxy[T]
+
     def __init__(
         self,
         factory: FactoryType[T],
         *,
+        cache_defaults: bool = False,
         owner: OwnedProxy[T] | None = None,
+        target: T | None = None,
     ) -> None:
-        object.__setattr__(self, '__owner__', owner)
+        object.__setattr__(self, '__proxy_owner__', owner)
         object.__setattr__(
             self,
-            '__finalizer__',
+            '__proxy_finalizer__',
             atexit.register(_WeakRefFinalizer(self, '__del__')),
         )
-        super().__init__(factory)
+        super().__init__(factory, cache_defaults=cache_defaults, target=target)
 
     def __del__(self) -> None:
-        atexit.unregister(object.__getattribute__(self, '__finalizer__'))
+        atexit.unregister(object.__getattribute__(self, '__proxy_finalizer__'))
         # If owner is None, then this RefMutProxy was likely serialized
         # and sent to a different process. As such, it is the responsibility
         # of that code to take over reference counting.
-        owner = object.__getattribute__(self, '__owner__')
+        owner = object.__getattribute__(self, '__proxy_owner__')
         if owner is not None:
-            ref_count = object.__getattribute__(owner, '__ref_count__')
+            ref_count = object.__getattribute__(owner, '__proxy_ref_count__')
             assert ref_count >= 1
-            object.__setattr__(owner, '__ref_count__', ref_count - 1)
-        object.__setattr__(self, '__owner__', None)
-        object.__setattr__(self, '__valid__', False)
+            object.__setattr__(owner, '__proxy_ref_count__', ref_count - 1)
+        object.__setattr__(self, '__proxy_owner__', None)
+        object.__setattr__(self, '__proxy_valid__', False)
 
     def __reduce__(  # type: ignore[override]
         self,
     ) -> tuple[Callable[[FactoryType[T]], RefProxy[T]], tuple[FactoryType[T]]]:
-        object.__setattr__(self, '__valid__', False)
+        object.__setattr__(self, '__proxy_valid__', False)
         return _ref_proxy_trampoline, (
-            object.__getattribute__(self, '__factory__'),
+            object.__getattribute__(self, '__proxy_factory__'),
         )
 
     def __reduce_ex__(  # type: ignore[override]
         self,
         protocol: SupportsIndex,
     ) -> tuple[Callable[[FactoryType[T]], RefProxy[T]], tuple[FactoryType[T]]]:
         return self.__reduce__()
@@ -282,72 +329,102 @@
 
 class RefMutProxy(BaseRefProxy[T]):
     """Represents a borrowed mutable reference to an object in the global store.
 
     Args:
         factory: [`StoreFactory`][proxystore.store.factory.StoreFactory] used
             to resolve the target object from the store.
+        cache_defaults: Precompute and cache the `__proxy_default_class__` and
+            `__proxy_default_hash__` attributes of the proxy instance from
+            `target`. Ignored if `target` is not provided.
         owner: Proxy which has ownership over the target object. This reference
             will keep the owner alive while this borrowed reference is alive.
             In the event this borrowed reference was initialized in a different
             address space from the proxy with ownership, then `owner` will
             be `None`.
+        target: Optionally preset the target object.
     """  # noqa: E501
 
+    __slots__ = ('__proxy_finalizer__', '__proxy_owner__')
+
+    __proxy_finalizer__: Any
+    __proxy_owner__: OwnedProxy[T]
+
     def __init__(
         self,
         factory: FactoryType[T],
         *,
+        cache_defaults: bool = False,
         owner: OwnedProxy[T] | None = None,
+        target: T | None = None,
     ) -> None:
-        object.__setattr__(self, '__owner__', owner)
+        object.__setattr__(self, '__proxy_owner__', owner)
         object.__setattr__(
             self,
-            '__finalizer__',
+            '__proxy_finalizer__',
             atexit.register(_WeakRefFinalizer(self, '__del__')),
         )
-        super().__init__(factory)
+        super().__init__(factory, cache_defaults=cache_defaults, target=target)
 
     def __del__(self) -> None:
-        atexit.unregister(object.__getattribute__(self, '__finalizer__'))
+        atexit.unregister(object.__getattribute__(self, '__proxy_finalizer__'))
         # If owner is None, then this RefMutProxy was likely serialized
         # and sent to a different process. As such, it is the responsibility
         # of that code to take over reference counting.
-        owner = object.__getattribute__(self, '__owner__')
+        owner = object.__getattribute__(self, '__proxy_owner__')
         if owner is not None:
             ref_mut_count = object.__getattribute__(
                 owner,
-                '__ref_mut_count__',
+                '__proxy_ref_mut_count__',
             )
             assert ref_mut_count == 1
-            object.__setattr__(owner, '__ref_mut_count__', 0)
-        object.__setattr__(self, '__owner__', None)
-        object.__setattr__(self, '__valid__', False)
+            object.__setattr__(owner, '__proxy_ref_mut_count__', 0)
+        object.__setattr__(self, '__proxy_owner__', None)
+        object.__setattr__(self, '__proxy_valid__', False)
 
     def __reduce__(  # type: ignore[override]
         self,
     ) -> tuple[
         Callable[[FactoryType[T]], RefMutProxy[T]],
         tuple[FactoryType[T]],
     ]:
-        object.__setattr__(self, '__valid__', False)
+        object.__setattr__(self, '__proxy_valid__', False)
         return _ref_mut_proxy_trampoline, (
-            object.__getattribute__(self, '__factory__'),
+            object.__getattribute__(self, '__proxy_factory__'),
         )
 
     def __reduce_ex__(  # type: ignore[override]
         self,
         protocol: SupportsIndex,
     ) -> tuple[
         Callable[[FactoryType[T]], RefMutProxy[T]],
         tuple[FactoryType[T]],
     ]:
         return self.__reduce__()
 
 
+def _copy_attributes(
+    source: Proxy[T],
+    dest: Proxy[T],
+    *,
+    deepcopy: bool = False,
+) -> None:
+    if source.__proxy_resolved__:
+        target = source.__proxy_wrapped__
+        if deepcopy:
+            target = copy.deepcopy(target)
+        dest.__proxy_wrapped__ = target
+
+    default_class = object.__getattribute__(source, '__proxy_default_class__')
+    default_hash = object.__getattribute__(source, '__proxy_default_hash__')
+
+    object.__setattr__(dest, '__proxy_default_class__', default_class)
+    object.__setattr__(dest, '__proxy_default_hash__', default_hash)
+
+
 def borrow(
     proxy: OwnedProxy[T],
     *,
     populate_target: bool = True,
 ) -> RefProxy[T]:
     """Borrow `T` by creating an immutable reference of `T`.
 
@@ -363,24 +440,24 @@
     Raises:
         ReferenceNotOwnedError: if `proxy` is not an
             [`OwnedProxy`][proxystore.store.ref.OwnedProxy] instance.
         MutableBorrowError: if `proxy` has already been mutably borrowed.
     """
     if not isinstance(proxy, OwnedProxy):
         raise ReferenceNotOwnedError('Only owned references can be borrowed.')
-    if object.__getattribute__(proxy, '__ref_mut_count__') > 0:
+    if object.__getattribute__(proxy, '__proxy_ref_mut_count__') > 0:
         raise MutableBorrowError('Proxy was already borrowed as mutable.')
     object.__setattr__(
         proxy,
-        '__ref_count__',
-        object.__getattribute__(proxy, '__ref_count__') + 1,
+        '__proxy_ref_count__',
+        object.__getattribute__(proxy, '__proxy_ref_count__') + 1,
     )
-    ref_proxy = RefProxy(proxy.__factory__, owner=proxy)
-    if populate_target and is_resolved(proxy):
-        ref_proxy.__wrapped__ = proxy.__wrapped__
+    ref_proxy = RefProxy(proxy.__proxy_factory__, owner=proxy)
+    if populate_target:
+        _copy_attributes(proxy, ref_proxy)
     return ref_proxy
 
 
 def mut_borrow(
     proxy: OwnedProxy[T],
     *,
     populate_target: bool = True,
@@ -400,51 +477,55 @@
         ReferenceNotOwnedError: if `proxy` is not an
             [`OwnedProxy`][proxystore.store.ref.OwnedProxy] instance.
         MutableBorrowError: if `proxy` has already been borrowed
             (mutable/immutable).
     """
     if not isinstance(proxy, OwnedProxy):
         raise ReferenceNotOwnedError('Only owned references can be borrowed.')
-    if object.__getattribute__(proxy, '__ref_mut_count__') > 0:
+    if object.__getattribute__(proxy, '__proxy_ref_mut_count__') > 0:
         raise MutableBorrowError('Proxy was already borrowed as mutable.')
-    if object.__getattribute__(proxy, '__ref_count__') > 0:
+    if object.__getattribute__(proxy, '__proxy_ref_count__') > 0:
         raise MutableBorrowError('Proxy was already borrowed as immutable.')
     object.__setattr__(
         proxy,
-        '__ref_mut_count__',
-        object.__getattribute__(proxy, '__ref_mut_count__') + 1,
+        '__proxy_ref_mut_count__',
+        object.__getattribute__(proxy, '__proxy_ref_mut_count__') + 1,
     )
-    ref_proxy = RefMutProxy(proxy.__factory__, owner=proxy)
-    if populate_target and is_resolved(proxy):
-        ref_proxy.__wrapped__ = proxy.__wrapped__
+    ref_proxy = RefMutProxy(proxy.__proxy_factory__, owner=proxy)
+    if populate_target:
+        _copy_attributes(proxy, ref_proxy)
     return ref_proxy
 
 
 def clone(proxy: OwnedProxy[T]) -> OwnedProxy[T]:
     """Clone the target object.
 
-    Creates a new copy of `T` in the global store.
+    Creates a new copy of `T` in the global store. If `proxy` is in
+    the resolved state, the local version of `T` belonging to `proxy` will
+    be deepcopied into the cloned proxy.
 
     Raises:
         ReferenceNotOwnedError: if `proxy` is not an
             [`OwnedProxy`][proxystore.store.ref.OwnedProxy] instance.
     """
     if not isinstance(proxy, OwnedProxy):
         raise ReferenceNotOwnedError('Only owned references can be cloned.')
-    factory = proxy.__factory__
+    factory = proxy.__proxy_factory__
     store = factory.get_store()
     data = store.connector.get(factory.key)
     new_key = store.connector.put(data)
     new_factory: StoreFactory[Any, T] = StoreFactory(
         new_key,
         store_config=store.config(),
         evict=factory.evict,
         deserializer=factory.deserializer,
     )
-    return OwnedProxy(new_factory)
+    owned = OwnedProxy(new_factory)
+    _copy_attributes(proxy, owned, deepcopy=True)
+    return owned
 
 
 def into_owned(
     proxy: Proxy[T],
     *,
     populate_target: bool = True,
 ) -> OwnedProxy[T]:
@@ -462,25 +543,33 @@
         populate_target: If the target of `proxy` has already been resolved,
             copy the reference to the target into the returned proxy such that
             the returned proxy is already resolved.
 
     Raises:
         ValueError: if `proxy` is already a
             [`BaseRefProxy`][proxystore.store.ref.BaseRefProxy] instance.
+        ProxyStoreFactoryError: If the proxy's factory is not an instance of
+            [`StoreFactory`][proxystore.store.base.StoreFactory].
     """
     if type(proxy) in (OwnedProxy, RefProxy, RefMutProxy):
         # We don't use isinstance to prevent resolving the proxy.
         raise ValueError(
             'Only a base proxy can be converted into an owned proxy.',
         )
-    factory = proxy.__factory__
+    factory = proxy.__proxy_factory__
+    if not isinstance(factory, StoreFactory):
+        raise ProxyStoreFactoryError(
+            'The proxy must contain a factory with type '
+            f'{StoreFactory.__name__}. {type(factory).__name__} '
+            'is not supported.',
+        )
     factory.evict = False
     owned_proxy = OwnedProxy(factory)
-    if populate_target and is_resolved(proxy):
-        owned_proxy.__wrapped__ = proxy.__wrapped__
+    if populate_target:
+        _copy_attributes(proxy, owned_proxy)
     return owned_proxy
 
 
 def update(
     proxy: OwnedProxy[T] | RefMutProxy[T],
     *,
     serializer: SerializerT | None = None,
@@ -509,28 +598,28 @@
         ReferenceNotOwnedError: if `proxy` is not an
             [`OwnedProxy`][proxystore.store.ref.OwnedProxy] or
             [`RefMutProxy`][proxystore.store.ref.RefMutProxy] instance.
     """
     if not isinstance(proxy, (OwnedProxy, RefMutProxy)):
         raise ReferenceNotOwnedError('Reference is an immutable borrow.')
     if isinstance(proxy, OwnedProxy) and (
-        object.__getattribute__(proxy, '__ref_mut_count__') > 0
-        or object.__getattribute__(proxy, '__ref_count__') > 0
+        object.__getattribute__(proxy, '__proxy_ref_mut_count__') > 0
+        or object.__getattribute__(proxy, '__proxy_ref_count__') > 0
     ):
         raise MutableBorrowError(
             'OwnedProxy has been borrowed. Cannot mutate.',
         )
     if not is_resolved(proxy):
         return
 
-    store = proxy.__factory__.get_store()
+    store = proxy.__proxy_factory__.get_store()
     try:
         store._set(
-            proxy.__factory__.key,
-            proxy.__wrapped__,
+            proxy.__proxy_factory__.key,
+            proxy.__proxy_wrapped__,
             serializer=serializer,
         )
     except NotImplementedError as e:  # pragma: no cover
         raise NotImplementedError(
             'Mutating the global copy of the value requires a connector '
             'type that supports set().',
         ) from e
```

### Comparing `proxystore-0.6.4/proxystore/store/scopes.py` & `proxystore-0.6.5/proxystore/store/scopes.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,38 +47,41 @@
         refs: Reference proxies to mark out of scope.
 
     Raises:
         RuntimeError: if a reference proxy does not have a reference to its
             owner.
     """
     for ref in refs:
-        if not object.__getattribute__(ref, '__valid__'):
+        if not object.__getattribute__(ref, '__proxy_valid__'):
             # We've already encountered and handled this reference
             continue
-        owner = object.__getattribute__(ref, '__owner__')
+        owner = object.__getattribute__(ref, '__proxy_owner__')
         if owner is None:
             raise RuntimeError(
                 f'Cannot mark {owner!r} as out of scope because it has '
                 'no reference to its owner.',
             )
 
         if isinstance(ref, RefProxy):
-            ref_count = object.__getattribute__(owner, '__ref_count__')
-            object.__setattr__(owner, '__ref_count__', ref_count - 1)
+            ref_count = object.__getattribute__(owner, '__proxy_ref_count__')
+            object.__setattr__(owner, '__proxy_ref_count__', ref_count - 1)
         elif isinstance(ref, RefMutProxy):
-            ref_count = object.__getattribute__(owner, '__ref_mut_count__')
-            object.__setattr__(owner, '__ref_mut_count__', ref_count - 1)
+            ref_count = object.__getattribute__(
+                owner,
+                '__proxy_ref_mut_count__',
+            )
+            object.__setattr__(owner, '__proxy_ref_mut_count__', ref_count - 1)
         else:
             raise AssertionError('Unreachable.')
 
         # Remove ref's reference to owner so it no longer keeps owner alive
-        object.__setattr__(ref, '__owner__', None)
+        object.__setattr__(ref, '__proxy_owner__', None)
         # Mark ref as invalid in case the user tries to use it after it
         # has already "gone out of scope."
-        object.__setattr__(ref, '__valid__', False)
+        object.__setattr__(ref, '__proxy_valid__', False)
 
 
 def _make_out_of_scope_callback(
     refs: Iterable[RefProxy[Any] | RefMutProxy[Any]],
 ) -> Callable[[FutureWithCallback], None]:
     def _out_of_scope_callback(_fut: FutureWithCallback) -> None:
         mark_refs_out_of_scope(*refs)
```

### Comparing `proxystore-0.6.4/proxystore/store/utils.py` & `proxystore-0.6.5/proxystore/store/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 from typing import Any
 from typing import Tuple
 from typing import TypeVar
 
+from proxystore.proxy import get_factory
 from proxystore.proxy import is_resolved
 from proxystore.proxy import Proxy
 from proxystore.store import base
 from proxystore.store.exceptions import ProxyStoreFactoryError
 
 T = TypeVar('T')
 ConnectorKeyT = Tuple[Any, ...]
@@ -26,21 +27,21 @@
         The key, a NamedTuple unique to the \
         [`Store`][proxystore.store.base.Store] that created the proxy..
 
     Raises:
         ProxyStoreFactoryError: If the proxy's factory is not an instance of
             [`StoreFactory`][proxystore.store.base.StoreFactory].
     """
-    factory = proxy.__factory__
+    factory = get_factory(proxy)
     if isinstance(factory, base.StoreFactory):
         return factory.key
     else:
         raise ProxyStoreFactoryError(
             'The proxy must contain a factory with type '
-            f'{type(base.StoreFactory).__name__}. {type(factory).__name__} '
+            f'{base.StoreFactory.__name__}. {type(factory).__name__} '
             'is not supported.',
         )
 
 
 def resolve_async(proxy: Proxy[T]) -> None:
     """Begin resolving proxy asynchronously.
 
@@ -59,10 +60,22 @@
     Note:
         The asynchronous resolving functionality is implemented
         by [`StoreFactory`][proxystore.store.base.StoreFactory]. Factories that
         are not of this type will error when used with this function.
 
     Args:
         proxy: Proxy instance to begin asynchronously resolving.
+
+    Raises:
+        ProxyStoreFactoryError: If the proxy's factory is not an instance of
+            [`StoreFactory`][proxystore.store.base.StoreFactory].
     """
-    if not is_resolved(proxy):
-        proxy.__factory__.resolve_async()
+    factory = get_factory(proxy)
+    if isinstance(factory, base.StoreFactory):
+        if not is_resolved(proxy):
+            factory.resolve_async()
+    else:
+        raise ProxyStoreFactoryError(
+            'The proxy must contain a factory with type '
+            f'{base.StoreFactory.__name__}. {type(factory).__name__} '
+            'is not supported.',
+        )
```

### Comparing `proxystore-0.6.4/proxystore/stream/__init__.py` & `proxystore-0.6.5/proxystore/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/stream/events.py` & `proxystore-0.6.5/proxystore/stream/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import dataclasses
 import enum
 import json
 from typing import Any
 from typing import Union
 
+from proxystore.store.types import StoreConfig
 from proxystore.utils.imports import get_object_path
 from proxystore.utils.imports import import_from_path
 
 
 @dataclasses.dataclass
 class EndOfStreamEvent:
     """End of stream event."""
@@ -72,15 +73,15 @@
 
 @dataclasses.dataclass
 class EventBatch:
     """Batch of stream events."""
 
     events: list[Event]
     topic: str
-    store_config: dict[str, Any]
+    store_config: StoreConfig
 
     @classmethod
     def from_dict(cls, data: dict[str, Any]) -> EventBatch:
         """Create a new event instance from its dictionary representation."""
         events = [dict_to_event(d) for d in data['events']]
         return cls(
             events=events,  # type: ignore[arg-type]
```

### Comparing `proxystore-0.6.4/proxystore/stream/filters.py` & `proxystore-0.6.5/proxystore/stream/filters.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/stream/interface.py` & `proxystore-0.6.5/proxystore/stream/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     from typing_extensions import Self
 
 from proxystore.proxy import Proxy
 from proxystore.store import get_store
 from proxystore.store import register_store
 from proxystore.store import unregister_store
 from proxystore.store.base import Store
+from proxystore.store.types import StoreConfig
 from proxystore.stream.events import bytes_to_event
 from proxystore.stream.events import EndOfStreamEvent
 from proxystore.stream.events import Event
 from proxystore.stream.events import event_to_bytes
 from proxystore.stream.events import EventBatch
 from proxystore.stream.events import NewObjectEvent
 from proxystore.stream.exceptions import TopicClosedError
@@ -349,15 +350,15 @@
         if len(self._buffer[topic].objects) >= self._batch_size:
             self.flush_topic(topic)
 
 
 class _EventInfo(NamedTuple):
     event: NewObjectEvent
     topic: str
-    store_config: dict[str, Any]
+    store_config: StoreConfig
 
 
 class StreamConsumer(Generic[T]):
     """Proxy stream consumer interface.
 
     This interface acts as an iterator that will yield items from the stream
     until the stream is closed.
```

### Comparing `proxystore-0.6.4/proxystore/stream/protocols.py` & `proxystore-0.6.5/proxystore/stream/protocols.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/stream/shims/__init__.py` & `proxystore-0.6.5/proxystore/stream/shims/__init__.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/stream/shims/kafka.py` & `proxystore-0.6.5/proxystore/stream/shims/kafka.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/stream/shims/queue.py` & `proxystore-0.6.5/proxystore/stream/shims/queue.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/stream/shims/redis.py` & `proxystore-0.6.5/proxystore/stream/shims/redis.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/stream/shims/zmq.py` & `proxystore-0.6.5/proxystore/stream/shims/zmq.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/utils/config.py` & `proxystore-0.6.5/proxystore/utils/config.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/utils/counter.py` & `proxystore-0.6.5/proxystore/utils/counter.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/utils/data.py` & `proxystore-0.6.5/proxystore/utils/data.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/utils/environment.py` & `proxystore-0.6.5/proxystore/utils/environment.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/utils/imports.py` & `proxystore-0.6.5/proxystore/utils/imports.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/utils/tasks.py` & `proxystore-0.6.5/proxystore/utils/tasks.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore/utils/timer.py` & `proxystore-0.6.5/proxystore/utils/timer.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/proxystore.egg-info/PKG-INFO` & `proxystore-0.6.5/proxystore.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: proxystore
-Version: 0.6.4
+Version: 0.6.5
 Summary: Lazy object proxy interface for distributed stores.
 Author: Globus Labs
 Author-email: Greg Pauloski <jgpauloski@uchicago.edu>
 Maintainer-email: Greg Pauloski <jgpauloski@uchicago.edu>, Valerie Hayot-Sasson <vhayot@uchicago.edu>
-License: FILE
-Project-URL: homepage, https://proxystore.dev
-Project-URL: documentation, https://docs.proxystore.dev
-Project-URL: repository, https://github.com/proxystore/proxystore
+License: MIT
+Project-URL: Homepage, https://proxystore.dev
+Project-URL: Documentation, https://docs.proxystore.dev
+Project-URL: Source, https://github.com/proxystore/proxystore
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -20,15 +20,14 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click!=8.1.4
 Requires-Dist: cloudpickle>=1.6.0
 Requires-Dist: cryptography>=39.0.1
 Requires-Dist: globus-sdk>=3.3.0
-Requires-Dist: lazy-object-proxy>=1.6.0
 Requires-Dist: typing-extensions>=4.3.0
 Provides-Extra: all
 Requires-Dist: proxystore[endpoints,extensions,kafka,redis,zmq]; extra == "all"
 Provides-Extra: endpoints
 Requires-Dist: aiortc>=1.3.2; extra == "endpoints"
 Requires-Dist: aiosqlite; extra == "endpoints"
 Requires-Dist: uvicorn[standard]; extra == "endpoints"
@@ -56,14 +55,15 @@
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio>=0.23.2; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-timeout; extra == "dev"
 Requires-Dist: ruff>=0.2.0; extra == "dev"
 Requires-Dist: tox; extra == "dev"
+Requires-Dist: types-psutil; extra == "dev"
 Requires-Dist: types-redis; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: virtualenv; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: black; extra == "docs"
 Requires-Dist: mkdocs-click; extra == "docs"
 Requires-Dist: mkdocs-gen-files; extra == "docs"
@@ -76,31 +76,32 @@
 Requires-Dist: proxystore[all]; extra == "docs"
 
 # ProxyStore
 
 ![PyPI - Version](https://img.shields.io/pypi/v/proxystore)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/proxystore)
 ![GitHub License](https://img.shields.io/github/license/proxystore/proxystore)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8077899.svg)](https://doi.org/10.5281/zenodo.8077899)
 
 [![docs](https://github.com/proxystore/proxystore/actions/workflows/docs.yml/badge.svg)](https://github.com/proxystore/proxystore/actions/workflows/docs.yml)
 [![tests](https://github.com/proxystore/proxystore/actions/workflows/tests.yml/badge.svg?label=tests)](https://github.com/proxystore/proxystore/actions)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/proxystore/proxystore/main.svg)](https://results.pre-commit.ci/latest/github/proxystore/proxystore/main)
 
 ProxyStore is a library that facilitates efficient data management in distributed Python applications.
-At the core of ProxyStore is the [*proxy*](https://docs.proxystore.dev/main/concepts/proxy/) object which acts as a transparent reference to an object living in a global object store.
+At the core of ProxyStore is the [*proxy*](https://docs.proxystore.dev/latest/concepts/proxy/) object which acts as a transparent reference to an object living in a global object store.
 This pass-by-reference interface with just-in-time object resolution works across processes, machines, and sites, and enables data producers to change the low-level communication method dynamically without altering application code or behavior.
 
 ProxyStore accelerates the development of dynamic task-based workflows, serverless applications, and more by (1) decoupling control flow from data flow, (2) abstracting low-level communication mechanisms, and (3) eliminating the need for shims, wrapper functions, and boilerplate code.
 
 ProxyStore supports a diverse set of programming paradigms:
 
 * [Task-based Workflows](https://arxiv.org/abs/2303.08803)
-* [Function-as-a-Service/Serverless Applications](https://docs.proxystore.dev/main/guides/globus-compute/)
-* [Distributed Futures](https://docs.proxystore.dev/main/guides/proxy-futures/)
-* [Bulk Data Streaming](https://docs.proxystore.dev/main/guides/streaming/)
+* [Function-as-a-Service/Serverless Applications](https://docs.proxystore.dev/latest/guides/globus-compute/)
+* [Distributed Futures](https://docs.proxystore.dev/latest/guides/proxy-futures/)
+* [Bulk Data Streaming](https://docs.proxystore.dev/latest/guides/streaming/)
 * and more!
 
 ProxyStore provides support for many third-party mediated communication methods
 out-of-the-box including
 [DAOS](https://docs.daos.io/v2.4/),
 [Globus Transfer](https://www.globus.org/data-transfer),
 [Kafka](https://kafka.apache.org/),
@@ -109,15 +110,15 @@
 Custom communication methods built on
 [Mochi](https://mochi.readthedocs.io/en/latest/margo.html),
 [UCX](https://openucx.org/),
 [WebRTC](https://webrtc.org/), and
 [ZeroMQ](https://zeromq.org/)
 are provided for high-performance and peer-to-peer applications.
 
-Read more about ProxyStore's concepts [here](https://docs.proxystore.dev/main/concepts/).
+Read more about ProxyStore's concepts [here](https://docs.proxystore.dev/latest/concepts/).
 Complete documentation for ProxyStore is available at
 [docs.proxystore.dev](https://docs.proxystore.dev).
 
 ## Installation
 
 The base ProxyStore package can be installed with [`pip`](https://pip.pypa.io/en/stable/).
 ```bash
@@ -131,17 +132,17 @@
 pip install proxystore[all]
 ```
 This will also install the [`proxystore-ex`](https://extensions.proxystore.dev/)
 package which contains extension and experimental features.
 The extensions package can also be installed with `pip` using
 `proxystore[extensions]` or `proxystore-ex`.
 
-See the [Installation](https://docs.proxystore.dev/main/installation) guide
+See the [Installation](https://docs.proxystore.dev/latest/installation) guide
 for more information about the available extras installation options.
-See the [Contributing](https://docs.proxystore.dev/main/contributing) guide
+See the [Contributing](https://docs.proxystore.dev/latest/contributing) guide
 to get started for local development.
 
 ## Example
 
 Getting started with ProxyStore requires a few lines of code.
 
 ```python
@@ -162,20 +163,20 @@
     # x is resolved my-store on first use transparently to the
     # function. Then x behaves as an instance of MyDataType.
     assert isinstance(x, MyDataType)
 
 my_function(proxy)  # Succeeds
 ```
 
-Check out the [Get Started](https://docs.proxystore.dev/main/get-started)
+Check out the [Get Started](https://docs.proxystore.dev/latest/get-started)
 guide to learn more!
 
 ## Citation
 
-[![DOI](https://zenodo.org/badge/357984234.svg)](https://zenodo.org/badge/latestdoi/357984234)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8077899.svg)](https://doi.org/10.5281/zenodo.8077899)
 
 If you use ProxyStore or any of this code in your work, please cite our [SC '23 paper](https://dl.acm.org/doi/10.1145/3581784.3607047).
 ```bibtex
 @inproceedings{pauloski2023proxystore,
     author = {Pauloski, J. Gregory and Hayot-Sasson, Valerie and Ward, Logan and Hudson, Nathaniel and Sabino, Charlie and Baughman, Matt and Chard, Kyle and Foster, Ian},
     title = {{Accelerating Communications in Federated Applications with Transparent Object Proxies}},
     address = {New York, NY, USA},
```

### Comparing `proxystore-0.6.4/proxystore.egg-info/SOURCES.txt` & `proxystore-0.6.5/proxystore.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .gitignore
 .pre-commit-config.yaml
 CITATION.cff
 LICENSE
 README.md
+THIRD_PARTY_LICENSES
 mkdocs.yml
 pyproject.toml
 tox.ini
 .github/CODE_OF_CONDUCT.md
 .github/CONTRIBUTING.md
 .github/SECURITY.md
 .github/dependabot.yml
@@ -18,19 +19,19 @@
 .github/ISSUE_TEMPLATE/config.yml
 .github/workflows/cache.yml
 .github/workflows/check-docs.yml
 .github/workflows/docs.yml
 .github/workflows/publish.yml
 .github/workflows/tests.yml
 docs/examples.md
+docs/faq.md
 docs/generate_api.py
 docs/get-started.md
 docs/index.md
 docs/installation.md
-docs/known-issues.md
 docs/_overrides/base.html
 docs/_templates/python/material/function.html
 docs/_templates/python/material/module.html
 docs/_templates/python/material/docstring/admonition.html
 docs/api/cli.md
 docs/concepts/connector.md
 docs/concepts/index.md
@@ -38,14 +39,15 @@
 docs/concepts/store.md
 docs/contributing/index.md
 docs/contributing/issues-pull-requests.md
 docs/contributing/releases.md
 docs/contributing/style-guide.md
 docs/css/extra.css
 docs/css/mkdocstrings.css
+docs/guides/dask-distributed.md
 docs/guides/endpoints-debugging.md
 docs/guides/endpoints.md
 docs/guides/globus-compute.md
 docs/guides/index.md
 docs/guides/object-lifetimes.md
 docs/guides/performance.md
 docs/guides/proxy-futures.md
@@ -70,15 +72,15 @@
 examples/globus-compute/run.sh
 examples/parsl/README.md
 examples/parsl/mapreduce_parsl.py
 examples/parsl/run.sh
 proxystore/__init__.py
 proxystore/ex.py
 proxystore/factory.py
-proxystore/proxy.py
+proxystore/mypy_plugin.py
 proxystore/py.typed
 proxystore/serialize.py
 proxystore/warnings.py
 proxystore.egg-info/PKG-INFO
 proxystore.egg-info/SOURCES.txt
 proxystore.egg-info/dependency_links.txt
 proxystore.egg-info/entry_points.txt
@@ -122,14 +124,17 @@
 proxystore/p2p/relay/client.py
 proxystore/p2p/relay/config.py
 proxystore/p2p/relay/exceptions.py
 proxystore/p2p/relay/manager.py
 proxystore/p2p/relay/messages.py
 proxystore/p2p/relay/run.py
 proxystore/p2p/relay/server.py
+proxystore/proxy/__init__.py
+proxystore/proxy/_property.py
+proxystore/proxy/_utils.py
 proxystore/store/__init__.py
 proxystore/store/base.py
 proxystore/store/cache.py
 proxystore/store/exceptions.py
 proxystore/store/factory.py
 proxystore/store/future.py
 proxystore/store/lifetimes.py
@@ -176,16 +181,16 @@
 testing/scripts/peer_endpoint_bandwidth.py
 testing/scripts/peer_manager_bandwidth.py
 testing/scripts/redis_pubsub.py
 tests/__init__.py
 tests/conftest.py
 tests/ex_test.py
 tests/factory_test.py
-tests/proxy_test.py
-tests/serialization_test.py
+tests/mypy_plugin_test.py
+tests/serialize_test.py
 tests/connectors/__init__.py
 tests/connectors/connector_test.py
 tests/connectors/dim_test.py
 tests/connectors/endpoint_test.py
 tests/connectors/file_test.py
 tests/connectors/globus_test.py
 tests/connectors/local_test.py
@@ -219,14 +224,21 @@
 tests/p2p/relay/authenticate_test.py
 tests/p2p/relay/client_test.py
 tests/p2p/relay/config_test.py
 tests/p2p/relay/manager_test.py
 tests/p2p/relay/messages_test.py
 tests/p2p/relay/run_test.py
 tests/p2p/relay/server_test.py
+tests/proxy/__init__.py
+tests/proxy/property_test.py
+tests/proxy/proxy_async_test.py
+tests/proxy/proxy_container_test.py
+tests/proxy/proxy_numeric_test.py
+tests/proxy/proxy_type_test.py
+tests/proxy/proxy_utils_test.py
 tests/store/__init__.py
 tests/store/cache_test.py
 tests/store/factory_test.py
 tests/store/init_test.py
 tests/store/lifetimes_test.py
 tests/store/metrics_test.py
 tests/store/ref_test.py
```

### Comparing `proxystore-0.6.4/proxystore.egg-info/requires.txt` & `proxystore-0.6.5/proxystore.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 click!=8.1.4
 cloudpickle>=1.6.0
 cryptography>=39.0.1
 globus-sdk>=3.3.0
-lazy-object-proxy>=1.6.0
 typing-extensions>=4.3.0
 
 [all]
 proxystore[endpoints,extensions,kafka,redis,zmq]
 
 [dev]
 covdefaults>=2.2
@@ -15,14 +14,15 @@
 pre-commit
 pytest
 pytest-asyncio>=0.23.2
 pytest-cov
 pytest-timeout
 ruff>=0.2.0
 tox
+types-psutil
 types-redis
 types-requests
 virtualenv
 
 [docs]
 black
 mkdocs-click
```

### Comparing `proxystore-0.6.4/pyproject.toml` & `proxystore-0.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=64.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proxystore"
-version = "0.6.4"
+version = "0.6.5"
 authors = [
-    {name = "Globus Labs"},
     {name = "Greg Pauloski", email = "jgpauloski@uchicago.edu"},
+    {name = "Globus Labs"},
 ]
 maintainers = [
     {name = "Greg Pauloski", email = "jgpauloski@uchicago.edu"},
     {name = "Valerie Hayot-Sasson", email = "vhayot@uchicago.edu"},
 ]
 description = "Lazy object proxy interface for distributed stores."
 readme = "README.md"
 requires-python = ">=3.8"
-license = {text = "FILE"}
+license = { text = "MIT" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
@@ -29,22 +29,21 @@
 ]
 dependencies = [
     # Click 8.1.4 fails mypy: https://github.com/pallets/click/issues/2558
     "click!=8.1.4",
     "cloudpickle>=1.6.0",
     "cryptography>=39.0.1",
     "globus-sdk>=3.3.0",
-    "lazy-object-proxy>=1.6.0",
     "typing-extensions>=4.3.0",
 ]
 
 [project.urls]
-homepage = "https://proxystore.dev"
-documentation = "https://docs.proxystore.dev"
-repository = "https://github.com/proxystore/proxystore"
+Homepage = "https://proxystore.dev"
+Documentation = "https://docs.proxystore.dev"
+Source = "https://github.com/proxystore/proxystore"
 
 [project.optional-dependencies]
 all = ["proxystore[endpoints,extensions,kafka,redis,zmq]"]
 endpoints = [
     "aiortc>=1.3.2",
     "aiosqlite",
     "uvicorn[standard]",
@@ -71,14 +70,15 @@
     "pre-commit",
     "pytest",
     "pytest-asyncio>=0.23.2",
     "pytest-cov",
     "pytest-timeout",
     "ruff>=0.2.0",
     "tox",
+    "types-psutil",
     "types-redis",
     "types-requests",
     "virtualenv",
 ]
 docs = [
     "black",
     "mkdocs-click",
@@ -107,19 +107,28 @@
 dist,
 .*egg-info
 """
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
 concurrency = ["multiprocessing", "thread"]
-omit = ["version_check.py", "testing/scripts/*"]
+omit = [
+    "proxystore/mypy_plugin.py",
+    "testing/scripts/*",
+    "version_check.py",
+]
 parallel = true
 
 [tool.mypy]
 python_version = "3.10"
+plugins = [
+    "mypy.plugins.proper_plugin",
+    "proxystore/mypy_plugin.py",
+    "pydantic.mypy",
+]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 no_implicit_optional = true
 warn_redundant_casts = true
 warn_unused_configs = true
```

### Comparing `proxystore-0.6.4/testing/compat.py` & `proxystore-0.6.5/testing/compat.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/testing/connectors.py` & `proxystore-0.6.5/testing/connectors.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/testing/endpoint.py` & `proxystore-0.6.5/testing/endpoint.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/testing/mocked/globus.py` & `proxystore-0.6.5/testing/mocked/globus.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/testing/mocked/kafka.py` & `proxystore-0.6.5/testing/mocked/kafka.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/testing/mocked/redis.py` & `proxystore-0.6.5/testing/mocked/redis.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/testing/mocking.py` & `proxystore-0.6.5/testing/mocking.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/testing/relay_server.py` & `proxystore-0.6.5/testing/relay_server.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/testing/scripts/kafka_pubsub.py` & `proxystore-0.6.5/testing/scripts/kafka_pubsub.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/testing/scripts/peer_connection_bandwidth.py` & `proxystore-0.6.5/testing/scripts/peer_connection_bandwidth.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/testing/scripts/peer_endpoint_bandwidth.py` & `proxystore-0.6.5/testing/scripts/peer_endpoint_bandwidth.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/testing/scripts/peer_manager_bandwidth.py` & `proxystore-0.6.5/testing/scripts/peer_manager_bandwidth.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/testing/scripts/redis_pubsub.py` & `proxystore-0.6.5/testing/scripts/redis_pubsub.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/testing/ssl.py` & `proxystore-0.6.5/testing/ssl.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     keyfile = tmp_path / 'key.pem'
     cert, key = create_self_signed_cert()
     write_cert_key_pair(cert, key, certfile, keyfile)
 
     ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
     ssl_context.load_cert_chain(certfile, keyfile=keyfile)
 
-    return SSLContextFixture(certfile, keyfile, ssl_context)
+    return SSLContextFixture(str(certfile), str(keyfile), ssl_context)
 
 
 def create_self_signed_cert() -> tuple[Certificate, RSAPrivateKey]:
     """Creates a self-signed certificate and private key pair."""
     key = generate_private_key(public_exponent=65537, key_size=2048)
 
     # Various details about who we are. For a self-signed certificate the
```

### Comparing `proxystore-0.6.4/testing/stores.py` & `proxystore-0.6.5/testing/stores.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/testing/utils.py` & `proxystore-0.6.5/testing/utils.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/conftest.py` & `proxystore-0.6.5/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from typing import ContextManager
 from typing import Generator
 from unittest import mock
 
 import pytest
 import uvloop
 
+import proxystore
+
 # Import fixtures from testing/ so they are known by pytest
 # and can be used with
 from testing.connectors import connectors
 from testing.connectors import endpoint_connector
 from testing.connectors import file_connector
 from testing.connectors import globus_connector
 from testing.connectors import local_connector
@@ -65,7 +67,18 @@
                 'should only be used when --use-uvloop is passed to pytest.',
             ),
         )
 
     policy = asyncio.get_event_loop_policy()
     with context:
         yield policy
+
+
+@pytest.fixture(autouse=True)
+def _verify_no_registered_stores() -> Generator[None, None, None]:
+    yield
+
+    if len(proxystore.store._stores) > 0:  # pragma: no cover
+        raise RuntimeError(
+            'Test left at least one store registered: '
+            f'{tuple(proxystore.store._stores.keys())}.',
+        )
```

### Comparing `proxystore-0.6.4/tests/connectors/connector_test.py` & `proxystore-0.6.5/tests/connectors/connector_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/connectors/endpoint_test.py` & `proxystore-0.6.5/tests/connectors/endpoint_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/connectors/file_test.py` & `proxystore-0.6.5/tests/connectors/file_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/connectors/globus_test.py` & `proxystore-0.6.5/tests/connectors/globus_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/connectors/multi_test.py` & `proxystore-0.6.5/tests/connectors/multi_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/connectors/redis_test.py` & `proxystore-0.6.5/tests/connectors/redis_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/endpoint/cli_test.py` & `proxystore-0.6.5/tests/endpoint/cli_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/endpoint/client_test.py` & `proxystore-0.6.5/tests/endpoint/client_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/endpoint/commands_test.py` & `proxystore-0.6.5/tests/endpoint/commands_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/endpoint/config_test.py` & `proxystore-0.6.5/tests/endpoint/config_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/endpoint/endpoint_peering_test.py` & `proxystore-0.6.5/tests/endpoint/endpoint_peering_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/endpoint/endpoint_solo_test.py` & `proxystore-0.6.5/tests/endpoint/endpoint_solo_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/endpoint/serve_test.py` & `proxystore-0.6.5/tests/endpoint/serve_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/endpoint/storage_test.py` & `proxystore-0.6.5/tests/endpoint/storage_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/factory_test.py` & `proxystore-0.6.5/tests/factory_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/globus/cli_test.py` & `proxystore-0.6.5/tests/globus/cli_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/globus/client_test.py` & `proxystore-0.6.5/tests/globus/client_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/globus/manager_test.py` & `proxystore-0.6.5/tests/globus/manager_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/globus/scopes_test.py` & `proxystore-0.6.5/tests/globus/scopes_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/globus/storage_test.py` & `proxystore-0.6.5/tests/globus/storage_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/globus/transfer_test.py` & `proxystore-0.6.5/tests/globus/transfer_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/integration/endpoints_test.py` & `proxystore-0.6.5/tests/integration/endpoints_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/p2p/chunks_test.py` & `proxystore-0.6.5/tests/p2p/chunks_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/p2p/connection_test.py` & `proxystore-0.6.5/tests/p2p/connection_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/p2p/manager_test.py` & `proxystore-0.6.5/tests/p2p/manager_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/p2p/nat_test.py` & `proxystore-0.6.5/tests/p2p/nat_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/p2p/relay/authenticate_test.py` & `proxystore-0.6.5/tests/p2p/relay/authenticate_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/p2p/relay/client_test.py` & `proxystore-0.6.5/tests/p2p/relay/client_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/p2p/relay/config_test.py` & `proxystore-0.6.5/tests/p2p/relay/config_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/p2p/relay/manager_test.py` & `proxystore-0.6.5/tests/p2p/relay/manager_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/p2p/relay/messages_test.py` & `proxystore-0.6.5/tests/p2p/relay/messages_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/p2p/relay/run_test.py` & `proxystore-0.6.5/tests/p2p/relay/run_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/p2p/relay/server_test.py` & `proxystore-0.6.5/tests/p2p/relay/server_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/proxy_test.py` & `proxystore-0.6.5/tests/proxy/proxy_utils_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 from __future__ import annotations
 
 import pickle as pkl
 
 import pytest
 
-import proxystore as ps
 from proxystore.factory import SimpleFactory
+from proxystore.proxy import extract
+from proxystore.proxy import get_factory
 from proxystore.proxy import is_resolved
 from proxystore.proxy import Proxy
 from proxystore.proxy import ProxyLocker
+from proxystore.proxy import resolve
 from proxystore.serialize import deserialize
 from proxystore.serialize import serialize
 
 
-def test_proxy() -> None:
+def test_proxy_utils() -> None:
     with pytest.raises(TypeError):
         # Proxy requires a callable type
         Proxy('not a factory')  # type: ignore
 
     x = [1, 2, 3]
     f = SimpleFactory(x)
     p = Proxy(f)
 
-    assert not ps.proxy.is_resolved(p)
+    assert not is_resolved(p)
 
     # Test pickleable
     p_pkl = pkl.dumps(p)
     p = pkl.loads(p_pkl)
 
-    assert not ps.proxy.is_resolved(p)
+    assert not is_resolved(p)
 
     assert isinstance(p, Proxy)
     assert isinstance(p, list)
-    assert ps.proxy.is_resolved(p)
+    assert is_resolved(p)
 
     # Test extracting
-    x_ = ps.proxy.extract(p)
+    x_ = extract(p)
     assert isinstance(x_, list)
     assert not isinstance(x_, Proxy)
     assert x == x_
 
     p = p + [1]  # noqa
     assert not isinstance(p, Proxy)
     assert p == [1, 2, 3, 1]
@@ -61,17 +63,23 @@
     assert not isinstance(res, Proxy)
     assert res == [2, 4, 6]
 
     p = Proxy(f)
     assert isinstance(p, list)
 
     p = Proxy(SimpleFactory('hello'))
-    assert not ps.proxy.is_resolved(p)
-    ps.proxy.resolve(p)
-    assert ps.proxy.is_resolved(p)
+    assert not is_resolved(p)
+    resolve(p)
+    assert is_resolved(p)
+
+
+def test_get_factory() -> None:
+    factory = SimpleFactory('value')
+    proxy = Proxy(factory)
+    assert get_factory(proxy) is factory
 
 
 def test_proxy_locker():
     value = [1, 2, 3]
     proxy = Proxy(SimpleFactory(value))
 
     locker = ProxyLocker(proxy)
```

### Comparing `proxystore-0.6.4/tests/serialization_test.py` & `proxystore-0.6.5/tests/serialize_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/store/cache_test.py` & `proxystore-0.6.5/tests/store/cache_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/store/factory_test.py` & `proxystore-0.6.5/tests/store/factory_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/store/init_test.py` & `proxystore-0.6.5/tests/store/init_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import pytest
 
 from proxystore.connectors.local import LocalConnector
 from proxystore.factory import SimpleFactory
 from proxystore.proxy import Proxy
+from proxystore.store import get_or_create_store
 from proxystore.store import get_store
 from proxystore.store import register_store
 from proxystore.store import store_registration
 from proxystore.store import unregister_store
 from proxystore.store.base import Store
 from proxystore.store.exceptions import ProxyStoreFactoryError
 from proxystore.store.exceptions import StoreExistsError
@@ -27,14 +28,33 @@
     unregister_store(store.name)
     assert get_store('test') is None
 
     # does not raise error
     unregister_store('not a valid store name')
 
 
+def test_get_or_create_store() -> None:
+    store = Store('test', connector=LocalConnector())
+
+    assert get_store(store.name) is None
+    new_store = get_or_create_store(store.config(), register=True)
+    assert get_store(store.name) is new_store
+    assert get_or_create_store(store.config()) is new_store
+
+    unregister_store(new_store)
+
+
+def test_get_or_create_store_no_register() -> None:
+    store = Store('test', connector=LocalConnector())
+
+    assert get_store(store.name) is None
+    get_or_create_store(store.config(), register=False)
+    assert get_store(store.name) is None
+
+
 def test_unregister_with_store() -> None:
     store = Store('test', connector=LocalConnector())
 
     register_store(store)
     assert get_store('test') == store
     unregister_store(store)
     assert get_store('test') is None
```

### Comparing `proxystore-0.6.4/tests/store/lifetimes_test.py` & `proxystore-0.6.5/tests/store/lifetimes_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from proxystore.proxy import Proxy
 from proxystore.store.base import Store
 from proxystore.store.exceptions import ProxyStoreFactoryError
 from proxystore.store.lifetimes import ContextLifetime
 from proxystore.store.lifetimes import LeaseLifetime
 from proxystore.store.lifetimes import Lifetime
 from proxystore.store.lifetimes import register_lifetime_atexit
+from proxystore.store.lifetimes import StaticLifetime
 
 
 def test_context_lifetime_protocol(store: Store[LocalConnector]) -> None:
     lifetime = ContextLifetime(store)
     assert isinstance(lifetime, Lifetime)
     lifetime.close()
 
@@ -131,15 +132,69 @@
     close_store: bool,
 ) -> None:
     key = store.put('value')
 
     lifetime = ContextLifetime(store)
     lifetime.add_key(key)
 
-    callback = register_lifetime_atexit(lifetime, close_store=close_store)
+    callback = register_lifetime_atexit(lifetime, close_stores=close_store)
 
     assert not lifetime.done()
     callback()
     assert lifetime.done()
     assert not store.exists(key)
 
     atexit.unregister(callback)
+
+
+def test_static_lifetime_is_singleton() -> None:
+    assert StaticLifetime() is StaticLifetime()
+
+
+def test_add_key_without_store_error() -> None:
+    with pytest.raises(ValueError, match='requires the store parameter'):
+        StaticLifetime().add_key(())
+
+
+def test_static_lifetime_add_bad_proxy() -> None:
+    proxy: Proxy[list[Any]] = Proxy(list)
+
+    with pytest.raises(ProxyStoreFactoryError):
+        StaticLifetime().add_proxy(proxy)
+
+
+def test_static_lifetime_cleanup(store: Store[LocalConnector]) -> None:
+    key1 = store.put('value1')
+    key2 = store.put('value2')
+    key3 = store.put('value3')
+    key4 = store.put('value4')
+    proxy1: Proxy[str] = store.proxy_from_key(key3)
+    proxy2: Proxy[str] = store.proxy_from_key(key4)
+
+    lifetime = StaticLifetime()
+    assert not lifetime.done()
+
+    lifetime.add_key(key1, key2, store=store)
+    lifetime.add_proxy(proxy1, proxy2)
+
+    # Will get back same lifetime object so both options to close work
+    # and are idempotent.
+    StaticLifetime().close()
+    lifetime.close()
+    assert lifetime.done()
+
+    assert not store.exists(key1)
+    assert not store.exists(key2)
+    assert not store.exists(key3)
+    assert not store.exists(key4)
+
+    # Cleanup singleton instance
+    StaticLifetime._instance = None
+
+
+def test_static_lifetime_close_store(store: Store[LocalConnector]) -> None:
+    store.put('value', lifetime=StaticLifetime())
+
+    StaticLifetime().close(close_stores=True)
+
+    # Cleanup singleton instance
+    StaticLifetime._instance = None
```

### Comparing `proxystore-0.6.4/tests/store/metrics_test.py` & `proxystore-0.6.5/tests/store/metrics_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any
 
 from proxystore.proxy import Proxy
 from proxystore.store.factory import StoreFactory
 from proxystore.store.metrics import Metrics
 from proxystore.store.metrics import StoreMetrics
 from proxystore.store.metrics import TimeStats
+from proxystore.store.types import StoreConfig
 
 
 def test_time_stats() -> None:
     stats1 = TimeStats()
     stats1.add_time(1)
     stats2 = TimeStats()
     stats2.add_time(3)
@@ -60,16 +61,16 @@
         [('key1',), ('key2',), ('key3',)],
     ]
 
     for key in keys:
         metrics.add_attribute('test-attribute', key, 'value')
         metrics.add_counter('test-counter', key, 1)
         metrics.add_counter('test-counter', key, 1)
-        metrics.add_time('test-timer', key, 1000)
-        metrics.add_time('test-timer', key, 2000)
+        metrics.add_time('test-timer', key, 1)
+        metrics.add_time('test-timer', key, 2)
 
         key_metrics = metrics.get_metrics(key)
         assert key_metrics is not None
 
         assert key_metrics.attributes == {'test-attribute': 'value'}
         assert key_metrics.counters == {'test-counter': 2}
         assert key_metrics.times['test-timer'].count == 2
@@ -83,37 +84,58 @@
     assert metrics.get_metrics(('test-key',)) is None
 
 
 def test_metrics_by_proxy() -> None:
     metrics = StoreMetrics()
 
     key = ('test-key',)
-    proxy: Proxy[Any] = Proxy(StoreFactory(key, {}))
+    proxy: Proxy[Any] = Proxy(
+        StoreFactory(
+            key,
+            StoreConfig(
+                name='test',
+                connector_type='test',
+                connector_config={},
+            ),
+        ),
+    )
 
     metrics.add_attribute('test-attribute', key, 'value')
     assert metrics.get_metrics(proxy) == metrics.get_metrics(key)
 
 
 def test_metrics_by_proxies() -> None:
     metrics = StoreMetrics()
 
     keys = [('key1',), ('key2',), ('key3',)]
-    proxies: list[Proxy[Any]] = [Proxy(StoreFactory(key, {})) for key in keys]
+    proxies: list[Proxy[Any]] = [
+        Proxy(
+            StoreFactory(
+                key,
+                StoreConfig(
+                    name='test',
+                    connector_type='test',
+                    connector_config={},
+                ),
+            ),
+        )
+        for key in keys
+    ]
 
     metrics.add_attribute('test-attribute', proxies, 'value')
     assert metrics.get_metrics(proxies) == metrics.get_metrics(keys)
 
 
 def test_store_metrics_aggregate_times() -> None:
     metrics = StoreMetrics()
     keys = [('key1',), ('key2',), ('key3',)]
 
     for i, key in enumerate(keys):
-        metrics.add_time('time1', key, (1 + i) * 1000)
-        metrics.add_time('time2', key, (1 + i) * 10000)
+        metrics.add_time('time1', key, (1 + i) * 1)
+        metrics.add_time('time2', key, (1 + i) * 10)
 
     times = metrics.aggregate_times()
     assert times['time1'].count == len(keys)
     assert times['time1'].avg_time_ms == 2
     assert times['time1'].min_time_ms == 1
     assert times['time1'].max_time_ms == 3
     assert times['time2'].count == len(keys)
```

### Comparing `proxystore-0.6.4/tests/store/ref_test.py` & `proxystore-0.6.5/tests/store/ref_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import pytest
 
 from proxystore.connectors.file import FileConnector
 from proxystore.proxy import is_resolved
 from proxystore.proxy import Proxy
 from proxystore.store import Store
 from proxystore.store import store_registration
+from proxystore.store.exceptions import ProxyStoreFactoryError
 from proxystore.store.factory import StoreFactory
 from proxystore.store.ref import _WeakRefFinalizer
 from proxystore.store.ref import borrow
 from proxystore.store.ref import clone
 from proxystore.store.ref import into_owned
 from proxystore.store.ref import mut_borrow
 from proxystore.store.ref import MutableBorrowError
@@ -209,15 +210,15 @@
     new_borrowed = pickle.loads(borrowed_pkl)
     assert new_borrowed == 'value'
 
     del new_borrowed
     # new_borrowed, because it was pickled and unpickled, does not have a
     # reference to is owned proxy so deleting new_borrowed will not
     # decrement the ref count on proxy.
-    assert object.__getattribute__(proxy, '__ref_count__') == 1
+    assert object.__getattribute__(proxy, '__proxy_ref_count__') == 1
 
 
 def test_pickle_ref_mut_proxy(store: Store[FileConnector]) -> None:
     factory = put_in_store('value', store)
     proxy = OwnedProxy(factory)
 
     borrowed = mut_borrow(proxy)
@@ -230,15 +231,15 @@
     new_borrowed = pickle.loads(borrowed_pkl)
     assert new_borrowed == 'value'
 
     del new_borrowed
     # new_borrowed, because it was pickled and unpickled, does not have a
     # reference to is owned proxy so deleting new_borrowed will not
     # decrement the ref count on proxy.
-    assert object.__getattribute__(proxy, '__ref_mut_count__') == 1
+    assert object.__getattribute__(proxy, '__proxy_ref_mut_count__') == 1
 
 
 def test_copy_not_implemented_error(store: Store[FileConnector]) -> None:
     factory = put_in_store('value', store)
     proxy = OwnedProxy(factory)
 
     message = '^Copy is not implemented'
@@ -359,27 +360,39 @@
 def test_into_owned_value_error(store: Store[FileConnector]) -> None:
     factory = put_in_store('value', store)
     proxy = OwnedProxy(factory)
     with pytest.raises(ValueError, match='Only a base proxy can be'):
         into_owned(proxy)
 
 
+def test_into_owned_factory_error(store: Store[FileConnector]) -> None:
+    def factory() -> str:  # pragma: no cover
+        return 'value'
+
+    proxy = Proxy(factory)
+    with pytest.raises(
+        ProxyStoreFactoryError,
+        match='The proxy must contain a factory with type StoreFactory.',
+    ):
+        into_owned(proxy)
+
+
 @pytest.mark.parametrize('populate_target', (True, False))
 def test_borrow_populate(
     populate_target: bool,
     store: Store[FileConnector],
 ) -> None:
     factory = put_in_store('value', store)
     proxy = OwnedProxy(factory)
     assert isinstance(proxy, str)
 
     borrowed = borrow(proxy, populate_target=populate_target)
     assert is_resolved(borrowed) == populate_target
 
-    del proxy.__wrapped__
+    del proxy.__proxy_wrapped__
     borrowed = borrow(proxy, populate_target=populate_target)
     assert not is_resolved(borrowed)
 
 
 @pytest.mark.parametrize('populate_target', (True, False))
 def test_mut_borrow_populate(
     populate_target: bool,
@@ -389,15 +402,15 @@
     proxy = OwnedProxy(factory)
     assert isinstance(proxy, str)
 
     borrowed = mut_borrow(proxy, populate_target=populate_target)
     assert is_resolved(borrowed) == populate_target
 
     del borrowed
-    del proxy.__wrapped__
+    del proxy.__proxy_wrapped__
     borrowed = mut_borrow(proxy, populate_target=populate_target)
     assert not is_resolved(borrowed)
 
 
 @pytest.mark.parametrize('populate_target', (True, False))
 def test_into_owned_populate(
     populate_target: bool,
@@ -418,7 +431,35 @@
     proxy_pkl = pickle.dumps(proxy)
     new_proxy = pickle.loads(proxy_pkl)
 
     # Should do nothing because old proxy was made invalid
     del proxy
 
     assert new_proxy == 'value'
+
+
+def test_clone_deepcopy(store: Store[FileConnector]) -> None:
+    value = [1, 2, 3]
+    factory = put_in_store(value, store)
+    proxy = OwnedProxy(factory, target=value)
+    assert is_resolved(proxy)
+
+    cloned = clone(proxy)
+    assert is_resolved(cloned)
+    cloned.append(4)
+    assert cloned == [1, 2, 3, 4]
+    assert proxy == [1, 2, 3]
+
+
+def test_owned_proxy_cache_defaults(store: Store[FileConnector]) -> None:
+    value = 'value'
+    factory = put_in_store(value, store)
+    proxy = OwnedProxy(factory, cache_defaults=True, target=value)
+    del proxy.__proxy_wrapped__
+
+    assert not is_resolved(proxy)
+    assert isinstance(proxy, str)
+    assert not is_resolved(proxy)
+
+    assert not is_resolved(proxy)
+    assert hash(proxy) == hash(value)
+    assert not is_resolved(proxy)
```

### Comparing `proxystore-0.6.4/tests/store/scopes_test.py` & `proxystore-0.6.5/tests/store/scopes_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,21 +95,21 @@
     with pytest.raises(ReferenceInvalidError):
         assert isinstance(borrowed, str)
 
 
 def test_mark_refs_out_of_scope_no_owner(store: Store[FileConnector]) -> None:
     proxy = store.owned_proxy('value')
     borrowed = borrow(proxy)
-    object.__setattr__(borrowed, '__owner__', None)
+    object.__setattr__(borrowed, '__proxy_owner__', None)
 
     with pytest.raises(RuntimeError, match='no reference to its owner'):
         mark_refs_out_of_scope(borrowed)
 
     # Restore owner so cleanup can be done correctly
-    object.__setattr__(borrowed, '__owner__', proxy)
+    object.__setattr__(borrowed, '__proxy_owner__', proxy)
 
 
 def test_make_out_of_scope_callback(store: Store[FileConnector]) -> None:
     proxy = store.owned_proxy('value1')
     borrowed = borrow(proxy)
 
     callback = _make_out_of_scope_callback([borrowed])
```

### Comparing `proxystore-0.6.4/tests/store/store_basics_test.py` & `proxystore-0.6.5/tests/store/store_basics_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,24 +5,39 @@
 from unittest import mock
 
 import pytest
 
 from proxystore.connectors.local import LocalConnector
 from proxystore.proxy import Proxy
 from proxystore.serialize import SerializationError
+from proxystore.store import get_store
 from proxystore.store import Store
+from proxystore.store.exceptions import StoreExistsError
 from proxystore.store.future import Future
 from proxystore.store.lifetimes import ContextLifetime
 
 
 def test_negative_cache_size() -> None:
     with pytest.raises(ValueError):
         Store('test', LocalConnector(), cache_size=-1)
 
 
+def test_init_and_register() -> None:
+    name = 'test-store'
+    assert get_store(name) is None
+    with Store(name, LocalConnector(), register=True) as store:
+        assert get_store(name) is store
+
+        with pytest.raises(StoreExistsError):
+            Store(name, LocalConnector(), register=True)
+
+    # Context manager close should unregister the store.
+    assert get_store(name) is None
+
+
 @pytest.mark.parametrize(
     'value',
     (b'value', 'value', lambda: 'value', ['value1', 'value2', 'value3']),
 )
 def test_basic_operations(value: Any, store: Store[LocalConnector]) -> None:
     key = store.put(value)
```

### Comparing `proxystore-0.6.4/tests/store/store_metrics_test.py` & `proxystore-0.6.5/tests/store/store_metrics_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/store/store_proxy_test.py` & `proxystore-0.6.5/tests/store/store_proxy_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,33 @@
 from __future__ import annotations
 
 from typing import Any
-from typing import Generator
 
 import pytest
 
-import proxystore
 from proxystore.connectors.local import LocalConnector
+from proxystore.proxy import get_factory
 from proxystore.proxy import is_resolved
 from proxystore.proxy import Proxy
 from proxystore.proxy import ProxyLocker
+from proxystore.proxy import resolve
 from proxystore.serialize import deserialize
 from proxystore.serialize import serialize
 from proxystore.store import get_store
 from proxystore.store import register_store
 from proxystore.store import unregister_store
 from proxystore.store.base import Store
 from proxystore.store.exceptions import NonProxiableTypeError
 from proxystore.store.exceptions import ProxyResolveMissingKeyError
 from proxystore.store.factory import StoreFactory
 from proxystore.store.lifetimes import ContextLifetime
 from proxystore.store.ref import OwnedProxy
 from proxystore.store.utils import get_key
 
 
-@pytest.fixture(autouse=True)
-def _verify_no_registered_stores() -> Generator[None, None, None]:
-    yield
-
-    if len(proxystore.store._stores) > 0:  # pragma: no cover
-        raise RuntimeError(
-            'Test left at least one store registered: '
-            f'{tuple(proxystore.store._stores.keys())}.',
-        )
-
-
 def test_factory_resolve(store: Store[LocalConnector]) -> None:
     key = store.put([1, 2, 3])
     f: StoreFactory[Any, list[int]] = StoreFactory(
         key,
         store_config=store.config(),
     )
     assert f() == [1, 2, 3]
@@ -121,14 +110,20 @@
 
 def test_proxy_populate_target(store: Store[LocalConnector]) -> None:
     p = store.proxy([1, 2, 3], populate_target=True)
     assert is_resolved(p)
     assert isinstance(p, Proxy)
     assert p == [1, 2, 3]
 
+    # populate_target should also set cache_defaults on the proxy
+    del p.__proxy_wrapped__
+    assert not is_resolved(p)
+    assert isinstance(p, list)
+    assert not is_resolved(p)
+
 
 def test_proxy_from_key(store: Store[LocalConnector]) -> None:
     key = store.put([1, 2, 3])
     p: Proxy[list[int]] = store.proxy_from_key(key)
     assert isinstance(p, Proxy)
     assert p == [1, 2, 3]
 
@@ -154,16 +149,17 @@
 
 def test_proxy_missing_key(store: Store[LocalConnector]) -> None:
     proxy = store.proxy([1, 2, 3])
     key = get_key(proxy)
     store.evict(key)
     assert not store.exists(key)
 
+    assert isinstance(get_factory(proxy), StoreFactory)
     with pytest.raises(ProxyResolveMissingKeyError):
-        proxy.__factory__.resolve()
+        resolve(proxy)
 
     proxy = store.proxy_from_key(key=key)
     with pytest.raises(ProxyResolveMissingKeyError):
         proxy()
 
 
 def test_proxy_bad_serializer(store: Store[LocalConnector]) -> None:
@@ -255,14 +251,21 @@
     )
     assert is_resolved(proxies[0])
     assert not isinstance(proxies[1], Proxy)
     assert is_resolved(proxies[2])
     for p, v in zip(proxies, values):
         assert p == v
 
+    # populate_target should also set cache_defaults on the proxy
+    del proxies[0].__proxy_wrapped__
+    assert not is_resolved(proxies[0])
+    assert isinstance(proxies[0], str)
+    assert hash(proxies[0]) == hash(values[0])
+    assert not is_resolved(proxies[0])
+
 
 def test_proxy_batch_custom_serializer(store: Store[LocalConnector]) -> None:
     values = [b'test_value1', b'test_value2', b'test_value3']
     proxies: list[Proxy[bytes]] = store.proxy_batch(
         values,
         serializer=lambda s: s,
         deserializer=lambda s: s,
@@ -334,16 +337,48 @@
             store.locked_proxy('test_value', evict=True, lifetime=lifetime)
 
 
 def test_owned_proxy(store: Store[LocalConnector]) -> None:
     assert isinstance(store.owned_proxy([1, 2, 3]), OwnedProxy)
 
 
+def test_owned_proxy_populate_target(store: Store[LocalConnector]) -> None:
+    value = 'test_value'
+    p = store.owned_proxy(value, populate_target=True)
+    assert is_resolved(p)
+    assert isinstance(p, Proxy)
+    assert p == value
+
+    # populate_target should also set cache_defaults on the proxy
+    del p.__proxy_wrapped__
+    assert not is_resolved(p)
+    assert isinstance(p, str)
+    assert hash(p) == hash(value)
+    assert not is_resolved(p)
+
+
 def test_owned_proxy_skip_nonproxiable(store: Store[LocalConnector]) -> None:
     p = store.owned_proxy(None, skip_nonproxiable=True)
     assert not isinstance(p, (Proxy, OwnedProxy))
     assert p is None
 
 
 def test_owned_proxy_nonproxiable_error(store: Store[LocalConnector]) -> None:
     with pytest.raises(NonProxiableTypeError):
         store.owned_proxy(None, skip_nonproxiable=False)
+
+
+@pytest.mark.parametrize('populate_target', (True, False))
+def test_default_populate_target(populate_target: bool) -> None:
+    with Store(
+        'test-default-populate-target',
+        LocalConnector(),
+        populate_target=populate_target,
+    ) as store:
+        proxy = store.proxy('value')
+        assert is_resolved(proxy) == populate_target
+
+        proxy = store.proxy('value', populate_target=True)
+        assert is_resolved(proxy)
+
+        proxy = store.proxy('value', populate_target=False)
+        assert not is_resolved(proxy)
```

### Comparing `proxystore-0.6.4/tests/stream/events_test.py` & `proxystore-0.6.5/tests/stream/events_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import NamedTuple
 
 import pytest
 
+from proxystore.store.types import StoreConfig
 from proxystore.stream.events import bytes_to_event
 from proxystore.stream.events import EndOfStreamEvent
 from proxystore.stream.events import Event
 from proxystore.stream.events import event_to_bytes
 from proxystore.stream.events import EventBatch
 from proxystore.stream.events import NewObjectEvent
 
@@ -24,15 +25,19 @@
         EventBatch(
             [
                 NewObjectEvent.from_key(_TestKey('a', 123), True, {}),
                 NewObjectEvent.from_key(_TestKey('b', 234), True, {}),
                 EndOfStreamEvent(),
             ],
             topic='default',
-            store_config={},
+            store_config=StoreConfig(
+                name='test',
+                connector_type='test',
+                connector_config={},
+            ),
         ),
         NewObjectEvent.from_key(_TestKey('a', 123), True, {}),
     ),
 )
 def test_encode_decode(event: Event) -> None:
     json_string = event_to_bytes(event)
     new_event = bytes_to_event(json_string)
```

### Comparing `proxystore-0.6.4/tests/stream/filters_test.py` & `proxystore-0.6.5/tests/stream/filters_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/stream/interface_test.py` & `proxystore-0.6.5/tests/stream/interface_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/stream/shims/kafka_test.py` & `proxystore-0.6.5/tests/stream/shims/kafka_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/stream/shims/queue_test.py` & `proxystore-0.6.5/tests/stream/shims/queue_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/stream/shims/redis_test.py` & `proxystore-0.6.5/tests/stream/shims/redis_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/stream/shims/zmq_test.py` & `proxystore-0.6.5/tests/stream/shims/zmq_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/utils/config_test.py` & `proxystore-0.6.5/tests/utils/config_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/utils/counter_test.py` & `proxystore-0.6.5/tests/utils/counter_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/utils/data_test.py` & `proxystore-0.6.5/tests/utils/data_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/utils/environment_test.py` & `proxystore-0.6.5/tests/utils/environment_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/utils/imports_test.py` & `proxystore-0.6.5/tests/utils/imports_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/utils/tasks_test.py` & `proxystore-0.6.5/tests/utils/tasks_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tests/utils/timer_test.py` & `proxystore-0.6.5/tests/utils/timer_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.6.4/tox.ini` & `proxystore-0.6.5/tox.ini`

 * *Files identical despite different names*


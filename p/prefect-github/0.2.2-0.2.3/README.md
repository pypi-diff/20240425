# Comparing `tmp/prefect-github-0.2.2.tar.gz` & `tmp/prefect_github-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-github-0.2.2.tar", last modified: Wed Nov 29 19:56:32 2023, max compression
+gzip compressed data, was "prefect_github-0.2.3.tar", last modified: Thu Apr 25 19:20:17 2024, max compression
```

## Comparing `prefect-github-0.2.2.tar` & `prefect_github-0.2.3.tar`

### file list

```diff
@@ -1,58 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:56:32.005450 prefect-github-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-11-29 19:55:51.000000 prefect-github-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-11-29 19:55:51.000000 prefect-github-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2023-11-29 19:56:32.005450 prefect-github-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2023-11-29 19:55:51.000000 prefect-github-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:56:32.005450 prefect-github-0.2.2/prefect_github/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-11-29 19:56:32.005450 prefect-github-0.2.2/prefect_github/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:56:31.993450 prefect-github-0.2.2/prefect_github/configs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:56:32.001449 prefect-github-0.2.2/prefect_github/configs/mutation/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/configs/mutation/add_comment.json
--rw-r--r--   0 runner    (1001) docker     (127)      695 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/configs/mutation/add_pull_request_review.json
--rw-r--r--   0 runner    (1001) docker     (127)      266 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/configs/mutation/add_reaction.json
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/configs/mutation/add_star.json
--rw-r--r--   0 runner    (1001) docker     (127)      872 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/configs/mutation/close_issue.json
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/configs/mutation/close_pull_request.json
--rw-r--r--   0 runner    (1001) docker     (127)      873 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/configs/mutation/create_issue.json
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/configs/mutation/create_pull_request.json
--rw-r--r--   0 runner    (1001) docker     (127)      269 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/configs/mutation/remove_reaction.json
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/configs/mutation/remove_star.json
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/configs/mutation/request_reviews.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:56:32.001449 prefect-github-0.2.2/prefect_github/configs/query/
--rw-r--r--   0 runner    (1001) docker     (127)     7626 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/configs/query/organization.json
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/configs/query/repository.json
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/configs/query/repository_owner.json
--rw-r--r--   0 runner    (1001) docker     (127)     9764 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/configs/query/user.json
--rw-r--r--   0 runner    (1001) docker     (127)     9766 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/configs/query/viewer.json
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)    20646 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)    64044 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)   108595 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/repository_owner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:56:32.001449 prefect-github-0.2.2/prefect_github/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1066892 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/schemas/graphql_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    75743 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    73099 2023-11-29 19:55:51.000000 prefect-github-0.2.2/prefect_github/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:56:32.005450 prefect-github-0.2.2/prefect_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2023-11-29 19:56:31.000000 prefect-github-0.2.2/prefect_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2023-11-29 19:56:31.000000 prefect-github-0.2.2/prefect_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 19:56:31.000000 prefect-github-0.2.2/prefect_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-11-29 19:56:31.000000 prefect-github-0.2.2/prefect_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-11-29 19:56:31.000000 prefect-github-0.2.2/prefect_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-29 19:56:31.000000 prefect-github-0.2.2/prefect_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-11-29 19:55:51.000000 prefect-github-0.2.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-29 19:55:51.000000 prefect-github-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      844 2023-11-29 19:56:32.005450 prefect-github-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2023-11-29 19:55:51.000000 prefect-github-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:56:32.005450 prefect-github-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-11-29 19:55:51.000000 prefect-github-0.2.2/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2023-11-29 19:55:51.000000 prefect-github-0.2.2/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2023-11-29 19:55:51.000000 prefect-github-0.2.2/tests/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     7665 2023-11-29 19:55:51.000000 prefect-github-0.2.2/tests/test_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-11-29 19:55:51.000000 prefect-github-0.2.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    80049 2023-11-29 19:55:51.000000 prefect-github-0.2.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:17.325906 prefect_github-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-25 19:20:17.325906 prefect_github-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-25 19:20:04.000000 prefect_github-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:17.313906 prefect_github-0.2.3/prefect_github/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:16.000000 prefect_github-0.2.3/prefect_github/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:17.309906 prefect_github-0.2.3/prefect_github/configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:17.313906 prefect_github-0.2.3/prefect_github/configs/mutation/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/configs/mutation/add_comment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/configs/mutation/add_pull_request_review.json
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/configs/mutation/add_reaction.json
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/configs/mutation/add_star.json
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/configs/mutation/close_issue.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/configs/mutation/close_pull_request.json
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/configs/mutation/create_issue.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/configs/mutation/create_pull_request.json
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/configs/mutation/remove_reaction.json
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/configs/mutation/remove_star.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/configs/mutation/request_reviews.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:17.317906 prefect_github-0.2.3/prefect_github/configs/query/
+-rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/configs/query/organization.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/configs/query/repository.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/configs/query/repository_owner.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/configs/query/user.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9766 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/configs/query/viewer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20646 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64980 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108596 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/repository_owner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:17.321906 prefect_github-0.2.3/prefect_github/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  4561834 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/schemas/graphql_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1066892 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/schemas/graphql_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77111 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73099 2024-04-25 19:20:04.000000 prefect_github-0.2.3/prefect_github/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:17.325906 prefect_github-0.2.3/prefect_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-25 19:20:17.000000 prefect_github-0.2.3/prefect_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-25 19:20:17.000000 prefect_github-0.2.3/prefect_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:17.000000 prefect_github-0.2.3/prefect_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 19:20:17.000000 prefect_github-0.2.3/prefect_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-25 19:20:17.000000 prefect_github-0.2.3/prefect_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 19:20:17.000000 prefect_github-0.2.3/prefect_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-25 19:20:04.000000 prefect_github-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:17.325906 prefect_github-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:17.325906 prefect_github-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-25 19:20:04.000000 prefect_github-0.2.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-25 19:20:04.000000 prefect_github-0.2.3/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-25 19:20:04.000000 prefect_github-0.2.3/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-25 19:20:04.000000 prefect_github-0.2.3/tests/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-25 19:20:04.000000 prefect_github-0.2.3/tests/test_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-25 19:20:04.000000 prefect_github-0.2.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-25 19:20:04.000000 prefect_github-0.2.3/tests/test_version.py
```

### Comparing `prefect-github-0.2.2/PKG-INFO` & `prefect_github-0.2.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,98 +1,85 @@
 Metadata-Version: 2.1
 Name: prefect-github
-Version: 0.2.2
+Version: 0.2.3
 Summary: Prefect integrations interacting with GitHub
-Home-page: https://github.com/PrefectHQ/prefect-github
-Author: Prefect Technologies Inc.
-Author-email: help@prefect.io
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-github
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: sgqlc>=15.0
 Requires-Dist: prefect>=2.13.5
 Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: interrogate; extra == "dev"
+Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: isort; extra == "dev"
+Requires-Dist: mock; python_version < "3.8" and extra == "dev"
+Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev"
-Requires-Dist: mkdocs-gen-files; extra == "dev"
-Requires-Dist: interrogate; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
-Requires-Dist: pillow; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
 
 # prefect-github
  
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-github/" alt="PyPI version">
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-github?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-github/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-github?color=0052FF&labelColor=090422" /></a>
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-github?color=26272B&labelColor=090422"></a>
     <a href="https://pepy.tech/badge/prefect-github/" alt="Downloads">
-        <img src="https://img.shields.io/pypi/dm/prefect-github?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-github/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-github?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
+        <img src="https://img.shields.io/pypi/dm/prefect-github?color=26272B&labelColor=090422" /></a>
 </p>
 
 ## Welcome!
 
 Prefect integrations interacting with GitHub.
 
 The tasks within this collection were created by a code generator using the GitHub GraphQL schema.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.7+.
+Requires an installation of Python 3.8 or newer.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
-These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://orion-docs.prefect.io/).
+These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
 
 Install `prefect-github` with `pip`:
 
 ```bash
 pip install prefect-github
 ```
 
-Then, register to [view the block](https://orion-docs.prefect.io/ui/blocks/) on Prefect Cloud:
+Then, register to [view the block](https://docs.prefect.io/ui/blocks/) on Prefect Cloud:
 
 ```bash
 prefect block register -m prefect_github
 ```
 
-Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
+Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or saved through the UI.
 
 ### Write and run a flow
 
 ```python
 from prefect import flow
 from prefect_github import GitHubCredentials
 from prefect_github.repository import query_repository
@@ -118,15 +105,15 @@
 github_add_star_flow()
 ```
 
 ## Resources
 
 If you encounter any bugs while using `prefect-github`, feel free to open an issue in the [prefect-github](https://github.com/PrefectHQ/prefect-github) repository.
 
-If you have any questions or issues while using `prefect-github`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
+If you have any questions or issues while using `prefect-github`, you can find help in the [Prefect Slack community](https://prefect.io/slack).
 
 Feel free to ⭐️ or watch [`prefect-github`](https://github.com/PrefectHQ/prefect-github) for updates too!
 
 ## Development
 
 If you'd like to install a version of `prefect-github` for development, clone the repository and perform an editable install with `pip`:
```

### Comparing `prefect-github-0.2.2/README.md` & `prefect_github-0.2.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,47 @@
 # prefect-github
  
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-github/" alt="PyPI version">
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-github?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-github/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-github?color=0052FF&labelColor=090422" /></a>
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-github?color=26272B&labelColor=090422"></a>
     <a href="https://pepy.tech/badge/prefect-github/" alt="Downloads">
-        <img src="https://img.shields.io/pypi/dm/prefect-github?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-github/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-github?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
+        <img src="https://img.shields.io/pypi/dm/prefect-github?color=26272B&labelColor=090422" /></a>
 </p>
 
 ## Welcome!
 
 Prefect integrations interacting with GitHub.
 
 The tasks within this collection were created by a code generator using the GitHub GraphQL schema.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.7+.
+Requires an installation of Python 3.8 or newer.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
-These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://orion-docs.prefect.io/).
+These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
 
 Install `prefect-github` with `pip`:
 
 ```bash
 pip install prefect-github
 ```
 
-Then, register to [view the block](https://orion-docs.prefect.io/ui/blocks/) on Prefect Cloud:
+Then, register to [view the block](https://docs.prefect.io/ui/blocks/) on Prefect Cloud:
 
 ```bash
 prefect block register -m prefect_github
 ```
 
-Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
+Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or saved through the UI.
 
 ### Write and run a flow
 
 ```python
 from prefect import flow
 from prefect_github import GitHubCredentials
 from prefect_github.repository import query_repository
@@ -76,15 +67,15 @@
 github_add_star_flow()
 ```
 
 ## Resources
 
 If you encounter any bugs while using `prefect-github`, feel free to open an issue in the [prefect-github](https://github.com/PrefectHQ/prefect-github) repository.
 
-If you have any questions or issues while using `prefect-github`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
+If you have any questions or issues while using `prefect-github`, you can find help in the [Prefect Slack community](https://prefect.io/slack).
 
 Feel free to ⭐️ or watch [`prefect-github`](https://github.com/PrefectHQ/prefect-github) for updates too!
 
 ## Development
 
 If you'd like to install a version of `prefect-github` for development, clone the repository and perform an editable install with `pip`:
```

### Comparing `prefect-github-0.2.2/prefect_github/configs/mutation/add_pull_request_review.json` & `prefect_github-0.2.3/prefect_github/configs/mutation/add_pull_request_review.json`

 * *Files identical despite different names*

### Comparing `prefect-github-0.2.2/prefect_github/configs/mutation/close_issue.json` & `prefect_github-0.2.3/prefect_github/configs/mutation/close_issue.json`

 * *Files identical despite different names*

### Comparing `prefect-github-0.2.2/prefect_github/configs/mutation/close_pull_request.json` & `prefect_github-0.2.3/prefect_github/configs/mutation/close_pull_request.json`

 * *Files identical despite different names*

### Comparing `prefect-github-0.2.2/prefect_github/configs/mutation/create_issue.json` & `prefect_github-0.2.3/prefect_github/configs/mutation/create_issue.json`

 * *Files identical despite different names*

### Comparing `prefect-github-0.2.2/prefect_github/configs/mutation/create_pull_request.json` & `prefect_github-0.2.3/prefect_github/configs/mutation/create_pull_request.json`

 * *Files identical despite different names*

### Comparing `prefect-github-0.2.2/prefect_github/configs/mutation/request_reviews.json` & `prefect_github-0.2.3/prefect_github/configs/mutation/request_reviews.json`

 * *Files identical despite different names*

### Comparing `prefect-github-0.2.2/prefect_github/configs/query/organization.json` & `prefect_github-0.2.3/prefect_github/configs/query/organization.json`

 * *Files identical despite different names*

### Comparing `prefect-github-0.2.2/prefect_github/configs/query/repository.json` & `prefect_github-0.2.3/prefect_github/configs/query/repository.json`

 * *Files identical despite different names*

### Comparing `prefect-github-0.2.2/prefect_github/configs/query/repository_owner.json` & `prefect_github-0.2.3/prefect_github/configs/query/repository_owner.json`

 * *Files identical despite different names*

### Comparing `prefect-github-0.2.2/prefect_github/configs/query/user.json` & `prefect_github-0.2.3/prefect_github/configs/query/user.json`

 * *Files identical despite different names*

### Comparing `prefect-github-0.2.2/prefect_github/configs/query/viewer.json` & `prefect_github-0.2.3/prefect_github/configs/query/viewer.json`

 * *Files identical despite different names*

### Comparing `prefect-github-0.2.2/prefect_github/credentials.py` & `prefect_github-0.2.3/prefect_github/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Credential classes used to perform authenticated interactions with GitHub"""
 
 import warnings
 
-from prefect.blocks.abstract import CredentialsBlock
 from pydantic import VERSION as PYDANTIC_VERSION
 
+from prefect.blocks.abstract import CredentialsBlock
+
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field, SecretStr
 else:
     from pydantic import Field, SecretStr
 
 from sgqlc.endpoint.http import HTTPEndpoint
```

### Comparing `prefect-github-0.2.2/prefect_github/graphql.py` & `prefect_github-0.2.3/prefect_github/graphql.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 # manually editing this file is not recommended.
 
 from functools import partial
 from pprint import pformat
 from typing import Any, Dict, Iterable, List, Tuple, Union
 
 from anyio import to_thread
-from prefect import task
 from sgqlc.operation import Operation, Selection
 
+from prefect import task
 from prefect_github import GitHubCredentials
 from prefect_github.utils import camel_to_snake_case
 
 
 async def _execute_graphql_op(
     op: Union[Operation, str],
     github_credentials: GitHubCredentials,
```

### Comparing `prefect-github-0.2.2/prefect_github/mutations.py` & `prefect_github-0.2.3/prefect_github/mutations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 # manually editing this file is not recommended. If this module
 # is outdated, rerun scripts/generate.py.
 
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Dict, Iterable
 
-from prefect import task
 from sgqlc.operation import Operation
 
+from prefect import task
 from prefect_github import GitHubCredentials
 from prefect_github.graphql import _execute_graphql_op, _subset_return_fields
 from prefect_github.schemas import graphql_schema
 from prefect_github.utils import initialize_return_fields_defaults, strip_kwargs
 
 config_dir = Path(__file__).parent.resolve() / "configs" / "mutation"
 return_fields_defaults = {}
```

### Comparing `prefect-github-0.2.2/prefect_github/organization.py` & `prefect_github-0.2.3/prefect_github/organization.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 # This module was auto-generated using prefect-collection-generator so
 # manually editing this file is not recommended. If this module
 # is outdated, rerun scripts/generate.py.
 
 from pathlib import Path
 from typing import Any, Dict, Iterable
 
-from prefect import task
 from sgqlc.operation import Operation
 
+from prefect import task
 from prefect_github import GitHubCredentials
 from prefect_github.graphql import _execute_graphql_op, _subset_return_fields
 from prefect_github.schemas import graphql_schema
 from prefect_github.utils import initialize_return_fields_defaults, strip_kwargs
 
 config_path = (
     Path(__file__).parent.resolve() / "configs" / "query" / "organization.json"
@@ -75,15 +75,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).team(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).team(
         **strip_kwargs(
             slug=slug,
         )
     )
 
     op_stack = (
         "organization",
@@ -139,15 +143,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).teams(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).teams(
         **strip_kwargs(
             user_logins=user_logins,
             privacy=privacy,
             role=role,
             query=query,
             order_by=order_by,
             ldap_mapped=ldap_mapped,
@@ -188,15 +196,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).project(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).project(
         **strip_kwargs(
             number=number,
         )
     )
 
     op_stack = (
         "organization",
@@ -244,15 +256,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).domains(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).domains(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
             is_verified=is_verified,
             is_approved=is_approved,
@@ -308,15 +324,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).packages(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).packages(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
             names=names,
             repository_id=repository_id,
@@ -370,15 +390,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).projects(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).projects(
         **strip_kwargs(
             states=states,
             order_by=order_by,
             search=search,
             after=after,
             before=before,
             first=first,
@@ -430,15 +454,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).sponsors(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).sponsors(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
             tier_id=tier_id,
             order_by=order_by,
@@ -489,15 +517,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).audit_log(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).audit_log(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
             query=query,
             order_by=order_by,
@@ -533,15 +565,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).project_v2(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).project_v2(
         **strip_kwargs(
             number=number,
         )
     )
 
     op_stack = (
         "organization",
@@ -584,15 +620,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).projects_v2(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).projects_v2(
         **strip_kwargs(
             query=query,
             order_by=order_by,
             after=after,
             before=before,
             first=first,
             last=last,
@@ -631,15 +671,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).repository(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).repository(
         **strip_kwargs(
             name=name,
             follow_renames=follow_renames,
         )
     )
 
     op_stack = (
@@ -682,15 +726,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).sponsoring(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).sponsoring(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
             order_by=order_by,
         )
@@ -725,15 +773,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).project_next(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).project_next(
         **strip_kwargs(
             number=number,
         )
     )
 
     op_stack = (
         "organization",
@@ -774,15 +826,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).pinned_items(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).pinned_items(
         **strip_kwargs(
             types=types,
             after=after,
             before=before,
             first=first,
             last=last,
         )
@@ -829,15 +885,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).projects_next(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).projects_next(
         **strip_kwargs(
             query=query,
             sort_by=sort_by,
             after=after,
             before=before,
             first=first,
             last=last,
@@ -906,15 +966,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).repositories(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).repositories(
         **strip_kwargs(
             privacy=privacy,
             order_by=order_by,
             affiliations=affiliations,
             owner_affiliations=owner_affiliations,
             is_locked=is_locked,
             after=after,
@@ -1003,15 +1067,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).pinnable_items(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).pinnable_items(
         **strip_kwargs(
             types=types,
             after=after,
             before=before,
             first=first,
             last=last,
         )
@@ -1054,15 +1122,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).recent_projects(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).recent_projects(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
         )
     )
@@ -1111,15 +1183,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).member_statuses(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).member_statuses(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
             order_by=order_by,
         )
@@ -1162,15 +1238,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).pending_members(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).pending_members(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
         )
     )
@@ -1249,15 +1329,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).members_with_role(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).members_with_role(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
         )
     )
@@ -1309,15 +1393,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).enterprise_owners(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).enterprise_owners(
         **strip_kwargs(
             query=query,
             organization_role=organization_role,
             order_by=order_by,
             after=after,
             before=before,
             first=first,
@@ -1375,15 +1463,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).sponsors_activities(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).sponsors_activities(
         **strip_kwargs(
             actions=actions,
             after=after,
             before=before,
             first=first,
             last=last,
             period=period,
@@ -1472,15 +1564,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).ip_allow_list_entries(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).ip_allow_list_entries(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
             order_by=order_by,
         )
@@ -1535,15 +1631,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).repository_migrations(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).repository_migrations(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
             state=state,
             repository_name=repository_name,
@@ -1640,15 +1740,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.organization(**strip_kwargs(login=login,)).repository_discussions(
+    op_selection = op.organization(
+        **strip_kwargs(
+            login=login,
+        )
+    ).repository_discussions(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
             order_by=order_by,
             repository_id=repository_id,
```

### Comparing `prefect-github-0.2.2/prefect_github/repository.py` & `prefect_github-0.2.3/prefect_github/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 from datetime import datetime
 from distutils.dir_util import copy_tree
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Any, Dict, Iterable, Optional, Tuple, Union
 from urllib.parse import urlparse, urlunparse
 
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect import task
 from prefect.filesystems import ReadableDeploymentStorage
 from prefect.utilities.asyncutils import sync_compatible
 from prefect.utilities.processutils import run_process
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field, validator
 else:
     from pydantic import Field, validator
 
 from sgqlc.operation import Operation
```

### Comparing `prefect-github-0.2.2/prefect_github/repository_owner.py` & `prefect_github-0.2.3/prefect_github/repository_owner.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 # This module was auto-generated using prefect-collection-generator so
 # manually editing this file is not recommended. If this module
 # is outdated, rerun scripts/generate.py.
 
 from pathlib import Path
 from typing import Any, Dict, Iterable
 
-from prefect import task
 from sgqlc.operation import Operation
 
+from prefect import task
 from prefect_github import GitHubCredentials
 from prefect_github.graphql import _execute_graphql_op, _subset_return_fields
 from prefect_github.schemas import graphql_schema
 from prefect_github.utils import initialize_return_fields_defaults, strip_kwargs
 
 config_path = (
     Path(__file__).parent.resolve() / "configs" / "query" / "repository_owner.json"
@@ -78,15 +78,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.repository_owner(**strip_kwargs(login=login,)).repository(
+    op_selection = op.repository_owner(
+        **strip_kwargs(
+            login=login,
+        )
+    ).repository(
         **strip_kwargs(
             name=name,
             follow_renames=follow_renames,
         )
     )
 
     op_stack = (
@@ -151,15 +155,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.repository_owner(**strip_kwargs(login=login,)).repositories(
+    op_selection = op.repository_owner(
+        **strip_kwargs(
+            login=login,
+        )
+    ).repositories(
         **strip_kwargs(
             privacy=privacy,
             order_by=order_by,
             affiliations=affiliations,
             owner_affiliations=owner_affiliations,
             is_locked=is_locked,
             after=after,
```

### Comparing `prefect-github-0.2.2/prefect_github/schemas/graphql_schema.py` & `prefect_github-0.2.3/prefect_github/schemas/graphql_schema.py`

 * *Files identical despite different names*

### Comparing `prefect-github-0.2.2/prefect_github/user.py` & `prefect_github-0.2.3/prefect_github/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 # manually editing this file is not recommended. If this module
 # is outdated, rerun scripts/generate.py.
 
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Dict, Iterable
 
-from prefect import task
 from sgqlc.operation import Operation
 
+from prefect import task
 from prefect_github import GitHubCredentials
 from prefect_github.graphql import _execute_graphql_op, _subset_return_fields
 from prefect_github.schemas import graphql_schema
 from prefect_github.utils import initialize_return_fields_defaults, strip_kwargs
 
 config_path = Path(__file__).parent.resolve() / "configs" / "query" / "user.json"
 return_fields_defaults = initialize_return_fields_defaults(config_path)
@@ -74,15 +74,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).gist(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).gist(
         **strip_kwargs(
             name=name,
         )
     )
 
     op_stack = (
         "user",
@@ -125,15 +129,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).gists(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).gists(
         **strip_kwargs(
             privacy=privacy,
             order_by=order_by,
             after=after,
             before=before,
             first=first,
             last=last,
@@ -187,15 +195,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).issues(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).issues(
         **strip_kwargs(
             labels=labels,
             states=states,
             order_by=order_by,
             filter_by=filter_by,
             after=after,
             before=before,
@@ -270,15 +282,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).project(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).project(
         **strip_kwargs(
             number=number,
         )
     )
 
     op_stack = (
         "user",
@@ -328,15 +344,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).packages(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).packages(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
             names=names,
             repository_id=repository_id,
@@ -390,15 +410,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).projects(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).projects(
         **strip_kwargs(
             states=states,
             order_by=order_by,
             search=search,
             after=after,
             before=before,
             first=first,
@@ -450,15 +474,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).sponsors(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).sponsors(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
             tier_id=tier_id,
             order_by=order_by,
@@ -523,15 +551,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).watching(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).watching(
         **strip_kwargs(
             privacy=privacy,
             order_by=order_by,
             affiliations=affiliations,
             owner_affiliations=owner_affiliations,
             is_locked=is_locked,
             after=after,
@@ -570,15 +602,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).project_v2(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).project_v2(
         **strip_kwargs(
             number=number,
         )
     )
 
     op_stack = (
         "user",
@@ -617,15 +653,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).followers(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).followers(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
         )
     )
@@ -667,15 +707,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).following(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).following(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
         )
     )
@@ -721,15 +765,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).projects_v2(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).projects_v2(
         **strip_kwargs(
             query=query,
             order_by=order_by,
             after=after,
             before=before,
             first=first,
             last=last,
@@ -768,15 +816,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).repository(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).repository(
         **strip_kwargs(
             name=name,
             follow_renames=follow_renames,
         )
     )
 
     op_stack = (
@@ -819,15 +871,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).sponsoring(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).sponsoring(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
             order_by=order_by,
         )
@@ -870,15 +926,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).public_keys(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).public_keys(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
         )
     )
@@ -912,15 +972,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).project_next(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).project_next(
         **strip_kwargs(
             number=number,
         )
     )
 
     op_stack = (
         "user",
@@ -961,15 +1025,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).pinned_items(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).pinned_items(
         **strip_kwargs(
             types=types,
             after=after,
             before=before,
             first=first,
             last=last,
         )
@@ -1016,15 +1084,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).projects_next(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).projects_next(
         **strip_kwargs(
             query=query,
             sort_by=sort_by,
             after=after,
             before=before,
             first=first,
             last=last,
@@ -1093,15 +1165,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).repositories(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).repositories(
         **strip_kwargs(
             privacy=privacy,
             order_by=order_by,
             affiliations=affiliations,
             owner_affiliations=owner_affiliations,
             is_locked=is_locked,
             after=after,
@@ -1187,15 +1263,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).gist_comments(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).gist_comments(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
         )
     )
@@ -1229,15 +1309,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).organization(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).organization(
         **strip_kwargs(
             login=organization_login,
         )
     )
 
     op_stack = (
         "user",
@@ -1290,15 +1374,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).pull_requests(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).pull_requests(
         **strip_kwargs(
             states=states,
             labels=labels,
             head_ref_name=head_ref_name,
             base_ref_name=base_ref_name,
             order_by=order_by,
             after=after,
@@ -1350,15 +1438,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).saved_replies(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).saved_replies(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
             order_by=order_by,
         )
@@ -1404,15 +1496,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).pinnable_items(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).pinnable_items(
         **strip_kwargs(
             types=types,
             after=after,
             before=before,
             first=first,
             last=last,
         )
@@ -1458,15 +1554,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).issue_comments(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).issue_comments(
         **strip_kwargs(
             order_by=order_by,
             after=after,
             before=before,
             first=first,
             last=last,
         )
@@ -1509,15 +1609,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).organizations(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).organizations(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
         )
     )
@@ -1559,15 +1663,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).recent_projects(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).recent_projects(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
         )
     )
@@ -1609,15 +1717,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).commit_comments(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).commit_comments(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
         )
     )
@@ -1703,15 +1815,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).top_repositories(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).top_repositories(
         **strip_kwargs(
             order_by=order_by,
             after=after,
             before=before,
             first=first,
             last=last,
             since=since,
@@ -1768,15 +1884,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).sponsors_activities(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).sponsors_activities(
         **strip_kwargs(
             actions=actions,
             after=after,
             before=before,
             first=first,
             last=last,
             period=period,
@@ -1864,15 +1984,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).starred_repositories(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).starred_repositories(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
             owned_by_viewer=owned_by_viewer,
             order_by=order_by,
@@ -1931,15 +2055,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).repository_discussions(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).repository_discussions(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
             order_by=order_by,
             repository_id=repository_id,
@@ -1991,15 +2119,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).sponsorships_as_sponsor(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).sponsorships_as_sponsor(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
             order_by=order_by,
         )
@@ -2050,15 +2182,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).sponsorship_newsletters(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).sponsorship_newsletters(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
             order_by=order_by,
         )
@@ -2102,15 +2238,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).contributions_collection(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).contributions_collection(
         **strip_kwargs(
             organization_id=organization_id,
             from_=from_,
             to=to,
         )
     )
 
@@ -2161,15 +2301,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).sponsorships_as_maintainer(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).sponsorships_as_maintainer(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
             include_private=include_private,
             order_by=order_by,
@@ -2231,15 +2375,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).repositories_contributed_to(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).repositories_contributed_to(
         **strip_kwargs(
             privacy=privacy,
             order_by=order_by,
             is_locked=is_locked,
             include_user_repositories=include_user_repositories,
             contribution_types=contribution_types,
             after=after,
@@ -2294,15 +2442,19 @@
         return_fields: Subset the return fields (as snake_case); defaults to
             fields listed in configs/query/*.json.
 
     Returns:
         A dict of the returned fields.
     """
     op = Operation(graphql_schema.Query)
-    op_selection = op.user(**strip_kwargs(login=login,)).repository_discussion_comments(
+    op_selection = op.user(
+        **strip_kwargs(
+            login=login,
+        )
+    ).repository_discussion_comments(
         **strip_kwargs(
             after=after,
             before=before,
             first=first,
             last=last,
             repository_id=repository_id,
             only_answers=only_answers,
```

### Comparing `prefect-github-0.2.2/prefect_github/utils.py` & `prefect_github-0.2.3/prefect_github/utils.py`

 * *Files identical despite different names*

### Comparing `prefect-github-0.2.2/prefect_github/viewer.py` & `prefect_github-0.2.3/prefect_github/viewer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 # manually editing this file is not recommended. If this module
 # is outdated, rerun scripts/generate.py.
 
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Dict, Iterable
 
-from prefect import task
 from sgqlc.operation import Operation
 
+from prefect import task
 from prefect_github import GitHubCredentials
 from prefect_github.graphql import _execute_graphql_op, _subset_return_fields
 from prefect_github.schemas import graphql_schema
 from prefect_github.utils import initialize_return_fields_defaults, strip_kwargs
 
 config_path = Path(__file__).parent.resolve() / "configs" / "query" / "viewer.json"
 return_fields_defaults = initialize_return_fields_defaults(config_path)
```

### Comparing `prefect-github-0.2.2/prefect_github.egg-info/PKG-INFO` & `prefect_github-0.2.3/prefect_github.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,98 +1,85 @@
 Metadata-Version: 2.1
 Name: prefect-github
-Version: 0.2.2
+Version: 0.2.3
 Summary: Prefect integrations interacting with GitHub
-Home-page: https://github.com/PrefectHQ/prefect-github
-Author: Prefect Technologies Inc.
-Author-email: help@prefect.io
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-github
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: sgqlc>=15.0
 Requires-Dist: prefect>=2.13.5
 Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: interrogate; extra == "dev"
+Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: isort; extra == "dev"
+Requires-Dist: mock; python_version < "3.8" and extra == "dev"
+Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev"
-Requires-Dist: mkdocs-gen-files; extra == "dev"
-Requires-Dist: interrogate; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
-Requires-Dist: pillow; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
 
 # prefect-github
  
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-github/" alt="PyPI version">
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-github?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-github/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-github?color=0052FF&labelColor=090422" /></a>
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-github?color=26272B&labelColor=090422"></a>
     <a href="https://pepy.tech/badge/prefect-github/" alt="Downloads">
-        <img src="https://img.shields.io/pypi/dm/prefect-github?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-github/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-github?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
+        <img src="https://img.shields.io/pypi/dm/prefect-github?color=26272B&labelColor=090422" /></a>
 </p>
 
 ## Welcome!
 
 Prefect integrations interacting with GitHub.
 
 The tasks within this collection were created by a code generator using the GitHub GraphQL schema.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.7+.
+Requires an installation of Python 3.8 or newer.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
-These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://orion-docs.prefect.io/).
+These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
 
 Install `prefect-github` with `pip`:
 
 ```bash
 pip install prefect-github
 ```
 
-Then, register to [view the block](https://orion-docs.prefect.io/ui/blocks/) on Prefect Cloud:
+Then, register to [view the block](https://docs.prefect.io/ui/blocks/) on Prefect Cloud:
 
 ```bash
 prefect block register -m prefect_github
 ```
 
-Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
+Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or saved through the UI.
 
 ### Write and run a flow
 
 ```python
 from prefect import flow
 from prefect_github import GitHubCredentials
 from prefect_github.repository import query_repository
@@ -118,15 +105,15 @@
 github_add_star_flow()
 ```
 
 ## Resources
 
 If you encounter any bugs while using `prefect-github`, feel free to open an issue in the [prefect-github](https://github.com/PrefectHQ/prefect-github) repository.
 
-If you have any questions or issues while using `prefect-github`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
+If you have any questions or issues while using `prefect-github`, you can find help in the [Prefect Slack community](https://prefect.io/slack).
 
 Feel free to ⭐️ or watch [`prefect-github`](https://github.com/PrefectHQ/prefect-github) for updates too!
 
 ## Development
 
 If you'd like to install a version of `prefect-github` for development, clone the repository and perform an editable install with `pip`:
```

### Comparing `prefect-github-0.2.2/prefect_github.egg-info/SOURCES.txt` & `prefect_github-0.2.3/prefect_github.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,9 @@
-LICENSE
-MANIFEST.in
 README.md
-requirements-dev.txt
-requirements.txt
-setup.cfg
-setup.py
-versioneer.py
+pyproject.toml
 prefect_github/__init__.py
 prefect_github/_version.py
 prefect_github/credentials.py
 prefect_github/exceptions.py
 prefect_github/graphql.py
 prefect_github/mutations.py
 prefect_github/organization.py
@@ -37,13 +31,16 @@
 prefect_github/configs/mutation/request_reviews.json
 prefect_github/configs/query/organization.json
 prefect_github/configs/query/repository.json
 prefect_github/configs/query/repository_owner.json
 prefect_github/configs/query/user.json
 prefect_github/configs/query/viewer.json
 prefect_github/schemas/__init__.py
+prefect_github/schemas/graphql_schema.json
 prefect_github/schemas/graphql_schema.py
+tests/conftest.py
 tests/test_block_standards.py
 tests/test_credentials.py
 tests/test_graphql.py
 tests/test_repository.py
-tests/test_utils.py
+tests/test_utils.py
+tests/test_version.py
```

### Comparing `prefect-github-0.2.2/tests/test_credentials.py` & `prefect_github-0.2.3/tests/test_credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pytest
-from sgqlc.endpoint.http import HTTPEndpoint
-
 from prefect_github import GitHubCredentials
+from sgqlc.endpoint.http import HTTPEndpoint
 
 
 @pytest.mark.parametrize("token", [None, "token_value"])
 def test_github_credentials_get_endpoint(token):
     endpoint = GitHubCredentials(token=token).get_endpoint()
     assert isinstance(endpoint, HTTPEndpoint)
     if token is not None:
```

### Comparing `prefect-github-0.2.2/tests/test_graphql.py` & `prefect_github-0.2.3/tests/test_graphql.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
-from prefect import flow
-from sgqlc.operation import Operation, Selector
-
 from prefect_github.graphql import _subset_return_fields, execute_graphql
 from prefect_github.schemas import graphql_schema
+from sgqlc.operation import Operation, Selector
+
+from prefect import flow
 
 
 @pytest.mark.parametrize(
     "return_fields_key", ["return_fields", "return_fields_defaults"]
 )
 def test_subset_return_fields(return_fields_key):
     op = Operation(graphql_schema.Query)
```

### Comparing `prefect-github-0.2.2/tests/test_repository.py` & `prefect_github-0.2.3/tests/test_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Tuple
 
 import pytest
-from prefect.testing.utilities import AsyncMock
 from pydantic import VERSION as PYDANTIC_VERSION
 
+from prefect.testing.utilities import AsyncMock
+
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1.error_wrappers import ValidationError
 else:
     from pydantic.error_wrappers import ValidationError
 
 import prefect_github
 from prefect_github import GitHubCredentials
@@ -141,17 +142,15 @@
 
         def __enter__(self):
             return self.dir
 
         def __exit__(self, *args, **kwargs):
             pass
 
-    async def test_dir_contents_copied_correctly_with_get_directory(
-        self, monkeypatch
-    ):  # noqa
+    async def test_dir_contents_copied_correctly_with_get_directory(self, monkeypatch):  # noqa
         """Check that `get_directory` is able to correctly copy contents from src->dst"""  # noqa
 
         class p:
             returncode = 0
 
         mock = AsyncMock(return_value=p())
         monkeypatch.setattr(prefect_github.repository, "run_process", mock)
```

### Comparing `prefect-github-0.2.2/tests/test_utils.py` & `prefect_github-0.2.3/tests/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 
 import pytest
-
 from prefect_github.utils import (
     camel_to_snake_case,
     initialize_return_fields_defaults,
     strip_kwargs,
 )
 
 test_config = {"categories": [{"category": ["title", "alias"]}, "total"]}
```


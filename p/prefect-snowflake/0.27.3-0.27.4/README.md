# Comparing `tmp/prefect-snowflake-0.27.3.tar.gz` & `tmp/prefect_snowflake-0.27.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-snowflake-0.27.3.tar", last modified: Fri Jan 19 21:16:53 2024, max compression
+gzip compressed data, was "prefect_snowflake-0.27.4.tar", last modified: Thu Apr 25 19:14:19 2024, max compression
```

## Comparing `prefect-snowflake-0.27.3.tar` & `prefect_snowflake-0.27.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 21:16:53.219792 prefect-snowflake-0.27.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-01-19 21:16:10.000000 prefect-snowflake-0.27.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-01-19 21:16:10.000000 prefect-snowflake-0.27.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12333 2024-01-19 21:16:53.219792 prefect-snowflake-0.27.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-01-19 21:16:10.000000 prefect-snowflake-0.27.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 21:16:53.219792 prefect-snowflake-0.27.3/prefect_snowflake/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-19 21:16:10.000000 prefect-snowflake-0.27.3/prefect_snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-01-19 21:16:53.219792 prefect-snowflake-0.27.3/prefect_snowflake/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-01-19 21:16:10.000000 prefect-snowflake-0.27.3/prefect_snowflake/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    30138 2024-01-19 21:16:10.000000 prefect-snowflake-0.27.3/prefect_snowflake/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 21:16:53.219792 prefect-snowflake-0.27.3/prefect_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12333 2024-01-19 21:16:53.000000 prefect-snowflake-0.27.3/prefect_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-01-19 21:16:53.000000 prefect-snowflake-0.27.3/prefect_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 21:16:53.000000 prefect-snowflake-0.27.3/prefect_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-19 21:16:53.000000 prefect-snowflake-0.27.3/prefect_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-01-19 21:16:53.000000 prefect-snowflake-0.27.3/prefect_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-19 21:16:53.000000 prefect-snowflake-0.27.3/prefect_snowflake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-19 21:16:10.000000 prefect-snowflake-0.27.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-19 21:16:10.000000 prefect-snowflake-0.27.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-01-19 21:16:53.219792 prefect-snowflake-0.27.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-01-19 21:16:10.000000 prefect-snowflake-0.27.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 21:16:53.219792 prefect-snowflake-0.27.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-01-19 21:16:10.000000 prefect-snowflake-0.27.3/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)    16773 2024-01-19 21:16:10.000000 prefect-snowflake-0.27.3/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-01-19 21:16:10.000000 prefect-snowflake-0.27.3/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    80049 2024-01-19 21:16:10.000000 prefect-snowflake-0.27.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:14:19.647247 prefect_snowflake-0.27.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-04-25 19:14:19.647247 prefect_snowflake-0.27.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9569 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:14:19.643247 prefect_snowflake-0.27.4/prefect_snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/prefect_snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-25 19:14:19.000000 prefect_snowflake-0.27.4/prefect_snowflake/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12965 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/prefect_snowflake/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30139 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/prefect_snowflake/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:14:19.643247 prefect_snowflake-0.27.4/prefect_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-04-25 19:14:19.000000 prefect_snowflake-0.27.4/prefect_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-25 19:14:19.000000 prefect_snowflake-0.27.4/prefect_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:14:19.000000 prefect_snowflake-0.27.4/prefect_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-25 19:14:19.000000 prefect_snowflake-0.27.4/prefect_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-25 19:14:19.000000 prefect_snowflake-0.27.4/prefect_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 19:14:19.000000 prefect_snowflake-0.27.4/prefect_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:14:19.647247 prefect_snowflake-0.27.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:14:19.643247 prefect_snowflake-0.27.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16774 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/tests/test_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:14:19.643247 prefect_snowflake-0.27.4/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/tests/test_data/test_cert.p8
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/tests/test_data/test_cert_malformed_format.p8
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/tests/test_data/test_cert_no_pass.p8
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-25 19:14:07.000000 prefect_snowflake-0.27.4/tests/test_version.py
```

### Comparing `prefect-snowflake-0.27.3/PKG-INFO` & `prefect_snowflake-0.27.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,54 @@
 Metadata-Version: 2.1
 Name: prefect-snowflake
-Version: 0.27.3
-Summary: Prefect integrations for interacting with Snowflake.
-Home-page: https://github.com/PrefectHQ/prefect-snowflake
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Version: 0.27.4
+Summary: Prefect integrations for interacting with Snowflake
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-snowflake
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
-Requires-Dist: prefect>=2.13.5
 Requires-Dist: snowflake-connector-python>=2.7.6
+Requires-Dist: prefect>=2.13.5
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
-Requires-Dist: mkdocstrings_python_legacy; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: mock; python_version < "3.8" and extra == "dev"
-Requires-Dist: mkdocs-gen-files; extra == "dev"
-Requires-Dist: interrogate; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
 
 # prefect-snowflake
 
 <p align="center">
-    <img src="https://user-images.githubusercontent.com/15331990/217983397-036ddfd1-22c4-4113-8045-d5d9e43b963c.png">
-    <br>
     <a href="https://pypi.python.org/pypi/prefect-snowflake/" alt="PyPI version">
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-snowflake?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-snowflake/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-snowflake?color=0052FF&labelColor=090422" /></a>
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-snowflake?color=26272B&labelColor=090422"></a>
     <a href="https://pepy.tech/badge/prefect-snowflake/" alt="Downloads">
-        <img src="https://img.shields.io/pypi/dm/prefect-snowflake?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-snowflake/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-snowflake?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
+        <img src="https://img.shields.io/pypi/dm/prefect-snowflake?color=26272B&labelColor=090422" /></a>
 </p>
 
-Visit the full docs [here](https://PrefectHQ.github.io/prefect-snowflake) to see additional examples and the API reference.
-
 ## Welcome!
 
 The prefect-snowflake collection makes it easy to connect to a Snowflake database in your Prefect flows. Check out the examples below to get started!
 
 ## Getting Started
 
 ### Integrate with Prefect flows
@@ -198,35 +182,35 @@
             database=snowflake_connector.database,
             schema=snowflake_connector.schema_  # note the "_" suffix
         )
 ```
 
 ## Resources
 
-For more tips on how to use tasks and flows in a Collection, check out [Using Collections](https://orion-docs.prefect.io/collections/usage/)!
+For more tips on how to use tasks and flows in an integration, check out [Using Collections](https://docs.prefect.io/integrations/usage/)!
 
 ### Installation
 
 Install `prefect-snowflake` with `pip`:
 
 ```bash
 pip install prefect-snowflake
 ```
 
 A list of available blocks in `prefect-snowflake` and their setup instructions can be found [here](https://PrefectHQ.github.io/prefect-snowflake/blocks_catalog).
 
-Requires an installation of Python 3.7+.
+Requires an installation of Python 3.8+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
-These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://orion-docs.prefect.io/).
+These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Saving credentials to block
 
-Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
+Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://docs.prefect.io/concepts/blocks/#saving-blocks) or saved through the UI.
 
 Below is a walkthrough on saving a `SnowflakeCredentials` block through code.
 
 1. Head over to https://app.snowflake.com/.
 2. Login to your Snowflake account, e.g. nh12345.us-east-2.aws, with your username and password.
 3. Use those credentials to fill replace the placeholders below.
 
@@ -270,15 +254,15 @@
 SnowflakeCredentials.load("CREDENTIALS-BLOCK-NAME-PLACEHOLDER")
 SnowflakeConnector.load("CONNECTOR-BLOCK-NAME-PLACEHOLDER")
 ```
 
 !!! info "Registering blocks"
 
 Register blocks in this module to
-[view and edit them](https://orion-docs.prefect.io/ui/blocks/)
+[view and edit them](https://docs.prefect.io/ui/blocks/)
 on Prefect Cloud:
 
 ```bash
 prefect block register -m prefect_snowflake
 ```
 
 A list of available blocks in `prefect-snowflake` and their setup instructions can be found [here](https://PrefectHQ.github.io/prefect-snowflake/blocks_catalog).
```

### Comparing `prefect-snowflake-0.27.3/README.md` & `prefect_snowflake-0.27.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,16 @@
 # prefect-snowflake
 
 <p align="center">
-    <img src="https://user-images.githubusercontent.com/15331990/217983397-036ddfd1-22c4-4113-8045-d5d9e43b963c.png">
-    <br>
     <a href="https://pypi.python.org/pypi/prefect-snowflake/" alt="PyPI version">
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-snowflake?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-snowflake/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-snowflake?color=0052FF&labelColor=090422" /></a>
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-snowflake?color=26272B&labelColor=090422"></a>
     <a href="https://pepy.tech/badge/prefect-snowflake/" alt="Downloads">
-        <img src="https://img.shields.io/pypi/dm/prefect-snowflake?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-snowflake/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-snowflake?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
+        <img src="https://img.shields.io/pypi/dm/prefect-snowflake?color=26272B&labelColor=090422" /></a>
 </p>
 
-Visit the full docs [here](https://PrefectHQ.github.io/prefect-snowflake) to see additional examples and the API reference.
-
 ## Welcome!
 
 The prefect-snowflake collection makes it easy to connect to a Snowflake database in your Prefect flows. Check out the examples below to get started!
 
 ## Getting Started
 
 ### Integrate with Prefect flows
@@ -157,35 +144,35 @@
             database=snowflake_connector.database,
             schema=snowflake_connector.schema_  # note the "_" suffix
         )
 ```
 
 ## Resources
 
-For more tips on how to use tasks and flows in a Collection, check out [Using Collections](https://orion-docs.prefect.io/collections/usage/)!
+For more tips on how to use tasks and flows in an integration, check out [Using Collections](https://docs.prefect.io/integrations/usage/)!
 
 ### Installation
 
 Install `prefect-snowflake` with `pip`:
 
 ```bash
 pip install prefect-snowflake
 ```
 
 A list of available blocks in `prefect-snowflake` and their setup instructions can be found [here](https://PrefectHQ.github.io/prefect-snowflake/blocks_catalog).
 
-Requires an installation of Python 3.7+.
+Requires an installation of Python 3.8+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
-These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://orion-docs.prefect.io/).
+These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Saving credentials to block
 
-Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
+Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://docs.prefect.io/concepts/blocks/#saving-blocks) or saved through the UI.
 
 Below is a walkthrough on saving a `SnowflakeCredentials` block through code.
 
 1. Head over to https://app.snowflake.com/.
 2. Login to your Snowflake account, e.g. nh12345.us-east-2.aws, with your username and password.
 3. Use those credentials to fill replace the placeholders below.
 
@@ -229,15 +216,15 @@
 SnowflakeCredentials.load("CREDENTIALS-BLOCK-NAME-PLACEHOLDER")
 SnowflakeConnector.load("CONNECTOR-BLOCK-NAME-PLACEHOLDER")
 ```
 
 !!! info "Registering blocks"
 
 Register blocks in this module to
-[view and edit them](https://orion-docs.prefect.io/ui/blocks/)
+[view and edit them](https://docs.prefect.io/ui/blocks/)
 on Prefect Cloud:
 
 ```bash
 prefect block register -m prefect_snowflake
 ```
 
 A list of available blocks in `prefect-snowflake` and their setup instructions can be found [here](https://PrefectHQ.github.io/prefect-snowflake/blocks_catalog).
```

### Comparing `prefect-snowflake-0.27.3/prefect_snowflake/credentials.py` & `prefect_snowflake-0.27.4/prefect_snowflake/credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 import snowflake.connector
-from prefect.blocks.abstract import CredentialsBlock
 from pydantic import VERSION as PYDANTIC_VERSION
 
+from prefect.blocks.abstract import CredentialsBlock
+
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field, SecretBytes, SecretField, SecretStr, root_validator
 else:
     from pydantic import Field, SecretBytes, SecretField, SecretStr, root_validator
 
 # PEM certificates have the pattern:
 #   -----BEGIN PRIVATE KEY-----
```

### Comparing `prefect-snowflake-0.27.3/prefect_snowflake/database.py` & `prefect_snowflake-0.27.4/prefect_snowflake/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Module for querying against Snowflake databases."""
 
 import asyncio
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect import task
 from prefect.blocks.abstract import DatabaseBlock
 from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
 from prefect.utilities.hashing import hash_objects
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field
 else:
     from pydantic import Field
 
 from snowflake.connector.connection import SnowflakeConnection
@@ -20,15 +21,14 @@
 from prefect_snowflake import SnowflakeCredentials
 
 BEGIN_TRANSACTION_STATEMENT = "BEGIN TRANSACTION"
 END_TRANSACTION_STATEMENT = "COMMIT"
 
 
 class SnowflakeConnector(DatabaseBlock):
-
     """
     Block used to manage connections with Snowflake.
 
     Upon instantiating, a connection is created and maintained for the life of
     the object until the close method is called.
 
     It is recommended to use this block as a context manager, which will automatically
@@ -770,15 +770,15 @@
             snowflake_connector = SnowflakeConnector(
                 database="database",
                 warehouse="warehouse",
                 schema="schema",
                 credentials=snowflake_credentials
             )
             result = snowflake_query_sync(
-                "put file://afile.csv @mystage;",
+                "put file://a_file.csv @mystage;",
                 snowflake_connector,
             )
             return result
 
         snowflake_query_sync_flow()
         ```
     """
```

### Comparing `prefect-snowflake-0.27.3/prefect_snowflake.egg-info/PKG-INFO` & `prefect_snowflake-0.27.4/prefect_snowflake.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,54 @@
 Metadata-Version: 2.1
 Name: prefect-snowflake
-Version: 0.27.3
-Summary: Prefect integrations for interacting with Snowflake.
-Home-page: https://github.com/PrefectHQ/prefect-snowflake
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Version: 0.27.4
+Summary: Prefect integrations for interacting with Snowflake
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-snowflake
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
-Requires-Dist: prefect>=2.13.5
 Requires-Dist: snowflake-connector-python>=2.7.6
+Requires-Dist: prefect>=2.13.5
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
-Requires-Dist: mkdocstrings_python_legacy; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: mock; python_version < "3.8" and extra == "dev"
-Requires-Dist: mkdocs-gen-files; extra == "dev"
-Requires-Dist: interrogate; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
 
 # prefect-snowflake
 
 <p align="center">
-    <img src="https://user-images.githubusercontent.com/15331990/217983397-036ddfd1-22c4-4113-8045-d5d9e43b963c.png">
-    <br>
     <a href="https://pypi.python.org/pypi/prefect-snowflake/" alt="PyPI version">
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-snowflake?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-snowflake/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-snowflake?color=0052FF&labelColor=090422" /></a>
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-snowflake?color=26272B&labelColor=090422"></a>
     <a href="https://pepy.tech/badge/prefect-snowflake/" alt="Downloads">
-        <img src="https://img.shields.io/pypi/dm/prefect-snowflake?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-snowflake/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-snowflake?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
+        <img src="https://img.shields.io/pypi/dm/prefect-snowflake?color=26272B&labelColor=090422" /></a>
 </p>
 
-Visit the full docs [here](https://PrefectHQ.github.io/prefect-snowflake) to see additional examples and the API reference.
-
 ## Welcome!
 
 The prefect-snowflake collection makes it easy to connect to a Snowflake database in your Prefect flows. Check out the examples below to get started!
 
 ## Getting Started
 
 ### Integrate with Prefect flows
@@ -198,35 +182,35 @@
             database=snowflake_connector.database,
             schema=snowflake_connector.schema_  # note the "_" suffix
         )
 ```
 
 ## Resources
 
-For more tips on how to use tasks and flows in a Collection, check out [Using Collections](https://orion-docs.prefect.io/collections/usage/)!
+For more tips on how to use tasks and flows in an integration, check out [Using Collections](https://docs.prefect.io/integrations/usage/)!
 
 ### Installation
 
 Install `prefect-snowflake` with `pip`:
 
 ```bash
 pip install prefect-snowflake
 ```
 
 A list of available blocks in `prefect-snowflake` and their setup instructions can be found [here](https://PrefectHQ.github.io/prefect-snowflake/blocks_catalog).
 
-Requires an installation of Python 3.7+.
+Requires an installation of Python 3.8+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
-These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://orion-docs.prefect.io/).
+These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Saving credentials to block
 
-Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
+Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://docs.prefect.io/concepts/blocks/#saving-blocks) or saved through the UI.
 
 Below is a walkthrough on saving a `SnowflakeCredentials` block through code.
 
 1. Head over to https://app.snowflake.com/.
 2. Login to your Snowflake account, e.g. nh12345.us-east-2.aws, with your username and password.
 3. Use those credentials to fill replace the placeholders below.
 
@@ -270,15 +254,15 @@
 SnowflakeCredentials.load("CREDENTIALS-BLOCK-NAME-PLACEHOLDER")
 SnowflakeConnector.load("CONNECTOR-BLOCK-NAME-PLACEHOLDER")
 ```
 
 !!! info "Registering blocks"
 
 Register blocks in this module to
-[view and edit them](https://orion-docs.prefect.io/ui/blocks/)
+[view and edit them](https://docs.prefect.io/ui/blocks/)
 on Prefect Cloud:
 
 ```bash
 prefect block register -m prefect_snowflake
 ```
 
 A list of available blocks in `prefect-snowflake` and their setup instructions can be found [here](https://PrefectHQ.github.io/prefect-snowflake/blocks_catalog).
```

### Comparing `prefect-snowflake-0.27.3/prefect_snowflake.egg-info/SOURCES.txt` & `prefect_snowflake-0.27.4/prefect_snowflake.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-LICENSE
-MANIFEST.in
 README.md
-requirements-dev.txt
-requirements.txt
-setup.cfg
-setup.py
-versioneer.py
+pyproject.toml
 prefect_snowflake/__init__.py
 prefect_snowflake/_version.py
 prefect_snowflake/credentials.py
 prefect_snowflake/database.py
 prefect_snowflake.egg-info/PKG-INFO
 prefect_snowflake.egg-info/SOURCES.txt
 prefect_snowflake.egg-info/dependency_links.txt
 prefect_snowflake.egg-info/entry_points.txt
 prefect_snowflake.egg-info/requires.txt
 prefect_snowflake.egg-info/top_level.txt
+tests/conftest.py
 tests/test_block_standards.py
 tests/test_credentials.py
-tests/test_database.py
+tests/test_database.py
+tests/test_version.py
+tests/test_data/test_cert.p8
+tests/test_data/test_cert_malformed_format.p8
+tests/test_data/test_cert_no_pass.p8
```

### Comparing `prefect-snowflake-0.27.3/tests/test_block_standards.py` & `prefect_snowflake-0.27.4/tests/test_block_standards.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from prefect.blocks.core import Block
 from prefect.testing.standard_test_suites import BlockStandardTestSuite
 from prefect.utilities.dispatch import get_registry_for_type
 from prefect.utilities.importtools import to_qualified_name
 
 
 def find_module_blocks():
```

### Comparing `prefect-snowflake-0.27.3/tests/test_credentials.py` & `prefect_snowflake-0.27.4/tests/test_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import sys
 from pathlib import Path
 from unittest.mock import MagicMock
 
 import pytest
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect import flow
 from prefect.utilities.filesystem import relative_path_to_current_platform
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import SecretBytes, SecretStr
 else:
     from pydantic import SecretBytes, SecretStr
 
 from prefect_snowflake.credentials import InvalidPemFormat, SnowflakeCredentials
```

### Comparing `prefect-snowflake-0.27.3/tests/test_database.py` & `prefect_snowflake-0.27.4/tests/test_database.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from unittest.mock import MagicMock
 
 import pytest
-from prefect import flow
 from pydantic import VERSION as PYDANTIC_VERSION
 
+from prefect import flow
+
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import SecretBytes, SecretStr
 else:
     from pydantic import SecretBytes, SecretStr
 
-from snowflake.connector import DictCursor
-from snowflake.connector.cursor import SnowflakeCursor as OriginalSnowflakeCursorClass
-
 from prefect_snowflake.database import (
     BEGIN_TRANSACTION_STATEMENT,
     END_TRANSACTION_STATEMENT,
     SnowflakeConnector,
     snowflake_multiquery,
     snowflake_query,
     snowflake_query_sync,
 )
+from snowflake.connector import DictCursor
+from snowflake.connector.cursor import SnowflakeCursor as OriginalSnowflakeCursorClass
 
 
 def test_snowflake_connector_init(connector_params):
     snowflake_connector = SnowflakeConnector(**connector_params)
     actual_connector_params = snowflake_connector.dict()
     for param in connector_params:
         expected = connector_params[param]
```


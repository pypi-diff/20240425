# Comparing `tmp/prefect-bitbucket-0.2.2.tar.gz` & `tmp/prefect_bitbucket-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-bitbucket-0.2.2.tar", last modified: Wed Nov 29 19:56:09 2023, max compression
+gzip compressed data, was "prefect_bitbucket-0.2.3.tar", last modified: Thu Apr 25 19:20:30 2024, max compression
```

## Comparing `prefect-bitbucket-0.2.2.tar` & `prefect_bitbucket-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:56:09.455529 prefect-bitbucket-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-11-29 19:55:25.000000 prefect-bitbucket-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      324 2023-11-29 19:55:25.000000 prefect-bitbucket-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8247 2023-11-29 19:56:09.455529 prefect-bitbucket-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2023-11-29 19:55:25.000000 prefect-bitbucket-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:56:09.455529 prefect-bitbucket-0.2.2/prefect_bitbucket/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-11-29 19:55:25.000000 prefect-bitbucket-0.2.2/prefect_bitbucket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-11-29 19:56:09.455529 prefect-bitbucket-0.2.2/prefect_bitbucket/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2023-11-29 19:55:25.000000 prefect-bitbucket-0.2.2/prefect_bitbucket/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     7331 2023-11-29 19:55:25.000000 prefect-bitbucket-0.2.2/prefect_bitbucket/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:56:09.455529 prefect-bitbucket-0.2.2/prefect_bitbucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8247 2023-11-29 19:56:09.000000 prefect-bitbucket-0.2.2/prefect_bitbucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      524 2023-11-29 19:56:09.000000 prefect-bitbucket-0.2.2/prefect_bitbucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 19:56:09.000000 prefect-bitbucket-0.2.2/prefect_bitbucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-11-29 19:56:09.000000 prefect-bitbucket-0.2.2/prefect_bitbucket.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      233 2023-11-29 19:56:09.000000 prefect-bitbucket-0.2.2/prefect_bitbucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-29 19:56:09.000000 prefect-bitbucket-0.2.2/prefect_bitbucket.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-11-29 19:55:25.000000 prefect-bitbucket-0.2.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-11-29 19:55:25.000000 prefect-bitbucket-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      853 2023-11-29 19:56:09.455529 prefect-bitbucket-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2023-11-29 19:55:25.000000 prefect-bitbucket-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:56:09.455529 prefect-bitbucket-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2023-11-29 19:55:25.000000 prefect-bitbucket-0.2.2/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    10002 2023-11-29 19:55:25.000000 prefect-bitbucket-0.2.2/tests/test_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    80049 2023-11-29 19:55:25.000000 prefect-bitbucket-0.2.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:30.371102 prefect_bitbucket-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-04-25 19:20:30.371102 prefect_bitbucket-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-04-25 19:20:16.000000 prefect_bitbucket-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:30.367102 prefect_bitbucket-0.2.3/prefect_bitbucket/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-25 19:20:16.000000 prefect_bitbucket-0.2.3/prefect_bitbucket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:29.000000 prefect_bitbucket-0.2.3/prefect_bitbucket/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-25 19:20:16.000000 prefect_bitbucket-0.2.3/prefect_bitbucket/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-25 19:20:16.000000 prefect_bitbucket-0.2.3/prefect_bitbucket/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:30.367102 prefect_bitbucket-0.2.3/prefect_bitbucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-04-25 19:20:30.000000 prefect_bitbucket-0.2.3/prefect_bitbucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-25 19:20:30.000000 prefect_bitbucket-0.2.3/prefect_bitbucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:30.000000 prefect_bitbucket-0.2.3/prefect_bitbucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-25 19:20:30.000000 prefect_bitbucket-0.2.3/prefect_bitbucket.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-25 19:20:30.000000 prefect_bitbucket-0.2.3/prefect_bitbucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 19:20:30.000000 prefect_bitbucket-0.2.3/prefect_bitbucket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-25 19:20:16.000000 prefect_bitbucket-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:30.371102 prefect_bitbucket-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:30.367102 prefect_bitbucket-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-25 19:20:16.000000 prefect_bitbucket-0.2.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-25 19:20:16.000000 prefect_bitbucket-0.2.3/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-04-25 19:20:16.000000 prefect_bitbucket-0.2.3/tests/test_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-25 19:20:16.000000 prefect_bitbucket-0.2.3/tests/test_version.py
```

### Comparing `prefect-bitbucket-0.2.2/PKG-INFO` & `prefect_bitbucket-0.2.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,96 +1,85 @@
 Metadata-Version: 2.1
 Name: prefect-bitbucket
-Version: 0.2.2
+Version: 0.2.3
 Summary: Prefect integrations for working with Bitbucket repositories.
-Home-page: https://github.com/PrefectHQ/prefect-bitbucket
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-bitbucket
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
-Requires-Dist: atlassian-python-api>=3.32.1
+Requires-Dist: prefect>=2.14.10
+Requires-Dist: atlassian-python-api!=3.41.5,!=3.41.6,!=3.41.7,!=3.41.8,>=3.32.1
 Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: aiohttp; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: interrogate; extra == "dev"
+Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest-asyncio; extra == "dev"
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
 
 # prefect-bitbucket
 
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-bitbucket/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-bitbucket?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-bitbucket/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-bitbucket?color=0052FF&labelColor=090422" /></a>
     <a href="https://pepy.tech/badge/prefect-bitbucket/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-bitbucket?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-bitbucket/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-bitbucket?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
 </p>
 
 
 ## Welcome!
 
 Prefect integrations for working with Bitbucket repositories.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.7+.
+Requires an installation of Python 3.8+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
-These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://orion-docs.prefect.io/).
+These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
 
 Install `prefect-bitbucket` with `pip`:
 
 ```bash
 pip install prefect-bitbucket
 ```
 
-Then, register to [view the block](https://orion-docs.prefect.io/ui/blocks/) on Prefect Cloud:
+Then, register to [view the block](https://docs.prefect.io/ui/blocks/) on Prefect Cloud:
 
 ```bash
 prefect block register -m prefect_bitbucket
 ```
 
-Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
+Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://docs.prefect.io/ui/blocks/).
 
 ### Write and run a flow
 #### Load a pre-existing BitBucketCredentials block
 
 ```python
 from prefect import flow
 from prefect_bitbucket.credentials import BitBucketCredentials
@@ -192,30 +181,7 @@
 # Saves the BitBucketRepository block to your Prefect workspace (in the Blocks tab)
 private_bitbucket_block.save(name="my-private-bitbucket-block")
 ```
 
 !!! info "Differences between Bitbucket Server and Bitbucket Cloud"
 
     For Bitbucket Cloud, only set the `token` to authenticate. For Bitbucket Server, set both the `token` and the `username`.
-
-## Resources
-
-If you encounter any bugs while using `prefect-bitbucket`, feel free to open an issue in the [prefect-bitbucket](https://github.com/PrefectHQ/prefect-bitbucket) repository.
-
-If you have any questions or issues while using `prefect-bitbucket`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
-
-Feel free to ⭐️ or watch [`prefect-bitbucket`](https://github.com/PrefectHQ/prefect-bitbucket) for updates too!
-
-## Development
-
-If you'd like to install a version of `prefect-bitbucket` for development, clone the repository and perform an editable install with `pip`:
-
-```bash
-git clone https://github.com/PrefectHQ/prefect-bitbucket.git
-
-cd prefect-bitbucket/
-
-pip install -e ".[dev]"
-
-# Install linting pre-commit hooks
-pre-commit install
-```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prefect-bitbucket-0.2.2/README.md` & `prefect_bitbucket-0.2.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,46 @@
 # prefect-bitbucket
 
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-bitbucket/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-bitbucket?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-bitbucket/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-bitbucket?color=0052FF&labelColor=090422" /></a>
     <a href="https://pepy.tech/badge/prefect-bitbucket/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-bitbucket?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-bitbucket/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-bitbucket?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
 </p>
 
 
 ## Welcome!
 
 Prefect integrations for working with Bitbucket repositories.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.7+.
+Requires an installation of Python 3.8+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
-These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://orion-docs.prefect.io/).
+These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
 
 Install `prefect-bitbucket` with `pip`:
 
 ```bash
 pip install prefect-bitbucket
 ```
 
-Then, register to [view the block](https://orion-docs.prefect.io/ui/blocks/) on Prefect Cloud:
+Then, register to [view the block](https://docs.prefect.io/ui/blocks/) on Prefect Cloud:
 
 ```bash
 prefect block register -m prefect_bitbucket
 ```
 
-Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
+Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://docs.prefect.io/ui/blocks/).
 
 ### Write and run a flow
 #### Load a pre-existing BitBucketCredentials block
 
 ```python
 from prefect import flow
 from prefect_bitbucket.credentials import BitBucketCredentials
@@ -150,31 +141,8 @@
 
 # Saves the BitBucketRepository block to your Prefect workspace (in the Blocks tab)
 private_bitbucket_block.save(name="my-private-bitbucket-block")
 ```
 
 !!! info "Differences between Bitbucket Server and Bitbucket Cloud"
 
-    For Bitbucket Cloud, only set the `token` to authenticate. For Bitbucket Server, set both the `token` and the `username`.
-
-## Resources
-
-If you encounter any bugs while using `prefect-bitbucket`, feel free to open an issue in the [prefect-bitbucket](https://github.com/PrefectHQ/prefect-bitbucket) repository.
-
-If you have any questions or issues while using `prefect-bitbucket`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
-
-Feel free to ⭐️ or watch [`prefect-bitbucket`](https://github.com/PrefectHQ/prefect-bitbucket) for updates too!
-
-## Development
-
-If you'd like to install a version of `prefect-bitbucket` for development, clone the repository and perform an editable install with `pip`:
-
-```bash
-git clone https://github.com/PrefectHQ/prefect-bitbucket.git
-
-cd prefect-bitbucket/
-
-pip install -e ".[dev]"
-
-# Install linting pre-commit hooks
-pre-commit install
-```
+    For Bitbucket Cloud, only set the `token` to authenticate. For Bitbucket Server, set both the `token` and the `username`.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prefect-bitbucket-0.2.2/prefect_bitbucket/credentials.py` & `prefect_bitbucket-0.2.3/prefect_bitbucket/credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Module to enable authenticate interactions with BitBucket."""
 import re
 from enum import Enum
 from typing import Optional, Union
 
-from prefect.blocks.abstract import CredentialsBlock
 from pydantic import VERSION as PYDANTIC_VERSION
 
+from prefect.blocks.abstract import CredentialsBlock
+
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field, SecretStr, validator
 else:
     from pydantic import Field, SecretStr, validator
 
 try:
     from atlassian.bitbucket import Bitbucket, Cloud
```

### Comparing `prefect-bitbucket-0.2.2/prefect_bitbucket/repository.py` & `prefect_bitbucket-0.2.3/prefect_bitbucket/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,19 +38,20 @@
 import io
 from distutils.dir_util import copy_tree
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Optional, Tuple, Union
 from urllib.parse import urlparse, urlunparse
 
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect.exceptions import InvalidRepositoryURLError
 from prefect.filesystems import ReadableDeploymentStorage
 from prefect.utilities.asyncutils import sync_compatible
 from prefect.utilities.processutils import run_process
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field, validator
 else:
     from pydantic import Field, validator
 
 from prefect_bitbucket.credentials import BitBucketCredentials
```

### Comparing `prefect-bitbucket-0.2.2/prefect_bitbucket.egg-info/PKG-INFO` & `prefect_bitbucket-0.2.3/prefect_bitbucket.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,96 +1,85 @@
 Metadata-Version: 2.1
 Name: prefect-bitbucket
-Version: 0.2.2
+Version: 0.2.3
 Summary: Prefect integrations for working with Bitbucket repositories.
-Home-page: https://github.com/PrefectHQ/prefect-bitbucket
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-bitbucket
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
-Requires-Dist: atlassian-python-api>=3.32.1
+Requires-Dist: prefect>=2.14.10
+Requires-Dist: atlassian-python-api!=3.41.5,!=3.41.6,!=3.41.7,!=3.41.8,>=3.32.1
 Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: aiohttp; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: interrogate; extra == "dev"
+Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest-asyncio; extra == "dev"
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
 
 # prefect-bitbucket
 
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-bitbucket/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-bitbucket?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-bitbucket/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-bitbucket?color=0052FF&labelColor=090422" /></a>
     <a href="https://pepy.tech/badge/prefect-bitbucket/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-bitbucket?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-bitbucket/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-bitbucket?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
 </p>
 
 
 ## Welcome!
 
 Prefect integrations for working with Bitbucket repositories.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.7+.
+Requires an installation of Python 3.8+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
-These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://orion-docs.prefect.io/).
+These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
 
 Install `prefect-bitbucket` with `pip`:
 
 ```bash
 pip install prefect-bitbucket
 ```
 
-Then, register to [view the block](https://orion-docs.prefect.io/ui/blocks/) on Prefect Cloud:
+Then, register to [view the block](https://docs.prefect.io/ui/blocks/) on Prefect Cloud:
 
 ```bash
 prefect block register -m prefect_bitbucket
 ```
 
-Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
+Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://docs.prefect.io/ui/blocks/).
 
 ### Write and run a flow
 #### Load a pre-existing BitBucketCredentials block
 
 ```python
 from prefect import flow
 from prefect_bitbucket.credentials import BitBucketCredentials
@@ -192,30 +181,7 @@
 # Saves the BitBucketRepository block to your Prefect workspace (in the Blocks tab)
 private_bitbucket_block.save(name="my-private-bitbucket-block")
 ```
 
 !!! info "Differences between Bitbucket Server and Bitbucket Cloud"
 
     For Bitbucket Cloud, only set the `token` to authenticate. For Bitbucket Server, set both the `token` and the `username`.
-
-## Resources
-
-If you encounter any bugs while using `prefect-bitbucket`, feel free to open an issue in the [prefect-bitbucket](https://github.com/PrefectHQ/prefect-bitbucket) repository.
-
-If you have any questions or issues while using `prefect-bitbucket`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
-
-Feel free to ⭐️ or watch [`prefect-bitbucket`](https://github.com/PrefectHQ/prefect-bitbucket) for updates too!
-
-## Development
-
-If you'd like to install a version of `prefect-bitbucket` for development, clone the repository and perform an editable install with `pip`:
-
-```bash
-git clone https://github.com/PrefectHQ/prefect-bitbucket.git
-
-cd prefect-bitbucket/
-
-pip install -e ".[dev]"
-
-# Install linting pre-commit hooks
-pre-commit install
-```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prefect-bitbucket-0.2.2/tests/test_credentials.py` & `prefect_bitbucket-0.2.3/tests/test_credentials.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 from atlassian.bitbucket import Bitbucket, Cloud
-from prefect.blocks.core import Block
-
 from prefect_bitbucket.credentials import BitBucketCredentials, ClientType
 
+from prefect.blocks.core import Block
+
 
 @pytest.mark.parametrize("token", [None, "token_value"])
 def test_bitbucket_credentials(token):
     """Test credentials is Block type."""
     credentials_block = BitBucketCredentials(token=token)
     assert isinstance(credentials_block, Block)
```

### Comparing `prefect-bitbucket-0.2.2/tests/test_repository.py` & `prefect_bitbucket-0.2.3/tests/test_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Set, Tuple
 
 import pytest
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect.exceptions import InvalidRepositoryURLError
 from prefect.testing.utilities import AsyncMock
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import SecretStr
 else:
     from pydantic import SecretStr
 
 import prefect_bitbucket
@@ -199,17 +200,15 @@
         )
         with pytest.raises(InvalidRepositoryURLError, match=error_msg):
             BitBucketRepository(
                 repository="git@bitbucket.org:PrefectHQ/prefect.git",
                 bitbucket_credentials=BitBucketCredentials(token=SecretStr(credential)),
             )
 
-    async def test_dir_contents_copied_correctly_with_get_directory(
-        self, monkeypatch
-    ):  # noqa
+    async def test_dir_contents_copied_correctly_with_get_directory(self, monkeypatch):  # noqa
         """Check that `get_directory` is able to correctly copy contents from src->dst"""  # noqa
 
         class p:
             returncode = 0
 
         mock = AsyncMock(return_value=p())
         monkeypatch.setattr(prefect_bitbucket.repository, "run_process", mock)
```


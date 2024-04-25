# Comparing `tmp/prefect-email-0.3.2.tar.gz` & `tmp/prefect_email-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-email-0.3.2.tar", last modified: Wed Nov 29 19:53:08 2023, max compression
+gzip compressed data, was "prefect_email-0.3.3.tar", last modified: Thu Apr 25 19:20:27 2024, max compression
```

## Comparing `prefect-email-0.3.2.tar` & `prefect_email-0.3.3.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:53:08.638612 prefect-email-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-11-29 19:52:30.000000 prefect-email-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-11-29 19:52:30.000000 prefect-email-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2023-11-29 19:53:08.638612 prefect-email-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8039 2023-11-29 19:52:30.000000 prefect-email-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:53:08.638612 prefect-email-0.3.2/prefect_email/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2023-11-29 19:52:30.000000 prefect-email-0.3.2/prefect_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-11-29 19:53:08.638612 prefect-email-0.3.2/prefect_email/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2023-11-29 19:52:30.000000 prefect-email-0.3.2/prefect_email/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2023-11-29 19:52:30.000000 prefect-email-0.3.2/prefect_email/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:53:08.638612 prefect-email-0.3.2/prefect_email.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2023-11-29 19:53:08.000000 prefect-email-0.3.2/prefect_email.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2023-11-29 19:53:08.000000 prefect-email-0.3.2/prefect_email.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 19:53:08.000000 prefect-email-0.3.2/prefect_email.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-11-29 19:53:08.000000 prefect-email-0.3.2/prefect_email.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-11-29 19:53:08.000000 prefect-email-0.3.2/prefect_email.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-29 19:53:08.000000 prefect-email-0.3.2/prefect_email.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-11-29 19:52:30.000000 prefect-email-0.3.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-29 19:52:30.000000 prefect-email-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      763 2023-11-29 19:53:08.638612 prefect-email-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2023-11-29 19:52:30.000000 prefect-email-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:53:08.638612 prefect-email-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-11-29 19:52:30.000000 prefect-email-0.3.2/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2023-11-29 19:52:30.000000 prefect-email-0.3.2/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2023-11-29 19:52:30.000000 prefect-email-0.3.2/tests/test_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    80049 2023-11-29 19:52:30.000000 prefect-email-0.3.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:27.354595 prefect_email-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-04-25 19:20:27.354595 prefect_email-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-25 19:20:13.000000 prefect_email-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:27.350595 prefect_email-0.3.3/prefect_email/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-25 19:20:13.000000 prefect_email-0.3.3/prefect_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:26.000000 prefect_email-0.3.3/prefect_email/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-04-25 19:20:13.000000 prefect_email-0.3.3/prefect_email/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-25 19:20:13.000000 prefect_email-0.3.3/prefect_email/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:27.354595 prefect_email-0.3.3/prefect_email.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-04-25 19:20:27.000000 prefect_email-0.3.3/prefect_email.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-25 19:20:27.000000 prefect_email-0.3.3/prefect_email.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:27.000000 prefect_email-0.3.3/prefect_email.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 19:20:27.000000 prefect_email-0.3.3/prefect_email.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-25 19:20:27.000000 prefect_email-0.3.3/prefect_email.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 19:20:27.000000 prefect_email-0.3.3/prefect_email.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-25 19:20:13.000000 prefect_email-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:27.354595 prefect_email-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:27.354595 prefect_email-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 19:20:13.000000 prefect_email-0.3.3/tests/attachment.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-25 19:20:13.000000 prefect_email-0.3.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-25 19:20:13.000000 prefect_email-0.3.3/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-25 19:20:13.000000 prefect_email-0.3.3/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-25 19:20:13.000000 prefect_email-0.3.3/tests/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-25 19:20:13.000000 prefect_email-0.3.3/tests/test_version.py
```

### Comparing `prefect-email-0.3.2/PKG-INFO` & `prefect_email-0.3.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,52 @@
 Metadata-Version: 2.1
 Name: prefect-email
-Version: 0.3.2
-Summary: Prefect tasks and subflows for interacting with email
-Home-page: https://github.com/PrefectHQ/prefect-email
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Version: 0.3.3
+Summary: Prefect integrations for interacting with email.
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-email
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
+Requires-Dist: prefect>=2.14.10
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
 
 # prefect-email
 
 <p align="center">
-    <img src="https://user-images.githubusercontent.com/15331990/218230330-face3c8d-7f09-47f5-a24a-708c6d707b1a.png">
-    <br>
     <a href="https://pypi.python.org/pypi/prefect-email/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-email?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-email/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-email?color=0052FF&labelColor=090422" /></a>
     <a href="https://pepy.tech/badge/prefect-email/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-email?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-email/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-email?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
 </p>
 
 Visit the full docs [here](https://PrefectHQ.github.io/prefect-email) to see additional examples and the API reference.
 
 `prefect-email` is a collection of prebuilt Prefect integrations that can be used to interact with email services.
 
 ## Getting Started
@@ -131,41 +118,41 @@
         raise
 
 example_flow()
 ```
 
 ## Resources
 
-For more tips on how to use tasks and flows in a Collection, check out [Using Collections](https://orion-docs.prefect.io/collections/usage/)!
+For more tips on how to use tasks and flows in a Collection, check out [Using Collections](https://docs.prefect.io/collections/usage/)!
 
 ### Installation
 
 Install `prefect-email` with `pip`:
 
 ```bash
 pip install prefect-email
 ```
 
-Then, register to [view the block](https://orion-docs.prefect.io/ui/blocks/) on Prefect Cloud:
+Then, register to [view the block](https://docs.prefect.io/ui/blocks/) on Prefect Cloud:
 
 ```bash
 prefect block register -m prefect_email
 ```
 
-Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
+Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://docs.prefect.io/ui/blocks/).
 
-Requires an installation of Python 3.7+.
+Requires an installation of Python 3.8+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
-These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://orion-docs.prefect.io/).
+These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Saving credentials to block
 
-Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
+Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://docs.prefect.io/ui/blocks/).
 
 Below is a walkthrough on saving block documents through code.
 
 Create a short script, replacing the placeholders.
 
 ```python
 from prefect_email import EmailServerCredentials
@@ -184,43 +171,13 @@
 
 EmailServerCredentials.load("BLOCK_NAME_PLACEHOLDER")
 ```
 
 !!! info "Registering blocks"
 
     Register blocks in this module to
-    [view and edit them](https://orion-docs.prefect.io/ui/blocks/)
+    [view and edit them](https://docs.prefect.io/ui/blocks/)
     on Prefect Cloud:
 
     ```bash
     prefect block register -m prefect_email
     ```
-
-A list of available blocks in `prefect-email` and their setup instructions can be found [here](https://PrefectHQ.github.io/prefect-email/blocks_catalog).
-
-### Feedback
-
-If you encounter any bugs while using `prefect-email`, feel free to open an issue in the [prefect-email](https://github.com/PrefectHQ/prefect-email) repository.
-
-If you have any questions or issues while using `prefect-email`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
- 
-Feel free to star or watch [`prefect-email`](https://github.com/PrefectHQ/prefect-email) for updates too!
-
-### Contributing
-If you'd like to help contribute to fix an issue or add a feature to `prefect-email`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
-
-Here are the steps:
-
-1. [Fork the repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository)
-2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
-3. Install the repository and its dependencies:
-```
-pip install -e ".[dev]"
-```
-4. Make desired changes
-5. Add tests
-6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-email/blob/main/CHANGELOG.md)
-7. Install `pre-commit` to perform quality checks prior to commit:
-```
-pre-commit install
-```
-8. `git commit`, `git push`, and create a pull request
```

### Comparing `prefect-email-0.3.2/README.md` & `prefect_email-0.3.3/prefect_email.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,52 @@
+Metadata-Version: 2.1
+Name: prefect-email
+Version: 0.3.3
+Summary: Prefect integrations for interacting with email.
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
+License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-email
+Keywords: prefect
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: prefect>=2.14.10
+Provides-Extra: dev
+Requires-Dist: aiohttp; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: interrogate; extra == "dev"
+Requires-Dist: mkdocs-gen-files; extra == "dev"
+Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: mkdocstrings[python]; extra == "dev"
+Requires-Dist: mock; python_version < "3.8" and extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pillow; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
+
 # prefect-email
 
 <p align="center">
-    <img src="https://user-images.githubusercontent.com/15331990/218230330-face3c8d-7f09-47f5-a24a-708c6d707b1a.png">
-    <br>
     <a href="https://pypi.python.org/pypi/prefect-email/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-email?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-email/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-email?color=0052FF&labelColor=090422" /></a>
     <a href="https://pepy.tech/badge/prefect-email/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-email?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-email/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-email?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
 </p>
 
 Visit the full docs [here](https://PrefectHQ.github.io/prefect-email) to see additional examples and the API reference.
 
 `prefect-email` is a collection of prebuilt Prefect integrations that can be used to interact with email services.
 
 ## Getting Started
@@ -91,41 +118,41 @@
         raise
 
 example_flow()
 ```
 
 ## Resources
 
-For more tips on how to use tasks and flows in a Collection, check out [Using Collections](https://orion-docs.prefect.io/collections/usage/)!
+For more tips on how to use tasks and flows in a Collection, check out [Using Collections](https://docs.prefect.io/collections/usage/)!
 
 ### Installation
 
 Install `prefect-email` with `pip`:
 
 ```bash
 pip install prefect-email
 ```
 
-Then, register to [view the block](https://orion-docs.prefect.io/ui/blocks/) on Prefect Cloud:
+Then, register to [view the block](https://docs.prefect.io/ui/blocks/) on Prefect Cloud:
 
 ```bash
 prefect block register -m prefect_email
 ```
 
-Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
+Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://docs.prefect.io/ui/blocks/).
 
-Requires an installation of Python 3.7+.
+Requires an installation of Python 3.8+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
-These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://orion-docs.prefect.io/).
+These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Saving credentials to block
 
-Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://orion-docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://orion-docs.prefect.io/ui/blocks/).
+Note, to use the `load` method on Blocks, you must already have a block document [saved through code](https://docs.prefect.io/concepts/blocks/#saving-blocks) or [saved through the UI](https://docs.prefect.io/ui/blocks/).
 
 Below is a walkthrough on saving block documents through code.
 
 Create a short script, replacing the placeholders.
 
 ```python
 from prefect_email import EmailServerCredentials
@@ -144,43 +171,13 @@
 
 EmailServerCredentials.load("BLOCK_NAME_PLACEHOLDER")
 ```
 
 !!! info "Registering blocks"
 
     Register blocks in this module to
-    [view and edit them](https://orion-docs.prefect.io/ui/blocks/)
+    [view and edit them](https://docs.prefect.io/ui/blocks/)
     on Prefect Cloud:
 
     ```bash
     prefect block register -m prefect_email
     ```
-
-A list of available blocks in `prefect-email` and their setup instructions can be found [here](https://PrefectHQ.github.io/prefect-email/blocks_catalog).
-
-### Feedback
-
-If you encounter any bugs while using `prefect-email`, feel free to open an issue in the [prefect-email](https://github.com/PrefectHQ/prefect-email) repository.
-
-If you have any questions or issues while using `prefect-email`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
- 
-Feel free to star or watch [`prefect-email`](https://github.com/PrefectHQ/prefect-email) for updates too!
-
-### Contributing
-If you'd like to help contribute to fix an issue or add a feature to `prefect-email`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
-
-Here are the steps:
-
-1. [Fork the repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository)
-2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
-3. Install the repository and its dependencies:
-```
-pip install -e ".[dev]"
-```
-4. Make desired changes
-5. Add tests
-6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-email/blob/main/CHANGELOG.md)
-7. Install `pre-commit` to perform quality checks prior to commit:
-```
-pre-commit install
-```
-8. `git commit`, `git push`, and create a pull request
```

### Comparing `prefect-email-0.3.2/prefect_email/credentials.py` & `prefect_email-0.3.3/prefect_email/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 import ssl
 from enum import Enum
 from functools import partial
 from smtplib import SMTP, SMTP_SSL
 from typing import Optional, Union
 
-from prefect.blocks.core import Block
 from pydantic import VERSION as PYDANTIC_VERSION
 
+from prefect.blocks.core import Block
+
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field, SecretStr, validator
 else:
     from pydantic import Field, SecretStr, validator
 
 
 class SMTPType(Enum):
```

### Comparing `prefect-email-0.3.2/prefect_email/message.py` & `prefect_email-0.3.3/prefect_email/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from email.mime.base import MIMEBase
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from functools import partial
 from typing import TYPE_CHECKING, List, Optional, Union
 
 from anyio import to_thread
+
 from prefect import task
 
 if TYPE_CHECKING:
     from prefect_email import EmailServerCredentials
 
 
 @task
```

### Comparing `prefect-email-0.3.2/tests/test_block_standards.py` & `prefect_email-0.3.3/tests/test_block_standards.py`

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

### Comparing `prefect-email-0.3.2/tests/test_credentials.py` & `prefect_email-0.3.3/tests/test_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-
 from prefect_email.credentials import (
     EmailServerCredentials,
     SMTPServer,
     SMTPType,
     _cast_to_enum,
 )
```

### Comparing `prefect-email-0.3.2/tests/test_message.py` & `prefect_email-0.3.3/tests/test_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import base64
 import pathlib
 
 import pytest
-from prefect import flow
-
 from prefect_email.message import email_send_message
 
+from prefect import flow
+
 EMAIL_TO = [
     "someone@email.com",
     "someone@email.com, someone_else@email.com",
     ["some_1@email.com", "some_2@email.com"],
     None,
 ]
 EMAIL_TO_CC = [
@@ -28,15 +28,14 @@
 
 @pytest.mark.parametrize("email_to", EMAIL_TO)
 @pytest.mark.parametrize("email_to_cc", EMAIL_TO_CC)
 @pytest.mark.parametrize("email_to_bcc", EMAIL_TO_BCC)
 async def test_email_send_message(
     email_to, email_to_cc, email_to_bcc, email_server_credentials
 ):
-
     subject = "Example Flow Notification"
     msg_plain = "This proves msg plain is attached first!"
     msg = "<h1>This proves msg is attached second!</h1>"
 
     attachment = pathlib.Path(__file__).parent.absolute() / "attachment.txt"
     with open(attachment, "rb") as f:
         attachment_text = f.read()
```


# Comparing `tmp/prefect-dask-0.2.6.tar.gz` & `tmp/prefect_dask-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-dask-0.2.6.tar", last modified: Mon Nov 13 22:53:02 2023, max compression
+gzip compressed data, was "prefect_dask-0.2.7.tar", last modified: Thu Apr 25 19:20:15 2024, max compression
```

## Comparing `prefect-dask-0.2.6.tar` & `prefect_dask-0.2.7.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 22:53:02.440204 prefect-dask-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-11-13 22:52:08.000000 prefect-dask-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      319 2023-11-13 22:52:08.000000 prefect-dask-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12629 2023-11-13 22:53:02.440204 prefect-dask-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10844 2023-11-13 22:52:08.000000 prefect-dask-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 22:53:02.444204 prefect-dask-0.2.6/prefect_dask/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-11-13 22:52:08.000000 prefect-dask-0.2.6/prefect_dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-11-13 22:53:02.444204 prefect-dask-0.2.6/prefect_dask/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2023-11-13 22:52:08.000000 prefect-dask-0.2.6/prefect_dask/task_runners.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2023-11-13 22:52:08.000000 prefect-dask-0.2.6/prefect_dask/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 22:53:02.440204 prefect-dask-0.2.6/prefect_dask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12629 2023-11-13 22:53:02.000000 prefect-dask-0.2.6/prefect_dask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-11-13 22:53:02.000000 prefect-dask-0.2.6/prefect_dask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-13 22:53:02.000000 prefect-dask-0.2.6/prefect_dask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-11-13 22:53:02.000000 prefect-dask-0.2.6/prefect_dask.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-11-13 22:53:02.000000 prefect-dask-0.2.6/prefect_dask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-13 22:53:02.000000 prefect-dask-0.2.6/prefect_dask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-11-13 22:52:08.000000 prefect-dask-0.2.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-11-13 22:52:08.000000 prefect-dask-0.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      896 2023-11-13 22:53:02.444204 prefect-dask-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2023-11-13 22:52:08.000000 prefect-dask-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 22:53:02.440204 prefect-dask-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2023-11-13 22:52:08.000000 prefect-dask-0.2.6/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     9836 2023-11-13 22:52:08.000000 prefect-dask-0.2.6/tests/test_task_runners.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2023-11-13 22:52:08.000000 prefect-dask-0.2.6/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    80049 2023-11-13 22:52:08.000000 prefect-dask-0.2.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:15.103096 prefect_dask-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-25 19:20:15.103096 prefect_dask-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9529 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:15.099096 prefect_dask-0.2.7/prefect_dask/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/prefect_dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:14.000000 prefect_dask-0.2.7/prefect_dask/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/prefect_dask/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/prefect_dask/task_runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/prefect_dask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:15.103096 prefect_dask-0.2.7/prefect_dask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-25 19:20:14.000000 prefect_dask-0.2.7/prefect_dask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-25 19:20:15.000000 prefect_dask-0.2.7/prefect_dask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:14.000000 prefect_dask-0.2.7/prefect_dask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-25 19:20:14.000000 prefect_dask-0.2.7/prefect_dask.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-25 19:20:14.000000 prefect_dask-0.2.7/prefect_dask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 19:20:14.000000 prefect_dask-0.2.7/prefect_dask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:15.103096 prefect_dask-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:15.103096 prefect_dask-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11490 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/tests/test_task_runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-25 19:20:00.000000 prefect_dask-0.2.7/tests/test_version.py
```

### Comparing `prefect-dask-0.2.6/PKG-INFO` & `prefect_dask-0.2.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,72 +1,56 @@
 Metadata-Version: 2.1
 Name: prefect-dask
-Version: 0.2.6
+Version: 0.2.7
 Summary: Prefect integrations with the Dask execution framework.
-Home-page: https://github.com/PrefectHQ/prefect-dask
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-dask
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
+Requires-Dist: anyio<4.0.0,>=3.7.1
 Requires-Dist: prefect>=2.13.5
 Requires-Dist: distributed==2022.2.0; python_version < "3.8"
 Requires-Dist: distributed!=2023.3.2,!=2023.3.2.1,!=2023.4.*,!=2023.5.*,>=2022.5.0; python_version >= "3.8"
 Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: flaky; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: mkdocs; extra == "dev"
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
+Requires-Dist: pytest-asyncio!=0.22.0,<0.23.0,>=0.18.2; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
 
-# Coordinate and parallelize your dataflow with `prefect-dask`
+# `prefect-dask`
 
 <p align="center">
-    <img src="https://user-images.githubusercontent.com/15331990/211682578-3e341709-6509-4c95-a6af-3b1160fe2961.png" width=40% height=40%>
-    <br>
     <a href="https://pypi.python.org/pypi/prefect-dask/" alt="PyPI version">
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-dask?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-dask/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-dask?color=0052FF&labelColor=090422" /></a>
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-dask?color=26272B&labelColor=090422"></a>
     <a href="https://pepy.tech/badge/prefect-dask/" alt="Downloads">
-        <img src="https://img.shields.io/pypi/dm/prefect-dask?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-dask/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-dask?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
+        <img src="https://img.shields.io/pypi/dm/prefect-dask?color=26272B&labelColor=090422" /></a>
 </p>
 
-Visit the full docs [here](https://PrefectHQ.github.io/prefect-dask) to see additional examples and the API reference.
-
 The `prefect-dask` collection makes it easy to include distributed processing for your flows. Check out the examples below to get started!
 
 ## Getting Started
 
 ### Integrate with Prefect flows
 
 Perhaps you're already working with Prefect flows. Say your flow downloads many images to train your machine learning model. Unfortunately, it takes a long time to download your flows because your code is running sequentially.
@@ -286,33 +270,30 @@
 
 We recommend using a Python virtual environment manager such as pipenv, conda, or virtualenv.
 
 These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Feedback
 
-If you encounter any bugs while using `prefect-dask`, feel free to open an issue in the [prefect-dask](https://github.com/PrefectHQ/prefect-dask) repository.
+If you encounter any bugs while using `prefect-dask`, feel free to open an issue in the [prefect](https://github.com/PrefectHQ/prefect) repository.
 
 If you have any questions or issues while using `prefect-dask`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
 
-Feel free to star or watch [`prefect-dask`](https://github.com/PrefectHQ/prefect-dask) for updates too!
-
 ### Contributing
 
 If you'd like to help contribute to fix an issue or add a feature to `prefect-dask`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
 
 Here are the steps:
 
 1. [Fork the repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository)
 2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
 3. Install the repository and its dependencies:
 ```
 pip install -e ".[dev]"
 ```
 4. Make desired changes
 5. Add tests
-6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-dask/blob/main/CHANGELOG.md)
-7. Install `pre-commit` to perform quality checks prior to commit:
+6. Install `pre-commit` to perform quality checks prior to commit:
 ```
 pre-commit install
 ```
-8. `git commit`, `git push`, and create a pull request
+7. `git commit`, `git push`, and create a pull request
```

### Comparing `prefect-dask-0.2.6/README.md` & `prefect_dask-0.2.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,16 @@
-# Coordinate and parallelize your dataflow with `prefect-dask`
+# `prefect-dask`
 
 <p align="center">
-    <img src="https://user-images.githubusercontent.com/15331990/211682578-3e341709-6509-4c95-a6af-3b1160fe2961.png" width=40% height=40%>
-    <br>
     <a href="https://pypi.python.org/pypi/prefect-dask/" alt="PyPI version">
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-dask?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-dask/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-dask?color=0052FF&labelColor=090422" /></a>
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-dask?color=26272B&labelColor=090422"></a>
     <a href="https://pepy.tech/badge/prefect-dask/" alt="Downloads">
-        <img src="https://img.shields.io/pypi/dm/prefect-dask?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-dask/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-dask?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
+        <img src="https://img.shields.io/pypi/dm/prefect-dask?color=26272B&labelColor=090422" /></a>
 </p>
 
-Visit the full docs [here](https://PrefectHQ.github.io/prefect-dask) to see additional examples and the API reference.
-
 The `prefect-dask` collection makes it easy to include distributed processing for your flows. Check out the examples below to get started!
 
 ## Getting Started
 
 ### Integrate with Prefect flows
 
 Perhaps you're already working with Prefect flows. Say your flow downloads many images to train your machine learning model. Unfortunately, it takes a long time to download your flows because your code is running sequentially.
@@ -243,33 +230,30 @@
 
 We recommend using a Python virtual environment manager such as pipenv, conda, or virtualenv.
 
 These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Feedback
 
-If you encounter any bugs while using `prefect-dask`, feel free to open an issue in the [prefect-dask](https://github.com/PrefectHQ/prefect-dask) repository.
+If you encounter any bugs while using `prefect-dask`, feel free to open an issue in the [prefect](https://github.com/PrefectHQ/prefect) repository.
 
 If you have any questions or issues while using `prefect-dask`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
 
-Feel free to star or watch [`prefect-dask`](https://github.com/PrefectHQ/prefect-dask) for updates too!
-
 ### Contributing
 
 If you'd like to help contribute to fix an issue or add a feature to `prefect-dask`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
 
 Here are the steps:
 
 1. [Fork the repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository)
 2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
 3. Install the repository and its dependencies:
 ```
 pip install -e ".[dev]"
 ```
 4. Make desired changes
 5. Add tests
-6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-dask/blob/main/CHANGELOG.md)
-7. Install `pre-commit` to perform quality checks prior to commit:
+6. Install `pre-commit` to perform quality checks prior to commit:
 ```
 pre-commit install
 ```
-8. `git commit`, `git push`, and create a pull request
+7. `git commit`, `git push`, and create a pull request
```

### Comparing `prefect-dask-0.2.6/prefect_dask/task_runners.py` & `prefect_dask-0.2.7/prefect_dask/task_runners.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 
 import inspect
 from contextlib import AsyncExitStack
 from typing import Awaitable, Callable, Dict, Optional, Union
 from uuid import UUID
 
 import distributed
+
 from prefect.context import FlowRunContext
 from prefect.futures import PrefectFuture
 from prefect.server.schemas.states import State
 from prefect.states import exception_to_crashed_state
 from prefect.task_runners import BaseTaskRunner, R, TaskConcurrencyType
 from prefect.utilities.collections import visit_collection
 from prefect.utilities.importtools import from_qualified_name, to_qualified_name
```

### Comparing `prefect-dask-0.2.6/prefect_dask/utils.py` & `prefect_dask-0.2.7/prefect_dask/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Utils to use alongside prefect-dask.
 """
 
 from contextlib import asynccontextmanager, contextmanager
 from datetime import timedelta
-from typing import Any, Dict, Optional, Union
+from typing import Any, AsyncGenerator, Dict, Generator, Optional, Union
 
 from distributed import Client, get_client
+
 from prefect.context import FlowRunContext, TaskRunContext
 
 
 def _generate_client_kwargs(
     async_client: bool,
     timeout: Optional[Union[int, float, str, timedelta]] = None,
     **client_kwargs: Dict[str, Any],
@@ -47,15 +48,15 @@
     return input_client_kwargs
 
 
 @contextmanager
 def get_dask_client(
     timeout: Optional[Union[int, float, str, timedelta]] = None,
     **client_kwargs: Dict[str, Any],
-) -> Client:
+) -> Generator[Client, None, None]:
     """
     Yields a temporary synchronous dask client; this is useful
     for parallelizing operations on dask collections,
     such as a `dask.DataFrame` or `dask.Bag`.
 
     Without invoking this, workers do not automatically get a client to connect
     to the full cluster. Therefore, it will attempt perform work within the
@@ -104,15 +105,15 @@
         yield client
 
 
 @asynccontextmanager
 async def get_async_dask_client(
     timeout: Optional[Union[int, float, str, timedelta]] = None,
     **client_kwargs: Dict[str, Any],
-) -> Client:
+) -> AsyncGenerator[Client, None]:
     """
     Yields a temporary asynchronous dask client; this is useful
     for parallelizing operations on dask collections,
     such as a `dask.DataFrame` or `dask.Bag`.
 
     Without invoking this, workers do not automatically get a client to connect
     to the full cluster. Therefore, it will attempt perform work within the
```

### Comparing `prefect-dask-0.2.6/prefect_dask.egg-info/PKG-INFO` & `prefect_dask-0.2.7/prefect_dask.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,72 +1,56 @@
 Metadata-Version: 2.1
 Name: prefect-dask
-Version: 0.2.6
+Version: 0.2.7
 Summary: Prefect integrations with the Dask execution framework.
-Home-page: https://github.com/PrefectHQ/prefect-dask
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-dask
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
+Requires-Dist: anyio<4.0.0,>=3.7.1
 Requires-Dist: prefect>=2.13.5
 Requires-Dist: distributed==2022.2.0; python_version < "3.8"
 Requires-Dist: distributed!=2023.3.2,!=2023.3.2.1,!=2023.4.*,!=2023.5.*,>=2022.5.0; python_version >= "3.8"
 Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: flaky; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: mkdocs; extra == "dev"
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
+Requires-Dist: pytest-asyncio!=0.22.0,<0.23.0,>=0.18.2; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
 
-# Coordinate and parallelize your dataflow with `prefect-dask`
+# `prefect-dask`
 
 <p align="center">
-    <img src="https://user-images.githubusercontent.com/15331990/211682578-3e341709-6509-4c95-a6af-3b1160fe2961.png" width=40% height=40%>
-    <br>
     <a href="https://pypi.python.org/pypi/prefect-dask/" alt="PyPI version">
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-dask?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-dask/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-dask?color=0052FF&labelColor=090422" /></a>
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-dask?color=26272B&labelColor=090422"></a>
     <a href="https://pepy.tech/badge/prefect-dask/" alt="Downloads">
-        <img src="https://img.shields.io/pypi/dm/prefect-dask?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-dask/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-dask?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
+        <img src="https://img.shields.io/pypi/dm/prefect-dask?color=26272B&labelColor=090422" /></a>
 </p>
 
-Visit the full docs [here](https://PrefectHQ.github.io/prefect-dask) to see additional examples and the API reference.
-
 The `prefect-dask` collection makes it easy to include distributed processing for your flows. Check out the examples below to get started!
 
 ## Getting Started
 
 ### Integrate with Prefect flows
 
 Perhaps you're already working with Prefect flows. Say your flow downloads many images to train your machine learning model. Unfortunately, it takes a long time to download your flows because your code is running sequentially.
@@ -286,33 +270,30 @@
 
 We recommend using a Python virtual environment manager such as pipenv, conda, or virtualenv.
 
 These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Feedback
 
-If you encounter any bugs while using `prefect-dask`, feel free to open an issue in the [prefect-dask](https://github.com/PrefectHQ/prefect-dask) repository.
+If you encounter any bugs while using `prefect-dask`, feel free to open an issue in the [prefect](https://github.com/PrefectHQ/prefect) repository.
 
 If you have any questions or issues while using `prefect-dask`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
 
-Feel free to star or watch [`prefect-dask`](https://github.com/PrefectHQ/prefect-dask) for updates too!
-
 ### Contributing
 
 If you'd like to help contribute to fix an issue or add a feature to `prefect-dask`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
 
 Here are the steps:
 
 1. [Fork the repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository)
 2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
 3. Install the repository and its dependencies:
 ```
 pip install -e ".[dev]"
 ```
 4. Make desired changes
 5. Add tests
-6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-dask/blob/main/CHANGELOG.md)
-7. Install `pre-commit` to perform quality checks prior to commit:
+6. Install `pre-commit` to perform quality checks prior to commit:
 ```
 pre-commit install
 ```
-8. `git commit`, `git push`, and create a pull request
+7. `git commit`, `git push`, and create a pull request
```

### Comparing `prefect-dask-0.2.6/tests/test_block_standards.py` & `prefect_dask-0.2.7/tests/test_block_standards.py`

 * *Files 10% similar despite different names*

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

### Comparing `prefect-dask-0.2.6/tests/test_task_runners.py` & `prefect_dask-0.2.7/tests/test_task_runners.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import asyncio
 import logging
 import sys
 from functools import partial
+from typing import List
 from uuid import uuid4
 
 import cloudpickle
 import distributed
-import prefect.engine
 import pytest
 from distributed import LocalCluster
 from distributed.scheduler import KilledWorker
+from prefect_dask import DaskTaskRunner
+
+import prefect.engine
 from prefect import flow, get_run_logger, task
 from prefect.client.schemas import TaskRun
 from prefect.server.schemas.states import StateType
 from prefect.states import State
 from prefect.task_runners import TaskConcurrencyType
 from prefect.testing.fixtures import (  # noqa: F401
     hosted_api_server,
     use_hosted_api_server,
 )
 from prefect.testing.standard_test_suites import TaskRunnerStandardTestSuite
 from prefect.testing.utilities import exceptions_equal
 
-from prefect_dask import DaskTaskRunner
-
 
 @pytest.fixture(scope="session")
 def event_loop(request):
     """
     Redefine the event loop to support session/module-scoped fixtures;
     see https://github.com/pytest-dev/pytest-asyncio/issues/68
     When running on Windows we need to use a non-default loop for subprocess support.
@@ -269,7 +270,58 @@
             # the adapt_kwargs argument triggers the calls to the adapt method
             task_runner = DaskTaskRunner(
                 cluster_class=task_runner_class,
                 adapt_kwargs={"minimum": 1, "maximum": 1},
             )
             async with task_runner.start():
                 assert task_runner._cluster._adapt_called
+
+    async def test_task_runner_can_execute_sync_task_in_async_flow(self, task_runner):
+        """
+        This is a regression test for https://github.com/PrefectHQ/prefect/issues/7422
+        """
+
+        @task
+        def identity(x):
+            return x
+
+        @flow(task_runner=task_runner)
+        async def test_flow() -> int:
+            mapped_futures = identity.map(range(1, 4))
+            single_future = identity.submit(1)
+
+            return sum([fut.result() for fut in mapped_futures + [single_future]])
+
+        result = await test_flow()
+        assert result == 7  # 1 + 2 + 3 + 1
+
+    class TestInputArguments:
+        async def test_dataclasses_can_be_passed_to_task_runners(self, task_runner):
+            """
+            this is a regression test for https://github.com/PrefectHQ/prefect/issues/6905
+            """
+            from dataclasses import dataclass
+
+            @dataclass
+            class Foo:
+                value: int
+
+            @task
+            def get_dataclass_values(n: int):
+                return [Foo(value=i) for i in range(n)]
+
+            @task
+            def print_foo(x: Foo) -> Foo:
+                print(x)
+                return x
+
+            @flow(task_runner=task_runner)
+            def test_dask_flow(n: int = 3) -> List[Foo]:
+                foos = get_dataclass_values(n)
+                future = print_foo.submit(foos[0])
+                futures = print_foo.map(foos)
+
+                return [fut.result() for fut in futures + [future]]
+
+            results = test_dask_flow()
+
+            assert results == [Foo(value=i) for i in range(3)] + [Foo(value=0)]
```

### Comparing `prefect-dask-0.2.6/tests/test_utils.py` & `prefect_dask-0.2.7/tests/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import sys
+
 import dask
 import pytest
 from distributed import Client
-from prefect import flow, task
-
 from prefect_dask import DaskTaskRunner, get_async_dask_client, get_dask_client
 
+from prefect import flow, task
+
 
 class TestDaskSyncClient:
     def test_from_task(self):
         @task
         def test_task():
             delayed_num = dask.delayed(42)
             with get_dask_client() as client:
@@ -75,16 +77,22 @@
             with get_async_dask_client():
                 pass
 
         @flow(task_runner=DaskTaskRunner)
         def test_flow():
             test_task.submit()
 
-        with pytest.raises(AttributeError, match="__enter__"):
-            test_flow()
+        if sys.version_info < (3, 11):
+            with pytest.raises(AttributeError, match="__enter__"):
+                test_flow()
+        else:
+            with pytest.raises(
+                TypeError, match="not support the context manager protocol"
+            ):
+                test_flow()
 
     async def test_from_flow(self):
         @flow(task_runner=DaskTaskRunner)
         async def test_flow():
             delayed_num = dask.delayed(42)
             async with get_async_dask_client() as client:
                 assert isinstance(client, Client)
@@ -95,16 +103,22 @@
 
     def test_from_sync_flow_error(self):
         @flow(task_runner=DaskTaskRunner)
         def test_flow():
             with get_async_dask_client():
                 pass
 
-        with pytest.raises(AttributeError, match="__enter__"):
-            test_flow()
+        if sys.version_info < (3, 11):
+            with pytest.raises(AttributeError, match="__enter__"):
+                test_flow()
+        else:
+            with pytest.raises(
+                TypeError, match="not support the context manager protocol"
+            ):
+                test_flow()
 
     async def test_outside_run_context(self):
         delayed_num = dask.delayed(42)
         async with get_async_dask_client() as client:
             assert isinstance(client, Client)
             result = await client.compute(delayed_num).result()
         assert result == 42
```


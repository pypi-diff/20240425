# Comparing `tmp/prefect-ray-0.3.3.tar.gz` & `tmp/prefect_ray-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-ray-0.3.3.tar", last modified: Wed Dec  6 17:55:48 2023, max compression
+gzip compressed data, was "prefect_ray-0.3.4.tar", last modified: Thu Apr 25 21:19:01 2024, max compression
```

## Comparing `prefect-ray-0.3.3.tar` & `prefect_ray-0.3.4.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 17:55:48.635358 prefect-ray-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-12-06 17:54:53.000000 prefect-ray-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-12-06 17:54:53.000000 prefect-ray-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11226 2023-12-06 17:55:48.635358 prefect-ray-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9684 2023-12-06 17:54:53.000000 prefect-ray-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 17:55:48.635358 prefect-ray-0.3.3/prefect_ray/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-06 17:54:53.000000 prefect-ray-0.3.3/prefect_ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-12-06 17:55:48.635358 prefect-ray-0.3.3/prefect_ray/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2023-12-06 17:54:53.000000 prefect-ray-0.3.3/prefect_ray/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     8881 2023-12-06 17:54:53.000000 prefect-ray-0.3.3/prefect_ray/task_runners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 17:55:48.631358 prefect-ray-0.3.3/prefect_ray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11226 2023-12-06 17:55:48.000000 prefect-ray-0.3.3/prefect_ray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-12-06 17:55:48.000000 prefect-ray-0.3.3/prefect_ray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 17:55:48.000000 prefect-ray-0.3.3/prefect_ray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-12-06 17:55:48.000000 prefect-ray-0.3.3/prefect_ray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-06 17:55:48.000000 prefect-ray-0.3.3/prefect_ray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2023-12-06 17:54:53.000000 prefect-ray-0.3.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-06 17:54:53.000000 prefect-ray-0.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      986 2023-12-06 17:55:48.635358 prefect-ray-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2023-12-06 17:54:53.000000 prefect-ray-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 17:55:48.631358 prefect-ray-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-12-06 17:54:53.000000 prefect-ray-0.3.3/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2023-12-06 17:54:53.000000 prefect-ray-0.3.3/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    11315 2023-12-06 17:54:53.000000 prefect-ray-0.3.3/tests/test_task_runners.py
--rw-r--r--   0 runner    (1001) docker     (127)    80049 2023-12-06 17:54:53.000000 prefect-ray-0.3.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:19:01.244249 prefect_ray-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     9157 2024-04-25 21:19:01.244249 prefect_ray-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-04-25 21:18:48.000000 prefect_ray-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:19:01.240249 prefect_ray-0.3.4/prefect_ray/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-25 21:18:48.000000 prefect_ray-0.3.4/prefect_ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 21:19:00.000000 prefect_ray-0.3.4/prefect_ray/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-25 21:18:48.000000 prefect_ray-0.3.4/prefect_ray/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-04-25 21:18:48.000000 prefect_ray-0.3.4/prefect_ray/task_runners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:19:01.240249 prefect_ray-0.3.4/prefect_ray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9157 2024-04-25 21:19:00.000000 prefect_ray-0.3.4/prefect_ray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-25 21:19:01.000000 prefect_ray-0.3.4/prefect_ray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:19:00.000000 prefect_ray-0.3.4/prefect_ray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 21:19:00.000000 prefect_ray-0.3.4/prefect_ray.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-25 21:19:00.000000 prefect_ray-0.3.4/prefect_ray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 21:19:00.000000 prefect_ray-0.3.4/prefect_ray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-25 21:18:48.000000 prefect_ray-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 21:19:01.244249 prefect_ray-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:19:01.240249 prefect_ray-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:18:48.000000 prefect_ray-0.3.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-25 21:18:48.000000 prefect_ray-0.3.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-25 21:18:48.000000 prefect_ray-0.3.4/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-25 21:18:48.000000 prefect_ray-0.3.4/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-04-25 21:18:48.000000 prefect_ray-0.3.4/tests/test_task_runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-25 21:18:48.000000 prefect_ray-0.3.4/tests/test_version.py
```

### Comparing `prefect-ray-0.3.3/PKG-INFO` & `prefect_ray-0.3.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,84 @@
 Metadata-Version: 2.1
 Name: prefect-ray
-Version: 0.3.3
+Version: 0.3.4
 Summary: Prefect integrations with the Ray execution framework.
-Home-page: https://github.com/PrefectHQ/prefect-ray
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-ray
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: prefect>=2.13.5
+Requires-Dist: prefect>=2.14.10
 Requires-Dist: ray[default]>=2.0.0
 Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: flaky; extra == "dev"
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
-Requires-Dist: pytest-asyncio<0.23.0; extra == "dev"
-Requires-Dist: mkdocs-gen-files; extra == "dev"
-Requires-Dist: interrogate; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
+Requires-Dist: mock; python_version < "3.8" and extra == "dev"
+Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-asyncio!=0.22.0,<0.23.0,>=0.18.2; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
 
 # prefect-ray
 
 <p align="center">
     <!--- Insert a cover image here -->
     <!--- <br> -->
     <a href="https://pypi.python.org/pypi/prefect-ray/" alt="PyPI version">
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-ray?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-ray/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-ray?color=0052FF&labelColor=090422" /></a>
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-ray?color=26272B&labelColor=090422"></a>
     <a href="https://pepy.tech/badge/prefect-ray/" alt="Downloads">
-        <img src="https://img.shields.io/pypi/dm/prefect-ray?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-ray/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-ray?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
+        <img src="https://img.shields.io/pypi/dm/prefect-ray?color=26272B&labelColor=090422" /></a>
 </p>
 
 ## Welcome!
 Visit the full docs [here](https://PrefectHQ.github.io/prefect-ray) to see additional examples and the API reference.
 
 `prefect-ray` contains Prefect integrations with the [Ray](https://www.ray.io/) execution framework, a flexible distributed computing framework for Python.
 
 Provides a `RayTaskRunner` that enables Prefect flows to run tasks execute tasks in parallel using Ray.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.7+.
+Requires an installation of Python 3.8 or newer.
 
 We recommend using a Python virtual environment manager such as pipenv, conda, or virtualenv.
 
-These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
+These tasks are designed to work with Prefect 2.0+. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
 
 Install `prefect-ray` with `pip`:
 
 ```bash
 pip install prefect-ray
 ```
 
-Users running Apple Silicon (such as M1 macs) will need to install ray in a miniforge conda environment.
-Click [here](https://docs.ray.io/en/master/ray-overview/installation.html#m1-mac-apple-silicon-support) for more details.
+Users running Apple Silicon (such as M1 macs) should check out the Ray docs [here](https://docs.ray.io/en/master/ray-overview/installation.html#m1-mac-apple-silicon-support) for more details.
 
 ## Running tasks on Ray
 
 The `RayTaskRunner` is a [Prefect task runner](https://docs.prefect.io/concepts/task-runners/) that submits tasks to [Ray](https://www.ray.io/) for parallel execution. 
 
 By default, a temporary Ray instance is created for the duration of the flow run.
 
@@ -172,15 +162,15 @@
 
 ## Running tasks on a Ray remote cluster
 
 When using the `RayTaskRunner` with a remote Ray cluster, you may run into issues that are not seen when using a local Ray instance. To resolve these issues, we recommend taking the following steps when working with a remote Ray cluster:
 
 1. By default, Prefect will not persist any data to the filesystem of the remote ray worker. However, if you want to take advantage of Prefect's caching ability, you will need to configure a remote result storage to persist results across task runs. 
 
-We recommend using the [Prefect UI to configure a storage block](https://docs.prefect.io/ui/blocks/) to use for remote results storage.
+We recommend using the [Prefect UI to configure a storage block](https://docs.prefect.io/concepts/blocks/) to use for remote results storage.
 
 Here's an example of a flow that uses caching and remote result storage:
 ```python
 from typing import List
 
 from prefect import flow, get_run_logger, task
 from prefect.filesystems import S3
@@ -214,15 +204,15 @@
 ```
 
 2. If you get an error stating that the module 'prefect' cannot be found, ensure `prefect` is installed on the remote cluster, with:
 ```bash
 pip install prefect
 ```
 
-3. If you get an error with a message similar to "File system created with scheme 's3' could not be created", ensure the required Python modules are installed on **both local and remote machines**. The required prerequisite modules can be found in the [Prefect documentation](https://docs.prefect.io/tutorials/storage/#prerequisites). For example, if using S3 for the remote storage:
+3. If you get an error with a message similar to "File system created with scheme 's3' could not be created", ensure the required Python modules are installed on **both local and remote machines**. The required prerequisite modules can be found in the [Prefect documentation](https://docs.prefect.io/guides/deployment/storage-guide). For example, if using S3 for the remote storage:
 ```bash
 pip install s3fs
 ```
 
 4. If you are seeing timeout or other connection errors, double check the address provided to the `RayTaskRunner`. The address should look similar to: `address='ray://<head_node_ip_address>:10001'`:
 ```bash
 RayTaskRunner(address="ray://1.23.199.255:10001")
@@ -246,37 +236,7 @@
 
 @flow(task_runner=RayTaskRunner())
 def my_flow():
     # equivalent to setting @ray.remote(num_cpus=4, num_gpus=2)
     with remote_options(num_cpus=4, num_gpus=2):
         process.submit(42)
 ```
-
-## Resources
-
-If you encounter and bugs while using `prefect-ray`, feel free to open an issue in the [prefect-ray](https://github.com/PrefectHQ/prefect-ray) repository.
-
-If you have any questions or issues while using `prefect-ray`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
-
-Feel free to star or watch [`prefect-ray`](https://github.com/PrefectHQ/prefect-ray) for updates too!
-
-## Development
-
-### Contributing
-
-If you'd like to help contribute to fix an issue or add a feature to `prefect-ray`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
-
-1. [Fork the repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository)
-2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
-3. Install the repository and its dependencies:
-```
- pip install -e ".[dev]"
-
-```
-4. Make desired changes
-5. Add tests
-6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-ray/blob/main/CHANGELOG.md)
-7. Install `pre-commit` to perform quality checks prior to commit:
-```
- pre-commit install
- ```
-8. `git commit`, `git push`, and create a pull request
```

### Comparing `prefect-ray-0.3.3/README.md` & `prefect_ray-0.3.4/prefect_ray.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,84 @@
+Metadata-Version: 2.1
+Name: prefect-ray
+Version: 0.3.4
+Summary: Prefect integrations with the Ray execution framework.
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
+License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-ray
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
+Requires-Dist: ray[default]>=2.0.0
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
+Requires-Dist: pytest-asyncio!=0.22.0,<0.23.0,>=0.18.2; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
+
 # prefect-ray
 
 <p align="center">
     <!--- Insert a cover image here -->
     <!--- <br> -->
     <a href="https://pypi.python.org/pypi/prefect-ray/" alt="PyPI version">
-        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-ray?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-ray/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-ray?color=0052FF&labelColor=090422" /></a>
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-ray?color=26272B&labelColor=090422"></a>
     <a href="https://pepy.tech/badge/prefect-ray/" alt="Downloads">
-        <img src="https://img.shields.io/pypi/dm/prefect-ray?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-ray/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-ray?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
+        <img src="https://img.shields.io/pypi/dm/prefect-ray?color=26272B&labelColor=090422" /></a>
 </p>
 
 ## Welcome!
 Visit the full docs [here](https://PrefectHQ.github.io/prefect-ray) to see additional examples and the API reference.
 
 `prefect-ray` contains Prefect integrations with the [Ray](https://www.ray.io/) execution framework, a flexible distributed computing framework for Python.
 
 Provides a `RayTaskRunner` that enables Prefect flows to run tasks execute tasks in parallel using Ray.
 
 ## Getting Started
 
 ### Python setup
 
-Requires an installation of Python 3.7+.
+Requires an installation of Python 3.8 or newer.
 
 We recommend using a Python virtual environment manager such as pipenv, conda, or virtualenv.
 
-These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
+These tasks are designed to work with Prefect 2.0+. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Installation
 
 Install `prefect-ray` with `pip`:
 
 ```bash
 pip install prefect-ray
 ```
 
-Users running Apple Silicon (such as M1 macs) will need to install ray in a miniforge conda environment.
-Click [here](https://docs.ray.io/en/master/ray-overview/installation.html#m1-mac-apple-silicon-support) for more details.
+Users running Apple Silicon (such as M1 macs) should check out the Ray docs [here](https://docs.ray.io/en/master/ray-overview/installation.html#m1-mac-apple-silicon-support) for more details.
 
 ## Running tasks on Ray
 
 The `RayTaskRunner` is a [Prefect task runner](https://docs.prefect.io/concepts/task-runners/) that submits tasks to [Ray](https://www.ray.io/) for parallel execution. 
 
 By default, a temporary Ray instance is created for the duration of the flow run.
 
@@ -132,15 +162,15 @@
 
 ## Running tasks on a Ray remote cluster
 
 When using the `RayTaskRunner` with a remote Ray cluster, you may run into issues that are not seen when using a local Ray instance. To resolve these issues, we recommend taking the following steps when working with a remote Ray cluster:
 
 1. By default, Prefect will not persist any data to the filesystem of the remote ray worker. However, if you want to take advantage of Prefect's caching ability, you will need to configure a remote result storage to persist results across task runs. 
 
-We recommend using the [Prefect UI to configure a storage block](https://docs.prefect.io/ui/blocks/) to use for remote results storage.
+We recommend using the [Prefect UI to configure a storage block](https://docs.prefect.io/concepts/blocks/) to use for remote results storage.
 
 Here's an example of a flow that uses caching and remote result storage:
 ```python
 from typing import List
 
 from prefect import flow, get_run_logger, task
 from prefect.filesystems import S3
@@ -174,15 +204,15 @@
 ```
 
 2. If you get an error stating that the module 'prefect' cannot be found, ensure `prefect` is installed on the remote cluster, with:
 ```bash
 pip install prefect
 ```
 
-3. If you get an error with a message similar to "File system created with scheme 's3' could not be created", ensure the required Python modules are installed on **both local and remote machines**. The required prerequisite modules can be found in the [Prefect documentation](https://docs.prefect.io/tutorials/storage/#prerequisites). For example, if using S3 for the remote storage:
+3. If you get an error with a message similar to "File system created with scheme 's3' could not be created", ensure the required Python modules are installed on **both local and remote machines**. The required prerequisite modules can be found in the [Prefect documentation](https://docs.prefect.io/guides/deployment/storage-guide). For example, if using S3 for the remote storage:
 ```bash
 pip install s3fs
 ```
 
 4. If you are seeing timeout or other connection errors, double check the address provided to the `RayTaskRunner`. The address should look similar to: `address='ray://<head_node_ip_address>:10001'`:
 ```bash
 RayTaskRunner(address="ray://1.23.199.255:10001")
@@ -206,37 +236,7 @@
 
 @flow(task_runner=RayTaskRunner())
 def my_flow():
     # equivalent to setting @ray.remote(num_cpus=4, num_gpus=2)
     with remote_options(num_cpus=4, num_gpus=2):
         process.submit(42)
 ```
-
-## Resources
-
-If you encounter and bugs while using `prefect-ray`, feel free to open an issue in the [prefect-ray](https://github.com/PrefectHQ/prefect-ray) repository.
-
-If you have any questions or issues while using `prefect-ray`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
-
-Feel free to star or watch [`prefect-ray`](https://github.com/PrefectHQ/prefect-ray) for updates too!
-
-## Development
-
-### Contributing
-
-If you'd like to help contribute to fix an issue or add a feature to `prefect-ray`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
-
-1. [Fork the repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository)
-2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
-3. Install the repository and its dependencies:
-```
- pip install -e ".[dev]"
-
-```
-4. Make desired changes
-5. Add tests
-6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-ray/blob/main/CHANGELOG.md)
-7. Install `pre-commit` to perform quality checks prior to commit:
-```
- pre-commit install
- ```
-8. `git commit`, `git push`, and create a pull request
```

### Comparing `prefect-ray-0.3.3/prefect_ray/context.py` & `prefect_ray-0.3.4/prefect_ray/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Contexts to manage Ray clusters and tasks.
 """
 
 from contextlib import contextmanager
 from typing import Any, Dict
 
-from prefect.context import ContextModel, ContextVar
 from pydantic import VERSION as PYDANTIC_VERSION
 
+from prefect.context import ContextModel, ContextVar
+
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field
 else:
     from pydantic import Field
 
 
 class RemoteOptionsContext(ContextModel):
```

### Comparing `prefect-ray-0.3.3/prefect_ray/task_runners.py` & `prefect_ray-0.3.4/prefect_ray/task_runners.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,22 +73,21 @@
 
 from contextlib import AsyncExitStack
 from typing import Awaitable, Callable, Dict, Optional
 from uuid import UUID
 
 import anyio
 import ray
+from ray.exceptions import RayTaskError
+
 from prefect.futures import PrefectFuture
-from prefect.server.schemas.states import State
-from prefect.states import exception_to_crashed_state
+from prefect.states import State, exception_to_crashed_state
 from prefect.task_runners import BaseTaskRunner, R, TaskConcurrencyType
 from prefect.utilities.asyncutils import sync_compatible
 from prefect.utilities.collections import visit_collection
-from ray.exceptions import RayTaskError
-
 from prefect_ray.context import RemoteOptionsContext
 
 
 class RayTaskRunner(BaseTaskRunner):
     """
     A parallel task_runner that submits tasks to `ray`.
     By default, a temporary Ray cluster is created for the duration of the flow run.
```

### Comparing `prefect-ray-0.3.3/tests/test_block_standards.py` & `prefect_ray-0.3.4/tests/test_block_standards.py`

 * *Files 11% similar despite different names*

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

### Comparing `prefect-ray-0.3.3/tests/test_context.py` & `prefect_ray-0.3.4/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `prefect-ray-0.3.3/tests/test_task_runners.py` & `prefect_ray-0.3.4/tests/test_task_runners.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,81 +3,76 @@
 import subprocess
 import sys
 import time
 import warnings
 from functools import partial
 from uuid import uuid4
 
-import prefect
-import prefect.engine
 import pytest
 import ray
 import ray.cluster_utils
+from prefect_ray import RayTaskRunner
+from prefect_ray.context import remote_options
+from ray.exceptions import TaskCancelledError
+
+import prefect
+import prefect.engine
+import tests
 from prefect import flow, get_run_logger, task
 from prefect.states import State, StateType
 from prefect.tasks import TaskRun
 from prefect.testing.fixtures import (  # noqa: F401
     hosted_api_server,
     use_hosted_api_server,
 )
 from prefect.testing.standard_test_suites import TaskRunnerStandardTestSuite
 from prefect.testing.utilities import exceptions_equal
-from ray.exceptions import TaskCancelledError
-
-import tests
-from prefect_ray import RayTaskRunner
-from prefect_ray.context import remote_options
 
 
 @pytest.fixture(scope="session")
 def event_loop(request):
     """
     Redefine the event loop to support session/module-scoped fixtures;
     see https://github.com/pytest-dev/pytest-asyncio/issues/68
     When running on Windows we need to use a non-default loop for subprocess support.
     """
     if sys.platform == "win32" and sys.version_info >= (3, 8):
         asyncio.set_event_loop_policy(asyncio.WindowsProactorEventLoopPolicy())
 
     policy = asyncio.get_event_loop_policy()
 
-    if sys.version_info < (3, 8) and sys.platform != "win32":
-        from prefect.utilities.compat import ThreadedChildWatcher
-
-        # Python < 3.8 does not use a `ThreadedChildWatcher` by default which can
-        # lead to errors in tests as the previous default `SafeChildWatcher`  is not
-        # compatible with threaded event loops.
-        policy.set_child_watcher(ThreadedChildWatcher())
-
     loop = policy.new_event_loop()
 
     # configure asyncio logging to capture long running tasks
     asyncio_logger = logging.getLogger("asyncio")
     asyncio_logger.setLevel("WARNING")
     asyncio_logger.addHandler(logging.StreamHandler())
     loop.set_debug(True)
     loop.slow_callback_duration = 0.25
 
     try:
         yield loop
     finally:
         loop.close()
 
-    # Workaround for failures in pytest_asyncio 0.17;
-    # see https://github.com/pytest-dev/pytest-asyncio/issues/257
-    policy.set_event_loop(loop)
-
 
 @pytest.fixture(scope="module")
 def machine_ray_instance():
     """
     Starts a ray instance for the current machine
     """
     subprocess.check_call(
-        ["ray", "start", "--head", "--include-dashboard", "False"],
+        [
+            "ray",
+            "start",
+            "--head",
+            "--include-dashboard",
+            "False",
+            "--disable-usage-stats",
+        ],
         cwd=str(prefect.__development_base_path__),
     )
     try:
         yield "ray://127.0.0.1:10001"
     finally:
         subprocess.run(["ray", "stop"])
 
@@ -91,15 +86,17 @@
         warnings.simplefilter("ignore", ResourceWarning)
 
         yield RayTaskRunner()
 
 
 @pytest.fixture
 def ray_task_runner_with_existing_cluster(
-    machine_ray_instance, use_hosted_api_server, hosted_api_server  # noqa: F811
+    machine_ray_instance,
+    use_hosted_api_server,  # noqa: F811
+    hosted_api_server,  # noqa: F811
 ):
     """
     Generate a ray task runner that's connected to a ray instance running in a separate
     process.
 
     This tests connection via `ray://` which is a client-based connection.
     """
@@ -126,15 +123,17 @@
         yield cluster
     finally:
         cluster.shutdown()
 
 
 @pytest.fixture
 def ray_task_runner_with_inprocess_cluster(
-    inprocess_ray_cluster, use_hosted_api_server, hosted_api_server  # noqa: F811
+    inprocess_ray_cluster,
+    use_hosted_api_server,  # noqa: F811
+    hosted_api_server,  # noqa: F811
 ):
     """
     Generate a ray task runner that's connected to an in-process cluster.
 
     This tests connection via 'localhost' which is not a client-based connection.
     """
 
@@ -148,15 +147,16 @@
             }
         },
     )
 
 
 @pytest.fixture
 def ray_task_runner_with_temporary_cluster(
-    use_hosted_api_server, hosted_api_server  # noqa: F811
+    use_hosted_api_server,  # noqa: F811
+    hosted_api_server,  # noqa: F811
 ):
     """
     Generate a ray task runner that creates a temporary cluster.
 
     This tests connection via 'localhost' which is not a client-based connection.
     """
 
@@ -167,23 +167,26 @@
                 # deserialize test tasks / flows
                 "py_modules": [tests]
             }
         },
     )
 
 
+task_runner_setups = [
+    default_ray_task_runner,
+    ray_task_runner_with_inprocess_cluster,
+    ray_task_runner_with_temporary_cluster,
+]
+
+if sys.version_info >= (3, 10):
+    task_runner_setups.append(ray_task_runner_with_existing_cluster)
+
+
 class TestRayTaskRunner(TaskRunnerStandardTestSuite):
-    @pytest.fixture(
-        params=[
-            default_ray_task_runner,
-            ray_task_runner_with_existing_cluster,
-            ray_task_runner_with_inprocess_cluster,
-            ray_task_runner_with_temporary_cluster,
-        ]
-    )
+    @pytest.fixture(params=task_runner_setups)
     def task_runner(self, request):
         yield request.getfixturevalue(
             request.param._pytestfixturefunction.name or request.param.__name__
         )
 
     def get_sleep_time(self) -> float:
         """
```


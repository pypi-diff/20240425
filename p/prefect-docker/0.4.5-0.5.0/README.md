# Comparing `tmp/prefect-docker-0.4.5.tar.gz` & `tmp/prefect_docker-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-docker-0.4.5.tar", last modified: Thu Feb 29 18:42:14 2024, max compression
+gzip compressed data, was "prefect_docker-0.5.0.tar", last modified: Thu Apr 25 19:20:11 2024, max compression
```

## Comparing `prefect-docker-0.4.5.tar` & `prefect_docker-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:42:14.276442 prefect-docker-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-02-29 18:41:26.000000 prefect-docker-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-02-29 18:41:26.000000 prefect-docker-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-02-29 18:42:14.276442 prefect-docker-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-02-29 18:41:26.000000 prefect-docker-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:42:14.276442 prefect-docker-0.4.5/prefect_docker/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-29 18:41:26.000000 prefect-docker-0.4.5/prefect_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-29 18:42:14.276442 prefect-docker-0.4.5/prefect_docker/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-02-29 18:41:26.000000 prefect-docker-0.4.5/prefect_docker/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-02-29 18:41:26.000000 prefect-docker-0.4.5/prefect_docker/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:42:14.272442 prefect-docker-0.4.5/prefect_docker/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 18:41:26.000000 prefect-docker-0.4.5/prefect_docker/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-02-29 18:41:26.000000 prefect-docker-0.4.5/prefect_docker/deployments/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-02-29 18:41:26.000000 prefect-docker-0.4.5/prefect_docker/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-02-29 18:41:26.000000 prefect-docker-0.4.5/prefect_docker/images.py
--rw-r--r--   0 runner    (1001) docker     (127)    30164 2024-02-29 18:41:26.000000 prefect-docker-0.4.5/prefect_docker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:42:14.272442 prefect-docker-0.4.5/prefect_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-02-29 18:42:14.000000 prefect-docker-0.4.5/prefect_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-02-29 18:42:14.000000 prefect-docker-0.4.5/prefect_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 18:42:14.000000 prefect-docker-0.4.5/prefect_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 18:42:14.000000 prefect-docker-0.4.5/prefect_docker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-29 18:42:14.000000 prefect-docker-0.4.5/prefect_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-29 18:42:14.000000 prefect-docker-0.4.5/prefect_docker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-29 18:41:26.000000 prefect-docker-0.4.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-29 18:41:26.000000 prefect-docker-0.4.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-29 18:42:14.276442 prefect-docker-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-02-29 18:41:26.000000 prefect-docker-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:42:14.272442 prefect-docker-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-02-29 18:41:26.000000 prefect-docker-0.4.5/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-29 18:41:26.000000 prefect-docker-0.4.5/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-02-29 18:41:26.000000 prefect-docker-0.4.5/tests/test_host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-02-29 18:41:26.000000 prefect-docker-0.4.5/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (127)    46153 2024-02-29 18:41:26.000000 prefect-docker-0.4.5/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    80049 2024-02-29 18:41:26.000000 prefect-docker-0.4.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:11.304209 prefect_docker-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-25 19:20:11.304209 prefect_docker-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:11.296209 prefect_docker-0.5.0/prefect_docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/prefect_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:10.000000 prefect_docker-0.5.0/prefect_docker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/prefect_docker/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/prefect_docker/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:11.300209 prefect_docker-0.5.0/prefect_docker/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/prefect_docker/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/prefect_docker/deployments/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/prefect_docker/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/prefect_docker/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30166 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/prefect_docker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:11.300209 prefect_docker-0.5.0/prefect_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-25 19:20:11.000000 prefect_docker-0.5.0/prefect_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-25 19:20:11.000000 prefect_docker-0.5.0/prefect_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:11.000000 prefect_docker-0.5.0/prefect_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 19:20:11.000000 prefect_docker-0.5.0/prefect_docker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-25 19:20:11.000000 prefect_docker-0.5.0/prefect_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 19:20:11.000000 prefect_docker-0.5.0/prefect_docker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:11.304209 prefect_docker-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:11.300209 prefect_docker-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:11.300209 prefect_docker-0.5.0/tests/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/tests/deployments/test_steps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:11.300209 prefect_docker-0.5.0/tests/test-project/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/tests/test-project/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/tests/test-project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/tests/test_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46168 2024-04-25 19:19:53.000000 prefect_docker-0.5.0/tests/test_worker.py
```

### Comparing `prefect-docker-0.4.5/PKG-INFO` & `prefect_docker-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,52 @@
 Metadata-Version: 2.1
 Name: prefect-docker
-Version: 0.4.5
-Summary: Prefect integrations for working with Docker
-Home-page: https://github.com/PrefectHQ/prefect-docker
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Version: 0.5.0
+Summary: Prefect integrations for interacting with Docker.
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-docker
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
 Requires-Dist: prefect>=2.13.5
 Requires-Dist: docker>=6.1.1
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: flaky; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: mock; python_version < "3.8" and extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: pytest-timeout; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 
 # prefect-docker
 
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-docker/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-docker?color=26272B&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-docker/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-docker?color=26272B&labelColor=090422" /></a>
     <a href="https://pepy.tech/badge/prefect-docker/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-docker?color=26272B&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-docker/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-docker?color=26272B&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=26272B&labelColor=090422&logo=slack" /></a>
-
 </p>
 
 ## Welcome!
 
 Prefect integrations for working with Docker.
 
 Note! The `DockerRegistryCredentials` in `prefect-docker` is a unique block, separate from the `DockerRegistry` in `prefect` core. While `DockerRegistry` implements a few functionality from both `DockerHost` and `DockerRegistryCredentials` for convenience, it does not allow much configuration to interact with a Docker host.
@@ -141,20 +127,18 @@
     )
 
 create_docker_container_flow()
 ```
 
 ## Resources
 
-If you encounter any bugs while using `prefect-docker`, feel free to open an issue in the [prefect-docker](https://github.com/PrefectHQ/prefect-docker) repository.
+If you encounter any bugs while using `prefect-docker`, feel free to open an issue in the [prefect](https://github.com/PrefectHQ/prefect) repository.
 
 If you have any questions or issues while using `prefect-docker`, you can find help in the [Prefect Slack community](https://prefect.io/slack).
 
-Feel free to ⭐️ or watch [`prefect-docker`](https://github.com/PrefectHQ/prefect-docker) for updates too!
-
 ## Development
 
 If you'd like to install a version of `prefect-docker` for development, clone the repository and perform an editable install with `pip`:
 
 ```bash
 git clone https://github.com/PrefectHQ/prefect-docker.git
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prefect-docker-0.4.5/README.md` & `prefect_docker-0.5.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 # prefect-docker
 
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-docker/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-docker?color=26272B&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-docker/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-docker?color=26272B&labelColor=090422" /></a>
     <a href="https://pepy.tech/badge/prefect-docker/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-docker?color=26272B&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-docker/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-docker?color=26272B&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=26272B&labelColor=090422&logo=slack" /></a>
-
 </p>
 
 ## Welcome!
 
 Prefect integrations for working with Docker.
 
 Note! The `DockerRegistryCredentials` in `prefect-docker` is a unique block, separate from the `DockerRegistry` in `prefect` core. While `DockerRegistry` implements a few functionality from both `DockerHost` and `DockerRegistryCredentials` for convenience, it does not allow much configuration to interact with a Docker host.
@@ -97,20 +89,18 @@
     )
 
 create_docker_container_flow()
 ```
 
 ## Resources
 
-If you encounter any bugs while using `prefect-docker`, feel free to open an issue in the [prefect-docker](https://github.com/PrefectHQ/prefect-docker) repository.
+If you encounter any bugs while using `prefect-docker`, feel free to open an issue in the [prefect](https://github.com/PrefectHQ/prefect) repository.
 
 If you have any questions or issues while using `prefect-docker`, you can find help in the [Prefect Slack community](https://prefect.io/slack).
 
-Feel free to ⭐️ or watch [`prefect-docker`](https://github.com/PrefectHQ/prefect-docker) for updates too!
-
 ## Development
 
 If you'd like to install a version of `prefect-docker` for development, clone the repository and perform an editable install with `pip`:
 
 ```bash
 git clone https://github.com/PrefectHQ/prefect-docker.git
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prefect-docker-0.4.5/prefect_docker/containers.py` & `prefect_docker-0.5.0/prefect_docker/containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Integrations with Docker Containers."""
 
 from typing import Any, Dict, List, Optional, Union
 
 from docker.models.containers import Container
+
 from prefect import get_run_logger, task
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
-
 from prefect_docker.host import DockerHost
 
 
 @task
 async def create_docker_container(
     image: str,
     command: Optional[Union[str, List[str]]] = None,
@@ -129,15 +129,15 @@
         **start_kwargs: Additional keyword arguments to pass to
             [`client.containers.get(container_id).start`](https://docker-py.readthedocs.io/en/stable/containers.html#docker.models.containers.Container.start).
 
     Returns:
         The Docker Container object.
 
     Examples:
-        Start a container with an ID that starts wtih "c157".
+        Start a container with an ID that starts with "c157".
         ```python
         from prefect import flow
         from prefect_docker.containers import start_docker_container
 
         @flow
         def start_docker_container_flow():
             container = start_docker_container(container_id="c157")
@@ -171,15 +171,15 @@
         **stop_kwargs: Additional keyword arguments to pass to
             [`client.containers.get(container_id).stop`](https://docker-py.readthedocs.io/en/stable/containers.html#docker.models.containers.Container.stop).
 
     Returns:
         The Docker Container object.
 
     Examples:
-        Stop a container with an ID that starts wtih "c157".
+        Stop a container with an ID that starts with "c157".
         ```python
         from prefect import flow
         from prefect_docker.containers import stop_docker_container
 
         @flow
         def stop_docker_container_flow():
             container = stop_docker_container(container_id="c157")
@@ -213,15 +213,15 @@
         **remove_kwargs: Additional keyword arguments to pass to
             [`client.containers.get(container_id).remove`](https://docker-py.readthedocs.io/en/stable/containers.html#docker.models.containers.Container.remove).
 
     Returns:
         The Docker Container object.
 
     Examples:
-        Removes a container with an ID that starts wtih "c157".
+        Removes a container with an ID that starts with "c157".
         ```python
         from prefect import flow
         from prefect_docker.containers import remove_docker_container
 
         @flow
         def remove_docker_container_flow():
             container = remove_docker_container(container_id="c157")
```

### Comparing `prefect-docker-0.4.5/prefect_docker/credentials.py` & `prefect_docker-0.5.0/prefect_docker/credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Module containing docker credentials."""
 import docker
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect import get_run_logger
 from prefect.blocks.core import Block
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field, SecretStr
 else:
     from pydantic import Field, SecretStr
```

### Comparing `prefect-docker-0.4.5/prefect_docker/deployments/steps.py` & `prefect_docker-0.5.0/prefect_docker/deployments/steps.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,31 +19,32 @@
     push:
         - prefect_docker.deployments.steps.push_docker_image:
             requires: prefect-docker
             image_name: "{{ build-image.image_name }}"
             tag: "{{ build-image.tag }}"
     ```
 """
+
 import os
 import sys
 from pathlib import Path
 from typing import Dict, List, Optional
 
 import docker.errors
 import pendulum
 from docker.models.images import Image
-from prefect._internal.compatibility.deprecated import deprecated_parameter
+from typing_extensions import TypedDict
+
 from prefect.utilities.dockerutils import (
     IMAGE_LABELS,
     BuildError,
     docker_client,
     get_prefect_image_name,
 )
 from prefect.utilities.slugify import slugify
-from typing_extensions import TypedDict
 
 
 class BuildDockerImageResult(TypedDict):
     """
     The result of a `build_docker_image` step.
 
     Attributes:
@@ -74,26 +75,18 @@
 
     image_name: str
     tag: str
     image: str
     additional_tags: Optional[str]
 
 
-@deprecated_parameter(
-    "push",
-    when=lambda y: y is True,
-    start_date="Jun 2023",
-    help="Use the `push_docker_image` step instead.",
-)
 def build_docker_image(
     image_name: str,
     dockerfile: str = "Dockerfile",
     tag: Optional[str] = None,
-    push: bool = False,
-    credentials: Optional[Dict] = None,
     additional_tags: Optional[List[str]] = None,
     **build_kwargs,
 ) -> BuildDockerImageResult:
     """
     Builds a Docker image for a Prefect deployment.
 
     Can be used within a `prefect.yaml` file to build a Docker
@@ -101,37 +94,34 @@
 
     Args:
         image_name: The name of the Docker image to build, including the registry and
             repository.
         dockerfile: The path to the Dockerfile used to build the image. If "auto" is
             passed, a temporary Dockerfile will be created to build the image.
         tag: The tag to apply to the built image.
-        push: DEPRECATED: Whether to push the built image to the registry.
-        credentials: A dictionary containing the username, password, and URL for the
-            registry to push the image to.
         additional_tags: Additional tags on the image, in addition to `tag`, to apply to the built image.
         **build_kwargs: Additional keyword arguments to pass to Docker when building
             the image. Available options can be found in the [`docker-py`](https://docker-py.readthedocs.io/en/stable/images.html#docker.models.images.ImageCollection.build)
             documentation.
 
     Returns:
         A dictionary containing the image name and tag of the
             built image.
 
     Example:
-        Build and push a Docker image prior to creating a deployment:
+        Build a Docker image prior to creating a deployment:
         ```yaml
         build:
             - prefect_docker.deployments.steps.build_docker_image:
                 requires: prefect-docker
                 image_name: repo-name/image-name
                 tag: dev
         ```
 
-        Build and push a Docker image with multiple tags:
+        Build a Docker image with multiple tags:
         ```yaml
         build:
             - prefect_docker.deployments.steps.build_docker_image:
                 requires: prefect-docker
                 image_name: repo-name/image-name
                 tag: dev
                 additional_tags:
@@ -143,27 +133,25 @@
         ```yaml
         build:
             - prefect_docker.deployments.steps.build_docker_image:
                 requires: prefect-docker
                 image_name: repo-name/image-name
                 tag: dev
                 dockerfile: auto
-                push: false
         ```
 
 
         Build a Docker image for a different platform:
         ```yaml
         build:
             - prefect_docker.deployments.steps.build_docker_image:
                 requires: prefect-docker
                 image_name: repo-name/image-name
                 tag: dev
                 dockerfile: Dockerfile
-                push: false
                 platform: amd64
         ```
     """  # noqa
     auto_build = dockerfile == "auto"
     if auto_build:
         lines = []
         base_image = get_prefect_image_name()
@@ -228,38 +216,14 @@
         image: Image = client.images.get(image_id)
         image.tag(repository=image_name, tag=tag)
 
         additional_tags = additional_tags or []
         for tag_ in additional_tags:
             image.tag(repository=image_name, tag=tag_)
 
-        if push:
-            if credentials is not None:
-                client.login(
-                    username=credentials.get("username"),
-                    password=credentials.get("password"),
-                    registry=credentials.get("registry_url"),
-                    reauth=credentials.get("reauth", True),
-                )
-            events = client.api.push(
-                repository=image_name, tag=tag, stream=True, decode=True
-            )
-            try:
-                for event in events:
-                    if "status" in event:
-                        sys.stdout.write(event["status"])
-                        if "progress" in event:
-                            sys.stdout.write(" " + event["progress"])
-                        sys.stdout.write("\n")
-                        sys.stdout.flush()
-                    elif "error" in event:
-                        raise OSError(event["error"])
-            finally:
-                client.api.remove_image(image=f"{image_name}:{tag}", noprune=True)
-
     return {
         "image_name": image_name,
         "tag": tag,
         "image": f"{image_name}:{tag}",
         "image_id": image_id,
         "additional_tags": additional_tags,
     }
```

### Comparing `prefect-docker-0.4.5/prefect_docker/host.py` & `prefect_docker-0.5.0/prefect_docker/host.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Module containing Docker host settings."""
 from typing import Any, Dict, Optional
 
 import docker
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect import get_run_logger
 from prefect.blocks.core import Block
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field
 else:
     from pydantic import Field
```

### Comparing `prefect-docker-0.4.5/prefect_docker/images.py` & `prefect_docker-0.5.0/prefect_docker/images.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Integrations with Docker Images."""
 
 from typing import Any, Dict, List, Optional, Union
 
 from docker.models.images import Image
+
 from prefect import get_run_logger, task
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
-
 from prefect_docker.credentials import DockerRegistryCredentials
 from prefect_docker.host import DockerHost
 
 
 @task
 async def pull_docker_image(
     repository: str,
```

### Comparing `prefect-docker-0.4.5/prefect_docker/worker.py` & `prefect_docker-0.5.0/prefect_docker/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,45 +9,46 @@
 
 Replace `my-work-pool` with the name of the work pool you want the worker
 to poll for flow runs.
 
 For more information about work pools and workers,
 checkout out the [Prefect docs](https://docs.prefect.io/concepts/work-pools/).
 """
+
 import enum
 import os
 import re
 import sys
 import urllib.parse
 import warnings
 from typing import Any, Dict, Generator, List, Optional, Tuple
 
 import anyio.abc
 import docker
 import docker.errors
 import packaging.version
-import prefect
 from docker import DockerClient
 from docker.models.containers import Container
+from pydantic import VERSION as PYDANTIC_VERSION
+
+import prefect
 from prefect.client.orchestration import ServerType, get_client
 from prefect.client.schemas import FlowRun
 from prefect.events import Event, RelatedResource, emit_event
 from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
 from prefect.server.schemas.core import Flow
 from prefect.server.schemas.responses import DeploymentResponse
 from prefect.settings import PREFECT_API_URL
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
 from prefect.utilities.dockerutils import (
     format_outlier_version_name,
     get_prefect_image_name,
     parse_image_tag,
 )
 from prefect.workers.base import BaseJobConfiguration, BaseWorker, BaseWorkerResult
-from pydantic import VERSION as PYDANTIC_VERSION
-
 from prefect_docker.credentials import DockerRegistryCredentials
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field, validator
 else:
     from pydantic import Field, validator
 
@@ -649,15 +650,15 @@
                     self._logger.warning(
                         f"Docker container {container.name} was marked for removal"
                         " before logs could be retrieved. Output will not be"
                         " streamed. "
                     )
                 else:
                     self._logger.exception(
-                        "An unexpected Docker API error occured while streaming output "
+                        "An unexpected Docker API error occurred while streaming output "
                         f"from container {container.name}."
                     )
 
             container.reload()
             if container.status != status:
                 self._logger.info(
                     f"Docker container {container.name!r} has status"
```

### Comparing `prefect-docker-0.4.5/prefect_docker.egg-info/PKG-INFO` & `prefect_docker-0.5.0/prefect_docker.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,52 @@
 Metadata-Version: 2.1
 Name: prefect-docker
-Version: 0.4.5
-Summary: Prefect integrations for working with Docker
-Home-page: https://github.com/PrefectHQ/prefect-docker
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Version: 0.5.0
+Summary: Prefect integrations for interacting with Docker.
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-docker
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
 Requires-Dist: prefect>=2.13.5
 Requires-Dist: docker>=6.1.1
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: flaky; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: mock; python_version < "3.8" and extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: pytest-timeout; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 
 # prefect-docker
 
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-docker/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-docker?color=26272B&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-docker/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-docker?color=26272B&labelColor=090422" /></a>
     <a href="https://pepy.tech/badge/prefect-docker/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-docker?color=26272B&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-docker/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-docker?color=26272B&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=26272B&labelColor=090422&logo=slack" /></a>
-
 </p>
 
 ## Welcome!
 
 Prefect integrations for working with Docker.
 
 Note! The `DockerRegistryCredentials` in `prefect-docker` is a unique block, separate from the `DockerRegistry` in `prefect` core. While `DockerRegistry` implements a few functionality from both `DockerHost` and `DockerRegistryCredentials` for convenience, it does not allow much configuration to interact with a Docker host.
@@ -141,20 +127,18 @@
     )
 
 create_docker_container_flow()
 ```
 
 ## Resources
 
-If you encounter any bugs while using `prefect-docker`, feel free to open an issue in the [prefect-docker](https://github.com/PrefectHQ/prefect-docker) repository.
+If you encounter any bugs while using `prefect-docker`, feel free to open an issue in the [prefect](https://github.com/PrefectHQ/prefect) repository.
 
 If you have any questions or issues while using `prefect-docker`, you can find help in the [Prefect Slack community](https://prefect.io/slack).
 
-Feel free to ⭐️ or watch [`prefect-docker`](https://github.com/PrefectHQ/prefect-docker) for updates too!
-
 ## Development
 
 If you'd like to install a version of `prefect-docker` for development, clone the repository and perform an editable install with `pip`:
 
 ```bash
 git clone https://github.com/PrefectHQ/prefect-docker.git
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prefect-docker-0.4.5/prefect_docker.egg-info/SOURCES.txt` & `prefect_docker-0.5.0/prefect_docker.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

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
 prefect_docker/__init__.py
 prefect_docker/_version.py
 prefect_docker/containers.py
 prefect_docker/credentials.py
 prefect_docker/host.py
 prefect_docker/images.py
 prefect_docker/worker.py
@@ -17,12 +11,17 @@
 prefect_docker.egg-info/SOURCES.txt
 prefect_docker.egg-info/dependency_links.txt
 prefect_docker.egg-info/entry_points.txt
 prefect_docker.egg-info/requires.txt
 prefect_docker.egg-info/top_level.txt
 prefect_docker/deployments/__init__.py
 prefect_docker/deployments/steps.py
+tests/conftest.py
 tests/test_containers.py
 tests/test_credentials.py
 tests/test_host.py
 tests/test_images.py
-tests/test_worker.py
+tests/test_version.py
+tests/test_worker.py
+tests/deployments/test_steps.py
+tests/test-project/flow.py
+tests/test-project/requirements.txt
```

### Comparing `prefect-docker-0.4.5/tests/test_containers.py` & `prefect_docker-0.5.0/tests/test_containers.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from unittest.mock import MagicMock
 
-from prefect.logging import disable_run_logger
-
 from prefect_docker.containers import (
     create_docker_container,
     get_docker_container_logs,
     remove_docker_container,
     start_docker_container,
     stop_docker_container,
 )
 
+from prefect.logging import disable_run_logger
+
 
 class TestCreateDockerContainer:
     async def test_create_kwargs(self, mock_docker_host: MagicMock):
         create_kwargs = dict(
             image="test_image",
             command="test_command",
             name="test_name",
```

### Comparing `prefect-docker-0.4.5/tests/test_host.py` & `prefect_docker-0.5.0/tests/test_host.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from unittest.mock import MagicMock
 
 import pytest
-from prefect.logging import disable_run_logger
-
 from prefect_docker.host import DockerHost
 
+from prefect.logging import disable_run_logger
+
 
 @pytest.fixture
 def mock_ctx_docker_client(mock_docker_client, monkeypatch) -> MagicMock:
     monkeypatch.setattr(
         "prefect_docker.host._ContextManageableDockerClient", mock_docker_client
     )
     return mock_docker_client
```

### Comparing `prefect-docker-0.4.5/tests/test_images.py` & `prefect_docker-0.5.0/tests/test_images.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from unittest.mock import MagicMock
 
 import pytest
-from prefect.logging import disable_run_logger
-
 from prefect_docker.images import pull_docker_image
 
+from prefect.logging import disable_run_logger
+
 
 class TestPullDockerImage:
     async def test_tag_and_all_tags(self, mock_docker_client_from_env: MagicMock):
         pull_kwargs = dict(repository="prefecthq/prefect", tag="latest", all_tags=True)
         with pytest.raises(
             ValueError, match="Cannot pass `tags` and `all_tags` together"
         ):
@@ -44,15 +44,15 @@
             repository="prefecthq/prefect",
             tag="latest",
         )
         with disable_run_logger():
             image = await pull_docker_image.fn(
                 docker_host=mock_docker_host,
                 docker_registry_credentials=mock_docker_registry_credentials,
-                **pull_kwargs
+                **pull_kwargs,
             )
         assert image.id == "id_1"
 
         client = mock_docker_host.get_client()
         client.__enter__.return_value.images.pull.assert_called_once_with(
             all_tags=False, **pull_kwargs
         )
```

### Comparing `prefect-docker-0.4.5/tests/test_worker.py` & `prefect_docker-0.5.0/tests/test_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 import uuid
 from unittest.mock import MagicMock, call, patch
 
 import anyio.abc
 import docker
 import docker.errors
 import docker.models.containers
-import prefect
 import pytest
 from docker import DockerClient
 from docker.models.containers import Container
 from packaging import version
+from prefect_docker.credentials import DockerRegistryCredentials
+from prefect_docker.worker import (
+    CONTAINER_LABELS,
+    DockerWorker,
+    DockerWorkerJobConfiguration,
+)
+
+import prefect
 from prefect.client.schemas import FlowRun
-from prefect.docker import get_prefect_image_name
 from prefect.events import RelatedResource
 from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
 from prefect.settings import (
     PREFECT_EXPERIMENTAL_ENABLE_WORKERS,
     PREFECT_EXPERIMENTAL_WARN_WORKERS,
     get_current_settings,
     temporary_settings,
 )
 from prefect.testing.utilities import assert_does_not_warn
-
-from prefect_docker.credentials import DockerRegistryCredentials
-from prefect_docker.worker import (
-    CONTAINER_LABELS,
-    DockerWorker,
-    DockerWorkerJobConfiguration,
-)
+from prefect.utilities.dockerutils import get_prefect_image_name
 
 FAKE_CONTAINER_ID = "fake-id"
 FAKE_BASE_URL = "http+docker://my-url"
 
 
 @pytest.fixture(autouse=True)
 def enable_workers():
@@ -955,15 +955,15 @@
 
 @pytest.mark.flaky(max_runs=3)
 async def test_container_name_collision(
     docker_client_with_cleanup: "DockerClient",
     flow_run,
     default_docker_worker_job_configuration,
 ):
-    # Generate a unique base name to avoid collissions with existing images
+    # Generate a unique base name to avoid collisions with existing images
     base_name = uuid.uuid4().hex
 
     default_docker_worker_job_configuration.name = base_name
     default_docker_worker_job_configuration.auto_remove = False
     default_docker_worker_job_configuration.prepare_for_flow_run(flow_run)
     async with DockerWorker(work_pool_name="test") as worker:
         result = await worker.run(
@@ -1045,15 +1045,15 @@
 
     async with DockerWorker(work_pool_name="test") as worker:
         await worker.run(
             flow_run=flow_run, configuration=default_docker_worker_job_configuration
         )
 
     assert (
-        "An unexpected Docker API error occured while streaming output from container"
+        "An unexpected Docker API error occurred while streaming output from container"
         " fake-name." in caplog.text
     )
 
 
 @pytest.mark.flaky(max_runs=3)
 async def test_stream_container_logs_on_real_container(
     capsys, flow_run, default_docker_worker_job_configuration
```


# Comparing `tmp/prefect-kubernetes-0.3.7.tar.gz` & `tmp/prefect_kubernetes-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-kubernetes-0.3.7.tar", last modified: Fri Mar 22 13:46:36 2024, max compression
+gzip compressed data, was "prefect_kubernetes-0.3.8.tar", last modified: Thu Apr 25 19:20:16 2024, max compression
```

## Comparing `prefect-kubernetes-0.3.7.tar` & `prefect_kubernetes-0.3.8.tar`

### file list

```diff
@@ -1,43 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:46:36.303693 prefect-kubernetes-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-03-22 13:46:36.303693 prefect-kubernetes-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:46:36.303693 prefect-kubernetes-0.3.7/prefect_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/prefect_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-22 13:46:36.303693 prefect-kubernetes-0.3.7/prefect_kubernetes/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/prefect_kubernetes/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    15378 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/prefect_kubernetes/custom_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/prefect_kubernetes/deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/prefect_kubernetes/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/prefect_kubernetes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/prefect_kubernetes/flows.py
--rw-r--r--   0 runner    (1001) docker     (127)    20339 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/prefect_kubernetes/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12069 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/prefect_kubernetes/pods.py
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/prefect_kubernetes/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/prefect_kubernetes/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    47688 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/prefect_kubernetes/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:46:36.299693 prefect-kubernetes-0.3.7/prefect_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-03-22 13:46:36.000000 prefect-kubernetes-0.3.7/prefect_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-03-22 13:46:36.000000 prefect-kubernetes-0.3.7/prefect_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 13:46:36.000000 prefect-kubernetes-0.3.7/prefect_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 13:46:36.000000 prefect-kubernetes-0.3.7/prefect_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-22 13:46:36.000000 prefect-kubernetes-0.3.7/prefect_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-22 13:46:36.000000 prefect-kubernetes-0.3.7/prefect_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-22 13:46:36.303693 prefect-kubernetes-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:46:36.299693 prefect-kubernetes-0.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9652 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/tests/test_custom_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/tests/test_deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)    14235 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/tests/test_events_replicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/tests/test_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/tests/test_pods.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)   117367 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    80043 2024-03-22 13:45:51.000000 prefect-kubernetes-0.3.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:16.429620 prefect_kubernetes-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-25 19:20:16.429620 prefect_kubernetes-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:16.421620 prefect_kubernetes-0.3.8/prefect_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:15.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/custom_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20340 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12069 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/pods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47720 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/prefect_kubernetes/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:16.429620 prefect_kubernetes-0.3.8/prefect_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-25 19:20:16.000000 prefect_kubernetes-0.3.8/prefect_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-25 19:20:16.000000 prefect_kubernetes-0.3.8/prefect_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:16.000000 prefect_kubernetes-0.3.8/prefect_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 19:20:16.000000 prefect_kubernetes-0.3.8/prefect_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-25 19:20:16.000000 prefect_kubernetes-0.3.8/prefect_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 19:20:16.000000 prefect_kubernetes-0.3.8/prefect_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:16.429620 prefect_kubernetes-0.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:16.425620 prefect_kubernetes-0.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/kube_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:16.429620 prefect_kubernetes-0.3.8/tests/sample_k8s_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/sample_k8s_resources/multiple_resource_defintion.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/sample_k8s_resources/sample_complex_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/sample_k8s_resources/sample_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/sample_k8s_resources/sample_job.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/sample_k8s_resources/sample_pod.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/sample_k8s_resources/sample_service.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_custom_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14235 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_events_replicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_pods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)   117678 2024-04-25 19:20:01.000000 prefect_kubernetes-0.3.8/tests/test_worker.py
```

### Comparing `prefect-kubernetes-0.3.7/PKG-INFO` & `prefect_kubernetes-0.3.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,54 @@
 Metadata-Version: 2.1
 Name: prefect-kubernetes
-Version: 0.3.7
+Version: 0.3.8
 Summary: Prefect integrations for interacting with Kubernetes.
-Home-page: https://github.com/PrefectHQ/prefect-kubernetes
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-kubernetes
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
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: prefect>=2.13.5
 Requires-Dist: kubernetes>=24.2.0
 Requires-Dist: tenacity>=8.2.3
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
+Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: flaky; extra == "dev"
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
+Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 
 # prefect-kubernetes
 
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-kubernetes/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-kubernetes?color=26272B&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-kubernetes/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-kubernetes?color=26272B&labelColor=090422" /></a>
     <a href="https://pypistats.org/packages/prefect-kubernetes/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-kubernetes?color=26272B&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-kubernetes/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-kubernetes?color=26272B&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=26272B&labelColor=090422&logo=slack" /></a>
-
 </p>
 
 
 ## Welcome!
 
 `prefect-kubernetes` is a collection of Prefect tasks, flows, and blocks enabling orchestration, observation and management of Kubernetes resources.
 
@@ -187,33 +173,30 @@
         deployment_updates=v1_deployment_updates,
         namespace="my-namespace"
     )
 ```
 
 ## Feedback
 
-If you encounter any bugs while using `prefect-kubernetes`, feel free to open an issue in the [prefect-kubernetes](https://github.com/PrefectHQ/prefect-kubernetes) repository.
+If you encounter any bugs while using `prefect-kubernetes`, feel free to open an issue in the [prefect](https://github.com/PrefectHQ/prefect) repository.
 
 If you have any questions or issues while using `prefect-kubernetes`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
 
-Feel free to star or watch [`prefect-kubernetes`](https://github.com/PrefectHQ/prefect-kubernetes) for updates too!
-
 ## Contributing
 
 If you'd like to help contribute to fix an issue or add a feature to `prefect-kubernetes`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
  
 Here are the steps:
  
 1. [Fork the repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository)
 2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
 3. Install the repository and its dependencies:
 ```
  pip install -e ".[dev]"
 ```
 4. Make desired changes
 5. Add tests
-6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-kubernetes/blob/main/CHANGELOG.md)
-7. Install `pre-commit` to perform quality checks prior to commit:
+6. Install `pre-commit` to perform quality checks prior to commit:
 ```
  pre-commit install
  ```
 8. `git commit`, `git push`, and create a pull request
```

### Comparing `prefect-kubernetes-0.3.7/README.md` & `prefect_kubernetes-0.3.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 # prefect-kubernetes
 
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-kubernetes/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-kubernetes?color=26272B&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-kubernetes/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-kubernetes?color=26272B&labelColor=090422" /></a>
     <a href="https://pypistats.org/packages/prefect-kubernetes/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-kubernetes?color=26272B&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-kubernetes/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-kubernetes?color=26272B&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=26272B&labelColor=090422&logo=slack" /></a>
-
 </p>
 
 
 ## Welcome!
 
 `prefect-kubernetes` is a collection of Prefect tasks, flows, and blocks enabling orchestration, observation and management of Kubernetes resources.
 
@@ -141,33 +133,30 @@
         deployment_updates=v1_deployment_updates,
         namespace="my-namespace"
     )
 ```
 
 ## Feedback
 
-If you encounter any bugs while using `prefect-kubernetes`, feel free to open an issue in the [prefect-kubernetes](https://github.com/PrefectHQ/prefect-kubernetes) repository.
+If you encounter any bugs while using `prefect-kubernetes`, feel free to open an issue in the [prefect](https://github.com/PrefectHQ/prefect) repository.
 
 If you have any questions or issues while using `prefect-kubernetes`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
 
-Feel free to star or watch [`prefect-kubernetes`](https://github.com/PrefectHQ/prefect-kubernetes) for updates too!
-
 ## Contributing
 
 If you'd like to help contribute to fix an issue or add a feature to `prefect-kubernetes`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
  
 Here are the steps:
  
 1. [Fork the repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository)
 2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
 3. Install the repository and its dependencies:
 ```
  pip install -e ".[dev]"
 ```
 4. Make desired changes
 5. Add tests
-6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-kubernetes/blob/main/CHANGELOG.md)
-7. Install `pre-commit` to perform quality checks prior to commit:
+6. Install `pre-commit` to perform quality checks prior to commit:
 ```
  pre-commit install
  ```
 8. `git commit`, `git push`, and create a pull request
```

### Comparing `prefect-kubernetes-0.3.7/prefect_kubernetes/credentials.py` & `prefect_kubernetes-0.3.8/prefect_kubernetes/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,20 @@
     AppsV1Api,
     BatchV1Api,
     Configuration,
     CoreV1Api,
     CustomObjectsApi,
 )
 from kubernetes.config.config_exception import ConfigException
-from prefect.blocks.core import Block
-from prefect.utilities.collections import listrepr
 from pydantic.version import VERSION as PYDANTIC_VERSION
 from typing_extensions import Literal, Self
 
+from prefect.blocks.core import Block
+from prefect.utilities.collections import listrepr
+
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field, validator
 else:
     from pydantic import Field, validator
 
 
 KubernetesClient = Union[AppsV1Api, BatchV1Api, CoreV1Api]
```

### Comparing `prefect-kubernetes-0.3.7/prefect_kubernetes/custom_objects.py` & `prefect_kubernetes-0.3.8/prefect_kubernetes/custom_objects.py`

 * *Files identical despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Any, Dict, Optional
 
 from prefect import task
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
-
 from prefect_kubernetes.credentials import KubernetesCredentials
 
 
 @task
 async def create_namespaced_custom_object(
     kubernetes_credentials: KubernetesCredentials,
     group: str,
```

### Comparing `prefect-kubernetes-0.3.7/prefect_kubernetes/deployments.py` & `prefect_kubernetes-0.3.8/prefect_kubernetes/deployments.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module for interacting with Kubernetes deployments from Prefect flows."""
 from typing import Any, Dict, Optional
 
 from kubernetes.client.models import V1DeleteOptions, V1Deployment, V1DeploymentList
+
 from prefect import task
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
-
 from prefect_kubernetes.credentials import KubernetesCredentials
 
 
 @task
 async def create_namespaced_deployment(
     kubernetes_credentials: KubernetesCredentials,
     new_deployment: V1Deployment,
```

### Comparing `prefect-kubernetes-0.3.7/prefect_kubernetes/events.py` & `prefect_kubernetes-0.3.8/prefect_kubernetes/events.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.3.7/prefect_kubernetes/exceptions.py` & `prefect_kubernetes-0.3.8/prefect_kubernetes/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.3.7/prefect_kubernetes/flows.py` & `prefect_kubernetes-0.3.8/prefect_kubernetes/flows.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """A module to define flows interacting with Kubernetes resources."""
 
 from typing import Any, Dict
 
 from prefect import flow, task
-
 from prefect_kubernetes.jobs import KubernetesJob
 
 
 @flow
 async def run_namespaced_job(
     kubernetes_job: KubernetesJob,
 ) -> Dict[str, Any]:
```

### Comparing `prefect-kubernetes-0.3.7/prefect_kubernetes/jobs.py` & `prefect_kubernetes-0.3.8/prefect_kubernetes/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 
 from asyncio import sleep
 from pathlib import Path
 from typing import Any, Dict, Optional, Type, Union
 
 import yaml
 from kubernetes.client.models import V1DeleteOptions, V1Job, V1JobList, V1Status
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect import task
 from prefect.blocks.abstract import JobBlock, JobRun
 from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field
 else:
     from pydantic import Field
 
 from typing_extensions import Self
```

### Comparing `prefect-kubernetes-0.3.7/prefect_kubernetes/pods.py` & `prefect_kubernetes-0.3.8/prefect_kubernetes/pods.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module for interacting with Kubernetes pods from Prefect flows."""
 from typing import Any, Callable, Dict, Optional, Union
 
 from kubernetes.client.models import V1DeleteOptions, V1Pod, V1PodList
 from kubernetes.watch import Watch
+
 from prefect import task
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
-
 from prefect_kubernetes.credentials import KubernetesCredentials
 
 
 @task
 async def create_namespaced_pod(
     kubernetes_credentials: KubernetesCredentials,
     new_pod: V1Pod,
```

### Comparing `prefect-kubernetes-0.3.7/prefect_kubernetes/services.py` & `prefect_kubernetes-0.3.8/prefect_kubernetes/services.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Tasks for working with Kubernetes services. """
 
 from typing import Any, Dict, Optional
 
 from kubernetes.client.models import V1DeleteOptions, V1Service, V1ServiceList
+
 from prefect import task
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
-
 from prefect_kubernetes.credentials import KubernetesCredentials
 
 
 @task
 async def create_namespaced_service(
     kubernetes_credentials: KubernetesCredentials,
     new_service: V1Service,
```

### Comparing `prefect-kubernetes-0.3.7/prefect_kubernetes/utilities.py` & `prefect_kubernetes-0.3.8/prefect_kubernetes/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import socket
 import sys
 from pathlib import Path
 from typing import Optional, TypeVar, Union
 
 from kubernetes.client import ApiClient
 from kubernetes.client import models as k8s_models
-from prefect.infrastructure.kubernetes import KubernetesJob, KubernetesManifest
 from slugify import slugify
 
+from prefect.infrastructure.kubernetes import KubernetesJob, KubernetesManifest
+
 # Note: `dict(str, str)` is the Kubernetes API convention for
 # representing an OpenAPI `dict` with `str` keys and values.
 base_types = {"str", "int", "float", "bool", "list[str]", "dict(str, str)", "object"}
 
 V1KubernetesModel = TypeVar("V1KubernetesModel")
```

### Comparing `prefect-kubernetes-0.3.7/prefect_kubernetes/worker.py` & `prefect_kubernetes-0.3.8/prefect_kubernetes/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,26 +99,29 @@
 For more information about work pools and workers,
 checkout out the [Prefect docs](https://docs.prefect.io/concepts/work-pools/).
 """
 
 import asyncio
 import base64
 import enum
+import json
 import logging
 import math
 import os
 import shlex
 import time
 from contextlib import contextmanager
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, Dict, Generator, Optional, Tuple, Union
 
 import anyio.abc
 from kubernetes.client.exceptions import ApiException
 from kubernetes.client.models import V1ObjectMeta, V1Secret
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect.blocks.kubernetes import KubernetesClusterConfig
 from prefect.exceptions import (
     InfrastructureError,
     InfrastructureNotAvailable,
     InfrastructureNotFound,
 )
 from prefect.server.schemas.core import Flow
@@ -130,15 +133,14 @@
 from prefect.utilities.templating import find_placeholders
 from prefect.workers.base import (
     BaseJobConfiguration,
     BaseVariables,
     BaseWorker,
     BaseWorkerResult,
 )
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field, validator
 else:
     from pydantic import Field, validator
 
 from tenacity import retry, stop_after_attempt, wait_fixed, wait_random
@@ -155,14 +157,15 @@
 if TYPE_CHECKING:
     import kubernetes
     import kubernetes.client
     import kubernetes.client.exceptions
     import kubernetes.config
     import kubernetes.watch
     from kubernetes.client import ApiClient, BatchV1Api, CoreV1Api, V1Job, V1Pod
+
     from prefect.client.schemas import FlowRun
 else:
     kubernetes = lazy_import("kubernetes")
 
 MAX_ATTEMPTS = 3
 RETRY_MIN_DELAY_SECONDS = 1
 RETRY_MIN_DELAY_JITTER_SECONDS = 0
@@ -791,16 +794,16 @@
                     configuration.namespace, configuration.job_manifest
                 )
         except kubernetes.client.exceptions.ApiException as exc:
             # Parse the reason and message from the response if feasible
             message = ""
             if exc.reason:
                 message += ": " + exc.reason
-            if exc.body and "message" in exc.body:
-                message += ": " + exc.body["message"]
+            if exc.body and "message" in (body := json.loads(exc.body)):
+                message += ": " + body["message"]
 
             raise InfrastructureError(
                 f"Unable to create Kubernetes job{message}"
             ) from exc
 
         return job
```

### Comparing `prefect-kubernetes-0.3.7/prefect_kubernetes.egg-info/PKG-INFO` & `prefect_kubernetes-0.3.8/prefect_kubernetes.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,54 @@
 Metadata-Version: 2.1
 Name: prefect-kubernetes
-Version: 0.3.7
+Version: 0.3.8
 Summary: Prefect integrations for interacting with Kubernetes.
-Home-page: https://github.com/PrefectHQ/prefect-kubernetes
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-kubernetes
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
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: prefect>=2.13.5
 Requires-Dist: kubernetes>=24.2.0
 Requires-Dist: tenacity>=8.2.3
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
+Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: flaky; extra == "dev"
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
+Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 
 # prefect-kubernetes
 
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-kubernetes/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-kubernetes?color=26272B&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-kubernetes/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-kubernetes?color=26272B&labelColor=090422" /></a>
     <a href="https://pypistats.org/packages/prefect-kubernetes/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-kubernetes?color=26272B&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-kubernetes/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-kubernetes?color=26272B&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=26272B&labelColor=090422&logo=slack" /></a>
-
 </p>
 
 
 ## Welcome!
 
 `prefect-kubernetes` is a collection of Prefect tasks, flows, and blocks enabling orchestration, observation and management of Kubernetes resources.
 
@@ -187,33 +173,30 @@
         deployment_updates=v1_deployment_updates,
         namespace="my-namespace"
     )
 ```
 
 ## Feedback
 
-If you encounter any bugs while using `prefect-kubernetes`, feel free to open an issue in the [prefect-kubernetes](https://github.com/PrefectHQ/prefect-kubernetes) repository.
+If you encounter any bugs while using `prefect-kubernetes`, feel free to open an issue in the [prefect](https://github.com/PrefectHQ/prefect) repository.
 
 If you have any questions or issues while using `prefect-kubernetes`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).
 
-Feel free to star or watch [`prefect-kubernetes`](https://github.com/PrefectHQ/prefect-kubernetes) for updates too!
-
 ## Contributing
 
 If you'd like to help contribute to fix an issue or add a feature to `prefect-kubernetes`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
  
 Here are the steps:
  
 1. [Fork the repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository)
 2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
 3. Install the repository and its dependencies:
 ```
  pip install -e ".[dev]"
 ```
 4. Make desired changes
 5. Add tests
-6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-kubernetes/blob/main/CHANGELOG.md)
-7. Install `pre-commit` to perform quality checks prior to commit:
+6. Install `pre-commit` to perform quality checks prior to commit:
 ```
  pre-commit install
  ```
 8. `git commit`, `git push`, and create a pull request
```

### Comparing `prefect-kubernetes-0.3.7/prefect_kubernetes.egg-info/SOURCES.txt` & `prefect_kubernetes-0.3.8/prefect_kubernetes.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

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
 prefect_kubernetes/__init__.py
 prefect_kubernetes/_version.py
 prefect_kubernetes/credentials.py
 prefect_kubernetes/custom_objects.py
 prefect_kubernetes/deployments.py
 prefect_kubernetes/events.py
 prefect_kubernetes/exceptions.py
@@ -21,18 +15,27 @@
 prefect_kubernetes/worker.py
 prefect_kubernetes.egg-info/PKG-INFO
 prefect_kubernetes.egg-info/SOURCES.txt
 prefect_kubernetes.egg-info/dependency_links.txt
 prefect_kubernetes.egg-info/entry_points.txt
 prefect_kubernetes.egg-info/requires.txt
 prefect_kubernetes.egg-info/top_level.txt
+tests/conftest.py
+tests/kube_config.yaml
 tests/test_block_standards.py
 tests/test_credentials.py
 tests/test_custom_objects.py
 tests/test_deployments.py
 tests/test_events_replicator.py
 tests/test_flows.py
 tests/test_jobs.py
 tests/test_pods.py
 tests/test_services.py
 tests/test_utilities.py
-tests/test_worker.py
+tests/test_version.py
+tests/test_worker.py
+tests/sample_k8s_resources/multiple_resource_defintion.yaml
+tests/sample_k8s_resources/sample_complex_deployment.yaml
+tests/sample_k8s_resources/sample_deployment.yaml
+tests/sample_k8s_resources/sample_job.yaml
+tests/sample_k8s_resources/sample_pod.yaml
+tests/sample_k8s_resources/sample_service.yaml
```

### Comparing `prefect-kubernetes-0.3.7/tests/test_block_standards.py` & `prefect_kubernetes-0.3.8/tests/test_block_standards.py`

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

### Comparing `prefect-kubernetes-0.3.7/tests/test_credentials.py` & `prefect_kubernetes-0.3.8/tests/test_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,16 @@
     ApiClient,
     AppsV1Api,
     BatchV1Api,
     CoreV1Api,
     CustomObjectsApi,
 )
 from kubernetes.config.kube_config import list_kube_config_contexts
-from pydantic.version import VERSION as PYDANTIC_VERSION
-
 from prefect_kubernetes.credentials import KubernetesClusterConfig
+from pydantic.version import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     import pydantic.v1 as pydantic
 else:
     import pydantic
 
 sample_base64_string = base64.b64encode(b"hello marvin from the other side")
```

### Comparing `prefect-kubernetes-0.3.7/tests/test_custom_objects.py` & `prefect_kubernetes-0.3.8/tests/test_custom_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pytest
 from kubernetes.client.exceptions import ApiValueError
-
 from prefect_kubernetes.custom_objects import (
     create_namespaced_custom_object,
     delete_namespaced_custom_object,
     get_namespaced_custom_object,
     get_namespaced_custom_object_status,
     list_namespaced_custom_object,
     patch_namespaced_custom_object,
```

### Comparing `prefect-kubernetes-0.3.7/tests/test_deployments.py` & `prefect_kubernetes-0.3.8/tests/test_deployments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pytest
 from kubernetes.client.models import V1DeleteOptions, V1Deployment
-
 from prefect_kubernetes.deployments import (
     create_namespaced_deployment,
     delete_namespaced_deployment,
     list_namespaced_deployment,
     patch_namespaced_deployment,
     read_namespaced_deployment,
     replace_namespaced_deployment,
```

### Comparing `prefect-kubernetes-0.3.7/tests/test_events_replicator.py` & `prefect_kubernetes-0.3.8/tests/test_events_replicator.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import copy
 import threading
 import time
 from unittest.mock import MagicMock, call, patch
 
 import pytest
 from kubernetes.client import V1Pod
+from prefect_kubernetes.events import EVICTED_REASONS, KubernetesEventsReplicator
+
 from prefect.events import RelatedResource
 from prefect.utilities.importtools import lazy_import
 
-from prefect_kubernetes.events import EVICTED_REASONS, KubernetesEventsReplicator
-
 kubernetes = lazy_import("kubernetes")
 
 
 @pytest.fixture
 def client():
     return MagicMock()
```

### Comparing `prefect-kubernetes-0.3.7/tests/test_flows.py` & `prefect_kubernetes-0.3.8/tests/test_flows.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
-from prefect import flow
-
 from prefect_kubernetes.exceptions import KubernetesJobTimeoutError
 from prefect_kubernetes.flows import run_namespaced_job
 
+from prefect import flow
+
 
 async def test_run_namespaced_job_timeout_respected(
     valid_kubernetes_job_block,
     mock_create_namespaced_job,
     mock_read_namespaced_job_status,
     mock_list_namespaced_pod,
     read_pod_logs,
```

### Comparing `prefect-kubernetes-0.3.7/tests/test_jobs.py` & `prefect_kubernetes-0.3.8/tests/test_jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pytest
 from kubernetes.client.exceptions import ApiValueError
 from kubernetes.client.models import V1Job
-
 from prefect_kubernetes.jobs import (
     KubernetesJob,
     create_namespaced_job,
     delete_namespaced_job,
     list_namespaced_job,
     patch_namespaced_job,
     read_namespaced_job,
```

### Comparing `prefect-kubernetes-0.3.7/tests/test_pods.py` & `prefect_kubernetes-0.3.8/tests/test_pods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pytest
 from kubernetes.client.exceptions import ApiException, ApiValueError
 from kubernetes.client.models import V1DeleteOptions, V1Pod
-
 from prefect_kubernetes.pods import (
     create_namespaced_pod,
     delete_namespaced_pod,
     list_namespaced_pod,
     patch_namespaced_pod,
     read_namespaced_pod,
     read_namespaced_pod_log,
```

### Comparing `prefect-kubernetes-0.3.7/tests/test_services.py` & `prefect_kubernetes-0.3.8/tests/test_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from kubernetes.client.models import V1DeleteOptions, V1Service
-
 from prefect_kubernetes.services import (
     create_namespaced_service,
     delete_namespaced_service,
     list_namespaced_service,
     patch_namespaced_service,
     read_namespaced_service,
     replace_namespaced_service,
```

### Comparing `prefect-kubernetes-0.3.7/tests/test_utilities.py` & `prefect_kubernetes-0.3.8/tests/test_utilities.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from unittest.mock import MagicMock
 
 import pytest
 from kubernetes.client import models as k8s_models
 from kubernetes.config import ConfigException
-from prefect.infrastructure.kubernetes import KubernetesJob
-
 from prefect_kubernetes.utilities import (
     convert_manifest_to_model,
     enable_socket_keep_alive,
 )
 
+from prefect.infrastructure.kubernetes import KubernetesJob
+
 FAKE_CLUSTER = "fake-cluster"
 
 base_path = "tests/sample_k8s_resources"
 
 sample_deployment_manifest = KubernetesJob.job_from_file(
     f"{base_path}/sample_deployment.yaml"
 )
```

### Comparing `prefect-kubernetes-0.3.7/tests/test_worker.py` & `prefect_kubernetes-0.3.8/tests/test_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import base64
+import json
 import re
 import uuid
 from contextlib import contextmanager
 from time import monotonic, sleep
 from unittest import mock
 from unittest.mock import MagicMock, Mock
 
 import anyio
 import anyio.abc
 import kubernetes
 import pendulum
-import prefect
 import pytest
 from kubernetes.client.exceptions import ApiException
 from kubernetes.client.models import (
     CoreV1Event,
     CoreV1EventList,
     V1ListMeta,
     V1ObjectMeta,
     V1ObjectReference,
     V1Secret,
 )
 from kubernetes.config import ConfigException
+from pydantic import VERSION as PYDANTIC_VERSION
+
+import prefect
 from prefect.client.schemas import FlowRun
 from prefect.exceptions import (
     InfrastructureError,
     InfrastructureNotAvailable,
     InfrastructureNotFound,
 )
 from prefect.server.schemas.core import Flow
@@ -34,15 +37,14 @@
     PREFECT_API_KEY,
     PREFECT_EXPERIMENTAL_ENABLE_WORKERS,
     PREFECT_EXPERIMENTAL_WARN_WORKERS,
     get_current_settings,
     temporary_settings,
 )
 from prefect.utilities.dockerutils import get_prefect_image_name
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import ValidationError
 else:
     from pydantic import ValidationError
 
 from prefect_kubernetes import KubernetesWorker
@@ -1004,15 +1006,15 @@
 class TestKubernetesWorkerJobConfiguration:
     @pytest.fixture
     def flow_run(self):
         return FlowRun(flow_id=uuid.uuid4(), name="my-flow-run-name")
 
     @pytest.fixture
     def deployment(self):
-        return DeploymentResponse(name="my-deployment-name")
+        return DeploymentResponse(name="my-deployment-name", flow_id=uuid.uuid4())
 
     @pytest.fixture
     def flow(self):
         return Flow(name="my-flow-name")
 
     @pytest.mark.parametrize(
         "template,values,expected_after_template,expected_after_preparation",
@@ -1518,24 +1520,26 @@
         self,
         flow_run,
         mock_core_client,
         mock_watch,
         mock_batch_client,
     ):
         response = MagicMock()
-        response.data = {
-            "kind": "Status",
-            "apiVersion": "v1",
-            "metadata": {},
-            "status": "Failure",
-            "message": 'jobs.batch is forbidden: User "system:serviceaccount:helm-test:prefect-worker-dev" cannot create resource "jobs" in API group "batch" in the namespace "prefect"',
-            "reason": "Forbidden",
-            "details": {"group": "batch", "kind": "jobs"},
-            "code": 403,
-        }
+        response.data = json.dumps(
+            {
+                "kind": "Status",
+                "apiVersion": "v1",
+                "metadata": {},
+                "status": "Failure",
+                "message": 'jobs.batch is forbidden: User "system:serviceaccount:helm-test:prefect-worker-dev" cannot create resource "jobs" in API group "batch" in the namespace "prefect"',
+                "reason": "Forbidden",
+                "details": {"group": "batch", "kind": "jobs"},
+                "code": 403,
+            }
+        )
         response.status = 403
         response.reason = "Forbidden"
 
         mock_batch_client.create_namespaced_job.side_effect = ApiException(
             http_resp=response
         )
 
@@ -1559,24 +1563,26 @@
         flow_run,
         mock_core_client,
         mock_watch,
         mock_batch_client,
     ):
         MAX_ATTEMPTS = 3
         response = MagicMock()
-        response.data = {
-            "kind": "Status",
-            "apiVersion": "v1",
-            "metadata": {},
-            "status": "Failure",
-            "message": 'jobs.batch is forbidden: User "system:serviceaccount:helm-test:prefect-worker-dev" cannot create resource "jobs" in API group "batch" in the namespace "prefect"',
-            "reason": "Forbidden",
-            "details": {"group": "batch", "kind": "jobs"},
-            "code": 403,
-        }
+        response.data = json.dumps(
+            {
+                "kind": "Status",
+                "apiVersion": "v1",
+                "metadata": {},
+                "status": "Failure",
+                "message": 'jobs.batch is forbidden: User "system:serviceaccount:helm-test:prefect-worker-dev" cannot create resource "jobs" in API group "batch" in the namespace "prefect"',
+                "reason": "Forbidden",
+                "details": {"group": "batch", "kind": "jobs"},
+                "code": 403,
+            }
+        )
         response.status = 403
         response.reason = "Forbidden"
 
         mock_batch_client.create_namespaced_job.side_effect = ApiException(
             http_resp=response
         )
 
@@ -1601,24 +1607,26 @@
         self,
         flow_run,
         mock_core_client,
         mock_watch,
         mock_batch_client,
     ):
         response = MagicMock()
-        response.data = {
-            "kind": "Status",
-            "apiVersion": "v1",
-            "metadata": {},
-            "status": "Failure",
-            "message": 'jobs.batch is forbidden: User "system:serviceaccount:helm-test:prefect-worker-dev" cannot create resource "jobs" in API group "batch" in the namespace "prefect"',
-            "reason": "Forbidden",
-            "details": {"group": "batch", "kind": "jobs"},
-            "code": 403,
-        }
+        response.data = json.dumps(
+            {
+                "kind": "Status",
+                "apiVersion": "v1",
+                "metadata": {},
+                "status": "Failure",
+                "message": 'jobs.batch is forbidden: User "system:serviceaccount:helm-test:prefect-worker-dev" cannot create resource "jobs" in API group "batch" in the namespace "prefect"',
+                "reason": "Forbidden",
+                "details": {"group": "batch", "kind": "jobs"},
+                "code": 403,
+            }
+        )
         response.status = 403
         response.reason = None
 
         mock_batch_client.create_namespaced_job.side_effect = ApiException(
             http_resp=response
         )
 
@@ -1641,23 +1649,25 @@
         self,
         flow_run,
         mock_core_client,
         mock_watch,
         mock_batch_client,
     ):
         response = MagicMock()
-        response.data = {
-            "kind": "Status",
-            "apiVersion": "v1",
-            "metadata": {},
-            "status": "Failure",
-            "reason": "Forbidden",
-            "details": {"group": "batch", "kind": "jobs"},
-            "code": 403,
-        }
+        response.data = json.dumps(
+            {
+                "kind": "Status",
+                "apiVersion": "v1",
+                "metadata": {},
+                "status": "Failure",
+                "reason": "Forbidden",
+                "details": {"group": "batch", "kind": "jobs"},
+                "code": 403,
+            }
+        )
         response.status = 403
         response.reason = "Test"
 
         mock_batch_client.create_namespaced_job.side_effect = ApiException(
             http_resp=response
         )
```


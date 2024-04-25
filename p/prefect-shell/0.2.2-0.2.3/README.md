# Comparing `tmp/prefect-shell-0.2.2.tar.gz` & `tmp/prefect_shell-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-shell-0.2.2.tar", last modified: Wed Nov 29 19:54:44 2023, max compression
+gzip compressed data, was "prefect_shell-0.2.3.tar", last modified: Thu Apr 25 15:15:08 2024, max compression
```

## Comparing `prefect-shell-0.2.2.tar` & `prefect_shell-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:54:44.451163 prefect-shell-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-11-29 19:54:03.000000 prefect-shell-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-11-29 19:54:03.000000 prefect-shell-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9432 2023-11-29 19:54:44.451163 prefect-shell-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7843 2023-11-29 19:54:03.000000 prefect-shell-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:54:44.451163 prefect-shell-0.2.2/prefect_shell/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-11-29 19:54:03.000000 prefect-shell-0.2.2/prefect_shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-11-29 19:54:44.451163 prefect-shell-0.2.2/prefect_shell/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    15326 2023-11-29 19:54:03.000000 prefect-shell-0.2.2/prefect_shell/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:54:44.451163 prefect-shell-0.2.2/prefect_shell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9432 2023-11-29 19:54:44.000000 prefect-shell-0.2.2/prefect_shell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      486 2023-11-29 19:54:44.000000 prefect-shell-0.2.2/prefect_shell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 19:54:44.000000 prefect-shell-0.2.2/prefect_shell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-11-29 19:54:44.000000 prefect-shell-0.2.2/prefect_shell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-11-29 19:54:44.000000 prefect-shell-0.2.2/prefect_shell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-29 19:54:44.000000 prefect-shell-0.2.2/prefect_shell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-11-29 19:54:03.000000 prefect-shell-0.2.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-29 19:54:03.000000 prefect-shell-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      763 2023-11-29 19:54:44.451163 prefect-shell-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2023-11-29 19:54:03.000000 prefect-shell-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 19:54:44.447163 prefect-shell-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-11-29 19:54:03.000000 prefect-shell-0.2.2/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     8396 2023-11-29 19:54:03.000000 prefect-shell-0.2.2/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     8078 2023-11-29 19:54:03.000000 prefect-shell-0.2.2/tests/test_commands_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)    80049 2023-11-29 19:54:03.000000 prefect-shell-0.2.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:08.558530 prefect_shell-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-04-25 15:15:08.558530 prefect_shell-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-04-25 15:14:54.000000 prefect_shell-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:08.554530 prefect_shell-0.2.3/prefect_shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 15:14:54.000000 prefect_shell-0.2.3/prefect_shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 15:15:08.000000 prefect_shell-0.2.3/prefect_shell/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15327 2024-04-25 15:14:54.000000 prefect_shell-0.2.3/prefect_shell/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:08.558530 prefect_shell-0.2.3/prefect_shell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-04-25 15:15:08.000000 prefect_shell-0.2.3/prefect_shell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-25 15:15:08.000000 prefect_shell-0.2.3/prefect_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:15:08.000000 prefect_shell-0.2.3/prefect_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 15:15:08.000000 prefect_shell-0.2.3/prefect_shell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-25 15:15:08.000000 prefect_shell-0.2.3/prefect_shell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 15:15:08.000000 prefect_shell-0.2.3/prefect_shell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-25 15:14:54.000000 prefect_shell-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:15:08.558530 prefect_shell-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:15:08.554530 prefect_shell-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 15:14:54.000000 prefect_shell-0.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-25 15:14:54.000000 prefect_shell-0.2.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-25 15:14:54.000000 prefect_shell-0.2.3/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-04-25 15:14:54.000000 prefect_shell-0.2.3/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-04-25 15:14:54.000000 prefect_shell-0.2.3/tests/test_commands_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-25 15:14:54.000000 prefect_shell-0.2.3/tests/test_version.py
```

### Comparing `prefect-shell-0.2.2/PKG-INFO` & `prefect_shell-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,65 +1,52 @@
 Metadata-Version: 2.1
 Name: prefect-shell
-Version: 0.2.2
-Summary: Prefect tasks and subflows for interacting with shell commands.
-Home-page: https://github.com/PrefectHQ/prefect-shell
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Version: 0.2.3
+Summary: Prefect integrations for interacting with shell commands.
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-shell
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
 
 # Integrating shell commands into your dataflow with `prefect-shell`
 
 <p align="center">
-    <img src="https://user-images.githubusercontent.com/15331990/216169092-20cc6e77-ee3b-4aef-a8e7-02747eb5a549.png">
-    <br>
     <a href="https://pypi.python.org/pypi/prefect-shell/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-shell?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-shell/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-shell?color=0052FF&labelColor=090422" /></a>
     <a href="https://pepy.tech/badge/prefect-shell/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-shell?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-shell/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-shell?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
 </p>
 
 Visit the full docs [here](https://PrefectHQ.github.io/prefect-shell) to see additional examples and the API reference.
 
 The prefect-shell collection makes it easy to execute shell commands in your Prefect flows. Check out the examples below to get started!
 
 ## Getting Started
```

### Comparing `prefect-shell-0.2.2/README.md` & `prefect_shell-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,14 @@
 # Integrating shell commands into your dataflow with `prefect-shell`
 
 <p align="center">
-    <img src="https://user-images.githubusercontent.com/15331990/216169092-20cc6e77-ee3b-4aef-a8e7-02747eb5a549.png">
-    <br>
     <a href="https://pypi.python.org/pypi/prefect-shell/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-shell?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-shell/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-shell?color=0052FF&labelColor=090422" /></a>
     <a href="https://pepy.tech/badge/prefect-shell/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-shell?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-shell/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-shell?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
 </p>
 
 Visit the full docs [here](https://PrefectHQ.github.io/prefect-shell) to see additional examples and the API reference.
 
 The prefect-shell collection makes it easy to execute shell commands in your Prefect flows. Check out the examples below to get started!
 
 ## Getting Started
```

### Comparing `prefect-shell-0.2.2/prefect_shell/commands.py` & `prefect_shell-0.2.3/prefect_shell/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 import tempfile
 from contextlib import AsyncExitStack, contextmanager
 from typing import Any, Dict, Generator, List, Optional, Union
 
 import anyio
 from anyio.abc import Process
 from anyio.streams.text import TextReceiveStream
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect import task
 from prefect.blocks.abstract import JobBlock, JobRun
 from prefect.logging import get_run_logger
 from prefect.utilities.asyncutils import sync_compatible
 from prefect.utilities.processutils import open_process
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import DirectoryPath, Field, PrivateAttr
 else:
     from pydantic import DirectoryPath, Field, PrivateAttr
```

### Comparing `prefect-shell-0.2.2/prefect_shell.egg-info/PKG-INFO` & `prefect_shell-0.2.3/prefect_shell.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,65 +1,52 @@
 Metadata-Version: 2.1
 Name: prefect-shell
-Version: 0.2.2
-Summary: Prefect tasks and subflows for interacting with shell commands.
-Home-page: https://github.com/PrefectHQ/prefect-shell
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Version: 0.2.3
+Summary: Prefect integrations for interacting with shell commands.
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-shell
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
 
 # Integrating shell commands into your dataflow with `prefect-shell`
 
 <p align="center">
-    <img src="https://user-images.githubusercontent.com/15331990/216169092-20cc6e77-ee3b-4aef-a8e7-02747eb5a549.png">
-    <br>
     <a href="https://pypi.python.org/pypi/prefect-shell/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-shell?color=0052FF&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-shell/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-shell?color=0052FF&labelColor=090422" /></a>
     <a href="https://pepy.tech/badge/prefect-shell/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-shell?color=0052FF&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-shell/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-shell?color=0052FF&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=0052FF&labelColor=090422&logo=slack" /></a>
-    <a href="https://discourse.prefect.io/" alt="Discourse">
-        <img src="https://img.shields.io/badge/discourse-browse_forum-red.svg?color=0052FF&labelColor=090422&logo=discourse" /></a>
 </p>
 
 Visit the full docs [here](https://PrefectHQ.github.io/prefect-shell) to see additional examples and the API reference.
 
 The prefect-shell collection makes it easy to execute shell commands in your Prefect flows. Check out the examples below to get started!
 
 ## Getting Started
```

### Comparing `prefect-shell-0.2.2/tests/test_block_standards.py` & `prefect_shell-0.2.3/tests/test_block_standards.py`

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

### Comparing `prefect-shell-0.2.2/tests/test_commands.py` & `prefect_shell-0.2.3/tests/test_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 import logging
 import os
 import sys
 from pathlib import Path
 
 import pytest
+from prefect_shell.commands import ShellOperation, shell_run_command
+
 from prefect import flow
 from prefect.testing.utilities import AsyncMock
 
-from prefect_shell.commands import ShellOperation, shell_run_command
-
 if sys.platform == "win32":
     pytest.skip(reason="see test_commands_windows.py", allow_module_level=True)
 
 
 def test_shell_run_command_error(prefect_task_runs_caplog):
     @flow
     def test_flow():
         return shell_run_command(command="ls this/is/invalid")
 
     match = "No such file or directory"
     with pytest.raises(RuntimeError, match=match):
         test_flow()
 
-    assert len(prefect_task_runs_caplog.records) == 7
-
 
 def test_shell_run_command(prefect_task_runs_caplog):
     prefect_task_runs_caplog.set_level(logging.INFO)
     echo_msg = "_THIS_ IS WORKING!!!!"
 
     @flow
     def test_flow():
```

### Comparing `prefect-shell-0.2.2/tests/test_commands_windows.py` & `prefect_shell-0.2.3/tests/test_commands_windows.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import glob
 import logging
 import os
 import sys
 from pathlib import Path
 
 import pytest
+from prefect_shell.commands import ShellOperation, shell_run_command
+
 from prefect import flow
 from prefect.testing.utilities import AsyncMock
 
-from prefect_shell.commands import ShellOperation, shell_run_command
-
 if sys.platform != "win32":
     pytest.skip(reason="see test_commands.py", allow_module_level=True)
 
 
 def test_shell_run_command_error_windows(prefect_task_runs_caplog):
     @flow
     def test_flow():
@@ -164,15 +164,16 @@
     assert len(glob.glob(f"{temp_dir}\\prefect-*.ps1")) == 0
 
 
 def test_shell_run_command_throw_exception_on_nonzero_exit_code():
     @flow
     def test_flow():
         return shell_run_command(
-            command="ping ???", shell="powershell"  # ping ??? returns exit code 1
+            command="ping ???",
+            shell="powershell",  # ping ??? returns exit code 1
         )
 
     with pytest.raises(RuntimeError, match=r"Command failed with exit code 1"):
         test_flow()
 
 
 class AsyncIter:
```


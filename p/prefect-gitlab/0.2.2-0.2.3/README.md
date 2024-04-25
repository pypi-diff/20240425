# Comparing `tmp/prefect-gitlab-0.2.2.tar.gz` & `tmp/prefect_gitlab-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-gitlab-0.2.2.tar", last modified: Wed Feb  7 19:34:21 2024, max compression
+gzip compressed data, was "prefect_gitlab-0.2.3.tar", last modified: Thu Apr 25 19:20:17 2024, max compression
```

## Comparing `prefect-gitlab-0.2.2.tar` & `prefect_gitlab-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:34:21.669501 prefect-gitlab-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-02-07 19:33:40.000000 prefect-gitlab-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-02-07 19:33:40.000000 prefect-gitlab-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-02-07 19:34:21.669501 prefect-gitlab-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-02-07 19:33:40.000000 prefect-gitlab-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:34:21.669501 prefect-gitlab-0.2.2/prefect_gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-07 19:33:40.000000 prefect-gitlab-0.2.2/prefect_gitlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-07 19:34:21.669501 prefect-gitlab-0.2.2/prefect_gitlab/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-02-07 19:33:40.000000 prefect-gitlab-0.2.2/prefect_gitlab/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-02-07 19:33:40.000000 prefect-gitlab-0.2.2/prefect_gitlab/repositories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:34:21.669501 prefect-gitlab-0.2.2/prefect_gitlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-02-07 19:34:21.000000 prefect-gitlab-0.2.2/prefect_gitlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-02-07 19:34:21.000000 prefect-gitlab-0.2.2/prefect_gitlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 19:34:21.000000 prefect-gitlab-0.2.2/prefect_gitlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-07 19:34:21.000000 prefect-gitlab-0.2.2/prefect_gitlab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-07 19:34:21.000000 prefect-gitlab-0.2.2/prefect_gitlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-07 19:34:21.000000 prefect-gitlab-0.2.2/prefect_gitlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-07 19:33:40.000000 prefect-gitlab-0.2.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-07 19:33:40.000000 prefect-gitlab-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-07 19:34:21.669501 prefect-gitlab-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-02-07 19:33:40.000000 prefect-gitlab-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 19:34:21.669501 prefect-gitlab-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-02-07 19:33:40.000000 prefect-gitlab-0.2.2/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-02-07 19:33:40.000000 prefect-gitlab-0.2.2/tests/test_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    80049 2024-02-07 19:33:40.000000 prefect-gitlab-0.2.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:17.937241 prefect_gitlab-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-25 19:20:17.937241 prefect_gitlab-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-25 19:20:05.000000 prefect_gitlab-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:17.933241 prefect_gitlab-0.2.3/prefect_gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-25 19:20:05.000000 prefect_gitlab-0.2.3/prefect_gitlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:20:17.000000 prefect_gitlab-0.2.3/prefect_gitlab/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-25 19:20:05.000000 prefect_gitlab-0.2.3/prefect_gitlab/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-04-25 19:20:05.000000 prefect_gitlab-0.2.3/prefect_gitlab/repositories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:17.937241 prefect_gitlab-0.2.3/prefect_gitlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-25 19:20:17.000000 prefect_gitlab-0.2.3/prefect_gitlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-25 19:20:17.000000 prefect_gitlab-0.2.3/prefect_gitlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:20:17.000000 prefect_gitlab-0.2.3/prefect_gitlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 19:20:17.000000 prefect_gitlab-0.2.3/prefect_gitlab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-25 19:20:17.000000 prefect_gitlab-0.2.3/prefect_gitlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 19:20:17.000000 prefect_gitlab-0.2.3/prefect_gitlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-25 19:20:05.000000 prefect_gitlab-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:20:17.937241 prefect_gitlab-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:20:17.937241 prefect_gitlab-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-25 19:20:05.000000 prefect_gitlab-0.2.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-25 19:20:05.000000 prefect_gitlab-0.2.3/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-04-25 19:20:05.000000 prefect_gitlab-0.2.3/tests/test_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-25 19:20:05.000000 prefect_gitlab-0.2.3/tests/test_version.py
```

### Comparing `prefect-gitlab-0.2.2/prefect_gitlab/credentials.py` & `prefect_gitlab-0.2.3/prefect_gitlab/credentials.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Module used to enable authenticated interactions with GitLab"""
 
 from gitlab import Gitlab
-from prefect.blocks.core import Block
 from pydantic import VERSION as PYDANTIC_VERSION
 
+from prefect.blocks.core import Block
+
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field, HttpUrl, SecretStr
 else:
     from pydantic import Field, HttpUrl, SecretStr
 
 
 class GitLabCredentials(Block):
```

### Comparing `prefect-gitlab-0.2.2/prefect_gitlab/repositories.py` & `prefect_gitlab-0.2.3/prefect_gitlab/repositories.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,20 +43,21 @@
 import io
 import urllib.parse
 from distutils.dir_util import copy_tree
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Optional, Tuple, Union
 
+from pydantic import VERSION as PYDANTIC_VERSION
+from tenacity import retry, stop_after_attempt, wait_fixed, wait_random
+
 from prefect.exceptions import InvalidRepositoryURLError
 from prefect.filesystems import ReadableDeploymentStorage
 from prefect.utilities.asyncutils import sync_compatible
 from prefect.utilities.processutils import run_process
-from pydantic import VERSION as PYDANTIC_VERSION
-from tenacity import retry, stop_after_attempt, wait_fixed, wait_random
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field, HttpUrl, validator
 else:
     from pydantic import Field, HttpUrl, validator
 
 from prefect_gitlab.credentials import GitLabCredentials
@@ -90,14 +91,20 @@
             "The URL of a GitLab repository to read from, in either HTTP/HTTPS or SSH format."  # noqa
         ),
     )
     reference: Optional[str] = Field(
         default=None,
         description="An optional reference to pin to; can be a branch name or tag.",
     )
+    git_depth: Optional[int] = Field(
+        default=1,
+        gte=1,
+        description="The number of commits that Git history is truncated to "
+        "during cloning. Set to None to fetch the entire history.",
+    )
     credentials: Optional[GitLabCredentials] = Field(
         default=None,
         description="An optional GitLab Credentials block for authenticating with "
         "private GitLab repos.",
     )
 
     @validator("credentials")
@@ -184,15 +191,16 @@
         """
         # CONSTRUCT COMMAND
         cmd = ["git", "clone", self._create_repo_url()]
         if self.reference:
             cmd += ["-b", self.reference]
 
         # Limit git history
-        cmd += ["--depth", "1"]
+        if self.git_depth is not None:
+            cmd += ["--depth", f"{self.git_depth}"]
 
         # Clone to a temporary directory and move the subdirectory over
         with TemporaryDirectory(suffix="prefect") as tmp_dir:
             cmd.append(tmp_dir)
 
             err_stream = io.StringIO()
             out_stream = io.StringIO()
```

### Comparing `prefect-gitlab-0.2.2/tests/test_credentials.py` & `prefect_gitlab-0.2.3/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-gitlab-0.2.2/tests/test_repositories.py` & `prefect_gitlab-0.2.3/tests/test_repositories.py`

 * *Files 4% similar despite different names*

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
 
 import prefect_gitlab
@@ -142,14 +143,37 @@
             "clone",
             f"http://oauth2:{credential}@gitlab.xxx.com/PrefectHQ/prefect.git",
             "--depth",
             "1",
         ]
         assert mock.await_args[0][0][: len(expected_cmd)] == expected_cmd
 
+    async def test_cloning_with_custom_depth(self, monkeypatch):
+        """Ensure that we can retrieve the whole history, i.e. support true git clone"""  # noqa: E501
+
+        class p:
+            returncode = 0
+
+        mock = AsyncMock(return_value=p())
+        monkeypatch.setattr(prefect_gitlab.repositories, "run_process", mock)
+        repo = "git@gitlab.com:PrefectHQ/prefect.git"
+        depth = None
+        g = GitLabRepository(
+            repository=repo,
+            git_depth=depth,
+        )
+        await g.get_directory()
+        assert mock.await_count == 1
+        expected_cmd = [
+            "git",
+            "clone",
+            repo,
+        ]
+        assert mock.await_args[0][0][: len(expected_cmd)] == expected_cmd
+
     async def test_ssh_fails_with_credential(self, monkeypatch):
         """Ensure that credentials cannot be passed in if the URL is not in the HTTPS/HTTP
         format.
         """
 
         class p:
             returncode = 0
@@ -166,17 +190,15 @@
         )
         with pytest.raises(InvalidRepositoryURLError, match=error_msg):
             GitLabRepository(
                 repository="git@gitlab.com:PrefectHQ/prefect.git",
                 credentials=GitLabCredentials(token=SecretStr(credential)),
             )
 
-    async def test_dir_contents_copied_correctly_with_get_directory(
-        self, monkeypatch
-    ):  # noqa
+    async def test_dir_contents_copied_correctly_with_get_directory(self, monkeypatch):  # noqa
         """Check that `get_directory` is able to correctly copy contents from src->dst"""  # noqa
 
         class p:
             returncode = 0
 
         mock = AsyncMock(return_value=p())
         monkeypatch.setattr(prefect_gitlab.repositories, "run_process", mock)
```


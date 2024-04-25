# Comparing `tmp/commitai-0.1.8.tar.gz` & `tmp/commitai-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitai-0.1.8.tar", last modified: Sat Mar  9 19:16:42 2024, max compression
+gzip compressed data, was "commitai-0.1.9.tar", last modified: Sat Mar  9 19:18:39 2024, max compression
```

## Comparing `commitai-0.1.8.tar` & `commitai-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 19:16:42.371791 commitai-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-03-09 19:16:42.371791 commitai-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-03-09 19:16:37.000000 commitai-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 19:16:42.371791 commitai-0.1.8/commitai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 19:16:37.000000 commitai-0.1.8/commitai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-03-09 19:16:37.000000 commitai-0.1.8/commitai/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-09 19:16:37.000000 commitai-0.1.8/commitai/git.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 19:16:42.371791 commitai-0.1.8/commitai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-03-09 19:16:42.000000 commitai-0.1.8/commitai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-09 19:16:42.000000 commitai-0.1.8/commitai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 19:16:42.000000 commitai-0.1.8/commitai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-09 19:16:42.000000 commitai-0.1.8/commitai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-09 19:16:42.000000 commitai-0.1.8/commitai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-09 19:16:42.000000 commitai-0.1.8/commitai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 19:16:42.371791 commitai-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-09 19:16:37.000000 commitai-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 19:18:39.344642 commitai-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-03-09 19:18:39.344642 commitai-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-03-09 19:18:34.000000 commitai-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 19:18:39.344642 commitai-0.1.9/commitai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 19:18:34.000000 commitai-0.1.9/commitai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-03-09 19:18:34.000000 commitai-0.1.9/commitai/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-09 19:18:34.000000 commitai-0.1.9/commitai/git.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 19:18:39.344642 commitai-0.1.9/commitai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-03-09 19:18:39.000000 commitai-0.1.9/commitai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-09 19:18:39.000000 commitai-0.1.9/commitai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 19:18:39.000000 commitai-0.1.9/commitai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-09 19:18:39.000000 commitai-0.1.9/commitai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-09 19:18:39.000000 commitai-0.1.9/commitai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-09 19:18:39.000000 commitai-0.1.9/commitai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 19:18:39.344642 commitai-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-09 19:18:34.000000 commitai-0.1.9/setup.py
```

### Comparing `commitai-0.1.8/PKG-INFO` & `commitai-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitai
-Version: 0.1.8
+Version: 0.1.9
 Summary: Commitai helps you generate git commit messages using AI
 Home-page: https://github.com/lguibr/commitai
 Author: Luis Guilherme
 Author-email: lgpelin92@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/lguibr/commitai/issues
 Project-URL: Documentation, https://github.com/lguibr/commitai/blob/main/README.md
@@ -23,15 +23,15 @@
 Description-Content-Type: text/markdown
 
 # CommitAi - Commit Message AI
 
 [![CI](https://github.com/lguibr/comai/workflows/CI/badge.svg)](https://github.com/lguibr/comai/actions)
 [![PyPI](https://img.shields.io/pypi/v/CommitAi.svg)](https://pypi.org/project/CommitAi/)
 [![Python Version](https://img.shields.io/pypi/pyversions/CommitAi.svg)](https://pypi.org/project/CommitAi/)
-[![License](https://img.shields.io/pypi/l/comai.svg)](https://github.com/lguibr/CommitAi/blob/main/LICENSE)
+[![License](https://img.shields.io/pypi/l/CommitAi.svg)](https://github.com/lguibr/CommitAi/blob/main/LICENSE)
 
 commitai is a command-line tool that helps you generate informative and relevant commit messages for your Git repositories using AI language models like GPT-4 and Claude. It analyzes your staged changes, combines them with a high-level explanation provided by you, and creates a commit message based on this information. Additionally, it supports custom commit message templates and a back command to reset to previous commits. This not only saves you time and effort but also ensures a consistent and meaningful commit history.
 
 ## Prerequisites
 
 - Python 3.x
 - API keys for the desired language models (e.g., OpenAI API key for GPT-4, Anthropic API key for Claude)
```

### Comparing `commitai-0.1.8/README.md` & `commitai-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # CommitAi - Commit Message AI
 
 [![CI](https://github.com/lguibr/comai/workflows/CI/badge.svg)](https://github.com/lguibr/comai/actions)
 [![PyPI](https://img.shields.io/pypi/v/CommitAi.svg)](https://pypi.org/project/CommitAi/)
 [![Python Version](https://img.shields.io/pypi/pyversions/CommitAi.svg)](https://pypi.org/project/CommitAi/)
-[![License](https://img.shields.io/pypi/l/comai.svg)](https://github.com/lguibr/CommitAi/blob/main/LICENSE)
+[![License](https://img.shields.io/pypi/l/CommitAi.svg)](https://github.com/lguibr/CommitAi/blob/main/LICENSE)
 
 commitai is a command-line tool that helps you generate informative and relevant commit messages for your Git repositories using AI language models like GPT-4 and Claude. It analyzes your staged changes, combines them with a high-level explanation provided by you, and creates a commit message based on this information. Additionally, it supports custom commit message templates and a back command to reset to previous commits. This not only saves you time and effort but also ensures a consistent and meaningful commit history.
 
 ## Prerequisites
 
 - Python 3.x
 - API keys for the desired language models (e.g., OpenAI API key for GPT-4, Anthropic API key for Claude)
```

### Comparing `commitai-0.1.8/commitai/cli.py` & `commitai-0.1.9/commitai/cli.py`

 * *Files identical despite different names*

### Comparing `commitai-0.1.8/commitai/git.py` & `commitai-0.1.9/commitai/git.py`

 * *Files identical despite different names*

### Comparing `commitai-0.1.8/commitai.egg-info/PKG-INFO` & `commitai-0.1.9/commitai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitai
-Version: 0.1.8
+Version: 0.1.9
 Summary: Commitai helps you generate git commit messages using AI
 Home-page: https://github.com/lguibr/commitai
 Author: Luis Guilherme
 Author-email: lgpelin92@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/lguibr/commitai/issues
 Project-URL: Documentation, https://github.com/lguibr/commitai/blob/main/README.md
@@ -23,15 +23,15 @@
 Description-Content-Type: text/markdown
 
 # CommitAi - Commit Message AI
 
 [![CI](https://github.com/lguibr/comai/workflows/CI/badge.svg)](https://github.com/lguibr/comai/actions)
 [![PyPI](https://img.shields.io/pypi/v/CommitAi.svg)](https://pypi.org/project/CommitAi/)
 [![Python Version](https://img.shields.io/pypi/pyversions/CommitAi.svg)](https://pypi.org/project/CommitAi/)
-[![License](https://img.shields.io/pypi/l/comai.svg)](https://github.com/lguibr/CommitAi/blob/main/LICENSE)
+[![License](https://img.shields.io/pypi/l/CommitAi.svg)](https://github.com/lguibr/CommitAi/blob/main/LICENSE)
 
 commitai is a command-line tool that helps you generate informative and relevant commit messages for your Git repositories using AI language models like GPT-4 and Claude. It analyzes your staged changes, combines them with a high-level explanation provided by you, and creates a commit message based on this information. Additionally, it supports custom commit message templates and a back command to reset to previous commits. This not only saves you time and effort but also ensures a consistent and meaningful commit history.
 
 ## Prerequisites
 
 - Python 3.x
 - API keys for the desired language models (e.g., OpenAI API key for GPT-4, Anthropic API key for Claude)
```

### Comparing `commitai-0.1.8/setup.py` & `commitai-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 repo_url = "https://github.com/lguibr/commitai"
 setup(
     name="commitai",
-    version="0.1.8",
+    version="0.1.9",
     author="Luis Guilherme",
     author_email="lgpelin92@gmail.com",
     packages=find_packages(),
     description="Commitai helps you generate git commit messages using AI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=repo_url,
```


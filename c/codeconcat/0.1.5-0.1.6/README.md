# Comparing `tmp/codeconcat-0.1.5.tar.gz` & `tmp/codeconcat-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeconcat-0.1.5.tar", last modified: Mon Apr  1 17:35:34 2024, max compression
+gzip compressed data, was "codeconcat-0.1.6.tar", last modified: Thu Apr 25 17:36:19 2024, max compression
```

## Comparing `codeconcat-0.1.5.tar` & `codeconcat-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:35:34.695770 codeconcat-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-01 17:35:34.695770 codeconcat-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-01 17:35:28.000000 codeconcat-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:35:34.695770 codeconcat-0.1.5/codeconcat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 17:35:28.000000 codeconcat-0.1.5/codeconcat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-01 17:35:28.000000 codeconcat-0.1.5/codeconcat/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:35:34.695770 codeconcat-0.1.5/codeconcat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-01 17:35:34.000000 codeconcat-0.1.5/codeconcat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-01 17:35:34.000000 codeconcat-0.1.5/codeconcat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 17:35:34.000000 codeconcat-0.1.5/codeconcat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 17:35:34.000000 codeconcat-0.1.5/codeconcat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 17:35:34.000000 codeconcat-0.1.5/codeconcat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 17:35:34.000000 codeconcat-0.1.5/codeconcat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 17:35:34.695770 codeconcat-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-01 17:35:28.000000 codeconcat-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:36:19.909926 codeconcat-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-25 17:36:13.000000 codeconcat-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-25 17:36:19.909926 codeconcat-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-25 17:36:13.000000 codeconcat-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:36:19.909926 codeconcat-0.1.6/codeconcat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:36:13.000000 codeconcat-0.1.6/codeconcat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-25 17:36:13.000000 codeconcat-0.1.6/codeconcat/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:36:19.909926 codeconcat-0.1.6/codeconcat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-25 17:36:19.000000 codeconcat-0.1.6/codeconcat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-25 17:36:19.000000 codeconcat-0.1.6/codeconcat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:36:19.000000 codeconcat-0.1.6/codeconcat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 17:36:19.000000 codeconcat-0.1.6/codeconcat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 17:36:19.000000 codeconcat-0.1.6/codeconcat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 17:36:19.000000 codeconcat-0.1.6/codeconcat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:36:19.909926 codeconcat-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-25 17:36:13.000000 codeconcat-0.1.6/setup.py
```

### Comparing `codeconcat-0.1.5/PKG-INFO` & `codeconcat-0.1.6/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,92 +1,66 @@
-Metadata-Version: 2.1
-Name: codeconcat
-Version: 0.1.5
-Summary: A tool to concatenate a folders into a single text file
-Home-page: https://github.com/lguibr/CodeConcat
-Author: Luis Guilherme
-Author-email: lgpelin92@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/lguibr/CodeConcat/issues
-Project-URL: Documentation, https://github.com/lguibr/CodeConcat/blob/main/README.md
-Project-URL: Source Code, https://github.com/lguibr/CodeConcat
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # CodeConcat
 
 [![CI](https://github.com/lguibr/codeconcat/workflows/CI/badge.svg)](https://github.com/lguibr/codeconcat/actions)
 [![PyPI](https://img.shields.io/pypi/v/codeconcat.svg)](https://pypi.org/project/codeconcat/)
 [![Python Version](https://img.shields.io/pypi/pyversions/codeconcat.svg)](https://pypi.org/project/codeconcat/)
 [![License](https://img.shields.io/pypi/l/codeconcat.svg)](https://github.com/lguibr/codeconcat/blob/main/LICENSE)
 
-CodeConcat is a command-line interface (CLI) tool that enables developers to quickly and easily concatenate an entire local code repository into a single text file. This bundled file includes a directory tree, file paths, and file content, making it an excellent resource for code review, documentation, or sharing with others.
+**CodeConcat** is a powerful command-line tool designed to simplify the process of concatenating the entire contents of local directories or code repositories into a single text file. This tool is particularly useful for developers who need to prepare large datasets for analysis or training in machine learning models, especially those that benefit from understanding the broader context provided by having complete codebases in a single file.
 
-## Features
+## Key Features
 
-- Process code from any local repository
-- Generate a directory tree for the entire codebase
-- Include file paths and file content in the output
-- Produce a human-readable text file
-- Customize the output file path and name
-- Exclude specific files or directories using patterns
-- Include only specific files or directories using whitelist patterns
+- **Efficiency**: Quickly concatenate entire directories or repositories.
+- **Flexibility**: Use include and exclude patterns to control exactly what gets included in the output.
+- **Clarity**: Each file's path is included in the output, maintaining the context necessary for large language models.
+- **Simplicity**: A straightforward command-line interface that integrates easily into any developer's workflow.
 
 ## Installation
 
-To install CodeConcat, you can use pip:
+You can install CodeConcat directly from PyPI:
 
 ```bash
-
 pip install codeconcat
 ```
 
-## Usage
+## How to Use
 
-To use CodeConcat, run the following command with the required arguments:
+### Basic Command Structure
 
 ```bash
-
-codeconcat <repo_path> <output_path> [--exclude <pattern>] [--whitelist <pattern>]
+codeconcat <source_path> <destination_file> [--exclude <pattern>] [--whitelist <pattern>]
 ```
 
-## Arguments
+### Parameters
 
-<repo_path>: The path to the local repository you want to process.
-<output_path>: The path to the output file where the concatenated codebase will be saved.
---exclude <pattern> (optional): Exclude files or directories matching the given pattern.
---whitelist <pattern> (optional): Include only files or directories matching the given pattern.
+- `<source_path>`: Path to the directory or repository to process.
+- `<destination_file>`: Path where the concatenated output will be saved.
+- `--exclude <pattern>`: (Optional) Exclude files matching this pattern.
+- `--whitelist <pattern>`: (Optional) Only include files matching this pattern.
 
-## Example
+### Examples
 
-Suppose you want to concatenate the codebase from the ~/projects/my-repo directory and save it in a file called output.txt in the current directory. The command would look like this:
+**Basic Concatenation:**
 
 ```bash
-codeconcat ~/projects/my-repo output.txt
-
+codeconcat ./my-repo output.txt
 ```
 
-If you want to exclude certain files or directories, you can use the --exclude option:
+**Using Exclude Patterns:**
 
 ```bash
-codeconcat ~/projects/my-repo output.txt --exclude "tests/\*"
-
+codeconcat ./my-repo output.txt --exclude "*.log"
 ```
 
-To include only specific files or directories, you can use the --whitelist option:
+**Using Whitelist Patterns:**
 
 ```bash
-
-codeconcat ~/projects/my-repo output.txt --whitelist "src/\*"
+codeconcat ./my-repo output.txt --whitelist "*.py"
 ```
 
+## Contributing
+
+Contributions to CodeConcat are welcome! Please check out the [issues on GitHub](https://github.com/lguibr/codeconcat/issues) or submit a pull request if you have an improvement or bug fix.
+
+## License
 
+CodeConcat is distributed under the MIT license. See the [LICENSE](LICENSE) file for more details.
```

### Comparing `codeconcat-0.1.5/codeconcat/main.py` & `codeconcat-0.1.6/codeconcat/main.py`

 * *Files identical despite different names*

### Comparing `codeconcat-0.1.5/setup.py` & `codeconcat-0.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 url = "https://github.com/lguibr/CodeConcat"
 
 setup(
     name="codeconcat",
-    version="0.1.5",
+    version="0.1.6",
     author="Luis Guilherme",
     author_email="lgpelin92@gmail.com",
     description="A tool to concatenate a folders into a single text file",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     url=url,
```


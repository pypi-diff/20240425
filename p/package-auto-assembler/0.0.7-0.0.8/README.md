# Comparing `tmp/package_auto_assembler-0.0.7.tar.gz` & `tmp/package_auto_assembler-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "package_auto_assembler-0.0.7.tar", last modified: Sun Mar  3 04:48:40 2024, max compression
+gzip compressed data, was "package_auto_assembler-0.0.8.tar", last modified: Thu Apr 25 00:58:49 2024, max compression
```

## Comparing `package_auto_assembler-0.0.7.tar` & `package_auto_assembler-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:48:40.187179 package_auto_assembler-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-03 04:45:46.000000 package_auto_assembler-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22305 2024-03-03 04:48:40.187179 package_auto_assembler-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-03-03 04:45:46.000000 package_auto_assembler-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:48:40.187179 package_auto_assembler-0.0.7/package_auto_assembler/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 04:48:35.000000 package_auto_assembler-0.0.7/package_auto_assembler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49310 2024-03-03 04:48:35.000000 package_auto_assembler-0.0.7/package_auto_assembler/package_auto_assembler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-03-03 04:48:39.000000 package_auto_assembler-0.0.7/package_auto_assembler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:48:40.187179 package_auto_assembler-0.0.7/package_auto_assembler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22305 2024-03-03 04:48:40.000000 package_auto_assembler-0.0.7/package_auto_assembler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-03 04:48:40.000000 package_auto_assembler-0.0.7/package_auto_assembler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 04:48:40.000000 package_auto_assembler-0.0.7/package_auto_assembler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-03 04:48:40.000000 package_auto_assembler-0.0.7/package_auto_assembler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-03 04:48:40.000000 package_auto_assembler-0.0.7/package_auto_assembler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 04:48:40.187179 package_auto_assembler-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:58:49.660907 package_auto_assembler-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-25 00:55:40.000000 package_auto_assembler-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    25016 2024-04-25 00:58:49.660907 package_auto_assembler-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-25 00:55:40.000000 package_auto_assembler-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:58:49.656907 package_auto_assembler-0.0.8/package_auto_assembler/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 00:58:44.000000 package_auto_assembler-0.0.8/package_auto_assembler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56391 2024-04-25 00:58:44.000000 package_auto_assembler-0.0.8/package_auto_assembler/package_auto_assembler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-25 00:58:49.000000 package_auto_assembler-0.0.8/package_auto_assembler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:58:49.660907 package_auto_assembler-0.0.8/package_auto_assembler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25016 2024-04-25 00:58:49.000000 package_auto_assembler-0.0.8/package_auto_assembler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-25 00:58:49.000000 package_auto_assembler-0.0.8/package_auto_assembler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 00:58:49.000000 package_auto_assembler-0.0.8/package_auto_assembler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 00:58:49.000000 package_auto_assembler-0.0.8/package_auto_assembler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 00:58:49.000000 package_auto_assembler-0.0.8/package_auto_assembler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 00:58:49.660907 package_auto_assembler-0.0.8/setup.cfg
```

### Comparing `package_auto_assembler-0.0.7/LICENSE` & `package_auto_assembler-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `package_auto_assembler-0.0.7/PKG-INFO` & `package_auto_assembler-0.0.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: package_auto_assembler
-Version: 0.0.7
+Version: 0.0.8
 Summary: A tool to automate package creation within ci based on just .py and optionally .ipynb file.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','packaging']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -30,28 +30,29 @@
 
 ```python
 import sys
 sys.path.append('../')
 from python_modules.package_auto_assembler import (VersionHandler, \
     ImportMappingHandler, RequirementsHandler, MetadataHandler, \
         LocalDependaciesHandler, LongDocHandler, SetupDirHandler, \
-            PackageAutoAssembler)
+            ReleaseNotesHandler, PackageAutoAssembler)
 ```
 
 ## Usage examples
 
 The examples contain: 
 1. package versioning
 2. import mapping
 3. extracting and merging requirements
 4. preparing metadata
 5. merging local dependacies into single module
 6. prepare README
 7. assembling setup directory
 8. making a package
+9. creating release notes from commit messages
 
 ### 1. Package versioning
 
 #### Initialize VersionHandler
 
 
 ```python
@@ -164,27 +165,27 @@
       <th>0</th>
       <td>2024-01-06 00:54:04</td>
       <td>example_module</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>1</th>
-      <td>2024-03-03 04:48:36</td>
+      <td>2024-04-25 00:58:46</td>
       <td>new_package</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>2</th>
-      <td>2024-03-03 04:48:36</td>
+      <td>2024-04-25 00:58:46</td>
       <td>new_package</td>
       <td>0.0.2</td>
     </tr>
     <tr>
       <th>3</th>
-      <td>2024-03-03 04:48:36</td>
+      <td>2024-04-25 00:58:46</td>
       <td>another_new_package</td>
       <td>0.0.1</td>
     </tr>
   </tbody>
 </table>
 </div>
 
@@ -275,15 +276,15 @@
     custom_modules_filepath="../tests/package_auto_assembler/dependancies"
 )
 ```
 
 
 
 
-    ['example_local_dependacy_2', 'example_local_dependacy_1']
+    ['example_local_dependacy_1', 'example_local_dependacy_2']
 
 
 
 #### Check if module is a standard python library
 
 
 ```python
@@ -820,10 +821,126 @@
     setup_directory = "./example_module"
 )
 ```
 
 
 
 
-    CompletedProcess(args=['python', './example_module/setup.py', 'sdist', 'bdist_wheel'], returncode=0, stdout="running sdist\nrunning egg_info\ncreating example_module.egg-info\nwriting example_module.egg-info/PKG-INFO\nwriting dependency_links to example_module.egg-info/dependency_links.txt\nwriting requirements to example_module.egg-info/requires.txt\nwriting top-level names to example_module.egg-info/top_level.txt\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nreading manifest file 'example_module.egg-info/SOURCES.txt'\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nrunning check\ncreating example_module-0.0.1\ncreating example_module-0.0.1/example_module\ncreating example_module-0.0.1/example_module.egg-info\ncopying files to example_module-0.0.1...\ncopying example_module/__init__.py -> example_module-0.0.1/example_module\ncopying example_module/example_module.py -> example_module-0.0.1/example_module\ncopying example_module/setup.py -> example_module-0.0.1/example_module\ncopying example_module.egg-info/PKG-INFO -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/dependency_links.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/requires.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/top_level.txt -> example_module-0.0.1/example_module.egg-info\nWriting example_module-0.0.1/setup.cfg\ncreating dist\nCreating tar archive\nremoving 'example_module-0.0.1' (and everything under it)\nrunning bdist_wheel\nrunning build\nrunning build_py\ncreating build\ncreating build/lib\ncreating build/lib/example_module\ncopying example_module/example_module.py -> build/lib/example_module\ncopying example_module/__init__.py -> build/lib/example_module\ncopying example_module/setup.py -> build/lib/example_module\ninstalling to build/bdist.linux-x86_64/wheel\nrunning install\nrunning install_lib\ncreating build/bdist.linux-x86_64\ncreating build/bdist.linux-x86_64/wheel\ncreating build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/example_module.py -> build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/__init__.py -> build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/setup.py -> build/bdist.linux-x86_64/wheel/example_module\nrunning install_egg_info\nCopying example_module.egg-info to build/bdist.linux-x86_64/wheel/example_module-0.0.1-py3.10.egg-info\nrunning install_scripts\ncreating build/bdist.linux-x86_64/wheel/example_module-0.0.1.dist-info/WHEEL\ncreating 'dist/example_module-0.0.1-py3-none-any.whl' and adding 'build/bdist.linux-x86_64/wheel' to it\nadding 'example_module/__init__.py'\nadding 'example_module/example_module.py'\nadding 'example_module/setup.py'\nadding 'example_module-0.0.1.dist-info/METADATA'\nadding 'example_module-0.0.1.dist-info/WHEEL'\nadding 'example_module-0.0.1.dist-info/top_level.txt'\nadding 'example_module-0.0.1.dist-info/RECORD'\nremoving build/bdist.linux-x86_64/wheel\n", stderr='warning: sdist: standard file not found: should have one of README, README.rst, README.txt, README.md\n\n/opt/hostedtoolcache/Python/3.10.13/x64/lib/python3.10/site-packages/setuptools/command/install.py:34: SetuptoolsDeprecationWarning: setup.py install is deprecated. Use build and pip and other standards-based tools.\n  warnings.warn(\n')
+    CompletedProcess(args=['python', './example_module/setup.py', 'sdist', 'bdist_wheel'], returncode=0, stdout="running sdist\nrunning egg_info\ncreating example_module.egg-info\nwriting example_module.egg-info/PKG-INFO\nwriting dependency_links to example_module.egg-info/dependency_links.txt\nwriting requirements to example_module.egg-info/requires.txt\nwriting top-level names to example_module.egg-info/top_level.txt\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nreading manifest file 'example_module.egg-info/SOURCES.txt'\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nrunning check\ncreating example_module-0.0.1\ncreating example_module-0.0.1/example_module\ncreating example_module-0.0.1/example_module.egg-info\ncopying files to example_module-0.0.1...\ncopying example_module/__init__.py -> example_module-0.0.1/example_module\ncopying example_module/example_module.py -> example_module-0.0.1/example_module\ncopying example_module/setup.py -> example_module-0.0.1/example_module\ncopying example_module.egg-info/PKG-INFO -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/dependency_links.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/requires.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/top_level.txt -> example_module-0.0.1/example_module.egg-info\nWriting example_module-0.0.1/setup.cfg\ncreating dist\nCreating tar archive\nremoving 'example_module-0.0.1' (and everything under it)\nrunning bdist_wheel\nrunning build\nrunning build_py\ncreating build\ncreating build/lib\ncreating build/lib/example_module\ncopying example_module/setup.py -> build/lib/example_module\ncopying example_module/__init__.py -> build/lib/example_module\ncopying example_module/example_module.py -> build/lib/example_module\ninstalling to build/bdist.linux-x86_64/wheel\nrunning install\nrunning install_lib\ncreating build/bdist.linux-x86_64\ncreating build/bdist.linux-x86_64/wheel\ncreating build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/setup.py -> build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/__init__.py -> build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/example_module.py -> build/bdist.linux-x86_64/wheel/example_module\nrunning install_egg_info\nCopying example_module.egg-info to build/bdist.linux-x86_64/wheel/example_module-0.0.1-py3.10.egg-info\nrunning install_scripts\ncreating build/bdist.linux-x86_64/wheel/example_module-0.0.1.dist-info/WHEEL\ncreating 'dist/example_module-0.0.1-py3-none-any.whl' and adding 'build/bdist.linux-x86_64/wheel' to it\nadding 'example_module/__init__.py'\nadding 'example_module/example_module.py'\nadding 'example_module/setup.py'\nadding 'example_module-0.0.1.dist-info/METADATA'\nadding 'example_module-0.0.1.dist-info/WHEEL'\nadding 'example_module-0.0.1.dist-info/top_level.txt'\nadding 'example_module-0.0.1.dist-info/RECORD'\nremoving build/bdist.linux-x86_64/wheel\n", stderr='warning: sdist: standard file not found: should have one of README, README.rst, README.txt, README.md\n\n/opt/hostedtoolcache/Python/3.10.14/x64/lib/python3.10/site-packages/setuptools/command/install.py:34: SetuptoolsDeprecationWarning: setup.py install is deprecated. Use build and pip and other standards-based tools.\n  warnings.warn(\n')
+
+
+
+### 9. Creating release notes from commit messages
+
+
+```python
+rnh = ReleaseNotesHandler(
+    # path to existing or new release notes file
+    filepath = '../tests/package_auto_assembler/release_notes.md',
+    # name of label in commit message [example_module] for filter
+    label_name = 'example_module',
+    # new version to be used in release notes
+    version = '0.0.2'
+)
+```
+
+    No messages to clean were provided
+
+
+##### - overwritting commit messages fro example
+
+
+```python
+# commit messages from last merge
+rnh.commit_messages
+```
+
+
+
+
+    ['Update README', 'Update requirements']
+
+
+
+
+```python
+example_commit_messages = [
+    '[example_module] usage example for initial release notes; bugfixes for RNH',
+    '[BUGFIX] missing parameterframe usage example and reduntant png file',
+    '[example_module] initial release notes handler',
+    'Update README',
+    'Update requirements'
+]
+rnh.commit_messages = example_commit_messages
+```
+
+##### - internal methods that run on intialiazation of ReleaseNotesHandler
+
+
+```python
+# get messages relevant only for label
+rnh._filter_commit_messages_by_package()
+print("Example filtered_messaged:")
+print(rnh.filtered_messages)
+# clean messages
+rnh._clean_and_split_commit_messages()
+print("Example processed_messages:")
+print(rnh.processed_messages)
+# augment existing release note with new entries or create new
+rnh._create_release_note_entry()
+print("Example processed_note_entries:")
+print(rnh.processed_note_entries)
+```
+
+    Example filtered_messaged:
+    ['[example_module] usage example for initial release notes; bugfixes for RNH', '[example_module] initial release notes handler']
+    Example processed_messages:
+    ['usage example for initial release notes', 'bugfixes for RNH', 'initial release notes handler']
+    Example processed_note_entries:
+    ['# Release notes\n', '\n', '### 0.0.2\n\n    - usage example for initial release notes\n    - bugfixes for RNH\n    - initial release notes handler\n\n', '### 0.0.1\n', '\n', '    - initial version of example_module\n']
+
+
+##### - saving updated relese notes
+
+
+```python
+rnh.existing_contents
+```
+
+
+
+
+    ['# Release notes\n',
+     '\n',
+     '### 0.0.1\n',
+     '\n',
+     '    - initial version of example_module\n']
+
+
+
+
+```python
+rnh.save_release_notes()
+```
+
+
+```python
+# updated content
+rnh.get_release_notes_content()
+```
+
+
+
+
+    ['# Release notes\n',
+     '\n',
+     '### 0.0.2\n',
+     '\n',
+     '    - usage example for initial release notes\n',
+     '    - bugfixes for RNH\n',
+     '    - initial release notes handler\n',
+     '\n',
+     '### 0.0.1\n',
+     '\n',
+     '    - initial version of example_module\n']
```

### Comparing `package_auto_assembler-0.0.7/README.md` & `package_auto_assembler-0.0.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -14,62 +14,62 @@
 - contains __package_metadata__ (won't package without it)
 - falls under common license
 
 The ones that were not packages, could still be used as packages with [this instruction](https://github.com/Kiril-Mordan/reusables/blob/main/docs/module_from_raw_file.md).
 
 ## Content:
  
-[module](python_modules/package_auto_assembler.py) | [usage](docs/package_auto_assembler.md) | [drawio: -Page-1](docs/package_auto_assembler-Page-1.png) | [![PyPiVersion](https://img.shields.io/pypi/v/package-auto-assembler)](https://pypi.org/project/package-auto-assembler/) - Package Auto Assembler
+[module](python_modules/shouterlog.py) | [usage](docs/shouterlog.md) | [![PyPiVersion](https://img.shields.io/pypi/v/shouterlog)](https://pypi.org/project/shouterlog/) - Shouter Log
+
+This class uses the logging module to create and manage a logger for displaying formatted messages.
+It provides a method to output various types of lines and headers, with customizable message and line lengths.
+The purpose is to be integrated into other classes that also use logger.
+
+[module](python_modules/gridlooper.py) | [usage](docs/gridlooper.md) | [drawio: -flow](docs/gridlooper-flow.png) | [![PyPiVersion](https://img.shields.io/pypi/v/gridlooper)](https://pypi.org/project/gridlooper/) - Grid Looper
+
+A tool to run experiments based on defined grid and function with single iteration.
+
+[module](python_modules/package_auto_assembler.py) | [usage](docs/package_auto_assembler.md) | [drawio: -flow](docs/package_auto_assembler-flow.png) | [drawio: -usage](docs/package_auto_assembler-usage.png) | [![PyPiVersion](https://img.shields.io/pypi/v/package-auto-assembler)](https://pypi.org/project/package-auto-assembler/) - Package Auto Assembler
 
 This tool is meant to streamline creation of single module packages.
 Its purpose is to automate as many aspects of python package creation as possible,
 to shorten a development cycle of reusable components, maintain certain standard of quality
 for reusable code. It provides tool to simplify the process of package creatrion
 to a point that it can be triggered automatically within ci/cd pipelines,
 with minimal preparations and requirements for new modules.
 
+[module](python_modules/retriever_tunner.py) | [usage](docs/retriever_tunner.md) - Retriever tunner
+
+A simple tool to compare and tune retriever performance, given a desired ranking to strive for.
+The goal is to provide a simple metric to measure how a given retriver is close to the 'ideal', generated for example
+with a use of more expensive, slower or simply no-existant method.
+
+[module](python_modules/google_drive_support.py) - Google Drive API Utilities Module
+
+This module provides a set of functions for interacting with the Google Drive API.
+It allows you to authenticate with the API, upload, download, and manage files and folders in Google Drive.
+
+[module](python_modules/parameterframe.py) | [usage](docs/parameterframe.md) | [drawio: -flow](docs/parameterframe-flow.png) | [drawio: -schema](docs/parameterframe-schema.png) | [drawio: -usage](docs/parameterframe-usage.png) | [![PyPiVersion](https://img.shields.io/pypi/v/parameterframe)](https://pypi.org/project/parameterframe/) - Parameter frame
+
+The module provides an interface for managing solution parameters.
+It allows for the structured storage and retrieval of parameter sets from a database.
+
 [module](python_modules/comparisonframe.py) | [usage](docs/comparisonframe.md) | [plantuml](docs/comparisonframe_plantuml.png) - Comparison Frame
 
 Designed to automate and streamline the process of comparing textual data, particularly focusing on various metrics
 such as character and word count, punctuation usage, and semantic similarity.
 It's particularly useful for scenarios where consistent text analysis is required,
 such as evaluating the performance of natural language processing models, monitoring content quality,
 or tracking changes in textual data over time using manual evaluation.
 
-[module](python_modules/mocker_db.py) | [usage](docs/mocker_db.md) | [![PyPiVersion](https://img.shields.io/pypi/v/mocker-db)](https://pypi.org/project/mocker-db/) - MockerDB
+[module](python_modules/mocker_db.py) | [usage](docs/mocker_db.md) | [drawio: -flow](docs/mocker_db-flow.png) | [release notes](release_notes/mocker_db.md) | [![PyPiVersion](https://img.shields.io/pypi/v/mocker-db)](https://pypi.org/project/mocker-db/) - MockerDB
 
 A python module that contains mock vector database like solution built around
 dictionary data type. It contains methods necessary to interact with this 'database',
 embed, search and persist.
 
-[module](python_modules/shouterlog.py) | [usage](docs/shouterlog.md) | [![PyPiVersion](https://img.shields.io/pypi/v/shouterlog)](https://pypi.org/project/shouterlog/) - Shouter Log
-
-This class uses the logging module to create and manage a logger for displaying formatted messages.
-It provides a method to output various types of lines and headers, with customizable message and line lengths.
-The purpose is to be integrated into other classes that also use logger.
-
-[module](python_modules/google_drive_support.py) - Google Drive API Utilities Module
-
-This module provides a set of functions for interacting with the Google Drive API.
-It allows you to authenticate with the API, upload, download, and manage files and folders in Google Drive.
-
 [module](python_modules/search_based_extractor.py) | [usage](docs/search_based_extractor.md) - Search Based Extractor
 
 Utility to simplify webscraping by taking advantave of search and assumptions about html structure.
 Extractor allows to find parent html element that contains searched term, record path to it in a file
 and reuse that to scrape data with same html structure.
 
-[module](python_modules/redis_database_handler.py) - Redis Database Handler
-
-A handler class for managing interactions with a Redis database. This class provides methods for initializing a logger,
-establishing a connection with the Redis server, performing CRUD operations, and searching within the stored data based on embeddings.
-
-[module](python_modules/retriever_tunner.py) | [usage](docs/retriever_tunner.md) - Retriever tunner
-
-A simple tool to compare and tune retriever performance, given a desired ranking to strive for.
-The goal is to provide a simple metric to measure how a given retriver is close to the 'ideal', generated for example
-with a use of more expensive, slower or simply no-existant method.
-
-[module](python_modules/gridlooper.py) | [drawio: -Page-1](docs/gridlooper-Page-1.png) - Grid Looper
-
-A tool to run experiments based on defined grid and function with single iteration.
-
```

### Comparing `package_auto_assembler-0.0.7/package_auto_assembler/package_auto_assembler.py` & `package_auto_assembler-0.0.8/package_auto_assembler/package_auto_assembler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1198,15 +1198,208 @@
     long_description_content_type='text/markdown',
     {metadata_str}
 )
         """
         with open(os.path.join(setup_directory, 'setup.py'), 'w') as file:
             file.write(setup_content)
 
+@attr.s
+class ReleaseNotesHandler:
+
+    # inputs
+    filepath = attr.ib(default='release_notes.md', type=str)
+    label_name = attr.ib(default=None, type=list)
+    version = attr.ib(default='0.0.1', type=str)
+
+    # processed
+    existing_contents = attr.ib(default=None, type=list)
+    commit_messages = attr.ib(default=None, type=list)
+    filtered_messages = attr.ib(default=None, type=list)
+    processed_messages = attr.ib(default=None, type=list)
+    processed_note_entries  = attr.ib(default=None, type=list)
+
+
+    logger = attr.ib(default=None)
+    logger_name = attr.ib(default='Release Notes Handler')
+    loggerLvl = attr.ib(default=logging.INFO)
+    logger_format = attr.ib(default=None)
+
+    def __attrs_post_init__(self):
+        self._initialize_logger()
+
+        if self.existing_contents is None:
+            self.existing_contents = self.get_release_notes_content()
+        if self.commit_messages is None:
+            self._get_commits_since_last_merge()
+        if self.filtered_messages is not []:
+            self._filter_commit_messages_by_package()
+        if self.processed_messages is None:
+            self._clean_and_split_commit_messages()
+        if self.processed_note_entries is None:
+            self._create_release_note_entry()
+
+
+    def _initialize_logger(self):
+
+        """
+        Initialize a logger for the class instance based on the specified logging level and logger name.
+        """
+
+        if self.logger is None:
+            logging.basicConfig(level=self.loggerLvl, format=self.logger_format)
+            logger = logging.getLogger(self.logger_name)
+            logger.setLevel(self.loggerLvl)
+
+            self.logger = logger
+
+    def _get_commits_since_last_merge(self):
+
+        # First, find the last merge commit
+        find_merge_command = ["git", "log", "--merges", "--format=%H", "-n", "1"]
+        merge_result = subprocess.run(find_merge_command, capture_output=True, text=True)
+        if merge_result.returncode != 0:
+            raise Exception("Failed to find last merge commit")
+
+        last_merge_commit_hash = merge_result.stdout.strip()
+        if not last_merge_commit_hash:
+            raise Exception("No merge commits found")
+
+        # Now, get all commits after the last merge commit
+        log_command = ["git", "log", f"{last_merge_commit_hash}..HEAD", "--no-merges", "--format=%s"]
+        log_result = subprocess.run(log_command, capture_output=True, text=True)
+        if log_result.returncode != 0:
+            raise Exception("Error running git log")
+
+        # Each commit message is separated by newlines
+        commit_messages = log_result.stdout.strip().split("\n")
+
+        self.commit_messages = commit_messages
+
+    def _filter_commit_messages_by_package(self,
+                                           commit_messages : list = None,
+                                           label_name : str = None):
+
+        if commit_messages is None:
+            commit_messages = self.commit_messages
+
+        if label_name is None:
+            label_name = self.label_name
+
+        # This pattern will match messages that start with optional spaces, followed by [<package_name>],
+        # possibly surrounded by spaces, and then any text. It is case-sensitive.
+        pattern = re.compile(rf'\s*\[\s*{re.escape(label_name)}\s*\].*')
+
+        # Filter messages that match the pattern
+        filtered_messages = [msg for msg in commit_messages if pattern.search(msg)]
+
+        self.filtered_messages = filtered_messages
+
+
+    def _clean_and_split_commit_messages(self,
+                                         commit_messages : list = None):
+
+        if commit_messages is None:
+            commit_messages = self.filtered_messages
+
+        # Remove the package name tag and split messages by ";"
+        cleaned_and_split_messages = []
+        tag_pattern = re.compile(r'\[\s*[^]]*\]\s*')  # Matches the package name tag
+
+        if len(commit_messages) == 0:
+            self.logger.warning("No messages to clean were provided")
+            cleaned_and_split_messages = []
+        else:
+            for msg in commit_messages:
+                # Remove the package name tag from the message
+                clean_msg = tag_pattern.sub('', msg).strip()
+                # Split the message by ";"
+                split_messages = clean_msg.split(';')
+                # Strip whitespace from each split message and filter out any empty strings
+                split_messages = [message.strip() for message in split_messages if message.strip()]
+                cleaned_and_split_messages.extend(split_messages)
+
+        self.processed_messages = cleaned_and_split_messages
+
+
+    def _create_release_note_entry(self,
+                                  existing_contents : str = None,
+                                  version : str = None,
+                                  new_messages : list = None):
+
+        if existing_contents is None:
+            existing_contents = self.existing_contents.copy()
+
+        if version is None:
+            version = self.version
+
+        if new_messages is None:
+            new_messages = self.processed_messages
+
+        # Prepare the new release note section
+        new_release_note = f"### {version}\n\n"
+        for msg in new_messages:
+            new_release_note += f"    - {msg}\n"
+
+        # If there are existing contents, integrate the new entry
+        if existing_contents:
+            # Find the location of the first version heading to insert the new release note right after
+            index = 0
+            for line in existing_contents:
+                if line.strip().startswith('###'):
+                    break
+                index += 1
+
+            # Insert the new release note section into the contents
+            existing_contents.insert(index, new_release_note + "\n")
+        else:
+            # If no existing contents, start a new list of contents
+            existing_contents = ['# Release notes\n\n', new_release_note + "\n"]
+
+        self.processed_note_entries = existing_contents
+
+
+    def get_release_notes_content(self,
+                                  filepath : str = None) -> str:
+
+        """
+        Get release notes content.
+        """
+
+        if filepath is None:
+            filepath = self.filepath
+
+        if os.path.exists(filepath):
+            # Read the existing release notes
+            with open(filepath, 'r') as file:
+                content = file.readlines()
+        else:
+            # No existing file, start with empty contents
+            content = None
+
+        return content
+
+
+    def save_release_notes(self,
+                           filepath : str = None,
+                           note_entries : str = None):
+
+        """
+        Save updated release notes content.
+        """
+
+        if filepath is None:
+            filepath = self.filepath
+
+        if note_entries is None:
+            note_entries = self.processed_note_entries
+
 
+        # Write the updated or new contents back to the file
+        with open(filepath, 'w') as file:
+            file.writelines(note_entries)
 
 @attr.s
 class PackageAutoAssembler:
     # pylint: disable=too-many-instance-attributes
 
     ## inputs
     module_name = attr.ib(type=str)
```

### Comparing `package_auto_assembler-0.0.7/package_auto_assembler/setup.py` & `package_auto_assembler-0.0.8/package_auto_assembler/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,14 @@
       long_description = fh.read()
 else:
   long_description = ''
 
 setup(
     name="package_auto_assembler",
     packages=["package_auto_assembler"],
-    install_requires=['### package_auto_assembler.py', 'pandas', 'attrs>=22.2.0', 'pyyaml', 'stdlib-list', 'nbformat', 'nbconvert'],
+    install_requires=['### package_auto_assembler.py', 'attrs>=22.2.0', 'pandas', 'pyyaml', 'stdlib-list', 'nbconvert', 'nbformat'],
     classifiers=['Development Status :: 3 - Alpha', 'Intended Audience :: Developers', 'Intended Audience :: Science/Research', 'Programming Language :: Python :: 3', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11', 'License :: OSI Approved :: MIT License', 'Topic :: Scientific/Engineering'],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to automate package creation within ci based on just .py and optionally .ipynb file.", keywords="['python', 'packaging']", version="0.0.7"
+    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to automate package creation within ci based on just .py and optionally .ipynb file.", keywords="['python', 'packaging']", version="0.0.8"
 )
```

### Comparing `package_auto_assembler-0.0.7/package_auto_assembler.egg-info/PKG-INFO` & `package_auto_assembler-0.0.8/package_auto_assembler.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: package-auto-assembler
-Version: 0.0.7
+Version: 0.0.8
 Summary: A tool to automate package creation within ci based on just .py and optionally .ipynb file.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','packaging']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -30,28 +30,29 @@
 
 ```python
 import sys
 sys.path.append('../')
 from python_modules.package_auto_assembler import (VersionHandler, \
     ImportMappingHandler, RequirementsHandler, MetadataHandler, \
         LocalDependaciesHandler, LongDocHandler, SetupDirHandler, \
-            PackageAutoAssembler)
+            ReleaseNotesHandler, PackageAutoAssembler)
 ```
 
 ## Usage examples
 
 The examples contain: 
 1. package versioning
 2. import mapping
 3. extracting and merging requirements
 4. preparing metadata
 5. merging local dependacies into single module
 6. prepare README
 7. assembling setup directory
 8. making a package
+9. creating release notes from commit messages
 
 ### 1. Package versioning
 
 #### Initialize VersionHandler
 
 
 ```python
@@ -164,27 +165,27 @@
       <th>0</th>
       <td>2024-01-06 00:54:04</td>
       <td>example_module</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>1</th>
-      <td>2024-03-03 04:48:36</td>
+      <td>2024-04-25 00:58:46</td>
       <td>new_package</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>2</th>
-      <td>2024-03-03 04:48:36</td>
+      <td>2024-04-25 00:58:46</td>
       <td>new_package</td>
       <td>0.0.2</td>
     </tr>
     <tr>
       <th>3</th>
-      <td>2024-03-03 04:48:36</td>
+      <td>2024-04-25 00:58:46</td>
       <td>another_new_package</td>
       <td>0.0.1</td>
     </tr>
   </tbody>
 </table>
 </div>
 
@@ -275,15 +276,15 @@
     custom_modules_filepath="../tests/package_auto_assembler/dependancies"
 )
 ```
 
 
 
 
-    ['example_local_dependacy_2', 'example_local_dependacy_1']
+    ['example_local_dependacy_1', 'example_local_dependacy_2']
 
 
 
 #### Check if module is a standard python library
 
 
 ```python
@@ -820,10 +821,126 @@
     setup_directory = "./example_module"
 )
 ```
 
 
 
 
-    CompletedProcess(args=['python', './example_module/setup.py', 'sdist', 'bdist_wheel'], returncode=0, stdout="running sdist\nrunning egg_info\ncreating example_module.egg-info\nwriting example_module.egg-info/PKG-INFO\nwriting dependency_links to example_module.egg-info/dependency_links.txt\nwriting requirements to example_module.egg-info/requires.txt\nwriting top-level names to example_module.egg-info/top_level.txt\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nreading manifest file 'example_module.egg-info/SOURCES.txt'\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nrunning check\ncreating example_module-0.0.1\ncreating example_module-0.0.1/example_module\ncreating example_module-0.0.1/example_module.egg-info\ncopying files to example_module-0.0.1...\ncopying example_module/__init__.py -> example_module-0.0.1/example_module\ncopying example_module/example_module.py -> example_module-0.0.1/example_module\ncopying example_module/setup.py -> example_module-0.0.1/example_module\ncopying example_module.egg-info/PKG-INFO -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/dependency_links.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/requires.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/top_level.txt -> example_module-0.0.1/example_module.egg-info\nWriting example_module-0.0.1/setup.cfg\ncreating dist\nCreating tar archive\nremoving 'example_module-0.0.1' (and everything under it)\nrunning bdist_wheel\nrunning build\nrunning build_py\ncreating build\ncreating build/lib\ncreating build/lib/example_module\ncopying example_module/example_module.py -> build/lib/example_module\ncopying example_module/__init__.py -> build/lib/example_module\ncopying example_module/setup.py -> build/lib/example_module\ninstalling to build/bdist.linux-x86_64/wheel\nrunning install\nrunning install_lib\ncreating build/bdist.linux-x86_64\ncreating build/bdist.linux-x86_64/wheel\ncreating build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/example_module.py -> build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/__init__.py -> build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/setup.py -> build/bdist.linux-x86_64/wheel/example_module\nrunning install_egg_info\nCopying example_module.egg-info to build/bdist.linux-x86_64/wheel/example_module-0.0.1-py3.10.egg-info\nrunning install_scripts\ncreating build/bdist.linux-x86_64/wheel/example_module-0.0.1.dist-info/WHEEL\ncreating 'dist/example_module-0.0.1-py3-none-any.whl' and adding 'build/bdist.linux-x86_64/wheel' to it\nadding 'example_module/__init__.py'\nadding 'example_module/example_module.py'\nadding 'example_module/setup.py'\nadding 'example_module-0.0.1.dist-info/METADATA'\nadding 'example_module-0.0.1.dist-info/WHEEL'\nadding 'example_module-0.0.1.dist-info/top_level.txt'\nadding 'example_module-0.0.1.dist-info/RECORD'\nremoving build/bdist.linux-x86_64/wheel\n", stderr='warning: sdist: standard file not found: should have one of README, README.rst, README.txt, README.md\n\n/opt/hostedtoolcache/Python/3.10.13/x64/lib/python3.10/site-packages/setuptools/command/install.py:34: SetuptoolsDeprecationWarning: setup.py install is deprecated. Use build and pip and other standards-based tools.\n  warnings.warn(\n')
+    CompletedProcess(args=['python', './example_module/setup.py', 'sdist', 'bdist_wheel'], returncode=0, stdout="running sdist\nrunning egg_info\ncreating example_module.egg-info\nwriting example_module.egg-info/PKG-INFO\nwriting dependency_links to example_module.egg-info/dependency_links.txt\nwriting requirements to example_module.egg-info/requires.txt\nwriting top-level names to example_module.egg-info/top_level.txt\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nreading manifest file 'example_module.egg-info/SOURCES.txt'\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nrunning check\ncreating example_module-0.0.1\ncreating example_module-0.0.1/example_module\ncreating example_module-0.0.1/example_module.egg-info\ncopying files to example_module-0.0.1...\ncopying example_module/__init__.py -> example_module-0.0.1/example_module\ncopying example_module/example_module.py -> example_module-0.0.1/example_module\ncopying example_module/setup.py -> example_module-0.0.1/example_module\ncopying example_module.egg-info/PKG-INFO -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/dependency_links.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/requires.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/top_level.txt -> example_module-0.0.1/example_module.egg-info\nWriting example_module-0.0.1/setup.cfg\ncreating dist\nCreating tar archive\nremoving 'example_module-0.0.1' (and everything under it)\nrunning bdist_wheel\nrunning build\nrunning build_py\ncreating build\ncreating build/lib\ncreating build/lib/example_module\ncopying example_module/setup.py -> build/lib/example_module\ncopying example_module/__init__.py -> build/lib/example_module\ncopying example_module/example_module.py -> build/lib/example_module\ninstalling to build/bdist.linux-x86_64/wheel\nrunning install\nrunning install_lib\ncreating build/bdist.linux-x86_64\ncreating build/bdist.linux-x86_64/wheel\ncreating build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/setup.py -> build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/__init__.py -> build/bdist.linux-x86_64/wheel/example_module\ncopying build/lib/example_module/example_module.py -> build/bdist.linux-x86_64/wheel/example_module\nrunning install_egg_info\nCopying example_module.egg-info to build/bdist.linux-x86_64/wheel/example_module-0.0.1-py3.10.egg-info\nrunning install_scripts\ncreating build/bdist.linux-x86_64/wheel/example_module-0.0.1.dist-info/WHEEL\ncreating 'dist/example_module-0.0.1-py3-none-any.whl' and adding 'build/bdist.linux-x86_64/wheel' to it\nadding 'example_module/__init__.py'\nadding 'example_module/example_module.py'\nadding 'example_module/setup.py'\nadding 'example_module-0.0.1.dist-info/METADATA'\nadding 'example_module-0.0.1.dist-info/WHEEL'\nadding 'example_module-0.0.1.dist-info/top_level.txt'\nadding 'example_module-0.0.1.dist-info/RECORD'\nremoving build/bdist.linux-x86_64/wheel\n", stderr='warning: sdist: standard file not found: should have one of README, README.rst, README.txt, README.md\n\n/opt/hostedtoolcache/Python/3.10.14/x64/lib/python3.10/site-packages/setuptools/command/install.py:34: SetuptoolsDeprecationWarning: setup.py install is deprecated. Use build and pip and other standards-based tools.\n  warnings.warn(\n')
+
+
+
+### 9. Creating release notes from commit messages
+
+
+```python
+rnh = ReleaseNotesHandler(
+    # path to existing or new release notes file
+    filepath = '../tests/package_auto_assembler/release_notes.md',
+    # name of label in commit message [example_module] for filter
+    label_name = 'example_module',
+    # new version to be used in release notes
+    version = '0.0.2'
+)
+```
+
+    No messages to clean were provided
+
+
+##### - overwritting commit messages fro example
+
+
+```python
+# commit messages from last merge
+rnh.commit_messages
+```
+
+
+
+
+    ['Update README', 'Update requirements']
+
+
+
+
+```python
+example_commit_messages = [
+    '[example_module] usage example for initial release notes; bugfixes for RNH',
+    '[BUGFIX] missing parameterframe usage example and reduntant png file',
+    '[example_module] initial release notes handler',
+    'Update README',
+    'Update requirements'
+]
+rnh.commit_messages = example_commit_messages
+```
+
+##### - internal methods that run on intialiazation of ReleaseNotesHandler
+
+
+```python
+# get messages relevant only for label
+rnh._filter_commit_messages_by_package()
+print("Example filtered_messaged:")
+print(rnh.filtered_messages)
+# clean messages
+rnh._clean_and_split_commit_messages()
+print("Example processed_messages:")
+print(rnh.processed_messages)
+# augment existing release note with new entries or create new
+rnh._create_release_note_entry()
+print("Example processed_note_entries:")
+print(rnh.processed_note_entries)
+```
+
+    Example filtered_messaged:
+    ['[example_module] usage example for initial release notes; bugfixes for RNH', '[example_module] initial release notes handler']
+    Example processed_messages:
+    ['usage example for initial release notes', 'bugfixes for RNH', 'initial release notes handler']
+    Example processed_note_entries:
+    ['# Release notes\n', '\n', '### 0.0.2\n\n    - usage example for initial release notes\n    - bugfixes for RNH\n    - initial release notes handler\n\n', '### 0.0.1\n', '\n', '    - initial version of example_module\n']
+
+
+##### - saving updated relese notes
+
+
+```python
+rnh.existing_contents
+```
+
+
+
+
+    ['# Release notes\n',
+     '\n',
+     '### 0.0.1\n',
+     '\n',
+     '    - initial version of example_module\n']
+
+
+
+
+```python
+rnh.save_release_notes()
+```
+
+
+```python
+# updated content
+rnh.get_release_notes_content()
+```
+
+
+
+
+    ['# Release notes\n',
+     '\n',
+     '### 0.0.2\n',
+     '\n',
+     '    - usage example for initial release notes\n',
+     '    - bugfixes for RNH\n',
+     '    - initial release notes handler\n',
+     '\n',
+     '### 0.0.1\n',
+     '\n',
+     '    - initial version of example_module\n']
```


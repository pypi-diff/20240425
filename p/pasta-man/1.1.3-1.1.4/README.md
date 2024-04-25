# Comparing `tmp/pasta_man-1.1.3.tar.gz` & `tmp/pasta_man-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasta_man-1.1.3.tar", last modified: Wed Apr 24 17:28:22 2024, max compression
+gzip compressed data, was "pasta_man-1.1.4.tar", last modified: Thu Apr 25 12:59:01 2024, max compression
```

## Comparing `pasta_man-1.1.3.tar` & `pasta_man-1.1.4.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:28:22.109753 pasta_man-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-24 17:28:15.000000 pasta_man-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-24 17:28:22.109753 pasta_man-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10181 2024-04-24 17:28:15.000000 pasta_man-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-24 17:28:15.000000 pasta_man-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)    10181 2024-04-24 17:28:15.000000 pasta_man-1.1.3/readmeforpypi.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 17:28:22.109753 pasta_man-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:28:22.105753 pasta_man-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:28:22.105753 pasta_man-1.1.3/src/pasta_man/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:28:22.109753 pasta_man-1.1.3/src/pasta_man/architectures/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11652 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/architectures/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)    12341 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/architectures/targets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/architectures/terminal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6109 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/pasta_man.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:28:22.109753 pasta_man-1.1.3/src/pasta_man/self_launch_thread/
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/self_launch_thread/Launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/self_launch_thread/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:28:22.109753 pasta_man-1.1.3/src/pasta_man/utilities/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:28:22.109753 pasta_man-1.1.3/src/pasta_man/utilities/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/utilities/Exceptions/TerminalExceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/utilities/Exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/utilities/Exceptions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/utilities/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/utilities/helptext.py
--rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/utilities/pasta_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/utilities/pasta_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/utilities/retransform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:28:22.109753 pasta_man-1.1.3/src/pasta_man.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-24 17:28:22.000000 pasta_man-1.1.3/src/pasta_man.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-24 17:28:22.000000 pasta_man-1.1.3/src/pasta_man.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 17:28:22.000000 pasta_man-1.1.3/src/pasta_man.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-24 17:28:22.000000 pasta_man-1.1.3/src/pasta_man.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-24 17:28:22.000000 pasta_man-1.1.3/src/pasta_man.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 17:28:22.000000 pasta_man-1.1.3/src/pasta_man.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:01.906044 pasta_man-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-25 12:58:56.000000 pasta_man-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-04-25 12:59:01.906044 pasta_man-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-04-25 12:58:56.000000 pasta_man-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-25 12:58:56.000000 pasta_man-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-04-25 12:58:56.000000 pasta_man-1.1.4/readmeforpypi.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 12:59:01.906044 pasta_man-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:01.898043 pasta_man-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:01.902044 pasta_man-1.1.4/src/pasta_man/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-25 12:58:56.000000 pasta_man-1.1.4/src/pasta_man/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-25 12:58:56.000000 pasta_man-1.1.4/src/pasta_man/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:01.902044 pasta_man-1.1.4/src/pasta_man/architectures/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 12:58:56.000000 pasta_man-1.1.4/src/pasta_man/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11652 2024-04-25 12:58:56.000000 pasta_man-1.1.4/src/pasta_man/architectures/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12341 2024-04-25 12:58:56.000000 pasta_man-1.1.4/src/pasta_man/architectures/targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-25 12:58:56.000000 pasta_man-1.1.4/src/pasta_man/architectures/terminal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6109 2024-04-25 12:58:56.000000 pasta_man-1.1.4/src/pasta_man/pasta_man.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:01.902044 pasta_man-1.1.4/src/pasta_man/self_launch_thread/
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-25 12:58:56.000000 pasta_man-1.1.4/src/pasta_man/self_launch_thread/Launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 12:58:56.000000 pasta_man-1.1.4/src/pasta_man/self_launch_thread/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:01.902044 pasta_man-1.1.4/src/pasta_man/utilities/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:01.902044 pasta_man-1.1.4/src/pasta_man/utilities/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-25 12:58:56.000000 pasta_man-1.1.4/src/pasta_man/utilities/Exceptions/TerminalExceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 12:58:56.000000 pasta_man-1.1.4/src/pasta_man/utilities/Exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-25 12:58:56.000000 pasta_man-1.1.4/src/pasta_man/utilities/Exceptions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 12:58:56.000000 pasta_man-1.1.4/src/pasta_man/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-25 12:58:56.000000 pasta_man-1.1.4/src/pasta_man/utilities/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-25 12:58:56.000000 pasta_man-1.1.4/src/pasta_man/utilities/helptext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-04-25 12:58:56.000000 pasta_man-1.1.4/src/pasta_man/utilities/pasta_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-04-25 12:58:56.000000 pasta_man-1.1.4/src/pasta_man/utilities/pasta_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-25 12:58:56.000000 pasta_man-1.1.4/src/pasta_man/utilities/retransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-25 12:58:56.000000 pasta_man-1.1.4/src/pasta_man/utilities/upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:59:01.906044 pasta_man-1.1.4/src/pasta_man.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-04-25 12:59:01.000000 pasta_man-1.1.4/src/pasta_man.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-25 12:59:01.000000 pasta_man-1.1.4/src/pasta_man.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:59:01.000000 pasta_man-1.1.4/src/pasta_man.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-25 12:59:01.000000 pasta_man-1.1.4/src/pasta_man.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-25 12:59:01.000000 pasta_man-1.1.4/src/pasta_man.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 12:59:01.000000 pasta_man-1.1.4/src/pasta_man.egg-info/top_level.txt
```

### Comparing `pasta_man-1.1.3/LICENSE` & `pasta_man-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.3/PKG-INFO` & `pasta_man-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta-man
-Version: 1.1.3
+Version: 1.1.4
 Summary: Password Manager
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>, Sairam Pimple <sairampimple003@gmail.com>, Shubham Narendra Singh <shubh1122000@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -47,14 +47,15 @@
 Requires-Dist: colorama
 Requires-Dist: tk
 Requires-Dist: optioner>=1.5.2
 Requires-Dist: pyperclip
 Requires-Dist: ttkthemes
 Requires-Dist: pyinstaller
 Requires-Dist: wrapper-bar>=0.1.4
+Requires-Dist: requests
 
 # Overview
 
 Pasta-Man is a software application designed to securely store passwords and sensitive information in an encrypted format. It provides users with a convenient way to manage their passwords, ensuring they are protected from unauthorized access.
 
 ## Project Badges
 
@@ -221,29 +222,30 @@
 - Win XP
 - Yaru
 
 ## Dependencies
 
 - Python>=3.9
 - pandas
+- requests
 - tk
 - ttkthemes
 - colorama
 - wrapper-bar>=0.1.4
 - pyperclip
 - optioner>=1.5.2
 - cryptography
 - pyinstaller
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.1.3
+pip install pasta-man==1.1.4
 ```
 
 ## README before [#Usage](#usage)
 
 After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man>=1.0.4` -> `pasta-man` and `pasta-man-launcher`.
 
 - `pasta-man` Command
@@ -271,15 +273,15 @@
     ...
     ```
 
 - To show full list of CLI commands supported by `pasta-man`, in terminal/CMD, run:
 
     ```bash
     $ pasta-man -h # or pasta-man --help
-    Pasta Man v1.1.3
+    Pasta Man v1.1.4
     helptext
       |  -h or --help                     : show this help and exit.
       |  -v or --version                  : show version and exit.
       |  -p or --path                     : show install path and exit.
       |  -rmc or --remove-configurations  : remove existing configs. [Warning] This is irreversible.
       |  -dwl or --doc-w-list             : list all modules of pasta-man. Enter the full-module-name for docstring.
       |  -i or --import                   : import a passwords file. Only files exported by pasta-man can be imported.
```

### Comparing `pasta_man-1.1.3/README.md` & `pasta_man-1.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -167,29 +167,30 @@
 - Win XP
 - Yaru
 
 ## Dependencies
 
 - Python>=3.9
 - pandas
+- requests
 - tk
 - ttkthemes
 - colorama
 - wrapper-bar>=0.1.4
 - pyperclip
 - optioner>=1.5.2
 - cryptography
 - pyinstaller
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.1.3
+pip install pasta-man==1.1.4
 ```
 
 ## README before [#Usage](#usage)
 
 After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man>=1.0.4` -> `pasta-man` and `pasta-man-launcher`.
 
 - `pasta-man` Command
@@ -217,15 +218,15 @@
     ...
     ```
 
 - To show full list of CLI commands supported by `pasta-man`, in terminal/CMD, run:
 
     ```bash
     $ pasta-man -h # or pasta-man --help
-    Pasta Man v1.1.3
+    Pasta Man v1.1.4
     helptext
       |  -h or --help                     : show this help and exit.
       |  -v or --version                  : show version and exit.
       |  -p or --path                     : show install path and exit.
       |  -rmc or --remove-configurations  : remove existing configs. [Warning] This is irreversible.
       |  -dwl or --doc-w-list             : list all modules of pasta-man. Enter the full-module-name for docstring.
       |  -i or --import                   : import a passwords file. Only files exported by pasta-man can be imported.
```

### Comparing `pasta_man-1.1.3/pyproject.toml` & `pasta_man-1.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pasta-man"
-version = "1.1.3"
+version = "1.1.4"
 description = "Password Manager"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Software Development",
     "Topic :: Security",
     "Programming Language :: Python :: 3.10",
@@ -25,15 +25,15 @@
     {name = "Soumyo Deep Gupta", email = "deep.main.ac@gmail.com"},
     {name = "Sairam Pimple", email = "sairampimple003@gmail.com"},
     {name = "Shubham Narendra Singh", email = "shubh1122000@gmail.com"}
 ]
 maintainers = [
     {name = "Soumyo Deep Gupta", email = "deep.main.ac@gmail.com"}
 ]
-dependencies = ['cryptography', 'pandas', 'colorama', 'tk', 'optioner>=1.5.2', 'pyperclip', 'ttkthemes', 'pyinstaller', 'wrapper-bar>=0.1.4']
+dependencies = ['cryptography', 'pandas', 'colorama', 'tk', 'optioner>=1.5.2', 'pyperclip', 'ttkthemes', 'pyinstaller', 'wrapper-bar>=0.1.4', 'requests']
 
 [project.scripts]
 pasta-man-launcher = "pasta_man.pasta_man:main"
 pasta-man = "pasta_man.self_launch_thread.Launcher:main"
 
 [project.urls]
 GitHub = 'https://github.com/d33pster/pasta-man'
```

### Comparing `pasta_man-1.1.3/readmeforpypi.md` & `pasta_man-1.1.4/readmeforpypi.md`

 * *Files 1% similar despite different names*

```diff
@@ -167,29 +167,30 @@
 - Win XP
 - Yaru
 
 ## Dependencies
 
 - Python>=3.9
 - pandas
+- requests
 - tk
 - ttkthemes
 - colorama
 - wrapper-bar>=0.1.4
 - pyperclip
 - optioner>=1.5.2
 - cryptography
 - pyinstaller
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.1.3
+pip install pasta-man==1.1.4
 ```
 
 ## README before [#Usage](#usage)
 
 After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man>=1.0.4` -> `pasta-man` and `pasta-man-launcher`.
 
 - `pasta-man` Command
@@ -217,15 +218,15 @@
     ...
     ```
 
 - To show full list of CLI commands supported by `pasta-man`, in terminal/CMD, run:
 
     ```bash
     $ pasta-man -h # or pasta-man --help
-    Pasta Man v1.1.3
+    Pasta Man v1.1.4
     helptext
       |  -h or --help                     : show this help and exit.
       |  -v or --version                  : show version and exit.
       |  -p or --path                     : show install path and exit.
       |  -rmc or --remove-configurations  : remove existing configs. [Warning] This is irreversible.
       |  -dwl or --doc-w-list             : list all modules of pasta-man. Enter the full-module-name for docstring.
       |  -i or --import                   : import a passwords file. Only files exported by pasta-man can be imported.
```

### Comparing `pasta_man-1.1.3/src/pasta_man/architectures/gui.py` & `pasta_man-1.1.4/src/pasta_man/architectures/gui.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.3/src/pasta_man/architectures/targets.py` & `pasta_man-1.1.4/src/pasta_man/architectures/targets.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.3/src/pasta_man/architectures/terminal.py` & `pasta_man-1.1.4/src/pasta_man/architectures/terminal.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,39 +11,72 @@
 from os.path import dirname, abspath, isdir, join as jPath, splitext, isfile
 from os import system as run, getcwd as pwd
 from pathlib import Path
 from optioner import options
 from colorama import Fore as f
 from shutil import rmtree
 from wrapper_bar.wrapper import Wrapper
-import sys, platform, threading, pyperclip
+import sys, platform, threading, requests
 from getpass import getpass
 
 class Terminal:
     def __init__(self, __version__:str, globalArgs: list[str], masterpassword: bytes) -> None:
+        self.__version = __version__
         self.__masterpassword = masterpassword
         self.__argv = globalArgs
-        self.__shortargs = ['h', 'v', 'p', 'rmc', 'dwl', 'i', 'e', 's']
-        self.__longargs = ['help', 'version', 'path', 'remove-configurations', 'doc-w-list', 'import', 'export', 'search']
+        self.__shortargs = ['h', 'v', 'p', 'rmc', 'dwl', 'i', 'e', 's', 'upg', 'upd']
+        self.__longargs = ['help', 'version', 'path', 'remove-configurations', 'doc-w-list', 'import', 'export', 'search', 'upgrade', 'update']
         self.__mutex = [
             ['help', 'h'],self.__remFromOriginal(['help', 'h']),
             ['v', 'version'], self.__remFromOriginal(['v', 'version']),
             ['p', 'path'], self.__remFromOriginal(['p', 'path']),
             ['rmc', 'remove-configurations'], self.__remFromOriginal(['rmc', 'remove-configurations']),
             ['dwl', 'doc-w-list'], self.__remFromOriginal(['dwl', 'doc-w-list']),
             ['i', 'import'], self.__remFromOriginal(['i', 'import']),
             ['e', 'export'], self.__remFromOriginal(['export', 'e']),
-            ['s', 'search'], self.__remFromOriginal(['s', 'search'])
+            ['s', 'search'], self.__remFromOriginal(['s', 'search']),
+            ['upg', 'upgrade'], self.__remFromOriginal(['upg', 'upgrade']),
+            ['upd', 'update'], self.__remFromOriginal(['upd', 'update'])
         ]
-
+        
         self.__analyze()
+        
+        if '-upd' in self.arguments or '--update' in self.arguments or '-upg' in self.arguments or '--upgrade' in self.arguments:
+            pass
+        else:
+            self.__updateCheck()
+        
         self.__help(__version__)
         self.__readOnlyArgs(__version__)
         self.__permanentEffectArgs()
-        
+    
+    @property
+    def version(self):
+        return self.__version
+    
+    def __updateCheck(self):
+        print(f"{f.BLUE}running *auto-update-check*{f.RESET}", end="\r")
+        if requests.get('https://google.com').status_code == 200:
+            from pasta_man.utilities.upgrade import VersionCheck
+            vc = VersionCheck()
+            vc.action = 'update'
+            available_update = vc.actionversion
+            
+            vc.action = 'upgrade'
+            available_upgrade = vc.actionversion
+            
+            print("                                                                    ", end='\r') # clear buffer
+            # if update/upgrade available, it wont be none
+            if available_update!=None and available_update!='0' and available_update!=0:
+                print(f"\n{f.RED}pasta-man can be updated{f.RESET} {self.version} -> {available_update}")
+            if available_upgrade!=None:
+                print(f"{f.GREEN}pasta-man can be upgraded{f.RESET} {self.version} -> {available_upgrade}\n")
+        else:
+            pass
+    
     def __remFromOriginal(self, excpt: list[str]) -> list[str]:
         self.ORIGINAL = self.__shortargs + self.__longargs
         withoutExcept: list[str] = []
         for x in self.ORIGINAL:
             if x in excpt:
                 continue
             else:
@@ -219,10 +252,20 @@
                 p, ext = splitext(path)
                 target = targets(masterpassword=self.__masterpassword)
                 t1 = threading.Thread(target=target.init)
                 t1.start()
                 t1.join()
                 threading.Thread(target=target.importer, args=(ext, path)).start()
             
-            
+        elif '-upd' in self.arguments or '--update' in self.arguments:
+            from pasta_man.utilities.upgrade import Update
+            upd = Update()
+            if upd.connectivity:
+                upd.update()
+                if upd.status:
+                    print(f"{f.BLUE}Update complete.{f.RESET}")
+                else:
+                    print(f"{f.RED}Update InComplete{f.RESET}")
+            else:
+                print(f"{f.RED}No Internet Connection Detected.{f.RESET}")
         else:
             pass
```

### Comparing `pasta_man-1.1.3/src/pasta_man/pasta_man.py` & `pasta_man-1.1.4/src/pasta_man/pasta_man.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 Working:
     - catch and analyse arguments if any. If Found, execute it. Else Move on.
     - Check for master password
     - If found, decrypt it and call pmanager class. If not found, ask the user for master password, encrypt and save it and then call pmanager class.
 """
 
 # version info
-__version__ = "1.1.3"
+__version__ = "1.1.4"
 
 # import internal modules
 from pathlib import Path
 from os.path import join as jPath, exists as there, dirname, abspath
 from os import makedirs
 from shutil import rmtree
 import sys, threading
```

### Comparing `pasta_man-1.1.3/src/pasta_man/self_launch_thread/Launcher.py` & `pasta_man-1.1.4/src/pasta_man/self_launch_thread/Launcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,42 +56,16 @@
         makedirs(jPath(str(Path.home()), '.pastaman'))
     
     if not there(jPath(str(Path.home()), '.pastaman', '.log')):
         with open(jPath(str(Path.home()), '.pastaman', '.log'), 'w') as logfile:
             logfile.write("log file init")
 
 def makePasta():
-    batdat = """
-@REM turn printing of commands off
-@echo off
-
-@REM install using pyinstaller.
-pyinstaller --onefile --noconsole pasta_man.py > NUL
-
-@REM After this delete .spec file and build folder tree.
-del build /s /q
-del pasta_man.spec
-
-@REM copy dist/pasta_man.exe to %USERPROFILE%\.pastaman\pasta-man.exe
-copy dist\pasta_man.exe %USERPROFILE%\.pastaman\pasta-man.exe
-
-@REM delete dist
-del dist /s /q
-
-@REM create vbs script
-cd %USERPROFILE%\.pastaman
-echo Set pastaShell = WScript.CreateObject('WScript.Shell') > pasta-man.vbs
-echo pastaShell.Run "%USERPROFILE%\.pastaman\pasta-man.exe", 0, False >> pasta-man.vbs
-
-@REM copy it 
-"""
     directory = dirname(dirname(abspath(__file__))) # pasta_man directory
     chdir(directory)
-    print(f'{f.RED}(one-time-setup){f.RESET}')
-    print('Operating System: Windows\nsetting up pasta-man...\nThis might take a while.')
     
     wrap = Wrapper()
     
     codes = [
         f"""subprocess.Popen(['pyinstaller', '--onefile', '--noconsole', 'pasta_man.py'], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()""",
     ]
     
@@ -127,14 +101,16 @@
         """from pathlib import Path""",
         """from os.path import join"""
     ]
     
     wrap.pyShellWrapper(codes, dependencies, delay=0.01, width=60, label="Garnishing:")
     
     print(f"{f.LIGHTGREEN_EX}Serving...{f.RESET}")
+
+
 def main():
     color()
     checklogfile()
     # check for arguments
     if len(sys.argv[1:])>0:
         sys.argv[0] += sys.argv[0]+'-launcher'
         command = basename(sys.argv[0])
@@ -146,12 +122,14 @@
         sys.exit(0)
     
     # if no arguments run these
     system = os()
     if system=='Darwin' or system=='Linux':
         run('nohup pasta-man-launcher > ~/.pastaman/.log &')
     elif system=='Windows':
-        if not there(jPath(str(Path.home()), '.pastaman', 'pasta-man.vbs')):
+        if (not there(jPath(str(Path.home()), '.pastaman', 'pasta-man.exe'))) or (not there(jPath(str(Path.home()), '.pastaman', 'pasta-man.vbs'))):
+            print(f'{f.RED}(one-time-setup){f.RESET}')
+            print('Operating System: Windows\nsetting up pasta-man...\nThis might take a while.')
             makePasta()
         chdir(jPath(str(Path.home()), '.pastaman'))
         run(f"start /B wscript.exe {jPath(str(Path.home()), '.pastaman', 'pasta-man.vbs')}")
     sys.exit(0)
```

### Comparing `pasta_man-1.1.3/src/pasta_man/utilities/Exceptions/exceptions.py` & `pasta_man-1.1.4/src/pasta_man/utilities/Exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.3/src/pasta_man/utilities/encryption.py` & `pasta_man-1.1.4/src/pasta_man/utilities/encryption.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.3/src/pasta_man/utilities/helptext.py` & `pasta_man-1.1.4/src/pasta_man/utilities/helptext.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.3/src/pasta_man/utilities/pasta_docs.py` & `pasta_man-1.1.4/src/pasta_man/utilities/pasta_docs.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.3/src/pasta_man/utilities/pasta_menu.py` & `pasta_man-1.1.4/src/pasta_man/utilities/pasta_menu.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.3/src/pasta_man/utilities/retransform.py` & `pasta_man-1.1.4/src/pasta_man/utilities/retransform.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.3/src/pasta_man.egg-info/PKG-INFO` & `pasta_man-1.1.4/src/pasta_man.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta-man
-Version: 1.1.3
+Version: 1.1.4
 Summary: Password Manager
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>, Sairam Pimple <sairampimple003@gmail.com>, Shubham Narendra Singh <shubh1122000@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -47,14 +47,15 @@
 Requires-Dist: colorama
 Requires-Dist: tk
 Requires-Dist: optioner>=1.5.2
 Requires-Dist: pyperclip
 Requires-Dist: ttkthemes
 Requires-Dist: pyinstaller
 Requires-Dist: wrapper-bar>=0.1.4
+Requires-Dist: requests
 
 # Overview
 
 Pasta-Man is a software application designed to securely store passwords and sensitive information in an encrypted format. It provides users with a convenient way to manage their passwords, ensuring they are protected from unauthorized access.
 
 ## Project Badges
 
@@ -221,29 +222,30 @@
 - Win XP
 - Yaru
 
 ## Dependencies
 
 - Python>=3.9
 - pandas
+- requests
 - tk
 - ttkthemes
 - colorama
 - wrapper-bar>=0.1.4
 - pyperclip
 - optioner>=1.5.2
 - cryptography
 - pyinstaller
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.1.3
+pip install pasta-man==1.1.4
 ```
 
 ## README before [#Usage](#usage)
 
 After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man>=1.0.4` -> `pasta-man` and `pasta-man-launcher`.
 
 - `pasta-man` Command
@@ -271,15 +273,15 @@
     ...
     ```
 
 - To show full list of CLI commands supported by `pasta-man`, in terminal/CMD, run:
 
     ```bash
     $ pasta-man -h # or pasta-man --help
-    Pasta Man v1.1.3
+    Pasta Man v1.1.4
     helptext
       |  -h or --help                     : show this help and exit.
       |  -v or --version                  : show version and exit.
       |  -p or --path                     : show install path and exit.
       |  -rmc or --remove-configurations  : remove existing configs. [Warning] This is irreversible.
       |  -dwl or --doc-w-list             : list all modules of pasta-man. Enter the full-module-name for docstring.
       |  -i or --import                   : import a passwords file. Only files exported by pasta-man can be imported.
```

### Comparing `pasta_man-1.1.3/src/pasta_man.egg-info/SOURCES.txt` & `pasta_man-1.1.4/src/pasta_man.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,10 +19,11 @@
 src/pasta_man/self_launch_thread/__init__.py
 src/pasta_man/utilities/__init__.py
 src/pasta_man/utilities/encryption.py
 src/pasta_man/utilities/helptext.py
 src/pasta_man/utilities/pasta_docs.py
 src/pasta_man/utilities/pasta_menu.py
 src/pasta_man/utilities/retransform.py
+src/pasta_man/utilities/upgrade.py
 src/pasta_man/utilities/Exceptions/TerminalExceptions.py
 src/pasta_man/utilities/Exceptions/__init__.py
 src/pasta_man/utilities/Exceptions/exceptions.py
```


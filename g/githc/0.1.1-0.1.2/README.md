# Comparing `tmp/githc-0.1.1.tar.gz` & `tmp/githc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/githc-0.1.1.tar", last modified: Tue Jul  7 22:47:58 2020, max compression
+gzip compressed data, was "githc-0.1.2.tar", last modified: Wed Apr 24 23:51:03 2024, max compression
```

## Comparing `githc-0.1.1.tar` & `githc-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 chrisgravel (723605) primarygroup (89939)        0 2020-07-07 22:47:58.000000 githc-0.1.1/
--rw-r--r--   0 chrisgravel (723605) primarygroup (89939)        5 2020-05-23 02:14:45.000000 githc-0.1.1/MANIFEST.in
--rw-r--r--   0 chrisgravel (723605) primarygroup (89939)      807 2020-07-07 22:47:58.000000 githc-0.1.1/PKG-INFO
--rw-r--r--   0 chrisgravel (723605) primarygroup (89939)     1047 2020-07-07 22:34:25.000000 githc-0.1.1/README.md
--rwxr-xr-x   0 chrisgravel (723605) primarygroup (89939)     4948 2020-07-07 22:31:05.000000 githc-0.1.1/gh.py
-drwxr-xr-x   0 chrisgravel (723605) primarygroup (89939)        0 2020-07-07 22:47:58.000000 githc-0.1.1/githc.egg-info/
--rw-r--r--   0 chrisgravel (723605) primarygroup (89939)      807 2020-07-07 22:47:58.000000 githc-0.1.1/githc.egg-info/PKG-INFO
--rw-r--r--   0 chrisgravel (723605) primarygroup (89939)      194 2020-07-07 22:47:58.000000 githc-0.1.1/githc.egg-info/SOURCES.txt
--rw-r--r--   0 chrisgravel (723605) primarygroup (89939)        1 2020-07-07 22:47:58.000000 githc-0.1.1/githc.egg-info/dependency_links.txt
--rw-r--r--   0 chrisgravel (723605) primarygroup (89939)       32 2020-07-07 22:47:58.000000 githc-0.1.1/githc.egg-info/entry_points.txt
--rw-r--r--   0 chrisgravel (723605) primarygroup (89939)        1 2020-07-07 22:47:58.000000 githc-0.1.1/githc.egg-info/top_level.txt
--rw-r--r--   0 chrisgravel (723605) primarygroup (89939)       79 2020-07-07 22:47:58.000000 githc-0.1.1/setup.cfg
--rw-r--r--   0 chrisgravel (723605) primarygroup (89939)      992 2020-07-07 22:35:49.000000 githc-0.1.1/setup.py
+drwxr-xr-x   0 chris.gravel   (502) staff       (20)        0 2024-04-24 23:51:03.404995 githc-0.1.2/
+-rw-r--r--   0 chris.gravel   (502) staff       (20)     1055 2024-04-24 22:19:20.000000 githc-0.1.2/LICENSE.md
+-rw-r--r--   0 chris.gravel   (502) staff       (20)        5 2024-04-24 22:19:20.000000 githc-0.1.2/MANIFEST.in
+-rw-r--r--   0 chris.gravel   (502) staff       (20)      793 2024-04-24 23:51:03.404733 githc-0.1.2/PKG-INFO
+-rw-r--r--   0 chris.gravel   (502) staff       (20)     1047 2024-04-24 22:19:20.000000 githc-0.1.2/README.md
+-rwxr-xr-x   0 chris.gravel   (502) staff       (20)     5059 2024-04-24 23:44:17.000000 githc-0.1.2/gh.py
+drwxr-xr-x   0 chris.gravel   (502) staff       (20)        0 2024-04-24 23:51:03.403977 githc-0.1.2/githc.egg-info/
+-rw-r--r--   0 chris.gravel   (502) staff       (20)      793 2024-04-24 23:51:03.000000 githc-0.1.2/githc.egg-info/PKG-INFO
+-rw-r--r--   0 chris.gravel   (502) staff       (20)      205 2024-04-24 23:51:03.000000 githc-0.1.2/githc.egg-info/SOURCES.txt
+-rw-r--r--   0 chris.gravel   (502) staff       (20)        1 2024-04-24 23:51:03.000000 githc-0.1.2/githc.egg-info/dependency_links.txt
+-rw-r--r--   0 chris.gravel   (502) staff       (20)       31 2024-04-24 23:51:03.000000 githc-0.1.2/githc.egg-info/entry_points.txt
+-rw-r--r--   0 chris.gravel   (502) staff       (20)        1 2024-04-24 23:51:03.000000 githc-0.1.2/githc.egg-info/top_level.txt
+-rw-r--r--   0 chris.gravel   (502) staff       (20)       79 2024-04-24 23:51:03.405474 githc-0.1.2/setup.cfg
+-rw-r--r--   0 chris.gravel   (502) staff       (20)      949 2024-04-24 23:45:46.000000 githc-0.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `githc-0.1.1/PKG-INFO` & `githc-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: githc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Git history checkout tool
 Home-page: https://github.com/cpagravel/gh
+Download-URL: https://github.com/cpagravel/gh/archive/0.1.2.tar.gz
 Author: Chris Gravel
 Author-email: cpagravel@gmail.com
 License: MIT
-Download-URL: https://github.com/cpagravel/gh/archive/0.1.1.tar.gz
-Description: UNKNOWN
 Keywords: git,git history,git checkout,git workflow
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+License-File: LICENSE.md
```

### Comparing `githc-0.1.1/README.md` & `githc-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `githc-0.1.1/gh.py` & `githc-0.1.2/gh.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,145 +1,175 @@
 #! /usr/bin/env python3
 # Lint as: python3
 
 import argparse
-from collections import OrderedDict
 import logging
-import os
 import re
 import subprocess
 import sys
 
-from typing import Callable, List, Union
+from typing import Callable
 
 ITEMS_TO_SHOW = 10
 DEBUG = False
 
 LOGGER = logging.getLogger(__name__)
 sh = logging.StreamHandler(sys.stdout)
 LOGGER.addHandler(sh)
 LOGGER.setLevel(logging.INFO)
 LOGGER.propagate = False
 
+
 # credit: https://stackoverflow.com/questions/3305287/python-how-do-you-view-output-that-doesnt-fit-the-screen
 # slight modification
 class Less(object):
-    def __init__(self, num_lines: int=40):
-        self.num_lines = num_lines
-    def __ror__(self, msg: str):
-        if (len(msg.split("\n")) <= self.num_lines):
-            LOGGER.info(msg)
-        else:
-            with subprocess.Popen(["less", "-R"], stdin=subprocess.PIPE) as less:
-                try:
-                    less.stdin.write(msg.encode("utf-8"))
-                    less.stdin.close()
-                    less.wait()
-                except KeyboardInterrupt:
-                    less.kill()
-                    bash("stty echo")
+  def __init__(self, num_lines: int = 40):
+    self.num_lines = num_lines
+
+  def __ror__(self, msg: str):
+    if (len(msg.split("\n")) <= self.num_lines):
+      LOGGER.info(msg)
+    else:
+      with subprocess.Popen(["less", "-R"], stdin=subprocess.PIPE) as less:
+        try:
+          less.stdin.write(msg.encode("utf-8"))
+          less.stdin.close()
+          less.wait()
+        except KeyboardInterrupt:
+          less.kill()
+          bash("stty echo")
 
 
 class Colors(object):
-    BLUE        = "\033[1;34m"
-    BOLD        = "\033[;1m"
-    CYAN        = "\033[1;36m"
-    GREEN       = "\033[1;32m"
-    OFF         = "\033[1;;m"
-    PURPLE      = "\033[1;35m"
-    RED         = "\033[1;31m"
-    RESET       = "\033[0;0m"
-    REVERSE     = "\033[;7m"
-    WHITE       = "\033[1;37m"
-    YELLOW      = "\033[1;33m"
-
-    @staticmethod
-    def colorize(text, color):
-        return color + str(text) + Colors.OFF
-
-def bash(command: Union[List[str], str]):
-    if ("list" in str(type(command))):
-        command_array = [cmd.replace('"', '') for cmd in command]
-    else:
-        command_array = command.split()
-    LOGGER.debug("Bash: %s", " ".join(command_array))
-    proc = subprocess.Popen(command_array, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=False)
-    (output, err) = proc.communicate()
-    return (output, err)
-
-def generateHistoryList() -> List[str]:
-    (output, err) = bash("git reflog show")
-    if (len(err) != 0):
-        raise RuntimeError(err.decode("utf-8"))
-    output = [line for line in output.decode().split("\n") if "checkout:" in line]
-    checkout_targets = re.findall(r"checkout: moving from ([^ ]+) to (?:[^ ]+)", "\n".join(output))
-    (current_branch, _) = bash("git rev-parse --abbrev-ref HEAD")
-    current_branch = current_branch.decode().strip()
-
-    checkout_set = OrderedDict()
-    checkout_set[current_branch] = 1
-    for target in checkout_targets:
-        checkout_set[target] = 1
-    return list(checkout_set.keys())
-
-def displayList(checkout_history, verbose=False):
-    header = Colors.colorize("#   BRANCH HISTORY", Colors.YELLOW)
-    LOGGER.info(header)
-    for (index, branch) in enumerate(checkout_history):
-        if not verbose and index > ITEMS_TO_SHOW:
-            break
-        index = Colors.colorize(index, Colors.PURPLE)
-        branch = Colors.colorize(branch, Colors.GREEN)
-        LOGGER.info("{:<16} {:<21} ({})".format(index, branch, index))
-
-def checkValidRef(item_count: int) -> Callable[[Union[str, int]], int]:
-    def _checkValidRef(ref: Union[str, int]) -> int:
-        ref = int(ref)
-        if ref < 0:
-            raise argparse.ArgumentTypeError("%s is an invalid positive int value" % ref)
-        elif ref > item_count:
-            raise argparse.ArgumentTypeError("%s is an out of range" % ref)
-        return ref
-    return _checkValidRef
+  BLUE = "\033[1;34m"
+  BOLD = "\033[;1m"
+  CYAN = "\033[1;36m"
+  GREEN = "\033[1;32m"
+  OFF = "\033[1;;m"
+  PURPLE = "\033[1;35m"
+  RED = "\033[1;31m"
+  RESET = "\033[0;0m"
+  REVERSE = "\033[;7m"
+  WHITE = "\033[1;37m"
+  YELLOW = "\033[1;33m"
+
+  @staticmethod
+  def colorize(text, color):
+    return color + str(text) + Colors.OFF
+
+
+def bash(command: list[str] | str):
+  if ("list" in str(type(command))):
+    command_array = [cmd.replace('"', '') for cmd in command]
+  else:
+    command_array = command.split()
+  LOGGER.debug("Bash: %s", " ".join(command_array))
+  proc = subprocess.Popen(
+      command_array, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=False)
+  (output, err) = proc.communicate()
+  return (output, err)
+
+
+def get_reflog_list() -> list[str]:
+  (output, err) = bash("git reflog show")
+  if (len(err) != 0):
+    raise RuntimeError(err.decode("utf-8"))
+  output = [line for line in output.decode().split("\n") if "checkout:" in line]
+  checkout_targets = re.findall(r"checkout: moving from ([^ ]+) to (?:[^ ]+)", "\n".join(output))
+  (current_branch, _) = bash("git rev-parse --abbrev-ref HEAD")
+  current_branch = current_branch.decode().strip()
+
+  checkout_set = dict()  # dicts in Python 3.7+ are ordered
+  checkout_set[current_branch] = 1
+  for target in checkout_targets:
+    checkout_set[target] = 1
+  return list(checkout_set.keys())
+
+
+def get_branch_list() -> list[str]:
+  (output, err) = bash("git branch")
+  if (len(err) != 0):
+    raise RuntimeError(err.decode("utf-8"))
+  return [line[2:].strip() for line in output.decode().split("\n")]
+
+
+def generate_history_list() -> list[str]:
+  reflog_list = get_reflog_list()
+  branch_set = set(get_branch_list())
+  print(reflog_list)
+  print(branch_set)
+  # Filter out branches that have been deleted
+  return [branch for branch in reflog_list if branch in branch_set]
+
+
+def display_list(checkout_history, verbose=False):
+  header = Colors.colorize("#   BRANCH HISTORY", Colors.YELLOW)
+  LOGGER.info(header)
+  for (index, branch) in enumerate(checkout_history):
+    if not verbose and index > ITEMS_TO_SHOW:
+      break
+    index = Colors.colorize(index, Colors.PURPLE)
+    branch = Colors.colorize(branch, Colors.GREEN)
+    LOGGER.info("{:<16} {:<21} ({})".format(index, branch, index))
+
+
+def check_valid_ref(item_count: int) -> Callable[[str | int], int]:
+  def _check_valid_ref(ref: str | int) -> int:
+    ref = int(ref)
+    if ref < 0:
+      raise argparse.ArgumentTypeError("%s is an invalid positive int value" % ref)
+    elif ref > item_count:
+      raise argparse.ArgumentTypeError("%s is an out of range" % ref)
+    return ref
+
+  return _check_valid_ref
+
 
 def main():
-    try:
-        checkout_history = generateHistoryList()
-    except RuntimeError as e:
-        LOGGER.info(e)
-        exit(1)
-    checkout_history.pop(0)  # Pop the branch that we"re currently on
-    item_count = len(checkout_history)
-
-    parser = argparse.ArgumentParser()
-
-    parser.add_argument(
-        "-v", "--verbose", action="store_true", help="show all branch references in history")
-    parser.add_argument("--debug", action="store_true", help="show bash commands")
-
-    group = parser.add_mutually_exclusive_group()
-    group.add_argument(
-        "REF", metavar="REF_INT", type=checkValidRef(item_count), nargs="?",
-        help="Output the branch reference in checkout history")
-    group.add_argument(
-        "-c", type=checkValidRef(item_count), metavar="REF_INT",
-        dest="checkout", help=("eq to " + Colors.colorize("git checkout ", Colors.GREEN)
-        + Colors.colorize("<BRANCH_REF>", Colors.RED)))
-
-    args = parser.parse_args()
-
-    if args.debug:
-        LOGGER.setLevel(logging.DEBUG)
-
-    if args.REF is not None:  # print branch name
-        LOGGER.info(checkout_history[args.REF])
-    elif args.checkout is not None:  # checkout branch
-        command = f"git checkout {checkout_history[args.checkout]}"
-        (output, err) = bash(command)
-        if err:
-            LOGGER.error(err.decode())
-        LOGGER.info(output.decode())
-    else:
-        displayList(checkout_history, args.verbose)
+  try:
+    checkout_history = generate_history_list()
+  except RuntimeError as e:
+    LOGGER.info(e)
+    exit(1)
+  checkout_history.pop(0)  # Pop the branch that we"re currently on
+  item_count = len(checkout_history)
+
+  parser = argparse.ArgumentParser()
+
+  parser.add_argument(
+      "-v", "--verbose", action="store_true", help="show all branch references in history")
+  parser.add_argument("--debug", action="store_true", help="show bash commands")
+
+  group = parser.add_mutually_exclusive_group()
+  group.add_argument(
+      "REF",
+      metavar="REF_INT",
+      type=check_valid_ref(item_count),
+      nargs="?",
+      help="Output the branch reference in checkout history")
+  group.add_argument(
+      "-c",
+      type=check_valid_ref(item_count),
+      metavar="REF_INT",
+      dest="checkout",
+      help=("eq to " + Colors.colorize("git checkout ", Colors.GREEN) + Colors.colorize(
+          "<BRANCH_REF>", Colors.RED)))
+
+  args = parser.parse_args()
+
+  if args.debug:
+    LOGGER.setLevel(logging.DEBUG)
+
+  if args.REF is not None:  # print branch name
+    LOGGER.info(checkout_history[args.REF])
+  elif args.checkout is not None:  # checkout branch
+    command = f"git checkout {checkout_history[args.checkout]}"
+    (output, err) = bash(command)
+    if err:
+      LOGGER.error(err.decode())
+    LOGGER.info(output.decode())
+  else:
+    display_list(checkout_history, args.verbose)
+
 
 if __name__ == "__main__":
-    main()
+  main()
```

### Comparing `githc-0.1.1/githc.egg-info/PKG-INFO` & `githc-0.1.2/githc.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: githc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Git history checkout tool
 Home-page: https://github.com/cpagravel/gh
+Download-URL: https://github.com/cpagravel/gh/archive/0.1.2.tar.gz
 Author: Chris Gravel
 Author-email: cpagravel@gmail.com
 License: MIT
-Download-URL: https://github.com/cpagravel/gh/archive/0.1.1.tar.gz
-Description: UNKNOWN
 Keywords: git,git history,git checkout,git workflow
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+License-File: LICENSE.md
```

### Comparing `githc-0.1.1/setup.py` & `githc-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 import setuptools
 
 setuptools.setup(
-    name = "githc",
-    packages = {".": "githc"},
-    version = "0.1.1",
+    name="githc",
+    packages={".": "githc"},
+    version="0.1.2",
     license="MIT",
-    description = "Git history checkout tool",
-    author = "Chris Gravel",
-    author_email = "cpagravel@gmail.com",
-    url = "https://github.com/cpagravel/gh",
-    download_url = "https://github.com/cpagravel/gh/archive/0.1.1.tar.gz",
-    keywords = ["git", "git history", "git checkout", "git workflow"],
+    description="Git history checkout tool",
+    author="Chris Gravel",
+    author_email="cpagravel@gmail.com",
+    url="https://github.com/cpagravel/gh",
+    download_url="https://github.com/cpagravel/gh/archive/0.1.2.tar.gz",
+    keywords=["git", "git history", "git checkout", "git workflow"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Version Control :: Git",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-  ],
-  entry_points = {
-      'console_scripts': [
-          'gh = gh:main'
-      ]
-  },
-)
+    ],
+    entry_points={'console_scripts': ['gh = gh:main']},
+)
```


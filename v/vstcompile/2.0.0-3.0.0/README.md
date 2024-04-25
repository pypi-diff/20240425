# Comparing `tmp/vstcompile-2.0.0.tar.gz` & `tmp/vstcompile-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstcompile-2.0.0.tar", last modified: Sat Jul 29 04:59:02 2023, max compression
+gzip compressed data, was "vstcompile-3.0.0.tar", last modified: Wed Apr 24 23:59:25 2024, max compression
```

## Comparing `vstcompile-2.0.0.tar` & `vstcompile-3.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 grey      (1000) grey      (1000)        0 2023-07-29 04:59:02.992552 vstcompile-2.0.0/
--rw-rw-r--   0 grey      (1000) grey      (1000)    11344 2023-07-29 03:48:47.000000 vstcompile-2.0.0/LICENSE
--rwxrwxr-x   0 grey      (1000) grey      (1000)       33 2023-07-29 04:06:42.000000 vstcompile-2.0.0/MANIFEST.in
--rw-rw-r--   0 grey      (1000) grey      (1000)      585 2023-07-29 03:48:47.000000 vstcompile-2.0.0/NOTICE
--rw-rw-r--   0 grey      (1000) grey      (1000)     2815 2023-07-29 04:59:02.992552 vstcompile-2.0.0/PKG-INFO
--rw-rw-r--   0 grey      (1000) grey      (1000)     1472 2023-07-29 04:58:15.000000 vstcompile-2.0.0/README.rst
--rw-rw-r--   0 grey      (1000) grey      (1000)     1698 2023-07-29 04:58:36.000000 vstcompile-2.0.0/pyproject.toml
--rw-rw-r--   0 grey      (1000) grey      (1000)       38 2023-07-29 04:59:02.992552 vstcompile-2.0.0/setup.cfg
--rw-rw-r--   0 grey      (1000) grey      (1000)      200 2023-07-29 04:07:16.000000 vstcompile-2.0.0/setup.py
-drwxrwxr-x   0 grey      (1000) grey      (1000)        0 2023-07-29 04:59:02.992552 vstcompile-2.0.0/vstcompile/
--rw-rw-r--   0 grey      (1000) grey      (1000)    11758 2023-07-29 04:18:29.000000 vstcompile-2.0.0/vstcompile/__init__.py
--rw-rw-r--   0 grey      (1000) grey      (1000)     1590 2023-07-29 04:54:34.000000 vstcompile-2.0.0/vstcompile/github.py
--rw-rw-r--   0 grey      (1000) grey      (1000)      742 2023-07-29 04:16:26.000000 vstcompile-2.0.0/vstcompile/utils.py
-drwxrwxr-x   0 grey      (1000) grey      (1000)        0 2023-07-29 04:59:02.992552 vstcompile-2.0.0/vstcompile.egg-info/
--rw-rw-r--   0 grey      (1000) grey      (1000)     2815 2023-07-29 04:59:02.000000 vstcompile-2.0.0/vstcompile.egg-info/PKG-INFO
--rw-rw-r--   0 grey      (1000) grey      (1000)      327 2023-07-29 04:59:02.000000 vstcompile-2.0.0/vstcompile.egg-info/SOURCES.txt
--rw-rw-r--   0 grey      (1000) grey      (1000)        1 2023-07-29 04:59:02.000000 vstcompile-2.0.0/vstcompile.egg-info/dependency_links.txt
--rw-rw-r--   0 grey      (1000) grey      (1000)        1 2023-07-29 04:59:02.000000 vstcompile-2.0.0/vstcompile.egg-info/not-zip-safe
--rw-rw-r--   0 grey      (1000) grey      (1000)       58 2023-07-29 04:59:02.000000 vstcompile-2.0.0/vstcompile.egg-info/requires.txt
--rw-rw-r--   0 grey      (1000) grey      (1000)       11 2023-07-29 04:59:02.000000 vstcompile-2.0.0/vstcompile.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 23:59:25.048229 vstcompile-3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11344 2024-04-24 23:59:21.000000 vstcompile-3.0.0/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-24 23:59:21.000000 vstcompile-3.0.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      585 2024-04-24 23:59:21.000000 vstcompile-3.0.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     2921 2024-04-24 23:59:25.048229 vstcompile-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1472 2024-04-24 23:59:21.000000 vstcompile-3.0.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1698 2024-04-24 23:59:21.000000 vstcompile-3.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 23:59:25.048229 vstcompile-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      200 2024-04-24 23:59:21.000000 vstcompile-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 23:59:25.046229 vstcompile-3.0.0/vstcompile/
+-rw-rw-rw-   0 root         (0) root         (0)    11753 2024-04-24 23:59:21.000000 vstcompile-3.0.0/vstcompile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2024-04-24 23:59:21.000000 vstcompile-3.0.0/vstcompile/github.py
+-rw-rw-rw-   0 root         (0) root         (0)      742 2024-04-24 23:59:21.000000 vstcompile-3.0.0/vstcompile/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 23:59:25.047229 vstcompile-3.0.0/vstcompile.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2921 2024-04-24 23:59:25.000000 vstcompile-3.0.0/vstcompile.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      327 2024-04-24 23:59:25.000000 vstcompile-3.0.0/vstcompile.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 23:59:25.000000 vstcompile-3.0.0/vstcompile.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 23:59:25.000000 vstcompile-3.0.0/vstcompile.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       58 2024-04-24 23:59:25.000000 vstcompile-3.0.0/vstcompile.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-24 23:59:25.000000 vstcompile-3.0.0/vstcompile.egg-info/top_level.txt
```

### Comparing `vstcompile-2.0.0/LICENSE` & `vstcompile-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vstcompile-2.0.0/NOTICE` & `vstcompile-3.0.0/NOTICE`

 * *Files identical despite different names*

### Comparing `vstcompile-2.0.0/PKG-INFO` & `vstcompile-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstcompile
-Version: 2.0.0
+Version: 3.0.0
 Summary: VST util for easy compile
 Author-email: VST Consulting <sergey.k@vstconsulting.net>
 License: Apache License 2.0
 Project-URL: Home, https://github.com/vstconsulting/vstcompile
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstcompile/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstcompile
 Project-URL: Releases, https://pypi.org/project/vstcompile/#history
@@ -20,18 +20,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: cython
-Provides-Extra: release
 License-File: LICENSE
 License-File: NOTICE
+Provides-Extra: cython
+Requires-Dist: cython>=0.29.36; extra == "cython"
+Provides-Extra: release
+Requires-Dist: githubrelease~=1.5.9; extra == "release"
 
 VST Compile utility
 ===================
 
 Lib for quick formatting `setup.py` in projects. Moved from `vstutils` projects for easyer integration.
 
 Quick start
```

### Comparing `vstcompile-2.0.0/README.rst` & `vstcompile-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `vstcompile-2.0.0/pyproject.toml` & `vstcompile-3.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vstcompile-2.0.0/vstcompile/__init__.py` & `vstcompile-3.0.0/vstcompile/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.0.0'
+__version__ = '3.0.0'
 
 # Compilation block
 ########################################################################################
 import re
 import os
 import sys
 import subprocess
@@ -308,16 +308,16 @@
             'install_lib': install_lib
         })
     if has_sphinx and 'build_sphinx' not in cmdclass:
         cmdclass['build_sphinx'] = BuildDoc
     cmdclass['githubrelease'] = GithubRelease
     opts['cmdclass'] = cmdclass
 
-    webpack_path = os.path.join(os.getcwd(), 'webpack.config.js')
-    if os.path.exists(webpack_path) and is_build and os.environ.get('DONT_YARN', "") != 'true':
+    package_path = os.path.join(os.getcwd(), 'package.json')
+    if os.path.exists(package_path) and is_build and os.environ.get('DONT_YARN', "") != 'true':
         try:
             subprocess.check_call(['yarn', 'install', '--pure-lockfile', '--mutex network'], stdout=sys.stdout, stderr=sys.stderr)
             subprocess.check_call(['yarn', 'devBuild' if is_develop else 'build'], stdout=sys.stdout, stderr=sys.stderr)
         except Exception as err:
             raise errors.CompileError(str(err))
 
     setup(**opts)
```

### Comparing `vstcompile-2.0.0/vstcompile/github.py` & `vstcompile-3.0.0/vstcompile/github.py`

 * *Files identical despite different names*

### Comparing `vstcompile-2.0.0/vstcompile/utils.py` & `vstcompile-3.0.0/vstcompile/utils.py`

 * *Files identical despite different names*

### Comparing `vstcompile-2.0.0/vstcompile.egg-info/PKG-INFO` & `vstcompile-3.0.0/vstcompile.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstcompile
-Version: 2.0.0
+Version: 3.0.0
 Summary: VST util for easy compile
 Author-email: VST Consulting <sergey.k@vstconsulting.net>
 License: Apache License 2.0
 Project-URL: Home, https://github.com/vstconsulting/vstcompile
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstcompile/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstcompile
 Project-URL: Releases, https://pypi.org/project/vstcompile/#history
@@ -20,18 +20,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: cython
-Provides-Extra: release
 License-File: LICENSE
 License-File: NOTICE
+Provides-Extra: cython
+Requires-Dist: cython>=0.29.36; extra == "cython"
+Provides-Extra: release
+Requires-Dist: githubrelease~=1.5.9; extra == "release"
 
 VST Compile utility
 ===================
 
 Lib for quick formatting `setup.py` in projects. Moved from `vstutils` projects for easyer integration.
 
 Quick start
```


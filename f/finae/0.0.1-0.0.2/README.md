# Comparing `tmp/finae-0.0.1.tar.gz` & `tmp/finae-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finae-0.0.1.tar", last modified: Thu Feb  2 08:10:19 2023, max compression
+gzip compressed data, was "finae-0.0.2.tar", last modified: Thu Apr 25 06:46:19 2024, max compression
```

## Comparing `finae-0.0.1.tar` & `finae-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,32 @@
-drwxrwxr-x   0 ningr     (1000) ningr     (1000)        0 2023-02-02 08:10:19.542427 finae-0.0.1/
--rw-rw-r--   0 ningr     (1000) ningr     (1000)        0 2023-02-02 08:06:14.000000 finae-0.0.1/LICENSE.txt
--rw-rw-r--   0 ningr     (1000) ningr     (1000)     1198 2023-02-02 08:10:19.542427 finae-0.0.1/PKG-INFO
--rw-rw-r--   0 ningr     (1000) ningr     (1000)       10 2023-02-02 07:53:22.000000 finae-0.0.1/README.md
--rw-rw-r--   0 ningr     (1000) ningr     (1000)     6132 2023-02-02 08:10:09.000000 finae-0.0.1/pyproject.toml
--rw-rw-r--   0 ningr     (1000) ningr     (1000)       38 2023-02-02 08:10:19.542427 finae-0.0.1/setup.cfg
-drwxrwxr-x   0 ningr     (1000) ningr     (1000)        0 2023-02-02 08:10:19.542427 finae-0.0.1/src/
-drwxrwxr-x   0 ningr     (1000) ningr     (1000)        0 2023-02-02 08:10:19.542427 finae-0.0.1/src/finae/
--rw-rw-r--   0 ningr     (1000) ningr     (1000)      110 2023-02-02 08:03:47.000000 finae-0.0.1/src/finae/__init__.py
-drwxrwxr-x   0 ningr     (1000) ningr     (1000)        0 2023-02-02 08:10:19.542427 finae-0.0.1/src/finae.egg-info/
--rw-rw-r--   0 ningr     (1000) ningr     (1000)     1198 2023-02-02 08:10:19.000000 finae-0.0.1/src/finae.egg-info/PKG-INFO
--rw-rw-r--   0 ningr     (1000) ningr     (1000)      258 2023-02-02 08:10:19.000000 finae-0.0.1/src/finae.egg-info/SOURCES.txt
--rw-rw-r--   0 ningr     (1000) ningr     (1000)        1 2023-02-02 08:10:19.000000 finae-0.0.1/src/finae.egg-info/dependency_links.txt
--rw-rw-r--   0 ningr     (1000) ningr     (1000)       37 2023-02-02 08:10:19.000000 finae-0.0.1/src/finae.egg-info/entry_points.txt
--rw-rw-r--   0 ningr     (1000) ningr     (1000)       50 2023-02-02 08:10:19.000000 finae-0.0.1/src/finae.egg-info/requires.txt
--rw-rw-r--   0 ningr     (1000) ningr     (1000)        6 2023-02-02 08:10:19.000000 finae-0.0.1/src/finae.egg-info/top_level.txt
+drwxrwxr-x   0 ningr     (1000) ningr     (1000)        0 2024-04-25 06:46:19.284681 finae-0.0.2/
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)        0 2023-02-02 08:06:14.000000 finae-0.0.2/LICENSE.txt
+-rw-r--r--   0 ningr     (1000) ningr     (1000)     4741 2024-04-25 06:46:19.284681 finae-0.0.2/PKG-INFO
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)     3384 2024-04-25 06:46:04.000000 finae-0.0.2/README.md
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)     6153 2024-04-25 06:45:28.000000 finae-0.0.2/pyproject.toml
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)       38 2024-04-25 06:46:19.284681 finae-0.0.2/setup.cfg
+drwxrwxr-x   0 ningr     (1000) ningr     (1000)        0 2024-04-25 06:46:19.276681 finae-0.0.2/src/
+drwxrwxr-x   0 ningr     (1000) ningr     (1000)        0 2024-04-25 06:46:19.280681 finae-0.0.2/src/finae/
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)      147 2023-11-24 21:52:22.000000 finae-0.0.2/src/finae/__init__.py
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)       36 2023-02-07 10:05:33.000000 finae-0.0.2/src/finae/__main__.py
+drwxrwxr-x   0 ningr     (1000) ningr     (1000)        0 2024-04-25 06:46:19.280681 finae-0.0.2/src/finae/builtin/
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)       57 2023-11-04 04:40:49.000000 finae-0.0.2/src/finae/builtin/__init__.py
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)      121 2023-12-06 10:29:58.000000 finae-0.0.2/src/finae/builtin/__main__.py
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)     1639 2023-12-07 07:34:25.000000 finae-0.0.2/src/finae/builtin/builtin.py
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)      296 2023-12-06 09:01:44.000000 finae-0.0.2/src/finae/builtin/integer.py
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)     7979 2023-12-11 09:37:30.000000 finae-0.0.2/src/finae/core.py
+drwxrwxr-x   0 ningr     (1000) ningr     (1000)        0 2024-04-25 06:46:19.280681 finae-0.0.2/src/finae/legacy/
+drwxrwxr-x   0 ningr     (1000) ningr     (1000)        0 2024-04-25 06:46:19.284681 finae-0.0.2/src/finae/legacy/example/
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)      311 2023-02-14 06:06:14.000000 finae-0.0.2/src/finae/legacy/example/foo.py
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)       15 2023-04-24 05:50:37.000000 finae-0.0.2/src/finae/legacy/example/simple_math.py
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)      588 2023-02-14 04:47:53.000000 finae-0.0.2/src/finae/legacy/exercise.py
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)     1847 2023-04-24 05:50:34.000000 finae-0.0.2/src/finae/legacy/learn.py
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)     1524 2024-01-23 22:21:34.000000 finae-0.0.2/src/finae/llm.py
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)       97 2023-09-05 04:30:19.000000 finae-0.0.2/src/finae/parser.py
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)       29 2023-12-01 23:51:22.000000 finae-0.0.2/src/finae/tot.py
+drwxrwxr-x   0 ningr     (1000) ningr     (1000)        0 2024-04-25 06:46:19.284681 finae-0.0.2/src/finae.egg-info/
+-rw-r--r--   0 ningr     (1000) ningr     (1000)     4741 2024-04-25 06:46:19.000000 finae-0.0.2/src/finae.egg-info/PKG-INFO
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)      597 2024-04-25 06:46:19.000000 finae-0.0.2/src/finae.egg-info/SOURCES.txt
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)        1 2024-04-25 06:46:19.000000 finae-0.0.2/src/finae.egg-info/dependency_links.txt
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)       37 2024-04-25 06:46:19.000000 finae-0.0.2/src/finae.egg-info/entry_points.txt
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)       76 2024-04-25 06:46:19.000000 finae-0.0.2/src/finae.egg-info/requires.txt
+-rw-rw-r--   0 ningr     (1000) ningr     (1000)        6 2024-04-25 06:46:19.000000 finae-0.0.2/src/finae.egg-info/top_level.txt
```

### Comparing `finae-0.0.1/pyproject.toml` & `finae-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [project]
 # This is the name of your project. The first time you publish this
 # package, this name will be registered for you. It will determine how
 # users can install this project, e.g.:
 #
-# $ pip install sampleproject
+# $ pip install finae
 #
 # And where it will live on PyPI: https://pypi.org/project/sampleproject/
 #
 # There are some restrictions on what makes a valid project name
 # specification here:
 # https://packaging.python.org/specifications/core-metadata/#name
 name = "finae"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.1"  # Required
+version = "0.0.2"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "A simple Python library"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -99,22 +99,24 @@
 # This field lists other packages that your project depends on to run.
 # Any package you put here will be installed by pip when your project is
 # installed, so they must be valid existing projects.
 #
 # For an analysis of this field vs pip's requirements files see:
 # https://packaging.python.org/discussions/install-requires-vs-requirements/
 dependencies = [ # Optional
-  "peppercorn"
+  "langchain",
+  "openai",
+  "ray[default]==2.6.0",
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
-#   $ pip install sampleproject[dev]
+#   $ pip install finae[dev]
 #
 # Similar to `dependencies` above, these must be valid existing
 # projects.
 [project.optional-dependencies] # Optional
 dev = ["check-manifest"]
 test = ["coverage"]
```


# Comparing `tmp/mitosis-0.5.0b1.tar.gz` & `tmp/mitosis-0.5.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitosis-0.5.0b1.tar", last modified: Wed Apr 10 11:59:36 2024, max compression
+gzip compressed data, was "mitosis-0.5.0b2.tar", last modified: Tue Apr 23 04:52:30 2024, max compression
```

## Comparing `mitosis-0.5.0b1.tar` & `mitosis-0.5.0b2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:36.907243 mitosis-0.5.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:36.899242 mitosis-0.5.0b1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:36.899242 mitosis-0.5.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/.github/workflows/main.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-04-10 11:59:36.907243 mitosis-0.5.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14025 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:36.899242 mitosis-0.5.0b1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:36.899242 mitosis-0.5.0b1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:36.903243 mitosis-0.5.0b1/mitosis/
--rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:36.903243 mitosis-0.5.0b1/mitosis/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/bad_return_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/mock_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/mock_paper.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/mock_part1.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/mock_part2.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/pyproject_malformed.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/pyproject_missing.toml
--rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/mitosis/tests/test_pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:59:36.907243 mitosis-0.5.0b1/mitosis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-04-10 11:59:36.000000 mitosis-0.5.0b1/mitosis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-10 11:59:36.000000 mitosis-0.5.0b1/mitosis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:59:36.000000 mitosis-0.5.0b1/mitosis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-10 11:59:36.000000 mitosis-0.5.0b1/mitosis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-10 11:59:36.000000 mitosis-0.5.0b1/mitosis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 11:59:36.000000 mitosis-0.5.0b1/mitosis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-10 11:59:30.000000 mitosis-0.5.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-10 11:59:36.907243 mitosis-0.5.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:30.138217 mitosis-0.5.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:30.126217 mitosis-0.5.0b2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:30.130217 mitosis-0.5.0b2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16118 2024-04-23 04:52:30.138217 mitosis-0.5.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14010 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:30.126217 mitosis-0.5.0b2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:30.130217 mitosis-0.5.0b2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:30.130217 mitosis-0.5.0b2/mitosis/
+-rw-r--r--   0 runner    (1001) docker     (127)    21114 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-23 04:52:30.000000 mitosis-0.5.0b2/mitosis/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:30.134217 mitosis-0.5.0b2/mitosis/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/bad_return_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/mock_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/mock_paper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/mock_part1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/mock_part2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/pyproject_malformed.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/pyproject_missing.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/test_pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:30.134217 mitosis-0.5.0b2/mitosis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16118 2024-04-23 04:52:30.000000 mitosis-0.5.0b2/mitosis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-23 04:52:30.000000 mitosis-0.5.0b2/mitosis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 04:52:30.000000 mitosis-0.5.0b2/mitosis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 04:52:30.000000 mitosis-0.5.0b2/mitosis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-23 04:52:30.000000 mitosis-0.5.0b2/mitosis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 04:52:30.000000 mitosis-0.5.0b2/mitosis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-23 04:52:30.138217 mitosis-0.5.0b2/setup.cfg
```

### Comparing `mitosis-0.5.0b1/.github/workflows/main.yaml` & `mitosis-0.5.0b2/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0b1/.github/workflows/release.yaml` & `mitosis-0.5.0b2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0b1/.gitignore` & `mitosis-0.5.0b2/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 commit-msg
 todo
 .vscode
 trials/
+mitosis/_version.py
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `mitosis-0.5.0b1/.pre-commit-config.yaml` & `mitosis-0.5.0b2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0b1/LICENSE` & `mitosis-0.5.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0b1/PKG-INFO` & `mitosis-0.5.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitosis
-Version: 0.5.0b1
+Version: 0.5.0b2
 Summary: Reproduce Machine Learning experiments easily
 Author-email: Jake Stevens-Haas <jacob.stevens.haas@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/Jacob-Stevens-Haas/mitosis
 Keywords: Machine Learning,Science,Mathematics,Experiments
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -260,16 +260,16 @@
     real_data = ["geospatial.datasets:load_data", "my_paper:data_config"]
     sim_data = ["first_exp:make_data", "my_paper:data_config"]
     fit_eval = ["first_exp:linear_pipeline", "my_paper:meth_config"]
 
 This also says that the lookup dicts for each step are all imported from `my_paper`.  You would invoke experiments like:
 
 ```
-mitosis sim_data fit_eval --p sim_data.noise=low -e linear_pipeline.alpha=.5
-mitosis real_data fit_eval -p real_data.file="oct-2024.hd5" -e linear_pipeline.alpha=.5
+mitosis sim_data fit_eval -p sim_data.noise=low -e fit_eval.alpha=.5
+mitosis real_data fit_eval -p real_data.file="oct-2024.hd5" -e fit_eval.alpha=.5
 ```
 
 Needless to say, all of the callables need to pass data compatibly, e.g.
 `first_exp.linear_pipeline(first_exp.make_data(...)["data"], ...)` must make sense, as must
 `first_exp.linear_pipeline(geospatial.datasets.load_data(...)["data"], ...)`.  Some caution here is advised - mitosis does not yet check all editably-installed packages for being git-clean.
 
 You could then have code in `my_paper` that loads the data from these trials and builds comparison plots, or you could rely on the plots each experiment creates.  You could also have a shell/batch script that spawns the main experiments of your paper.
```

### Comparing `mitosis-0.5.0b1/README.md` & `mitosis-0.5.0b2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -205,16 +205,16 @@
     real_data = ["geospatial.datasets:load_data", "my_paper:data_config"]
     sim_data = ["first_exp:make_data", "my_paper:data_config"]
     fit_eval = ["first_exp:linear_pipeline", "my_paper:meth_config"]
 
 This also says that the lookup dicts for each step are all imported from `my_paper`.  You would invoke experiments like:
 
 ```
-mitosis sim_data fit_eval --p sim_data.noise=low -e linear_pipeline.alpha=.5
-mitosis real_data fit_eval -p real_data.file="oct-2024.hd5" -e linear_pipeline.alpha=.5
+mitosis sim_data fit_eval -p sim_data.noise=low -e fit_eval.alpha=.5
+mitosis real_data fit_eval -p real_data.file="oct-2024.hd5" -e fit_eval.alpha=.5
 ```
 
 Needless to say, all of the callables need to pass data compatibly, e.g.
 `first_exp.linear_pipeline(first_exp.make_data(...)["data"], ...)` must make sense, as must
 `first_exp.linear_pipeline(geospatial.datasets.load_data(...)["data"], ...)`.  Some caution here is advised - mitosis does not yet check all editably-installed packages for being git-clean.
 
 You could then have code in `my_paper` that loads the data from these trials and builds comparison plots, or you could rely on the plots each experiment creates.  You could also have a shell/batch script that spawns the main experiments of your paper.
```

### Comparing `mitosis-0.5.0b1/docs/source/conf.py` & `mitosis-0.5.0b2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0b1/mitosis/__init__.py` & `mitosis-0.5.0b2/mitosis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,18 @@
 from sqlalchemy import MetaData
 from sqlalchemy import select
 from sqlalchemy import String
 from sqlalchemy import Table
 from sqlalchemy import update
 
 from . import _disk
+from ._disk import _locate_trial_folder
 from ._typing import ExpStep
 from ._typing import Parameter
-from mitosis._disk import _locate_trial_folder
+from ._version import version as __version__  # noqa: F401
 
 
 def trials_columns():
     return [
         Column("variant", String, primary_key=True),
         Column("iteration", Integer, primary_key=True),
         Column("commit", String, nullable=False),
```

### Comparing `mitosis-0.5.0b1/mitosis/__main__.py` & `mitosis-0.5.0b2/mitosis/__main__.py`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0b1/mitosis/_disk.py` & `mitosis-0.5.0b2/mitosis/_disk.py`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0b1/mitosis/_typing.py` & `mitosis-0.5.0b2/mitosis/_typing.py`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0b1/mitosis/tests/test_all.py` & `mitosis-0.5.0b2/mitosis/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0b1/mitosis/tests/test_cli.py` & `mitosis-0.5.0b2/mitosis/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0b1/mitosis.egg-info/PKG-INFO` & `mitosis-0.5.0b2/mitosis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitosis
-Version: 0.5.0b1
+Version: 0.5.0b2
 Summary: Reproduce Machine Learning experiments easily
 Author-email: Jake Stevens-Haas <jacob.stevens.haas@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/Jacob-Stevens-Haas/mitosis
 Keywords: Machine Learning,Science,Mathematics,Experiments
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -260,16 +260,16 @@
     real_data = ["geospatial.datasets:load_data", "my_paper:data_config"]
     sim_data = ["first_exp:make_data", "my_paper:data_config"]
     fit_eval = ["first_exp:linear_pipeline", "my_paper:meth_config"]
 
 This also says that the lookup dicts for each step are all imported from `my_paper`.  You would invoke experiments like:
 
 ```
-mitosis sim_data fit_eval --p sim_data.noise=low -e linear_pipeline.alpha=.5
-mitosis real_data fit_eval -p real_data.file="oct-2024.hd5" -e linear_pipeline.alpha=.5
+mitosis sim_data fit_eval -p sim_data.noise=low -e fit_eval.alpha=.5
+mitosis real_data fit_eval -p real_data.file="oct-2024.hd5" -e fit_eval.alpha=.5
 ```
 
 Needless to say, all of the callables need to pass data compatibly, e.g.
 `first_exp.linear_pipeline(first_exp.make_data(...)["data"], ...)` must make sense, as must
 `first_exp.linear_pipeline(geospatial.datasets.load_data(...)["data"], ...)`.  Some caution here is advised - mitosis does not yet check all editably-installed packages for being git-clean.
 
 You could then have code in `my_paper` that loads the data from these trials and builds comparison plots, or you could rely on the plots each experiment creates.  You could also have a shell/batch script that spawns the main experiments of your paper.
```

### Comparing `mitosis-0.5.0b1/mitosis.egg-info/SOURCES.txt` & `mitosis-0.5.0b2/mitosis.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 .github/workflows/release.yaml
 docs/source/conf.py
 docs/source/index.rst
 mitosis/__init__.py
 mitosis/__main__.py
 mitosis/_disk.py
 mitosis/_typing.py
+mitosis/_version.py
 mitosis/py.typed
 mitosis.egg-info/PKG-INFO
 mitosis.egg-info/SOURCES.txt
 mitosis.egg-info/dependency_links.txt
 mitosis.egg-info/entry_points.txt
 mitosis.egg-info/requires.txt
 mitosis.egg-info/top_level.txt
```

### Comparing `mitosis-0.5.0b1/pyproject.toml` & `mitosis-0.5.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 [project.scripts]
 mitosis="mitosis.__main__:main"
 
 [tool.setuptools]
 packages = ["mitosis"]
 
 [tool.setuptools_scm]
+version_file = "mitosis/_version.py"
 
 [tool.black]
 line-length = 88
 extend-exclude = '''
 /(
     \.git
   | \.mypy_cache
```


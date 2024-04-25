# Comparing `tmp/ropt_nomad-0.1.0.tar.gz` & `tmp/ropt_nomad-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ropt_nomad-0.1.0.tar", last modified: Mon Apr 22 08:00:43 2024, max compression
+gzip compressed data, was "ropt_nomad-0.2.0.tar", last modified: Thu Apr 25 09:41:05 2024, max compression
```

## Comparing `ropt_nomad-0.1.0.tar` & `ropt_nomad-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 08:00:43.695659 ropt_nomad-0.1.0/
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 08:00:43.687659 ropt_nomad-0.1.0/.github/
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 08:00:43.687659 ropt_nomad-0.1.0/.github/workflows/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      969 2024-04-22 07:50:18.000000 ropt_nomad-0.1.0/.github/workflows/static-checks.yml
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      754 2024-04-22 07:56:55.000000 ropt_nomad-0.1.0/.github/workflows/tests.yml
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       96 2024-04-22 07:36:12.000000 ropt_nomad-0.1.0/.gitignore
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    35149 2024-04-22 07:45:10.000000 ropt_nomad-0.1.0/LICENSE
--rw-r--r--   0 verveerpj  (1000) verveerpj  (1000)     2919 2024-04-22 08:00:43.695659 ropt_nomad-0.1.0/PKG-INFO
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2052 2024-04-22 07:57:34.000000 ropt_nomad-0.1.0/README.md
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 08:00:43.691659 ropt_nomad-0.1.0/examples/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2544 2024-04-22 07:39:56.000000 ropt_nomad-0.1.0/examples/discrete.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2269 2024-04-22 07:39:56.000000 ropt_nomad-0.1.0/examples/rosenbrock.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2184 2024-04-22 07:38:53.000000 ropt_nomad-0.1.0/pyproject.toml
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       38 2024-04-22 08:00:43.695659 ropt_nomad-0.1.0/setup.cfg
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 08:00:43.687659 ropt_nomad-0.1.0/src/
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 08:00:43.691659 ropt_nomad-0.1.0/src/ropt_nomad/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       78 2024-04-22 07:40:01.000000 ropt_nomad-0.1.0/src/ropt_nomad/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    12443 2024-04-22 07:40:04.000000 ropt_nomad-0.1.0/src/ropt_nomad/nomad.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        0 2023-12-04 15:07:29.000000 ropt_nomad-0.1.0/src/ropt_nomad/py.typed
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      411 2024-04-22 08:00:43.000000 ropt_nomad-0.1.0/src/ropt_nomad/version.py
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 08:00:43.691659 ropt_nomad-0.1.0/src/ropt_nomad.egg-info/
--rw-r--r--   0 verveerpj  (1000) verveerpj  (1000)     2919 2024-04-22 08:00:43.000000 ropt_nomad-0.1.0/src/ropt_nomad.egg-info/PKG-INFO
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      569 2024-04-22 08:00:43.000000 ropt_nomad-0.1.0/src/ropt_nomad.egg-info/SOURCES.txt
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        1 2024-04-22 08:00:43.000000 ropt_nomad-0.1.0/src/ropt_nomad.egg-info/dependency_links.txt
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       65 2024-04-22 08:00:43.000000 ropt_nomad-0.1.0/src/ropt_nomad.egg-info/entry_points.txt
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       36 2024-04-22 08:00:43.000000 ropt_nomad-0.1.0/src/ropt_nomad.egg-info/requires.txt
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       11 2024-04-22 08:00:43.000000 ropt_nomad-0.1.0/src/ropt_nomad.egg-info/top_level.txt
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 08:00:43.691659 ropt_nomad-0.1.0/tests/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        0 2023-12-04 15:07:29.000000 ropt_nomad-0.1.0/tests/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2496 2024-04-22 07:40:06.000000 ropt_nomad-0.1.0/tests/conftest.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      815 2024-02-20 14:41:06.000000 ropt_nomad-0.1.0/tests/test_examples.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    11327 2024-04-22 07:40:07.000000 ropt_nomad-0.1.0/tests/test_nomad_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:05.132851 ropt_nomad-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:05.124851 ropt_nomad-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:05.128851 ropt_nomad-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/.github/workflows/static-checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-25 09:41:05.132851 ropt_nomad-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:05.128851 ropt_nomad-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/examples/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/examples/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 09:41:05.132851 ropt_nomad-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:05.124851 ropt_nomad-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:05.128851 ropt_nomad-0.2.0/src/ropt_nomad/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/src/ropt_nomad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12571 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/src/ropt_nomad/nomad.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/src/ropt_nomad/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 09:41:05.000000 ropt_nomad-0.2.0/src/ropt_nomad/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:05.128851 ropt_nomad-0.2.0/src/ropt_nomad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-25 09:41:05.000000 ropt_nomad-0.2.0/src/ropt_nomad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-25 09:41:05.000000 ropt_nomad-0.2.0/src/ropt_nomad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:41:05.000000 ropt_nomad-0.2.0/src/ropt_nomad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-25 09:41:05.000000 ropt_nomad-0.2.0/src/ropt_nomad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 09:41:05.000000 ropt_nomad-0.2.0/src/ropt_nomad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 09:41:05.000000 ropt_nomad-0.2.0/src/ropt_nomad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:05.128851 ropt_nomad-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/tests/test_nomad_backend.py
```

### Comparing `ropt_nomad-0.1.0/.github/workflows/static-checks.yml` & `ropt_nomad-0.2.0/.github/workflows/static-checks.yml`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.1.0/.github/workflows/tests.yml` & `ropt_nomad-0.2.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.1.0/LICENSE` & `ropt_nomad-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.1.0/PKG-INFO` & `ropt_nomad-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ropt-nomad
-Version: 0.1.0
-Summary: A NOMAD backend for the ropt robust optimization packages
+Version: 0.2.0
+Summary: A NOMAD backend for the ropt robust optimization package
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -39,17 +39,16 @@
 ```bash
 pip install ropt-nomad
 ```
 
 
 ## Usage
 An optimization by ropt using the plugin works mostly as any other optimization
-run (see also the `ropt` documentation on
-[GitHubPages](https://tno-ropt.github.io/ropt/) or on [Read the
-Docs](https://ropt.readthedocs.io/)). However, there are a few things to
+run (see also the [ropt documentation](https://tno-ropt.github.io/ropt/)).
+However, there are a few things to
 consider:
 
 1. Gradients are not used, any specifications relating to gradient calculations
    in ropt are ignored.
 2. Some standard optimization parameters that can be specified in the
    optimization section are ignored, specifically:
     - `algorithm`
@@ -65,20 +64,23 @@
    - The `MAX_ITERATIONS` keyword can only be used if the `max_iterations` field
      is not set in the optimizer configuration.
    - `BB_OUTPUT_TYPE` can be overridden, which is useful to change the type of
      constraint handling.
 
 
 ## Developement
-To install, enter the distribution directory and execute:
+The `ropt-nomad` source distribution can be found on
+[GitHub](https://github.com/tno-ropt/ropt-nomad). To install from source, enter
+the `ropt-pymoo` distribution directory and execute:
 
 ```bash
 pip install .
 ```
 
+
 ## Running the tests
 To run the test suite, install the necessary dependencies and execute `pytest`:
 
 ```bash
 pip install .[test]
 pytest
 ```
```

### Comparing `ropt_nomad-0.1.0/README.md` & `ropt_nomad-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -16,17 +16,16 @@
 ```bash
 pip install ropt-nomad
 ```
 
 
 ## Usage
 An optimization by ropt using the plugin works mostly as any other optimization
-run (see also the `ropt` documentation on
-[GitHubPages](https://tno-ropt.github.io/ropt/) or on [Read the
-Docs](https://ropt.readthedocs.io/)). However, there are a few things to
+run (see also the [ropt documentation](https://tno-ropt.github.io/ropt/)).
+However, there are a few things to
 consider:
 
 1. Gradients are not used, any specifications relating to gradient calculations
    in ropt are ignored.
 2. Some standard optimization parameters that can be specified in the
    optimization section are ignored, specifically:
     - `algorithm`
@@ -42,20 +41,23 @@
    - The `MAX_ITERATIONS` keyword can only be used if the `max_iterations` field
      is not set in the optimizer configuration.
    - `BB_OUTPUT_TYPE` can be overridden, which is useful to change the type of
      constraint handling.
 
 
 ## Developement
-To install, enter the distribution directory and execute:
+The `ropt-nomad` source distribution can be found on
+[GitHub](https://github.com/tno-ropt/ropt-nomad). To install from source, enter
+the `ropt-pymoo` distribution directory and execute:
 
 ```bash
 pip install .
 ```
 
+
 ## Running the tests
 To run the test suite, install the necessary dependencies and execute `pytest`:
 
 ```bash
 pip install .[test]
 pytest
 ```
```

### Comparing `ropt_nomad-0.1.0/examples/discrete.py` & `ropt_nomad-0.2.0/examples/discrete.py`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.1.0/examples/rosenbrock.py` & `ropt_nomad-0.2.0/examples/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.1.0/pyproject.toml` & `ropt_nomad-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ropt-nomad"
-description = "A NOMAD backend for the ropt robust optimization packages"
+description = "A NOMAD backend for the ropt robust optimization package"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: English",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
```

### Comparing `ropt_nomad-0.1.0/src/ropt_nomad/nomad.py` & `ropt_nomad-0.2.0/src/ropt_nomad/nomad.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,20 +134,17 @@
             upper_bounds = upper_bounds[variable_indices]
         return lower_bounds.tolist(), upper_bounds.tolist()
 
     def _evaluate(
         self,
         block_or_eval_point: Union[PyNomad.PyNomadEvalPoint, PyNomad.PyNomadBlock],
     ) -> Union[int, List[int]]:
-        return_value: Union[int, List[int]]
         if isinstance(block_or_eval_point, PyNomad.PyNomadEvalPoint):
-            return_value = 1
             eval_points = [block_or_eval_point]
         else:
-            return_value = [1] * block_or_eval_point.size()
             eval_points = [
                 block_or_eval_point.get_x(block_idx)
                 for block_idx in range(block_or_eval_point.size())
             ]
         variables = np.vstack(
             [
                 np.fromiter(
@@ -162,15 +159,20 @@
         for idx, eval_point in enumerate(eval_points):
             result_string = str(objectives[idx])
             if constraints.size:
                 result_string += " " + " ".join(
                     str(value) for value in constraints[idx, :]
                 )
             eval_point.setBBO(result_string.encode("UTF-8"))
-        return return_value
+
+        return (
+            not np.isnan(objectives[0])
+            if isinstance(block_or_eval_point, PyNomad.PyNomadEvalPoint)
+            else [not np.isnan(objective) for objective in objectives]
+        )
 
     def _get_parameters(self) -> List[str]:  # noqa: C901, PLR0912
         variable_indices = self._config.variables.indices
         dim = (
             self._config.variables.initial_values.size
             if variable_indices is None
             else variable_indices.size
@@ -316,11 +318,14 @@
         ):
             self._cached_variables = None
             self._cached_function = None
         if self._cached_function is None:
             self._cached_variables = variables.copy()
             with self._redirector.stop():
                 function, _ = self._optimizer_callback(
-                    variables, return_functions=True, return_gradients=False
+                    variables,
+                    return_functions=True,
+                    return_gradients=False,
+                    allow_nan=True,
                 )
             self._cached_function = function.copy()
         return self._cached_function
```

### Comparing `ropt_nomad-0.1.0/src/ropt_nomad.egg-info/PKG-INFO` & `ropt_nomad-0.2.0/src/ropt_nomad.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ropt-nomad
-Version: 0.1.0
-Summary: A NOMAD backend for the ropt robust optimization packages
+Version: 0.2.0
+Summary: A NOMAD backend for the ropt robust optimization package
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -39,17 +39,16 @@
 ```bash
 pip install ropt-nomad
 ```
 
 
 ## Usage
 An optimization by ropt using the plugin works mostly as any other optimization
-run (see also the `ropt` documentation on
-[GitHubPages](https://tno-ropt.github.io/ropt/) or on [Read the
-Docs](https://ropt.readthedocs.io/)). However, there are a few things to
+run (see also the [ropt documentation](https://tno-ropt.github.io/ropt/)).
+However, there are a few things to
 consider:
 
 1. Gradients are not used, any specifications relating to gradient calculations
    in ropt are ignored.
 2. Some standard optimization parameters that can be specified in the
    optimization section are ignored, specifically:
     - `algorithm`
@@ -65,20 +64,23 @@
    - The `MAX_ITERATIONS` keyword can only be used if the `max_iterations` field
      is not set in the optimizer configuration.
    - `BB_OUTPUT_TYPE` can be overridden, which is useful to change the type of
      constraint handling.
 
 
 ## Developement
-To install, enter the distribution directory and execute:
+The `ropt-nomad` source distribution can be found on
+[GitHub](https://github.com/tno-ropt/ropt-nomad). To install from source, enter
+the `ropt-pymoo` distribution directory and execute:
 
 ```bash
 pip install .
 ```
 
+
 ## Running the tests
 To run the test suite, install the necessary dependencies and execute `pytest`:
 
 ```bash
 pip install .[test]
 pytest
 ```
```

### Comparing `ropt_nomad-0.1.0/src/ropt_nomad.egg-info/SOURCES.txt` & `ropt_nomad-0.2.0/src/ropt_nomad.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 LICENSE
 README.md
 pyproject.toml
+.github/workflows/release.yml
 .github/workflows/static-checks.yml
 .github/workflows/tests.yml
 examples/discrete.py
 examples/rosenbrock.py
 src/ropt_nomad/__init__.py
 src/ropt_nomad/nomad.py
 src/ropt_nomad/py.typed
```

### Comparing `ropt_nomad-0.1.0/tests/conftest.py` & `ropt_nomad-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.1.0/tests/test_examples.py` & `ropt_nomad-0.2.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.1.0/tests/test_nomad_backend.py` & `ropt_nomad-0.2.0/tests/test_nomad_backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -313,7 +313,55 @@
     enopt_config["optimizer"]["parallel"] = True
     optimizer = EnsembleOptimizer(evaluator())
     with pytest.raises(
         ConfigError,
         match="Option Error: BB_MAX_BLOCK_SIZE must be specified",
     ):
         optimizer.start_optimization(plan=[{"config": enopt_config}, {"optimizer": {}}])
+
+
+@pytest.mark.parametrize("parallel", [False, True])
+def test_nomad_evaluation_failure(
+    enopt_config: Dict[str, Any], evaluator: Any, parallel: bool, test_functions: Any
+) -> None:
+    enopt_config["variables"]["lower_bounds"] = [0.15, -1.0, -1.0]
+    enopt_config["variables"]["upper_bounds"] = [1.0, 1.0, 0.2]
+    enopt_config["optimizer"]["max_iterations"] = 3
+    enopt_config["optimizer"]["parallel"] = parallel
+    enopt_config["realizations"] = {"realization_min_success": 0}
+    if parallel:
+        enopt_config["optimizer"]["options"] = ["BB_MAX_BLOCK_SIZE 4"]
+
+    optimizer = EnsembleOptimizer(evaluator())
+    result1 = optimizer.start_optimization(
+        plan=[
+            {"config": enopt_config},
+            {"optimizer": {"id": "opt"}},
+            {"tracker": {"id": "optimum", "source": "opt"}},
+        ],
+    )
+    assert result1 is not None
+    assert np.allclose(result1.evaluations.variables, [0.15, 0.0, 0.2], atol=0.02)
+
+    counter = 0
+
+    def _add_nan(x: Any) -> Any:
+        nonlocal counter
+        counter += 1
+        if counter == 2:
+            counter = 0
+            return np.nan
+        return test_functions[0](x)
+
+    optimizer = EnsembleOptimizer(evaluator((_add_nan, test_functions[1])))
+    result2 = optimizer.start_optimization(
+        plan=[
+            {"config": enopt_config},
+            {"optimizer": {"id": "opt"}},
+            {"tracker": {"id": "optimum", "source": "opt"}},
+        ],
+    )
+    assert result2 is not None
+    assert np.allclose(result2.evaluations.variables, [0.15, 0.0, 0.2], atol=0.02)
+    assert not np.all(
+        np.equal(result1.evaluations.variables, result2.evaluations.variables)
+    )
```


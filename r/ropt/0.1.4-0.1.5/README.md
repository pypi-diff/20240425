# Comparing `tmp/ropt-0.1.4.tar.gz` & `tmp/ropt-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ropt-0.1.4.tar", last modified: Wed Apr 24 09:22:00 2024, max compression
+gzip compressed data, was "ropt-0.1.5.tar", last modified: Thu Apr 25 09:31:32 2024, max compression
```

## Comparing `ropt-0.1.4.tar` & `ropt-0.1.5.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.033425 ropt-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.001425 ropt-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.005425 ropt-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-24 09:21:50.000000 ropt-0.1.4/.github/workflows/build-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-24 09:21:50.000000 ropt-0.1.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-24 09:21:50.000000 ropt-0.1.4/.github/workflows/static-checks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-24 09:21:50.000000 ropt-0.1.4/.github/workflows/tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-04-24 09:21:50.000000 ropt-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 09:21:50.000000 ropt-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-24 09:22:00.033425 ropt-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-24 09:21:50.000000 ropt-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.005425 ropt-0.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-24 09:21:50.000000 ropt-0.1.4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.005425 ropt-0.1.4/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-24 09:21:50.000000 ropt-0.1.4/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.009425 ropt-0.1.4/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-24 09:21:50.000000 ropt-0.1.4/docs/reference/enopt_config.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-24 09:21:50.000000 ropt-0.1.4/docs/reference/enums.md
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-24 09:21:50.000000 ropt-0.1.4/docs/reference/evaluator.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-24 09:21:50.000000 ropt-0.1.4/docs/reference/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-24 09:21:50.000000 ropt-0.1.4/docs/reference/function_transforms.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-24 09:21:50.000000 ropt-0.1.4/docs/reference/optimization.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-24 09:21:50.000000 ropt-0.1.4/docs/reference/optimization_steps.md
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-24 09:21:50.000000 ropt-0.1.4/docs/reference/optimizer_backends.md
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-24 09:21:50.000000 ropt-0.1.4/docs/reference/plan_config.md
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 09:21:50.000000 ropt-0.1.4/docs/reference/plugins.md
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-24 09:21:50.000000 ropt-0.1.4/docs/reference/realization_filters.md
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 09:21:50.000000 ropt-0.1.4/docs/reference/reporting.md
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-24 09:21:50.000000 ropt-0.1.4/docs/reference/results.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-24 09:21:50.000000 ropt-0.1.4/docs/reference/sampler_backends.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-24 09:21:50.000000 ropt-0.1.4/docs/reference/utilities.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.009425 ropt-0.1.4/docs/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-24 09:21:50.000000 ropt-0.1.4/docs/usage/robust_optimization.md
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-24 09:21:50.000000 ropt-0.1.4/docs/usage/running.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.009425 ropt-0.1.4/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-24 09:21:50.000000 ropt-0.1.4/examples/de_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-24 09:21:50.000000 ropt-0.1.4/examples/de_nonlinear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-24 09:21:50.000000 ropt-0.1.4/examples/rosenbrock_deterministic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-24 09:21:50.000000 ropt-0.1.4/examples/rosenbrock_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.009425 ropt-0.1.4/examples/script_optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-24 09:21:50.000000 ropt-0.1.4/examples/script_optimizer/rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-24 09:21:50.000000 ropt-0.1.4/examples/script_optimizer/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-24 09:21:50.000000 ropt-0.1.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-24 09:21:50.000000 ropt-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 09:22:00.033425 ropt-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.001425 ropt-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.013425 ropt-0.1.4/src/ropt/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.013425 ropt-0.1.4/src/ropt/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17499 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/apps/_script_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.013425 ropt-0.1.4/src/ropt/config/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.017425 ropt-0.1.4/src/ropt/config/enopt/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/enopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/enopt/_enopt_base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/enopt/_enopt_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/enopt/_function_transform_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/enopt/_gradient_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/enopt/_linear_constraints_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/enopt/_nonlinear_constraints_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/enopt/_objective_functions_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/enopt/_optimizer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/enopt/_realization_filter_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/enopt/_realizations_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/enopt/_sampler_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/enopt/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/enopt/_variables_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/enopt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.017425 ropt-0.1.4/src/ropt/config/plan/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/plan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/plan/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/plan/_plan_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/plan/_step_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.017425 ropt-0.1.4/src/ropt/evaluator/
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/evaluator/_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    25277 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/evaluator/_ensemble_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/evaluator/_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/evaluator/_evaluator_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/evaluator/_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/evaluator/_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/evaluator/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/evaluator/parsl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.017425 ropt-0.1.4/src/ropt/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/optimization/_bases.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/optimization/_ensemble_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/optimization/_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/optimization/_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/optimization/_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.021425 ropt-0.1.4/src/ropt/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.021425 ropt-0.1.4/src/ropt/plugins/function_transform/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/function_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/function_transform/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/function_transform/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.021425 ropt-0.1.4/src/ropt/plugins/optimization_steps/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/optimization_steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/optimization_steps/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/optimization_steps/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/optimization_steps/enopt_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/optimization_steps/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/optimization_steps/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/optimization_steps/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/optimization_steps/reset_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/optimization_steps/restart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/optimization_steps/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/optimization_steps/update_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.021425 ropt-0.1.4/src/ropt/plugins/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/optimizer/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    20113 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/optimizer/scipy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/optimizer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.021425 ropt-0.1.4/src/ropt/plugins/realization_filter/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/realization_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15031 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/realization_filter/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/realization_filter/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.025425 ropt-0.1.4/src/ropt/plugins/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/sampler/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/plugins/sampler/scipy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.025425 ropt-0.1.4/src/ropt/report/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/report/_data_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/report/_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/report/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.029425 ropt-0.1.4/src/ropt/results/
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/results/_bound_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/results/_function_evaluations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/results/_function_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/results/_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/results/_gradient_evaluations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/results/_gradient_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/results/_gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/results/_linear_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/results/_maximize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/results/_nonlinear_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/results/_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/results/_realizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/results/_result_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/results/_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/results/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/results/_xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.029425 ropt-0.1.4/src/ropt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/utils/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-24 09:21:50.000000 ropt-0.1.4/src/ropt/utils/scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 09:21:59.000000 ropt-0.1.4/src/ropt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.033425 ropt-0.1.4/src/ropt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-24 09:21:59.000000 ropt-0.1.4/src/ropt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-24 09:21:59.000000 ropt-0.1.4/src/ropt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:21:59.000000 ropt-0.1.4/src/ropt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-24 09:21:59.000000 ropt-0.1.4/src/ropt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 09:21:59.000000 ropt-0.1.4/src/ropt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:22:00.033425 ropt-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:21:50.000000 ropt-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-24 09:21:50.000000 ropt-0.1.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-24 09:21:50.000000 ropt-0.1.4/tests/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    25786 2024-04-24 09:21:50.000000 ropt-0.1.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-24 09:21:50.000000 ropt-0.1.4/tests/test_ensemble_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-24 09:21:50.000000 ropt-0.1.4/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-24 09:21:50.000000 ropt-0.1.4/tests/test_failed_realizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-24 09:21:50.000000 ropt-0.1.4/tests/test_function_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-24 09:21:50.000000 ropt-0.1.4/tests/test_netcdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    42608 2024-04-24 09:21:50.000000 ropt-0.1.4/tests/test_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-04-24 09:21:50.000000 ropt-0.1.4/tests/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-04-24 09:21:50.000000 ropt-0.1.4/tests/test_parsl.py
--rw-r--r--   0 runner    (1001) docker     (127)    27696 2024-04-24 09:21:50.000000 ropt-0.1.4/tests/test_realization_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-04-24 09:21:50.000000 ropt-0.1.4/tests/test_result_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-04-24 09:21:50.000000 ropt-0.1.4/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-24 09:21:50.000000 ropt-0.1.4/tests/test_results_data_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-24 09:21:50.000000 ropt-0.1.4/tests/test_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19164 2024-04-24 09:21:50.000000 ropt-0.1.4/tests/test_scipy_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-24 09:21:50.000000 ropt-0.1.4/tests/test_scipy_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-24 09:21:50.000000 ropt-0.1.4/tests/test_xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.443644 ropt-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.415644 ropt-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.419644 ropt-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-25 09:31:25.000000 ropt-0.1.5/.github/workflows/build-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-25 09:31:25.000000 ropt-0.1.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-25 09:31:25.000000 ropt-0.1.5/.github/workflows/static-checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-25 09:31:25.000000 ropt-0.1.5/.github/workflows/tests.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-04-25 09:31:25.000000 ropt-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 09:31:25.000000 ropt-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-25 09:31:32.443644 ropt-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-25 09:31:25.000000 ropt-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.419644 ropt-0.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-25 09:31:25.000000 ropt-0.1.5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.419644 ropt-0.1.5/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-25 09:31:25.000000 ropt-0.1.5/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.423644 ropt-0.1.5/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-25 09:31:25.000000 ropt-0.1.5/docs/reference/enopt_config.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 09:31:25.000000 ropt-0.1.5/docs/reference/enums.md
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-25 09:31:25.000000 ropt-0.1.5/docs/reference/evaluator.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 09:31:25.000000 ropt-0.1.5/docs/reference/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-25 09:31:25.000000 ropt-0.1.5/docs/reference/function_transforms.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 09:31:25.000000 ropt-0.1.5/docs/reference/optimization.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 09:31:25.000000 ropt-0.1.5/docs/reference/optimization_steps.md
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-25 09:31:25.000000 ropt-0.1.5/docs/reference/optimizer_backends.md
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-25 09:31:25.000000 ropt-0.1.5/docs/reference/plan_config.md
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 09:31:25.000000 ropt-0.1.5/docs/reference/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-25 09:31:25.000000 ropt-0.1.5/docs/reference/realization_filters.md
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-25 09:31:25.000000 ropt-0.1.5/docs/reference/reporting.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-25 09:31:25.000000 ropt-0.1.5/docs/reference/results.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-25 09:31:25.000000 ropt-0.1.5/docs/reference/sampler_backends.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 09:31:25.000000 ropt-0.1.5/docs/reference/utilities.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.423644 ropt-0.1.5/docs/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-25 09:31:25.000000 ropt-0.1.5/docs/usage/robust_optimization.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-25 09:31:25.000000 ropt-0.1.5/docs/usage/running.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.423644 ropt-0.1.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-25 09:31:25.000000 ropt-0.1.5/examples/de_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-25 09:31:25.000000 ropt-0.1.5/examples/de_nonlinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-25 09:31:25.000000 ropt-0.1.5/examples/rosenbrock_deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-25 09:31:25.000000 ropt-0.1.5/examples/rosenbrock_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.423644 ropt-0.1.5/examples/script_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-25 09:31:25.000000 ropt-0.1.5/examples/script_optimizer/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-25 09:31:25.000000 ropt-0.1.5/examples/script_optimizer/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-25 09:31:25.000000 ropt-0.1.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-25 09:31:25.000000 ropt-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 09:31:32.443644 ropt-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.415644 ropt-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.423644 ropt-0.1.5/src/ropt/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.423644 ropt-0.1.5/src/ropt/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17499 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/apps/_script_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.423644 ropt-0.1.5/src/ropt/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.427644 ropt-0.1.5/src/ropt/config/enopt/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/enopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/enopt/_enopt_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/enopt/_enopt_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/enopt/_function_transform_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/enopt/_gradient_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/enopt/_linear_constraints_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/enopt/_nonlinear_constraints_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/enopt/_objective_functions_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/enopt/_optimizer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/enopt/_realization_filter_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/enopt/_realizations_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/enopt/_sampler_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/enopt/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/enopt/_variables_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/enopt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.427644 ropt-0.1.5/src/ropt/config/plan/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/plan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/plan/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/plan/_plan_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/plan/_step_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.431644 ropt-0.1.5/src/ropt/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/evaluator/_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25967 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/evaluator/_ensemble_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/evaluator/_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/evaluator/_evaluator_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/evaluator/_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/evaluator/_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/evaluator/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/evaluator/parsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.431644 ropt-0.1.5/src/ropt/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/optimization/_bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/optimization/_ensemble_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/optimization/_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/optimization/_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/optimization/_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.431644 ropt-0.1.5/src/ropt/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.431644 ropt-0.1.5/src/ropt/plugins/function_transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/function_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/function_transform/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/function_transform/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.435644 ropt-0.1.5/src/ropt/plugins/optimization_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/optimization_steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/optimization_steps/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/optimization_steps/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/optimization_steps/enopt_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/optimization_steps/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/optimization_steps/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/optimization_steps/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/optimization_steps/reset_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/optimization_steps/restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/optimization_steps/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/optimization_steps/update_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.435644 ropt-0.1.5/src/ropt/plugins/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/optimizer/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20113 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/optimizer/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/optimizer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.435644 ropt-0.1.5/src/ropt/plugins/realization_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/realization_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15031 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/realization_filter/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/realization_filter/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.435644 ropt-0.1.5/src/ropt/plugins/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/sampler/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/plugins/sampler/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.435644 ropt-0.1.5/src/ropt/report/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/report/_data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/report/_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/report/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.439644 ropt-0.1.5/src/ropt/results/
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/results/_bound_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/results/_function_evaluations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/results/_function_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/results/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/results/_gradient_evaluations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/results/_gradient_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/results/_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/results/_linear_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/results/_maximize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/results/_nonlinear_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/results/_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/results/_realizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/results/_result_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/results/_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/results/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/results/_xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.439644 ropt-0.1.5/src/ropt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/utils/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-25 09:31:25.000000 ropt-0.1.5/src/ropt/utils/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 09:31:32.000000 ropt-0.1.5/src/ropt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.443644 ropt-0.1.5/src/ropt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-25 09:31:32.000000 ropt-0.1.5/src/ropt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-25 09:31:32.000000 ropt-0.1.5/src/ropt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:31:32.000000 ropt-0.1.5/src/ropt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-25 09:31:32.000000 ropt-0.1.5/src/ropt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 09:31:32.000000 ropt-0.1.5/src/ropt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:32.443644 ropt-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:31:25.000000 ropt-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-25 09:31:25.000000 ropt-0.1.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-25 09:31:25.000000 ropt-0.1.5/tests/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25786 2024-04-25 09:31:25.000000 ropt-0.1.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-25 09:31:25.000000 ropt-0.1.5/tests/test_ensemble_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-25 09:31:25.000000 ropt-0.1.5/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-25 09:31:25.000000 ropt-0.1.5/tests/test_failed_realizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-25 09:31:25.000000 ropt-0.1.5/tests/test_function_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-25 09:31:25.000000 ropt-0.1.5/tests/test_netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43104 2024-04-25 09:31:25.000000 ropt-0.1.5/tests/test_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-04-25 09:31:25.000000 ropt-0.1.5/tests/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-04-25 09:31:25.000000 ropt-0.1.5/tests/test_parsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27696 2024-04-25 09:31:25.000000 ropt-0.1.5/tests/test_realization_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-04-25 09:31:25.000000 ropt-0.1.5/tests/test_result_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-04-25 09:31:25.000000 ropt-0.1.5/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-25 09:31:25.000000 ropt-0.1.5/tests/test_results_data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-25 09:31:25.000000 ropt-0.1.5/tests/test_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19164 2024-04-25 09:31:25.000000 ropt-0.1.5/tests/test_scipy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-25 09:31:25.000000 ropt-0.1.5/tests/test_scipy_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-25 09:31:25.000000 ropt-0.1.5/tests/test_xarray.py
```

### Comparing `ropt-0.1.4/.github/workflows/build-docs.yml` & `ropt-0.1.5/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/.github/workflows/release.yml` & `ropt-0.1.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/.github/workflows/static-checks.yml` & `ropt-0.1.5/.github/workflows/static-checks.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/.github/workflows/tests.yml` & `ropt-0.1.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/LICENSE` & `ropt-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/PKG-INFO` & `ropt-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ropt
-Version: 0.1.4
+Version: 0.1.5
 Summary: The ropt ensemble optimizer module
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ropt-0.1.4/README.md` & `ropt-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/docs/index.md` & `ropt-0.1.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/docs/reference/evaluator.md` & `ropt-0.1.5/docs/reference/evaluator.md`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/docs/reference/realization_filters.md` & `ropt-0.1.5/docs/reference/realization_filters.md`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/docs/reference/results.md` & `ropt-0.1.5/docs/reference/results.md`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/docs/usage/robust_optimization.md` & `ropt-0.1.5/docs/usage/robust_optimization.md`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/docs/usage/running.md` & `ropt-0.1.5/docs/usage/running.md`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/examples/de_linear.py` & `ropt-0.1.5/examples/de_linear.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/examples/de_nonlinear.py` & `ropt-0.1.5/examples/de_nonlinear.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/examples/rosenbrock_deterministic.py` & `ropt-0.1.5/examples/rosenbrock_deterministic.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/examples/rosenbrock_ensemble.py` & `ropt-0.1.5/examples/rosenbrock_ensemble.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/examples/script_optimizer/rosenbrock.py` & `ropt-0.1.5/examples/script_optimizer/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/examples/script_optimizer/run.py` & `ropt-0.1.5/examples/script_optimizer/run.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/mkdocs.yml` & `ropt-0.1.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/pyproject.toml` & `ropt-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/apps/_script_optimizer.py` & `ropt-0.1.5/src/ropt/apps/_script_optimizer.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/config/enopt/__init__.py` & `ropt-0.1.5/src/ropt/config/enopt/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/config/enopt/_enopt_config.py` & `ropt-0.1.5/src/ropt/config/enopt/_enopt_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/config/enopt/_function_transform_config.py` & `ropt-0.1.5/src/ropt/config/enopt/_function_transform_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/config/enopt/_gradient_config.py` & `ropt-0.1.5/src/ropt/config/enopt/_gradient_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/config/enopt/_linear_constraints_config.py` & `ropt-0.1.5/src/ropt/config/enopt/_linear_constraints_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/config/enopt/_nonlinear_constraints_config.py` & `ropt-0.1.5/src/ropt/config/enopt/_nonlinear_constraints_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/config/enopt/_objective_functions_config.py` & `ropt-0.1.5/src/ropt/config/enopt/_objective_functions_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/config/enopt/_optimizer_config.py` & `ropt-0.1.5/src/ropt/config/enopt/_optimizer_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/config/enopt/_realization_filter_config.py` & `ropt-0.1.5/src/ropt/config/enopt/_realization_filter_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/config/enopt/_realizations_config.py` & `ropt-0.1.5/src/ropt/config/enopt/_realizations_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Configuration class for realizations."""
 
 from __future__ import annotations
 
 from typing import Optional
 
 import numpy as np
-from pydantic import PositiveInt, model_validator
+from pydantic import NonNegativeInt, model_validator
 
 from ropt.config.utils import (
     Array1D,
     UniqueNames,
     broadcast_1d_array,
     normalize,
 )
@@ -57,15 +57,15 @@
         weights:                 The weights of the realizations (default: 1)
         realization_min_success: The minimum number of successful realizations
                                  (default: equal to the number of realizations)
     """
 
     names: Optional[UniqueNames] = None
     weights: Array1D = np.array(1.0)
-    realization_min_success: Optional[PositiveInt] = None
+    realization_min_success: Optional[NonNegativeInt] = None
 
     @model_validator(mode="after")
     def _broadcast_normalize_and_check(self) -> RealizationsConfig:
         if self.names:
             size = len(self.names)
             self.weights = broadcast_1d_array(self.weights, "weights", size)
         else:
```

### Comparing `ropt-0.1.4/src/ropt/config/enopt/_sampler_config.py` & `ropt-0.1.5/src/ropt/config/enopt/_sampler_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/config/enopt/_utils.py` & `ropt-0.1.5/src/ropt/config/enopt/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/config/enopt/_variables_config.py` & `ropt-0.1.5/src/ropt/config/enopt/_variables_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/config/enopt/constants.py` & `ropt-0.1.5/src/ropt/config/enopt/constants.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/config/plan/__init__.py` & `ropt-0.1.5/src/ropt/config/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/config/plan/_config.py` & `ropt-0.1.5/src/ropt/config/plan/_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/config/plan/_plan_config.py` & `ropt-0.1.5/src/ropt/config/plan/_plan_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/config/plan/_step_config.py` & `ropt-0.1.5/src/ropt/config/plan/_step_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/config/utils.py` & `ropt-0.1.5/src/ropt/config/utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/enums.py` & `ropt-0.1.5/src/ropt/enums.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/evaluator/__init__.py` & `ropt-0.1.5/src/ropt/evaluator/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/evaluator/_concurrent.py` & `ropt-0.1.5/src/ropt/evaluator/_concurrent.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/evaluator/_ensemble_evaluator.py` & `ropt-0.1.5/src/ropt/evaluator/_ensemble_evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -380,48 +380,61 @@
         constraints: Optional[NDArray[np.float64]],
         objective_weights: Optional[NDArray[np.float64]],
         constraint_weights: Optional[NDArray[np.float64]],
         failed_realizations: NDArray[np.bool_],
     ) -> Functions:
         # Individual objective and constraint functions are calculated from the
         # realizations using one or more function transforms:
-        objectives = _calculate_transformed_functions(
-            self._config,
-            self._function_transforms,
-            objectives,
-            objective_weights,
-            failed_realizations,
-        )
-        if constraints is not None:
-            constraints = _calculate_transformed_functions(
+        if np.all(failed_realizations):
+            objectives = np.empty(
+                self._config.objective_functions.weights.size, dtype=np.float64
+            )
+            objectives.fill(np.nan)
+            if constraints is not None:
+                assert self._config.nonlinear_constraints is not None
+                constraints = np.empty(
+                    self._config.nonlinear_constraints.rhs_values, dtype=np.float64
+                )
+                constraints.fill(np.nan)
+            weighted_objective = np.array(np.nan)
+        else:
+            objectives = _calculate_transformed_functions(
                 self._config,
                 self._function_transforms,
-                constraints,
-                constraint_weights,
+                objectives,
+                objective_weights,
                 failed_realizations,
-                constraints=True,
             )
-        else:
-            constraints = None
+            if constraints is not None:
+                constraints = _calculate_transformed_functions(
+                    self._config,
+                    self._function_transforms,
+                    constraints,
+                    constraint_weights,
+                    failed_realizations,
+                    constraints=True,
+                )
+            else:
+                constraints = None
 
-        if self._objective_auto_scales is None:
-            self._objective_auto_scales = _compute_auto_scales(
-                objectives, self._config.objective_functions.auto_scale
-            )
-        if constraints is not None and self._constraint_auto_scales is None:
-            assert self._config.nonlinear_constraints is not None
-            self._constraint_auto_scales = _compute_auto_scales(
-                constraints, self._config.nonlinear_constraints.auto_scale
-            )
+            if self._objective_auto_scales is None:
+                self._objective_auto_scales = _compute_auto_scales(
+                    objectives, self._config.objective_functions.auto_scale
+                )
+            if constraints is not None and self._constraint_auto_scales is None:
+                assert self._config.nonlinear_constraints is not None
+                self._constraint_auto_scales = _compute_auto_scales(
+                    constraints, self._config.nonlinear_constraints.auto_scale
+                )
 
-        weighted_objective = _calculate_weighted_function(
-            objectives,
-            self._config.objective_functions.weights,
-            self._get_objective_scales(self._objective_auto_scales),
-        )
+            weighted_objective = _calculate_weighted_function(
+                objectives,
+                self._config.objective_functions.weights,
+                self._get_objective_scales(self._objective_auto_scales),
+            )
 
         return Functions.create(
             config=self._config,
             objective_auto_scales=self._objective_auto_scales,
             constraint_auto_scales=self._constraint_auto_scales,
             weighted_objective=weighted_objective,
             objectives=objectives,
```

### Comparing `ropt-0.1.4/src/ropt/evaluator/_evaluator.py` & `ropt-0.1.5/src/ropt/evaluator/_evaluator.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/evaluator/_evaluator_results.py` & `ropt-0.1.5/src/ropt/evaluator/_evaluator_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/evaluator/_function.py` & `ropt-0.1.5/src/ropt/evaluator/_function.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/evaluator/_gradient.py` & `ropt-0.1.5/src/ropt/evaluator/_gradient.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/evaluator/_utils.py` & `ropt-0.1.5/src/ropt/evaluator/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/evaluator/parsl.py` & `ropt-0.1.5/src/ropt/evaluator/parsl.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/events.py` & `ropt-0.1.5/src/ropt/events.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/exceptions.py` & `ropt-0.1.5/src/ropt/exceptions.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/optimization/_bases.py` & `ropt-0.1.5/src/ropt/optimization/_bases.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/optimization/_ensemble_optimizer.py` & `ropt-0.1.5/src/ropt/optimization/_ensemble_optimizer.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/optimization/_events.py` & `ropt-0.1.5/src/ropt/optimization/_events.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/optimization/_optimizer.py` & `ropt-0.1.5/src/ropt/optimization/_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional, Tuple
 
 import numpy as np
 
 from ropt.enums import ConstraintType, OptimizerExitCode
-from ropt.exceptions import OptimizationAborted
+from ropt.exceptions import ConfigError, OptimizationAborted
 from ropt.results import (
     BoundConstraints,
     FunctionResults,
     GradientResults,
     LinearConstraints,
     NonlinearConstraints,
 )
@@ -59,15 +59,23 @@
 
     def _optimizer_callback(
         self,
         variables: NDArray[np.float64],
         *,
         return_functions: bool,
         return_gradients: bool,
+        allow_nan: bool = False,
     ) -> Tuple[NDArray[np.float64], NDArray[np.float64]]:
+        if (
+            self._enopt_config.realizations.realization_min_success < 1
+            and not allow_nan
+        ):
+            msg = "Failed function evaluations by the optimizer"
+            raise ConfigError(msg)
+
         assert return_functions or return_gradients
 
         self._check_stopping_criteria()
 
         variables = self._get_completed_variables(variables)
 
         # Run any nested steps, when this improves the objective, this may
```

### Comparing `ropt-0.1.4/src/ropt/optimization/_plan.py` & `ropt-0.1.5/src/ropt/optimization/_plan.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/__init__.py` & `ropt-0.1.5/src/ropt/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/_manager.py` & `ropt-0.1.5/src/ropt/plugins/_manager.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/function_transform/default.py` & `ropt-0.1.5/src/ropt/plugins/function_transform/default.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/function_transform/protocol.py` & `ropt-0.1.5/src/ropt/plugins/function_transform/protocol.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/optimization_steps/_utils.py` & `ropt-0.1.5/src/ropt/plugins/optimization_steps/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/optimization_steps/default.py` & `ropt-0.1.5/src/ropt/plugins/optimization_steps/default.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/optimization_steps/enopt_config.py` & `ropt-0.1.5/src/ropt/plugins/optimization_steps/enopt_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/optimization_steps/evaluator.py` & `ropt-0.1.5/src/ropt/plugins/optimization_steps/evaluator.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/optimization_steps/label.py` & `ropt-0.1.5/src/ropt/plugins/optimization_steps/label.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/optimization_steps/optimizer.py` & `ropt-0.1.5/src/ropt/plugins/optimization_steps/optimizer.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/optimization_steps/reset_tracker.py` & `ropt-0.1.5/src/ropt/plugins/optimization_steps/reset_tracker.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/optimization_steps/restart.py` & `ropt-0.1.5/src/ropt/plugins/optimization_steps/restart.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/optimization_steps/tracker.py` & `ropt-0.1.5/src/ropt/plugins/optimization_steps/tracker.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/optimization_steps/update_config.py` & `ropt-0.1.5/src/ropt/plugins/optimization_steps/update_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/optimizer/__init__.py` & `ropt-0.1.5/src/ropt/plugins/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/optimizer/protocol.py` & `ropt-0.1.5/src/ropt/plugins/optimizer/protocol.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,44 +30,52 @@
     def __call__(
         self,
         variables: NDArray[np.float64],
         /,
         *,
         return_functions: bool,
         return_gradients: bool,
+        allow_nan: bool = False,
     ) -> Tuple[NDArray[np.float64], NDArray[np.float64]]:
         """The signature of the optimizer callback.
 
         The optimizer callback expects a vector or matrix with variables to
         evaluate. Discrete optimizers may request function evaluations for
         multiple variable vectors, passed as the rows of a matrix.
         Gradient-based algorithms may currently only pass a single variable
         vector at a time.
 
         The `return_functions` and `return_gradients` flags determine whether
         functions and/or gradients are to be evaluated. The results are returned
         as a tuple of arrays, one for functions and constraints, the other for
-        gradients. If one of `return_functions` or `return_gradients` is `False`,
-        the corresponding result is an empty array.
+        gradients. If one of `return_functions` or `return_gradients` is
+        `False`, the corresponding result is an empty array.
 
         Multiple function evaluations are returned as a matrix where the rows
         are the result vectors for each evaluation. The first element of a
         result vector is the value of the objective value, and the remaining
         elements are the values of the non-linear constraints.
 
         The gradients of the objective function and the non-linear constraints
         are returned as a matrix. The first row contains the gradient of the
         objective function, while the remaining rows contain the gradients of
         the non-linear constraints. Gradient-based methods currently support
         only a single evaluation, hence there is also only a single result.
 
+        In most cases, the optimizer cannot handle failed function evaluations,
+        which are indicated by `NaN` values. Some optimizers, in particular
+        those that use multiple function evaluations do determine a next step
+        are robust in this regard. By returning `allow_nan=True`, these
+        optimizers can indicate that this is the case.
+
         Args:
-            variables:        The variable vector or matrix to evaluate.
-            return_functions: If `True`, evaluate and return functions.
-            return_gradients: If `True`, evaluate and return gradients.
+            variables:        The variable vector or matrix to evaluate
+            return_functions: If `True`, evaluate and return functions
+            return_gradients: If `True`, evaluate and return gradients
+            allow_nan:        If `True`, accept `NaN` values
 
         Returns:
             A tuple with function and gradient values.
         """
 
 
 class Optimizer(Protocol):
```

### Comparing `ropt-0.1.4/src/ropt/plugins/optimizer/scipy.py` & `ropt-0.1.5/src/ropt/plugins/optimizer/scipy.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/optimizer/utils.py` & `ropt-0.1.5/src/ropt/plugins/optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/realization_filter/__init__.py` & `ropt-0.1.5/src/ropt/plugins/realization_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/realization_filter/default.py` & `ropt-0.1.5/src/ropt/plugins/realization_filter/default.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/realization_filter/protocol.py` & `ropt-0.1.5/src/ropt/plugins/realization_filter/protocol.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/sampler/__init__.py` & `ropt-0.1.5/src/ropt/plugins/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/sampler/protocol.py` & `ropt-0.1.5/src/ropt/plugins/sampler/protocol.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/plugins/sampler/scipy.py` & `ropt-0.1.5/src/ropt/plugins/sampler/scipy.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/report/__init__.py` & `ropt-0.1.5/src/ropt/report/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/report/_data_frame.py` & `ropt-0.1.5/src/ropt/report/_data_frame.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/report/_table.py` & `ropt-0.1.5/src/ropt/report/_table.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/report/_utils.py` & `ropt-0.1.5/src/ropt/report/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/results/__init__.py` & `ropt-0.1.5/src/ropt/results/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/results/_bound_constraints.py` & `ropt-0.1.5/src/ropt/results/_bound_constraints.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/results/_function_evaluations.py` & `ropt-0.1.5/src/ropt/results/_function_evaluations.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/results/_function_results.py` & `ropt-0.1.5/src/ropt/results/_function_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/results/_functions.py` & `ropt-0.1.5/src/ropt/results/_functions.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/results/_gradient_evaluations.py` & `ropt-0.1.5/src/ropt/results/_gradient_evaluations.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/results/_gradient_results.py` & `ropt-0.1.5/src/ropt/results/_gradient_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/results/_gradients.py` & `ropt-0.1.5/src/ropt/results/_gradients.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/results/_linear_constraints.py` & `ropt-0.1.5/src/ropt/results/_linear_constraints.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/results/_maximize.py` & `ropt-0.1.5/src/ropt/results/_maximize.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/results/_nonlinear_constraints.py` & `ropt-0.1.5/src/ropt/results/_nonlinear_constraints.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/results/_pandas.py` & `ropt-0.1.5/src/ropt/results/_pandas.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/results/_realizations.py` & `ropt-0.1.5/src/ropt/results/_realizations.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/results/_result_field.py` & `ropt-0.1.5/src/ropt/results/_result_field.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/results/_results.py` & `ropt-0.1.5/src/ropt/results/_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/results/_utils.py` & `ropt-0.1.5/src/ropt/results/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/results/_xarray.py` & `ropt-0.1.5/src/ropt/results/_xarray.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/utils/_misc.py` & `ropt-0.1.5/src/ropt/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt/utils/scaling.py` & `ropt-0.1.5/src/ropt/utils/scaling.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/src/ropt.egg-info/PKG-INFO` & `ropt-0.1.5/src/ropt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ropt
-Version: 0.1.4
+Version: 0.1.5
 Summary: The ropt ensemble optimizer module
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ropt-0.1.4/src/ropt.egg-info/SOURCES.txt` & `ropt-0.1.5/src/ropt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/tests/conftest.py` & `ropt-0.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/tests/test_concurrent.py` & `ropt-0.1.5/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/tests/test_config.py` & `ropt-0.1.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/tests/test_ensemble_gradient.py` & `ropt-0.1.5/tests/test_ensemble_gradient.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/tests/test_examples.py` & `ropt-0.1.5/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/tests/test_failed_realizations.py` & `ropt-0.1.5/tests/test_failed_realizations.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/tests/test_function_transforms.py` & `ropt-0.1.5/tests/test_function_transforms.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/tests/test_netcdf.py` & `ropt-0.1.5/tests/test_netcdf.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/tests/test_optimizer.py` & `ropt-0.1.5/tests/test_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,27 @@
     functions = [lambda _0, _1: np.array(1.0), lambda _0, _1: np.array(np.nan)]
     optimizer = EnsembleOptimizer(evaluator(functions))
     optimizer.add_observer(EventType.FINISHED_EVALUATION, _observer)
     optimizer.add_observer(EventType.FINISHED_OPTIMIZER_STEP, handle_finished)
     optimizer.start_optimization(plan=[{"config": enopt_config}, {"optimizer": {}}])
 
 
+def test_all_failed_realizations_not_supported(
+    enopt_config: Any, evaluator: Any
+) -> None:
+    enopt_config["realizations"] = {"realization_min_success": 0}
+
+    functions = [lambda _0, _1: np.array(1.0), lambda _0, _1: np.array(np.nan)]
+    optimizer = EnsembleOptimizer(evaluator(functions))
+    with pytest.raises(
+        ConfigError, match="Failed function evaluations by the optimizer"
+    ):
+        optimizer.start_optimization(plan=[{"config": enopt_config}, {"optimizer": {}}])
+
+
 def test_user_abort(enopt_config: Any, evaluator: Any) -> None:
     last_evaluation = 100
 
     def _observer(event: OptimizationEvent, optimizer: EnsembleOptimizer) -> None:
         nonlocal last_evaluation
         assert event.results is not None
         last_evaluation = event.results[0].result_id
```

### Comparing `ropt-0.1.4/tests/test_pandas.py` & `ropt-0.1.5/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/tests/test_parsl.py` & `ropt-0.1.5/tests/test_parsl.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/tests/test_realization_filters.py` & `ropt-0.1.5/tests/test_realization_filters.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/tests/test_result_table.py` & `ropt-0.1.5/tests/test_result_table.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/tests/test_results.py` & `ropt-0.1.5/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/tests/test_results_data_frame.py` & `ropt-0.1.5/tests/test_results_data_frame.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/tests/test_samplers.py` & `ropt-0.1.5/tests/test_samplers.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/tests/test_scipy_backend.py` & `ropt-0.1.5/tests/test_scipy_backend.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/tests/test_scipy_samplers.py` & `ropt-0.1.5/tests/test_scipy_samplers.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.4/tests/test_xarray.py` & `ropt-0.1.5/tests/test_xarray.py`

 * *Files identical despite different names*


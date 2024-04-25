# Comparing `tmp/ropt-0.1.6.tar.gz` & `tmp/ropt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ropt-0.1.6.tar", last modified: Thu Apr 25 10:58:14 2024, max compression
+gzip compressed data, was "ropt-0.2.0.tar", last modified: Thu Apr 25 11:31:44 2024, max compression
```

## Comparing `ropt-0.1.6.tar` & `ropt-0.2.0.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.840336 ropt-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.808336 ropt-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.812336 ropt-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-25 10:58:09.000000 ropt-0.1.6/.github/workflows/build-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-25 10:58:09.000000 ropt-0.1.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-25 10:58:09.000000 ropt-0.1.6/.github/workflows/static-checks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-25 10:58:09.000000 ropt-0.1.6/.github/workflows/tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-04-25 10:58:09.000000 ropt-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 10:58:09.000000 ropt-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-25 10:58:14.840336 ropt-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-25 10:58:09.000000 ropt-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.816336 ropt-0.1.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-25 10:58:09.000000 ropt-0.1.6/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.816336 ropt-0.1.6/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-25 10:58:09.000000 ropt-0.1.6/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.816336 ropt-0.1.6/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-25 10:58:09.000000 ropt-0.1.6/docs/reference/enopt_config.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 10:58:09.000000 ropt-0.1.6/docs/reference/enums.md
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-25 10:58:09.000000 ropt-0.1.6/docs/reference/evaluator.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 10:58:09.000000 ropt-0.1.6/docs/reference/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-25 10:58:09.000000 ropt-0.1.6/docs/reference/function_transforms.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 10:58:09.000000 ropt-0.1.6/docs/reference/optimization.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 10:58:09.000000 ropt-0.1.6/docs/reference/optimization_steps.md
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-25 10:58:09.000000 ropt-0.1.6/docs/reference/optimizer_backends.md
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-25 10:58:09.000000 ropt-0.1.6/docs/reference/plan_config.md
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 10:58:09.000000 ropt-0.1.6/docs/reference/plugins.md
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-25 10:58:09.000000 ropt-0.1.6/docs/reference/realization_filters.md
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-25 10:58:09.000000 ropt-0.1.6/docs/reference/reporting.md
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-25 10:58:09.000000 ropt-0.1.6/docs/reference/results.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-25 10:58:09.000000 ropt-0.1.6/docs/reference/sampler_backends.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 10:58:09.000000 ropt-0.1.6/docs/reference/utilities.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.816336 ropt-0.1.6/docs/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-25 10:58:09.000000 ropt-0.1.6/docs/usage/robust_optimization.md
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-25 10:58:09.000000 ropt-0.1.6/docs/usage/running.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.820336 ropt-0.1.6/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-25 10:58:09.000000 ropt-0.1.6/examples/de_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-25 10:58:09.000000 ropt-0.1.6/examples/de_nonlinear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-25 10:58:09.000000 ropt-0.1.6/examples/rosenbrock_deterministic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-25 10:58:09.000000 ropt-0.1.6/examples/rosenbrock_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.820336 ropt-0.1.6/examples/script_optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-25 10:58:09.000000 ropt-0.1.6/examples/script_optimizer/rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-25 10:58:09.000000 ropt-0.1.6/examples/script_optimizer/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-25 10:58:09.000000 ropt-0.1.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-25 10:58:09.000000 ropt-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 10:58:14.840336 ropt-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.808336 ropt-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.820336 ropt-0.1.6/src/ropt/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.820336 ropt-0.1.6/src/ropt/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17499 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/apps/_script_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.820336 ropt-0.1.6/src/ropt/config/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.824336 ropt-0.1.6/src/ropt/config/enopt/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/enopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/enopt/_enopt_base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/enopt/_enopt_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/enopt/_function_transform_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/enopt/_gradient_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/enopt/_linear_constraints_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/enopt/_nonlinear_constraints_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/enopt/_objective_functions_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/enopt/_optimizer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/enopt/_realization_filter_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/enopt/_realizations_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/enopt/_sampler_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/enopt/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/enopt/_variables_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/enopt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.824336 ropt-0.1.6/src/ropt/config/plan/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/plan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/plan/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/plan/_plan_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/plan/_step_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.824336 ropt-0.1.6/src/ropt/evaluator/
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/evaluator/_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    25967 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/evaluator/_ensemble_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/evaluator/_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/evaluator/_evaluator_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/evaluator/_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/evaluator/_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/evaluator/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/evaluator/parsl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.828336 ropt-0.1.6/src/ropt/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/optimization/_bases.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/optimization/_ensemble_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/optimization/_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/optimization/_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/optimization/_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.828336 ropt-0.1.6/src/ropt/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.828336 ropt-0.1.6/src/ropt/plugins/function_transform/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/function_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/function_transform/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/function_transform/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.828336 ropt-0.1.6/src/ropt/plugins/optimization_steps/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/optimization_steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/optimization_steps/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/optimization_steps/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/optimization_steps/enopt_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/optimization_steps/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/optimization_steps/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/optimization_steps/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/optimization_steps/reset_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/optimization_steps/restart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/optimization_steps/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/optimization_steps/update_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.828336 ropt-0.1.6/src/ropt/plugins/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/optimizer/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    20113 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/optimizer/scipy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/optimizer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.832336 ropt-0.1.6/src/ropt/plugins/realization_filter/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/realization_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15031 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/realization_filter/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/realization_filter/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.832336 ropt-0.1.6/src/ropt/plugins/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/sampler/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/plugins/sampler/scipy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.832336 ropt-0.1.6/src/ropt/report/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/report/_data_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/report/_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/report/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.836336 ropt-0.1.6/src/ropt/results/
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/results/_bound_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/results/_function_evaluations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/results/_function_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/results/_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/results/_gradient_evaluations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/results/_gradient_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/results/_gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/results/_linear_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/results/_maximize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/results/_nonlinear_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/results/_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/results/_realizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/results/_result_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/results/_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/results/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/results/_xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.836336 ropt-0.1.6/src/ropt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/utils/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-25 10:58:09.000000 ropt-0.1.6/src/ropt/utils/scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 10:58:14.000000 ropt-0.1.6/src/ropt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.836336 ropt-0.1.6/src/ropt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-25 10:58:14.000000 ropt-0.1.6/src/ropt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-25 10:58:14.000000 ropt-0.1.6/src/ropt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 10:58:14.000000 ropt-0.1.6/src/ropt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-25 10:58:14.000000 ropt-0.1.6/src/ropt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 10:58:14.000000 ropt-0.1.6/src/ropt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:14.836336 ropt-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:09.000000 ropt-0.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-25 10:58:09.000000 ropt-0.1.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-25 10:58:09.000000 ropt-0.1.6/tests/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    25786 2024-04-25 10:58:09.000000 ropt-0.1.6/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-25 10:58:09.000000 ropt-0.1.6/tests/test_ensemble_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-25 10:58:09.000000 ropt-0.1.6/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-25 10:58:09.000000 ropt-0.1.6/tests/test_failed_realizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-25 10:58:09.000000 ropt-0.1.6/tests/test_function_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-25 10:58:09.000000 ropt-0.1.6/tests/test_netcdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    43207 2024-04-25 10:58:09.000000 ropt-0.1.6/tests/test_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-04-25 10:58:09.000000 ropt-0.1.6/tests/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-04-25 10:58:09.000000 ropt-0.1.6/tests/test_parsl.py
--rw-r--r--   0 runner    (1001) docker     (127)    27696 2024-04-25 10:58:09.000000 ropt-0.1.6/tests/test_realization_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-04-25 10:58:09.000000 ropt-0.1.6/tests/test_result_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-04-25 10:58:09.000000 ropt-0.1.6/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-25 10:58:09.000000 ropt-0.1.6/tests/test_results_data_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-25 10:58:09.000000 ropt-0.1.6/tests/test_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19164 2024-04-25 10:58:09.000000 ropt-0.1.6/tests/test_scipy_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-25 10:58:09.000000 ropt-0.1.6/tests/test_scipy_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-25 10:58:09.000000 ropt-0.1.6/tests/test_xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.476220 ropt-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.444220 ropt-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.448220 ropt-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-25 11:31:38.000000 ropt-0.2.0/.github/workflows/build-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-25 11:31:38.000000 ropt-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-25 11:31:38.000000 ropt-0.2.0/.github/workflows/static-checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-25 11:31:38.000000 ropt-0.2.0/.github/workflows/tests.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-04-25 11:31:38.000000 ropt-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 11:31:38.000000 ropt-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-25 11:31:44.476220 ropt-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-25 11:31:38.000000 ropt-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.448220 ropt-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-25 11:31:38.000000 ropt-0.2.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.448220 ropt-0.2.0/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-25 11:31:38.000000 ropt-0.2.0/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.448220 ropt-0.2.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-25 11:31:38.000000 ropt-0.2.0/docs/reference/enopt_config.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 11:31:38.000000 ropt-0.2.0/docs/reference/enums.md
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-25 11:31:38.000000 ropt-0.2.0/docs/reference/evaluator.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 11:31:38.000000 ropt-0.2.0/docs/reference/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-25 11:31:38.000000 ropt-0.2.0/docs/reference/function_transforms.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 11:31:38.000000 ropt-0.2.0/docs/reference/optimization.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 11:31:38.000000 ropt-0.2.0/docs/reference/optimization_steps.md
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-25 11:31:38.000000 ropt-0.2.0/docs/reference/optimizer_backends.md
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-25 11:31:38.000000 ropt-0.2.0/docs/reference/plan_config.md
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 11:31:38.000000 ropt-0.2.0/docs/reference/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-25 11:31:38.000000 ropt-0.2.0/docs/reference/realization_filters.md
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-25 11:31:38.000000 ropt-0.2.0/docs/reference/reporting.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-25 11:31:38.000000 ropt-0.2.0/docs/reference/results.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-25 11:31:38.000000 ropt-0.2.0/docs/reference/sampler_backends.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 11:31:38.000000 ropt-0.2.0/docs/reference/utilities.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.448220 ropt-0.2.0/docs/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-25 11:31:38.000000 ropt-0.2.0/docs/usage/robust_optimization.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-25 11:31:38.000000 ropt-0.2.0/docs/usage/running.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.452220 ropt-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-25 11:31:38.000000 ropt-0.2.0/examples/de_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-25 11:31:38.000000 ropt-0.2.0/examples/de_nonlinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-25 11:31:38.000000 ropt-0.2.0/examples/rosenbrock_deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-25 11:31:38.000000 ropt-0.2.0/examples/rosenbrock_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.452220 ropt-0.2.0/examples/script_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-25 11:31:38.000000 ropt-0.2.0/examples/script_optimizer/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-25 11:31:38.000000 ropt-0.2.0/examples/script_optimizer/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-25 11:31:38.000000 ropt-0.2.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-25 11:31:38.000000 ropt-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 11:31:44.476220 ropt-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.444220 ropt-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.452220 ropt-0.2.0/src/ropt/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.452220 ropt-0.2.0/src/ropt/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17499 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/apps/_script_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.452220 ropt-0.2.0/src/ropt/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.456220 ropt-0.2.0/src/ropt/config/enopt/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/enopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/enopt/_enopt_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/enopt/_enopt_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/enopt/_function_transform_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/enopt/_gradient_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/enopt/_linear_constraints_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/enopt/_nonlinear_constraints_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/enopt/_objective_functions_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/enopt/_optimizer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/enopt/_realization_filter_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/enopt/_realizations_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/enopt/_sampler_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/enopt/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/enopt/_variables_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/enopt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.456220 ropt-0.2.0/src/ropt/config/plan/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/plan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/plan/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/plan/_plan_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/plan/_step_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.460220 ropt-0.2.0/src/ropt/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/evaluator/_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25967 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/evaluator/_ensemble_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/evaluator/_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/evaluator/_evaluator_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/evaluator/_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/evaluator/_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/evaluator/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/evaluator/parsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.460220 ropt-0.2.0/src/ropt/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/optimization/_bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/optimization/_ensemble_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/optimization/_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/optimization/_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/optimization/_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.460220 ropt-0.2.0/src/ropt/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.460220 ropt-0.2.0/src/ropt/plugins/function_transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/function_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/function_transform/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/function_transform/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.464220 ropt-0.2.0/src/ropt/plugins/optimization_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/optimization_steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/optimization_steps/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/optimization_steps/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/optimization_steps/enopt_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/optimization_steps/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/optimization_steps/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/optimization_steps/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/optimization_steps/reset_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/optimization_steps/restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/optimization_steps/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/optimization_steps/update_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.464220 ropt-0.2.0/src/ropt/plugins/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/optimizer/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20113 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/optimizer/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/optimizer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.464220 ropt-0.2.0/src/ropt/plugins/realization_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/realization_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15031 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/realization_filter/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/realization_filter/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.464220 ropt-0.2.0/src/ropt/plugins/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/sampler/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/plugins/sampler/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.464220 ropt-0.2.0/src/ropt/report/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/report/_data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/report/_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/report/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.468220 ropt-0.2.0/src/ropt/results/
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/results/_bound_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/results/_function_evaluations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/results/_function_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/results/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/results/_gradient_evaluations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/results/_gradient_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/results/_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/results/_linear_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/results/_maximize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/results/_nonlinear_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/results/_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/results/_realizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/results/_result_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/results/_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/results/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/results/_xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.468220 ropt-0.2.0/src/ropt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/utils/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-25 11:31:38.000000 ropt-0.2.0/src/ropt/utils/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 11:31:44.000000 ropt-0.2.0/src/ropt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.472220 ropt-0.2.0/src/ropt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-25 11:31:44.000000 ropt-0.2.0/src/ropt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-25 11:31:44.000000 ropt-0.2.0/src/ropt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 11:31:44.000000 ropt-0.2.0/src/ropt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-25 11:31:44.000000 ropt-0.2.0/src/ropt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 11:31:44.000000 ropt-0.2.0/src/ropt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:44.472220 ropt-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:31:38.000000 ropt-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-25 11:31:38.000000 ropt-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-25 11:31:38.000000 ropt-0.2.0/tests/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25786 2024-04-25 11:31:38.000000 ropt-0.2.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-25 11:31:38.000000 ropt-0.2.0/tests/test_ensemble_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-25 11:31:38.000000 ropt-0.2.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-25 11:31:38.000000 ropt-0.2.0/tests/test_failed_realizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-25 11:31:38.000000 ropt-0.2.0/tests/test_function_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-25 11:31:38.000000 ropt-0.2.0/tests/test_netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43207 2024-04-25 11:31:38.000000 ropt-0.2.0/tests/test_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-04-25 11:31:38.000000 ropt-0.2.0/tests/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-04-25 11:31:38.000000 ropt-0.2.0/tests/test_parsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27696 2024-04-25 11:31:38.000000 ropt-0.2.0/tests/test_realization_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-04-25 11:31:38.000000 ropt-0.2.0/tests/test_result_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-04-25 11:31:38.000000 ropt-0.2.0/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-25 11:31:38.000000 ropt-0.2.0/tests/test_results_data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-25 11:31:38.000000 ropt-0.2.0/tests/test_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19164 2024-04-25 11:31:38.000000 ropt-0.2.0/tests/test_scipy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-25 11:31:38.000000 ropt-0.2.0/tests/test_scipy_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-25 11:31:38.000000 ropt-0.2.0/tests/test_xarray.py
```

### Comparing `ropt-0.1.6/.github/workflows/build-docs.yml` & `ropt-0.2.0/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/.github/workflows/release.yml` & `ropt-0.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/.github/workflows/static-checks.yml` & `ropt-0.2.0/.github/workflows/static-checks.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/.github/workflows/tests.yml` & `ropt-0.2.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/LICENSE` & `ropt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/PKG-INFO` & `ropt-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ropt
-Version: 0.1.6
+Version: 0.2.0
 Summary: The ropt ensemble optimizer module
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ropt-0.1.6/README.md` & `ropt-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/docs/index.md` & `ropt-0.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/docs/reference/evaluator.md` & `ropt-0.2.0/docs/reference/evaluator.md`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/docs/reference/realization_filters.md` & `ropt-0.2.0/docs/reference/realization_filters.md`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/docs/reference/results.md` & `ropt-0.2.0/docs/reference/results.md`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/docs/usage/robust_optimization.md` & `ropt-0.2.0/docs/usage/robust_optimization.md`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/docs/usage/running.md` & `ropt-0.2.0/docs/usage/running.md`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/examples/de_linear.py` & `ropt-0.2.0/examples/de_linear.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/examples/de_nonlinear.py` & `ropt-0.2.0/examples/de_nonlinear.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/examples/rosenbrock_deterministic.py` & `ropt-0.2.0/examples/rosenbrock_deterministic.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/examples/rosenbrock_ensemble.py` & `ropt-0.2.0/examples/rosenbrock_ensemble.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/examples/script_optimizer/rosenbrock.py` & `ropt-0.2.0/examples/script_optimizer/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/examples/script_optimizer/run.py` & `ropt-0.2.0/examples/script_optimizer/run.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/mkdocs.yml` & `ropt-0.2.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/pyproject.toml` & `ropt-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/apps/_script_optimizer.py` & `ropt-0.2.0/src/ropt/apps/_script_optimizer.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/config/enopt/__init__.py` & `ropt-0.2.0/src/ropt/config/enopt/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/config/enopt/_enopt_config.py` & `ropt-0.2.0/src/ropt/config/enopt/_enopt_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/config/enopt/_function_transform_config.py` & `ropt-0.2.0/src/ropt/config/enopt/_function_transform_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/config/enopt/_gradient_config.py` & `ropt-0.2.0/src/ropt/config/enopt/_gradient_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/config/enopt/_linear_constraints_config.py` & `ropt-0.2.0/src/ropt/config/enopt/_linear_constraints_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/config/enopt/_nonlinear_constraints_config.py` & `ropt-0.2.0/src/ropt/config/enopt/_nonlinear_constraints_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/config/enopt/_objective_functions_config.py` & `ropt-0.2.0/src/ropt/config/enopt/_objective_functions_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/config/enopt/_optimizer_config.py` & `ropt-0.2.0/src/ropt/config/enopt/_optimizer_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/config/enopt/_realization_filter_config.py` & `ropt-0.2.0/src/ropt/config/enopt/_realization_filter_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/config/enopt/_realizations_config.py` & `ropt-0.2.0/src/ropt/config/enopt/_realizations_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/config/enopt/_sampler_config.py` & `ropt-0.2.0/src/ropt/config/enopt/_sampler_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/config/enopt/_utils.py` & `ropt-0.2.0/src/ropt/config/enopt/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/config/enopt/_variables_config.py` & `ropt-0.2.0/src/ropt/config/enopt/_variables_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/config/enopt/constants.py` & `ropt-0.2.0/src/ropt/config/enopt/constants.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/config/plan/__init__.py` & `ropt-0.2.0/src/ropt/config/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/config/plan/_config.py` & `ropt-0.2.0/src/ropt/config/plan/_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/config/plan/_plan_config.py` & `ropt-0.2.0/src/ropt/config/plan/_plan_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/config/plan/_step_config.py` & `ropt-0.2.0/src/ropt/config/plan/_step_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/config/utils.py` & `ropt-0.2.0/src/ropt/config/utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/enums.py` & `ropt-0.2.0/src/ropt/enums.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/evaluator/__init__.py` & `ropt-0.2.0/src/ropt/evaluator/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/evaluator/_concurrent.py` & `ropt-0.2.0/src/ropt/evaluator/_concurrent.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/evaluator/_ensemble_evaluator.py` & `ropt-0.2.0/src/ropt/evaluator/_ensemble_evaluator.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/evaluator/_evaluator.py` & `ropt-0.2.0/src/ropt/evaluator/_evaluator.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/evaluator/_evaluator_results.py` & `ropt-0.2.0/src/ropt/evaluator/_evaluator_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/evaluator/_function.py` & `ropt-0.2.0/src/ropt/evaluator/_function.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/evaluator/_gradient.py` & `ropt-0.2.0/src/ropt/evaluator/_gradient.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/evaluator/_utils.py` & `ropt-0.2.0/src/ropt/evaluator/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/evaluator/parsl.py` & `ropt-0.2.0/src/ropt/evaluator/parsl.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/events.py` & `ropt-0.2.0/src/ropt/events.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/exceptions.py` & `ropt-0.2.0/src/ropt/exceptions.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/optimization/_bases.py` & `ropt-0.2.0/src/ropt/optimization/_bases.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/optimization/_ensemble_optimizer.py` & `ropt-0.2.0/src/ropt/optimization/_ensemble_optimizer.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/optimization/_events.py` & `ropt-0.2.0/src/ropt/optimization/_events.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/optimization/_optimizer.py` & `ropt-0.2.0/src/ropt/optimization/_optimizer.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/optimization/_plan.py` & `ropt-0.2.0/src/ropt/optimization/_plan.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/__init__.py` & `ropt-0.2.0/src/ropt/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/_manager.py` & `ropt-0.2.0/src/ropt/plugins/_manager.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/function_transform/default.py` & `ropt-0.2.0/src/ropt/plugins/function_transform/default.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/function_transform/protocol.py` & `ropt-0.2.0/src/ropt/plugins/function_transform/protocol.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/optimization_steps/_utils.py` & `ropt-0.2.0/src/ropt/plugins/optimization_steps/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/optimization_steps/default.py` & `ropt-0.2.0/src/ropt/plugins/optimization_steps/default.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/optimization_steps/enopt_config.py` & `ropt-0.2.0/src/ropt/plugins/optimization_steps/enopt_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/optimization_steps/evaluator.py` & `ropt-0.2.0/src/ropt/plugins/optimization_steps/evaluator.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/optimization_steps/label.py` & `ropt-0.2.0/src/ropt/plugins/optimization_steps/label.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/optimization_steps/optimizer.py` & `ropt-0.2.0/src/ropt/plugins/optimization_steps/optimizer.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/optimization_steps/reset_tracker.py` & `ropt-0.2.0/src/ropt/plugins/optimization_steps/reset_tracker.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/optimization_steps/restart.py` & `ropt-0.2.0/src/ropt/plugins/optimization_steps/restart.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/optimization_steps/tracker.py` & `ropt-0.2.0/src/ropt/plugins/optimization_steps/tracker.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/optimization_steps/update_config.py` & `ropt-0.2.0/src/ropt/plugins/optimization_steps/update_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/optimizer/__init__.py` & `ropt-0.2.0/src/ropt/plugins/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/optimizer/protocol.py` & `ropt-0.2.0/src/ropt/plugins/optimizer/protocol.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/optimizer/scipy.py` & `ropt-0.2.0/src/ropt/plugins/optimizer/scipy.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/optimizer/utils.py` & `ropt-0.2.0/src/ropt/plugins/optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/realization_filter/__init__.py` & `ropt-0.2.0/src/ropt/plugins/realization_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/realization_filter/default.py` & `ropt-0.2.0/src/ropt/plugins/realization_filter/default.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/realization_filter/protocol.py` & `ropt-0.2.0/src/ropt/plugins/realization_filter/protocol.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/sampler/__init__.py` & `ropt-0.2.0/src/ropt/plugins/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/sampler/protocol.py` & `ropt-0.2.0/src/ropt/plugins/sampler/protocol.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/plugins/sampler/scipy.py` & `ropt-0.2.0/src/ropt/plugins/sampler/scipy.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/report/__init__.py` & `ropt-0.2.0/src/ropt/report/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/report/_data_frame.py` & `ropt-0.2.0/src/ropt/report/_data_frame.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/report/_table.py` & `ropt-0.2.0/src/ropt/report/_table.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/report/_utils.py` & `ropt-0.2.0/src/ropt/report/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/results/__init__.py` & `ropt-0.2.0/src/ropt/results/__init__.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/results/_bound_constraints.py` & `ropt-0.2.0/src/ropt/results/_bound_constraints.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/results/_function_evaluations.py` & `ropt-0.2.0/src/ropt/results/_function_evaluations.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/results/_function_results.py` & `ropt-0.2.0/src/ropt/results/_function_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/results/_functions.py` & `ropt-0.2.0/src/ropt/results/_functions.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/results/_gradient_evaluations.py` & `ropt-0.2.0/src/ropt/results/_gradient_evaluations.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/results/_gradient_results.py` & `ropt-0.2.0/src/ropt/results/_gradient_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/results/_gradients.py` & `ropt-0.2.0/src/ropt/results/_gradients.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/results/_linear_constraints.py` & `ropt-0.2.0/src/ropt/results/_linear_constraints.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/results/_maximize.py` & `ropt-0.2.0/src/ropt/results/_maximize.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/results/_nonlinear_constraints.py` & `ropt-0.2.0/src/ropt/results/_nonlinear_constraints.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/results/_pandas.py` & `ropt-0.2.0/src/ropt/results/_pandas.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/results/_realizations.py` & `ropt-0.2.0/src/ropt/results/_realizations.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/results/_result_field.py` & `ropt-0.2.0/src/ropt/results/_result_field.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/results/_results.py` & `ropt-0.2.0/src/ropt/results/_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/results/_utils.py` & `ropt-0.2.0/src/ropt/results/_utils.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/results/_xarray.py` & `ropt-0.2.0/src/ropt/results/_xarray.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/utils/_misc.py` & `ropt-0.2.0/src/ropt/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt/utils/scaling.py` & `ropt-0.2.0/src/ropt/utils/scaling.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/src/ropt.egg-info/PKG-INFO` & `ropt-0.2.0/src/ropt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ropt
-Version: 0.1.6
+Version: 0.2.0
 Summary: The ropt ensemble optimizer module
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ropt-0.1.6/src/ropt.egg-info/SOURCES.txt` & `ropt-0.2.0/src/ropt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/tests/conftest.py` & `ropt-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/tests/test_concurrent.py` & `ropt-0.2.0/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/tests/test_config.py` & `ropt-0.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/tests/test_ensemble_gradient.py` & `ropt-0.2.0/tests/test_ensemble_gradient.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/tests/test_examples.py` & `ropt-0.2.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/tests/test_failed_realizations.py` & `ropt-0.2.0/tests/test_failed_realizations.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/tests/test_function_transforms.py` & `ropt-0.2.0/tests/test_function_transforms.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/tests/test_netcdf.py` & `ropt-0.2.0/tests/test_netcdf.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/tests/test_optimizer.py` & `ropt-0.2.0/tests/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/tests/test_pandas.py` & `ropt-0.2.0/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/tests/test_parsl.py` & `ropt-0.2.0/tests/test_parsl.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/tests/test_realization_filters.py` & `ropt-0.2.0/tests/test_realization_filters.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/tests/test_result_table.py` & `ropt-0.2.0/tests/test_result_table.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/tests/test_results.py` & `ropt-0.2.0/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/tests/test_results_data_frame.py` & `ropt-0.2.0/tests/test_results_data_frame.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/tests/test_samplers.py` & `ropt-0.2.0/tests/test_samplers.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/tests/test_scipy_backend.py` & `ropt-0.2.0/tests/test_scipy_backend.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/tests/test_scipy_samplers.py` & `ropt-0.2.0/tests/test_scipy_samplers.py`

 * *Files identical despite different names*

### Comparing `ropt-0.1.6/tests/test_xarray.py` & `ropt-0.2.0/tests/test_xarray.py`

 * *Files identical despite different names*


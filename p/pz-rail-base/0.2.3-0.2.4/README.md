# Comparing `tmp/pz-rail-base-0.2.3.tar.gz` & `tmp/pz_rail_base-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-base-0.2.3.tar", last modified: Tue Apr  9 18:21:35 2024, max compression
+gzip compressed data, was "pz_rail_base-0.2.4.tar", last modified: Thu Apr 25 00:36:37 2024, max compression
```

## Comparing `pz-rail-base-0.2.3.tar` & `pz_rail_base-0.2.4.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.122435 pz-rail-base-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.090434 pz-rail-base-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.090434 pz-rail-base-0.2.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.090434 pz-rail-base-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-09 18:21:35.122435 pz-rail-base-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/rail_packages.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 18:21:35.122435 pz-rail-base-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.082434 pz-rail-base-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.118435 pz-rail-base-0.2.3/src/pz_rail_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-09 18:21:35.000000 pz-rail-base-0.2.3/src/pz_rail_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-09 18:21:35.000000 pz-rail-base-0.2.3/src/pz_rail_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:21:35.000000 pz-rail-base-0.2.3/src/pz_rail_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-09 18:21:35.000000 pz-rail-base-0.2.3/src/pz_rail_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 18:21:35.000000 pz-rail-base-0.2.3/src/pz_rail_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 18:21:35.000000 pz-rail-base-0.2.3/src/pz_rail_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.086434 pz-rail-base-0.2.3/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.090434 pz-rail-base-0.2.3/src/rail/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/cli/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.094434 pz-rail-base-0.2.3/src/rail/core/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 18:21:34.000000 pz-rail-base-0.2.3/src/rail/core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/core/algo_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/core/common_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    25183 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/core/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/core/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/core/point_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14637 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/core/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/core/util_stages.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.094434 pz-rail-base-0.2.3/src/rail/creation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.094434 pz-rail-base-0.2.3/src/rail/creation/degradation/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/creation/degradation/addRandom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/creation/degradation/quantityCut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/creation/degrader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/creation/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/creation/noisifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/creation/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.094434 pz-rail-base-0.2.3/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.094434 pz-rail-base-0.2.3/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/algos/equal_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/algos/naive_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/algos/point_est_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/algos/random_gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/algos/train_z.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/algos/uniform_binning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/algos/var_inf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/informer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/estimation/summarizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.098435 pz-rail-base-0.2.3/src/rail/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/evaluation/dist_to_dist_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/evaluation/dist_to_point_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/evaluation/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.098435 pz-rail-base-0.2.3/src/rail/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/evaluation/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/evaluation/metrics/cdeloss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/evaluation/metrics/pointestimates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/evaluation/point_to_point_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21261 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/evaluation/single_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/evaluation/stats_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.098435 pz-rail-base-0.2.3/src/rail/examples_data/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.086434 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.098435 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/configs/flowModeler.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.098435 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.102434 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_I_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1000000 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)   431705 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.086434 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.102434 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.102434 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/AB/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/AB/dummy.txt
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.102434 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/
--rw-r--r--   0 runner    (1001) docker     (127)    98003 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res
--rw-r--r--   0 runner    (1001) docker     (127)    95326 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res
--rw-r--r--   0 runner    (1001) docker     (127)    96635 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res
--rw-r--r--   0 runner    (1001) docker     (127)    90216 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res
--rw-r--r--   0 runner    (1001) docker     (127)   100126 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res
--rw-r--r--   0 runner    (1001) docker     (127)    93013 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.106434 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/CWWSB4.list
--rwxr-xr-x   0 runner    (1001) docker     (127)    43750 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    42830 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    72228 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    68560 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    43351 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    42789 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)   179585 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)   179584 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.106434 pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.106434 pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.110435 pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1158108 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   873947 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/goldenspike.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.118435 pz-rail-base-0.2.3/src/rail/examples_data/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    91936 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/lsst_filters.npy
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/make_rail_sample_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    43200 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/output_BPZ_lite.fits
--rw-r--r--   0 runner    (1001) docker     (127)    37192 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/output_BPZ_lite.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)    24574 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq
--rw-r--r--   0 runner    (1001) docker     (127)   662976 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)   873930 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/test_dc2_training_9816.pq
--rw-r--r--   0 runner    (1001) docker     (127)  1192254 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq
--rw-r--r--   0 runner    (1001) docker     (127)  1316984 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/training_100gal.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/examples_data/testdata/validation_10gal.hdf5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.118435 pz-rail-base-0.2.3/src/rail/stages/
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/src/rail/stages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.086434 pz-rail-base-0.2.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.118435 pz-rail-base-0.2.3/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/cli/hello_world.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/cli/single_number.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/cli/test_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.118435 pz-rail-base-0.2.3/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/core/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/core/test_introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/core/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/core/test_point_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.118435 pz-rail-base-0.2.3/tests/creation/
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/creation/test_degraders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.118435 pz-rail-base-0.2.3/tests/estimation/
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/estimation/test_algos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/estimation/test_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/estimation/test_summarizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:21:35.118435 pz-rail-base-0.2.3/tests/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-09 18:21:28.000000 pz-rail-base-0.2.3/tests/evaluation/test_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.484645 pz_rail_base-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.484645 pz_rail_base-0.2.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.488645 pz_rail_base-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/rail_packages.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.480645 pz_rail_base-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/src/pz_rail_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-25 00:36:37.000000 pz_rail_base-0.2.4/src/pz_rail_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-25 00:36:37.000000 pz_rail_base-0.2.4/src/pz_rail_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 00:36:37.000000 pz_rail_base-0.2.4/src/pz_rail_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-25 00:36:37.000000 pz_rail_base-0.2.4/src/pz_rail_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-25 00:36:37.000000 pz_rail_base-0.2.4/src/pz_rail_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 00:36:37.000000 pz_rail_base-0.2.4/src/pz_rail_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.484645 pz_rail_base-0.2.4/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.488645 pz_rail_base-0.2.4/src/rail/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/cli/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.488645 pz_rail_base-0.2.4/src/rail/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 00:36:37.000000 pz_rail_base-0.2.4/src/rail/core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/core/algo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/core/common_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25183 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/core/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/core/point_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14637 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/core/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/core/util_stages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.488645 pz_rail_base-0.2.4/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.492645 pz_rail_base-0.2.4/src/rail/creation/degradation/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/creation/degradation/addRandom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/creation/degradation/quantityCut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/creation/degrader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/creation/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/creation/noisifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/creation/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.492645 pz_rail_base-0.2.4/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.492645 pz_rail_base-0.2.4/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/algos/equal_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/algos/naive_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/algos/point_est_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/algos/random_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/algos/train_z.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/algos/uniform_binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/algos/var_inf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/informer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/summarizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.492645 pz_rail_base-0.2.4/src/rail/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/evaluation/dist_to_dist_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/evaluation/dist_to_point_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/evaluation/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.492645 pz_rail_base-0.2.4/src/rail/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/evaluation/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/evaluation/metrics/cdeloss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/evaluation/metrics/pointestimates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/evaluation/point_to_point_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21261 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/evaluation/single_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/evaluation/stats_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.492645 pz_rail_base-0.2.4/src/rail/examples_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.480645 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.492645 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/configs/flowModeler.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.492645 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.496645 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_I_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1000000 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   431705 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.480645 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.496645 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.496645 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/AB/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/AB/dummy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.500645 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/
+-rw-r--r--   0 runner    (1001) docker     (127)    98003 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res
+-rw-r--r--   0 runner    (1001) docker     (127)    95326 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res
+-rw-r--r--   0 runner    (1001) docker     (127)    96635 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res
+-rw-r--r--   0 runner    (1001) docker     (127)    90216 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res
+-rw-r--r--   0 runner    (1001) docker     (127)   100126 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res
+-rw-r--r--   0 runner    (1001) docker     (127)    93013 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.500645 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/CWWSB4.list
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43750 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42830 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    72228 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    68560 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43351 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42789 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179585 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179584 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.500645 pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.500645 pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.504645 pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1158108 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   873947 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/goldenspike.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/src/rail/examples_data/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    91936 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/lsst_filters.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/make_rail_sample_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    43200 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/output_BPZ_lite.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    37192 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/output_BPZ_lite.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)    24574 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq
+-rw-r--r--   0 runner    (1001) docker     (127)   662976 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)   873930 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/test_dc2_training_9816.pq
+-rw-r--r--   0 runner    (1001) docker     (127)  1192254 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq
+-rw-r--r--   0 runner    (1001) docker     (127)  1316984 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/training_100gal.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/validation_10gal.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/src/rail/stages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/stages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.484645 pz_rail_base-0.2.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/cli/hello_world.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/cli/single_number.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/cli/test_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/core/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/core/test_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/core/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/core/test_point_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/tests/creation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/creation/test_degraders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/tests/estimation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/estimation/test_algos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/estimation/test_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/estimation/test_summarizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/tests/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/evaluation/test_evaluation.py
```

### Comparing `pz-rail-base-0.2.3/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_base-0.2.4/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_base-0.2.4/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/.github/pull_request_template.md` & `pz_rail_base-0.2.4/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/.github/workflows/linting.yml` & `pz_rail_base-0.2.4/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/.github/workflows/publish-to-pypi.yml` & `pz_rail_base-0.2.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/.github/workflows/smoke-test.yml` & `pz_rail_base-0.2.4/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/.github/workflows/testing-and-coverage.yml` & `pz_rail_base-0.2.4/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/.gitignore` & `pz_rail_base-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/.pre-commit-config.yaml` & `pz_rail_base-0.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/LICENSE` & `pz_rail_base-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/PKG-INFO` & `pz_rail_base-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-base
-Version: 0.2.3
+Version: 0.2.4
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-base-0.2.3/README.md` & `pz_rail_base-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/pyproject.toml` & `pz_rail_base-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/pz_rail_base.egg-info/PKG-INFO` & `pz_rail_base-0.2.4/src/pz_rail_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-base
-Version: 0.2.3
+Version: 0.2.4
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-base-0.2.3/src/pz_rail_base.egg-info/SOURCES.txt` & `pz_rail_base-0.2.4/src/pz_rail_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/cli/commands.py` & `pz_rail_base-0.2.4/src/rail/cli/commands.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/cli/options.py` & `pz_rail_base-0.2.4/src/rail/cli/options.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/cli/scripts.py` & `pz_rail_base-0.2.4/src/rail/cli/scripts.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/core/__init__.py` & `pz_rail_base-0.2.4/src/rail/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/core/algo_utils.py` & `pz_rail_base-0.2.4/src/rail/core/algo_utils.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/core/common_params.py` & `pz_rail_base-0.2.4/src/rail/core/common_params.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/core/data.py` & `pz_rail_base-0.2.4/src/rail/core/data.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/core/introspection.py` & `pz_rail_base-0.2.4/src/rail/core/introspection.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/core/point_estimation.py` & `pz_rail_base-0.2.4/src/rail/core/point_estimation.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/core/stage.py` & `pz_rail_base-0.2.4/src/rail/core/stage.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/core/util_stages.py` & `pz_rail_base-0.2.4/src/rail/core/util_stages.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/core/utils.py` & `pz_rail_base-0.2.4/src/rail/core/utils.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/creation/degradation/addRandom.py` & `pz_rail_base-0.2.4/src/rail/creation/degradation/addRandom.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/creation/degradation/quantityCut.py` & `pz_rail_base-0.2.4/src/rail/creation/degradation/quantityCut.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/creation/degrader.py` & `pz_rail_base-0.2.4/src/rail/creation/degrader.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/creation/engine.py` & `pz_rail_base-0.2.4/src/rail/creation/engine.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/creation/noisifier.py` & `pz_rail_base-0.2.4/src/rail/creation/noisifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 The key feature here is the run adds noise to the catalog. 
 Intended subclasses are noisifier that adds LSST noise / other telescope noise
 """
 
 from rail.core.stage import RailStage
 from rail.core.data import PqHandle
-
+from ceci.config import StageParameter as Param
 
 class Noisifier(RailStage):
     """Base class Noisifier, which adds noise to the input catalog
 
     Noisifier take "input" data in the form of pandas dataframes in Parquet 
     files and provide as "output" another pandas dataframes written to Parquet 
     files.
     """
 
     name = 'Noisifier'
     config_options = RailStage.config_options.copy()
-    config_options.update(seed=1337)
+    config_options.update(
+        seed=Param(default=None, required=False, msg="Set to an `int` to force reproducible results."),
+    )
     inputs = [('input', PqHandle)]
     outputs = [('output', PqHandle)]
 
     def __init__(self, args, comm=None):
         """Initialize Noisifier that can add noise to photometric data"""
         RailStage.__init__(self, args, comm=comm)
```

### Comparing `pz-rail-base-0.2.3/src/rail/creation/selector.py` & `pz_rail_base-0.2.4/src/rail/creation/selector.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     files.
     """
 
     name = 'Selector'
     config_options = RailStage.config_options.copy()
     config_options.update(
         drop_rows=Param(bool, True, msg="Drop selected rows from output table"),
+        seed=Param(default=None, required=False, msg="Set to an `int` to force reproducible results."),
     )
     inputs = [('input', PqHandle)]
     outputs = [('output', PqHandle)]
 
     def __init__(self, args, comm=None):
         """Initialize Noisifier that can add noise to photometric data"""
         RailStage.__init__(self, args, comm=comm)
```

### Comparing `pz-rail-base-0.2.3/src/rail/estimation/algos/equal_count.py` & `pz_rail_base-0.2.4/src/rail/estimation/algos/equal_count.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/estimation/algos/naive_stack.py` & `pz_rail_base-0.2.4/src/rail/estimation/algos/naive_stack.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/estimation/algos/point_est_hist.py` & `pz_rail_base-0.2.4/src/rail/estimation/algos/point_est_hist.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/estimation/algos/random_gauss.py` & `pz_rail_base-0.2.4/src/rail/estimation/algos/random_gauss.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/estimation/algos/train_z.py` & `pz_rail_base-0.2.4/src/rail/estimation/algos/train_z.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/estimation/algos/uniform_binning.py` & `pz_rail_base-0.2.4/src/rail/estimation/algos/uniform_binning.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/estimation/algos/var_inf.py` & `pz_rail_base-0.2.4/src/rail/estimation/algos/var_inf.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/estimation/classifier.py` & `pz_rail_base-0.2.4/src/rail/estimation/classifier.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/estimation/estimator.py` & `pz_rail_base-0.2.4/src/rail/estimation/estimator.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/estimation/informer.py` & `pz_rail_base-0.2.4/src/rail/estimation/informer.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/estimation/summarizer.py` & `pz_rail_base-0.2.4/src/rail/estimation/summarizer.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/evaluation/dist_to_dist_evaluator.py` & `pz_rail_base-0.2.4/src/rail/evaluation/dist_to_dist_evaluator.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/evaluation/dist_to_point_evaluator.py` & `pz_rail_base-0.2.4/src/rail/evaluation/dist_to_point_evaluator.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/evaluation/evaluator.py` & `pz_rail_base-0.2.4/src/rail/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/evaluation/metrics/base.py` & `pz_rail_base-0.2.4/src/rail/evaluation/metrics/base.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/evaluation/metrics/cdeloss.py` & `pz_rail_base-0.2.4/src/rail/evaluation/metrics/cdeloss.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/evaluation/metrics/pointestimates.py` & `pz_rail_base-0.2.4/src/rail/evaluation/metrics/pointestimates.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/evaluation/point_to_point_evaluator.py` & `pz_rail_base-0.2.4/src/rail/evaluation/point_to_point_evaluator.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/evaluation/single_evaluator.py` & `pz_rail_base-0.2.4/src/rail/evaluation/single_evaluator.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt` & `pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt` & `pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt` & `pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt` & `pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt` & `pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res` & `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res` & `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res` & `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res` & `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res` & `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res` & `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed` & `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed` & `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed` & `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed` & `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed` & `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed` & `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed` & `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed` & `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml` & `pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl` & `pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq` & `pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/goldenspike_data/goldenspike.yml` & `pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/goldenspike.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/testdata/README.md` & `pz_rail_base-0.2.4/src/rail/examples_data/testdata/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/testdata/lsst_filters.npy` & `pz_rail_base-0.2.4/src/rail/examples_data/testdata/lsst_filters.npy`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/testdata/make_rail_sample_data.ipynb` & `pz_rail_base-0.2.4/src/rail/examples_data/testdata/make_rail_sample_data.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/testdata/output_BPZ_lite.fits` & `pz_rail_base-0.2.4/src/rail/examples_data/testdata/output_BPZ_lite.fits`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/testdata/output_BPZ_lite.hdf5` & `pz_rail_base-0.2.4/src/rail/examples_data/testdata/output_BPZ_lite.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq` & `pz_rail_base-0.2.4/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5` & `pz_rail_base-0.2.4/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/testdata/test_dc2_training_9816.pq` & `pz_rail_base-0.2.4/src/rail/examples_data/testdata/test_dc2_training_9816.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq` & `pz_rail_base-0.2.4/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq` & `pz_rail_base-0.2.4/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5` & `pz_rail_base-0.2.4/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/testdata/training_100gal.hdf5` & `pz_rail_base-0.2.4/src/rail/examples_data/testdata/training_100gal.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/examples_data/testdata/validation_10gal.hdf5` & `pz_rail_base-0.2.4/src/rail/examples_data/testdata/validation_10gal.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/src/rail/stages/__init__.py` & `pz_rail_base-0.2.4/src/rail/stages/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 from rail.creation.engine import *
 
 # from rail.creation.engines.flowEngine import *
 # from rail.creation.engines.galaxy_population_components import *
 # from rail.creation.engines.dsps_photometry_creator import *
 # from rail.creation.engines.dsps_sed_modeler import *
 
-# from rail.evaluation.evaluator import Evaluator
+from rail.evaluation.dist_to_dist_evaluator import DistToDistEvaluator
+from rail.evaluation.dist_to_point_evaluator import DistToPointEvaluator
+from rail.evaluation.evaluator import Evaluator, OldEvaluator
+from rail.evaluation.point_to_point_evaluator import PointToPointEvaluator
+from rail.evaluation.single_evaluator import SingleEvaluator
 
 
 def import_and_attach_all():
     """Import all the packages in the rail ecosystem and attach them to this module"""
     RailEnv.import_all_packages()
     RailEnv.attach_stages(rail.stages)
```

### Comparing `pz-rail-base-0.2.3/tests/cli/hello_world.ipynb` & `pz_rail_base-0.2.4/tests/cli/hello_world.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/tests/cli/single_number.ipynb` & `pz_rail_base-0.2.4/tests/cli/single_number.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/tests/cli/test_scripts.py` & `pz_rail_base-0.2.4/tests/cli/test_scripts.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/tests/core/test_core.py` & `pz_rail_base-0.2.4/tests/core/test_core.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/tests/core/test_introspection.py` & `pz_rail_base-0.2.4/tests/core/test_introspection.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/tests/core/test_pipeline.py` & `pz_rail_base-0.2.4/tests/core/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/tests/core/test_point_estimation.py` & `pz_rail_base-0.2.4/tests/core/test_point_estimation.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/tests/creation/test_degraders.py` & `pz_rail_base-0.2.4/tests/creation/test_degraders.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/tests/estimation/test_algos.py` & `pz_rail_base-0.2.4/tests/estimation/test_algos.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/tests/estimation/test_classifier.py` & `pz_rail_base-0.2.4/tests/estimation/test_classifier.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/tests/estimation/test_summarizers.py` & `pz_rail_base-0.2.4/tests/estimation/test_summarizers.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.3/tests/evaluation/test_evaluation.py` & `pz_rail_base-0.2.4/tests/evaluation/test_evaluation.py`

 * *Files identical despite different names*


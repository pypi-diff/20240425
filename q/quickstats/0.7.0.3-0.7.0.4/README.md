# Comparing `tmp/quickstats-0.7.0.3.tar.gz` & `tmp/quickstats-0.7.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstats-0.7.0.3.tar", last modified: Thu Apr 18 15:44:32 2024, max compression
+gzip compressed data, was "quickstats-0.7.0.4.tar", last modified: Thu Apr 25 03:41:34 2024, max compression
```

## Comparing `quickstats-0.7.0.3.tar` & `quickstats-0.7.0.4.tar`

### file list

```diff
@@ -1,285 +1,295 @@
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:32.000000 quickstats-0.7.0.3/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4125 2024-04-18 15:44:32.000000 quickstats-0.7.0.3/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2024-03-20 05:53:30.000000 quickstats-0.7.0.3/README.md
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/bin/
--rwxr-xr-x   0 chlcheng (124202) zp        (1307)       93 2024-03-20 05:53:30.000000 quickstats-0.7.0.3/bin/quickstats
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      134 2024-04-18 15:35:29.000000 quickstats-0.7.0.3/quickstats/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)       24 2024-04-18 15:41:01.000000 quickstats-0.7.0.3/quickstats/_version.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/algorithms/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:30.000000 quickstats-0.7.0.3/quickstats/algorithms/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/algorithms/nll_crossing/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4350 2024-03-20 05:53:31.000000 quickstats-0.7.0.3/quickstats/algorithms/nll_crossing/BaseMethod.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.3/quickstats/algorithms/nll_crossing/BisectionMethod.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.3/quickstats/algorithms/nll_crossing/NovelMethod.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.3/quickstats/algorithms/nll_crossing/SteppingMethod.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.3/quickstats/algorithms/nll_crossing/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/analysis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2024-04-18 15:35:43.000000 quickstats-0.7.0.3/quickstats/analysis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9725 2024-04-18 15:35:49.000000 quickstats-0.7.0.3/quickstats/analysis/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4025 2024-03-20 05:53:31.000000 quickstats-0.7.0.3/quickstats/analysis/analysis_path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21556 2024-04-18 15:36:06.000000 quickstats-0.7.0.3/quickstats/analysis/config_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    41208 2024-04-18 15:35:54.000000 quickstats-0.7.0.3/quickstats/analysis/data_loading.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1311 2024-04-18 15:36:08.000000 quickstats-0.7.0.3/quickstats/analysis/data_preprocessing.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    85738 2024-04-18 15:35:54.000000 quickstats-0.7.0.3/quickstats/analysis/event_categorization.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8048 2024-03-20 05:53:31.000000 quickstats-0.7.0.3/quickstats/analysis/multi_class_boundary_tree.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9238 2024-04-18 15:35:54.000000 quickstats-0.7.0.3/quickstats/analysis/ntuple_conversion_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    33328 2024-04-18 15:39:29.000000 quickstats-0.7.0.3/quickstats/analysis/ntuple_process_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8906 2024-03-20 05:53:31.000000 quickstats-0.7.0.3/quickstats/analysis/sample_poly_param_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/analysis/systematics/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2024-03-20 05:53:31.000000 quickstats-0.7.0.3/quickstats/analysis/systematics/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29468 2024-03-20 05:53:31.000000 quickstats-0.7.0.3/quickstats/analysis/systematics/base_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9760 2024-03-20 05:53:31.000000 quickstats-0.7.0.3/quickstats/analysis/systematics/gaussian_shape_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6753 2024-03-20 05:53:31.000000 quickstats-0.7.0.3/quickstats/analysis/systematics/normalization_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11890 2024-03-20 05:53:31.000000 quickstats-0.7.0.3/quickstats/analysis/systematics/systematics_evaluation_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/clis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      237 2024-03-20 05:53:31.000000 quickstats-0.7.0.3/quickstats/clis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2816 2024-03-20 05:53:31.000000 quickstats-0.7.0.3/quickstats/clis/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1908 2024-03-20 05:53:31.000000 quickstats-0.7.0.3/quickstats/clis/inspect_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    23980 2024-03-20 05:53:31.000000 quickstats-0.7.0.3/quickstats/clis/likelihood_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15027 2024-03-20 05:53:31.000000 quickstats-0.7.0.3/quickstats/clis/limit_setting.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    19517 2024-04-18 15:43:10.000000 quickstats-0.7.0.3/quickstats/clis/nuisance_parameter_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1609 2024-03-20 05:53:31.000000 quickstats-0.7.0.3/quickstats/clis/processor_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18230 2024-03-20 05:53:32.000000 quickstats-0.7.0.3/quickstats/clis/stat_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18810 2024-03-20 05:54:19.000000 quickstats-0.7.0.3/quickstats/clis/workspace_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/components/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1113 2024-04-18 15:39:11.000000 quickstats-0.7.0.3/quickstats/components/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3136 2024-03-20 05:53:32.000000 quickstats-0.7.0.3/quickstats/components/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15200 2024-03-20 05:53:32.000000 quickstats-0.7.0.3/quickstats/components/analysis_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7330 2024-03-20 05:53:32.000000 quickstats-0.7.0.3/quickstats/components/asimov_generator.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    31508 2024-03-20 05:53:32.000000 quickstats-0.7.0.3/quickstats/components/asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3273 2024-03-20 05:53:32.000000 quickstats-0.7.0.3/quickstats/components/basics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3156 2024-03-20 05:53:32.000000 quickstats-0.7.0.3/quickstats/components/caching_nll_wrapper.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10479 2024-03-20 05:53:32.000000 quickstats-0.7.0.3/quickstats/components/discrete_nuisance.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    56823 2024-04-18 15:35:32.000000 quickstats-0.7.0.3/quickstats/components/extended_minimizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)   105095 2024-03-20 05:53:32.000000 quickstats-0.7.0.3/quickstats/components/extended_model.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5859 2024-04-18 15:34:25.000000 quickstats-0.7.0.3/quickstats/components/extended_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14097 2024-04-18 15:41:02.000000 quickstats-0.7.0.3/quickstats/components/likelihood.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/components/modelling/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.7.0.3/quickstats/components/modelling/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2504 2024-03-20 05:53:32.000000 quickstats-0.7.0.3/quickstats/components/modelling/component_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20116 2024-04-18 15:35:32.000000 quickstats-0.7.0.3/quickstats/components/modelling/data_modelling.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      735 2024-03-20 05:53:33.000000 quickstats-0.7.0.3/quickstats/components/modelling/model_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4502 2024-03-20 05:53:33.000000 quickstats-0.7.0.3/quickstats/components/modelling/parameter_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5550 2024-03-20 05:53:33.000000 quickstats-0.7.0.3/quickstats/components/modelling/pdf_fit_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3483 2024-03-20 05:53:33.000000 quickstats-0.7.0.3/quickstats/components/modelling/tree_data_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10864 2024-03-20 05:53:33.000000 quickstats-0.7.0.3/quickstats/components/nuisance_parameter_harmonizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    17594 2024-03-20 05:53:33.000000 quickstats-0.7.0.3/quickstats/components/nuisance_parameter_pull.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12380 2024-04-18 15:35:32.000000 quickstats-0.7.0.3/quickstats/components/nuisance_parameter_ranking.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/components/processors/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2024-04-18 15:34:50.000000 quickstats-0.7.0.3/quickstats/components/processors/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1417 2024-04-18 15:34:47.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      388 2024-04-18 15:34:45.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/auxiliary.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      358 2024-04-18 15:36:38.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/formatter.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1608 2024-04-18 15:39:37.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2306 2024-04-18 15:39:21.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_as_hdf.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1983 2024-04-18 15:39:21.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_as_numpy.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1592 2024-04-18 15:39:21.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_as_parquet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4421 2024-04-18 15:39:37.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_base_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      866 2024-04-18 15:34:45.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_declare.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1826 2024-04-18 15:39:37.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1228 2024-04-18 15:34:47.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_export.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1245 2024-04-18 15:36:45.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_filter.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1331 2024-04-18 15:34:45.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_global_variables.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_helper_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_hybrid_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      755 2024-04-18 15:34:45.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_if_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      763 2024-04-18 15:34:45.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_if_not_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      726 2024-04-18 15:34:45.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_load_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1211 2024-04-18 15:34:45.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_load_macro.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-04-18 15:34:45.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_max.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      225 2024-04-18 15:34:45.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_mean.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-04-18 15:34:45.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_min.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_nested_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3237 2024-04-18 15:39:37.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_output_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      757 2024-04-18 15:34:47.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_progressbar.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_rdf_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      481 2024-04-18 15:34:45.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_redefine.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1854 2024-04-18 15:36:45.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_report.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      723 2024-04-18 15:36:56.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_safe_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      539 2024-04-18 15:34:45.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_safe_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1774 2024-04-18 15:39:21.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_save.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      735 2024-04-18 15:34:45.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_save_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1433 2024-04-18 15:39:37.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_stat.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-04-18 15:34:45.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_sum.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      606 2024-04-18 15:34:45.000000 quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_treename.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13111 2024-04-18 15:34:23.000000 quickstats-0.7.0.3/quickstats/components/processors/builtin_methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12425 2024-04-18 15:39:35.000000 quickstats-0.7.0.3/quickstats/components/processors/roo_process_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12542 2024-04-18 15:39:29.000000 quickstats-0.7.0.3/quickstats/components/processors/roo_processor.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5406 2024-03-20 05:53:34.000000 quickstats-0.7.0.3/quickstats/components/pvalue_toys.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2978 2024-04-18 15:35:39.000000 quickstats-0.7.0.3/quickstats/components/roo_inspector.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3103 2024-03-20 05:53:34.000000 quickstats-0.7.0.3/quickstats/components/root_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21325 2024-03-20 05:53:34.000000 quickstats-0.7.0.3/quickstats/components/toy_limit_calculator.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/components/workspaces/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2024-03-20 05:53:34.000000 quickstats-0.7.0.3/quickstats/components/workspaces/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2024-03-20 05:53:34.000000 quickstats-0.7.0.3/quickstats/components/workspaces/asimov_handler.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2024-03-20 05:53:34.000000 quickstats-0.7.0.3/quickstats/components/workspaces/core_argument_sets.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2024-03-20 05:53:34.000000 quickstats-0.7.0.3/quickstats/components/workspaces/sample.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2024-03-20 05:53:34.000000 quickstats-0.7.0.3/quickstats/components/workspaces/settings.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8910 2024-03-20 05:53:34.000000 quickstats-0.7.0.3/quickstats/components/workspaces/systematic.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2024-03-20 05:53:34.000000 quickstats-0.7.0.3/quickstats/components/workspaces/systematics_domain.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    53148 2024-04-18 15:35:32.000000 quickstats-0.7.0.3/quickstats/components/workspaces/ws_comparer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8787 2024-04-18 15:35:32.000000 quickstats-0.7.0.3/quickstats/components/workspaces/ws_decomposer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1724 2024-03-20 05:53:34.000000 quickstats-0.7.0.3/quickstats/components/workspaces/ws_modifier_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10827 2024-03-20 05:53:34.000000 quickstats-0.7.0.3/quickstats/components/workspaces/xml_ws_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    87015 2024-03-20 05:53:34.000000 quickstats-0.7.0.3/quickstats/components/workspaces/xml_ws_builder_v1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    76446 2024-04-18 15:34:27.000000 quickstats-0.7.0.3/quickstats/components/workspaces/xml_ws_builder_v2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    52888 2024-04-18 15:35:32.000000 quickstats-0.7.0.3/quickstats/components/workspaces/xml_ws_combiner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    55314 2024-04-18 15:35:32.000000 quickstats-0.7.0.3/quickstats/components/workspaces/xml_ws_modifier.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/concurrent/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      372 2024-03-20 05:53:34.000000 quickstats-0.7.0.3/quickstats/concurrent/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4197 2024-04-18 15:35:40.000000 quickstats-0.7.0.3/quickstats/concurrent/abstract_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.7.0.3/quickstats/concurrent/logging.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5209 2024-03-20 05:53:34.000000 quickstats-0.7.0.3/quickstats/concurrent/nuisance_parameter_ranking_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5285 2024-04-18 15:36:29.000000 quickstats-0.7.0.3/quickstats/concurrent/parameterised_asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10852 2024-04-18 15:36:29.000000 quickstats-0.7.0.3/quickstats/concurrent/parameterised_likelihood.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5822 2024-03-20 05:54:19.000000 quickstats-0.7.0.3/quickstats/concurrent/parameterised_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7694 2024-04-18 15:41:02.000000 quickstats-0.7.0.3/quickstats/concurrent/parameterised_significance.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/core/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      411 2024-04-18 15:36:36.000000 quickstats-0.7.0.3/quickstats/core/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      783 2024-03-20 05:53:35.000000 quickstats-0.7.0.3/quickstats/core/abstract_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    32252 2024-04-18 15:36:37.000000 quickstats-0.7.0.3/quickstats/core/configuration.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4546 2024-04-18 15:35:34.000000 quickstats-0.7.0.3/quickstats/core/constraints.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4603 2024-04-18 15:36:10.000000 quickstats-0.7.0.3/quickstats/core/decorators.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7569 2024-04-18 15:36:10.000000 quickstats-0.7.0.3/quickstats/core/enums.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7707 2024-04-18 15:35:35.000000 quickstats-0.7.0.3/quickstats/core/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2106 2024-04-18 15:36:02.000000 quickstats-0.7.0.3/quickstats/core/metaclasses.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7624 2024-04-18 15:39:09.000000 quickstats-0.7.0.3/quickstats/core/methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9554 2024-03-20 05:53:35.000000 quickstats-0.7.0.3/quickstats/core/path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      721 2024-04-18 15:35:28.000000 quickstats-0.7.0.3/quickstats/core/setup.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6584 2024-04-18 15:36:06.000000 quickstats-0.7.0.3/quickstats/core/type_validation.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3895 2024-04-18 15:35:28.000000 quickstats-0.7.0.3/quickstats/core/virtual_trees.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/extensions/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       85 2024-03-20 05:53:35.000000 quickstats-0.7.0.3/quickstats/extensions/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4147 2024-03-20 05:53:35.000000 quickstats-0.7.0.3/quickstats/extensions/extension_dataframe.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/interface/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:35:04.000000 quickstats-0.7.0.3/quickstats/interface/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/interface/cppyy/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      198 2024-04-18 15:39:03.000000 quickstats-0.7.0.3/quickstats/interface/cppyy/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      392 2024-03-20 05:53:35.000000 quickstats-0.7.0.3/quickstats/interface/cppyy/basic_methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2023-09-01 18:55:46.000000 quickstats-0.7.0.3/quickstats/interface/cppyy/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12794 2024-03-20 05:53:35.000000 quickstats-0.7.0.3/quickstats/interface/cppyy/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4540 2024-03-20 05:53:36.000000 quickstats-0.7.0.3/quickstats/interface/cppyy/vectorize.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/interface/kerberos/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      109 2024-04-18 15:39:14.000000 quickstats-0.7.0.3/quickstats/interface/kerberos/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1709 2024-04-18 15:39:14.000000 quickstats-0.7.0.3/quickstats/interface/kerberos/core.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/interface/root/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3819 2024-03-20 05:53:36.000000 quickstats-0.7.0.3/quickstats/interface/root/ModelConfig.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8814 2024-04-18 15:34:43.000000 quickstats-0.7.0.3/quickstats/interface/root/RDataFrame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2306 2024-03-20 05:53:36.000000 quickstats-0.7.0.3/quickstats/interface/root/RooAbsArg.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.7.0.3/quickstats/interface/root/RooAbsData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21668 2024-03-20 05:53:36.000000 quickstats-0.7.0.3/quickstats/interface/root/RooAbsPdf.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3531 2024-03-20 05:53:36.000000 quickstats-0.7.0.3/quickstats/interface/root/RooArgSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2024-03-20 05:53:36.000000 quickstats-0.7.0.3/quickstats/interface/root/RooCategory.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    44967 2024-03-20 05:53:36.000000 quickstats-0.7.0.3/quickstats/interface/root/RooDataSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.7.0.3/quickstats/interface/root/RooMsgService.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6728 2024-03-20 05:53:36.000000 quickstats-0.7.0.3/quickstats/interface/root/RooRealVar.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.7.0.3/quickstats/interface/root/TArrayData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2905 2024-04-18 15:34:20.000000 quickstats-0.7.0.3/quickstats/interface/root/TChain.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2024-03-20 05:53:36.000000 quickstats-0.7.0.3/quickstats/interface/root/TF1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11385 2024-04-18 15:39:39.000000 quickstats-0.7.0.3/quickstats/interface/root/TFile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2024-03-20 05:53:36.000000 quickstats-0.7.0.3/quickstats/interface/root/TH1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5747 2024-03-20 05:53:36.000000 quickstats-0.7.0.3/quickstats/interface/root/TH2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6043 2024-03-20 05:53:36.000000 quickstats-0.7.0.3/quickstats/interface/root/TH3.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      378 2024-04-18 15:34:42.000000 quickstats-0.7.0.3/quickstats/interface/root/TObject.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      748 2024-04-18 15:39:11.000000 quickstats-0.7.0.3/quickstats/interface/root/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.7.0.3/quickstats/interface/root/helper.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.7.0.3/quickstats/interface/root/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    27713 2024-03-20 05:53:36.000000 quickstats-0.7.0.3/quickstats/interface/root/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5634 2024-03-20 05:53:37.000000 quickstats-0.7.0.3/quickstats/interface/root/roofit_extension.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/interface/servicex/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       91 2024-04-18 15:39:16.000000 quickstats-0.7.0.3/quickstats/interface/servicex/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1725 2024-04-18 15:39:16.000000 quickstats-0.7.0.3/quickstats/interface/servicex/core.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/interface/xrootd/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      149 2024-04-18 15:39:06.000000 quickstats-0.7.0.3/quickstats/interface/xrootd/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      448 2024-04-18 15:39:06.000000 quickstats-0.7.0.3/quickstats/interface/xrootd/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5850 2024-04-18 15:39:41.000000 quickstats-0.7.0.3/quickstats/interface/xrootd/filesystem.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1163 2024-04-18 15:39:41.000000 quickstats-0.7.0.3/quickstats/interface/xrootd/path.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2563 2024-04-18 15:39:07.000000 quickstats-0.7.0.3/quickstats/interface/xrootd/xrd_helper.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/macros/
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/macros/AsymptoticCLsTool/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7366 2024-03-20 05:53:37.000000 quickstats-0.7.0.3/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1591 2024-03-20 05:53:37.000000 quickstats-0.7.0.3/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/macros/FlexibleInterpVarMkII/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.7.0.3/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.7.0.3/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/macros/QuickStatsCore/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3133 2024-03-20 05:53:37.000000 quickstats-0.7.0.3/quickstats/macros/QuickStatsCore/QStringUtils.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1259 2024-03-20 05:53:37.000000 quickstats-0.7.0.3/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10312 2024-03-20 05:53:37.000000 quickstats-0.7.0.3/quickstats/macros/QuickStatsCore/RooFitExt.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3868 2024-03-20 05:53:37.000000 quickstats-0.7.0.3/quickstats/macros/QuickStatsCore/RooFitExt.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/macros/ResponseFunction/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13749 2024-04-18 15:34:34.000000 quickstats-0.7.0.3/quickstats/macros/ResponseFunction/ResponseFunction.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.7.0.3/quickstats/macros/ResponseFunction/ResponseFunction.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/macros/RooTwoSidedCBShape/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.7.0.3/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.7.0.3/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/maths/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.7.0.3/quickstats/maths/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4366 2024-03-20 05:53:37.000000 quickstats-0.7.0.3/quickstats/maths/interpolation.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8729 2024-04-18 15:41:02.000000 quickstats-0.7.0.3/quickstats/maths/numerics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    40281 2024-04-18 15:41:02.000000 quickstats-0.7.0.3/quickstats/maths/statistics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2024-03-20 05:53:37.000000 quickstats-0.7.0.3/quickstats/maths/statistics_jitted.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.7.0.3/quickstats/maths/symbolics.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats/parsers/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      187 2024-03-20 05:53:37.000000 quickstats-0.7.0.3/quickstats/parsers/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.7.0.3/quickstats/parsers/config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16764 2024-03-20 05:53:37.000000 quickstats-0.7.0.3/quickstats/parsers/param_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5204 2024-03-20 05:53:37.000000 quickstats-0.7.0.3/quickstats/parsers/roo_param_setup_parser.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:32.000000 quickstats-0.7.0.3/quickstats/plots/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1345 2024-03-20 05:53:37.000000 quickstats-0.7.0.3/quickstats/plots/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    28606 2024-04-18 15:41:02.000000 quickstats-0.7.0.3/quickstats/plots/abstract_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14144 2024-04-18 15:38:50.000000 quickstats-0.7.0.3/quickstats/plots/bidirectional_bar_chart.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.7.0.3/quickstats/plots/collective_data_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3467 2024-04-18 15:35:22.000000 quickstats-0.7.0.3/quickstats/plots/color_schemes.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5899 2024-03-20 05:53:37.000000 quickstats-0.7.0.3/quickstats/plots/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4951 2024-03-20 05:53:37.000000 quickstats-0.7.0.3/quickstats/plots/correlation_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7581 2024-04-18 15:38:51.000000 quickstats-0.7.0.3/quickstats/plots/general_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4061 2024-04-18 15:38:51.000000 quickstats-0.7.0.3/quickstats/plots/general_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22203 2024-04-18 15:41:03.000000 quickstats-0.7.0.3/quickstats/plots/general_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6078 2024-04-18 15:38:56.000000 quickstats-0.7.0.3/quickstats/plots/hypotest_inverter_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8981 2024-03-20 05:53:38.000000 quickstats-0.7.0.3/quickstats/plots/likelihood_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16926 2024-04-18 15:38:51.000000 quickstats-0.7.0.3/quickstats/plots/likelihood_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29155 2024-03-20 05:53:38.000000 quickstats-0.7.0.3/quickstats/plots/np_ranking_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    25684 2024-04-18 15:41:03.000000 quickstats-0.7.0.3/quickstats/plots/pdf_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5096 2024-04-18 15:38:51.000000 quickstats-0.7.0.3/quickstats/plots/sample_purity_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10353 2024-04-18 15:38:51.000000 quickstats-0.7.0.3/quickstats/plots/score_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4122 2024-03-20 05:53:38.000000 quickstats-0.7.0.3/quickstats/plots/stat_plot_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    30210 2024-04-18 15:41:03.000000 quickstats-0.7.0.3/quickstats/plots/template.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13785 2024-04-18 15:38:51.000000 quickstats-0.7.0.3/quickstats/plots/test_statistic_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5122 2024-03-20 05:53:38.000000 quickstats-0.7.0.3/quickstats/plots/two_axis_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9999 2024-04-18 15:42:16.000000 quickstats-0.7.0.3/quickstats/plots/upper_limit_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    19292 2024-04-18 15:38:51.000000 quickstats-0.7.0.3/quickstats/plots/upper_limit_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13182 2024-04-18 15:38:51.000000 quickstats-0.7.0.3/quickstats/plots/upper_limit_3D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    23223 2024-04-18 15:41:04.000000 quickstats-0.7.0.3/quickstats/plots/upper_limit_benchmark_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    34148 2024-04-18 15:41:04.000000 quickstats-0.7.0.3/quickstats/plots/variable_distribution_plot.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:32.000000 quickstats-0.7.0.3/quickstats/resources/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2024-03-20 05:53:39.000000 quickstats-0.7.0.3/quickstats/resources/default_workspace_extensions.json
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:32.000000 quickstats-0.7.0.3/quickstats/resources/mpl_stylesheets/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2024-03-20 05:53:39.000000 quickstats-0.7.0.3/quickstats/resources/mpl_stylesheets/hep.mplstyle
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:39.000000 quickstats-0.7.0.3/quickstats/resources/mpl_stylesheets/no_latex.mplstyle
--rw-r--r--   0 chlcheng (124202) zp        (1307)      325 2024-03-20 05:53:39.000000 quickstats-0.7.0.3/quickstats/resources/mpl_stylesheets/science.mplstyle
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4604 2024-03-20 05:53:39.000000 quickstats-0.7.0.3/quickstats/root_checker.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:32.000000 quickstats-0.7.0.3/quickstats/utils/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.7.0.3/quickstats/utils/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    19071 2024-04-18 15:36:53.000000 quickstats-0.7.0.3/quickstats/utils/common_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.7.0.3/quickstats/utils/condor_tasks.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18666 2024-04-18 15:39:08.000000 quickstats-0.7.0.3/quickstats/utils/data_conversion.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.7.0.3/quickstats/utils/hep_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2080 2024-04-18 15:41:04.000000 quickstats-0.7.0.3/quickstats/utils/path_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      563 2024-04-18 15:35:24.000000 quickstats-0.7.0.3/quickstats/utils/py_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    27521 2024-04-18 15:36:12.000000 quickstats-0.7.0.3/quickstats/utils/roofit_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10914 2024-03-20 05:53:39.000000 quickstats-0.7.0.3/quickstats/utils/roostats_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15330 2024-04-18 15:36:32.000000 quickstats-0.7.0.3/quickstats/utils/root_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15638 2024-04-18 15:39:31.000000 quickstats-0.7.0.3/quickstats/utils/string_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2321 2024-04-18 15:36:21.000000 quickstats-0.7.0.3/quickstats/utils/sys_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15128 2024-04-18 15:35:57.000000 quickstats-0.7.0.3/quickstats/utils/xml_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:44:31.000000 quickstats-0.7.0.3/quickstats.egg-info/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4125 2024-04-18 15:44:30.000000 quickstats-0.7.0.3/quickstats.egg-info/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10761 2024-04-18 15:44:30.000000 quickstats-0.7.0.3/quickstats.egg-info/SOURCES.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2024-04-18 15:44:30.000000 quickstats-0.7.0.3/quickstats.egg-info/dependency_links.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2024-04-18 15:44:30.000000 quickstats-0.7.0.3/quickstats.egg-info/requires.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2024-04-18 15:44:30.000000 quickstats-0.7.0.3/quickstats.egg-info/top_level.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2024-04-18 15:44:32.000000 quickstats-0.7.0.3/setup.cfg
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1771 2024-04-18 15:34:33.000000 quickstats-0.7.0.3/setup.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:34.000000 quickstats-0.7.0.4/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4125 2024-04-25 03:41:34.000000 quickstats-0.7.0.4/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2024-03-20 05:53:30.000000 quickstats-0.7.0.4/README.md
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:18.000000 quickstats-0.7.0.4/bin/
+-rwxr-xr-x   0 chlcheng (124202) zp        (1307)       93 2024-03-20 05:53:30.000000 quickstats-0.7.0.4/bin/quickstats
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:19.000000 quickstats-0.7.0.4/quickstats/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      134 2024-04-18 15:35:29.000000 quickstats-0.7.0.4/quickstats/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       24 2024-04-25 03:40:17.000000 quickstats-0.7.0.4/quickstats/_version.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:20.000000 quickstats-0.7.0.4/quickstats/algorithms/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:30.000000 quickstats-0.7.0.4/quickstats/algorithms/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:20.000000 quickstats-0.7.0.4/quickstats/algorithms/nll_crossing/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4350 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/algorithms/nll_crossing/BaseMethod.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/algorithms/nll_crossing/BisectionMethod.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/algorithms/nll_crossing/NovelMethod.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/algorithms/nll_crossing/SteppingMethod.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/algorithms/nll_crossing/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:21.000000 quickstats-0.7.0.4/quickstats/analysis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2024-04-18 15:35:43.000000 quickstats-0.7.0.4/quickstats/analysis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9725 2024-04-18 15:35:49.000000 quickstats-0.7.0.4/quickstats/analysis/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4025 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/analysis/analysis_path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21556 2024-04-18 15:36:06.000000 quickstats-0.7.0.4/quickstats/analysis/config_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    41208 2024-04-18 15:35:54.000000 quickstats-0.7.0.4/quickstats/analysis/data_loading.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1311 2024-04-18 15:36:08.000000 quickstats-0.7.0.4/quickstats/analysis/data_preprocessing.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    85738 2024-04-18 15:35:54.000000 quickstats-0.7.0.4/quickstats/analysis/event_categorization.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8048 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/analysis/multi_class_boundary_tree.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9238 2024-04-18 15:35:54.000000 quickstats-0.7.0.4/quickstats/analysis/ntuple_conversion_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    33252 2024-04-25 03:40:17.000000 quickstats-0.7.0.4/quickstats/analysis/ntuple_process_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8906 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/analysis/sample_poly_param_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:21.000000 quickstats-0.7.0.4/quickstats/analysis/systematics/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/analysis/systematics/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29468 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/analysis/systematics/base_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9760 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/analysis/systematics/gaussian_shape_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6753 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/analysis/systematics/normalization_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11890 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/analysis/systematics/systematics_evaluation_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:21.000000 quickstats-0.7.0.4/quickstats/clis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      237 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/clis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2816 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/clis/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1908 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/clis/inspect_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    23632 2024-04-25 03:40:17.000000 quickstats-0.7.0.4/quickstats/clis/likelihood_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15027 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/clis/limit_setting.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19517 2024-04-18 15:43:10.000000 quickstats-0.7.0.4/quickstats/clis/nuisance_parameter_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1609 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/clis/processor_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18230 2024-03-20 05:53:32.000000 quickstats-0.7.0.4/quickstats/clis/stat_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18810 2024-03-20 05:54:19.000000 quickstats-0.7.0.4/quickstats/clis/workspace_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:22.000000 quickstats-0.7.0.4/quickstats/components/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1113 2024-04-18 15:39:11.000000 quickstats-0.7.0.4/quickstats/components/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3136 2024-03-20 05:53:32.000000 quickstats-0.7.0.4/quickstats/components/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15274 2024-04-25 03:40:17.000000 quickstats-0.7.0.4/quickstats/components/analysis_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7330 2024-03-20 05:53:32.000000 quickstats-0.7.0.4/quickstats/components/asimov_generator.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    31508 2024-03-20 05:53:32.000000 quickstats-0.7.0.4/quickstats/components/asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3273 2024-03-20 05:53:32.000000 quickstats-0.7.0.4/quickstats/components/basics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3156 2024-03-20 05:53:32.000000 quickstats-0.7.0.4/quickstats/components/caching_nll_wrapper.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10479 2024-03-20 05:53:32.000000 quickstats-0.7.0.4/quickstats/components/discrete_nuisance.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    56823 2024-04-18 15:35:32.000000 quickstats-0.7.0.4/quickstats/components/extended_minimizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)   105095 2024-03-20 05:53:32.000000 quickstats-0.7.0.4/quickstats/components/extended_model.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5859 2024-04-18 15:34:25.000000 quickstats-0.7.0.4/quickstats/components/extended_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14097 2024-04-18 15:41:02.000000 quickstats-0.7.0.4/quickstats/components/likelihood.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:23.000000 quickstats-0.7.0.4/quickstats/components/modelling/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.7.0.4/quickstats/components/modelling/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2504 2024-03-20 05:53:32.000000 quickstats-0.7.0.4/quickstats/components/modelling/component_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20116 2024-04-18 15:35:32.000000 quickstats-0.7.0.4/quickstats/components/modelling/data_modelling.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      735 2024-03-20 05:53:33.000000 quickstats-0.7.0.4/quickstats/components/modelling/model_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4502 2024-03-20 05:53:33.000000 quickstats-0.7.0.4/quickstats/components/modelling/parameter_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5550 2024-03-20 05:53:33.000000 quickstats-0.7.0.4/quickstats/components/modelling/pdf_fit_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3483 2024-03-20 05:53:33.000000 quickstats-0.7.0.4/quickstats/components/modelling/tree_data_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10864 2024-03-20 05:53:33.000000 quickstats-0.7.0.4/quickstats/components/nuisance_parameter_harmonizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17594 2024-03-20 05:53:33.000000 quickstats-0.7.0.4/quickstats/components/nuisance_parameter_pull.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12380 2024-04-18 15:35:32.000000 quickstats-0.7.0.4/quickstats/components/nuisance_parameter_ranking.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:23.000000 quickstats-0.7.0.4/quickstats/components/processors/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2024-04-18 15:34:50.000000 quickstats-0.7.0.4/quickstats/components/processors/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:24.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1457 2024-04-25 03:40:17.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      388 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/auxiliary.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      358 2024-04-18 15:36:38.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/formatter.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1608 2024-04-18 15:39:37.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2360 2024-04-25 03:40:17.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_as_hdf.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2037 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_as_numpy.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1589 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_as_parquet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4421 2024-04-18 15:39:37.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_base_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1049 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_cache.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      866 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_declare.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1826 2024-04-18 15:39:37.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1228 2024-04-18 15:34:47.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_export.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1903 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_filter.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1331 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_global_variables.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_helper_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_hybrid_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      755 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_if_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      763 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_if_not_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      726 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_load_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1211 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_load_macro.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_max.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      225 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_mean.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_min.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_nested_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2249 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_output_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      757 2024-04-18 15:34:47.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_progressbar.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_rdf_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      481 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_redefine.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1854 2024-04-18 15:36:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_report.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      723 2024-04-18 15:36:56.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_safe_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      539 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_safe_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1770 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_save.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      735 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_save_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1433 2024-04-18 15:39:37.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_stat.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_sum.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      606 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_treename.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13111 2024-04-18 15:34:23.000000 quickstats-0.7.0.4/quickstats/components/processors/builtin_methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12481 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/components/processors/roo_process_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13856 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/components/processors/roo_processor.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5406 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/pvalue_toys.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2978 2024-04-18 15:35:39.000000 quickstats-0.7.0.4/quickstats/components/roo_inspector.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3103 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/root_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21325 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/toy_limit_calculator.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:25.000000 quickstats-0.7.0.4/quickstats/components/workspaces/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/workspaces/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/workspaces/asimov_handler.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/workspaces/core_argument_sets.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/workspaces/sample.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/workspaces/settings.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8910 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/workspaces/systematic.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/workspaces/systematics_domain.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    53148 2024-04-18 15:35:32.000000 quickstats-0.7.0.4/quickstats/components/workspaces/ws_comparer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8787 2024-04-18 15:35:32.000000 quickstats-0.7.0.4/quickstats/components/workspaces/ws_decomposer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1724 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/workspaces/ws_modifier_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10827 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/workspaces/xml_ws_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    87015 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/workspaces/xml_ws_builder_v1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    76446 2024-04-18 15:34:27.000000 quickstats-0.7.0.4/quickstats/components/workspaces/xml_ws_builder_v2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    52888 2024-04-18 15:35:32.000000 quickstats-0.7.0.4/quickstats/components/workspaces/xml_ws_combiner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    55314 2024-04-18 15:35:32.000000 quickstats-0.7.0.4/quickstats/components/workspaces/xml_ws_modifier.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:26.000000 quickstats-0.7.0.4/quickstats/concurrent/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      372 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/concurrent/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4197 2024-04-18 15:35:40.000000 quickstats-0.7.0.4/quickstats/concurrent/abstract_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.7.0.4/quickstats/concurrent/logging.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5209 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/concurrent/nuisance_parameter_ranking_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5285 2024-04-18 15:36:29.000000 quickstats-0.7.0.4/quickstats/concurrent/parameterised_asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10852 2024-04-18 15:36:29.000000 quickstats-0.7.0.4/quickstats/concurrent/parameterised_likelihood.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5822 2024-03-20 05:54:19.000000 quickstats-0.7.0.4/quickstats/concurrent/parameterised_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7694 2024-04-18 15:41:02.000000 quickstats-0.7.0.4/quickstats/concurrent/parameterised_significance.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:27.000000 quickstats-0.7.0.4/quickstats/core/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      411 2024-04-18 15:36:36.000000 quickstats-0.7.0.4/quickstats/core/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      783 2024-03-20 05:53:35.000000 quickstats-0.7.0.4/quickstats/core/abstract_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    32252 2024-04-18 15:36:37.000000 quickstats-0.7.0.4/quickstats/core/configuration.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4546 2024-04-18 15:35:34.000000 quickstats-0.7.0.4/quickstats/core/constraints.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4603 2024-04-18 15:36:10.000000 quickstats-0.7.0.4/quickstats/core/decorators.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7569 2024-04-18 15:36:10.000000 quickstats-0.7.0.4/quickstats/core/enums.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7707 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/core/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2106 2024-04-18 15:36:02.000000 quickstats-0.7.0.4/quickstats/core/metaclasses.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7624 2024-04-18 15:39:09.000000 quickstats-0.7.0.4/quickstats/core/methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9554 2024-03-20 05:53:35.000000 quickstats-0.7.0.4/quickstats/core/path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      721 2024-04-18 15:35:28.000000 quickstats-0.7.0.4/quickstats/core/setup.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6584 2024-04-18 15:36:06.000000 quickstats-0.7.0.4/quickstats/core/type_validation.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3895 2024-04-18 15:35:28.000000 quickstats-0.7.0.4/quickstats/core/virtual_trees.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:27.000000 quickstats-0.7.0.4/quickstats/daq/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      151 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/daq/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6933 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/daq/remote_data_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3849 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/daq/servicex_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2553 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/daq/xrootd_source.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:27.000000 quickstats-0.7.0.4/quickstats/extensions/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       85 2024-03-20 05:53:35.000000 quickstats-0.7.0.4/quickstats/extensions/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4147 2024-03-20 05:53:35.000000 quickstats-0.7.0.4/quickstats/extensions/extension_dataframe.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:27.000000 quickstats-0.7.0.4/quickstats/interface/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:35:04.000000 quickstats-0.7.0.4/quickstats/interface/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:28.000000 quickstats-0.7.0.4/quickstats/interface/cppyy/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      198 2024-04-18 15:39:03.000000 quickstats-0.7.0.4/quickstats/interface/cppyy/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      392 2024-03-20 05:53:35.000000 quickstats-0.7.0.4/quickstats/interface/cppyy/basic_methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2023-09-01 18:55:46.000000 quickstats-0.7.0.4/quickstats/interface/cppyy/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12794 2024-03-20 05:53:35.000000 quickstats-0.7.0.4/quickstats/interface/cppyy/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4540 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/cppyy/vectorize.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:28.000000 quickstats-0.7.0.4/quickstats/interface/kerberos/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      109 2024-04-18 15:39:14.000000 quickstats-0.7.0.4/quickstats/interface/kerberos/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1709 2024-04-18 15:39:14.000000 quickstats-0.7.0.4/quickstats/interface/kerberos/core.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:30.000000 quickstats-0.7.0.4/quickstats/interface/root/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3819 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/root/ModelConfig.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10737 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/root/RDataFrame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2306 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/root/RooAbsArg.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.7.0.4/quickstats/interface/root/RooAbsData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21668 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/root/RooAbsPdf.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3531 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/root/RooArgSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/root/RooCategory.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    44967 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/root/RooDataSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.7.0.4/quickstats/interface/root/RooMsgService.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6728 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/root/RooRealVar.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.7.0.4/quickstats/interface/root/TArrayData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2905 2024-04-18 15:34:20.000000 quickstats-0.7.0.4/quickstats/interface/root/TChain.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/root/TF1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11390 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/root/TFile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/root/TH1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5813 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/root/TH2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6043 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/root/TH3.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      378 2024-04-18 15:34:42.000000 quickstats-0.7.0.4/quickstats/interface/root/TObject.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      748 2024-04-18 15:39:11.000000 quickstats-0.7.0.4/quickstats/interface/root/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.7.0.4/quickstats/interface/root/helper.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.7.0.4/quickstats/interface/root/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    27713 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/root/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5634 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/interface/root/roofit_extension.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:30.000000 quickstats-0.7.0.4/quickstats/interface/servicex/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      163 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/servicex/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5409 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/servicex/config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2872 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/servicex/core.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:30.000000 quickstats-0.7.0.4/quickstats/interface/tinydb/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       67 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/tinydb/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      947 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/tinydb/methods.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:30.000000 quickstats-0.7.0.4/quickstats/interface/xrootd/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      149 2024-04-18 15:39:06.000000 quickstats-0.7.0.4/quickstats/interface/xrootd/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      448 2024-04-18 15:39:06.000000 quickstats-0.7.0.4/quickstats/interface/xrootd/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5850 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/xrootd/filesystem.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1163 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/xrootd/path.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/xrootd/xrd_helper.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:18.000000 quickstats-0.7.0.4/quickstats/macros/
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:30.000000 quickstats-0.7.0.4/quickstats/macros/AsymptoticCLsTool/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7366 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1591 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:30.000000 quickstats-0.7.0.4/quickstats/macros/FlexibleInterpVarMkII/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.7.0.4/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.7.0.4/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:30.000000 quickstats-0.7.0.4/quickstats/macros/QuickStatsCore/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3133 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/macros/QuickStatsCore/QStringUtils.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1259 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10312 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/macros/QuickStatsCore/RooFitExt.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3868 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/macros/QuickStatsCore/RooFitExt.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:30.000000 quickstats-0.7.0.4/quickstats/macros/ResponseFunction/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13749 2024-04-18 15:34:34.000000 quickstats-0.7.0.4/quickstats/macros/ResponseFunction/ResponseFunction.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.7.0.4/quickstats/macros/ResponseFunction/ResponseFunction.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:31.000000 quickstats-0.7.0.4/quickstats/macros/RooTwoSidedCBShape/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.7.0.4/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.7.0.4/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:31.000000 quickstats-0.7.0.4/quickstats/maths/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.7.0.4/quickstats/maths/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4366 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/maths/interpolation.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9053 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/maths/numerics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    40281 2024-04-18 15:41:02.000000 quickstats-0.7.0.4/quickstats/maths/statistics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/maths/statistics_jitted.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.7.0.4/quickstats/maths/symbolics.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:31.000000 quickstats-0.7.0.4/quickstats/parsers/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      187 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/parsers/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.7.0.4/quickstats/parsers/config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16764 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/parsers/param_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5204 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/parsers/roo_param_setup_parser.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:33.000000 quickstats-0.7.0.4/quickstats/plots/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1345 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/plots/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    28606 2024-04-18 15:41:02.000000 quickstats-0.7.0.4/quickstats/plots/abstract_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14144 2024-04-18 15:38:50.000000 quickstats-0.7.0.4/quickstats/plots/bidirectional_bar_chart.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.7.0.4/quickstats/plots/collective_data_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3467 2024-04-18 15:35:22.000000 quickstats-0.7.0.4/quickstats/plots/color_schemes.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5899 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/plots/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4951 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/plots/correlation_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7581 2024-04-18 15:38:51.000000 quickstats-0.7.0.4/quickstats/plots/general_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4061 2024-04-18 15:38:51.000000 quickstats-0.7.0.4/quickstats/plots/general_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22203 2024-04-18 15:41:03.000000 quickstats-0.7.0.4/quickstats/plots/general_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6078 2024-04-18 15:38:56.000000 quickstats-0.7.0.4/quickstats/plots/hypotest_inverter_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8981 2024-03-20 05:53:38.000000 quickstats-0.7.0.4/quickstats/plots/likelihood_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16926 2024-04-18 15:38:51.000000 quickstats-0.7.0.4/quickstats/plots/likelihood_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29155 2024-03-20 05:53:38.000000 quickstats-0.7.0.4/quickstats/plots/np_ranking_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    25684 2024-04-18 15:41:03.000000 quickstats-0.7.0.4/quickstats/plots/pdf_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5096 2024-04-18 15:38:51.000000 quickstats-0.7.0.4/quickstats/plots/sample_purity_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10353 2024-04-18 15:38:51.000000 quickstats-0.7.0.4/quickstats/plots/score_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4122 2024-03-20 05:53:38.000000 quickstats-0.7.0.4/quickstats/plots/stat_plot_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    30210 2024-04-18 15:41:03.000000 quickstats-0.7.0.4/quickstats/plots/template.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13785 2024-04-18 15:38:51.000000 quickstats-0.7.0.4/quickstats/plots/test_statistic_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5122 2024-03-20 05:53:38.000000 quickstats-0.7.0.4/quickstats/plots/two_axis_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9999 2024-04-18 15:42:16.000000 quickstats-0.7.0.4/quickstats/plots/upper_limit_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19292 2024-04-18 15:38:51.000000 quickstats-0.7.0.4/quickstats/plots/upper_limit_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13182 2024-04-18 15:38:51.000000 quickstats-0.7.0.4/quickstats/plots/upper_limit_3D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    23223 2024-04-18 15:41:04.000000 quickstats-0.7.0.4/quickstats/plots/upper_limit_benchmark_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    34148 2024-04-18 15:41:04.000000 quickstats-0.7.0.4/quickstats/plots/variable_distribution_plot.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:33.000000 quickstats-0.7.0.4/quickstats/resources/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2024-03-20 05:53:39.000000 quickstats-0.7.0.4/quickstats/resources/default_workspace_extensions.json
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:33.000000 quickstats-0.7.0.4/quickstats/resources/mpl_stylesheets/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2024-03-20 05:53:39.000000 quickstats-0.7.0.4/quickstats/resources/mpl_stylesheets/hep.mplstyle
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:39.000000 quickstats-0.7.0.4/quickstats/resources/mpl_stylesheets/no_latex.mplstyle
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      325 2024-03-20 05:53:39.000000 quickstats-0.7.0.4/quickstats/resources/mpl_stylesheets/science.mplstyle
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4604 2024-03-20 05:53:39.000000 quickstats-0.7.0.4/quickstats/root_checker.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:34.000000 quickstats-0.7.0.4/quickstats/utils/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.7.0.4/quickstats/utils/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19773 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/utils/common_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.7.0.4/quickstats/utils/condor_tasks.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18666 2024-04-18 15:39:08.000000 quickstats-0.7.0.4/quickstats/utils/data_conversion.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.7.0.4/quickstats/utils/hep_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3039 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/utils/path_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      563 2024-04-18 15:35:24.000000 quickstats-0.7.0.4/quickstats/utils/py_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    27521 2024-04-18 15:36:12.000000 quickstats-0.7.0.4/quickstats/utils/roofit_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10914 2024-03-20 05:53:39.000000 quickstats-0.7.0.4/quickstats/utils/roostats_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15330 2024-04-18 15:36:32.000000 quickstats-0.7.0.4/quickstats/utils/root_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15638 2024-04-18 15:39:31.000000 quickstats-0.7.0.4/quickstats/utils/string_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2321 2024-04-18 15:36:21.000000 quickstats-0.7.0.4/quickstats/utils/sys_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15128 2024-04-18 15:35:57.000000 quickstats-0.7.0.4/quickstats/utils/xml_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:20.000000 quickstats-0.7.0.4/quickstats.egg-info/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4125 2024-04-25 03:41:13.000000 quickstats-0.7.0.4/quickstats.egg-info/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11068 2024-04-25 03:41:16.000000 quickstats-0.7.0.4/quickstats.egg-info/SOURCES.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2024-04-25 03:41:15.000000 quickstats-0.7.0.4/quickstats.egg-info/dependency_links.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2024-04-25 03:41:15.000000 quickstats-0.7.0.4/quickstats.egg-info/requires.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2024-04-25 03:41:15.000000 quickstats-0.7.0.4/quickstats.egg-info/top_level.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2024-04-25 03:41:34.000000 quickstats-0.7.0.4/setup.cfg
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1771 2024-04-18 15:34:33.000000 quickstats-0.7.0.4/setup.py
```

### Comparing `quickstats-0.7.0.3/PKG-INFO` & `quickstats-0.7.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.7.0.3
+Version: 0.7.0.4
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.7.0.3/README.md` & `quickstats-0.7.0.4/README.md`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/algorithms/nll_crossing/BaseMethod.py` & `quickstats-0.7.0.4/quickstats/algorithms/nll_crossing/BaseMethod.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/analysis/analysis_base.py` & `quickstats-0.7.0.4/quickstats/analysis/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/analysis/analysis_path_manager.py` & `quickstats-0.7.0.4/quickstats/analysis/analysis_path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/analysis/config_templates.py` & `quickstats-0.7.0.4/quickstats/analysis/config_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/analysis/data_loading.py` & `quickstats-0.7.0.4/quickstats/analysis/data_loading.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/analysis/data_preprocessing.py` & `quickstats-0.7.0.4/quickstats/analysis/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/analysis/event_categorization.py` & `quickstats-0.7.0.4/quickstats/analysis/event_categorization.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/analysis/multi_class_boundary_tree.py` & `quickstats-0.7.0.4/quickstats/analysis/multi_class_boundary_tree.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/analysis/ntuple_conversion_tool.py` & `quickstats-0.7.0.4/quickstats/analysis/ntuple_conversion_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/analysis/ntuple_process_tool.py` & `quickstats-0.7.0.4/quickstats/analysis/ntuple_process_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,16 @@
     def __init__(self, sample_config:Union[Dict, str],
                  outdir:str='output',
                  process_config:Optional[Union["RooProcessConfig", str]]=None,
                  process_flags:Optional[List[str]]=None,
                  cache:bool=True,
                  use_template:bool=False,
                  multithread:bool=True,
+                 data_service:Optional[str]=None,
+                 data_service_options:Optional[Dict]=None,                 
                  backend:Optional[str]=None,
                  backend_options:Optional[Dict]=None,
                  verbosity:Optional[Union[int, str]]="INFO",
                  **kwargs):
         
         super().__init__(verbosity=verbosity)
         
@@ -80,15 +82,20 @@
         self.load_sample_config(sample_config)
         
         self.processor = None        
         if process_config is not None:
             self.load_process_config(process_config,
                                      cache=cache,
                                      use_template=use_template,
-                                     multithread=multithread)
+                                     multithread=multithread,
+                                     data_service=data_service,
+                                     data_service_options=data_service_options,
+                                     backend=backend,
+                                     backend_options=backend_options,
+                                     **kwargs)
             
         if process_flags is not None:
             self.process_flags = list(process_flags)
         else:
             self.process_flags = []
         
         self.cutflow_report = None
@@ -175,28 +182,19 @@
                     attribute_data['syst_var'].append(syst_var)
                     attribute_data['sample_type'].append(sample_type)
         import pandas as pd
         index_list = ['syst_theme', 'sample', 'syst_name', 'sample_type', 'syst_var']
         attribute_df = pd.DataFrame(attribute_data).set_index(index_list)
         return attribute_df
     
-    def load_process_config(self, config_source:Union["RooProcessConfig", str],
-                            cache:bool=True,
-                            multithread:bool=True,
-                            use_template:bool=False,
-                            backend:Optional[str]=None,
-                            backend_options:Optional[Dict]=None):
+    def load_process_config(self, config_source:Union["RooProcessConfig", str], **kwargs):
         from quickstats.components import RooProcessor
         self.processor = RooProcessor(config_source,
-                                      cache=cache,
-                                      use_template=use_template,
-                                      multithread=multithread,
-                                      backend=backend,
-                                      backend_options=backend_options,
-                                      verbosity=self.stdout.verbosity)
+                                      verbosity=self.stdout.verbosity,
+                                      **kwargs)
         if isinstance(config_source, str):
             self.path_manager.set_file("process_config", os.path.abspath(config_source))
         
     def get_validated_syst_themes(self, syst_themes:Optional[List[str]]=None):
         if syst_themes is None:
             return [theme for theme in list(self.syst_theme_list) if theme != 'Nominal']
         invalid_syst_themes = list(set(syst_themes) - set(self.syst_theme_list))
```

### Comparing `quickstats-0.7.0.3/quickstats/analysis/sample_poly_param_tool.py` & `quickstats-0.7.0.4/quickstats/analysis/sample_poly_param_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/analysis/systematics/base_systematics.py` & `quickstats-0.7.0.4/quickstats/analysis/systematics/base_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/analysis/systematics/gaussian_shape_systematics.py` & `quickstats-0.7.0.4/quickstats/analysis/systematics/gaussian_shape_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/analysis/systematics/normalization_systematics.py` & `quickstats-0.7.0.4/quickstats/analysis/systematics/normalization_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/analysis/systematics/systematics_evaluation_tool.py` & `quickstats-0.7.0.4/quickstats/analysis/systematics/systematics_evaluation_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/clis/core.py` & `quickstats-0.7.0.4/quickstats/clis/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/clis/inspect_rfile.py` & `quickstats-0.7.0.4/quickstats/clis/inspect_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/clis/likelihood_tools.py` & `quickstats-0.7.0.4/quickstats/clis/likelihood_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,51 +5,45 @@
 from .core import cli
 
 __all__ = ['likelihood_fit', 'likelihood_scan']
 
 @cli.command(name='likelihood_fit')
 @click.option('-i', '--input_file', "filename", required=True, 
               help='Path to the input workspace file.')
-@click.option('-o', '--outname', default='fit_result.json', show_default=True,
-              help='Name of output file.')
 @click.option('--display/--no-display', default=True, show_default=True,
               help='Display fit result.')
-@click.option('--save/--no-save', "save_result", default=False, show_default=True,
-              help='Save fit result.')
-@click.option('--save_log/--skip_log', default=False, show_default=True,
-              help='Save log file.')
-@click.option('--save_ws', default=None, show_default=True,
-              help='Save fitted workspace to a given path.')
-@click.option('--save_snapshot', default=None, show_default=True,
+@click.option('--save-result', default=None, show_default=True,
+              help='Save fit result as a json file to the given path.')
+@click.option('--save-log', default=None, show_default=True,
+              help='Save log as a text file to the given path.')
+@click.option('--save-ws', default=None, show_default=True,
+              help='Save fitted workspace to the given path.')
+@click.option('--save-snapshot', default=None, show_default=True,
               help='Save fitted values of all variables as a snapshot and restore all variables to '
               'their initial values. Should be used together with --save_ws.')
+@click.option('--save-pulls', default=None, show_default=True,
+              help='Export (constrained) NP results for pulls to the given directory.')
 @click.option('--rebuild/--no-rebuild', default=True, show_default=True,
               help='Save fitted workspace by rebuilding it. Should be used together with --save_ws.')
-@click.option('--export_as_np_pulls/--skip_export_as_np_pulls', default=False, show_default=True,
-              help='Export (constrained) NP results for pulls plot.')
-@click.option('--outdir', default="pulls", show_default=True,
-              help='Output directory for pulls output.')
 @click.option('-w', '--workspace', 'ws_name', default=None, show_default=True,
               help='Name of workspace. Auto-detect by default.')
 @click.option('-m', '--model_config', 'mc_name', default=None, show_default=True,
               help='Name of model config. Auto-detect by default.')
 @click.option('-d', '--data', 'data_name', default='combData', show_default=True,
               help='Name of dataset.')
 @click.option('-s', '--snapshot', 'snapshot_name', default=None, show_default=True,
               help='Name of initial snapshot.')
 @click.option('-r', '--profile', 'profile_param', default="", show_default=True,
               help='Parameters to profile.')
 @click.option('-f', '--fix', 'fix_param', default="", show_default=True,
               help='Parameters to fix.')
-@click.option('--pois', default="", show_default=True,
-              help='Define the set of POIs (separated by commas) set for calculating Minos errors.')
 @click.option('--constrain/--no-constrain', 'constrain_nuis', default=True, show_default=True,
               help='Use constrained NLL (i.e. include systematics).')
-@click.option('--minos/--no-minos', default=False, show_default=True,
-              help='Evaluate errors using Minos.')
+@click.option('--minos', default="", show_default=True,
+              help='Set of POIs (separated by commas) for evaluating errors with Minos.')
 @click.option('-t', '--minimizer_type', default="Minuit2", show_default=True,
               help='Minimizer type.')
 @click.option('-a', '--minimizer_algo', default="Migrad", show_default=True,
               help='Minimizer algorithm.')
 @click.option('--strategy', type=int, default=1, show_default=True,
               help='Default minimization strategy.')
 @click.option('-e', '--eps', type=float, default=1.0, show_default=True,
@@ -82,41 +76,43 @@
 @click.option('-v', '--verbosity', default='INFO', show_default=True,
               type=click.Choice(["DEBUG", "INFO", "WARNING", "ERROR"], case_sensitive=False),
               help='Verbosity level.')
 def likelihood_fit(**kwargs):
     """
     Perform likelihood fit on a workspace
     """
+    
     from quickstats import stdout
-    do_minos = kwargs.pop("minos")
-    rebuild = kwargs.pop("rebuild")
     from quickstats.utils.string_utils import split_str
-    pois = split_str(kwargs.pop("pois"), sep=',', remove_empty=True)
+    from quickstats.components import AnalysisBase
+    from quickstats.concurrent.logging import standard_log
+    
+    rebuild = kwargs.pop("rebuild")
+    minos_pois = kwargs.pop("minos")
+    minos_pois = split_str(minos_pois, sep=',', remove_empty=True)
+    do_minos = len(minos_pois) > 0
+    do_pulls = kwargs['save_pulls'] is not None
     _kwargs = {}
-    for arg_name in ["outname", "save_log", "display", "save_result",
-                     "export_as_np_pulls", "outdir", "save_ws", "save_snapshot"]:
+    for arg_name in ["display", "save_result", "save_log",
+                     "save_pulls", "save_ws", "save_snapshot"]:
         _kwargs[arg_name] = kwargs.pop(arg_name)
     _init_kwargs = {}
     for arg_name in ["filename", "data_name", "verbosity"]:
         _init_kwargs[arg_name] = kwargs.pop(arg_name)
     _init_kwargs['config'] = kwargs
-    _init_kwargs['poi_name'] = pois
-    from quickstats.components import AnalysisBase
-    if _kwargs['save_log']:
-        from quickstats.concurrent.logging import standard_log
-        log_path = os.path.splitext(_kwargs["outname"])[0] + ".log"
-        with standard_log(log_path):
-            analysis = AnalysisBase(**_init_kwargs)
-            if _kwargs['export_as_np_pulls']:
-                analysis.minimizer.configure(hesse=True)
-            fit_result = analysis.nll_fit(mode=3, do_minos=do_minos)
-        stdout.info(f"Saved fit log to `{log_path}`")
-    else:
+    _init_kwargs['poi_name'] = minos_pois
+    log_path = _kwargs['save_log']
+    with standard_log(log_path):
         analysis = AnalysisBase(**_init_kwargs)
+        if do_pulls:
+            analysis.minimizer.configure(hesse=True)
         fit_result = analysis.nll_fit(mode=3, do_minos=do_minos)
+    if log_path:
+        stdout.info(f'Saved fit log as "{log_path}"')
+    analysis.stdout.verbosity = "SILENT"
     output = {}
     output['fit_result'] = fit_result
     df = {'pois':{}, 'nuisance_parameters':{}}
     analysis.load_snapshot("currentSnapshot")
     df['pois']['prefit'] = analysis.model.as_dataframe('poi')
     df['nuisance_parameters']['prefit'] = analysis.model.as_dataframe('nuisance_parameter')
     analysis.load_snapshot("nllFit")
@@ -137,45 +133,50 @@
             df[key]['combined']['errorlo_postfit'] = df[key]['postfit']['errorlo']
             df[key]['combined']['errorhi_postfit'] = df[key]['postfit']['errorhi']
         else:
             df[key]['combined']['error_postfit'] = df[key]['postfit']['error']
         output[key] = df[key]['combined'].to_dict("list")
         if _kwargs['display']:
             stdout.info(f"{key.title()}:\n{df[key]['combined']}\n\n")
-    if _kwargs['save_result']:
-        with open(_kwargs["outname"], "w") as f:
+    # save fit result
+    result_path = _kwargs['save_result']
+    if result_path:
+        with open(result_path, "w") as f:
             json.dump(output, f, indent=2)
-        stdout.info(f"Saved fit result to `{_kwargs['outname']}`")
-    if _kwargs['export_as_np_pulls']:
-        outdir = _kwargs['outdir']
-        if not os.path.exists(outdir):
-            os.makedirs(outdir, exist_ok=True)
+        stdout.info(f'Saved fit result as "{result_path}"')
+    # save pulls
+    pulls_dir = _kwargs['save_pulls']
+    if pulls_dir:
+        os.makedirs(pulls_dir, exist_ok=True)
         nuis_df = df[key]['combined'].drop(['min', 'max', 'is_constant', 'error_prefit'], axis=1)
         nuis_df = nuis_df.rename(columns={"value_prefit":"nuis_nom", "name":"nuisance", 
                                           "value_postfit":"nuis_hat", "error_postfit":"nuis_hi"})
         nuis_df["nuis_lo"] = nuis_df["nuis_hi"]
         nuis_df["nuis_prefit"] = 1.0
         nuis_df = nuis_df.set_index(['nuisance'])
         constrained_np = [i.GetName() for i in analysis.model.get_constrained_nuisance_parameters()]
         nuis_df = nuis_df.loc[constrained_np].reset_index()
         nuis_data = nuis_df.to_dict('index')
         for i in nuis_data:
             data = nuis_data[i]
             np_name = data['nuisance']
-            outpath = os.path.join(outdir, f"{np_name}.json")
+            outpath = os.path.join(pulls_dir, f"{np_name}.json")
             with open(outpath, "w") as outfile:
                 json.dump({"nuis": data}, outfile, indent=2)
-    if _kwargs["save_ws"] is not None:
-        filename = _kwargs["save_ws"]
-        if _kwargs["save_snapshot"] is not None:
-            snapshot_name = _kwargs["save_snapshot"]
+        stdout.info(f'Saved pull results to "{pulls_dir}"')
+    # save fitted workspace (and snapshot)
+    ws_path = _kwargs["save_ws"]
+    if ws_path:
+        snapshot_name = _kwargs["save_snapshot"]
+        if snapshot_name:
             from quickstats.components.basics import WSArgument
             analysis.save_snapshot(snapshot_name, WSArgument.MUTABLE)
             analysis.load_snapshot(analysis.kInitialSnapshotName)
-        analysis.save(filename, rebuild=rebuild)
+        analysis.save(ws_path, rebuild=rebuild)
+        stdout.info(f'Saved fitted workspace as "{ws_path}"')
 
 @cli.command(name='likelihood_scan')
 @click.option('-i', '--input_path', required=True, 
               help='Input directory/path containing the workspace file(s) to process.')
 @click.option('--file_expr', default=None, show_default=True,
               help='\b\n File name expression describing the external parameterisation.'
                    '\b\n Example: "<mass[F]>_kl_<klambda[P]>"'
```

### Comparing `quickstats-0.7.0.3/quickstats/clis/limit_setting.py` & `quickstats-0.7.0.4/quickstats/clis/limit_setting.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/clis/nuisance_parameter_tools.py` & `quickstats-0.7.0.4/quickstats/clis/nuisance_parameter_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/clis/processor_tools.py` & `quickstats-0.7.0.4/quickstats/clis/processor_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/clis/stat_tools.py` & `quickstats-0.7.0.4/quickstats/clis/stat_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/clis/workspace_tools.py` & `quickstats-0.7.0.4/quickstats/clis/workspace_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/__init__.py` & `quickstats-0.7.0.4/quickstats/components/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/analysis_base.py` & `quickstats-0.7.0.4/quickstats/components/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/analysis_object.py` & `quickstats-0.7.0.4/quickstats/components/analysis_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,15 @@
             self.stdout.info(f'POI set to "{poi_names[0]}"')
         elif len(poi_names) > 1:
             text = ", ".join([f'"{name}"' for name in poi_names])
             self.stdout.info(f'POIs set to {text}')
         
     def setup_model(self, **kwargs):
         model = ExtendedModel(**kwargs, verbosity=self.stdout.verbosity)
+        model.stdout = self.stdout
         self.model = model
     
     def setup_parameters(self, fix_param:str='', profile_param:str='', update_snapshot:bool=True):
         if not self.model:
             raise RuntimeError('uninitialized analysis object')
         fixed_parameters = []
         profiled_parameters = []
@@ -245,14 +246,15 @@
             if conditional_obs:
                 nll_options['conditional_observables'] = conditional_obs
             #nll_commands.append(ROOT.RooFit.ExternalConstraints(ROOT.RooArgSet()))
         
         minimizer_options = {k:v for k,v in kwargs.items() if k in ExtendedMinimizer._DEFAULT_MINIMIZER_OPTION_}
         minimizer.configure_nll(**nll_options)
         minimizer.configure(**minimizer_options)
+        minimizer.stdout = self.stdout
         self.minimizer = minimizer
         self.model.set_minimizer(self.minimizer)
         self.default_nll_options = nll_options
         self.default_minimizer_options = minimizer_options
     
     def set_data(self, data_name:str='combData'):
         if isinstance(data_name, ROOT.RooDataSet):
```

### Comparing `quickstats-0.7.0.3/quickstats/components/asimov_generator.py` & `quickstats-0.7.0.4/quickstats/components/asimov_generator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/asymptotic_cls.py` & `quickstats-0.7.0.4/quickstats/components/asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/basics.py` & `quickstats-0.7.0.4/quickstats/components/basics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/caching_nll_wrapper.py` & `quickstats-0.7.0.4/quickstats/components/caching_nll_wrapper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/discrete_nuisance.py` & `quickstats-0.7.0.4/quickstats/components/discrete_nuisance.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/extended_minimizer.py` & `quickstats-0.7.0.4/quickstats/components/extended_minimizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/extended_model.py` & `quickstats-0.7.0.4/quickstats/components/extended_model.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/extended_rfile.py` & `quickstats-0.7.0.4/quickstats/components/extended_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/likelihood.py` & `quickstats-0.7.0.4/quickstats/components/likelihood.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/modelling/component_source.py` & `quickstats-0.7.0.4/quickstats/components/modelling/component_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/modelling/data_modelling.py` & `quickstats-0.7.0.4/quickstats/components/modelling/data_modelling.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/modelling/model_source.py` & `quickstats-0.7.0.4/quickstats/components/modelling/model_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/modelling/parameter_templates.py` & `quickstats-0.7.0.4/quickstats/components/modelling/parameter_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/modelling/pdf_fit_tool.py` & `quickstats-0.7.0.4/quickstats/components/modelling/pdf_fit_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/modelling/tree_data_source.py` & `quickstats-0.7.0.4/quickstats/components/modelling/tree_data_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/nuisance_parameter_harmonizer.py` & `quickstats-0.7.0.4/quickstats/components/nuisance_parameter_harmonizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/nuisance_parameter_pull.py` & `quickstats-0.7.0.4/quickstats/components/nuisance_parameter_pull.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/nuisance_parameter_ranking.py` & `quickstats-0.7.0.4/quickstats/components/nuisance_parameter_ranking.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/__init__.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,8 +24,9 @@
 from .rooproc_load_frame import RooProcLoadFrame
 from .rooproc_as_numpy import RooProcAsNumpy
 from .rooproc_if_defined import RooProcIfDefined
 from .rooproc_if_not_defined import RooProcIfNotDefined
 from .rooproc_load_macro import RooProcLoadMacro
 from .rooproc_as_parquet import RooProcAsParquet
 from .rooproc_as_hdf import RooProcAsHDF
-from .rooproc_progressbar import RooProcProgressBar
+from .rooproc_progressbar import RooProcProgressBar
+from .rooproc_cache import RooProcCache
```

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_alias.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_as_hdf.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_as_hdf.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,29 +28,30 @@
             processor.stdout.info(f'Cached output from "{filename}".')
             return rdf, processor
         processor.stdout.info(f'Writing output to "{filename}".')
         import awkward as ak
         import pandas as pd
         columns = params.get('columns', None)
         exclude = params.get('exclude', None)
-        save_columns = self.get_save_columns(rdf, processor, columns=columns,
-                                             exclude=exclude,
-                                             mode="REMOVE_NON_STANDARD_TYPE")
-        array = None
-        if module_exist('awkward'):
-            try:
-                import awkward as ak
-                # NB: RDF Dask/Spark does not support GetColumnType yet
-                if processor.backend in [RDataFrameBackend.DASK, RDataFrameBackend.SPARK]:
-                    rdf.GetColumnType = rdf._headnode._localdf.GetColumnType
-                array = ak.from_rdataframe(rdf, columns=save_columns)
-                array = ak.to_numpy(array)
-            except:
-                array = None
-                processor.stdout.warning("Failed to convert output to numpy arrays with awkward backend. "
-                                         "Falling back to use ROOT instead")
-        if array is None:
-            array = rdf.AsNumpy(save_columns)
+        save_columns = self.resolve_columns(rdf, processor, columns=columns,
+                                            exclude=exclude,
+                                            mode="REMOVE_NON_STANDARD_TYPE")
+        array = rdf.AsNumpy(save_columns)
+        #array = None
+        #if module_exist('awkward'):
+        #    try:
+        #        import awkward as ak
+        #        # NB: RDF Dask/Spark does not support GetColumnType yet
+        #        if processor.backend in [RDataFrameBackend.DASK, RDataFrameBackend.SPARK]:
+        #            rdf.GetColumnType = rdf._headnode._localdf.GetColumnType
+        #        array = ak.from_rdataframe(rdf, columns=save_columns)
+        #        array = ak.to_numpy(array)
+        #    except:
+        #        array = None
+        #        processor.stdout.warning("Failed to convert output to numpy arrays with awkward backend. "
+        #                                 "Falling back to use ROOT instead")
+        #if array is None:
+        #    array = rdf.AsNumpy(save_columns)
         df = pd.DataFrame(array)
         self.makedirs(filename)
         df.to_hdf(filename, key=key)
         return rdf, processor
```

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_as_numpy.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_as_numpy.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,28 +19,29 @@
         filename = params['filename']
         if processor.cache and is_valid_file(filename):
             processor.stdout.info(f'Cached output from "{filename}".')
             return rdf, processor
         processor.stdout.info(f'Writing output to "{filename}".')
         columns = params.get('columns', None)
         exclude = params.get('exclude', None)
-        save_columns = self.get_save_columns(rdf, processor, columns=columns,
-                                             exclude=exclude,
-                                             mode="REMOVE_NON_STANDARD_TYPE")
-        array = None
-        if module_exist('awkward'):
-            try:
-                import awkward as ak
-                # NB: RDF Dask/Spark does not support GetColumnType yet
-                if processor.backend in [RDataFrameBackend.DASK, RDataFrameBackend.SPARK]:
-                    rdf.GetColumnType = rdf._headnode._localdf.GetColumnType
-                array = ak.from_rdataframe(rdf, columns=save_columns)
-                array = ak.to_numpy(array)
-            except:
-                array = None
-                processor.stdout.warning("Failed to convert output to numpy arrays with awkward backend. "
-                                         "Falling back to use ROOT instead")
-        if array is None:
-            array = rdf.AsNumpy(save_columns)
+        save_columns = self.resolve_columns(rdf, processor, columns=columns,
+                                            exclude=exclude,
+                                            mode="REMOVE_NON_STANDARD_TYPE")
+        array = rdf.AsNumpy(save_columns)
+        #array = None
+        #if module_exist('awkward'):
+        #    try:
+        #        import awkward as ak
+        #        # NB: RDF Dask/Spark does not support GetColumnType yet
+        #        if processor.backend in [RDataFrameBackend.DASK, RDataFrameBackend.SPARK]:
+        #            rdf.GetColumnType = rdf._headnode._localdf.GetColumnType
+        #        array = ak.from_rdataframe(rdf, columns=save_columns)
+        #        array = ak.to_numpy(array)
+        #    except:
+        #        array = None
+        #        processor.stdout.warning("Failed to convert output to numpy arrays with awkward backend. "
+        #                                 "Falling back to use ROOT instead")
+        #if array is None:
+        #    array = rdf.AsNumpy(save_columns)
         self.makedirs(filename)
         np.save(filename, array)
         return rdf, processor
```

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_as_parquet.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_as_parquet.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,17 @@
         filename = params['filename']
         if processor.cache and is_valid_file(filename):
             processor.stdout.info(f'Cached output from "{filename}".')
             return rdf, processor
         processor.stdout.info(f'Writing output to "{filename}".')
         columns = params.get('columns', None)
         exclude = params.get('exclude', None)
-        save_columns = self.get_save_columns(rdf, processor, columns=columns,
-                                             exclude=exclude,
-                                             mode="REMOVE_NON_STANDARD_TYPE")
+        save_columns = self.resolve_columns(rdf, processor, columns=columns,
+                                            exclude=exclude,
+                                            mode="REMOVE_NON_STANDARD_TYPE")
         import awkward as ak
         try:
             # NB: RDF Dask/Spark does not support GetColumnType yet
             if processor.backend in [RDataFrameBackend.DASK, RDataFrameBackend.SPARK]:
                 rdf.GetColumnType = rdf._headnode._localdf.GetColumnType
             array = ak.from_rdataframe(rdf, columns=save_columns)
         except:
```

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_base_action.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_base_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_declare.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_declare.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_define.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_define.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_export.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_export.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_global_variables.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_global_variables.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_hybrid_action.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_hybrid_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_if_defined.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_if_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_if_not_defined.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_if_not_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_load_frame.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_load_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_load_macro.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_load_macro.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_nested_action.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_nested_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_progressbar.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_progressbar.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_report.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_report.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_safe_alias.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_safe_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_safe_define.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_safe_define.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_save.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_save.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,18 +24,18 @@
         treename = params['treename']
         filename = params['filename']
         if processor.cache and is_valid_file(filename):
             processor.stdout.info(f'INFO: Cached output from "{filename}".')
             return rdf, processor
         columns = params.get('columns', None)
         exclude = params.get('exclude', None)
-        save_columns = self.get_save_columns(rdf, processor,
-                                             columns=columns,
-                                             exclude=exclude,
-                                             mode="ALL")
+        save_columns = self.resolve_columns(rdf, processor,
+                                            columns=columns,
+                                            exclude=exclude,
+                                            mode="ALL")
         processor.stdout.info(f'Writing output to "{filename}".')
         self.makedirs(filename)
         if processor.use_template:
             from quickstats.utils.root_utils import templated_rdf_snapshot 
             rdf_next = templated_rdf_snapshot(rdf, save_columns)(treename, filename, save_columns)
         else:
             rdf_next = rdf.Snapshot(treename, filename, save_columns)
```

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_save_frame.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_save_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_stat.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_stat.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/actions/rooproc_treename.py` & `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_treename.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/builtin_methods.py` & `quickstats-0.7.0.4/quickstats/components/processors/builtin_methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/roo_process_config.py` & `quickstats-0.7.0.4/quickstats/components/processors/roo_process_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,15 @@
         referenced_columns = self._get_columns(col_func, global_vars,
                                                exclude_global=exclude_global)
         if exclude_defined:
             defined_columns = self.get_defined_columns(global_vars=global_vars,
                                                        exclude_global=False)
             referenced_columns = [col for col in referenced_columns \
                                   if col not in defined_columns]
+        referenced_columns = sorted(referenced_columns)
         return referenced_columns
 
     def get_defined_columns(self, global_vars:Optional[Dict]=None,
                             exclude_global:bool=True):
         col_func = lambda node, glob_vars_: node.action.get_defined_columns(glob_vars_)
         return self._get_columns(col_func, global_vars,
                                  exclude_global=exclude_global)
```

### Comparing `quickstats-0.7.0.3/quickstats/components/processors/roo_processor.py` & `quickstats-0.7.0.4/quickstats/components/processors/roo_processor.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 import time
 import ROOT
 
 from .builtin_methods import BUILTIN_METHODS
 from .actions import *
 from .roo_process_config import RooProcessConfig
 
-from quickstats import timer, AbstractObject, PathManager, GeneralEnum
+from quickstats import timer, AbstractObject, PathManager, GeneralEnum, module_exist
 from quickstats.interface.root import TFile, RDataFrame, RDataFrameBackend
 from quickstats.interface.xrootd import get_cachedir, set_cachedir, switch_cachedir
 from quickstats.utils.root_utils import declare_expression, close_all_root_files, set_multithread
 from quickstats.utils.path_utils import is_remote_path
-from quickstats.utils.common_utils import get_cpu_count
+from quickstats.utils.common_utils import get_cpu_count, combine_dict
+from quickstats.daq import DEFAULT_CACHE_DIR, XRootDSource, ServiceXSource
 
 class RDFVerbosity(GeneralEnum):
     UNSET   = (0, 'kUnset')
     FATAL   = (1, 'kFatal')
     ERROR   = (2, 'kError')
     WARNING = (3, 'kWarning')
     INFO    = (4, 'kInfo')
@@ -26,27 +27,60 @@
 
     def __new__(cls, value:int, key:str):
         obj = object.__new__(cls)
         obj._value_ = value
         obj.key = key
         return obj
 
+class DataDeliveryService(GeneralEnum):
+    XROOTD   = (0, "XRootD")
+    SERVICEX = (1, "ServiceX")
+    
+    def __new__(cls, value:int, key:str):
+        obj = object.__new__(cls)
+        obj._value_ = value
+        obj.key = key
+        return obj
+
+DEFAULT_DATA_DELIVERY_OPTIONS = {
+    DataDeliveryService.XROOTD: {
+        "cachedir": DEFAULT_CACHE_DIR,
+        "local_cache": False,
+        "localize": False
+    },
+    DataDeliveryService.SERVICEX: {
+        "cachedir": DEFAULT_CACHE_DIR,
+        "local_cache": True,
+        "deliver_options": {
+            "batchsize" : None,
+            "retry" : 5,
+            "ignore_failure": True
+        }
+    }    
+}
+
+DATASOURCE_MAP = {
+    DataDeliveryService.XROOTD: XRootDSource,
+    DataDeliveryService.SERVICEX: ServiceXSource
+}
+
 class RooProcessor(AbstractObject):
 
     @property
     def distributed(self):
         return self.backend != RDataFrameBackend.DEFAULT
         
     def __init__(self, config_source:Optional[Union[RooProcessConfig, str]]=None,
-                 config_text:Optional[str]=None,
                  flags:Optional[List[str]]=None,
-                 backend:Optional[str]=None,
-                 backend_options:Optional[Dict]=None,
                  multithread:int=True,
                  cache:bool=False,
+                 backend:Optional[Union[str, RDataFrameBackend]]=None,
+                 backend_options:Optional[Dict]=None,
+                 data_service:Optional[Union[str, DataDeliveryService]]=None,
+                 data_service_options:Optional[Dict]=None,
                  use_template:bool=False,
                  verbosity:Optional[Union[int, str]]="INFO"):
         super().__init__(verbosity=verbosity)
         self.cache = cache
         self.action_tree = None
         if flags is not None:
             self.flags = list(flags)
@@ -56,52 +90,59 @@
         self.rdf = None
         self.global_variables = {}
         self.external_variables = {}
         self.default_treename = None
         self.use_template = use_template
         self.rdf_verbosity = None
         self.result_metadata = None
-        if backend is None:
-            self.backend = RDataFrameBackend.DEFAULT
-        else:
-            self.backend = RDataFrameBackend.parse(backend)
-        self.backend_options = backend_options
-        self.set_remote_file_options(localize=False,
-                                     cachedir=get_cachedir())
         self.set_profile_options()
+        self.set_backend(backend, backend_options)
+        self.set_data_service(data_service, data_service_options)
         self.load_buildin_functions()
 
         self.set_multithread(multithread)
         
         if config_source is not None:
             self.load_config(config_source)
 
+    def set_backend(self, backend:Optional[Union[str, RDataFrameBackend]]=None,
+                    options:Optional[Dict]=None):
+        if backend is None:
+            self.backend = RDataFrameBackend.DEFAULT
+        else:
+            self.backend = RDataFrameBackend.parse(backend)
+        # TODO: add default options
+        self.backend_options = combine_dict(options)
+
+    def set_data_service(self, service:Optional[Union[str, DataDeliveryService]]=None,
+                         options:Optional[Dict]=None):
+        # auto-detect by default
+        if service is None:
+            if module_exist("servicex"):
+                service = "servicex"
+            else:
+                service = "xrootd"            
+        service = DataDeliveryService.parse(service)
+        self.stdout.info(f"Using data delivery service: {service.key}")
+        self.data_service = service
+        default_options = DEFAULT_DATA_DELIVERY_OPTIONS[service]
+        self.data_service_options = combine_dict(default_options, options)    
+
     def set_multithread(self, num_threads:Optional[int]=None):
         if num_threads is None:
             num_threads = self.multithread
         num_threads = set_multithread(num_threads)
         if num_threads is None:
             self.stdout.info("Disabled multithreading.")
         else:
             self.stdout.info(f"Enabled multithreading with {num_threads} threads.")
         self.multithread = num_threads
             
     def set_cache(self, cache:bool=True):
         self.cache = cache
-        
-    def set_remote_file_options(self, localize:bool=False,
-                                cache:bool=True, cachedir:Optional[str]="/tmp",
-                                copy_options:Optional[Dict]=None):
-        remote_file_options = {
-            'localize': localize,
-            'cache': cache,
-            'cachedir': cachedir,
-            'copy_options': copy_options
-        }
-        self.remote_file_options = remote_file_options
 
     def set_profile_options(self, throughput:bool=False):
         profile_options = {
             "throughput": throughput
         }
         self.profile_options = profile_options
             
@@ -194,52 +235,34 @@
             
     def sanity_check(self):
         if not self.action_tree:
             raise RuntimeError("action tree not initialized")        
         if not self.action_tree.root_node.has_child:
             self.stdout.warning("No actions to be performed.")
             return None
-
-    @staticmethod
-    def _has_remote_files(filenames:List[str]):
-        return any(is_remote_path(filename) for filename in filenames)
-
-    def list_files(self, filenames:List[str], resolve_cache:bool=True):
-        cachedir = self.remote_file_options['cachedir']
-        with switch_cachedir(cachedir):
-            files = TFile.list_files(filenames, resolve_cache=resolve_cache,
-                                     raise_on_error=False)
-        return files
-
-    def resolve_filenames(self, filenames:Union[List[str], str]):
-        filenames = self.list_files(filenames, resolve_cache=True)
-        if not filenames:
-            return []
-        has_remote_file = self._has_remote_files(filenames)
-        # copy remote files to local storage
-        if has_remote_file and self.remote_file_options['localize']:
-            remote_files = [filename for filename in filenames if is_remote_path(filename)]
-            self._copy_remote_files(remote_files)
-            filenames = self.list_files(filenames, resolve_cache=True)
+            
+    def get_source_files(self, filenames:Union[List[str], str]):
+        data_source_cls = DATASOURCE_MAP[self.data_service]
+        data_service_options = self.data_service_options.copy()
+        if self.data_service == DataDeliveryService.SERVICEX:
+            data_service_options["columns"] = self.get_referenced_columns()
+        deliver_options = data_service_options.pop("deliver_options", {})
+        data_source = data_source_cls(**data_service_options)
+        data_source.add_files(filenames)
+        filenames = data_source.deliver(**deliver_options)
+        if self.data_service == DataDeliveryService.SERVICEX:
+            # TO FIX
+            self.default_treename = "servicex"
         return filenames
-
-    def _copy_remote_files(self, filenames:List[str]):
-        opts = self.remote_file_options
-        copy_options = opts.get('copy_options', None)
-        if copy_options is None:
-            copy_options = {}
-        TFile.copy_remote_files(filenames, cache=opts['cache'],
-                                 cachedir=opts['cachedir'],
-                                 **copy_options)
         
     def load_rdf(self,
                  filenames:Union[List[str], str],
                  treename:Optional[str]=None):
             
-        filenames = self.resolve_filenames(filenames)
+        filenames = self.get_source_files(filenames)
         if not filenames:
             self.stdout.info('No files to be processed. Skipping.')
             return None
         self._filenames = filenames
 
         if treename is None:
             treename = self.default_treename
@@ -283,19 +306,31 @@
         if rdf is None:
             raise RuntimeError('RDataFrame instance not initialized')
         return rdf
 
     def get_referenced_columns(self):
         action_tree = self.action_tree
         return action_tree.get_referenced_columns(self.global_variables)
+
+    def resolve_columns(self, frame:Optional[str]=None,
+                        columns:Optional[List[str]]=None,
+                        exclude:Optional[List[str]]=None,
+                        mode:str="ALL"):
+        rdf = self.get_rdf(frame)
+        selected_columns, _ = RDataFrame._resolve_columns(rdf=rdf,
+                                                          columns=columns,
+                                                          exclude=exclude,
+                                                          mode=mode)
+        return selected_columns
         
     def awkward_array(self, frame:Optional[str]=None,
                       columns:Optional[List[str]]=None):
         rdf = self.get_rdf(frame)
-        return RDataFrame._awkward_array(rdf, columns=columns)
+        selected_columns = self.resolve_columns(frame, columns=columns)
+        return RDataFrame._awkward_array(rdf, columns=selected_columns)
 
     def display(self, frame:Optional[str]=None,
                 columns:Union[str, List[str]]="",
                 n_rows:int=5, n_max_collection_elements:int=10,
                 lazy:bool=False):
         rdf = self.get_rdf(frame)
         result = self.rdf.Display(columns, n_rows, n_max_collection_elements)
```

### Comparing `quickstats-0.7.0.3/quickstats/components/pvalue_toys.py` & `quickstats-0.7.0.4/quickstats/components/pvalue_toys.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/roo_inspector.py` & `quickstats-0.7.0.4/quickstats/components/roo_inspector.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/root_object.py` & `quickstats-0.7.0.4/quickstats/components/root_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/toy_limit_calculator.py` & `quickstats-0.7.0.4/quickstats/components/toy_limit_calculator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/workspaces/__init__.py` & `quickstats-0.7.0.4/quickstats/components/workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/workspaces/asimov_handler.py` & `quickstats-0.7.0.4/quickstats/components/workspaces/asimov_handler.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/workspaces/core_argument_sets.py` & `quickstats-0.7.0.4/quickstats/components/workspaces/core_argument_sets.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/workspaces/sample.py` & `quickstats-0.7.0.4/quickstats/components/workspaces/sample.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/workspaces/settings.py` & `quickstats-0.7.0.4/quickstats/components/workspaces/settings.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/workspaces/systematic.py` & `quickstats-0.7.0.4/quickstats/components/workspaces/systematic.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/workspaces/systematics_domain.py` & `quickstats-0.7.0.4/quickstats/components/workspaces/systematics_domain.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/workspaces/ws_comparer.py` & `quickstats-0.7.0.4/quickstats/components/workspaces/ws_comparer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/workspaces/ws_decomposer.py` & `quickstats-0.7.0.4/quickstats/components/workspaces/ws_decomposer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/workspaces/ws_modifier_config.py` & `quickstats-0.7.0.4/quickstats/components/workspaces/ws_modifier_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/workspaces/xml_ws_base.py` & `quickstats-0.7.0.4/quickstats/components/workspaces/xml_ws_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/workspaces/xml_ws_builder_v1.py` & `quickstats-0.7.0.4/quickstats/components/workspaces/xml_ws_builder_v1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/workspaces/xml_ws_builder_v2.py` & `quickstats-0.7.0.4/quickstats/components/workspaces/xml_ws_builder_v2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/workspaces/xml_ws_combiner.py` & `quickstats-0.7.0.4/quickstats/components/workspaces/xml_ws_combiner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/components/workspaces/xml_ws_modifier.py` & `quickstats-0.7.0.4/quickstats/components/workspaces/xml_ws_modifier.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/concurrent/abstract_runner.py` & `quickstats-0.7.0.4/quickstats/concurrent/abstract_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/concurrent/logging.py` & `quickstats-0.7.0.4/quickstats/concurrent/logging.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/concurrent/nuisance_parameter_ranking_runner.py` & `quickstats-0.7.0.4/quickstats/concurrent/nuisance_parameter_ranking_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/concurrent/parameterised_asymptotic_cls.py` & `quickstats-0.7.0.4/quickstats/concurrent/parameterised_asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/concurrent/parameterised_likelihood.py` & `quickstats-0.7.0.4/quickstats/concurrent/parameterised_likelihood.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/concurrent/parameterised_runner.py` & `quickstats-0.7.0.4/quickstats/concurrent/parameterised_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/concurrent/parameterised_significance.py` & `quickstats-0.7.0.4/quickstats/concurrent/parameterised_significance.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/core/abstract_object.py` & `quickstats-0.7.0.4/quickstats/core/abstract_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/core/configuration.py` & `quickstats-0.7.0.4/quickstats/core/configuration.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/core/constraints.py` & `quickstats-0.7.0.4/quickstats/core/constraints.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/core/decorators.py` & `quickstats-0.7.0.4/quickstats/core/decorators.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/core/enums.py` & `quickstats-0.7.0.4/quickstats/core/enums.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/core/io.py` & `quickstats-0.7.0.4/quickstats/core/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,22 +67,22 @@
 
 getThreads = True
 getMultiprocessing = True
 getProcesses = True
 
 @total_ordering
 class Verbosity(Enum):
-    IGNORE = (100, 'IGNORE')
+    SILENT = (100, 'SILENT')
     CRITICAL = (50, 'CRITICAL')
     ERROR = (40, 'ERROR')
     TIPS = (35, 'TIPS')
     WARNING = (30, 'WARNING')
     INFO = (20, 'INFO')
     DEBUG = (10, 'DEBUG')
-    NOTSET = (0, 'NOTSET')
+    IGNORE = (0, 'IGNORE')
     
     def __new__(cls, value:int, levelname:str=""):
         obj = object.__new__(cls)
         obj._value_ = value
         obj.levelname = levelname
         return obj    
     
@@ -155,15 +155,15 @@
     def critical(self, text:str='', color=None, bare:bool=False):
         self.__call__(text, Verbosity.CRITICAL, color=color, bare=bare)
 
     def debug(self, text:str='', color=None, bare:bool=False):
         self.__call__(text, Verbosity.DEBUG, color=color, bare=bare)
 
     def write(self, text:str='', color=None):
-        self.__call__(text, verbosity.IGNORE, color=color, bare=True)
+        self.__call__(text, verbosity.SILENT, color=color, bare=True)
         
     def set_format(self, fmt:Optional[str]=None):
         if fmt is None:
             fmt = self.DEFAULT_FORMAT
         self._formatter = logging.Formatter(fmt)
         
     def set_timefmt(self, datefmt:Optional[str]=None, msecfmt:Optional[str]=None):
```

### Comparing `quickstats-0.7.0.3/quickstats/core/metaclasses.py` & `quickstats-0.7.0.4/quickstats/core/metaclasses.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/core/methods.py` & `quickstats-0.7.0.4/quickstats/core/methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/core/path_manager.py` & `quickstats-0.7.0.4/quickstats/core/path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/core/setup.py` & `quickstats-0.7.0.4/quickstats/core/setup.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/core/type_validation.py` & `quickstats-0.7.0.4/quickstats/core/type_validation.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/core/virtual_trees.py` & `quickstats-0.7.0.4/quickstats/core/virtual_trees.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/extensions/extension_dataframe.py` & `quickstats-0.7.0.4/quickstats/extensions/extension_dataframe.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/cppyy/core.py` & `quickstats-0.7.0.4/quickstats/interface/cppyy/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/cppyy/macros.py` & `quickstats-0.7.0.4/quickstats/interface/cppyy/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/cppyy/vectorize.py` & `quickstats-0.7.0.4/quickstats/interface/cppyy/vectorize.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/kerberos/core.py` & `quickstats-0.7.0.4/quickstats/interface/kerberos/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/root/ModelConfig.py` & `quickstats-0.7.0.4/quickstats/interface/root/ModelConfig.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/root/RDataFrame.py` & `quickstats-0.7.0.4/quickstats/interface/root/RDataFrame.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import json
 from typing import Optional, Union, List, Dict
 from tempfile import NamedTemporaryFile
 
+import numpy as np
+
 import quickstats
 from quickstats import semistaticmethod, DescriptiveEnum
 from .TObject import TObject
 from .TChain import TChain
 from .TFile import TFile
 
 class RDataFrameBackend(DescriptiveEnum):
@@ -201,8 +203,46 @@
             self.stdout.warning("Creating RDataFrame from DatasetSpec is not supported " +\
                                f"with the {backend.name} backend. Fall back to default " +\
                                 "backend")
             backend = RDataFrameBackend.DEFAULT
         if backend_options is None:
             backend_options = {}
         kernel = self._get_kernel(backend)
-        return kernel(dataset_spec, **backend_options)
+        return kernel(dataset_spec, **backend_options)
+
+    @staticmethod
+    def _resolve_columns(rdf,
+                         columns:Optional[List[str]]=None,
+                         exclude:Optional[List[str]]=None,
+                         mode:str="ALL"):
+        from quickstats.utils.common_utils import filter_by_wildcards, remove_duplicates
+        from quickstats.utils.data_conversion import (root_datatypes, get_rdf_column_type,
+                                                      ConversionMode, reduce_vector_types)
+        all_columns = list([str(col) for col in rdf.GetColumnNames()])
+        
+        if columns is None:
+            columns = list(all_columns)
+        if exclude is None:
+            exclude = []
+        
+        selected_columns = filter_by_wildcards(all_columns, columns)
+        selected_columns = filter_by_wildcards(selected_columns, exclude, exclusion=True)
+        selected_columns = remove_duplicates(selected_columns)
+    
+        mode = ConversionMode.parse(mode)
+        if mode in [ConversionMode.REMOVE_NON_STANDARD_TYPE,
+                    ConversionMode.REMOVE_NON_ARRAY_TYPE]:
+            column_types = np.array([get_rdf_column_type(rdf, col) for col in selected_columns])
+            if mode == ConversionMode.REMOVE_NON_ARRAY_TYPE:
+                column_types = reduce_vector_types(column_types)
+            new_columns = list(np.array(selected_columns)[np.where(np.isin(column_types, root_datatypes))])
+            removed_columns = np.setdiff1d(selected_columns, new_columns)
+            selected_columns = new_columns
+        else:
+            removed_columns = []
+        return selected_columns, removed_columns
+
+    def resolve_columns(self,
+                        columns:Optional[List[str]]=None,
+                        exclude:Optional[List[str]]=None,
+                        mode:str="ALL"):
+        return self._resolve_columns(self.rdf, columns=columns, exclude=exclude, mode=mode)
```

### Comparing `quickstats-0.7.0.3/quickstats/interface/root/RooAbsArg.py` & `quickstats-0.7.0.4/quickstats/interface/root/RooAbsArg.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/root/RooAbsData.py` & `quickstats-0.7.0.4/quickstats/interface/root/RooAbsData.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/root/RooAbsPdf.py` & `quickstats-0.7.0.4/quickstats/interface/root/RooAbsPdf.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/root/RooArgSet.py` & `quickstats-0.7.0.4/quickstats/interface/root/RooArgSet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/root/RooCategory.py` & `quickstats-0.7.0.4/quickstats/interface/root/RooCategory.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/root/RooDataSet.py` & `quickstats-0.7.0.4/quickstats/interface/root/RooDataSet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/root/RooMsgService.py` & `quickstats-0.7.0.4/quickstats/interface/root/RooMsgService.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/root/RooRealVar.py` & `quickstats-0.7.0.4/quickstats/interface/root/RooRealVar.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/root/TChain.py` & `quickstats-0.7.0.4/quickstats/interface/root/TChain.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/root/TF1.py` & `quickstats-0.7.0.4/quickstats/interface/root/TF1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/root/TFile.py` & `quickstats-0.7.0.4/quickstats/interface/root/TFile.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import glob
 
 import numpy as np
 
 from quickstats import semistaticmethod
 from quickstats.utils.path_utils import (resolve_paths, is_remote_path, remote_glob,
                                          remote_isdir, remote_listdir, listdir,
-                                         local_file_exist, split_url,
-                                         remote_file_exist)
+                                         local_path_exists, split_uri,
+                                         remote_path_exists)
 from quickstats.utils.root_utils import is_corrupt
 from quickstats.utils.common_utils import in_notebook
 from quickstats.utils.sys_utils import bytes_to_readable
 from .TObject import TObject
 
 class TFile(TObject):
 
@@ -74,15 +74,15 @@
     @semistaticmethod
     def _filter_valid_filenames(self, filenames:List[str]):
         filenames = [filename for filename in filenames if self._is_valid_filename(filename)]
         return filenames
 
     @semistaticmethod
     def _get_cache_path(self, path:str, cachedir:str="/tmp"):
-        host, filename = split_url(path)
+        host, filename = split_uri(path)
         filename = filename.lstrip('/.~')
         cache_path = os.path.join(cachedir, filename)
         return cache_path
     
     @semistaticmethod
     def _resolve_cached_remote_paths(self, paths:List[str],
                                      strict_format:Optional[bool]=True,
@@ -128,17 +128,17 @@
         
         if resolve_cache:
             paths = self._resolve_cached_remote_paths(paths)
             
         # expand directories if necessary
         for path in paths:
             if is_remote_path(path):
-                if local_file_exist(path):
-                    host, path = split_url(path)
-                elif remote_file_exist(path):
+                if local_path_exists(path):
+                    host, path = split_uri(path)
+                elif remote_path_exists(path):
                     if expand_remote_files and remote_isdir(path):
                         filenames.extend(remote_listdir(path))
                     else:
                         filenames.append(path)
                 else:
                     self.stdout.warning(f'Remote file "{path}" does not exist')
             elif os.path.isdir(path):
@@ -254,16 +254,16 @@
         if isinstance(paths, str):
             paths = [paths]
         remote_paths = []
         for path in paths:
             if not is_remote_path(path):
                 self.stdout.warning(f"Not a remote file: {path}. Skipped.")
                 continue
-            if local_file_exist(path):
-                self.stdout.warning(f"Remote file {path} can be accessed locally. Skipped.")
+            if local_path_exists(path):
+                self.stdout.warning(f"Remote path {path} can be accessed locally. Skipped.")
                 continue
             remote_paths.append(path)
         from quickstats.interface.xrootd import switch_cachedir
         with switch_cachedir(cachedir):
             filenames = self.list_files(remote_paths, resolve_cache=cache,
                                         expand_remote_files=True)
         cached_files = [filename for filename in filenames if not is_remote_path(filename)]
```

### Comparing `quickstats-0.7.0.3/quickstats/interface/root/TH1.py` & `quickstats-0.7.0.4/quickstats/interface/root/TH1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/root/TH2.py` & `quickstats-0.7.0.4/quickstats/interface/root/TH2.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,24 +39,25 @@
         self.y_bin_width    = self.GetYBinWidthArray(h, self.dtype, self.underflow_bin, self.overflow_bin)
         self.x_bin_low_edge = self.GetXBinLowEdgeArray(h, self.dtype, self.underflow_bin, self.overflow_bin)
         self.y_bin_low_edge = self.GetYBinLowEdgeArray(h, self.dtype, self.underflow_bin, self.overflow_bin) 
         
     @staticmethod
     def GetBinContentArray(h, dtype:str='double', underflow_bin:bool=False, overflow_bin:bool=False):
         arr = h.GetArray()
-        n_bins_x = h.GetNbinsX()
-        n_bins_y = h.GetNbinsY()
         # account for underflow and overflow bins
-        size = (n_bins_x + 2) * (n_bins_y + 2)
+        n_bins_x = h.GetNbinsX() + 2
+        n_bins_y = h.GetNbinsY() + 2
+        size = n_bins_x * n_bins_y
         np_arr = c_array_to_np_array(arr, size=size)
-        np_arr = np_arr.reshape((n_bins_x + 2, n_bins_y + 2), order='F')
+        # NB: order used to be 'F' (fortran array ordering, or column-major ordering)
+        np_arr = np_arr.reshape((n_bins_x, n_bins_y), order='C')
         x_start = 1 if not underflow_bin else 0
         y_start = x_start
-        x_end = -1 if not overflow_bin else n_bins_x + 2
-        y_end = -1 if not overflow_bin else n_bins_y + 2
+        x_end = -1 if not overflow_bin else n_bins_x
+        y_end = -1 if not overflow_bin else n_bins_y
         np_arr = np_arr[x_start:x_end, y_start:y_end]
         return np_arr
     
     @staticmethod
     def GetXLabelArray(h:"ROOT.TH2"):
         return np.array(h.GetXaxis().GetLabels(), dtype=str)
     
@@ -111,15 +112,15 @@
         dtype = self.DTYPE_MAP.get(h.ClassName(), "double")
         data = self.GetBinContentArray(h, dtype)
         xlabels = self.GetXLabelArray(h)
         ylabels = self.GetYLabelArray(h)
         if not np.array_equal(xlabels, ylabels):
             raise RuntimeError("invalid correlation histogram: labels along x-axis and y-axis do not match")
         if (data.shape[0] != len(xlabels)) or (data.shape[1] != len(ylabels)):
-            raise RuntimeError("invaiid correlation histogram: size of matrix does not match number of labels")
+            raise RuntimeError("invalid correlation histogram: size of matrix does not match number of labels")
         _data = {}
         for i, label in enumerate(xlabels):
             _data[label] = data[:, i]
         import pandas as pd
         df = pd.DataFrame(_data)
         df.index = ylabels[::-1]
         df = df.loc[df.index[::-1]]
```

### Comparing `quickstats-0.7.0.3/quickstats/interface/root/TH3.py` & `quickstats-0.7.0.4/quickstats/interface/root/TH3.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,23 +57,23 @@
         x_end = -1 if not overflow_bin else n_bins_x + 2
         y_end = -1 if not overflow_bin else n_bins_y + 2
         z_end = -1 if not overflow_bin else n_bins_z + 2
         np_arr = np_arr[x_start:x_end, y_start:y_end, z_start:z_end]
         return np_arr
     
     @staticmethod
-    def GetXLabelArray(h:"ROOT.TH2"):
+    def GetXLabelArray(h:"ROOT.TH3"):
         return np.array(h.GetXaxis().GetLabels(), dtype=str)
     
     @staticmethod
-    def GetYLabelArray(h:"ROOT.TH2"):
+    def GetYLabelArray(h:"ROOT.TH3"):
         return np.array(h.GetYaxis().GetLabels(), dtype=str)
     
     @staticmethod
-    def GetZLabelArray(h:"ROOT.TH2"):
+    def GetZLabelArray(h:"ROOT.TH3"):
         return np.array(h.GetYaxis().GetLabels(), dtype=str)
     
     @staticmethod
     def GetAxisBinCenterArray(ax:"ROOT.TAxis", dtype:str='double', underflow_bin:int=0, overflow_bin:int=0):
         import ROOT
         c_vector = ROOT.TAxisUtils.GetBinCenterArray[dtype](ax, underflow_bin, overflow_bin)
         return TArrayData.vec_to_array(c_vector)
```

### Comparing `quickstats-0.7.0.3/quickstats/interface/root/__init__.py` & `quickstats-0.7.0.4/quickstats/interface/root/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/root/helper.py` & `quickstats-0.7.0.4/quickstats/interface/root/helper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/root/macros.py` & `quickstats-0.7.0.4/quickstats/interface/root/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/root/roofit_extension.py` & `quickstats-0.7.0.4/quickstats/interface/root/roofit_extension.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/interface/xrootd/filesystem.py` & `quickstats-0.7.0.4/quickstats/interface/xrootd/filesystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from XRootD.client.flags import StatInfoFlags
 from  XRootD.client import glob_funcs
 
 FILESYSTEMS = {}
 
 __all__ = ["FileSystem", "get_filesystem"]
 
-def split_url(url):
-    parsed_uri = urlparse(url)
+def split_uri(uri):
+    parsed_uri = urlparse(uri)
     domain = '{uri.scheme}://{uri.netloc}/'.format(uri=parsed_uri)
     path = parsed_uri.path
     if path.startswith("//"):
         path = path[1:]
     return domain, path
 
 class FileSystem(AbstractObject):
```

### Comparing `quickstats-0.7.0.3/quickstats/interface/xrootd/path.py` & `quickstats-0.7.0.4/quickstats/interface/xrootd/path.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from .filesystem import split_url, get_filesystem
+from .filesystem import split_uri, get_filesystem
 
 def _call_path_method(method:str, path:str, **kwargs):
-    domain, path = split_url(path)
+    domain, path = split_uri(path)
     filesystem = get_filesystem(domain)
     if not hasattr(filesystem, method):
         raise ValueError(f'not implemented method: {method}')
     return getattr(filesystem, method)(path, **kwargs)
 
 def listdir(path:str, **kwargs):
     return _call_path_method('listdir', path, **kwargs)
```

### Comparing `quickstats-0.7.0.3/quickstats/interface/xrootd/xrd_helper.py` & `quickstats-0.7.0.4/quickstats/interface/xrootd/xrd_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.stdout.info(f'Destination(s):\n' + '\n'.join(dst))
         with timer() as t:
             copy_process = CopyProcess()
             for src_i, dst_i in zip(src, dst):
                 copy_process.add_job(src_i, dst_i, force=force, **kwargs)
             copy_process.prepare()
             copy_process.run()
-        self.stdout.info(f"Copy finished. Total time taken: {t.interval}.")
+        self.stdout.info(f"Copy finished. Total time taken: {t.interval:.3f}s.")
 
     @semistaticmethod
     def copy_file_cli(self, src:str, dst:str, recursive:bool=False,
                       force:bool=False, allow_http:bool=False, pbar:bool=True,
                       retry:Optional[int]=None, silent:bool=False):
         options = []
         if allow_http:
@@ -54,8 +54,8 @@
         self.stdout.info(f'Copying remote file(s):\n' + '\n'.join(src))
         self.stdout.info(f'Destination(s):\n' + '\n'.join(dst))
         with timer() as t:
             for src_i, dst_i in zip(src, dst):
                 self.copy_file_cli(src_i, dst_i, recursive=recursive,
                                    force=force, allow_http=allow_http,
                                    pbar=pbar, retry=retry, silent=silent)
-        self.stdout.info(f"Copy finished. Total time taken: {t.interval}.")
+        self.stdout.info(f"Copy finished. Total time taken: {t.interval:.3f}s.")
```

### Comparing `quickstats-0.7.0.3/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx` & `quickstats-0.7.0.4/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h` & `quickstats-0.7.0.4/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx` & `quickstats-0.7.0.4/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h` & `quickstats-0.7.0.4/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/macros/QuickStatsCore/QStringUtils.cxx` & `quickstats-0.7.0.4/quickstats/macros/QuickStatsCore/QStringUtils.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx` & `quickstats-0.7.0.4/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/macros/QuickStatsCore/RooFitExt.cxx` & `quickstats-0.7.0.4/quickstats/macros/QuickStatsCore/RooFitExt.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/macros/QuickStatsCore/RooFitExt.h` & `quickstats-0.7.0.4/quickstats/macros/QuickStatsCore/RooFitExt.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/macros/ResponseFunction/ResponseFunction.cxx` & `quickstats-0.7.0.4/quickstats/macros/ResponseFunction/ResponseFunction.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/macros/ResponseFunction/ResponseFunction.h` & `quickstats-0.7.0.4/quickstats/macros/ResponseFunction/ResponseFunction.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx` & `quickstats-0.7.0.4/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h` & `quickstats-0.7.0.4/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/maths/interpolation.py` & `quickstats-0.7.0.4/quickstats/maths/interpolation.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/maths/numerics.py` & `quickstats-0.7.0.4/quickstats/maths/numerics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Union, Any, List, Dict, Optional, Tuple, Callable
 from fractions import Fraction
 import decimal
+import math
 
 ctx = decimal.Context()
 ctx.prec = 20
 
 # taken from https://stackoverflow.com/questions/38847690
 def float_to_str(f):
     """
@@ -183,18 +184,24 @@
     if rmin > rmax:
         raise ValueError('max range must be larger than min range')
     if require_finite and (not (np.isfinite(rmin) and np.isfinite(rmax))):
         raise ValueError(f'supplied range of [{rmin}, {rmax}] is not finite')
     return rmin, rmax
 
 def get_batch_slice_indices(totalsize:int, batchsize:int):
-    assert (totalsize > 0) and (batchsize > 0)
+    if not ((totalsize > 0) and (batchsize > 0)):
+        raise ValueError("Batch size and total size must be greater than zero")
     for i in range(0, totalsize, batchsize):
         yield (i, min(i + batchsize, totalsize))
         
+def get_nbatch(totalsize:int, batchsize:int):
+    if not ((totalsize > 0) and (batchsize > 0)):
+        raise ValueError("Batch size and total size must be greater than zero")
+    return math.ceil(totalsize / batchsize)
+        
 def safe_div(dividend, divisor, usenan:bool=False):
     out = np.full(dividend.shape, np.nan) if usenan else np.zeros_like(dividend)
     return np.divide(dividend, divisor, out=out, where=divisor!=0)
 
 # taken from https://stackoverflow.com/questions/11144513/
 def cartesian_product(*arrays):
     la = len(arrays)
```

### Comparing `quickstats-0.7.0.3/quickstats/maths/statistics.py` & `quickstats-0.7.0.4/quickstats/maths/statistics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/maths/statistics_jitted.py` & `quickstats-0.7.0.4/quickstats/maths/statistics_jitted.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/maths/symbolics.py` & `quickstats-0.7.0.4/quickstats/maths/symbolics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/parsers/param_parser.py` & `quickstats-0.7.0.4/quickstats/parsers/param_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/parsers/roo_param_setup_parser.py` & `quickstats-0.7.0.4/quickstats/parsers/roo_param_setup_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/__init__.py` & `quickstats-0.7.0.4/quickstats/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/abstract_plot.py` & `quickstats-0.7.0.4/quickstats/plots/abstract_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/bidirectional_bar_chart.py` & `quickstats-0.7.0.4/quickstats/plots/bidirectional_bar_chart.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/collective_data_plot.py` & `quickstats-0.7.0.4/quickstats/plots/collective_data_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/color_schemes.py` & `quickstats-0.7.0.4/quickstats/plots/color_schemes.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/core.py` & `quickstats-0.7.0.4/quickstats/plots/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/correlation_plot.py` & `quickstats-0.7.0.4/quickstats/plots/correlation_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/general_1D_plot.py` & `quickstats-0.7.0.4/quickstats/plots/general_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/general_2D_plot.py` & `quickstats-0.7.0.4/quickstats/plots/general_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/general_distribution_plot.py` & `quickstats-0.7.0.4/quickstats/plots/general_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/hypotest_inverter_plot.py` & `quickstats-0.7.0.4/quickstats/plots/hypotest_inverter_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/likelihood_1D_plot.py` & `quickstats-0.7.0.4/quickstats/plots/likelihood_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/likelihood_2D_plot.py` & `quickstats-0.7.0.4/quickstats/plots/likelihood_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/np_ranking_plot.py` & `quickstats-0.7.0.4/quickstats/plots/np_ranking_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/pdf_distribution_plot.py` & `quickstats-0.7.0.4/quickstats/plots/pdf_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/sample_purity_plot.py` & `quickstats-0.7.0.4/quickstats/plots/sample_purity_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/score_distribution_plot.py` & `quickstats-0.7.0.4/quickstats/plots/score_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/stat_plot_config.py` & `quickstats-0.7.0.4/quickstats/plots/stat_plot_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/template.py` & `quickstats-0.7.0.4/quickstats/plots/template.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/test_statistic_distribution_plot.py` & `quickstats-0.7.0.4/quickstats/plots/test_statistic_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/two_axis_1D_plot.py` & `quickstats-0.7.0.4/quickstats/plots/two_axis_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/upper_limit_1D_plot.py` & `quickstats-0.7.0.4/quickstats/plots/upper_limit_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/upper_limit_2D_plot.py` & `quickstats-0.7.0.4/quickstats/plots/upper_limit_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/upper_limit_3D_plot.py` & `quickstats-0.7.0.4/quickstats/plots/upper_limit_3D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/upper_limit_benchmark_plot.py` & `quickstats-0.7.0.4/quickstats/plots/upper_limit_benchmark_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/plots/variable_distribution_plot.py` & `quickstats-0.7.0.4/quickstats/plots/variable_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/root_checker.py` & `quickstats-0.7.0.4/quickstats/root_checker.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/utils/common_utils.py` & `quickstats-0.7.0.4/quickstats/utils/common_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import time
 import json
 import yaml
 import inspect
 import datetime
 import functools
 import collections.abc
+from collections import Counter
 
 import numpy as np
 
 class disable_cout:    
     def __enter__(self):
         import cppyy
         cppyy.gbl.std.cout.setstate(cppyy.gbl.std.ios_base.failbit)
@@ -525,8 +526,23 @@
     Parameters:
     lst (list): The list from which duplicates are to be removed.
 
     Returns:
     list: A new list containing the unique elements of the original list in the order they first appeared.
     """
     seen = set()
-    return [x for x in lst if not (x in seen or seen.add(x))]
+    return [x for x in lst if not (x in seen or seen.add(x))]
+    
+def list_diff(list1: List, list2: List) -> List:
+    """
+    Computes the multiset difference between two lists, considering the frequency of elements.
+    
+    Args:
+        list1 (List[int]): The primary list from which elements will be subtracted.
+        list2 (List[int]): The secondary list whose elements are subtracted from the first.
+    
+    Returns:
+        List[int]: A list containing elements from list1 with the counts reduced by the elements in list2.
+    """
+    # Calculate the difference using Counter, which accounts for element frequencies
+    difference_counter = Counter(list1) - Counter(list2)
+    return list(difference_counter.elements())
```

### Comparing `quickstats-0.7.0.3/quickstats/utils/data_conversion.py` & `quickstats-0.7.0.4/quickstats/utils/data_conversion.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/utils/hep_utils.py` & `quickstats-0.7.0.4/quickstats/utils/hep_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/utils/py_utils.py` & `quickstats-0.7.0.4/quickstats/utils/py_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/utils/roofit_utils.py` & `quickstats-0.7.0.4/quickstats/utils/roofit_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/utils/roostats_utils.py` & `quickstats-0.7.0.4/quickstats/utils/roostats_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/utils/root_utils.py` & `quickstats-0.7.0.4/quickstats/utils/root_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/utils/string_utils.py` & `quickstats-0.7.0.4/quickstats/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/utils/sys_utils.py` & `quickstats-0.7.0.4/quickstats/utils/sys_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats/utils/xml_tools.py` & `quickstats-0.7.0.4/quickstats/utils/xml_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.3/quickstats.egg-info/PKG-INFO` & `quickstats-0.7.0.4/quickstats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.7.0.3
+Version: 0.7.0.4
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.7.0.3/quickstats.egg-info/SOURCES.txt` & `quickstats-0.7.0.4/quickstats.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 quickstats/components/processors/actions/auxiliary.py
 quickstats/components/processors/actions/formatter.py
 quickstats/components/processors/actions/rooproc_alias.py
 quickstats/components/processors/actions/rooproc_as_hdf.py
 quickstats/components/processors/actions/rooproc_as_numpy.py
 quickstats/components/processors/actions/rooproc_as_parquet.py
 quickstats/components/processors/actions/rooproc_base_action.py
+quickstats/components/processors/actions/rooproc_cache.py
 quickstats/components/processors/actions/rooproc_declare.py
 quickstats/components/processors/actions/rooproc_define.py
 quickstats/components/processors/actions/rooproc_export.py
 quickstats/components/processors/actions/rooproc_filter.py
 quickstats/components/processors/actions/rooproc_global_variables.py
 quickstats/components/processors/actions/rooproc_helper_action.py
 quickstats/components/processors/actions/rooproc_hybrid_action.py
@@ -137,14 +138,18 @@
 quickstats/core/io.py
 quickstats/core/metaclasses.py
 quickstats/core/methods.py
 quickstats/core/path_manager.py
 quickstats/core/setup.py
 quickstats/core/type_validation.py
 quickstats/core/virtual_trees.py
+quickstats/daq/__init__.py
+quickstats/daq/remote_data_source.py
+quickstats/daq/servicex_source.py
+quickstats/daq/xrootd_source.py
 quickstats/extensions/__init__.py
 quickstats/extensions/extension_dataframe.py
 quickstats/interface/__init__.py
 quickstats/interface/cppyy/__init__.py
 quickstats/interface/cppyy/basic_methods.py
 quickstats/interface/cppyy/core.py
 quickstats/interface/cppyy/macros.py
@@ -171,15 +176,18 @@
 quickstats/interface/root/TObject.py
 quickstats/interface/root/__init__.py
 quickstats/interface/root/helper.py
 quickstats/interface/root/io.py
 quickstats/interface/root/macros.py
 quickstats/interface/root/roofit_extension.py
 quickstats/interface/servicex/__init__.py
+quickstats/interface/servicex/config.py
 quickstats/interface/servicex/core.py
+quickstats/interface/tinydb/__init__.py
+quickstats/interface/tinydb/methods.py
 quickstats/interface/xrootd/__init__.py
 quickstats/interface/xrootd/core.py
 quickstats/interface/xrootd/filesystem.py
 quickstats/interface/xrootd/path.py
 quickstats/interface/xrootd/xrd_helper.py
 quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
 quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
```

### Comparing `quickstats-0.7.0.3/setup.py` & `quickstats-0.7.0.4/setup.py`

 * *Files identical despite different names*


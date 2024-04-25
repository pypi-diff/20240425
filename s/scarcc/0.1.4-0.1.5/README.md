# Comparing `tmp/scarcc-0.1.4.tar.gz` & `tmp/scarcc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scarcc-0.1.4.tar", last modified: Thu Mar 28 22:13:23 2024, max compression
+gzip compressed data, was "scarcc-0.1.5.tar", last modified: Thu Apr 25 11:38:11 2024, max compression
```

## Comparing `scarcc-0.1.4.tar` & `scarcc-0.1.5.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 22:13:23.699186 scarcc-0.1.4/
--rw-rw-rw-   0        0        0     1085 2024-02-15 07:25:04.000000 scarcc-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1722 2024-03-28 22:13:23.697194 scarcc-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1211 2024-03-22 16:35:36.000000 scarcc-0.1.4/README.md
--rw-rw-rw-   0        0        0      500 2024-02-21 18:05:28.000000 scarcc-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-28 22:13:23.700184 scarcc-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      692 2024-03-28 22:12:42.000000 scarcc-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:13:20.552604 scarcc-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-03-28 22:13:20.880728 scarcc-0.1.4/src/scarcc/
--rw-rw-rw-   0        0        0      267 2024-02-15 07:22:40.000000 scarcc-0.1.4/src/scarcc/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:13:21.000406 scarcc-0.1.4/src/scarcc/data_analysis/
--rw-rw-rw-   0        0        0      559 2024-03-25 23:28:31.000000 scarcc-0.1.4/src/scarcc/data_analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:13:21.053265 scarcc-0.1.4/src/scarcc/data_analysis/drug_combination_response/
--rw-rw-rw-   0        0        0        0 2024-02-23 14:56:55.000000 scarcc-0.1.4/src/scarcc/data_analysis/drug_combination_response/__init__.py
--rw-rw-rw-   0        0        0      823 2024-03-25 22:50:09.000000 scarcc-0.1.4/src/scarcc/data_analysis/drug_combination_response/classification.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:13:21.286640 scarcc-0.1.4/src/scarcc/data_analysis/flux/
--rw-rw-rw-   0        0        0        0 2024-02-22 18:48:10.000000 scarcc-0.1.4/src/scarcc/data_analysis/flux/__init__.py
--rw-rw-rw-   0        0        0     7726 2024-02-23 15:25:50.000000 scarcc-0.1.4/src/scarcc/data_analysis/flux/carbon_allocation.py
--rw-rw-rw-   0        0        0        0 2024-02-15 07:22:40.000000 scarcc-0.1.4/src/scarcc/data_analysis/flux/flux_correction.py
--rw-rw-rw-   0        0        0     5784 2024-02-23 15:15:08.000000 scarcc-0.1.4/src/scarcc/data_analysis/flux/flux_ratio_analysis.py
--rw-rw-rw-   0        0        0     4966 2024-03-26 02:25:24.000000 scarcc-0.1.4/src/scarcc/data_analysis/flux/flux_snapshot.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:13:21.696544 scarcc-0.1.4/src/scarcc/data_analysis/growth/
--rw-rw-rw-   0        0        0        0 2024-02-20 23:08:37.000000 scarcc-0.1.4/src/scarcc/data_analysis/growth/__init__.py
--rw-rw-rw-   0        0        0     8441 2024-03-01 18:10:42.000000 scarcc-0.1.4/src/scarcc/data_analysis/growth/_pathway_summary.py
--rw-rw-rw-   0        0        0     2764 2024-03-25 23:40:17.000000 scarcc-0.1.4/src/scarcc/data_analysis/growth/growth_rate.py
--rw-rw-rw-   0        0        0     9151 2024-03-25 23:43:24.000000 scarcc-0.1.4/src/scarcc/data_analysis/growth/growth_summary.py
--rw-rw-rw-   0        0        0     1753 2024-03-14 00:45:31.000000 scarcc-0.1.4/src/scarcc/data_analysis/growth/plot_growth_curve.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:13:22.230116 scarcc-0.1.4/src/scarcc/data_analysis/plot/
--rw-rw-rw-   0        0        0        0 2024-02-23 15:27:03.000000 scarcc-0.1.4/src/scarcc/data_analysis/plot/__init__.py
--rw-rw-rw-   0        0        0     4089 2024-02-23 15:55:05.000000 scarcc-0.1.4/src/scarcc/data_analysis/plot/heatmap.py
--rw-rw-rw-   0        0        0     2254 2024-02-23 15:45:34.000000 scarcc-0.1.4/src/scarcc/data_analysis/plot/kde.py
--rw-rw-rw-   0        0        0     1059 2024-02-23 15:40:21.000000 scarcc-0.1.4/src/scarcc/data_analysis/plot/legend.py
--rw-rw-rw-   0        0        0     2115 2024-03-01 18:11:19.000000 scarcc-0.1.4/src/scarcc/data_analysis/plot/scatter.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:13:22.236101 scarcc-0.1.4/src/scarcc/preparation/
--rw-rw-rw-   0        0        0      264 2024-03-14 22:26:47.000000 scarcc-0.1.4/src/scarcc/preparation/__init__.py
--rw-rw-rw-   0        0        0     2056 2024-03-20 20:32:39.000000 scarcc-0.1.4/src/scarcc/preparation/find_directory.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:13:22.246075 scarcc-0.1.4/src/scarcc/preparation/metabolic_model/
--rw-rw-rw-   0        0        0      253 2024-02-27 18:05:15.000000 scarcc-0.1.4/src/scarcc/preparation/metabolic_model/__init__.py
--rw-rw-rw-   0        0        0     5924 2024-03-22 20:07:00.000000 scarcc-0.1.4/src/scarcc/preparation/metabolic_model/basic_model.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:13:22.483443 scarcc-0.1.4/src/scarcc/preparation/metabolic_model/core/
--rw-rw-rw-   0        0        0      205 2024-02-15 17:45:27.000000 scarcc-0.1.4/src/scarcc/preparation/metabolic_model/core/__init__.py
--rw-rw-rw-   0        0        0     5272 2024-03-25 21:05:43.000000 scarcc-0.1.4/src/scarcc/preparation/metabolic_model/core/component.py
--rw-rw-rw-   0        0        0     2439 2024-03-22 19:56:46.000000 scarcc-0.1.4/src/scarcc/preparation/metabolic_model/core/flux_weighting.py
--rw-rw-rw-   0        0        0     1771 2024-03-25 21:04:43.000000 scarcc-0.1.4/src/scarcc/preparation/metabolic_model/core/medium.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:13:22.486431 scarcc-0.1.4/src/scarcc/preparation/perturbation/
--rw-rw-rw-   0        0        0      125 2024-02-20 16:56:52.000000 scarcc-0.1.4/src/scarcc/preparation/perturbation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:13:22.712825 scarcc-0.1.4/src/scarcc/preparation/perturbation/alpha_finder/
--rw-rw-rw-   0        0        0       97 2024-03-14 22:26:47.000000 scarcc-0.1.4/src/scarcc/preparation/perturbation/alpha_finder/__init__.py
--rw-rw-rw-   0        0        0     8603 2024-03-26 20:40:55.000000 scarcc-0.1.4/src/scarcc/preparation/perturbation/alpha_finder/alpha_finder.py
--rw-rw-rw-   0        0        0    12229 2024-03-23 00:20:37.000000 scarcc-0.1.4/src/scarcc/preparation/perturbation/alpha_finder/checkerboard.py
--rw-rw-rw-   0        0        0    14230 2024-03-23 00:28:37.000000 scarcc-0.1.4/src/scarcc/preparation/perturbation/alpha_finder/coculture.py
--rw-rw-rw-   0        0        0    16012 2024-03-28 22:06:39.000000 scarcc-0.1.4/src/scarcc/preparation/perturbation/alpha_finder/monoculture.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:13:23.051921 scarcc-0.1.4/src/scarcc/preparation/perturbation/function/
--rw-rw-rw-   0        0        0      107 2024-02-15 20:12:37.000000 scarcc-0.1.4/src/scarcc/preparation/perturbation/function/__init__.py
--rw-rw-rw-   0        0        0     1344 2024-03-23 02:15:32.000000 scarcc-0.1.4/src/scarcc/preparation/perturbation/function/iter_species.py
--rw-rw-rw-   0        0        0     4748 2024-03-20 13:20:40.000000 scarcc-0.1.4/src/scarcc/preparation/perturbation/function/stoichiometry_scaling.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:13:23.148660 scarcc-0.1.4/src/scarcc/preparation/target_gene/
--rw-rw-rw-   0        0        0        0 2024-02-15 07:22:40.000000 scarcc-0.1.4/src/scarcc/preparation/target_gene/__init__.py
--rw-rw-rw-   0        0        0     4786 2024-03-23 02:30:34.000000 scarcc-0.1.4/src/scarcc/preparation/target_gene/gene_format_handler.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:13:23.388019 scarcc-0.1.4/src/scarcc/sim_engine/
--rw-rw-rw-   0        0        0        0 2024-02-15 07:22:40.000000 scarcc-0.1.4/src/scarcc/sim_engine/__init__.py
--rw-rw-rw-   0        0        0     4173 2024-03-26 00:43:33.000000 scarcc-0.1.4/src/scarcc/sim_engine/checkerboard_workflow.py
--rw-rw-rw-   0        0        0     5900 2024-03-26 23:35:39.000000 scarcc-0.1.4/src/scarcc/sim_engine/flux_extraction.py
--rw-rw-rw-   0        0        0    10971 2024-03-27 00:05:21.000000 scarcc-0.1.4/src/scarcc/sim_engine/output.py
--rw-rw-rw-   0        0        0     6517 2024-03-25 22:14:27.000000 scarcc-0.1.4/src/scarcc/sim_engine/simulation_configuration.py
--rw-rw-rw-   0        0        0    10695 2024-03-27 00:06:37.000000 scarcc-0.1.4/src/scarcc/sim_engine/simulation_workflow.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:13:23.396996 scarcc-0.1.4/src/scarcc/utils/
--rw-rw-rw-   0        0        0       94 2024-02-15 17:51:16.000000 scarcc-0.1.4/src/scarcc/utils/__init__.py
--rw-rw-rw-   0        0        0     1506 2024-03-25 22:51:28.000000 scarcc-0.1.4/src/scarcc/utils/util.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:13:23.684227 scarcc-0.1.4/src/scarcc.egg-info/
--rw-rw-rw-   0        0        0     1722 2024-03-28 22:13:18.000000 scarcc-0.1.4/src/scarcc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2667 2024-03-28 22:13:19.000000 scarcc-0.1.4/src/scarcc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 22:13:18.000000 scarcc-0.1.4/src/scarcc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-03-28 22:13:18.000000 scarcc-0.1.4/src/scarcc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-28 22:13:18.000000 scarcc-0.1.4/src/scarcc.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-28 22:13:23.650317 scarcc-0.1.4/test/
--rw-rw-rw-   0        0        0      529 2024-02-23 15:06:29.000000 scarcc-0.1.4/test/test_Everything.py
--rw-rw-rw-   0        0        0     1572 2024-03-19 23:07:25.000000 scarcc-0.1.4/test/test_GeneFormatHandler.py
--rw-rw-rw-   0        0        0      676 2024-02-15 17:49:12.000000 scarcc-0.1.4/test/test_basic_model.py
--rw-rw-rw-   0        0        0      500 2024-03-02 00:40:54.000000 scarcc-0.1.4/test/test_growth_rate.py
--rw-rw-rw-   0        0        0      977 2024-03-14 22:26:47.000000 scarcc-0.1.4/test/test_monoculture_search.py
--rw-rw-rw-   0        0        0     2244 2024-03-12 03:13:43.000000 scarcc-0.1.4/test/test_simulation_workflow.py
--rw-rw-rw-   0        0        0     1612 2024-02-15 23:36:03.000000 scarcc-0.1.4/test/test_stoichiometry_scaling.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:38:11.458814 scarcc-0.1.5/
+-rw-rw-rw-   0        0        0     1085 2024-02-15 07:25:04.000000 scarcc-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1480 2024-04-25 11:38:11.457817 scarcc-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1211 2024-03-22 16:35:36.000000 scarcc-0.1.5/README.md
+-rw-rw-rw-   0        0        0      500 2024-02-21 18:05:28.000000 scarcc-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 11:38:11.459812 scarcc-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      692 2024-04-25 11:37:33.000000 scarcc-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:38:10.170262 scarcc-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-25 11:38:10.423584 scarcc-0.1.5/src/scarcc/
+-rw-rw-rw-   0        0        0      267 2024-02-15 07:22:40.000000 scarcc-0.1.5/src/scarcc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:38:10.511349 scarcc-0.1.5/src/scarcc/data_analysis/
+-rw-rw-rw-   0        0        0      559 2024-03-25 23:28:31.000000 scarcc-0.1.5/src/scarcc/data_analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:38:10.574181 scarcc-0.1.5/src/scarcc/data_analysis/drug_combination_response/
+-rw-rw-rw-   0        0        0        0 2024-02-23 14:56:55.000000 scarcc-0.1.5/src/scarcc/data_analysis/drug_combination_response/__init__.py
+-rw-rw-rw-   0        0        0      823 2024-03-25 22:50:09.000000 scarcc-0.1.5/src/scarcc/data_analysis/drug_combination_response/classification.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:38:10.607093 scarcc-0.1.5/src/scarcc/data_analysis/flux/
+-rw-rw-rw-   0        0        0        0 2024-02-22 18:48:10.000000 scarcc-0.1.5/src/scarcc/data_analysis/flux/__init__.py
+-rw-rw-rw-   0        0        0     7756 2024-03-28 22:47:05.000000 scarcc-0.1.5/src/scarcc/data_analysis/flux/carbon_allocation.py
+-rw-rw-rw-   0        0        0        0 2024-02-15 07:22:40.000000 scarcc-0.1.5/src/scarcc/data_analysis/flux/flux_correction.py
+-rw-rw-rw-   0        0        0     5784 2024-02-23 15:15:08.000000 scarcc-0.1.5/src/scarcc/data_analysis/flux/flux_ratio_analysis.py
+-rw-rw-rw-   0        0        0     4966 2024-03-26 02:25:24.000000 scarcc-0.1.5/src/scarcc/data_analysis/flux/flux_snapshot.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:38:10.629037 scarcc-0.1.5/src/scarcc/data_analysis/growth/
+-rw-rw-rw-   0        0        0        0 2024-02-20 23:08:37.000000 scarcc-0.1.5/src/scarcc/data_analysis/growth/__init__.py
+-rw-rw-rw-   0        0        0     8441 2024-03-01 18:10:42.000000 scarcc-0.1.5/src/scarcc/data_analysis/growth/_pathway_summary.py
+-rw-rw-rw-   0        0        0     2764 2024-03-25 23:40:17.000000 scarcc-0.1.5/src/scarcc/data_analysis/growth/growth_rate.py
+-rw-rw-rw-   0        0        0     9151 2024-03-25 23:43:24.000000 scarcc-0.1.5/src/scarcc/data_analysis/growth/growth_summary.py
+-rw-rw-rw-   0        0        0     1753 2024-03-14 00:45:31.000000 scarcc-0.1.5/src/scarcc/data_analysis/growth/plot_growth_curve.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:38:10.658954 scarcc-0.1.5/src/scarcc/data_analysis/plot/
+-rw-rw-rw-   0        0        0        0 2024-02-23 15:27:03.000000 scarcc-0.1.5/src/scarcc/data_analysis/plot/__init__.py
+-rw-rw-rw-   0        0        0     4089 2024-02-23 15:55:05.000000 scarcc-0.1.5/src/scarcc/data_analysis/plot/heatmap.py
+-rw-rw-rw-   0        0        0     2254 2024-02-23 15:45:34.000000 scarcc-0.1.5/src/scarcc/data_analysis/plot/kde.py
+-rw-rw-rw-   0        0        0     1059 2024-02-23 15:40:21.000000 scarcc-0.1.5/src/scarcc/data_analysis/plot/legend.py
+-rw-rw-rw-   0        0        0     2115 2024-03-01 18:11:19.000000 scarcc-0.1.5/src/scarcc/data_analysis/plot/scatter.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:38:10.675909 scarcc-0.1.5/src/scarcc/preparation/
+-rw-rw-rw-   0        0        0      264 2024-03-14 22:26:47.000000 scarcc-0.1.5/src/scarcc/preparation/__init__.py
+-rw-rw-rw-   0        0        0     2056 2024-03-20 20:32:39.000000 scarcc-0.1.5/src/scarcc/preparation/find_directory.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:38:10.719793 scarcc-0.1.5/src/scarcc/preparation/metabolic_model/
+-rw-rw-rw-   0        0        0      253 2024-02-27 18:05:15.000000 scarcc-0.1.5/src/scarcc/preparation/metabolic_model/__init__.py
+-rw-rw-rw-   0        0        0     5974 2024-04-25 11:36:44.000000 scarcc-0.1.5/src/scarcc/preparation/metabolic_model/basic_model.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:38:10.789605 scarcc-0.1.5/src/scarcc/preparation/metabolic_model/core/
+-rw-rw-rw-   0        0        0      205 2024-02-15 17:45:27.000000 scarcc-0.1.5/src/scarcc/preparation/metabolic_model/core/__init__.py
+-rw-rw-rw-   0        0        0     5272 2024-03-25 21:05:43.000000 scarcc-0.1.5/src/scarcc/preparation/metabolic_model/core/component.py
+-rw-rw-rw-   0        0        0     2439 2024-03-22 19:56:46.000000 scarcc-0.1.5/src/scarcc/preparation/metabolic_model/core/flux_weighting.py
+-rw-rw-rw-   0        0        0     1771 2024-03-25 21:04:43.000000 scarcc-0.1.5/src/scarcc/preparation/metabolic_model/core/medium.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:38:10.793594 scarcc-0.1.5/src/scarcc/preparation/perturbation/
+-rw-rw-rw-   0        0        0      125 2024-02-20 16:56:52.000000 scarcc-0.1.5/src/scarcc/preparation/perturbation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:38:10.906292 scarcc-0.1.5/src/scarcc/preparation/perturbation/alpha_finder/
+-rw-rw-rw-   0        0        0       97 2024-03-14 22:26:47.000000 scarcc-0.1.5/src/scarcc/preparation/perturbation/alpha_finder/__init__.py
+-rw-rw-rw-   0        0        0     8603 2024-03-26 20:40:55.000000 scarcc-0.1.5/src/scarcc/preparation/perturbation/alpha_finder/alpha_finder.py
+-rw-rw-rw-   0        0        0    12229 2024-03-23 00:20:37.000000 scarcc-0.1.5/src/scarcc/preparation/perturbation/alpha_finder/checkerboard.py
+-rw-rw-rw-   0        0        0    14230 2024-03-23 00:28:37.000000 scarcc-0.1.5/src/scarcc/preparation/perturbation/alpha_finder/coculture.py
+-rw-rw-rw-   0        0        0    16012 2024-03-28 22:06:39.000000 scarcc-0.1.5/src/scarcc/preparation/perturbation/alpha_finder/monoculture.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:38:11.038939 scarcc-0.1.5/src/scarcc/preparation/perturbation/function/
+-rw-rw-rw-   0        0        0      107 2024-02-15 20:12:37.000000 scarcc-0.1.5/src/scarcc/preparation/perturbation/function/__init__.py
+-rw-rw-rw-   0        0        0     1344 2024-03-23 02:15:32.000000 scarcc-0.1.5/src/scarcc/preparation/perturbation/function/iter_species.py
+-rw-rw-rw-   0        0        0     4748 2024-03-20 13:20:40.000000 scarcc-0.1.5/src/scarcc/preparation/perturbation/function/stoichiometry_scaling.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:38:11.221450 scarcc-0.1.5/src/scarcc/preparation/target_gene/
+-rw-rw-rw-   0        0        0        0 2024-02-15 07:22:40.000000 scarcc-0.1.5/src/scarcc/preparation/target_gene/__init__.py
+-rw-rw-rw-   0        0        0     4772 2024-03-28 23:26:27.000000 scarcc-0.1.5/src/scarcc/preparation/target_gene/gene_format_handler.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:38:11.306223 scarcc-0.1.5/src/scarcc/sim_engine/
+-rw-rw-rw-   0        0        0        0 2024-02-15 07:22:40.000000 scarcc-0.1.5/src/scarcc/sim_engine/__init__.py
+-rw-rw-rw-   0        0        0     4173 2024-03-26 00:43:33.000000 scarcc-0.1.5/src/scarcc/sim_engine/checkerboard_workflow.py
+-rw-rw-rw-   0        0        0     5900 2024-03-26 23:35:39.000000 scarcc-0.1.5/src/scarcc/sim_engine/flux_extraction.py
+-rw-rw-rw-   0        0        0    10971 2024-03-27 00:05:21.000000 scarcc-0.1.5/src/scarcc/sim_engine/output.py
+-rw-rw-rw-   0        0        0     6628 2024-04-25 11:36:00.000000 scarcc-0.1.5/src/scarcc/sim_engine/simulation_configuration.py
+-rw-rw-rw-   0        0        0    10695 2024-03-27 00:06:37.000000 scarcc-0.1.5/src/scarcc/sim_engine/simulation_workflow.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:38:11.311209 scarcc-0.1.5/src/scarcc/utils/
+-rw-rw-rw-   0        0        0       94 2024-02-15 17:51:16.000000 scarcc-0.1.5/src/scarcc/utils/__init__.py
+-rw-rw-rw-   0        0        0     1506 2024-03-25 22:51:28.000000 scarcc-0.1.5/src/scarcc/utils/util.py
+drwxrwxrwx   0        0        0        0 2024-04-25 11:38:10.492399 scarcc-0.1.5/src/scarcc.egg-info/
+-rw-rw-rw-   0        0        0     1480 2024-04-25 11:38:08.000000 scarcc-0.1.5/src/scarcc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2667 2024-04-25 11:38:09.000000 scarcc-0.1.5/src/scarcc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 11:38:08.000000 scarcc-0.1.5/src/scarcc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-25 11:38:08.000000 scarcc-0.1.5/src/scarcc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-25 11:38:08.000000 scarcc-0.1.5/src/scarcc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 11:38:11.454826 scarcc-0.1.5/test/
+-rw-rw-rw-   0        0        0      529 2024-02-23 15:06:29.000000 scarcc-0.1.5/test/test_Everything.py
+-rw-rw-rw-   0        0        0     1572 2024-03-19 23:07:25.000000 scarcc-0.1.5/test/test_GeneFormatHandler.py
+-rw-rw-rw-   0        0        0      676 2024-02-15 17:49:12.000000 scarcc-0.1.5/test/test_basic_model.py
+-rw-rw-rw-   0        0        0      500 2024-03-02 00:40:54.000000 scarcc-0.1.5/test/test_growth_rate.py
+-rw-rw-rw-   0        0        0      977 2024-03-14 22:26:47.000000 scarcc-0.1.5/test/test_monoculture_search.py
+-rw-rw-rw-   0        0        0     2244 2024-03-12 03:13:43.000000 scarcc-0.1.5/test/test_simulation_workflow.py
+-rw-rw-rw-   0        0        0     1612 2024-02-15 23:36:03.000000 scarcc-0.1.5/test/test_stoichiometry_scaling.py
```

### Comparing `scarcc-0.1.4/LICENSE` & `scarcc-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/PKG-INFO` & `scarcc-0.1.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,17 @@
 Metadata-Version: 2.1
 Name: scarcc
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://github.com/TFwongw/scarccpy
 Author: Thomas Wong
 Author-email: wong0755@umn.edu
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pandas<2.3
-Requires-Dist: matplotlib
-Requires-Dist: seaborn>0.11
-Requires-Dist: cobra
-Requires-Dist: cometspy
-Requires-Dist: scipy
 Provides-Extra: docs
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: sphinx_rtd_theme; extra == "docs"
+License-File: LICENSE
 
 
 # SCARCCpy - Simulation of Combined Antibiotics in Cross-feeding Communities
 
 SCARCC is a python package developed by the Harcombe Lab designed to identify synergistic interactions between antibiotics within our two-species cross-feeding microbial community. 
 
 This package utilizes [COBRA](https://github.com/opencobra/cobrapy) to analyze the perturbation effects caused by antibiotics in the genome-scale metabolic network using Flux Balance Analysis (FBA), and [COMETS](https://github.com/segrelab/cometspy) simulations to incorporate multispecies growth simulation using Dynamic Flux Balance Analysis (dFBA).
```

### Comparing `scarcc-0.1.4/README.md` & `scarcc-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/setup.py` & `scarcc-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='scarcc',
-    version='0.1.4',
+    version='0.1.5',
     url='https://github.com/TFwongw/scarccpy',
     author='Thomas Wong',
     author_email='wong0755@umn.edu',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(where="src"),
     package_dir = {"": "src"},
```

### Comparing `scarcc-0.1.4/src/scarcc/data_analysis/__init__.py` & `scarcc-0.1.5/src/scarcc/data_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/data_analysis/drug_combination_response/classification.py` & `scarcc-0.1.5/src/scarcc/data_analysis/drug_combination_response/classification.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/data_analysis/flux/carbon_allocation.py` & `scarcc-0.1.5/src/scarcc/data_analysis/flux/carbon_allocation.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,33 +59,34 @@
     carbon_allocation = pd.concat([carbon_allocation, waste_row])
     if format:
         carbon_allocation['percent'] = carbon_allocation['percent'].apply(lambda x: f'{x:.2%}')
     carbon_allocation['Gene_inhibition'] = s.name if isinstance(s.name, str) else s.name[0]
     carbon_allocation.index.name = 'reaction'
     return carbon_allocation
 
-def get_carbon_allocation_E_wide(E0, all_components, additive_threshold=0.05, flux_analysis_file='./Data/flux_analysis_m1.csv', gr_file='./Data/gr_DG_m1_normalized.csv', end_BM=None):
+def get_carbon_allocation_E_wide(E0, all_components, additive_threshold=0.05, flux_analysis_file='./Data/flux_analysis_m1.csv', gr_file='normalized_gr_DG_m1.csv', end_BM=None):
     # flux_analysis_full = pd.read_csv('./Data/flux_analysis_m1.csv', index_col=0)
     flux_analysis_full = pd.read_csv(flux_analysis_file, index_col=0)
     co_E = flux_analysis_full.query('Species=="E0"')
     if 'culture' in co_E.columns:
         co_E = co_E.query('culture=="coculture"')
     # if 'XG'in co_E.columns:
     #     co_E = co_E.query('XG=="DG"')
     gr_df = pd.read_csv(gr_file, index_col=0)
     # gr_df = pd.read_csv('./Data/gr_DG_m1_normalized.csv', index_col=0)
-    carbon_allocation_E = pd.concat(co_E.apply(lambda x: 
+    carbon_allocation_E = pd.concat(co_E.apply(lambda x:
                                             get_carbon_allocation_summary(x, E0, all_components,format=False), axis=1)
                                                 .tolist())
     carbon_allocation_rxns = get_carbon_allocation_summary(co_E.iloc[0], E0, all_components).index # carbon allocation fluxes
 
     carbon_allocation_E_wide = carbon_allocation_E.reset_index().pivot(index='Gene_inhibition',columns='reaction',values=['total_carbon', 'percent'])
     # carbon_allocation_E_pivot = carbon_allocation_E.pivot(index='Gene_inhibition',columns='reaction',values=['total_carbon', 'percent'])
     carbon_allocation_E_wide.columns = ['_'.join([col[0], col[1]]) for col in carbon_allocation_E_wide.columns]
-    carbon_allocation_E_wide = carbon_allocation_E_wide.merge(co_E[['XG']], left_index=True, right_index=True) # only E0
+    # if 'XG' in co_E.columns:
+    #     carbon_allocation_E_wide = carbon_allocation_E_wide.merge(co_E[['XG']], left_index=True, right_index=True) # only E0
     partial_convert_po_col = lambda x: convert_po_col(x, additive_threshold=additive_threshold)
     carbon_allocation_E_wide['Drug_comb_effect_coc'] = partial_convert_po_col(gr_df['po_diff_E0_coculture'])
     carbon_allocation_E_wide['Drug_comb_effect_Emono'] = partial_convert_po_col(gr_df['po_diff_E0_monoculture'])
     carbon_allocation_E_wide['Drug_comb_effect_Smono'] = partial_convert_po_col(gr_df['po_diff_S0_monoculture'])
 
     # return carbon_allocation_E_wide
     if 'BM_consortia_frac_binned' not in carbon_allocation_E_wide.columns and end_BM is not None:
```

### Comparing `scarcc-0.1.4/src/scarcc/data_analysis/flux/flux_ratio_analysis.py` & `scarcc-0.1.5/src/scarcc/data_analysis/flux/flux_ratio_analysis.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/data_analysis/flux/flux_snapshot.py` & `scarcc-0.1.5/src/scarcc/data_analysis/flux/flux_snapshot.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/data_analysis/growth/_pathway_summary.py` & `scarcc-0.1.5/src/scarcc/data_analysis/growth/_pathway_summary.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/data_analysis/growth/growth_rate.py` & `scarcc-0.1.5/src/scarcc/data_analysis/growth/growth_rate.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/data_analysis/growth/growth_summary.py` & `scarcc-0.1.5/src/scarcc/data_analysis/growth/growth_summary.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/data_analysis/growth/plot_growth_curve.py` & `scarcc-0.1.5/src/scarcc/data_analysis/growth/plot_growth_curve.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/data_analysis/plot/heatmap.py` & `scarcc-0.1.5/src/scarcc/data_analysis/plot/heatmap.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/data_analysis/plot/kde.py` & `scarcc-0.1.5/src/scarcc/data_analysis/plot/kde.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/data_analysis/plot/legend.py` & `scarcc-0.1.5/src/scarcc/data_analysis/plot/legend.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/data_analysis/plot/scatter.py` & `scarcc-0.1.5/src/scarcc/data_analysis/plot/scatter.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/preparation/find_directory.py` & `scarcc-0.1.5/src/scarcc/preparation/find_directory.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/preparation/metabolic_model/basic_model.py` & `scarcc-0.1.5/src/scarcc/preparation/metabolic_model/basic_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,11 +106,12 @@
         if self.E_carbon_byproduct_reuptake is False:
             logging.debug('GAL reuptake is turned off')
             self.E0.reactions.GALtex.upper_bound = 0
             self.E0.reactions.ACtex.upper_bound = 0
         self.set_ES_medium()
         self.all_components = get_all_components(self.E0, self.S0)
         if self.flux_weighting is True:
+            print('Flux weighting is turned on')
             logging.debug('Flux weighting is turned on')
             self.implement_flux_weighting()
         return self.E0, self.S0, self.all_components
```

### Comparing `scarcc-0.1.4/src/scarcc/preparation/metabolic_model/core/component.py` & `scarcc-0.1.5/src/scarcc/preparation/metabolic_model/core/component.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/preparation/metabolic_model/core/flux_weighting.py` & `scarcc-0.1.5/src/scarcc/preparation/metabolic_model/core/flux_weighting.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/preparation/metabolic_model/core/medium.py` & `scarcc-0.1.5/src/scarcc/preparation/metabolic_model/core/medium.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/preparation/perturbation/alpha_finder/alpha_finder.py` & `scarcc-0.1.5/src/scarcc/preparation/perturbation/alpha_finder/alpha_finder.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/preparation/perturbation/alpha_finder/checkerboard.py` & `scarcc-0.1.5/src/scarcc/preparation/perturbation/alpha_finder/checkerboard.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/preparation/perturbation/alpha_finder/coculture.py` & `scarcc-0.1.5/src/scarcc/preparation/perturbation/alpha_finder/coculture.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/preparation/perturbation/alpha_finder/monoculture.py` & `scarcc-0.1.5/src/scarcc/preparation/perturbation/alpha_finder/monoculture.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/preparation/perturbation/function/iter_species.py` & `scarcc-0.1.5/src/scarcc/preparation/perturbation/function/iter_species.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/preparation/perturbation/function/stoichiometry_scaling.py` & `scarcc-0.1.5/src/scarcc/preparation/perturbation/function/stoichiometry_scaling.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/preparation/target_gene/gene_format_handler.py` & `scarcc-0.1.5/src/scarcc/preparation/target_gene/gene_format_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,17 +97,17 @@
         self.gene_str = self.trim(gene_str)
         self.is_checkerboard_format = None
         self.DG = None
         self.first_gene = None
         self.second_gene = None
 
         self.SG = None
-        self.XG = None
         self.classify_XG()
         self.set_fs_gene()
+        self.XG = 'DG' if self.DG else 'SG'
 
     @staticmethod
     def trim(gene_str):
         """Remove Species and culture condition information from gene string"""
         replacements = ["[A-Z]0_", "_(coculture|monoculture)"] # TODO: remove all id in species list
         return re.sub('|'.join(replacements),'', gene_str)
 
@@ -117,15 +117,14 @@
             self.is_checkerboard_format = True
             genes, lvs = self.gene_str.split('_')
             self.first_gene, self.second_gene = [
                 '_'.join(ele) for ele in zip(genes.split('.'), lvs.split('.'))] # g1_l1, g2_l2 
             if '0' in lvs:
                 self.SG = self.gene_str
             else:
-                self.is_DG = True
                 self.DG = self.gene_str
         else:
             if '.' in self.gene_str:
                 self.DG = self.gene_str
             else:
                 self.SG = self.gene_str
```

### Comparing `scarcc-0.1.4/src/scarcc/sim_engine/checkerboard_workflow.py` & `scarcc-0.1.5/src/scarcc/sim_engine/checkerboard_workflow.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/sim_engine/flux_extraction.py` & `scarcc-0.1.5/src/scarcc/sim_engine/flux_extraction.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/sim_engine/output.py` & `scarcc-0.1.5/src/scarcc/sim_engine/output.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/sim_engine/simulation_configuration.py` & `scarcc-0.1.5/src/scarcc/sim_engine/simulation_configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,15 +66,20 @@
     # comets model specifications
     initial_pop: float = 1e-8
     obj_style: str = 'MAX_OBJECTIVE_MIN_TOTAL'
 
     def __post_init__(self):
         if self.mono is False:
             self.mono_E, self.mono_S = False, False
-        self.Smono_carbon_source = 'bulk_ac_e' if any('EX_bulk_ac_e' in ele.id for ele in self.S0.reactions) else 'ac_e'
+        
+        if any('EX_bulk_ac_e' in ele.id for ele in self.S0.reactions):
+            self.Smono_carbon_source = 'bulk_ac_e'
+        elif 'ac_e' in self.Smono_carbon_source:
+            self.Smono_carbon_source = 'ac_e'
+
         if self.base_nutrients is None:
             self.base_nutrients = [
                 "ca2_e", "cl_e", "cobalt2_e", "cu2_e","fe2_e", "fe3_e", "k_e", "mg2_e",
                 "mn2_e", "mobd_e", "ni2_e", "o2_e", "pi_e", "so4_e", "zn2_e", "nh4_e"]
         if self.carbon_source is None:
             self.carbon_source = {'co': 'lcts_e', 'mono_E': 'lcts_e', 'mono_S': self.Smono_carbon_source}
```

### Comparing `scarcc-0.1.4/src/scarcc/sim_engine/simulation_workflow.py` & `scarcc-0.1.5/src/scarcc/sim_engine/simulation_workflow.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc/utils/util.py` & `scarcc-0.1.5/src/scarcc/utils/util.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/src/scarcc.egg-info/PKG-INFO` & `scarcc-0.1.5/src/scarcc.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,17 @@
 Metadata-Version: 2.1
 Name: scarcc
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://github.com/TFwongw/scarccpy
 Author: Thomas Wong
 Author-email: wong0755@umn.edu
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pandas<2.3
-Requires-Dist: matplotlib
-Requires-Dist: seaborn>0.11
-Requires-Dist: cobra
-Requires-Dist: cometspy
-Requires-Dist: scipy
 Provides-Extra: docs
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: sphinx_rtd_theme; extra == "docs"
+License-File: LICENSE
 
 
 # SCARCCpy - Simulation of Combined Antibiotics in Cross-feeding Communities
 
 SCARCC is a python package developed by the Harcombe Lab designed to identify synergistic interactions between antibiotics within our two-species cross-feeding microbial community. 
 
 This package utilizes [COBRA](https://github.com/opencobra/cobrapy) to analyze the perturbation effects caused by antibiotics in the genome-scale metabolic network using Flux Balance Analysis (FBA), and [COMETS](https://github.com/segrelab/cometspy) simulations to incorporate multispecies growth simulation using Dynamic Flux Balance Analysis (dFBA).
```

### Comparing `scarcc-0.1.4/src/scarcc.egg-info/SOURCES.txt` & `scarcc-0.1.5/src/scarcc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/test/test_Everything.py` & `scarcc-0.1.5/test/test_Everything.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/test/test_GeneFormatHandler.py` & `scarcc-0.1.5/test/test_GeneFormatHandler.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/test/test_basic_model.py` & `scarcc-0.1.5/test/test_basic_model.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/test/test_monoculture_search.py` & `scarcc-0.1.5/test/test_monoculture_search.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/test/test_simulation_workflow.py` & `scarcc-0.1.5/test/test_simulation_workflow.py`

 * *Files identical despite different names*

### Comparing `scarcc-0.1.4/test/test_stoichiometry_scaling.py` & `scarcc-0.1.5/test/test_stoichiometry_scaling.py`

 * *Files identical despite different names*


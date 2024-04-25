# Comparing `tmp/rtc-tools-interface-0.7.3.tar.gz` & `tmp/rtc-tools-interface-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtc-tools-interface-0.7.3.tar", last modified: Tue Mar  5 10:32:43 2024, max compression
+gzip compressed data, was "rtc-tools-interface-0.7.4.tar", last modified: Thu Apr 25 14:36:24 2024, max compression
```

## Comparing `rtc-tools-interface-0.7.3.tar` & `rtc-tools-interface-0.7.4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 10:32:43.980459 rtc-tools-interface-0.7.3/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/COPYING.LESSER
--rw-r--r--   0 root         (0) root         (0)      268 2024-03-05 10:32:43.980459 rtc-tools-interface-0.7.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12418 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 10:32:43.972459 rtc-tools-interface-0.7.3/rtc_tools_interface.egg-info/
--rw-r--r--   0 root         (0) root         (0)      268 2024-03-05 10:32:43.000000 rtc-tools-interface-0.7.3/rtc_tools_interface.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1882 2024-03-05 10:32:43.000000 rtc-tools-interface-0.7.3/rtc_tools_interface.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-05 10:32:43.000000 rtc-tools-interface-0.7.3/rtc_tools_interface.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-03-05 10:32:43.000000 rtc-tools-interface-0.7.3/rtc_tools_interface.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-05 10:32:43.000000 rtc-tools-interface-0.7.3/rtc_tools_interface.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 10:32:43.981459 rtc-tools-interface-0.7.3/rtctools_interface/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2024-03-05 10:32:43.981459 rtc-tools-interface-0.7.3/rtctools_interface/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 10:32:43.974459 rtc-tools-interface-0.7.3/rtctools_interface/optimization/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/optimization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10183 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/optimization/base_goal.py
--rw-rw-rw-   0 root         (0) root         (0)     1066 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/optimization/base_optimization_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     4068 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/optimization/goal_generator_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     5055 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/optimization/goal_performance_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3613 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/optimization/goal_table_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 10:32:43.975459 rtc-tools-interface-0.7.3/rtctools_interface/optimization/helpers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/optimization/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3032 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/optimization/helpers/statistics_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)      401 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/optimization/plot_goals_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     2010 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/optimization/plot_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3292 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/optimization/read_goals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 10:32:43.975459 rtc-tools-interface-0.7.3/rtctools_interface/plotting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/plotting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11028 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/plotting/plot_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    12382 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/plotting/subplot_classes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 10:32:43.976459 rtc-tools-interface-0.7.3/rtctools_interface/simulation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/simulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/simulation/base_simulation_problem.py
--rw-rw-rw-   0 root         (0) root         (0)      970 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/simulation/plot_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 10:32:43.977459 rtc-tools-interface-0.7.3/rtctools_interface/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/utils/plot_table_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1399 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/utils/read_goals_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     2094 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/utils/read_plot_table.py
--rw-rw-rw-   0 root         (0) root         (0)     7742 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/utils/results_collection.py
--rw-rw-rw-   0 root         (0) root         (0)     2450 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/utils/serialization.py
--rw-rw-rw-   0 root         (0) root         (0)     1722 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/rtctools_interface/utils/type_definitions.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2024-03-05 10:32:43.980459 rtc-tools-interface-0.7.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      504 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 10:32:43.978459 rtc-tools-interface-0.7.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 10:32:43.979459 rtc-tools-interface-0.7.3/tests/optimization/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/tests/optimization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1079 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/tests/optimization/test_base_optimization_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     1265 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/tests/optimization/test_passing_goals_directly.py
--rw-rw-rw-   0 root         (0) root         (0)     2076 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/tests/optimization/test_plot_goals_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/tests/optimization/test_read_goals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 10:32:43.979459 rtc-tools-interface-0.7.3/tests/simulation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/tests/simulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/tests/simulation/test_base_simulation_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     1892 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/tests/simulation/test_plot_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 10:32:43.980459 rtc-tools-interface-0.7.3/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/tests/utils/get_test.py
--rw-rw-rw-   0 root         (0) root         (0)    83607 2024-03-05 10:32:42.000000 rtc-tools-interface-0.7.3/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.492177 rtc-tools-interface-0.7.4/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/COPYING.LESSER
+-rw-r--r--   0 root         (0) root         (0)      268 2024-04-25 14:36:24.492177 rtc-tools-interface-0.7.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    12418 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.485177 rtc-tools-interface-0.7.4/rtc_tools_interface.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      268 2024-04-25 14:36:24.000000 rtc-tools-interface-0.7.4/rtc_tools_interface.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1882 2024-04-25 14:36:24.000000 rtc-tools-interface-0.7.4/rtc_tools_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 14:36:24.000000 rtc-tools-interface-0.7.4/rtc_tools_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2024-04-25 14:36:24.000000 rtc-tools-interface-0.7.4/rtc_tools_interface.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-25 14:36:24.000000 rtc-tools-interface-0.7.4/rtc_tools_interface.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.493177 rtc-tools-interface-0.7.4/rtctools_interface/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2024-04-25 14:36:24.493177 rtc-tools-interface-0.7.4/rtctools_interface/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.487177 rtc-tools-interface-0.7.4/rtctools_interface/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10183 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/base_goal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1066 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/base_optimization_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     4068 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/goal_generator_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     5055 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/goal_performance_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3613 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/goal_table_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.487177 rtc-tools-interface-0.7.4/rtctools_interface/optimization/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3032 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/helpers/statistics_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      401 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/plot_goals_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2010 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/plot_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3292 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/optimization/read_goals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.488177 rtc-tools-interface-0.7.4/rtctools_interface/plotting/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/plotting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11028 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/plotting/plot_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    12382 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/plotting/subplot_classes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.488177 rtc-tools-interface-0.7.4/rtctools_interface/simulation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/simulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/simulation/base_simulation_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)      970 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/simulation/plot_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.490177 rtc-tools-interface-0.7.4/rtctools_interface/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/utils/plot_table_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/utils/read_goals_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2094 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/utils/read_plot_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     7748 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/utils/results_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2450 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/utils/serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/rtctools_interface/utils/type_definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2024-04-25 14:36:24.493177 rtc-tools-interface-0.7.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      504 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.490177 rtc-tools-interface-0.7.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.491177 rtc-tools-interface-0.7.4/tests/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/optimization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/optimization/test_base_optimization_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1265 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/optimization/test_passing_goals_directly.py
+-rw-rw-rw-   0 root         (0) root         (0)     2076 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/optimization/test_plot_goals_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/optimization/test_read_goals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.492177 rtc-tools-interface-0.7.4/tests/simulation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/simulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/simulation/test_base_simulation_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1892 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/simulation/test_plot_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:36:24.492177 rtc-tools-interface-0.7.4/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/tests/utils/get_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    83607 2024-04-25 14:36:23.000000 rtc-tools-interface-0.7.4/versioneer.py
```

### Comparing `rtc-tools-interface-0.7.3/COPYING.LESSER` & `rtc-tools-interface-0.7.4/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/README.md` & `rtc-tools-interface-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/rtc_tools_interface.egg-info/SOURCES.txt` & `rtc-tools-interface-0.7.4/rtc_tools_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/rtctools_interface/optimization/base_goal.py` & `rtc-tools-interface-0.7.4/rtctools_interface/optimization/base_goal.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/rtctools_interface/optimization/base_optimization_problem.py` & `rtc-tools-interface-0.7.4/rtctools_interface/optimization/base_optimization_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/rtctools_interface/optimization/goal_generator_mixin.py` & `rtc-tools-interface-0.7.4/rtctools_interface/optimization/goal_generator_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/rtctools_interface/optimization/goal_performance_metrics.py` & `rtc-tools-interface-0.7.4/rtctools_interface/optimization/goal_performance_metrics.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/rtctools_interface/optimization/goal_table_schema.py` & `rtc-tools-interface-0.7.4/rtctools_interface/optimization/goal_table_schema.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/rtctools_interface/optimization/helpers/statistics_mixin.py` & `rtc-tools-interface-0.7.4/rtctools_interface/optimization/helpers/statistics_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/rtctools_interface/optimization/plot_mixin.py` & `rtc-tools-interface-0.7.4/rtctools_interface/optimization/plot_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/rtctools_interface/optimization/read_goals.py` & `rtc-tools-interface-0.7.4/rtctools_interface/optimization/read_goals.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/rtctools_interface/plotting/plot_tools.py` & `rtc-tools-interface-0.7.4/rtctools_interface/plotting/plot_tools.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/rtctools_interface/plotting/subplot_classes.py` & `rtc-tools-interface-0.7.4/rtctools_interface/plotting/subplot_classes.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/rtctools_interface/simulation/base_simulation_problem.py` & `rtc-tools-interface-0.7.4/rtctools_interface/simulation/base_simulation_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/rtctools_interface/simulation/plot_mixin.py` & `rtc-tools-interface-0.7.4/rtctools_interface/simulation/plot_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/rtctools_interface/utils/plot_table_schema.py` & `rtc-tools-interface-0.7.4/rtctools_interface/utils/plot_table_schema.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/rtctools_interface/utils/read_goals_mixin.py` & `rtc-tools-interface-0.7.4/rtctools_interface/utils/read_goals_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/rtctools_interface/utils/read_plot_table.py` & `rtc-tools-interface-0.7.4/rtctools_interface/utils/read_plot_table.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/rtctools_interface/utils/results_collection.py` & `rtc-tools-interface-0.7.4/rtctools_interface/utils/results_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         extracted_results = copy.deepcopy(self.extract_results())
         timeseries_data = {}
         for timeseries_name in all_variables_to_store:
             try:
                 timeseries_data[timeseries_name] = extracted_results[timeseries_name]
             except KeyError:
                 try:
-                    timeseries_data[timeseries_name] = self.get_timeseries(timeseries_name)
+                    timeseries_data[timeseries_name] = self.io.get_timeseries(timeseries_name)[1]
                 except KeyError as exc:
                     raise KeyError("Cannot find timeseries for %s" % timeseries_name) from exc
         return timeseries_data
 
     def create_plot_data_and_config(self, base_goals: list) -> PlotDataAndConfig:
         """Create the PlotDataAndConfig dict."""
         prio_independent_data: PrioIndependentData = {
```

### Comparing `rtc-tools-interface-0.7.3/rtctools_interface/utils/serialization.py` & `rtc-tools-interface-0.7.4/rtctools_interface/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/rtctools_interface/utils/type_definitions.py` & `rtc-tools-interface-0.7.4/rtctools_interface/utils/type_definitions.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/tests/optimization/test_base_optimization_problem.py` & `rtc-tools-interface-0.7.4/tests/optimization/test_base_optimization_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/tests/optimization/test_passing_goals_directly.py` & `rtc-tools-interface-0.7.4/tests/optimization/test_passing_goals_directly.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/tests/optimization/test_plot_goals_mixin.py` & `rtc-tools-interface-0.7.4/tests/optimization/test_plot_goals_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/tests/simulation/test_base_simulation_problem.py` & `rtc-tools-interface-0.7.4/tests/simulation/test_base_simulation_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/tests/simulation/test_plot_mixin.py` & `rtc-tools-interface-0.7.4/tests/simulation/test_plot_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/tests/utils/get_test.py` & `rtc-tools-interface-0.7.4/tests/utils/get_test.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-interface-0.7.3/versioneer.py` & `rtc-tools-interface-0.7.4/versioneer.py`

 * *Files identical despite different names*


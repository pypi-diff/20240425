# Comparing `tmp/safe_autonomy_sims-3.2.9.tar.gz` & `tmp/safe_autonomy_sims-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe_autonomy_sims-3.2.9.tar", max compression
+gzip compressed data, was "safe_autonomy_sims-4.0.0.tar", max compression
```

## Comparing `safe_autonomy_sims-3.2.9.tar` & `safe_autonomy_sims-4.0.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0       34 2024-03-26 22:05:54.676286 safe_autonomy_sims-3.2.9/LICENSE
--rw-r--r--   0        0        0     6533 2024-03-26 22:05:54.676286 safe_autonomy_sims-3.2.9/README.md
--rw-r--r--   0        0        0    11104 2024-03-26 22:05:54.680286 safe_autonomy_sims-3.2.9/docs/configuration.md
--rw-r--r--   0        0        0      282 2024-03-26 22:05:54.680286 safe_autonomy_sims-3.2.9/docs/css/images.css
--rw-r--r--   0        0        0       90 2024-03-26 22:05:54.680286 safe_autonomy_sims-3.2.9/docs/css/material.css
--rw-r--r--   0        0        0      263 2024-03-26 22:05:54.680286 safe_autonomy_sims-3.2.9/docs/css/mkdocstrings.css
--rw-r--r--   0        0        0      895 2024-03-26 22:05:54.680286 safe_autonomy_sims-3.2.9/docs/css/style.css
--rw-r--r--   0        0        0    36430 2024-03-26 22:05:54.680286 safe_autonomy_sims-3.2.9/docs/experiments.md
--rw-r--r--   0        0        0     1005 2024-03-26 22:05:54.680286 safe_autonomy_sims-3.2.9/docs/gen_ref_nav.py
--rw-r--r--   0        0        0   129349 2024-03-26 22:05:56.080272 safe_autonomy_sims-3.2.9/docs/images/HillsFrame2.png
--rw-r--r--   0        0        0   130401 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/images/HillsFrame3.png
--rw-r--r--   0        0        0    50311 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/images/inspection_problem.png
--rw-r--r--   0        0        0    41425 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/images/linear.png
--rw-r--r--   0        0        0    31143 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/images/relu.png
--rw-r--r--   0        0        0    33502 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/images/tanh.png
--rw-r--r--   0        0        0     6407 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/index.md
--rw-r--r--   0        0        0     1393 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/install.md
--rw-r--r--   0        0        0      392 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/javascripts/mathjax.js
--rw-r--r--   0        0        0    22587 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/tasks/CWH/docking.md
--rw-r--r--   0        0        0     2650 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/tasks/CWH/index.md
--rw-r--r--   0        0        0    23806 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/tasks/CWH/multiagent_docking.md
--rw-r--r--   0        0        0    27267 2024-03-26 22:05:56.088272 safe_autonomy_sims-3.2.9/docs/tasks/CWH/multiagent_translational_inspection.md
--rw-r--r--   0        0        0    34877 2024-03-26 22:05:56.088272 safe_autonomy_sims-3.2.9/docs/tasks/CWH/multiagent_weighted_six_dof_inspection.md
--rw-r--r--   0        0        0    28120 2024-03-26 22:05:56.088272 safe_autonomy_sims-3.2.9/docs/tasks/CWH/multiagent_weighted_translational_inspection.md
--rw-r--r--   0        0        0    26682 2024-03-26 22:05:56.088272 safe_autonomy_sims-3.2.9/docs/tasks/CWH/translational_inspection.md
--rw-r--r--   0        0        0    30735 2024-03-26 22:05:56.088272 safe_autonomy_sims-3.2.9/docs/tasks/CWH/weighted_six_dof_inspection.md
--rw-r--r--   0        0        0    27367 2024-03-26 22:05:56.088272 safe_autonomy_sims-3.2.9/docs/tasks/CWH/weighted_translational_inspection.md
--rw-r--r--   0        0        0     1207 2024-03-26 22:05:56.088272 safe_autonomy_sims-3.2.9/docs/tasks/index.md
--rw-r--r--   0        0        0     2323 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/pyproject.toml
--rw-r--r--   0        0        0      826 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/__init__.py
--rw-r--r--   0        0        0      839 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/agents/__init__.py
--rw-r--r--   0        0        0     2828 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/agents/rta_agent.py
--rw-r--r--   0        0        0      935 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/__init__.py
--rw-r--r--   0        0        0    12175 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/common_dones.py
--rw-r--r--   0        0        0      627 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/cwh/__init__.py
--rw-r--r--   0        0        0    11159 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/cwh/common.py
--rw-r--r--   0        0        0    13464 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/cwh/docking_dones.py
--rw-r--r--   0        0        0    12337 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/cwh/inspection_dones.py
--rw-r--r--   0        0        0      673 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/__init__.py
--rw-r--r--   0        0        0      642 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/animation/__init__.py
--rw-r--r--   0        0        0     8202 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/animation/base_animation.py
--rw-r--r--   0        0        0    19448 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/animation/inspection_animation.py
--rw-r--r--   0        0        0    10705 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/animation/six_dof_animation.py
--rw-r--r--   0        0        0    38230 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/evaluation_api.py
--rw-r--r--   0        0        0     4992 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/general_metrics.py
--rw-r--r--   0        0        0     6725 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/inspection_metrics.py
--rw-r--r--   0        0        0      660 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/launch/__init__.py
--rw-r--r--   0        0        0     1824 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/launch/serialize_cwh3d.py
--rw-r--r--   0        0        0      786 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/experiments/__init__.py
--rw-r--r--   0        0        0     7087 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/experiments/rllib_api_experiment.py
--rw-r--r--   0        0        0    20658 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/experiments/safe_autonomy_rllib_api_experiment.py
--rw-r--r--   0        0        0     1265 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/__init__.py
--rw-r--r--   0        0        0     3174 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/coordinate_axis_glue.py
--rw-r--r--   0        0        0     3348 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/dot_product_glue.py
--rw-r--r--   0        0        0      983 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/magnitude_glue.py
--rw-r--r--   0        0        0    10361 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/rta_glue.py
--rw-r--r--   0        0        0     7716 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/six_dof_glues.py
--rw-r--r--   0        0        0     3928 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/vel_limit_glue.py
--rw-r--r--   0        0        0     1063 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/__init__.py
--rw-r--r--   0        0        0      614 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/common/__init__.py
--rw-r--r--   0        0        0     3895 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/common/controllers.py
--rw-r--r--   0        0        0     1757 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/common/platform.py
--rw-r--r--   0        0        0     2085 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/common/sensors.py
--rw-r--r--   0        0        0      612 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/__init__.py
--rw-r--r--   0        0        0     1499 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/cwh_available_platforms.py
--rw-r--r--   0        0        0     7656 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/cwh_platform.py
--rw-r--r--   0        0        0    15755 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/cwh_properties.py
--rw-r--r--   0        0        0    21104 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/cwh_sensors.py
--rw-r--r--   0        0        0     5449 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/rotation_sensors.py
--rw-r--r--   0        0        0      970 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/__init__.py
--rw-r--r--   0        0        0      597 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/__init__.py
--rw-r--r--   0        0        0    21575 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/docking_rewards.py
--rw-r--r--   0        0        0     3976 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/done_state_rewards.py
--rw-r--r--   0        0        0     4320 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/gaussian_decay_from_target_value.py
--rw-r--r--   0        0        0    15636 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/inspection_rewards.py
--rw-r--r--   0        0        0     2097 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/live_timestep_reward.py
--rw-r--r--   0        0        0     1820 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/rta_rewards.py
--rw-r--r--   0        0        0     1016 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rta/__init__.py
--rw-r--r--   0        0        0      602 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rta/cwh/__init__.py
--rw-r--r--   0        0        0     9407 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rta/cwh/cwh_rta.py
--rw-r--r--   0        0        0     5785 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rta/cwh/inspection_rta_1v1.py
--rw-r--r--   0        0        0     8206 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rta/rta_rejection_sampler.py
--rw-r--r--   0        0        0     1122 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/__init__.py
--rw-r--r--   0        0        0     1262 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/cwh_simulator.py
--rw-r--r--   0        0        0    22988 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/illumination_functions.py
--rw-r--r--   0        0        0      830 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/initializers/__init__.py
--rw-r--r--   0        0        0    15278 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/initializers/cwh.py
--rw-r--r--   0        0        0     7033 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/initializers/initializer.py
--rw-r--r--   0        0        0    31944 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/inspection_simulator.py
--rw-r--r--   0        0        0    16947 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/saferl_simulator.py
--rw-r--r--   0        0        0     9010 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/utils.py
--rw-r--r--   0        0        0     7696 1970-01-01 00:00:00.000000 safe_autonomy_sims-3.2.9/PKG-INFO
+-rw-r--r--   0        0        0       34 2024-04-25 14:19:43.956817 safe_autonomy_sims-4.0.0/LICENSE
+-rw-r--r--   0        0        0     6533 2024-04-25 14:19:43.956817 safe_autonomy_sims-4.0.0/README.md
+-rw-r--r--   0        0        0    11104 2024-04-25 14:19:43.960817 safe_autonomy_sims-4.0.0/docs/configuration.md
+-rw-r--r--   0        0        0      282 2024-04-25 14:19:43.960817 safe_autonomy_sims-4.0.0/docs/css/images.css
+-rw-r--r--   0        0        0       90 2024-04-25 14:19:43.960817 safe_autonomy_sims-4.0.0/docs/css/material.css
+-rw-r--r--   0        0        0      263 2024-04-25 14:19:43.960817 safe_autonomy_sims-4.0.0/docs/css/mkdocstrings.css
+-rw-r--r--   0        0        0      895 2024-04-25 14:19:43.960817 safe_autonomy_sims-4.0.0/docs/css/style.css
+-rw-r--r--   0        0        0    36430 2024-04-25 14:19:43.960817 safe_autonomy_sims-4.0.0/docs/experiments.md
+-rw-r--r--   0        0        0     1005 2024-04-25 14:19:43.960817 safe_autonomy_sims-4.0.0/docs/gen_ref_nav.py
+-rw-r--r--   0        0        0   129349 2024-04-25 14:19:44.732819 safe_autonomy_sims-4.0.0/docs/images/HillsFrame2.png
+-rw-r--r--   0        0        0   130401 2024-04-25 14:19:44.736819 safe_autonomy_sims-4.0.0/docs/images/HillsFrame3.png
+-rw-r--r--   0        0        0    50311 2024-04-25 14:19:44.736819 safe_autonomy_sims-4.0.0/docs/images/inspection_problem.png
+-rw-r--r--   0        0        0    41425 2024-04-25 14:19:44.736819 safe_autonomy_sims-4.0.0/docs/images/linear.png
+-rw-r--r--   0        0        0    31143 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/images/relu.png
+-rw-r--r--   0        0        0    33502 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/images/tanh.png
+-rw-r--r--   0        0        0     6407 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/index.md
+-rw-r--r--   0        0        0     1393 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/install.md
+-rw-r--r--   0        0        0      392 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/javascripts/mathjax.js
+-rw-r--r--   0        0        0    22587 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/tasks/CWH/docking.md
+-rw-r--r--   0        0        0     2650 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/tasks/CWH/index.md
+-rw-r--r--   0        0        0    23806 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/tasks/CWH/multiagent_docking.md
+-rw-r--r--   0        0        0    27267 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/tasks/CWH/multiagent_translational_inspection.md
+-rw-r--r--   0        0        0    34877 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/tasks/CWH/multiagent_weighted_six_dof_inspection.md
+-rw-r--r--   0        0        0    28120 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/tasks/CWH/multiagent_weighted_translational_inspection.md
+-rw-r--r--   0        0        0    26682 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/tasks/CWH/translational_inspection.md
+-rw-r--r--   0        0        0    30735 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/tasks/CWH/weighted_six_dof_inspection.md
+-rw-r--r--   0        0        0    27367 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/tasks/CWH/weighted_translational_inspection.md
+-rw-r--r--   0        0        0     1207 2024-04-25 14:19:44.740819 safe_autonomy_sims-4.0.0/docs/tasks/index.md
+-rw-r--r--   0        0        0     2322 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0      827 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/__init__.py
+-rw-r--r--   0        0        0      839 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/agents/__init__.py
+-rw-r--r--   0        0        0     2828 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/agents/rta_agent.py
+-rw-r--r--   0        0        0      936 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/__init__.py
+-rw-r--r--   0        0        0    12173 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/common_dones.py
+-rw-r--r--   0        0        0      628 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/cwh/__init__.py
+-rw-r--r--   0        0        0    11159 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/cwh/common.py
+-rw-r--r--   0        0        0    13464 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/cwh/docking_dones.py
+-rw-r--r--   0        0        0    12330 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/cwh/inspection_dones.py
+-rw-r--r--   0        0        0      674 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/__init__.py
+-rw-r--r--   0        0        0      643 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/animation/__init__.py
+-rw-r--r--   0        0        0     8202 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/animation/base_animation.py
+-rw-r--r--   0        0        0    19448 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/animation/inspection_animation.py
+-rw-r--r--   0        0        0    10705 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/animation/six_dof_animation.py
+-rw-r--r--   0        0        0    18823 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/evaluation_api.py
+-rw-r--r--   0        0        0     4992 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/general_metrics.py
+-rw-r--r--   0        0        0     6725 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/inspection_metrics.py
+-rw-r--r--   0        0        0      661 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/launch/__init__.py
+-rw-r--r--   0        0        0     1824 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/launch/serialize_cwh3d.py
+-rw-r--r--   0        0        0      787 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/experiments/__init__.py
+-rw-r--r--   0        0        0     7087 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/experiments/rllib_api_experiment.py
+-rw-r--r--   0        0        0    20658 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/experiments/safe_autonomy_rllib_api_experiment.py
+-rw-r--r--   0        0        0     1266 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/__init__.py
+-rw-r--r--   0        0        0     3174 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/coordinate_axis_glue.py
+-rw-r--r--   0        0        0     3348 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/dot_product_glue.py
+-rw-r--r--   0        0        0      984 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/magnitude_glue.py
+-rw-r--r--   0        0        0    10361 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/rta_glue.py
+-rw-r--r--   0        0        0     7716 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/six_dof_glues.py
+-rw-r--r--   0        0        0     3902 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/vel_limit_glue.py
+-rw-r--r--   0        0        0     1064 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/__init__.py
+-rw-r--r--   0        0        0      615 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/common/__init__.py
+-rw-r--r--   0        0        0     3895 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/common/controllers.py
+-rw-r--r--   0        0        0     1757 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/common/platform.py
+-rw-r--r--   0        0        0     2085 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/common/sensors.py
+-rw-r--r--   0        0        0      613 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/__init__.py
+-rw-r--r--   0        0        0     1499 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/cwh_available_platforms.py
+-rw-r--r--   0        0        0     7656 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/cwh_platform.py
+-rw-r--r--   0        0        0    15755 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/cwh_properties.py
+-rw-r--r--   0        0        0    21104 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/cwh_sensors.py
+-rw-r--r--   0        0        0     5449 2024-04-25 14:19:44.744819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/rotation_sensors.py
+-rw-r--r--   0        0        0      971 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/__init__.py
+-rw-r--r--   0        0        0      598 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/__init__.py
+-rw-r--r--   0        0        0    21566 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/docking_rewards.py
+-rw-r--r--   0        0        0     3971 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/done_state_rewards.py
+-rw-r--r--   0        0        0     4319 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/gaussian_decay_from_target_value.py
+-rw-r--r--   0        0        0    15621 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/inspection_rewards.py
+-rw-r--r--   0        0        0     2097 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/live_timestep_reward.py
+-rw-r--r--   0        0        0     1820 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/rta_rewards.py
+-rw-r--r--   0        0        0     1017 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rta/__init__.py
+-rw-r--r--   0        0        0      603 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rta/cwh/__init__.py
+-rw-r--r--   0        0        0     9407 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rta/cwh/cwh_rta.py
+-rw-r--r--   0        0        0     5785 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rta/cwh/inspection_rta_1v1.py
+-rw-r--r--   0        0        0     8226 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/rta/rta_rejection_sampler.py
+-rw-r--r--   0        0        0     1123 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/__init__.py
+-rw-r--r--   0        0        0     1262 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/cwh_simulator.py
+-rw-r--r--   0        0        0    22988 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/illumination_functions.py
+-rw-r--r--   0        0        0      831 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/initializers/__init__.py
+-rw-r--r--   0        0        0    15277 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/initializers/cwh.py
+-rw-r--r--   0        0        0     7033 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/initializers/initializer.py
+-rw-r--r--   0        0        0    31944 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/inspection_simulator.py
+-rw-r--r--   0        0        0    16947 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/saferl_simulator.py
+-rw-r--r--   0        0        0     9010 2024-04-25 14:19:44.748819 safe_autonomy_sims-4.0.0/safe_autonomy_sims/utils.py
+-rw-r--r--   0        0        0     7695 1970-01-01 00:00:00.000000 safe_autonomy_sims-4.0.0/PKG-INFO
```

### Comparing `safe_autonomy_sims-3.2.9/README.md` & `safe_autonomy_sims-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/configuration.md` & `safe_autonomy_sims-4.0.0/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/css/style.css` & `safe_autonomy_sims-4.0.0/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/experiments.md` & `safe_autonomy_sims-4.0.0/docs/experiments.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/gen_ref_nav.py` & `safe_autonomy_sims-4.0.0/docs/gen_ref_nav.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/images/HillsFrame2.png` & `safe_autonomy_sims-4.0.0/docs/images/HillsFrame2.png`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/images/HillsFrame3.png` & `safe_autonomy_sims-4.0.0/docs/images/HillsFrame3.png`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/images/inspection_problem.png` & `safe_autonomy_sims-4.0.0/docs/images/inspection_problem.png`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/images/linear.png` & `safe_autonomy_sims-4.0.0/docs/images/linear.png`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/images/relu.png` & `safe_autonomy_sims-4.0.0/docs/images/relu.png`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/images/tanh.png` & `safe_autonomy_sims-4.0.0/docs/images/tanh.png`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/index.md` & `safe_autonomy_sims-4.0.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/install.md` & `safe_autonomy_sims-4.0.0/docs/install.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/tasks/CWH/docking.md` & `safe_autonomy_sims-4.0.0/docs/tasks/CWH/docking.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/tasks/CWH/index.md` & `safe_autonomy_sims-4.0.0/docs/tasks/CWH/index.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/tasks/CWH/multiagent_docking.md` & `safe_autonomy_sims-4.0.0/docs/tasks/CWH/multiagent_docking.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/tasks/CWH/multiagent_translational_inspection.md` & `safe_autonomy_sims-4.0.0/docs/tasks/CWH/multiagent_translational_inspection.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/tasks/CWH/multiagent_weighted_six_dof_inspection.md` & `safe_autonomy_sims-4.0.0/docs/tasks/CWH/multiagent_weighted_six_dof_inspection.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/tasks/CWH/multiagent_weighted_translational_inspection.md` & `safe_autonomy_sims-4.0.0/docs/tasks/CWH/multiagent_weighted_translational_inspection.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/tasks/CWH/translational_inspection.md` & `safe_autonomy_sims-4.0.0/docs/tasks/CWH/translational_inspection.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/tasks/CWH/weighted_six_dof_inspection.md` & `safe_autonomy_sims-4.0.0/docs/tasks/CWH/weighted_six_dof_inspection.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/tasks/CWH/weighted_translational_inspection.md` & `safe_autonomy_sims-4.0.0/docs/tasks/CWH/weighted_translational_inspection.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/docs/tasks/index.md` & `safe_autonomy_sims-4.0.0/docs/tasks/index.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/pyproject.toml` & `safe_autonomy_sims-4.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "safe-autonomy-sims"
-version = "3.2.9"
+version = "4.0.0"
 description = "The Safe-Autonomy-Sims library provides the components and tools to build modular, integration-focused Reinforcement Learning environments with Run Time Assurance (RTA)"
 authors = [
     "Charles Keating <Charles.Keating@udri.udayton.edu>",
 ]
 license = ""
 readme = "README.md"
 homepage = "https://github.com/act3-ace/safe-autonomy-sims.git"
@@ -26,17 +26,17 @@
 tqdm = "^4.66.1"
 scikit-learn = "1.2.1"
 seaborn = "^0.12.0"
 torch = "1.13.0"
 imageio = "2.25.0"
 imageio-ffmpeg = "0.4.8"
 pint = "^0.22"
-safe-autonomy-dynamics = "1.2.2"
-run-time-assurance = "1.15.3"
-corl = "3.14.13"
+safe-autonomy-dynamics = "1.2.3"
+run-time-assurance = "1.16.1"
+corl = "3.16.2"
 
 [tool.poetry.group.lint.dependencies]
 pylint = "2.15.4"
 flake8 = "3.9.2"
 yapf = "^0.40.0"
 isort = "5.9.3"
 bashate = "^2.1.0"
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/__init__.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 
 The `safe-autonomy-sims` package provides reinforement learning environments
 built using the CoRL framework.
 
 The included environments define safety-critical spacecraft docking and
 spacecraft inspection tasks. The intent of these environments is to
 provide a baseline for training RL agents to safely perform these tasks.
-"""
+"""
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/agents/__init__.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/agents/rta_agent.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/agents/rta_agent.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/__init__.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 learning environments.
 
 Done functions are called by [simulators](../simulators/index.md)
 at each timestep of the simulation. These functions are tasked with
 determining when an agent has reached a done condition for their
 current training episode on a given task. They take in the current
 and previous observation and action spaces and output a boolean value.
-"""
+"""
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/common_dones.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/common_dones.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     """
     A done function that determines if the max episode time
     has been reached.
 
     Attributes
     ----------
     config: TimeoutDoneValidator
-        The function's validated configuration parameters 
+        The function's validated configuration parameters
     """
 
     def __init__(self, **kwargs) -> None:
         self.config: TimeoutDoneValidator
         super().__init__(**kwargs)
 
     @staticmethod
@@ -118,15 +118,15 @@
     """
     A done function that determines if an agent's spacecraft
     has collided with another agent's spacecraft in the environemt.
 
     Attributes
     ----------
     config: CollisionDoneFunctionValidator
-        The function's validated configuration parameters 
+        The function's validated configuration parameters
     """
 
     @staticmethod
     def get_validator() -> typing.Type[SharedDoneFuncBaseValidator]:
         """
         Returns the validator for this done function.
 
@@ -233,15 +233,15 @@
     """
     This done function determines whether every agent in the
     environment has reached a specified successful done condition.
 
     Attributes
     ----------
     config: MultiagentSuccessDoneFunctionValidator
-        The function's validated configuration parameters 
+        The function's validated configuration parameters
     """
 
     @staticmethod
     def get_validator() -> typing.Type[SharedDoneFuncBaseValidator]:
         """
         Returns the validator for this done function.
 
@@ -359,8 +359,8 @@
         dones = DoneDict()
 
         done = any(local_dones.values())
 
         for name in platform_names:
             dones[name] = done
 
-        return dones
+        return dones
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/cwh/__init__.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/cwh/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 
 This package implements done functions for the docking and inspection
 space environments using Clohessy-Wiltshire dynamics.
-"""
+"""
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/cwh/common.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/cwh/common.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/cwh/docking_dones.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/cwh/docking_dones.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/cwh/inspection_dones.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/dones/cwh/inspection_dones.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         """
         Returns configuration validator object for this done
         function.
 
         Returns
         -------
         SafeSuccessfulInspectionDoneValidator
-            Config validator for the SafeSuccessfulInspectionDoneFunction.        """
+            Config validator for the SafeSuccessfulInspectionDoneFunction."""
         return SafeSuccessfulInspectionDoneValidator
 
     def __call__(
         self,
         observation: OrderedDict,
         action: OrderedDict,
         next_observation: OrderedDict,
@@ -199,15 +199,15 @@
             state = np.concatenate((pos, vel))
             n = self.config.mean_motion
             times = np.arange(0, 2 * np.pi / n, self.config.fft_time_step)
             dist = get_closest_fft_distance(state, self.config.mean_motion, times)
             if dist >= self.config.crash_region_radius:
                 next_state.episode_state[self.config.platform_name][self.name] = DoneStatusCodes.WIN
             else:
-                #TODO: why is done set to False if deputy is within crash radius? Would crash not end episode?
+                # TODO: why is done set to False if deputy is within crash radius? Would crash not end episode?
                 done = False
 
         return done
 
 
 class CrashAfterSuccessfulInspectionDoneFunction(SuccessfulInspectionDoneFunction):
     """
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/__init__.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 
 This package implements scripts and metrics designed to work with the
 CoRL evaluation framework for evaluating agents trained in the
 docking and inspection environments.
-"""
+"""
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/animation/__init__.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/animation/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 
 This package implements animation objects which allow users to
 animate training and evaluation episodes within the inspection
 environment.
-"""
+"""
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/animation/base_animation.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/animation/base_animation.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/animation/inspection_animation.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/animation/inspection_animation.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/animation/six_dof_animation.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/animation/six_dof_animation.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/general_metrics.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/general_metrics.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/inspection_metrics.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/inspection_metrics.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/launch/__init__.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/launch/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 
 <!-- TODO: flatten this into a module -->
 
 This package implements serialization of `CWH3DPlatform` data
 for evaluation using the CoRL evaluation framework.
-"""
+"""
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/launch/serialize_cwh3d.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/evaluation/launch/serialize_cwh3d.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/experiments/__init__.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/experiments/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 This package implements CoRL experiments for safe autonomy training
 runs.
 
 CoRL `Experiment`s act as containers around training runs. Within
 an experiment a user can define custom training behavior and
 develop integration for different RL frameworks and backend simulator
 solutions.
-"""
+"""
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/experiments/rllib_api_experiment.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/experiments/rllib_api_experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,33 +17,34 @@
 import argparse
 import pickle
 import socket
 import typing
 from datetime import datetime
 
 import ray
-# import ray.rllib.agents.ppo as ppo
-from ray.rllib.algorithms.ppo import ppo
 import tqdm
 from corl.environment.multi_agent_env import ACT3MultiAgentEnv, ACT3MultiAgentEnvValidator
 from corl.episode_parameter_providers.remote import RemoteEpisodeParameterProvider
 from corl.experiments.rllib_experiment import RllibExperiment, RllibExperimentValidator
 from corl.libraries.factory import Factory
 
+# import ray.rllib.agents.ppo as ppo
+from ray.rllib.algorithms.ppo import ppo
+
 
 class RllibAPIExperimentValidator(RllibExperimentValidator):
     """
     The validator for the RllibAPIExperiment class.
 
     Attributes
     ----------
     serialized_ray_config_path: str
         path to params.pkl file
     trained_models_checkpoint_path: str
-        path to checkpoint directory 
+        path to checkpoint directory
     """
     serialized_ray_config_path: str
     trained_models_checkpoint_path: str
 
 
 class RllibAPIExperiment(RllibExperiment):
     """
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/experiments/safe_autonomy_rllib_api_experiment.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/experiments/safe_autonomy_rllib_api_experiment.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/__init__.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 A glue may also transform and send data from a training framework to
 a platform part as an action. The full set of glues which provide
 actions over all agents in the environment defines the environment's
 action space.
 
 Multiple glues may be used in a decorator pattern to reuse common
 transformation logic.
-"""
+"""
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/coordinate_axis_glue.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/coordinate_axis_glue.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/dot_product_glue.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/dot_product_glue.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/magnitude_glue.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/magnitude_glue.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 
 This module implements an extension of the CoRL Magnitude Glue with the observation_prop property.
 """
 
 from functools import cached_property
+
 from corl.glues.common.magnitude import MagnitudeGlue
-from corl.libraries.property import DictProp, BoxProp
+from corl.libraries.property import BoxProp, DictProp
+
 
 class SimsMagnitudeGlue(MagnitudeGlue):
 
     @cached_property
     def observation_prop(self):
         prop = DictProp(name=self._uname, spaces={self.Fields.MAG: BoxProp(low=[-10000], high=[10000], unit='m/s')})
         return prop
-
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/rta_glue.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/rta_glue.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/six_dof_glues.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/six_dof_glues.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/vel_limit_glue.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/glues/vel_limit_glue.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 
 Wrapper glue which returns a velocity constraint based on position and velocity sensor data as an observation.
 """
+import typing
 from collections import OrderedDict
+from functools import cached_property
 
-import typing
 import gymnasium
 import numpy as np
-from functools import cached_property
 from corl.glues.base_glue import BaseAgentGlueNormalizationValidator
 from corl.glues.common.observe_sensor import ObserveSensor, ObserveSensorValidator
 from corl.libraries.normalization import StandardNormalNormalizer
-from corl.libraries.property import DictProp, BoxProp
+from corl.libraries.property import BoxProp, DictProp
 from corl.libraries.units import corl_get_ureg
 
 
 class VelocityLimitGlueValidator(ObserveSensorValidator):
     """
     A configuration validator for the VelocityLimitGlue.
 
@@ -62,17 +62,15 @@
 
     def _vel_limit(self, dist):
         return self.config.velocity_threshold + (self.config.slope * self.config.mean_motion * (dist - self.config.threshold_distance))
 
     @cached_property
     def observation_prop(self):
         prop = BoxProp(low=[-10000], high=[10000], unit='m/s')
-        return DictProp(
-            spaces={self.Fields.DIRECT_OBSERVATION: prop}
-        )
+        return DictProp(spaces={self.Fields.DIRECT_OBSERVATION: prop})
 
     @cached_property
     def observation_space(self) -> typing.Optional[gymnasium.spaces.Space]:
         pos_obs_space = super().observation_space[self.Fields.DIRECT_OBSERVATION]
         high = self._vel_limit(np.linalg.norm(pos_obs_space.high)) * np.sign(pos_obs_space.high)[0]
         low = self._vel_limit(np.linalg.norm(pos_obs_space.low)) * np.sign(pos_obs_space.low)[0]
         d = gymnasium.spaces.dict.Dict()
@@ -85,11 +83,11 @@
         d = OrderedDict()
         d[self.Fields.DIRECT_OBSERVATION] = obs
         return d
 
     @cached_property
     def normalized_action_space(self) -> typing.Optional[gymnasium.spaces.Space]:
         return self.action_space
-    
+
     @cached_property
     def normalized_observation_space(self) -> typing.Optional[gymnasium.spaces.Space]:
         return self.observation_space
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/__init__.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 (vehicles, robots, etc.). Platforms can contain multiple custom
 `PlatformPart`s which define platform behavior. The most common
 types of parts are `Controller`s and `Sensor`s. `Controller`s
 apply controls to thrusters and control surfaces to interact with
 environment dynamics. `Sensor`s measure various aspects of the
 environment. Platform parts are often analogous to the parts used
 in a physical system.
-"""
+"""
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/common/__init__.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/common/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 
 This package implements common platforms, controllers, and sensors
 used across the safe autonomy environments.
-"""
+"""
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/common/controllers.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/common/controllers.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/common/platform.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/common/platform.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/common/sensors.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/common/sensors.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/__init__.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rta/cwh/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 
-This package implements platforms, controllers, and sensors
-used in the docking and inspection environments.
-"""
+This package implements Runtime Assurance modules used in
+the docking and inspection environments.
+"""
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/cwh_available_platforms.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/cwh_available_platforms.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 This is a US Government Work not subject to copyright protection in the US.
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 
-This module defines and registers the available CWH platform types to the proper simulators. 
+This module defines and registers the available CWH platform types to the proper simulators.
 """
 
 from __future__ import annotations
 
 from corl.libraries.plugin_library import PluginLibrary
 from corl.simulators.base_platform_type import BasePlatformType
 
@@ -32,9 +32,10 @@
 
         if config["name"] == "CWH":
             return True
         if config["name"] == "CWHSixDOF":
             return True
         return False
 
+
 PluginLibrary.add_platform_to_sim(CWHAvailablePlatformTypes, CWHSimulator)
 PluginLibrary.add_platform_to_sim(CWHAvailablePlatformTypes, InspectionSimulator)
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/cwh_platform.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/cwh_platform.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/cwh_properties.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/cwh_properties.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/cwh_sensors.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/cwh_sensors.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/rotation_sensors.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/platforms/cwh/rotation_sensors.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/__init__.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 Rewards are used to incentivize certain [agent](../agents/index.md)
 behavior during training. Over the course of a training episode,
 the following reward functions take in current and previous
 observations and actions and return a `RewardDict`,
 allocating an appropriate reward (or penalty) to an agent based on
 its behavior and the [simulation](../simulators/index.md) state.
-"""
+"""
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/__init__.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 
 This package implements the reward functions used in the docking
 and inspection environments.
-"""
+"""
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/docking_rewards.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/docking_rewards.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         # get relative dist
         # Assumes one platfrom per agent!
         platform = get_platform_by_name(next_state, self.config.platform_names[0])
         relative_position = get_relative_position(platform, self.config.reference_position_sensor_name)
         distance = np.linalg.norm(relative_position)
 
         self._dist_buffer.append(distance)
-        
+
         reward = 0.0
 
         # TODO intialize distance buffer from initial state
         if len(self._dist_buffer) == 2:
             reward = self.config.scale * (self._dist_buffer[1] - self._dist_buffer[0])
 
         return reward
@@ -397,15 +397,14 @@
         next_observation: OrderedDict,
         state: StateDict,
         next_state: StateDict,
         observation_space: StateDict,
         observation_units: StateDict,
     ) -> float:
 
-
         # Get relative position and velocity
         # Assumes one platfrom per agent!
         platform = get_platform_by_name(next_state, self.config.platform_names[0])
         relative_position = get_relative_position(platform, self.config.reference_position_sensor_name)
         relative_velocity = get_relative_velocity(platform, self.config.reference_velocity_sensor_name)
 
         violated, violation = max_vel_violation(
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/done_state_rewards.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/done_state_rewards.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 
 The use, dissemination or disclosure of data in this file is subject to
 limitation or restriction. See accompanying README and LICENSE for details.
 ---------------------------------------------------------------------------
 
 This module implements reward functions based on done status
 """
+import typing
 from collections import OrderedDict
 from functools import partial
-import typing
-from pydantic import validator
 
 from corl.dones.done_func_base import DoneStatusCodes
-from corl.rewards.episode_done import EpisodeDoneStateReward, EpisodeDoneStateRewardValidator
 from corl.libraries.state_dict import StateDict
+from corl.rewards.episode_done import EpisodeDoneStateReward, EpisodeDoneStateRewardValidator
+from pydantic import validator
 
 
 class WinLoseDoneRewardValidator(EpisodeDoneStateRewardValidator):
     """A configuration validator for WinLoseDoneReward
-    
+
     Attributes
     ----------
     done_name : str
-        name of done to generate reward from 
+        name of done to generate reward from
     done_status : str
         done status code to generate reward from
     scale : float
         reward scaling value
     """
     done_name: str
     done_status: str = "lose"
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/gaussian_decay_from_target_value.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/gaussian_decay_from_target_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 ---------------------------------------------------------------------------
 
 This module implements a gaussian decay reward function.
 """
 
 import logging
 import typing
-import numpy as np
 
+import numpy as np
 from corl.libraries.utils import get_wrap_diff
 from corl.rewards.base_measurement_operation import BaseMeasurementOperation, BaseMeasurementOperationValidator
 
 
 class GaussianDecayFromTargetValueValidator(BaseMeasurementOperationValidator):
     """
-    A configuration validator for GaussianDecayFromTargetValue 
+    A configuration validator for GaussianDecayFromTargetValue
 
     Attributes
     ----------
     reward scale: scale of this reward, this would be the maximum reward value
                   for a given time step
     eps: the length of the reward curve for the exponential decay, would
          recommend playing with this value in a plotting software to determine
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/inspection_rewards.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/inspection_rewards.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
             The current state of the system.
 
         Returns
         -------
         d_v: float
             The agent's change in velocity
         """
-        deputy = get_platform_by_name(state, self.config.platform_names[0])     # TODO: assuming 1:1 agent:platform
+        deputy = get_platform_by_name(state, self.config.platform_names[0])  # TODO: assuming 1:1 agent:platform
         control_vec = deputy.get_applied_action().m
         d_v = np.sum(np.abs(control_vec)) / self.mass * self.step_size
         return d_v
 
     def linear_scalar(self, time):
         """
         Delta-v penalty increases linearly with training iteration
@@ -232,15 +232,15 @@
         action,
         next_observation: OrderedDict,
         state: StateDict,
         next_state: StateDict,
         observation_space: StateDict,
         observation_units: StateDict,
     ) -> float:
-        
+
         if self.constant_scale is None:
             self.scale = state.delta_v_scale
         else:
             self.scale = self.constant_scale
         reward = 0.0
         if self.mode == "scale":
             reward = self.scale * self.delta_v(next_state) + self.bias
@@ -425,15 +425,15 @@
 
         in_crash_region = distance <= self.config.crash_region_radius
 
         if in_crash_region:
             reward = self.config.scale
 
         return reward
-    
+
 
 class MaxDistanceRewardValidator(RewardFuncBaseValidator):
     """
     A configuration validator for the InspectionCollisionRewardValidator Reward Function.
 
     Attributes
     ----------
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/live_timestep_reward.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/cwh/live_timestep_reward.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/rta_rewards.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rewards/rta_rewards.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rta/__init__.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rta/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 Runtime Assurance (RTA) is a safety technique which intercepts
 a control or action before it is executed and checks it against
 a well-defined safety constraint to see if the action is safe.
 If the action is safe, the RTA module allows it to execute.
 If the action is deemed **unsafe** the RTA module provides an
 alternative action which is guaranteed to be safe under the assumption
 that the system is already in a safe state.
-"""
+"""
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rta/cwh/cwh_rta.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rta/cwh/cwh_rta.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rta/cwh/inspection_rta_1v1.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rta/cwh/inspection_rta_1v1.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rta/rta_rejection_sampler.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/rta/rta_rejection_sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         """
         assert isinstance(self.config.rta.functor(**self.config.rta.args).rta,
                           ConstraintBasedRTA), ("Must use constraint based rta for rejection sampling.")
         init_state_safe = True
 
         # For each constraint, check if satisfied
         for c in self.config.rta.functor(**self.config.rta.args).rta.constraints.values():
-            if c.phi(to_jnp_array_jit(state)) < 0 or c(to_jnp_array_jit(state)) < 0:
+            if c.phi(to_jnp_array_jit(state), c.params) < 0 or c(to_jnp_array_jit(state), c.params) < 0:
                 init_state_safe = False
                 break
         return init_state_safe
 
 
 class RejectionSamplerInitializerValidator(InitializerValidator):
     """
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/__init__.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 
 `SafeRLSimulator` and its subclasses pair
 [platforms](../platforms/index.md) with their backend simulation
 entities to enable accurate environment interactions with respect to
 implemented dynamics models. They also coordinate execution of
 [done functions](../dones/index.md) to terminate training
 episodes appropriately.
-"""
+"""
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/cwh_simulator.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/cwh_simulator.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/illumination_functions.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/illumination_functions.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/initializers/__init__.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/initializers/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 
 This package implements initializers for the safe autonomy simulators.
 
 Initializers are responsible for setting up the initial conditions
 of platforms in a simulation. Given a set of sampled parameters,
 initializers return a set of initialization parameters expected by
 the platforms and their associated simulation entities.
-"""
+"""
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/initializers/cwh.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/initializers/cwh.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,21 +11,20 @@
 
 This module implements initializers for CWH platforms.
 """
 
 import typing
 
 import numpy as np
+from corl.libraries.units import Quantity
 from scipy.spatial.transform import Rotation
 
 from safe_autonomy_sims.simulators.initializers.initializer import BaseInitializerWithPint, InitializerValidator, strip_units_from_dict
 from safe_autonomy_sims.utils import velocity_limit
 
-from corl.libraries.units import Quantity
-
 
 class CWH3DRadialInitializer(BaseInitializerWithPint):
     """
     This class handles the initialization of agent reset parameters for the cwh 3D environment.
     Both position and velocity are initialized radially (with radius and angles) to allow for control over magnitude and direction
     of the resulting vectors.
     """
```

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/initializers/initializer.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/inspection_simulator.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/inspection_simulator.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/saferl_simulator.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/simulators/saferl_simulator.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/safe_autonomy_sims/utils.py` & `safe_autonomy_sims-4.0.0/safe_autonomy_sims/utils.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.9/PKG-INFO` & `safe_autonomy_sims-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: safe-autonomy-sims
-Version: 3.2.9
+Version: 4.0.0
 Summary: The Safe-Autonomy-Sims library provides the components and tools to build modular, integration-focused Reinforcement Learning environments with Run Time Assurance (RTA)
 Home-page: https://github.com/act3-ace/safe-autonomy-sims.git
 Author: Charles Keating
 Author-email: Charles.Keating@udri.udayton.edu
 Requires-Python: >=3.10,<3.11
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: corl (==3.14.13)
+Requires-Dist: corl (==3.16.2)
 Requires-Dist: imageio (==2.25.0)
 Requires-Dist: imageio-ffmpeg (==0.4.8)
 Requires-Dist: numpy (==1.24.0)
 Requires-Dist: pint (>=0.22,<0.23)
-Requires-Dist: run-time-assurance (==1.15.3)
-Requires-Dist: safe-autonomy-dynamics (==1.2.2)
+Requires-Dist: run-time-assurance (==1.16.1)
+Requires-Dist: safe-autonomy-dynamics (==1.2.3)
 Requires-Dist: scikit-learn (==1.2.1)
 Requires-Dist: seaborn (>=0.12.0,<0.13.0)
 Requires-Dist: torch (==1.13.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Project-URL: Documentation, https://github.com/act3-ace/safe-autonomy-sims/docs
 Project-URL: Repository, https://github.com/act3-ace/safe-autonomy-sims.git
 Description-Content-Type: text/markdown
```


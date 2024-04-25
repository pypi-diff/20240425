# Comparing `tmp/gt4sd-1.4.0.tar.gz` & `tmp/gt4sd-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gt4sd-1.4.0.tar", last modified: Thu Mar  7 15:49:18 2024, max compression
+gzip compressed data, was "/home/runner/work/gt4sd-core/gt4sd-core/dist/.tmp-8yxmxmla/gt4sd-1.4.1.tar", last modified: Thu Apr 25 07:08:08 2024, max compression
```

## Comparing `gt4sd-1.4.0.tar` & `gt4sd-1.4.1.tar`

### file list

```diff
@@ -1,399 +1,399 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.677968 gt4sd-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-07 15:49:13.000000 gt4sd-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19936 2024-03-07 15:49:18.677968 gt4sd-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18296 2024-03-07 15:49:13.000000 gt4sd-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-07 15:49:13.000000 gt4sd-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-03-07 15:49:18.677968 gt4sd-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-07 15:49:13.000000 gt4sd-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.609967 gt4sd-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.625967 gt4sd-1.4.0/src/gt4sd/
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.625967 gt4sd-1.4.0/src/gt4sd/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.625967 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.629967 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29460 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.629967 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/
--rw-r--r--   0 runner    (1001) docker     (127)    22153 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_ga.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_mcts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_aae.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_organ.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_vae.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_ga.py
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_hc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.629967 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/key_bert/
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/key_bert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/key_bert/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/key_bert/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.629967 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/molgx/
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/molgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8860 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/molgx/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/molgx/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.629967 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14210 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.633967 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20484 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    53178 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.633967 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/reinvent/
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/reinvent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/reinvent/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/reinvent/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.633967 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.633967 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/template/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/template/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/template/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.633967 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/tests/test_guacamol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/tests/test_key_bert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/tests/test_molgx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/tests/test_moses.py
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/tests/test_paccmann_rl.py
--rw-r--r--   0 runner    (1001) docker     (127)    14669 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/tests/test_regression_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/tests/test_reinvent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.633967 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.633967 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.633967 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19830 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.637967 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.637967 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.637967 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13448 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.637967 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/tests/test_advanced_manufacturing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/tests/test_class_controlled_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/tests/test_paccmann_gp.py
--rw-r--r--   0 runner    (1001) docker     (127)    34978 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.637967 gt4sd-1.4.0/src/gt4sd/algorithms/generation/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.637967 gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12649 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.637967 gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/geodiff/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/geodiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/geodiff/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.637967 gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.641968 gt4sd-1.4.0/src/gt4sd/algorithms/generation/hugging_face/
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/hugging_face/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12564 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/hugging_face/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/hugging_face/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.641968 gt4sd-1.4.0/src/gt4sd/algorithms/generation/moler/
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/moler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/moler/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/moler/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.641968 gt4sd-1.4.0/src/gt4sd/algorithms/generation/paccmann_vae/
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/paccmann_vae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/paccmann_vae/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/paccmann_vae/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.641968 gt4sd-1.4.0/src/gt4sd/algorithms/generation/pgt/
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/pgt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13254 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/pgt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    15685 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/pgt/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.641968 gt4sd-1.4.0/src/gt4sd/algorithms/generation/polymer_blocks/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/polymer_blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/polymer_blocks/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/polymer_blocks/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.645968 gt4sd-1.4.0/src/gt4sd/algorithms/generation/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   128648 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/tests/mol_dct.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/tests/test_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/tests/test_hugging_face.py
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/tests/test_moler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/tests/test_paccmann_vae.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/tests/test_pgt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/tests/test_polymer_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/tests/test_torchdrug.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.645968 gt4sd-1.4.0/src/gt4sd/algorithms/generation/torchdrug/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/torchdrug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/torchdrug/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/generation/torchdrug/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.645968 gt4sd-1.4.0/src/gt4sd/algorithms/prediction/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/prediction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.645968 gt4sd-1.4.0/src/gt4sd/algorithms/prediction/paccmann/
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/prediction/paccmann/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/prediction/paccmann/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/prediction/paccmann/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.645968 gt4sd-1.4.0/src/gt4sd/algorithms/prediction/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/prediction/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/prediction/tests/test_paccmann.py
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/prediction/tests/test_topics_zero_shot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.645968 gt4sd-1.4.0/src/gt4sd/algorithms/prediction/topics_zero_shot/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/prediction/topics_zero_shot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/prediction/topics_zero_shot/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/prediction/topics_zero_shot/implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14124 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.645968 gt4sd-1.4.0/src/gt4sd/algorithms/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/algorithms/tests/test_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.649968 gt4sd-1.4.0/src/gt4sd/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/cli/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/cli/argument_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4380 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/cli/hf_to_st_converter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6910 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/cli/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/cli/load_arguments_from_dataclass.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7893 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/cli/saving.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6950 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/cli/trainer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8169 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/cli/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    12452 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.649968 gt4sd-1.4.0/src/gt4sd/domains/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/domains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/domains/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.649968 gt4sd-1.4.0/src/gt4sd/domains/materials/
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/domains/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/domains/materials/protein_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.649968 gt4sd-1.4.0/src/gt4sd/domains/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/domains/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.649968 gt4sd-1.4.0/src/gt4sd/extras/
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.649968 gt4sd-1.4.0/src/gt4sd/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.649968 gt4sd-1.4.0/src/gt4sd/frameworks/cgcnn/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/cgcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/cgcnn/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/cgcnn/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.649968 gt4sd-1.4.0/src/gt4sd/frameworks/crystals_rfc/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/crystals_rfc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32266 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/crystals_rfc/atomic_data.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/crystals_rfc/feature_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/crystals_rfc/rf_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.649968 gt4sd-1.4.0/src/gt4sd/frameworks/enzeptional/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/enzeptional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/enzeptional/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    20040 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/enzeptional/processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.653968 gt4sd-1.4.0/src/gt4sd/frameworks/enzeptional/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/enzeptional/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/enzeptional/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/enzeptional/tests/test_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.653968 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.653968 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/arg_parser/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/arg_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/arg_parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/arg_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.653968 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/dataloader/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/dataloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/dataloader/data_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    11695 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/dataloader/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11674 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/dataloader/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.653968 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/envs/
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27081 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/envs/graph_building_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    14389 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/envs/mol_building_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.653968 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/loss/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/loss/td_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    19297 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/loss/trajectory_balance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.653968 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/ml/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.653968 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/ml/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/ml/models/graph_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    34044 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/ml/models/mxmnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/ml/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.657968 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/tests/qm9.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/tests/test_gfn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.657968 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/train/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/train/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.657968 gt4sd-1.4.0/src/gt4sd/frameworks/granular/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.657968 gt4sd-1.4.0/src/gt4sd/frameworks/granular/arg_parser/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/arg_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/arg_parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/arg_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.657968 gt4sd-1.4.0/src/gt4sd/frameworks/granular/dataloader/
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/dataloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/dataloader/data_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    18863 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/dataloader/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/dataloader/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.657968 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.657968 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.657968 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.661968 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    35475 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.661968 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/no_encoding/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/no_encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/no_encoding/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.661968 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/vae_mlp/
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/vae_mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10825 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/vae_mlp/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.661968 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/vae_rnn/
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/vae_rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12917 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/vae_rnn/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.661968 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/vae_trans/
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/vae_trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/vae_trans/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.661968 gt4sd-1.4.0/src/gt4sd/frameworks/granular/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/tests/test_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.661968 gt4sd-1.4.0/src/gt4sd/frameworks/granular/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18134 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/tokenizer/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.661968 gt4sd-1.4.0/src/gt4sd/frameworks/granular/train/
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/granular/train/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.661968 gt4sd-1.4.0/src/gt4sd/frameworks/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/frameworks/torch/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.661968 gt4sd-1.4.0/src/gt4sd/properties/
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/properties/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.661968 gt4sd-1.4.0/src/gt4sd/properties/crystals/
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/properties/crystals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11103 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/properties/crystals/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.665968 gt4sd-1.4.0/src/gt4sd/properties/molecules/
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/properties/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30897 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/properties/molecules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/properties/molecules/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.665968 gt4sd-1.4.0/src/gt4sd/properties/proteins/
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/properties/proteins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/properties/proteins/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/properties/proteins/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/properties/scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.665968 gt4sd-1.4.0/src/gt4sd/properties/scores/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/properties/scores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/properties/scores/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.665968 gt4sd-1.4.0/src/gt4sd/properties/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/properties/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9859 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/properties/tests/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/properties/tests/test_properties_scorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/properties/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.665968 gt4sd-1.4.0/src/gt4sd/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.665968 gt4sd-1.4.0/src/gt4sd/training_pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.665968 gt4sd-1.4.0/src/gt4sd/training_pipelines/cgcnn/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/cgcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24878 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/cgcnn/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.665968 gt4sd-1.4.0/src/gt4sd/training_pipelines/crystals_crf/
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/crystals_crf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/crystals_crf/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.669968 gt4sd-1.4.0/src/gt4sd/training_pipelines/diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16237 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/diffusion/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.669968 gt4sd-1.4.0/src/gt4sd/training_pipelines/guacamol_baselines/
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/guacamol_baselines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/guacamol_baselines/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.669968 gt4sd-1.4.0/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/mock_training_pipeline.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.669968 gt4sd-1.4.0/src/gt4sd/training_pipelines/moses/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/moses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/moses/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.669968 gt4sd-1.4.0/src/gt4sd/training_pipelines/moses/organ/
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/moses/organ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/moses/organ/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.669968 gt4sd-1.4.0/src/gt4sd/training_pipelines/moses/vae/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/moses/vae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/moses/vae/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.669968 gt4sd-1.4.0/src/gt4sd/training_pipelines/paccmann/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/paccmann/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/paccmann/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.669968 gt4sd-1.4.0/src/gt4sd/training_pipelines/paccmann/vae/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/paccmann/vae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13987 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/paccmann/vae/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.669968 gt4sd-1.4.0/src/gt4sd/training_pipelines/pytorch_lightning/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/pytorch_lightning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.669968 gt4sd-1.4.0/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16893 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.669968 gt4sd-1.4.0/src/gt4sd/training_pipelines/pytorch_lightning/granular/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/pytorch_lightning/granular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/pytorch_lightning/granular/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.669968 gt4sd-1.4.0/src/gt4sd/training_pipelines/pytorch_lightning/molformer/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/pytorch_lightning/molformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16070 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/pytorch_lightning/molformer/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.673968 gt4sd-1.4.0/src/gt4sd/training_pipelines/regression_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/regression_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/regression_transformer/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    15316 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/regression_transformer/implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16473 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/regression_transformer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/terminator_training.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.673968 gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/molecules.smi
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_cgnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_crystals_rfc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_gflownet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_guacamol_baselines_smiles_lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_moses_organ.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_moses_vae.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_paccmann_vae.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_regression_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_torchdrug_gcpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_torchdrug_graphaf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.673968 gt4sd-1.4.0/src/gt4sd/training_pipelines/torchdrug/
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/torchdrug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/torchdrug/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/torchdrug/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.677968 gt4sd-1.4.0/src/gt4sd/training_pipelines/torchdrug/gcpn/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/torchdrug/gcpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11880 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/torchdrug/gcpn/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.677968 gt4sd-1.4.0/src/gt4sd/training_pipelines/torchdrug/graphaf/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/torchdrug/graphaf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13413 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/torchdrug/graphaf/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-03-07 15:49:13.000000 gt4sd-1.4.0/src/gt4sd/training_pipelines/torchdrug/unpatch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:49:18.677968 gt4sd-1.4.0/src/gt4sd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19936 2024-03-07 15:49:18.000000 gt4sd-1.4.0/src/gt4sd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15802 2024-03-07 15:49:18.000000 gt4sd-1.4.0/src/gt4sd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 15:49:18.000000 gt4sd-1.4.0/src/gt4sd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-07 15:49:18.000000 gt4sd-1.4.0/src/gt4sd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-07 15:49:18.000000 gt4sd-1.4.0/src/gt4sd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-07 15:49:18.000000 gt4sd-1.4.0/src/gt4sd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-25 07:08:01.000000 gt4sd-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18722 2024-04-25 07:08:08.000000 gt4sd-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18258 2024-04-25 07:08:01.000000 gt4sd-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-25 07:08:01.000000 gt4sd-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-25 07:08:08.000000 gt4sd-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-25 07:08:01.000000 gt4sd-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29460 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/
+-rw-r--r--   0 runner    (1001) docker     (127)    22153 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_mcts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_aae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_organ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_vae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_hc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/key_bert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/key_bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/key_bert/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/key_bert/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/molgx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/molgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8860 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/molgx/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/molgx/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/paccmann_rl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/paccmann_rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/paccmann_rl/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14210 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/paccmann_rl/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/regression_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/regression_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20484 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/regression_transformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53178 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/regression_transformer/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/regression_transformer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/reinvent/
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/reinvent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/reinvent/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/reinvent/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/template/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/template/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/template/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/tests/test_guacamol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/tests/test_key_bert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/tests/test_molgx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/tests/test_moses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/tests/test_paccmann_rl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14669 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/tests/test_regression_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/tests/test_reinvent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19830 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13448 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/tests/test_advanced_manufacturing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/tests/test_class_controlled_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/tests/test_paccmann_gp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34978 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12649 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/geodiff/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/geodiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/geodiff/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/geodiff/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/geodiff/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/geodiff/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/geodiff/model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/geodiff/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/hugging_face/
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/hugging_face/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12564 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/hugging_face/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/hugging_face/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/moler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/moler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/moler/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/moler/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/paccmann_vae/
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/paccmann_vae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/paccmann_vae/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/paccmann_vae/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/pgt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/pgt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13254 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/pgt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15685 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/pgt/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/polymer_blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/polymer_blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/polymer_blocks/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/polymer_blocks/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128648 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/tests/mol_dct.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/tests/test_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/tests/test_hugging_face.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/tests/test_moler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/tests/test_paccmann_vae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/tests/test_pgt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/tests/test_polymer_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/tests/test_torchdrug.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/torchdrug/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/torchdrug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/torchdrug/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/generation/torchdrug/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/prediction/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/prediction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/prediction/paccmann/
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/prediction/paccmann/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/prediction/paccmann/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/prediction/paccmann/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/prediction/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/prediction/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/prediction/tests/test_paccmann.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/prediction/tests/test_topics_zero_shot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/prediction/topics_zero_shot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/prediction/topics_zero_shot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/prediction/topics_zero_shot/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/prediction/topics_zero_shot/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14124 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/algorithms/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/algorithms/tests/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/cli/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/cli/argument_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4380 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/cli/hf_to_st_converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6910 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/cli/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/cli/load_arguments_from_dataclass.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7893 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/cli/saving.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6950 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/cli/trainer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8169 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/cli/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12452 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/domains/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/domains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/domains/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/domains/materials/
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/domains/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/domains/materials/protein_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/domains/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/domains/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/cgcnn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/cgcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/cgcnn/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/cgcnn/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/crystals_rfc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/crystals_rfc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32266 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/crystals_rfc/atomic_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/crystals_rfc/feature_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/crystals_rfc/rf_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/enzeptional/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/enzeptional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24803 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/enzeptional/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20040 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/enzeptional/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/enzeptional/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/enzeptional/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/enzeptional/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/enzeptional/tests/test_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/arg_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/arg_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/arg_parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/arg_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/dataloader/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/dataloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/dataloader/data_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11695 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/dataloader/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11674 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/dataloader/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27081 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/envs/graph_building_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14389 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/envs/mol_building_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/loss/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/loss/td_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19297 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/loss/trajectory_balance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/ml/models/graph_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34044 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/ml/models/mxmnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/ml/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/tests/qm9.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/tests/test_gfn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/train/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/train/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/arg_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/arg_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/arg_parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/arg_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/dataloader/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/dataloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/dataloader/data_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18863 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/dataloader/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/dataloader/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35475 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/no_encoding/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/no_encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/no_encoding/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/vae_mlp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/vae_mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10825 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/vae_mlp/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/vae_rnn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/vae_rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12917 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/vae_rnn/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/vae_trans/
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/vae_trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/vae_trans/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18134 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/tokenizer/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/train/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/granular/train/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/frameworks/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/frameworks/torch/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/properties/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/properties/crystals/
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/properties/crystals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11103 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/properties/crystals/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/properties/molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/properties/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30897 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/properties/molecules/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/properties/molecules/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/properties/proteins/
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/properties/proteins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/properties/proteins/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/properties/proteins/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/properties/scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/properties/scores/
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/properties/scores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/properties/scores/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/properties/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/properties/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9859 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/properties/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/properties/tests/test_properties_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/properties/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/cgcnn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/cgcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24878 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/cgcnn/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/crystals_crf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/crystals_crf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/crystals_crf/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16237 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/diffusion/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/guacamol_baselines/
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/guacamol_baselines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/guacamol_baselines/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/mock_training_pipeline.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/moses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/moses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/moses/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/moses/organ/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/moses/organ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/moses/organ/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/moses/vae/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/moses/vae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/moses/vae/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/paccmann/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/paccmann/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/paccmann/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/paccmann/vae/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/paccmann/vae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13987 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/paccmann/vae/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/pytorch_lightning/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/pytorch_lightning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16893 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/pytorch_lightning/granular/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/pytorch_lightning/granular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/pytorch_lightning/granular/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/pytorch_lightning/molformer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/pytorch_lightning/molformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16070 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/pytorch_lightning/molformer/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/regression_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/regression_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/regression_transformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15316 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/regression_transformer/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16473 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/regression_transformer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/terminator_training.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/molecules.smi
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_cgnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_crystals_rfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_gflownet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_guacamol_baselines_smiles_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_moses_organ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_moses_vae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_paccmann_vae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_regression_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_torchdrug_gcpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_torchdrug_graphaf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/torchdrug/
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/torchdrug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/torchdrug/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/torchdrug/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/torchdrug/gcpn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/torchdrug/gcpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11880 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/torchdrug/gcpn/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/torchdrug/graphaf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/torchdrug/graphaf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13413 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/torchdrug/graphaf/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-04-25 07:08:01.000000 gt4sd-1.4.1/src/gt4sd/training_pipelines/torchdrug/unpatch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18722 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15802 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 07:08:08.000000 gt4sd-1.4.1/src/gt4sd.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `gt4sd-1.4.0/LICENSE` & `gt4sd-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/PKG-INFO` & `gt4sd-1.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,20 @@
 Metadata-Version: 2.1
 Name: gt4sd
-Version: 1.4.0
+Version: 1.4.1
 Summary: Generative Toolkit for Scientific Discovery (GT4SD).
 Author: GT4SD team
 Keywords: GT4SD Generative Models Inference Training
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: accelerate
-Requires-Dist: datasets
-Requires-Dist: diffusers
-Requires-Dist: importlib_metadata
-Requires-Dist: importlib_resources
-Requires-Dist: ipaddress
-Requires-Dist: joblib
-Requires-Dist: gt4sd-molformer
-Requires-Dist: gt4sd-trainer-hf-pl
-Requires-Dist: keras
-Requires-Dist: keybert
-Requires-Dist: minio
-Requires-Dist: modlamp
-Requires-Dist: molecule_generation
-Requires-Dist: molgx
-Requires-Dist: nglview
-Requires-Dist: numpy
-Requires-Dist: pytorch_lightning
-Requires-Dist: pyarrow
-Requires-Dist: pydantic
-Requires-Dist: pymatgen
-Requires-Dist: pyTDC!=0.3.8
-Requires-Dist: pyyaml
-Requires-Dist: rdkit
-Requires-Dist: regex
-Requires-Dist: reinvent-chemistry
-Requires-Dist: sacremoses
-Requires-Dist: scikit-learn
-Requires-Dist: scikit-optimize
-Requires-Dist: scipy
-Requires-Dist: sentencepiece
-Requires-Dist: sympy
-Requires-Dist: tables
-Requires-Dist: tape-proteins
-Requires-Dist: tensorboard
-Requires-Dist: tensorflow
-Requires-Dist: torch
-Requires-Dist: torchdrug
-Requires-Dist: torchmetrics
-Requires-Dist: torchvision
-Requires-Dist: transformers<4.26.0
-Requires-Dist: typing_extensions
-Requires-Dist: wheel
 Provides-Extra: extras
-Requires-Dist: cogmol-inference; extra == "extras"
+License-File: LICENSE
 
 # GT4SD (Generative Toolkit for Scientific Discovery)
 
 [![PyPI version](https://badge.fury.io/py/gt4sd.svg)](https://badge.fury.io/py/gt4sd)
 [![Actions tests](https://github.com/gt4sd/gt4sd-core/actions/workflows/tests.yaml/badge.svg)](https://github.com/gt4sd/gt4sd-core/actions)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -93,40 +49,39 @@
 ### Conda
 
 The recommended way to install the `gt4sd` is to create a dedicated conda environment, this will ensure all requirements are satisfied. For CPU:
 
 ```sh
 git clone https://github.com/GT4SD/gt4sd-core.git
 cd gt4sd-core/
-conda env create -f conda.yml 
+conda env create -f conda_cpu_mac.yml # for linux use conda_cpu_linux.yml
 conda activate gt4sd
 pip install gt4sd
 ```
 
-**NOTE 1:** By default `gt4sd` is installed with CPU requirements. For GPU usage replace `conda env create -f conda.yml` with:
+**NOTE 1:** By default `gt4sd` is installed with CPU requirements. For GPU usage replace with:
+
 ```sh
 conda env create -f conda_gpu.yml
 ```
 
 **NOTE 2:** In case you want to reuse an existing compatible environment (see [requirements](#requirements)), you can use `pip`, but as of now (:eyes: on [issue](https://github.com/GT4SD/gt4sd-core/issues/31) for changes), some dependencies require installation from GitHub, so for a complete setup install them with:
 
 ```sh
 pip install -r vcs_requirements.txt
 ```
 
 A few VCS dependencies require Git LFS (make sure it's available on your system).
 
 ### Development setup & installation
 
-If you would like to contribute to the package, we recommend the following development setup:
+If you would like to contribute to the package, we recommend to install gt4sd in
+editable mode inside your `conda` environment:
 
 ```sh
-conda env create -f conda.yml
-conda activate gt4sd
-# install gt4sd in editable mode
 pip install --no-deps -e .
 ```
 
 Learn more in [CONTRIBUTING.md](./CONTRIBUTING.md)
 
 ## Getting started
```

### Comparing `gt4sd-1.4.0/README.md` & `gt4sd-1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,40 +35,39 @@
 ### Conda
 
 The recommended way to install the `gt4sd` is to create a dedicated conda environment, this will ensure all requirements are satisfied. For CPU:
 
 ```sh
 git clone https://github.com/GT4SD/gt4sd-core.git
 cd gt4sd-core/
-conda env create -f conda.yml 
+conda env create -f conda_cpu_mac.yml # for linux use conda_cpu_linux.yml
 conda activate gt4sd
 pip install gt4sd
 ```
 
-**NOTE 1:** By default `gt4sd` is installed with CPU requirements. For GPU usage replace `conda env create -f conda.yml` with:
+**NOTE 1:** By default `gt4sd` is installed with CPU requirements. For GPU usage replace with:
+
 ```sh
 conda env create -f conda_gpu.yml
 ```
 
 **NOTE 2:** In case you want to reuse an existing compatible environment (see [requirements](#requirements)), you can use `pip`, but as of now (:eyes: on [issue](https://github.com/GT4SD/gt4sd-core/issues/31) for changes), some dependencies require installation from GitHub, so for a complete setup install them with:
 
 ```sh
 pip install -r vcs_requirements.txt
 ```
 
 A few VCS dependencies require Git LFS (make sure it's available on your system).
 
 ### Development setup & installation
 
-If you would like to contribute to the package, we recommend the following development setup:
+If you would like to contribute to the package, we recommend to install gt4sd in
+editable mode inside your `conda` environment:
 
 ```sh
-conda env create -f conda.yml
-conda activate gt4sd
-# install gt4sd in editable mode
 pip install --no-deps -e .
 ```
 
 Learn more in [CONTRIBUTING.md](./CONTRIBUTING.md)
 
 ## Getting started
```

### Comparing `gt4sd-1.4.0/setup.cfg` & `gt4sd-1.4.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 	torch
 	torchdrug
 	torchmetrics
 	torchvision
 	transformers<4.26.0
 	typing_extensions
 	wheel
+	xgboost
 setup_requires = 
 	setuptools
 package_dir = 
 	= src
 packages = find_namespace:
 
 [options.entry_points]
@@ -276,11 +277,14 @@
 
 [mypy-tensorflow.*]
 ignore_missing_imports = True
 
 [mypy-ruamel.*]
 ignore_missing_imports = True
 
+[mypy-xgboost.*]
+ignore_missing_imports = True
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `gt4sd-1.4.0/src/gt4sd/__init__.py` & `gt4sd-1.4.1/src/gt4sd/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """Module initialization."""
 
-__version__ = "1.4.0"
+__version__ = "1.4.1"
 __name__ = "gt4sd"
 
 # NOTE: configure SSL to allow unverified contexts by default
 from .configuration import GT4SDConfiguration
 
 gt4sd_configuration_instance = GT4SDConfiguration.get_instance()
```

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_ga.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_ga.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_mcts.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/graph_mcts.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_aae.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_aae.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_organ.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_organ.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_vae.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/moses_vae.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_ga.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_ga.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_hc.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_hc.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_ppo.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/guacamol/implementation/smiles_lstm_ppo.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/key_bert/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/key_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/key_bert/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/key_bert/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/key_bert/implementation.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/key_bert/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/molgx/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/molgx/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/molgx/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/molgx/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/molgx/implementation.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/molgx/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/paccmann_rl/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/paccmann_rl/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/paccmann_rl/implementation.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/paccmann_rl/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/regression_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/regression_transformer/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/implementation.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/regression_transformer/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/regression_transformer/utils.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/regression_transformer/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/reinvent/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/reinvent/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/reinvent/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/reinvent/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/reinvent/implementation.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/reinvent/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/reinvent/reinvent_core/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/template/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/template/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/template/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/template/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/template/implementation.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/template/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/tests/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/tests/test_guacamol.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/tests/test_guacamol.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/tests/test_key_bert.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/tests/test_key_bert.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/tests/test_molgx.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/tests/test_molgx.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/tests/test_moses.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/tests/test_moses.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/tests/test_paccmann_rl.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/tests/test_paccmann_rl.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/tests/test_regression_transformer.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/tests/test_regression_transformer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/conditional_generation/tests/test_reinvent.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/conditional_generation/tests/test_reinvent.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/advanced_manufacturing/implementation/nccr/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/class_controlled_sampling/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/implementation.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/paccmann_gp/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/tests/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/tests/test_advanced_manufacturing.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/tests/test_advanced_manufacturing.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/tests/test_class_controlled_sampling.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/tests/test_class_controlled_sampling.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/controlled_sampling/tests/test_paccmann_gp.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/controlled_sampling/tests/test_paccmann_gp.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/geodiff/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/geodiff/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/geodiff/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/geodiff/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/geodiff/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/geodiff/model/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/layers.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/geodiff/model/layers.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/geodiff/model/utils.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/geodiff/model/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/diffusion/implementation.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/diffusion/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/hugging_face/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/hugging_face/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/hugging_face/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/hugging_face/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/hugging_face/implementation.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/hugging_face/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/moler/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/moler/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/moler/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/moler/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/moler/implementation.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/moler/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/paccmann_vae/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/paccmann_vae/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/paccmann_vae/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/paccmann_vae/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/paccmann_vae/implementation.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/paccmann_vae/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/pgt/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/pgt/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/pgt/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/pgt/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/pgt/implementation.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/pgt/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/polymer_blocks/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/polymer_blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/polymer_blocks/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/polymer_blocks/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/polymer_blocks/implementation.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/polymer_blocks/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/tests/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/tests/mol_dct.pkl` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/tests/mol_dct.pkl`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/tests/test_diffusion.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/tests/test_diffusion.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/tests/test_hugging_face.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/tests/test_hugging_face.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/tests/test_moler.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/tests/test_moler.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/tests/test_paccmann_vae.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/tests/test_paccmann_vae.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/tests/test_pgt.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/tests/test_pgt.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/tests/test_polymer_blocks.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/tests/test_polymer_blocks.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/tests/test_torchdrug.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/tests/test_torchdrug.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/torchdrug/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/torchdrug/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/torchdrug/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/torchdrug/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/generation/torchdrug/implementation.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/generation/torchdrug/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/prediction/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/prediction/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/prediction/paccmann/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/prediction/paccmann/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/prediction/paccmann/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/prediction/paccmann/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/prediction/paccmann/implementation.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/prediction/paccmann/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/prediction/tests/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/prediction/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/prediction/tests/test_paccmann.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/prediction/tests/test_paccmann.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/prediction/tests/test_topics_zero_shot.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/prediction/tests/test_topics_zero_shot.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/prediction/topics_zero_shot/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/prediction/topics_zero_shot/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/prediction/topics_zero_shot/core.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/prediction/topics_zero_shot/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/prediction/topics_zero_shot/implementation.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/prediction/topics_zero_shot/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/registry.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/registry.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/tests/__init__.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/tests/test_config.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/algorithms/tests/test_registry.py` & `gt4sd-1.4.1/src/gt4sd/algorithms/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/cli/__init__.py` & `gt4sd-1.4.1/src/gt4sd/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/cli/algorithms.py` & `gt4sd-1.4.1/src/gt4sd/cli/algorithms.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/cli/argument_parser.py` & `gt4sd-1.4.1/src/gt4sd/cli/argument_parser.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/cli/hf_to_st_converter.py` & `gt4sd-1.4.1/src/gt4sd/cli/hf_to_st_converter.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/cli/inference.py` & `gt4sd-1.4.1/src/gt4sd/cli/inference.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/cli/load_arguments_from_dataclass.py` & `gt4sd-1.4.1/src/gt4sd/cli/load_arguments_from_dataclass.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/cli/saving.py` & `gt4sd-1.4.1/src/gt4sd/cli/saving.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/cli/trainer.py` & `gt4sd-1.4.1/src/gt4sd/cli/trainer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/cli/upload.py` & `gt4sd-1.4.1/src/gt4sd/cli/upload.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/configuration.py` & `gt4sd-1.4.1/src/gt4sd/configuration.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/conftest.py` & `gt4sd-1.4.1/src/gt4sd/conftest.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/domains/__init__.py` & `gt4sd-1.4.1/src/gt4sd/domains/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/domains/core.py` & `gt4sd-1.4.1/src/gt4sd/domains/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/domains/materials/__init__.py` & `gt4sd-1.4.1/src/gt4sd/domains/materials/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/domains/materials/protein_encoding.py` & `gt4sd-1.4.1/src/gt4sd/domains/materials/protein_encoding.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/domains/tests/__init__.py` & `gt4sd-1.4.1/src/gt4sd/domains/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/exceptions.py` & `gt4sd-1.4.1/src/gt4sd/exceptions.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/extras/__init__.py` & `gt4sd-1.4.1/src/gt4sd/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/cgcnn/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/cgcnn/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/cgcnn/data.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/cgcnn/data.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/cgcnn/model.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/cgcnn/model.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/crystals_rfc/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/crystals_rfc/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/crystals_rfc/atomic_data.csv` & `gt4sd-1.4.1/src/gt4sd/frameworks/crystals_rfc/atomic_data.csv`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/crystals_rfc/feature_engine.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/crystals_rfc/feature_engine.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/crystals_rfc/rf_classifier.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/crystals_rfc/rf_classifier.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/enzeptional/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/enzeptional/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/enzeptional/core.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/enzeptional/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional, Tuple
 import random
 import logging
 from itertools import product as iter_product
 import time
 from joblib import load
+import xgboost as xgb
 from .processing import (
     HFandTAPEModelUtility,
     SelectionGenerator,
     CrossoverGenerator,
     sanitize_intervals,
     sanitize_intervals_with_padding,
 )
@@ -363,38 +364,44 @@
         top_k: int = 2,
         selection_ratio: float = 0.5,
         perform_crossover: bool = False,
         crossover_type: str = "uniform",
         minimum_interval_length: int = 8,
         pad_intervals: bool = False,
         concat_order=["sequence", "substrate", "product"],
+        scaler_filepath: Optional[str] = None,
+        use_xgboost_scorer: Optional[bool] = False,
     ):
         """Initializes the optimizer with models, sequences, and
         optimization parameters.
 
 
         Args:
             sequence (str): The initial protein sequence.
             protein_model (HFandTAPEModelUtility): Model for protein embeddings.
             substrate_smiles (str): SMILES representation of the substrate.
             product_smiles (str): SMILES representation of the product.
             chem_model_path (str): Path to the chemical model.
             chem_tokenizer_path (str): Path to the chemical tokenizer.
-            scorer_filepath (str): Path to the scoring model.
-            mutator (SequenceMutator): The mutator for generating sequence variants.
-            intervals (List[Tuple[int, int]]): Intervals for mutation.
-            batch_size (int, optional): The number of sequences to process in one batch. Defaults to 2.
-            seed (int, optional): Random seed. Defaults to 123.
-            top_k (int, optional): Number of top mutations to consider. Defaults to 2.
-            selection_ratio (float, optional): Ratio of sequences to select after scoring. Defaults to 0.5.
-            perform_crossover (bool, optional): Flag to perform crossover operation. Defaults to False.
-            crossover_type (str, optional): Type of crossover operation. Defaults to "uniform".
-            minimum_interval_length (int, optional): Minimum length of mutation intervals. Defaults to 8.
-            pad_intervals (bool, optional): Flag to pad the intervals. Defaults to False.
-            concat_order (list, optional): Order of concatenating embeddings. Defaults to ["sequence", "substrate", "product"].
+            scorer_filepath (str): File path to the scoring model.
+            mutator (SequenceMutator): The mutator for generating
+            sequence variants.
+            intervals (List[List[int]]): Intervals for mutation.
+            batch_size (int): The number of sequences to process in one batch.
+            top_k (int): Number of top mutations to consider.
+            selection_ratio (float): Ratio of sequences to select
+            after scoring.
+            perform_crossover (bool): Flag to perform crossover operation.
+            crossover_type (str): Type of crossover operation.
+            minimum_interval_length (int): Minimum length of
+            mutation intervals.
+            pad_intervals (bool): Flag to pad the intervals.
+            concat_order (list): Order of concatenating embeddings.
+            scaler_filepath (str): Path to the scaller in case you are usinh the Kcat model.
+            use_xgboost_scorer (bool): flag to specify if the fitness function is the Kcat.
         """
         self.sequence = sequence
         self.protein_model = protein_model
         self.mutator = mutator
         self.intervals = intervals
         self.batch_size = batch_size
         self.top_k = top_k
@@ -403,15 +410,17 @@
         self.crossover_type = crossover_type
         self.concat_order = concat_order
         self.minimum_interval_length = minimum_interval_length
         self.pad_intervals = pad_intervals
         self.mutator.set_top_k(top_k)
         self.concat_order = concat_order
         self.scorer = load(scorer_filepath)
-        self.seed = seed
+        if scaler_filepath is not None:
+            self.scaler = load(scaler_filepath)
+        self.use_xgboost_scorer = use_xgboost_scorer
 
         self.chem_model = HFandTAPEModelUtility(chem_model_path, chem_tokenizer_path)
         self.substrate_embedding = self.chem_model.embed([substrate_smiles])[0]
         self.product_embedding = self.chem_model.embed([product_smiles])[0]
 
         self.selection_generator = SelectionGenerator()
         self.crossover_generator = CrossoverGenerator()
@@ -420,15 +429,15 @@
             self.intervals = [(0, len(sequence))]
         else:
             self.intervals = sanitize_intervals(intervals)
             if pad_intervals:
                 self.intervals = sanitize_intervals_with_padding(
                     self.intervals, minimum_interval_length, len(sequence)
                 )
-
+        self.seed = seed
         random.seed(self.seed)
 
     def optimize(
         self,
         num_iterations: int,
         num_sequences: int,
         num_mutations: int,
@@ -610,15 +619,21 @@
         ]
         ordered_embeddings = [
             embeddings[self.concat_order.index(item)] for item in self.concat_order
         ]
         combined_embedding = np.concatenate(ordered_embeddings)
         combined_embedding = combined_embedding.reshape(1, -1)
 
-        score = self.scorer.predict_proba(combined_embedding)[0][1]
+        if self.use_xgboost_scorer:
+            if self.scaler is not None:
+                combined_embedding = self.scaler.transform(combined_embedding)
+            score = self.scorer.predict(xgb.DMatrix(combined_embedding))[0]
+        else:
+            score = self.scorer.predict_proba(combined_embedding)[0][1]
+
         return {"sequence": sequence, "score": score}
 
     def score_sequences(self, sequences: List[str]) -> List[Dict[str, float]]:
         """Scores a list of protein sequences.
 
         Args:
             sequences (List[str]): The list of protein sequences to score.
@@ -639,11 +654,16 @@
             ]
             ordered_embeddings = [
                 embeddings[self.concat_order.index(item)] for item in self.concat_order
             ]
             combined_embedding = np.concatenate(ordered_embeddings)
             combined_embedding = combined_embedding.reshape(1, -1)
 
-            score = self.scorer.predict_proba(combined_embedding)[0][1]
+            if self.use_xgboost_scorer:
+                if self.scaler is not None:
+                    combined_embedding = self.scaler.transform(combined_embedding)
+                score = self.scorer.predict(xgb.DMatrix(combined_embedding))[0]
+            else:
+                score = self.scorer.predict_proba(combined_embedding)[0][1]
             output.append({"sequence": sequences[position], "score": score})
 
         return output
```

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/enzeptional/processing.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/enzeptional/processing.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/enzeptional/tests/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/enzeptional/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/enzeptional/tests/test_core.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/enzeptional/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/enzeptional/tests/test_processing.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/enzeptional/tests/test_processing.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/arg_parser/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/arg_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/arg_parser/parser.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/arg_parser/parser.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/arg_parser/utils.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/arg_parser/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/dataloader/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/dataloader/data_module.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/dataloader/data_module.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/dataloader/dataset.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/dataloader/dataset.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/dataloader/sampler.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/dataloader/sampler.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/envs/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/envs/graph_building_env.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/envs/graph_building_env.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/envs/mol_building_env.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/envs/mol_building_env.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/loss/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/loss/td_loss.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/loss/td_loss.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/loss/trajectory_balance.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/loss/trajectory_balance.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/ml/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/ml/models/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/ml/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/ml/models/graph_transformer.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/ml/models/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/ml/models/mxmnet.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/ml/models/mxmnet.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/ml/module.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/ml/module.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/tests/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/tests/qm9.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/tests/qm9.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/tests/test_gfn.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/tests/test_gfn.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/train/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/train/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/train/core.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/train/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/gflownet/util.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/gflownet/util.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/arg_parser/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/arg_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/arg_parser/parser.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/arg_parser/parser.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/arg_parser/utils.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/arg_parser/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/dataloader/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/dataloader/data_module.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/dataloader/data_module.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/dataloader/dataset.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/dataloader/dataset.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/dataloader/sampler.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/dataloader/sampler.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/activation.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/activation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/base_model.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/base_model.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/loss.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/loss.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/core.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/mlp_auto_encoder/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/core.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/mlp_predictor/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/model_builder.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/model_builder.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/module.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/module.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/no_encoding/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/no_encoding/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/no_encoding/core.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/no_encoding/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/utils.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/vae_mlp/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/vae_mlp/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/vae_mlp/core.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/vae_mlp/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/vae_rnn/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/vae_rnn/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/vae_rnn/core.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/vae_rnn/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/vae_trans/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/vae_trans/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/models/vae_trans/core.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/models/vae_trans/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/ml/module.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/ml/module.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/tests/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/tests/test_tokenizer.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/tokenizer/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/tokenizer/tokenizer.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/train/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/train/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/granular/train/core.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/granular/train/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/torch/__init__.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/frameworks/torch/vae.py` & `gt4sd-1.4.1/src/gt4sd/frameworks/torch/vae.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/properties/__init__.py` & `gt4sd-1.4.1/src/gt4sd/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/properties/core.py` & `gt4sd-1.4.1/src/gt4sd/properties/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/properties/crystals/__init__.py` & `gt4sd-1.4.1/src/gt4sd/properties/crystals/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/properties/crystals/core.py` & `gt4sd-1.4.1/src/gt4sd/properties/crystals/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/properties/molecules/__init__.py` & `gt4sd-1.4.1/src/gt4sd/properties/molecules/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/properties/molecules/core.py` & `gt4sd-1.4.1/src/gt4sd/properties/molecules/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/properties/molecules/functions.py` & `gt4sd-1.4.1/src/gt4sd/properties/molecules/functions.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/properties/proteins/__init__.py` & `gt4sd-1.4.1/src/gt4sd/properties/proteins/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/properties/proteins/core.py` & `gt4sd-1.4.1/src/gt4sd/properties/proteins/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/properties/proteins/functions.py` & `gt4sd-1.4.1/src/gt4sd/properties/proteins/functions.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/properties/scorer.py` & `gt4sd-1.4.1/src/gt4sd/properties/scorer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/properties/scores/__init__.py` & `gt4sd-1.4.1/src/gt4sd/properties/scores/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/properties/scores/core.py` & `gt4sd-1.4.1/src/gt4sd/properties/scores/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/properties/tests/__init__.py` & `gt4sd-1.4.1/src/gt4sd/properties/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/properties/tests/test_properties.py` & `gt4sd-1.4.1/src/gt4sd/properties/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/properties/tests/test_properties_scorer.py` & `gt4sd-1.4.1/src/gt4sd/properties/tests/test_properties_scorer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/properties/utils.py` & `gt4sd-1.4.1/src/gt4sd/properties/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/s3.py` & `gt4sd-1.4.1/src/gt4sd/s3.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/tests/__init__.py` & `gt4sd-1.4.1/src/gt4sd/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/tests/test_configuration.py` & `gt4sd-1.4.1/src/gt4sd/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/tests/test_exceptions.py` & `gt4sd-1.4.1/src/gt4sd/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/tests/test_s3.py` & `gt4sd-1.4.1/src/gt4sd/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/tests/utils.py` & `gt4sd-1.4.1/src/gt4sd/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/__init__.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/cgcnn/__init__.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/cgcnn/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/cgcnn/core.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/cgcnn/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/core.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/crystals_crf/__init__.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/crystals_crf/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/crystals_crf/core.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/crystals_crf/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/diffusion/__init__.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/diffusion/core.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/diffusion/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/guacamol_baselines/__init__.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/guacamol_baselines/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/guacamol_baselines/core.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/guacamol_baselines/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/__init__.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/core.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/guacamol_baselines/smiles_lstm/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/moses/__init__.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/moses/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/moses/core.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/moses/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/moses/organ/__init__.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/moses/organ/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/moses/organ/core.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/moses/organ/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/moses/vae/__init__.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/moses/vae/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/moses/vae/core.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/moses/vae/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/paccmann/__init__.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/paccmann/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/paccmann/core.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/paccmann/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/paccmann/vae/__init__.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/paccmann/vae/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/paccmann/vae/core.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/paccmann/vae/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/pytorch_lightning/__init__.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/pytorch_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/__init__.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/core.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/pytorch_lightning/gflownet/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/pytorch_lightning/granular/__init__.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/pytorch_lightning/granular/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/pytorch_lightning/granular/core.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/pytorch_lightning/granular/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/pytorch_lightning/molformer/__init__.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/pytorch_lightning/molformer/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/pytorch_lightning/molformer/core.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/pytorch_lightning/molformer/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/regression_transformer/__init__.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/regression_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/regression_transformer/core.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/regression_transformer/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/regression_transformer/implementation.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/regression_transformer/implementation.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/regression_transformer/utils.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/regression_transformer/utils.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/terminator_training.json` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/terminator_training.json`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/__init__.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/molecules.smi` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/molecules.smi`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_argument_parser.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_argument_parser.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_cgnn.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_cgnn.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_crystals_rfc.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_crystals_rfc.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_diffusion.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_diffusion.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_gflownet.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_gflownet.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_guacamol_baselines_smiles_lstm.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_guacamol_baselines_smiles_lstm.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_moses_organ.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_moses_organ.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_moses_vae.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_moses_vae.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_paccmann_vae.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_paccmann_vae.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_pipelines.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_pipelines.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_regression_transformer.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_regression_transformer.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_torchdrug_gcpn.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_torchdrug_gcpn.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/tests/test_training_torchdrug_graphaf.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/tests/test_training_torchdrug_graphaf.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/torchdrug/__init__.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/torchdrug/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/torchdrug/core.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/torchdrug/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/torchdrug/dataset.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/torchdrug/dataset.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/torchdrug/gcpn/__init__.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/torchdrug/gcpn/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/torchdrug/gcpn/core.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/torchdrug/gcpn/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/torchdrug/graphaf/__init__.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/torchdrug/graphaf/__init__.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/torchdrug/graphaf/core.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/torchdrug/graphaf/core.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd/training_pipelines/torchdrug/unpatch.py` & `gt4sd-1.4.1/src/gt4sd/training_pipelines/torchdrug/unpatch.py`

 * *Files identical despite different names*

### Comparing `gt4sd-1.4.0/src/gt4sd.egg-info/PKG-INFO` & `gt4sd-1.4.1/src/gt4sd.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,20 @@
 Metadata-Version: 2.1
 Name: gt4sd
-Version: 1.4.0
+Version: 1.4.1
 Summary: Generative Toolkit for Scientific Discovery (GT4SD).
 Author: GT4SD team
 Keywords: GT4SD Generative Models Inference Training
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: accelerate
-Requires-Dist: datasets
-Requires-Dist: diffusers
-Requires-Dist: importlib_metadata
-Requires-Dist: importlib_resources
-Requires-Dist: ipaddress
-Requires-Dist: joblib
-Requires-Dist: gt4sd-molformer
-Requires-Dist: gt4sd-trainer-hf-pl
-Requires-Dist: keras
-Requires-Dist: keybert
-Requires-Dist: minio
-Requires-Dist: modlamp
-Requires-Dist: molecule_generation
-Requires-Dist: molgx
-Requires-Dist: nglview
-Requires-Dist: numpy
-Requires-Dist: pytorch_lightning
-Requires-Dist: pyarrow
-Requires-Dist: pydantic
-Requires-Dist: pymatgen
-Requires-Dist: pyTDC!=0.3.8
-Requires-Dist: pyyaml
-Requires-Dist: rdkit
-Requires-Dist: regex
-Requires-Dist: reinvent-chemistry
-Requires-Dist: sacremoses
-Requires-Dist: scikit-learn
-Requires-Dist: scikit-optimize
-Requires-Dist: scipy
-Requires-Dist: sentencepiece
-Requires-Dist: sympy
-Requires-Dist: tables
-Requires-Dist: tape-proteins
-Requires-Dist: tensorboard
-Requires-Dist: tensorflow
-Requires-Dist: torch
-Requires-Dist: torchdrug
-Requires-Dist: torchmetrics
-Requires-Dist: torchvision
-Requires-Dist: transformers<4.26.0
-Requires-Dist: typing_extensions
-Requires-Dist: wheel
 Provides-Extra: extras
-Requires-Dist: cogmol-inference; extra == "extras"
+License-File: LICENSE
 
 # GT4SD (Generative Toolkit for Scientific Discovery)
 
 [![PyPI version](https://badge.fury.io/py/gt4sd.svg)](https://badge.fury.io/py/gt4sd)
 [![Actions tests](https://github.com/gt4sd/gt4sd-core/actions/workflows/tests.yaml/badge.svg)](https://github.com/gt4sd/gt4sd-core/actions)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -93,40 +49,39 @@
 ### Conda
 
 The recommended way to install the `gt4sd` is to create a dedicated conda environment, this will ensure all requirements are satisfied. For CPU:
 
 ```sh
 git clone https://github.com/GT4SD/gt4sd-core.git
 cd gt4sd-core/
-conda env create -f conda.yml 
+conda env create -f conda_cpu_mac.yml # for linux use conda_cpu_linux.yml
 conda activate gt4sd
 pip install gt4sd
 ```
 
-**NOTE 1:** By default `gt4sd` is installed with CPU requirements. For GPU usage replace `conda env create -f conda.yml` with:
+**NOTE 1:** By default `gt4sd` is installed with CPU requirements. For GPU usage replace with:
+
 ```sh
 conda env create -f conda_gpu.yml
 ```
 
 **NOTE 2:** In case you want to reuse an existing compatible environment (see [requirements](#requirements)), you can use `pip`, but as of now (:eyes: on [issue](https://github.com/GT4SD/gt4sd-core/issues/31) for changes), some dependencies require installation from GitHub, so for a complete setup install them with:
 
 ```sh
 pip install -r vcs_requirements.txt
 ```
 
 A few VCS dependencies require Git LFS (make sure it's available on your system).
 
 ### Development setup & installation
 
-If you would like to contribute to the package, we recommend the following development setup:
+If you would like to contribute to the package, we recommend to install gt4sd in
+editable mode inside your `conda` environment:
 
 ```sh
-conda env create -f conda.yml
-conda activate gt4sd
-# install gt4sd in editable mode
 pip install --no-deps -e .
 ```
 
 Learn more in [CONTRIBUTING.md](./CONTRIBUTING.md)
 
 ## Getting started
```

### Comparing `gt4sd-1.4.0/src/gt4sd.egg-info/SOURCES.txt` & `gt4sd-1.4.1/src/gt4sd.egg-info/SOURCES.txt`

 * *Files identical despite different names*


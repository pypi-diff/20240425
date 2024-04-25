# Comparing `tmp/y0-0.2.8.tar.gz` & `tmp/y0-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "y0-0.2.8.tar", last modified: Sat Jan 27 10:17:37 2024, max compression
+gzip compressed data, was "y0-0.2.9.tar", last modified: Fri Mar 22 08:21:17 2024, max compression
```

## Comparing `y0-0.2.8.tar` & `y0-0.2.9.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.890333 y0-0.2.8/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1509 2023-08-16 16:13:12.000000 y0-0.2.8/LICENSE
--rw-r--r--   0 cthoyt     (501) staff       (20)      359 2023-08-16 16:13:12.000000 y0-0.2.8/MANIFEST.in
--rw-r--r--   0 cthoyt     (501) staff       (20)    11035 2024-01-27 10:17:37.890250 y0-0.2.8/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     8916 2024-01-17 08:44:23.000000 y0-0.2.8/README.md
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.864516 y0-0.2.8/docs/
--rw-r--r--   0 cthoyt     (501) staff       (20)      605 2023-08-16 16:13:12.000000 y0-0.2.8/docs/Makefile
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.867810 y0-0.2.8/docs/source/
--rw-r--r--   0 cthoyt     (501) staff       (20)      191 2023-08-08 20:19:58.000000 y0-0.2.8/docs/source/cli.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      321 2024-01-26 18:14:16.000000 y0-0.2.8/docs/source/conditional_independence.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     6956 2024-01-27 10:17:37.000000 y0-0.2.8/docs/source/conf.py
--rw-r--r--   0 cthoyt     (501) staff       (20)       63 2023-08-08 20:19:58.000000 y0-0.2.8/docs/source/dsl.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       72 2023-08-08 20:19:58.000000 y0-0.2.8/docs/source/examples.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       51 2023-08-08 20:19:58.000000 y0-0.2.8/docs/source/graph.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      595 2024-01-27 10:16:25.000000 y0-0.2.8/docs/source/graph_mutation.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       82 2024-01-17 08:44:23.000000 y0-0.2.8/docs/source/identification.rst
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.868506 y0-0.2.8/docs/source/img/
--rw-r--r--   0 cthoyt     (501) staff       (20)    87578 2023-08-16 16:13:12.000000 y0-0.2.8/docs/source/img/simulation_graph_algorithm.png
--rw-r--r--   0 cthoyt     (501) staff       (20)    29002 2023-08-16 16:13:12.000000 y0-0.2.8/docs/source/img/simulation_graph_diagram.png
--rw-r--r--   0 cthoyt     (501) staff       (20)      391 2024-01-27 10:16:49.000000 y0-0.2.8/docs/source/index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      505 2023-08-08 20:19:58.000000 y0-0.2.8/docs/source/installation.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     7328 2023-08-08 20:19:58.000000 y0-0.2.8/docs/source/logo.png
--rw-r--r--   0 cthoyt     (501) staff       (20)      159 2024-01-17 08:44:23.000000 y0-0.2.8/docs/source/lvdags.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       58 2023-08-16 16:13:12.000000 y0-0.2.8/docs/source/mutation.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       54 2023-08-08 20:19:58.000000 y0-0.2.8/docs/source/parser.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       72 2024-01-17 08:44:23.000000 y0-0.2.8/docs/source/struct.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       73 2024-01-26 07:45:26.000000 y0-0.2.8/docs/source/transport.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      350 2023-08-16 16:13:12.000000 y0-0.2.8/pyproject.toml
--rw-r--r--   0 cthoyt     (501) staff       (20)     2532 2024-01-27 10:17:37.890702 y0-0.2.8/setup.cfg
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.862897 y0-0.2.8/src/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.862731 y0-0.2.8/src/kestrel/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.862768 y0-0.2.8/src/kestrel/curation/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.862804 y0-0.2.8/src/kestrel/curation/vaccines/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.868675 y0-0.2.8/src/kestrel/curation/vaccines/.ipynb_checkpoints/
--rw-r--r--   0 cthoyt     (501) staff       (20)    37588 2023-09-18 11:22:16.000000 y0-0.2.8/src/kestrel/curation/vaccines/.ipynb_checkpoints/Platforms-checkpoint.ipynb
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.872666 y0-0.2.8/src/y0/
--rw-r--r--   0 cthoyt     (501) staff       (20)       64 2023-08-08 20:19:58.000000 y0-0.2.8/src/y0/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      319 2023-08-16 16:13:12.000000 y0-0.2.8/src/y0/__main__.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.874713 y0-0.2.8/src/y0/algorithm/
--rw-r--r--   0 cthoyt     (501) staff       (20)       71 2023-08-08 20:19:58.000000 y0-0.2.8/src/y0/algorithm/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    10341 2024-01-27 10:16:25.000000 y0-0.2.8/src/y0/algorithm/conditional_independencies.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.875337 y0-0.2.8/src/y0/algorithm/estimation/
--rw-r--r--   0 cthoyt     (501) staff       (20)     3702 2024-01-17 08:44:23.000000 y0-0.2.8/src/y0/algorithm/estimation/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1488 2024-01-19 14:49:13.000000 y0-0.2.8/src/y0/algorithm/estimation/linear_scm.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     4652 2024-01-26 18:14:15.000000 y0-0.2.8/src/y0/algorithm/falsification.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.877296 y0-0.2.8/src/y0/algorithm/identify/
--rw-r--r--   0 cthoyt     (501) staff       (20)     3211 2024-01-26 18:14:16.000000 y0-0.2.8/src/y0/algorithm/identify/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     7923 2023-09-06 15:45:51.000000 y0-0.2.8/src/y0/algorithm/identify/_extras.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1602 2024-01-17 08:44:23.000000 y0-0.2.8/src/y0/algorithm/identify/api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    19765 2024-01-17 09:02:23.000000 y0-0.2.8/src/y0/algorithm/identify/cg.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2253 2024-01-26 18:14:16.000000 y0-0.2.8/src/y0/algorithm/identify/id_c.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    12056 2024-01-26 18:14:16.000000 y0-0.2.8/src/y0/algorithm/identify/id_star.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    12056 2024-01-26 18:14:16.000000 y0-0.2.8/src/y0/algorithm/identify/id_std.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     8787 2024-01-26 18:14:16.000000 y0-0.2.8/src/y0/algorithm/identify/idc_star.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    11617 2024-01-26 13:13:33.000000 y0-0.2.8/src/y0/algorithm/identify/utils.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.877799 y0-0.2.8/src/y0/algorithm/separation/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1929 2024-01-26 18:14:16.000000 y0-0.2.8/src/y0/algorithm/separation/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    10601 2024-01-26 18:14:16.000000 y0-0.2.8/src/y0/algorithm/separation/sigma_separation.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     7753 2024-01-27 10:00:53.000000 y0-0.2.8/src/y0/algorithm/simplify_latent.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    11681 2024-01-17 08:44:23.000000 y0-0.2.8/src/y0/algorithm/taheri_design.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    29280 2024-01-17 08:44:23.000000 y0-0.2.8/src/y0/algorithm/transport.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      775 2023-08-16 16:42:32.000000 y0-0.2.8/src/y0/causaleffect.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      830 2023-08-16 16:13:12.000000 y0-0.2.8/src/y0/cli.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2401 2023-09-08 17:44:46.000000 y0-0.2.8/src/y0/complexity.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    64083 2024-01-27 09:01:58.000000 y0-0.2.8/src/y0/dsl.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.879387 y0-0.2.8/src/y0/examples/
--rw-r--r--   0 cthoyt     (501) staff       (20)    42564 2024-01-17 08:44:23.000000 y0-0.2.8/src/y0/examples/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1610 2023-09-06 15:45:51.000000 y0-0.2.8/src/y0/examples/backdoor.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1778 2023-09-06 15:45:51.000000 y0-0.2.8/src/y0/examples/frontdoor.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1808 2024-01-26 13:08:36.000000 y0-0.2.8/src/y0/examples/frontdoor_backdoor.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3612 2023-09-06 15:45:51.000000 y0-0.2.8/src/y0/examples/sars.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1858 2024-01-17 08:44:23.000000 y0-0.2.8/src/y0/examples/smoke_cancer.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1798 2024-01-19 14:49:13.000000 y0-0.2.8/src/y0/examples/utils.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    34957 2024-01-27 09:43:37.000000 y0-0.2.8/src/y0/graph.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.880427 y0-0.2.8/src/y0/mutate/
--rw-r--r--   0 cthoyt     (501) staff       (20)      334 2023-08-16 16:13:12.000000 y0-0.2.8/src/y0/mutate/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     4309 2024-01-17 09:02:23.000000 y0-0.2.8/src/y0/mutate/canonicalize_expr.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     4488 2024-01-17 08:44:23.000000 y0-0.2.8/src/y0/mutate/chain.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1773 2024-01-17 08:44:23.000000 y0-0.2.8/src/y0/mutate/contract.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1757 2024-01-17 08:44:23.000000 y0-0.2.8/src/y0/mutate/utils.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.881085 y0-0.2.8/src/y0/parser/
--rw-r--r--   0 cthoyt     (501) staff       (20)      185 2023-09-08 17:44:46.000000 y0-0.2.8/src/y0/parser/__init__.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.881622 y0-0.2.8/src/y0/parser/ce/
--rw-r--r--   0 cthoyt     (501) staff       (20)      108 2023-08-16 16:13:12.000000 y0-0.2.8/src/y0/parser/ce/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1976 2023-09-08 17:44:46.000000 y0-0.2.8/src/y0/parser/ce/grammar.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1919 2023-09-08 17:44:46.000000 y0-0.2.8/src/y0/parser/ce/utils.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1423 2024-01-17 08:44:23.000000 y0-0.2.8/src/y0/parser/internal.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1055 2023-08-16 16:13:12.000000 y0-0.2.8/src/y0/predicates.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1831 2023-08-16 16:42:32.000000 y0-0.2.8/src/y0/r_utils.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.882998 y0-0.2.8/src/y0/resources/
--rw-r--r--   0 cthoyt     (501) staff       (20)      226 2023-08-16 16:13:12.000000 y0-0.2.8/src/y0/resources/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)   242724 2023-08-16 16:13:12.000000 y0-0.2.8/src/y0/resources/asia.csv
--rw-r--r--   0 cthoyt     (501) staff       (20)    72805 2023-08-16 16:13:12.000000 y0-0.2.8/src/y0/resources/viral_pathogenesis.json
--rw-r--r--   0 cthoyt     (501) staff       (20)     6719 2024-01-19 14:49:13.000000 y0-0.2.8/src/y0/simulation.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     8935 2024-01-26 18:20:51.000000 y0-0.2.8/src/y0/struct.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.883187 y0-0.2.8/src/y0/util/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1503 2023-08-16 16:13:12.000000 y0-0.2.8/src/y0/util/combinatorics.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      984 2024-01-27 10:17:37.000000 y0-0.2.8/src/y0/version.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.873665 y0-0.2.8/src/y0.egg-info/
--rw-r--r--   0 cthoyt     (501) staff       (20)    11035 2024-01-27 10:17:37.000000 y0-0.2.8/src/y0.egg-info/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     3271 2024-01-27 10:17:37.000000 y0-0.2.8/src/y0.egg-info/SOURCES.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2024-01-27 10:17:37.000000 y0-0.2.8/src/y0.egg-info/dependency_links.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       35 2024-01-27 10:17:37.000000 y0-0.2.8/src/y0.egg-info/entry_points.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-08-09 17:14:42.000000 y0-0.2.8/src/y0.egg-info/not-zip-safe
--rw-r--r--   0 cthoyt     (501) staff       (20)      222 2024-01-27 10:17:37.000000 y0-0.2.8/src/y0.egg-info/requires.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        3 2024-01-27 10:17:37.000000 y0-0.2.8/src/y0.egg-info/top_level.txt
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.884752 y0-0.2.8/tests/
--rw-r--r--   0 cthoyt     (501) staff       (20)       52 2023-08-08 20:19:58.000000 y0-0.2.8/tests/__init__.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.884924 y0-0.2.8/tests/data/
--rw-r--r--   0 cthoyt     (501) staff       (20)     3419 2024-01-17 08:44:23.000000 y0-0.2.8/tests/data/generate.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.887749 y0-0.2.8/tests/test_algorithm/
--rw-r--r--   0 cthoyt     (501) staff       (20)       53 2023-08-08 20:19:58.000000 y0-0.2.8/tests/test_algorithm/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2082 2024-01-26 07:45:26.000000 y0-0.2.8/tests/test_algorithm/cases.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    33649 2024-01-17 09:02:23.000000 y0-0.2.8/tests/test_algorithm/test_cg.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    10896 2024-01-26 18:14:48.000000 y0-0.2.8/tests/test_algorithm/test_conditional_independencies.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3079 2024-01-26 13:40:51.000000 y0-0.2.8/tests/test_algorithm/test_falsification.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    12601 2024-01-17 08:44:23.000000 y0-0.2.8/tests/test_algorithm/test_id_alg.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    23264 2023-09-06 15:45:51.000000 y0-0.2.8/tests/test_algorithm/test_id_star.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    21609 2023-09-06 15:45:51.000000 y0-0.2.8/tests/test_algorithm/test_original_id_star.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     4014 2024-01-26 18:14:16.000000 y0-0.2.8/tests/test_algorithm/test_sigma_separation.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    17840 2024-01-17 08:44:23.000000 y0-0.2.8/tests/test_algorithm/test_simplify_latent.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    36423 2024-01-17 08:44:23.000000 y0-0.2.8/tests/test_algorithm/test_transport.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2318 2023-08-29 10:54:36.000000 y0-0.2.8/tests/test_causaleffect.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2972 2023-08-16 16:13:12.000000 y0-0.2.8/tests/test_complexity.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    22485 2024-01-17 09:02:23.000000 y0-0.2.8/tests/test_dsl.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    25955 2024-01-27 09:15:06.000000 y0-0.2.8/tests/test_graph.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     6726 2024-01-17 08:44:23.000000 y0-0.2.8/tests/test_is_identifiable.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.888919 y0-0.2.8/tests/test_mutate/
--rw-r--r--   0 cthoyt     (501) staff       (20)       88 2023-08-08 20:19:58.000000 y0-0.2.8/tests/test_mutate/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     8824 2024-01-17 09:02:21.000000 y0-0.2.8/tests/test_mutate/test_canonicalize.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2262 2023-09-08 17:44:46.000000 y0-0.2.8/tests/test_mutate/test_chain.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      710 2024-01-17 08:44:23.000000 y0-0.2.8/tests/test_mutate/test_contract.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1678 2023-09-08 17:44:46.000000 y0-0.2.8/tests/test_mutate/test_simplify.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-01-27 10:17:37.889528 y0-0.2.8/tests/test_parser/
--rw-r--r--   0 cthoyt     (501) staff       (20)       78 2023-08-08 20:19:58.000000 y0-0.2.8/tests/test_parser/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1474 2023-08-16 16:13:12.000000 y0-0.2.8/tests/test_parser/test_causaleffect.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      914 2023-09-08 17:44:46.000000 y0-0.2.8/tests/test_parser/test_internal.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1928 2023-08-16 16:13:12.000000 y0-0.2.8/tests/test_predicates.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.721069 y0-0.2.9/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1509 2023-08-16 16:13:12.000000 y0-0.2.9/LICENSE
+-rw-r--r--   0 cthoyt     (501) staff       (20)      359 2023-08-16 16:13:12.000000 y0-0.2.9/MANIFEST.in
+-rw-r--r--   0 cthoyt     (501) staff       (20)    11035 2024-03-22 08:21:17.720993 y0-0.2.9/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8916 2024-03-21 09:04:42.000000 y0-0.2.9/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.690033 y0-0.2.9/docs/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      605 2023-08-16 16:13:12.000000 y0-0.2.9/docs/Makefile
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.693338 y0-0.2.9/docs/source/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      191 2023-08-08 20:19:58.000000 y0-0.2.9/docs/source/cli.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      321 2024-03-18 07:00:36.000000 y0-0.2.9/docs/source/conditional_independence.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     6956 2024-03-22 08:21:17.000000 y0-0.2.9/docs/source/conf.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)       63 2023-08-08 20:19:58.000000 y0-0.2.9/docs/source/dsl.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       72 2023-08-08 20:19:58.000000 y0-0.2.9/docs/source/examples.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       51 2023-08-08 20:19:58.000000 y0-0.2.9/docs/source/graph.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      859 2024-03-18 07:00:36.000000 y0-0.2.9/docs/source/graph_mutation.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       82 2024-01-17 08:44:23.000000 y0-0.2.9/docs/source/identification.rst
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.693937 y0-0.2.9/docs/source/img/
+-rw-r--r--   0 cthoyt     (501) staff       (20)    87578 2023-08-16 16:13:12.000000 y0-0.2.9/docs/source/img/simulation_graph_algorithm.png
+-rw-r--r--   0 cthoyt     (501) staff       (20)    29002 2023-08-16 16:13:12.000000 y0-0.2.9/docs/source/img/simulation_graph_diagram.png
+-rw-r--r--   0 cthoyt     (501) staff       (20)      391 2024-03-22 07:58:55.000000 y0-0.2.9/docs/source/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      505 2023-08-08 20:19:58.000000 y0-0.2.9/docs/source/installation.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7328 2023-08-08 20:19:58.000000 y0-0.2.9/docs/source/logo.png
+-rw-r--r--   0 cthoyt     (501) staff       (20)      159 2024-01-17 08:44:23.000000 y0-0.2.9/docs/source/lvdags.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       58 2023-08-16 16:13:12.000000 y0-0.2.9/docs/source/mutation.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       54 2023-08-08 20:19:58.000000 y0-0.2.9/docs/source/parser.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       72 2024-01-17 08:44:23.000000 y0-0.2.9/docs/source/struct.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       73 2024-03-22 07:58:55.000000 y0-0.2.9/docs/source/transport.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      350 2023-08-16 16:13:12.000000 y0-0.2.9/pyproject.toml
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2532 2024-03-22 08:21:17.721452 y0-0.2.9/setup.cfg
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.688425 y0-0.2.9/src/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.688248 y0-0.2.9/src/kestrel/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.688284 y0-0.2.9/src/kestrel/curation/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.688324 y0-0.2.9/src/kestrel/curation/vaccines/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.694106 y0-0.2.9/src/kestrel/curation/vaccines/.ipynb_checkpoints/
+-rw-r--r--   0 cthoyt     (501) staff       (20)    37588 2023-09-18 11:22:16.000000 y0-0.2.9/src/kestrel/curation/vaccines/.ipynb_checkpoints/Platforms-checkpoint.ipynb
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.697775 y0-0.2.9/src/y0/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       64 2023-08-08 20:19:58.000000 y0-0.2.9/src/y0/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      319 2023-08-16 16:13:12.000000 y0-0.2.9/src/y0/__main__.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.703565 y0-0.2.9/src/y0/algorithm/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       71 2023-08-08 20:19:58.000000 y0-0.2.9/src/y0/algorithm/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    10168 2024-03-18 07:00:36.000000 y0-0.2.9/src/y0/algorithm/conditional_independencies.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.704159 y0-0.2.9/src/y0/algorithm/estimation/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3702 2024-01-17 08:44:23.000000 y0-0.2.9/src/y0/algorithm/estimation/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2707 2024-03-22 08:16:23.000000 y0-0.2.9/src/y0/algorithm/estimation/linear_scm.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4919 2024-03-18 07:00:36.000000 y0-0.2.9/src/y0/algorithm/falsification.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.706236 y0-0.2.9/src/y0/algorithm/identify/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3490 2024-03-18 07:00:36.000000 y0-0.2.9/src/y0/algorithm/identify/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7923 2023-09-06 15:45:51.000000 y0-0.2.9/src/y0/algorithm/identify/_extras.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1602 2024-01-17 08:44:23.000000 y0-0.2.9/src/y0/algorithm/identify/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    19765 2024-01-17 09:02:23.000000 y0-0.2.9/src/y0/algorithm/identify/cg.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2253 2024-03-18 07:00:36.000000 y0-0.2.9/src/y0/algorithm/identify/id_c.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    12056 2024-03-18 07:00:36.000000 y0-0.2.9/src/y0/algorithm/identify/id_star.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    12056 2024-03-18 07:00:36.000000 y0-0.2.9/src/y0/algorithm/identify/id_std.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8787 2024-03-18 07:00:36.000000 y0-0.2.9/src/y0/algorithm/identify/idc_star.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    11617 2024-03-18 07:00:36.000000 y0-0.2.9/src/y0/algorithm/identify/utils.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.706680 y0-0.2.9/src/y0/algorithm/separation/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1929 2024-03-18 07:00:36.000000 y0-0.2.9/src/y0/algorithm/separation/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    10601 2024-03-18 07:00:36.000000 y0-0.2.9/src/y0/algorithm/separation/sigma_separation.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7661 2024-03-18 07:00:36.000000 y0-0.2.9/src/y0/algorithm/simplify_latent.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    11681 2024-01-17 08:44:23.000000 y0-0.2.9/src/y0/algorithm/taheri_design.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    29277 2024-03-18 07:00:46.000000 y0-0.2.9/src/y0/algorithm/transport.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      775 2023-08-16 16:42:32.000000 y0-0.2.9/src/y0/causaleffect.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      830 2023-08-16 16:13:12.000000 y0-0.2.9/src/y0/cli.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2401 2023-09-08 17:44:46.000000 y0-0.2.9/src/y0/complexity.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    64288 2024-03-22 07:58:55.000000 y0-0.2.9/src/y0/dsl.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.708447 y0-0.2.9/src/y0/examples/
+-rw-r--r--   0 cthoyt     (501) staff       (20)    42564 2024-01-17 08:44:23.000000 y0-0.2.9/src/y0/examples/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1610 2023-09-06 15:45:51.000000 y0-0.2.9/src/y0/examples/backdoor.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1778 2023-09-06 15:45:51.000000 y0-0.2.9/src/y0/examples/frontdoor.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1808 2024-01-26 13:08:36.000000 y0-0.2.9/src/y0/examples/frontdoor_backdoor.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3612 2023-09-06 15:45:51.000000 y0-0.2.9/src/y0/examples/sars.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1858 2024-01-17 08:44:23.000000 y0-0.2.9/src/y0/examples/smoke_cancer.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1798 2024-03-22 07:59:06.000000 y0-0.2.9/src/y0/examples/utils.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    36668 2024-03-22 07:58:55.000000 y0-0.2.9/src/y0/graph.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.709565 y0-0.2.9/src/y0/mutate/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      334 2023-08-16 16:13:12.000000 y0-0.2.9/src/y0/mutate/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4309 2024-01-17 09:02:23.000000 y0-0.2.9/src/y0/mutate/canonicalize_expr.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4488 2024-01-17 08:44:23.000000 y0-0.2.9/src/y0/mutate/chain.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1773 2024-01-17 08:44:23.000000 y0-0.2.9/src/y0/mutate/contract.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1757 2024-01-17 08:44:23.000000 y0-0.2.9/src/y0/mutate/utils.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.710050 y0-0.2.9/src/y0/parser/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      185 2023-09-08 17:44:46.000000 y0-0.2.9/src/y0/parser/__init__.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.710657 y0-0.2.9/src/y0/parser/ce/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      108 2023-08-16 16:13:12.000000 y0-0.2.9/src/y0/parser/ce/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1976 2023-09-08 17:44:46.000000 y0-0.2.9/src/y0/parser/ce/grammar.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1919 2023-09-08 17:44:46.000000 y0-0.2.9/src/y0/parser/ce/utils.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1423 2024-01-17 08:44:23.000000 y0-0.2.9/src/y0/parser/internal.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1055 2023-08-16 16:13:12.000000 y0-0.2.9/src/y0/predicates.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1831 2023-08-16 16:42:32.000000 y0-0.2.9/src/y0/r_utils.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.711883 y0-0.2.9/src/y0/resources/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      226 2023-08-16 16:13:12.000000 y0-0.2.9/src/y0/resources/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)   242724 2023-08-16 16:13:12.000000 y0-0.2.9/src/y0/resources/asia.csv
+-rw-r--r--   0 cthoyt     (501) staff       (20)    72805 2023-08-16 16:13:12.000000 y0-0.2.9/src/y0/resources/viral_pathogenesis.json
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7450 2024-03-22 07:58:55.000000 y0-0.2.9/src/y0/simulation.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8935 2024-03-18 07:00:36.000000 y0-0.2.9/src/y0/struct.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.712099 y0-0.2.9/src/y0/util/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1503 2023-08-16 16:13:12.000000 y0-0.2.9/src/y0/util/combinatorics.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      984 2024-03-22 08:21:17.000000 y0-0.2.9/src/y0/version.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.720412 y0-0.2.9/src/y0.egg-info/
+-rw-r--r--   0 cthoyt     (501) staff       (20)    11035 2024-03-22 08:21:17.000000 y0-0.2.9/src/y0.egg-info/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3271 2024-03-22 08:21:17.000000 y0-0.2.9/src/y0.egg-info/SOURCES.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2024-03-22 08:21:17.000000 y0-0.2.9/src/y0.egg-info/dependency_links.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       35 2024-03-22 08:21:17.000000 y0-0.2.9/src/y0.egg-info/entry_points.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-08-09 17:14:42.000000 y0-0.2.9/src/y0.egg-info/not-zip-safe
+-rw-r--r--   0 cthoyt     (501) staff       (20)      222 2024-03-22 08:21:17.000000 y0-0.2.9/src/y0.egg-info/requires.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        3 2024-03-22 08:21:17.000000 y0-0.2.9/src/y0.egg-info/top_level.txt
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.714853 y0-0.2.9/tests/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       52 2023-08-08 20:19:58.000000 y0-0.2.9/tests/__init__.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.715060 y0-0.2.9/tests/data/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3419 2024-01-17 08:44:23.000000 y0-0.2.9/tests/data/generate.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.718160 y0-0.2.9/tests/test_algorithm/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       53 2023-08-08 20:19:58.000000 y0-0.2.9/tests/test_algorithm/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2082 2024-03-22 07:58:55.000000 y0-0.2.9/tests/test_algorithm/cases.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    33649 2024-01-17 09:02:23.000000 y0-0.2.9/tests/test_algorithm/test_cg.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    10896 2024-03-18 07:00:36.000000 y0-0.2.9/tests/test_algorithm/test_conditional_independencies.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3079 2024-01-26 13:40:51.000000 y0-0.2.9/tests/test_algorithm/test_falsification.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    12601 2024-01-17 08:44:23.000000 y0-0.2.9/tests/test_algorithm/test_id_alg.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    23264 2023-09-06 15:45:51.000000 y0-0.2.9/tests/test_algorithm/test_id_star.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    21609 2023-09-06 15:45:51.000000 y0-0.2.9/tests/test_algorithm/test_original_id_star.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4014 2024-03-18 07:00:36.000000 y0-0.2.9/tests/test_algorithm/test_sigma_separation.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    17840 2024-01-17 08:44:23.000000 y0-0.2.9/tests/test_algorithm/test_simplify_latent.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    36423 2024-01-17 08:44:23.000000 y0-0.2.9/tests/test_algorithm/test_transport.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2318 2023-08-29 10:54:36.000000 y0-0.2.9/tests/test_causaleffect.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2972 2023-08-16 16:13:12.000000 y0-0.2.9/tests/test_complexity.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    22485 2024-01-17 09:02:23.000000 y0-0.2.9/tests/test_dsl.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    25955 2024-03-18 07:00:36.000000 y0-0.2.9/tests/test_graph.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     6726 2024-01-17 08:44:23.000000 y0-0.2.9/tests/test_is_identifiable.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.719584 y0-0.2.9/tests/test_mutate/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       88 2023-08-08 20:19:58.000000 y0-0.2.9/tests/test_mutate/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8824 2024-01-17 09:02:21.000000 y0-0.2.9/tests/test_mutate/test_canonicalize.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2262 2023-09-08 17:44:46.000000 y0-0.2.9/tests/test_mutate/test_chain.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      710 2024-01-17 08:44:23.000000 y0-0.2.9/tests/test_mutate/test_contract.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1678 2023-09-08 17:44:46.000000 y0-0.2.9/tests/test_mutate/test_simplify.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-22 08:21:17.720184 y0-0.2.9/tests/test_parser/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       78 2023-08-08 20:19:58.000000 y0-0.2.9/tests/test_parser/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1474 2023-08-16 16:13:12.000000 y0-0.2.9/tests/test_parser/test_causaleffect.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      914 2023-09-08 17:44:46.000000 y0-0.2.9/tests/test_parser/test_internal.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1928 2023-08-16 16:13:12.000000 y0-0.2.9/tests/test_predicates.py
```

### Comparing `y0-0.2.8/LICENSE` & `y0-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/PKG-INFO` & `y0-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y0
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python code for causal modeling.
 Home-page: https://github.com/y0-causal-inference/y0
 Download-URL: https://github.com/y0-causal-inference/y0/releases
 Author: Jeremy Zucker
 Author-email: jeremy.zucker@pnnl.gov
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: y0 Version: 0.2.8 Summary: Python code for causal
+Metadata-Version: 2.1 Name: y0 Version: 0.2.9 Summary: Python code for causal
 modeling. Home-page: https://github.com/y0-causal-inference/y0 Download-URL:
 https://github.com/y0-causal-inference/y0/releases Author: Jeremy Zucker
 Author-email: jeremy.zucker@pnnl.gov Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com License: BSD-3-Clause Project-URL: Bug
 Tracker, https://github.com/y0-causal-inference/y0/issues Project-URL: Source
 Code, https://github.com/y0-causal-inference/y0 Keywords:
 cthoyt,cookiecutter,structural causal modeling Classifier: Development Status
```

### Comparing `y0-0.2.8/README.md` & `y0-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/docs/Makefile` & `y0-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/docs/source/conf.py` & `y0-0.2.9/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "y0"
 copyright = f"{date.today().year}, Jeremy Zucker and Charles Tapley Hoyt"
 author = "Jeremy Zucker and Charles Tapley Hoyt"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.2.8"
+release = "0.2.9"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
```

### Comparing `y0-0.2.8/docs/source/img/simulation_graph_algorithm.png` & `y0-0.2.9/docs/source/img/simulation_graph_algorithm.png`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/docs/source/img/simulation_graph_diagram.png` & `y0-0.2.9/docs/source/img/simulation_graph_diagram.png`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/docs/source/logo.png` & `y0-0.2.9/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/setup.cfg` & `y0-0.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = y0
-version = 0.2.8
+version = 0.2.9
 description = Python code for causal modeling.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/y0-causal-inference/y0
 download_url = https://github.com/y0-causal-inference/y0/releases
 project_urls = 
 	Bug Tracker = https://github.com/y0-causal-inference/y0/issues
```

### Comparing `y0-0.2.8/src/kestrel/curation/vaccines/.ipynb_checkpoints/Platforms-checkpoint.ipynb` & `y0-0.2.9/src/kestrel/curation/vaccines/.ipynb_checkpoints/Platforms-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/algorithm/conditional_independencies.py` & `y0-0.2.9/src/y0/algorithm/conditional_independencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 # -*- coding: utf-8 -*-
 
-"""An implementation to get conditional independencies of an ADMG from [pearl2009]_.
-
-.. [taheri2024] Eliater: a workflow and open source implementation for estimation of
-   outcomes of perturbations from observational measurements in biomolecular networks
-"""
+"""An implementation to get conditional independencies of an ADMG from [pearl2009]_."""
 
 from functools import partial
 from itertools import combinations, groupby
 from typing import Callable, Iterable, List, Optional, Sequence, Set, Tuple, Union
 
 import networkx as nx
 import pandas as pd
```

### Comparing `y0-0.2.8/src/y0/algorithm/estimation/__init__.py` & `y0-0.2.9/src/y0/algorithm/estimation/__init__.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/algorithm/falsification.py` & `y0-0.2.9/src/y0/algorithm/falsification.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,71 +43,78 @@
     graph: NxMixedGraph,
     df: pd.DataFrame,
     *,
     significance_level: Optional[float] = None,
     max_given: Optional[int] = None,
     verbose: bool = False,
     method: Optional[CITest] = None,
+    sep: Optional[str] = None,
 ) -> Falsifications:
     """Test conditional independencies implied by a graph.
 
     :param graph: An ADMG
     :param df: Data to check for consistency with a causal implications
     :param significance_level: Significance for p-value test
     :param max_given: The maximum set size in the power set of the vertices minus the d-separable pairs
     :param verbose: If true, use tqdm for status updates.
     :param method: Conditional independence from :mod:`pgmpy` to use. If none,
         defaults to :func:`pgmpy.estimators.CITests.cressie_read`.
+    :param sep: The separator between givens when outputting the dataframe
     :return: Falsifications report
     """
     judgements = get_conditional_independencies(graph, max_conditions=max_given, verbose=verbose)
     return get_falsifications(
         judgements=judgements,
         df=df,
         significance_level=significance_level,
         verbose=verbose,
         method=method,
+        sep=sep,
     )
 
 
 def get_falsifications(
     judgements: Union[NxMixedGraph, Iterable[DSeparationJudgement]],
     df: pd.DataFrame,
     *,
     significance_level: Optional[float] = None,
     verbose: bool = False,
     method: Optional[CITest] = None,
     correction: Optional[str] = None,
+    sep: Optional[str] = None,
 ) -> Falsifications:
     """Test conditional independencies implied by a list of D-separation judgements.
 
     :param judgements: A list of D-separation judgements to check.
     :param df: Data to check for consistency with a causal implications
     :param verbose: If true, use tqdm for status updates.
     :param method: Conditional independence from :mod:`pgmpy` to use. If none,
         defaults to :func:`pgmpy.estimators.CITests.cressie_read`.
     :param correction: Method used for multiple hypothesis test correction. Defaults to ``holm``.
         See :func:`statsmodels.stats.multitest.multipletests` for possible methods.
     :param significance_level: Significance for p-value test, applied after multiple hypothesis testing correction
+    :param sep: The separator between givens when outputting the dataframe
     :return: Falsifications report
     """
     if significance_level is None:
         significance_level = 0.05
     if correction is None:
         correction = "holm"
+    if sep is None:
+        sep = "|"
     # Make this loop explicit for clarity
     results = []
     method = _ensure_method(method, df)
     for judgement in tqdm(judgements, disable=not verbose, desc="Checking conditionals"):
         result = judgement.test(df, method=method, boolean=False)
         results.append(
             (
                 judgement.left.name,
                 judgement.right.name,
-                "|".join(c.name for c in judgement.conditions),
+                sep.join(c.name for c in judgement.conditions),
                 result.statistic,
                 result.p_value,
                 result.dof,
             )
         )
     evidence_df = pd.DataFrame(
         results,
```

### Comparing `y0-0.2.8/src/y0/algorithm/identify/__init__.py` & `y0-0.2.9/src/y0/algorithm/identify/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 IDC* [shpitser2012]_    :mod:`y0.algorithm.identifiy.idc_star`
 Cyclic ID [forre2019]_  `Issue #71 <https://github.com/y0-causal-inference/y0/issues/71>`_
 gID [correa2019]_       `Issue #72 <https://github.com/y0-causal-inference/y0/issues/72>`_
 gID* [correa2021]_      `Issue #121 <https://github.com/y0-causal-inference/y0/issues/121>`_
 Data ID [nabi2020]_     `Issue #73 <https://github.com/y0-causal-inference/y0/issues/73>`_
 ======================  ====================================================================
 
+This table partially draws from [tikka2021]_, which made a nice review of non-counterfactual
+identification methods.
+
 Transport
 ---------
 =============================================  ======================================
 Algorithm                                      Implementation
 =============================================  ======================================
 Surrogate Outcomes [tikka2018]_                :mod:`y0.algorithm.transport`
 Transportability [correa2020]_                 :mod:`y0.algorithm.transport`
@@ -39,14 +42,16 @@
 .. [forre2019] `Causal Calculus in the Presence of Cycles, Latent Confounders and Selection
     Bias <https://arxiv.org/abs/1901.00433v2>`_
 .. [nabi2020] `Full Law Identification In Graphical Models Of Missing Data: Completeness Results
     <https://arxiv.org/abs/2004.04872>`_
 .. [correa2019] `General Identifiability with Arbitrary Surrogate Experiments <https://causalai.net/r46.pdf>`_
 .. [correa2021] `Nested Counterfactual Identification from Arbitrary Surrogate Experiments
     <https://causalai.net/r79.pdf>`_
+.. [tikka2021] `Causal Effect Identification from Multiple Incomplete Data Sources:
+    A General Search-based Approach <https://arxiv.org/pdf/1902.01073.pdf>`_
 
 """
 
 from .api import identify_outcomes
 from .id_c import idc
 from .id_star import id_star
 from .id_std import identify
```

### Comparing `y0-0.2.8/src/y0/algorithm/identify/_extras.py` & `y0-0.2.9/src/y0/algorithm/identify/_extras.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/algorithm/identify/api.py` & `y0-0.2.9/src/y0/algorithm/identify/api.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/algorithm/identify/cg.py` & `y0-0.2.9/src/y0/algorithm/identify/cg.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/algorithm/identify/id_c.py` & `y0-0.2.9/src/y0/algorithm/identify/id_c.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/algorithm/identify/id_star.py` & `y0-0.2.9/src/y0/algorithm/identify/id_star.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/algorithm/identify/id_std.py` & `y0-0.2.9/src/y0/algorithm/identify/id_std.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/algorithm/identify/idc_star.py` & `y0-0.2.9/src/y0/algorithm/identify/idc_star.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/algorithm/identify/utils.py` & `y0-0.2.9/src/y0/algorithm/identify/utils.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/algorithm/separation/__init__.py` & `y0-0.2.9/src/y0/algorithm/separation/__init__.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/algorithm/separation/sigma_separation.py` & `y0-0.2.9/src/y0/algorithm/separation/sigma_separation.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/algorithm/simplify_latent.py` & `y0-0.2.9/src/y0/algorithm/simplify_latent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """Implement Robin Evans' simplification algorithms from [evans2012]_ and [evans2016]_.
 
-.. [evans2016] `Graphs for margins of Bayesian networks <https://arxiv.org/abs/1408.1809>`_
 .. [evans2012] `Constraints on marginalised DAGs
       <https://www.fields.utoronto.ca/programs/scientific/11-12/graphicmodels/Evans.pdf>`_
 """
 
 import itertools as itt
 import logging
 from typing import Iterable, Mapping, NamedTuple, Optional, Set, Tuple, Union
```

### Comparing `y0-0.2.8/src/y0/algorithm/taheri_design.py` & `y0-0.2.9/src/y0/algorithm/taheri_design.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/algorithm/transport.py` & `y0-0.2.9/src/y0/algorithm/transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,15 +417,15 @@
         for transportability_node in transportability_nodes
         if transportability_node in graph_without_interventions
         for outcome in target_outcomes
     )
 
 
 def trso_line9(query: TRSOQuery, district: set[Variable]) -> Expression:
-    """Return the probability in the case with exactly one districts_without_interventions and it is present in districts.
+    """Get the probability in the case with exactly one districts_without_interventions and it is present in districts.
 
     :param query: A TRSO query
     :param district: The C-component present in both districts_without_interventions and districts
     :returns: An Expression
     :raises RuntimeError: If the query's expression is zero. This should never happen
     """
     logger.debug(
```

### Comparing `y0-0.2.8/src/y0/causaleffect.py` & `y0-0.2.9/src/y0/causaleffect.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/cli.py` & `y0-0.2.9/src/y0/cli.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/complexity.py` & `y0-0.2.9/src/y0/complexity.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/dsl.py` & `y0-0.2.9/src/y0/dsl.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,28 +30,32 @@
 
 import functools
 import itertools as itt
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from operator import attrgetter
 from typing import (
+    TYPE_CHECKING,
     Callable,
     Dict,
     Iterable,
     List,
     Optional,
     Protocol,
     Sequence,
     Set,
     Tuple,
     TypeVar,
     Union,
     cast,
 )
 
+if TYPE_CHECKING:
+    import sympy
+
 __all__ = [
     "Element",
     "Variable",
     "Intervention",
     "CounterfactualVariable",
     "Distribution",
     "Event",
@@ -208,14 +212,20 @@
         """Return the base variable, with no other nonsense."""
         return Variable(self.name)
 
     def to_text(self) -> str:
         """Output this variable in the internal string format."""
         return self.name
 
+    def to_sympy(self) -> "sympy.Symbol":
+        """Get the object for sympy."""
+        import sympy
+
+        return sympy.Symbol(self.to_latex())
+
     def to_latex(self) -> str:
         """Output this variable in the LaTeX string format.
 
         :returns: The LaTeX representaton of this variable.
 
         >>> Variable('X').to_latex()
         'X'
@@ -1559,15 +1569,15 @@
 Q = QFactor
 
 AA = Variable("AA")
 A, B, C, D, E, F, G, M, R, S, T, U, W, X, Y, Z = map(Variable, "ABCDEFGMRSTUWXYZ")  # type: ignore
 U1, U2, U3, U4, U5, U6 = [Variable(f"U{i}") for i in range(1, 7)]
 V1, V2, V3, V4, V5, V6 = [Variable(f"V{i}") for i in range(1, 7)]
 W0, W1, W2, W3, W4, W5, W6 = [Variable(f"W{i}") for i in range(7)]
-M1, M2, M2, M3, M4, M5, M6 = [Variable(f"M{i}") for i in range(7)]
+M0, M1, M2, M3, M4, M5, M6 = [Variable(f"M{i}") for i in range(7)]
 X1, X2, X3, X4, X5, X6 = [Variable(f"X{i}") for i in range(1, 7)]
 Y1, Y2, Y3, Y4, Y5, Y6 = [Variable(f"Y{i}") for i in range(1, 7)]
 Z1, Z2, Z3, Z4, Z5, Z6 = [Variable(f"Z{i}") for i in range(1, 7)]
 π1, π2, π3, π4, π5, π6 = Pi1, Pi2, Pi3, Pi4, Pi5, Pi6 = [Variable(f"π{i}") for i in range(1, 7)]
 
 
 def _sort_interventions(interventions: Iterable[Intervention]) -> Tuple[Intervention, ...]:
```

### Comparing `y0-0.2.8/src/y0/examples/__init__.py` & `y0-0.2.9/src/y0/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/examples/backdoor.py` & `y0-0.2.9/src/y0/examples/backdoor.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/examples/frontdoor.py` & `y0-0.2.9/src/y0/examples/frontdoor.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/examples/frontdoor_backdoor.py` & `y0-0.2.9/src/y0/examples/frontdoor_backdoor.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/examples/sars.py` & `y0-0.2.9/src/y0/examples/sars.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/examples/smoke_cancer.py` & `y0-0.2.9/src/y0/examples/smoke_cancer.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/examples/utils.py` & `y0-0.2.9/src/y0/examples/utils.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/graph.py` & `y0-0.2.9/src/y0/graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,26 +16,28 @@
     Iterable,
     Mapping,
     Optional,
     Sequence,
     Set,
     Tuple,
     Union,
+    cast,
 )
 
 import networkx as nx
 from networkx.classes.reportviews import NodeView
 from networkx.utils import open_file
 
 from .dsl import CounterfactualVariable, Intervention, Variable, vmap_adj, vmap_pairs
 
 if TYPE_CHECKING:
     import ananke.graphs
     import pgmpy.inference.CausalInference
     import pgmpy.models
+    import sympy
 
 __all__ = [
     "NxMixedGraph",
     "CausalEffectGraph",
     "DEFULT_PREFIX",
     "DEFAULT_TAG",
     "set_latent",
@@ -170,14 +172,51 @@
 
     def to_pgmpy_causal_inference(self) -> "pgmpy.inference.CausalInference.CausalInference":
         """Get a pgmpy causal inference object."""
         from pgmpy.inference.CausalInference import CausalInference
 
         return CausalInference(self.to_pgmpy_bayesian_network())
 
+    def to_linear_scm_sympy(self) -> dict[Variable, "sympy.Expr"]:
+        """Generate a Sympy system of equations."""
+        import sympy
+
+        variable_to_equation = {}
+        for node in self.topological_sort():
+            terms = []
+
+            # Add parent edges
+            for parent in self.directed.predecessors(node):
+                beta = sympy_nested(r"\beta", parent, node)
+                terms.append(beta * parent.to_sympy())
+
+            # Add noise term
+            epsilon_symbol = sympy_nested(r"\epsilon", node)
+            terms.append(epsilon_symbol)
+
+            # get bidirected edges
+            for u, v in self.undirected.edges(node):
+                u, v = sorted([u, v])
+                gamma_symbol = sympy_nested(r"\gamma", u, v)
+                terms.append(gamma_symbol)
+
+            variable_to_equation[node] = cast(sympy.Expr, sum(terms))
+        return variable_to_equation
+
+    def to_linear_scm_latex(self) -> str:
+        """Generate a Sympy system of equations."""
+        import sympy
+
+        equations_dict = self.to_linear_scm_sympy()
+        latex_equations = [
+            rf"{variable.to_latex()} &= {sympy.latex(expression)} \\"
+            for variable, expression in equations_dict.items()
+        ]
+        return _LatexStr(r"\begin{align*}" + "\n ".join(latex_equations) + r"\end{align*}")
+
     @classmethod
     def from_admg(cls, admg) -> NxMixedGraph:
         """Create from an ananke ADMG."""
         return cls.from_str_edges(
             nodes=admg.vertices,
             directed=admg.di_edges,
             undirected=admg.bi_edges,
@@ -623,14 +662,19 @@
         for node in topological_sort_order:
             if node in node_set:
                 break
             pre.append(node)
         return pre
 
 
+class _LatexStr(str):
+    def _repr_latex_(self):
+        return self
+
+
 def _node_not_an_intervention(node: Variable, interventions: Set[Intervention]) -> bool:
     """Confirm that node is not an intervention."""
     if isinstance(node, (Intervention, CounterfactualVariable)):
         raise TypeError(
             "this shouldn't happen since the graph should not have interventions as nodes"
         )
     return (+node not in interventions) and (-node not in interventions)
@@ -948,7 +992,15 @@
 ) -> set[Variable]:
     return {
         node
         for source, target in itt.product(sources, targets)
         for causal_path in nx.all_simple_paths(graph, source, target)
         for node in causal_path
     }
+
+
+def sympy_nested(glyph: str, *variables: Variable) -> "sympy.Symbol":
+    """Create a sympy nested symbol."""
+    import sympy
+
+    inner_latex = ",".join(variable.to_latex() for variable in variables)
+    return sympy.Symbol(rf"{glyph}_{{{inner_latex}}}")
```

### Comparing `y0-0.2.8/src/y0/mutate/canonicalize_expr.py` & `y0-0.2.9/src/y0/mutate/canonicalize_expr.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/mutate/chain.py` & `y0-0.2.9/src/y0/mutate/chain.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/mutate/contract.py` & `y0-0.2.9/src/y0/mutate/contract.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/mutate/utils.py` & `y0-0.2.9/src/y0/mutate/utils.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/parser/ce/grammar.py` & `y0-0.2.9/src/y0/parser/ce/grammar.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/parser/ce/utils.py` & `y0-0.2.9/src/y0/parser/ce/utils.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/parser/internal.py` & `y0-0.2.9/src/y0/parser/internal.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/predicates.py` & `y0-0.2.9/src/y0/predicates.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/r_utils.py` & `y0-0.2.9/src/y0/r_utils.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/resources/asia.csv` & `y0-0.2.9/src/y0/resources/asia.csv`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/resources/viral_pathogenesis.json` & `y0-0.2.9/src/y0/resources/viral_pathogenesis.json`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/simulation.py` & `y0-0.2.9/src/y0/simulation.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,35 +63,39 @@
     regression: LinearRegression
     slope: float
     intercept: float
     r2: float
     d_separation: Optional[DSeparationJudgement]
 
 
+FitsDict = Dict[FrozenSet[Variable], FitTuple]
+
+
 def simulate(
     graph: NxMixedGraph,
     trials: int = 200,
     return_fits: bool = True,
+    progress: bool = False,
     tqdm_kwargs: Optional[Mapping[str, Any]] = None,
     **kwargs,
-) -> Union[pd.DataFrame, Tuple[pd.DataFrame, Mapping[FrozenSet[Variable], FitTuple]]]:
+) -> Union[pd.DataFrame, Tuple[pd.DataFrame, FitsDict]]:
     """Simulate a graph using a linear structural causal model."""
     judgements = get_conditional_independencies(graph)
     cis: Mapping[FrozenSet[Variable], DSeparationJudgement] = {
         frozenset((judgement.left, judgement.right)): judgement for judgement in judgements
     }
 
     _tqdm_kwargs = dict(desc="Simulation", unit="trial", unit_scale=True)
     if tqdm_kwargs:
         _tqdm_kwargs.update(tqdm_kwargs)
 
     linear_scm = LinearSCM(graph, **kwargs)
     results = {
         trial: {variable.name: values for variable, values in linear_scm.trial().items()}
-        for trial in trange(trials, **_tqdm_kwargs)
+        for trial in trange(trials, disable=not progress, **_tqdm_kwargs)
     }
     rv = pd.DataFrame(results).T
 
     # Get a prioritized ordering for edges actually in graph
     order = list(graph.directed.edges())
     _x = {frozenset(edge) for edge in order}
     order.extend(
@@ -99,15 +103,15 @@
         for left, right in itt.combinations(sorted(graph.nodes(), key=lambda n: n.name), 2)
         if frozenset((left, right)) not in _x
     )
 
     if not return_fits:
         return rv
 
-    fits: Dict[FrozenSet[Variable], FitTuple] = {}
+    fits: FitsDict = {}
     for parent, child in order:
         x, y = rv[parent.name].to_numpy().reshape(-1, 1), rv[child.name]
         regression = LinearRegression()
         regression.fit(x, y)
         r2 = regression.score(x, y)
         key = frozenset((parent, child))
         fits[key] = FitTuple(
@@ -120,14 +124,35 @@
 
     return rv, fits
 
 
 Generator = Callable[[], float]
 
 
+def get_fits_df(fits_dict: FitsDict) -> pd.DataFrame:
+    """Convert a fits dictionary into a pandas dataframe."""
+    rows = [
+        (
+            a.name,
+            b.name,
+            fits_tuple.slope,
+            fits_tuple.intercept,
+            fits_tuple.r2,
+            # t.edge,
+            False if fits_tuple.d_separation is None else fits_tuple.d_separation.separated,
+            None if fits_tuple.d_separation is None else fits_tuple.d_separation.conditions,
+        )
+        for (a, b), fits_tuple in fits_dict.items()
+    ]
+    df = pd.DataFrame(
+        rows, columns=["parent", "child", "slope", "intercept", "r2", "d_separated", "d_sep_cond"]
+    )
+    return df
+
+
 class LinearSCM:
     """A data structure for a simulation.
 
     Provides an implementation of the simulation presented in Figure 1 and Example 2.2 in
     `Graphical criteria for efficient total effect estimation via adjustment in causal
     linear models <https://arxiv.org/abs/1907.02435>`_
     """
```

### Comparing `y0-0.2.8/src/y0/struct.py` & `y0-0.2.9/src/y0/struct.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/util/combinatorics.py` & `y0-0.2.9/src/y0/util/combinatorics.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/src/y0/version.py` & `y0-0.2.9/src/y0/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.2.8"
+VERSION = "0.2.9"
 
 
 def get_git_hash() -> str:
     """Get the :mod:`y0` git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `y0-0.2.8/src/y0.egg-info/PKG-INFO` & `y0-0.2.9/src/y0.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y0
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python code for causal modeling.
 Home-page: https://github.com/y0-causal-inference/y0
 Download-URL: https://github.com/y0-causal-inference/y0/releases
 Author: Jeremy Zucker
 Author-email: jeremy.zucker@pnnl.gov
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: y0 Version: 0.2.8 Summary: Python code for causal
+Metadata-Version: 2.1 Name: y0 Version: 0.2.9 Summary: Python code for causal
 modeling. Home-page: https://github.com/y0-causal-inference/y0 Download-URL:
 https://github.com/y0-causal-inference/y0/releases Author: Jeremy Zucker
 Author-email: jeremy.zucker@pnnl.gov Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com License: BSD-3-Clause Project-URL: Bug
 Tracker, https://github.com/y0-causal-inference/y0/issues Project-URL: Source
 Code, https://github.com/y0-causal-inference/y0 Keywords:
 cthoyt,cookiecutter,structural causal modeling Classifier: Development Status
```

### Comparing `y0-0.2.8/src/y0.egg-info/SOURCES.txt` & `y0-0.2.9/src/y0.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/data/generate.py` & `y0-0.2.9/tests/data/generate.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_algorithm/cases.py` & `y0-0.2.9/tests/test_algorithm/cases.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_algorithm/test_cg.py` & `y0-0.2.9/tests/test_algorithm/test_cg.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_algorithm/test_conditional_independencies.py` & `y0-0.2.9/tests/test_algorithm/test_conditional_independencies.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_algorithm/test_falsification.py` & `y0-0.2.9/tests/test_algorithm/test_falsification.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_algorithm/test_id_alg.py` & `y0-0.2.9/tests/test_algorithm/test_id_alg.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_algorithm/test_id_star.py` & `y0-0.2.9/tests/test_algorithm/test_id_star.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_algorithm/test_original_id_star.py` & `y0-0.2.9/tests/test_algorithm/test_original_id_star.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_algorithm/test_sigma_separation.py` & `y0-0.2.9/tests/test_algorithm/test_sigma_separation.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_algorithm/test_simplify_latent.py` & `y0-0.2.9/tests/test_algorithm/test_simplify_latent.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_algorithm/test_transport.py` & `y0-0.2.9/tests/test_algorithm/test_transport.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_causaleffect.py` & `y0-0.2.9/tests/test_causaleffect.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_complexity.py` & `y0-0.2.9/tests/test_complexity.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_dsl.py` & `y0-0.2.9/tests/test_dsl.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_graph.py` & `y0-0.2.9/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_is_identifiable.py` & `y0-0.2.9/tests/test_is_identifiable.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_mutate/test_canonicalize.py` & `y0-0.2.9/tests/test_mutate/test_canonicalize.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_mutate/test_chain.py` & `y0-0.2.9/tests/test_mutate/test_chain.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_mutate/test_contract.py` & `y0-0.2.9/tests/test_mutate/test_contract.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_mutate/test_simplify.py` & `y0-0.2.9/tests/test_mutate/test_simplify.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_parser/test_causaleffect.py` & `y0-0.2.9/tests/test_parser/test_causaleffect.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_parser/test_internal.py` & `y0-0.2.9/tests/test_parser/test_internal.py`

 * *Files identical despite different names*

### Comparing `y0-0.2.8/tests/test_predicates.py` & `y0-0.2.9/tests/test_predicates.py`

 * *Files identical despite different names*


# Comparing `tmp/mentpy-0.1.0a8.tar.gz` & `tmp/mentpy-0.1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentpy-0.1.0a8.tar", last modified: Mon Jul 17 00:07:07 2023, max compression
+gzip compressed data, was "mentpy-0.1.0a9.tar", last modified: Mon Oct 23 17:09:52 2023, max compression
```

## Comparing `mentpy-0.1.0a8.tar` & `mentpy-0.1.0a9.tar`

### file list

```diff
@@ -1,71 +1,68 @@
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.416164 mentpy-0.1.0a8/
--rw-r--r--   0 luismantilla   (501) staff       (20)    35149 2023-03-17 11:11:29.000000 mentpy-0.1.0a8/LICENSE
--rw-r--r--   0 luismantilla   (501) staff       (20)     3336 2023-07-17 00:07:07.415284 mentpy-0.1.0a8/PKG-INFO
--rw-r--r--   0 luismantilla   (501) staff       (20)     3056 2023-05-08 04:08:41.000000 mentpy-0.1.0a8/README.md
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.405648 mentpy-0.1.0a8/mentpy/
--rw-r--r--   0 luismantilla   (501) staff       (20)      278 2023-05-23 00:36:24.000000 mentpy-0.1.0a8/mentpy/__init__.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.407677 mentpy-0.1.0a8/mentpy/calculator/
--rw-r--r--   0 luismantilla   (501) staff       (20)       68 2023-07-07 03:46:01.000000 mentpy-0.1.0a8/mentpy/calculator/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      137 2023-05-23 00:43:44.000000 mentpy-0.1.0a8/mentpy/calculator/borrows.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1128 2023-05-23 00:43:45.000000 mentpy-0.1.0a8/mentpy/calculator/linalg2.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      137 2023-07-07 16:03:15.000000 mentpy-0.1.0a8/mentpy/calculator/states.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.408422 mentpy-0.1.0a8/mentpy/gradients/
--rw-r--r--   0 luismantilla   (501) staff       (20)       20 2023-06-10 07:26:23.000000 mentpy-0.1.0a8/mentpy/gradients/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2002 2023-06-10 07:30:42.000000 mentpy-0.1.0a8/mentpy/gradients/_finite_difference.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1599 2023-06-10 07:39:36.000000 mentpy-0.1.0a8/mentpy/gradients/_parameter_shift.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1934 2023-06-10 07:39:36.000000 mentpy-0.1.0a8/mentpy/gradients/grad.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.409194 mentpy-0.1.0a8/mentpy/mbqc/
--rw-r--r--   0 luismantilla   (501) staff       (20)      343 2023-04-16 02:07:08.000000 mentpy-0.1.0a8/mentpy/mbqc/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    18653 2023-05-31 21:43:20.000000 mentpy-0.1.0a8/mentpy/mbqc/flow.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    29788 2023-07-07 16:03:16.000000 mentpy-0.1.0a8/mentpy/mbqc/mbqcircuit.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.409823 mentpy-0.1.0a8/mentpy/mbqc/states/
--rw-r--r--   0 luismantilla   (501) staff       (20)      149 2023-05-06 07:23:30.000000 mentpy-0.1.0a8/mentpy/mbqc/states/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      197 2023-05-06 07:23:09.000000 mentpy-0.1.0a8/mentpy/mbqc/states/aklt.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      229 2023-05-06 07:23:14.000000 mentpy-0.1.0a8/mentpy/mbqc/states/cluster.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2976 2023-04-16 05:41:03.000000 mentpy-0.1.0a8/mentpy/mbqc/states/graphstate.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     7716 2023-06-21 22:34:00.000000 mentpy-0.1.0a8/mentpy/mbqc/templates.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.410152 mentpy-0.1.0a8/mentpy/noise/
--rw-r--r--   0 luismantilla   (501) staff       (20)       34 2023-03-17 21:21:26.000000 mentpy-0.1.0a8/mentpy/noise/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      173 2023-03-17 21:21:26.000000 mentpy-0.1.0a8/mentpy/noise/base_noise.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.410962 mentpy-0.1.0a8/mentpy/operators/
--rw-r--r--   0 luismantilla   (501) staff       (20)      285 2023-05-10 00:16:14.000000 mentpy-0.1.0a8/mentpy/operators/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3693 2023-06-28 21:20:40.000000 mentpy-0.1.0a8/mentpy/operators/controlled_ment.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1599 2023-05-07 19:04:31.000000 mentpy-0.1.0a8/mentpy/operators/gates.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     8449 2023-06-28 21:20:41.000000 mentpy-0.1.0a8/mentpy/operators/ment.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     5931 2023-05-31 23:51:54.000000 mentpy-0.1.0a8/mentpy/operators/pauliop.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.411880 mentpy-0.1.0a8/mentpy/optimizers/
--rw-r--r--   0 luismantilla   (501) staff       (20)      245 2023-04-25 08:17:14.000000 mentpy-0.1.0a8/mentpy/optimizers/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3277 2023-06-21 22:51:32.000000 mentpy-0.1.0a8/mentpy/optimizers/adam.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      707 2023-06-21 22:49:12.000000 mentpy-0.1.0a8/mentpy/optimizers/base_optimizer.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      366 2023-06-10 07:32:18.000000 mentpy-0.1.0a8/mentpy/optimizers/bp_tools.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3024 2023-06-21 22:52:45.000000 mentpy-0.1.0a8/mentpy/optimizers/rcd.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2814 2023-06-21 23:18:49.000000 mentpy-0.1.0a8/mentpy/optimizers/sgd.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.413530 mentpy-0.1.0a8/mentpy/simulators/
--rw-r--r--   0 luismantilla   (501) staff       (20)      281 2023-04-16 02:18:15.000000 mentpy-0.1.0a8/mentpy/simulators/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2441 2023-05-07 19:04:31.000000 mentpy-0.1.0a8/mentpy/simulators/base_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1156 2023-04-18 08:22:14.000000 mentpy-0.1.0a8/mentpy/simulators/cirq_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    19570 2023-07-16 02:01:47.000000 mentpy-0.1.0a8/mentpy/simulators/np_simulator_dm.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    19392 2023-06-02 22:34:53.000000 mentpy-0.1.0a8/mentpy/simulators/np_simulator_sv.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2678 2023-05-18 06:35:37.000000 mentpy-0.1.0a8/mentpy/simulators/pattern_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     5677 2023-05-18 08:04:21.000000 mentpy-0.1.0a8/mentpy/simulators/pennylane_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1254 2023-04-25 08:57:09.000000 mentpy-0.1.0a8/mentpy/simulators/qiskit_simulators.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.414510 mentpy-0.1.0a8/mentpy/utils/
--rw-r--r--   0 luismantilla   (501) staff       (20)      140 2023-05-23 00:17:19.000000 mentpy-0.1.0a8/mentpy/utils/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     6673 2023-04-25 08:57:09.000000 mentpy-0.1.0a8/mentpy/utils/expressivity.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3183 2023-04-16 01:51:56.000000 mentpy-0.1.0a8/mentpy/utils/flow_space.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     4466 2023-04-16 01:44:39.000000 mentpy-0.1.0a8/mentpy/utils/generate_data.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    10395 2023-05-06 07:13:49.000000 mentpy-0.1.0a8/mentpy/utils/lc_equivalence.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     5403 2023-06-28 16:40:04.000000 mentpy-0.1.0a8/mentpy/utils/lie_algebra.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.406856 mentpy-0.1.0a8/mentpy.egg-info/
--rw-r--r--   0 luismantilla   (501) staff       (20)     3336 2023-07-17 00:07:07.000000 mentpy-0.1.0a8/mentpy.egg-info/PKG-INFO
--rw-r--r--   0 luismantilla   (501) staff       (20)     1588 2023-07-17 00:07:07.000000 mentpy-0.1.0a8/mentpy.egg-info/SOURCES.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)        1 2023-07-17 00:07:07.000000 mentpy-0.1.0a8/mentpy.egg-info/dependency_links.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)       49 2023-07-17 00:07:07.000000 mentpy-0.1.0a8/mentpy.egg-info/requires.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)        7 2023-07-17 00:07:07.000000 mentpy-0.1.0a8/mentpy.egg-info/top_level.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)       38 2023-07-17 00:07:07.416229 mentpy-0.1.0a8/setup.cfg
--rw-r--r--   0 luismantilla   (501) staff       (20)      553 2023-07-17 00:06:20.000000 mentpy-0.1.0a8/setup.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-07-17 00:07:07.415043 mentpy-0.1.0a8/tests/
--rw-r--r--   0 luismantilla   (501) staff       (20)       58 2023-04-16 01:51:49.000000 mentpy-0.1.0a8/tests/test_flow.py
--rw-r--r--   0 luismantilla   (501) staff       (20)       64 2023-04-16 01:52:08.000000 mentpy-0.1.0a8/tests/test_graph_state.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      579 2023-04-16 01:52:23.000000 mentpy-0.1.0a8/tests/test_mbqc_templates.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2110 2023-05-18 06:15:48.000000 mentpy-0.1.0a8/tests/test_simulators.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-10-23 17:09:52.466171 mentpy-0.1.0a9/
+-rw-r--r--   0 luismantilla   (501) staff       (20)    11357 2023-10-23 16:19:15.000000 mentpy-0.1.0a9/LICENSE
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3735 2023-10-23 17:09:52.465888 mentpy-0.1.0a9/PKG-INFO
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2775 2023-10-23 16:19:15.000000 mentpy-0.1.0a9/README.md
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-10-23 17:09:52.452522 mentpy-0.1.0a9/mentpy/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      428 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/__init__.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-10-23 17:09:52.454490 mentpy-0.1.0a9/mentpy/calculator/
+-rw-r--r--   0 luismantilla   (501) staff       (20)       71 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/calculator/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      137 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/calculator/borrows.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1335 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/calculator/linalg2.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     4087 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/calculator/state_ops.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-10-23 17:09:52.455253 mentpy-0.1.0a9/mentpy/gradients/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      171 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/gradients/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2224 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/gradients/_finite_difference.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1749 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/gradients/_parameter_shift.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2084 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/gradients/grad.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-10-23 17:09:52.456690 mentpy-0.1.0a9/mentpy/mbqc/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      363 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/mbqc/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    18759 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/mbqc/flow.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    22973 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/mbqc/mbqcircuit.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-10-23 17:09:52.457836 mentpy-0.1.0a9/mentpy/mbqc/states/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      299 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/mbqc/states/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      348 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/mbqc/states/aklt.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      380 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/mbqc/states/cluster.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3129 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/mbqc/states/graphstate.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     9073 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/mbqc/templates.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     7880 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/mbqc/view.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-10-23 17:09:52.458387 mentpy-0.1.0a9/mentpy/noise/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      184 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/noise/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      323 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/noise/base_noise.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-10-23 17:09:52.459652 mentpy-0.1.0a9/mentpy/operators/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      435 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/operators/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3882 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/operators/controlled_ment.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     4546 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/operators/gates.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     8641 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/operators/ment.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     6287 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/operators/pauliop.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-10-23 17:09:52.461211 mentpy-0.1.0a9/mentpy/optimizers/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      395 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/optimizers/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3474 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/optimizers/adam.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      895 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/optimizers/base_optimizer.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      565 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/optimizers/bp_tools.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3242 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/optimizers/rcd.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3010 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/optimizers/sgd.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-10-23 17:09:52.462884 mentpy-0.1.0a9/mentpy/simulators/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      368 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/simulators/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2619 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/simulators/base_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    15023 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/simulators/np_simulator_dm.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    14968 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/simulators/np_simulator_sv.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2707 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/simulators/pattern_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     5873 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/simulators/pennylane_simulator.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-10-23 17:09:52.464451 mentpy-0.1.0a9/mentpy/utils/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      310 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/utils/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     6895 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/utils/expressivity.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3375 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/utils/flow_space.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     4480 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/utils/generate_data.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    10395 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/utils/lc_equivalence.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     5624 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/mentpy/utils/lie_algebra.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-10-23 17:09:52.453422 mentpy-0.1.0a9/mentpy.egg-info/
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3735 2023-10-23 17:09:52.000000 mentpy-0.1.0a9/mentpy.egg-info/PKG-INFO
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1493 2023-10-23 17:09:52.000000 mentpy-0.1.0a9/mentpy.egg-info/SOURCES.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)        1 2023-10-23 17:09:52.000000 mentpy-0.1.0a9/mentpy.egg-info/dependency_links.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)      237 2023-10-23 17:09:52.000000 mentpy-0.1.0a9/mentpy.egg-info/requires.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)        7 2023-10-23 17:09:52.000000 mentpy-0.1.0a9/mentpy.egg-info/top_level.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)      874 2023-10-23 16:19:15.000000 mentpy-0.1.0a9/pyproject.toml
+-rw-r--r--   0 luismantilla   (501) staff       (20)       38 2023-10-23 17:09:52.466226 mentpy-0.1.0a9/setup.cfg
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-10-23 17:09:52.464907 mentpy-0.1.0a9/tests/
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1744 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/tests/test_calculator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2298 2023-10-20 19:46:02.000000 mentpy-0.1.0a9/tests/test_simulators.py
```

### Comparing `mentpy-0.1.0a8/mentpy/gradients/_finite_difference.py` & `mentpy-0.1.0a9/mentpy/gradients/_finite_difference.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
+"""Module to calculate gradients using the finite difference method."""
 import numpy as np
 
 
 def fd_gradient(f, x, h=1e-5, type="central"):
     if type not in ["central", "forward", "backward"]:
         raise UserWarning(
             f"Expected type to be 'central', 'forward', or 'backward' but {type} was given"
```

### Comparing `mentpy-0.1.0a8/mentpy/gradients/_parameter_shift.py` & `mentpy-0.1.0a9/mentpy/gradients/_parameter_shift.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
 """Module to calculate gradients using the parameter shift rule."""
 import numpy as np
 
 
 def psr_gradient(cost, x, shift=1.5):
     """Calculate the gradient of a cost function using the parameter shift rule.
```

### Comparing `mentpy-0.1.0a8/mentpy/gradients/grad.py` & `mentpy-0.1.0a9/mentpy/gradients/grad.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
 """Module that contains functions to calculate gradients of cost functions."""
 import numpy as np
 from ._finite_difference import fd_gradient, fd_hessian
 from ._parameter_shift import psr_gradient, psr_hessian
 
 __all__ = ["get_gradient", "get_hessian"]
```

### Comparing `mentpy-0.1.0a8/mentpy/mbqc/flow.py` & `mentpy-0.1.0a9/mentpy/mbqc/flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-# Author: Luis Mantilla
-# Github: BestQuark
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
 """This is the Flow module. It deals with the flow of a given graph state"""
 import math
 import numpy as np
 import networkx as nx
 
 from mentpy.mbqc import GraphState
 from typing import Any, List
```

### Comparing `mentpy-0.1.0a8/mentpy/mbqc/states/graphstate.py` & `mentpy-0.1.0a9/mentpy/mbqc/states/graphstate.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,12 @@
-# Author: Luis Mantilla
-# Github: BestQuark
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
+"""Graph state class and related functions."""
 import numpy as np
 from mentpy.operators import PauliOp
 import networkx as nx
 from typing import Optional, List
 
 __all__ = ["GraphState", "entanglement_entropy"]
```

### Comparing `mentpy-0.1.0a8/mentpy/mbqc/templates.py` & `mentpy-0.1.0a9/mentpy/mbqc/templates.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-# Author: Luis Mantilla
-# Github: BestQuark
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
 """
 This is the common_ansatz module. 
 It has several common ansatzes that can be used for MBQC algorithms
 """
 
 from typing import List
-from mentpy.operators import Ment
+from mentpy.operators import Ment, PauliOp
 from mentpy.mbqc.states.graphstate import GraphState
 from mentpy.mbqc.mbqcircuit import MBQCircuit, hstack, merge
 
 
 def linear_cluster(n, **kwargs) -> MBQCircuit:
     r"""Returns a linear cluster state of n qubits.
 
@@ -286,7 +288,47 @@
                 n2 = spt_ansatz.output_nodes[(i + 2) % n_qubits]
                 if m % 2 == 0:
                     spt_ansatz = merge(spt_ansatz, sym_block1, [(n1, 0), (n2, 7)])
                 else:
                     spt_ansatz = merge(spt_ansatz, sym_block2, [(n1, 0), (n2, 7)])
 
     return spt_ansatz
+
+
+def from_pauli(pauli_op: PauliOp):
+    """Returns a graph state that can implement :math:`U=e^{-i\theta P}`"""
+
+    if len(pauli_op) != 1:
+        raise ValueError(
+            f"Can only create the template for a single Pauli operator, but {len(pauli_op)} were given."
+        )
+
+    n_qubits = pauli_op.number_of_qubits
+    exp_ansatz = many_wires([3] * n_qubits).graph
+    exp_ansatz.add_nodes_from([3 * n_qubits, 3 * n_qubits + 1])
+    exp_ansatz.add_edge(3 * n_qubits, 3 * n_qubits + 1)
+
+    measurements = {3 * n_qubits + 1: Ment("XY")}
+
+    for q in range(n_qubits):
+        has_x, has_z = False, False
+        if pauli_op.matrix[0, q] == 1:
+            exp_ansatz.add_edge(3 * q + 1, 3 * n_qubits)
+            has_x = True
+
+        if pauli_op.matrix[0, q + n_qubits] == 1:
+            exp_ansatz.add_edge(3 * q, 3 * n_qubits)
+            has_z = True
+
+        if has_x and has_z:
+            measurements[3 * n_qubits] = Ment("Y")
+
+    input_nodes = [3 * q for q in range(n_qubits)]
+    output_nodes = [3 * q + 2 for q in range(n_qubits)]
+
+    return MBQCircuit(
+        exp_ansatz,
+        measurements=measurements,
+        default_measurement=Ment("X"),
+        input_nodes=input_nodes,
+        output_nodes=output_nodes,
+    )
```

### Comparing `mentpy-0.1.0a8/mentpy/operators/controlled_ment.py` & `mentpy-0.1.0a9/mentpy/operators/controlled_ment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
+"""Controlled measurement operator."""
 from typing import Optional, Union, Callable
 import numpy as np
 import warnings
 
 from .gates import PauliX, PauliY, PauliZ
 from .ment import Ment, MentOutcome
```

### Comparing `mentpy-0.1.0a8/mentpy/operators/ment.py` & `mentpy-0.1.0a9/mentpy/operators/ment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
+"""A module for measurement operators."""
 from typing import Optional, Union, Callable, Any
 import numpy as np
 import warnings
 
 from .gates import PauliX, PauliY, PauliZ
```

### Comparing `mentpy-0.1.0a8/mentpy/operators/pauliop.py` & `mentpy-0.1.0a9/mentpy/operators/pauliop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
+"""Module for representing Pauli operators."""
 import numpy as np
 from typing import Union, List
 import galois
 import copy
 
 __all__ = ["PauliOp"]
 
@@ -144,14 +149,19 @@
                 elif char == "Z":
                     mat[i, j + n_qubits] = 1
                 elif char == "Y":
                     mat[i, j] = 1
                     mat[i, j + n_qubits] = 1
         return GF(mat)
 
+    @property
+    def number_of_qubits(self):
+        """Returns the number of qubits in the Pauli operator."""
+        return int(self.matrix.shape[1] // 2)
+
     def commutator(self, other) -> "PauliOp":
         """Returns the commutator of two Pauli operators."""
         if not self.symplectic_prod(other):
             return 0
         new_matrix = GF(self.matrix) + GF(other.matrix)
         return PauliOp(new_matrix)
```

### Comparing `mentpy-0.1.0a8/mentpy/optimizers/adam.py` & `mentpy-0.1.0a9/mentpy/optimizers/adam.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
+"""This module contains the Adam optimizer."""
 import numpy as np
 from mentpy.gradients import get_gradient
 
 from mentpy.optimizers.base_optimizer import BaseOptimizer
 
 
 class AdamOptimizer(BaseOptimizer):
```

### Comparing `mentpy-0.1.0a8/mentpy/optimizers/base_optimizer.py` & `mentpy-0.1.0a9/mentpy/optimizers/base_optimizer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
+"""A base class for optimizers.""" ""
 import abc
 
 
 class BaseOptimizer(abc.ABC):
     """Base class for optimizers.
 
     Note
```

### Comparing `mentpy-0.1.0a8/mentpy/optimizers/rcd.py` & `mentpy-0.1.0a9/mentpy/optimizers/rcd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
+"""This module contains the random coordinate descent optimizer."""
 from mentpy.optimizers.base_optimizer import BaseOptimizer
 
 import numpy as np
 import random
 
 
 class RCDOptimizer(BaseOptimizer):
```

### Comparing `mentpy-0.1.0a8/mentpy/optimizers/sgd.py` & `mentpy-0.1.0a9/mentpy/optimizers/sgd.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
+"""This module contains the SGD optimizer."""
 from mentpy.optimizers.base_optimizer import BaseOptimizer
 from mentpy.gradients import get_gradient
 
 import numpy as np
 
 
 class SGDOptimizer(BaseOptimizer):
```

### Comparing `mentpy-0.1.0a8/mentpy/simulators/base_simulator.py` & `mentpy-0.1.0a9/mentpy/simulators/base_simulator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
+"""Base class for simulators.""" ""
 import abc
 import numpy as np
 from typing import Union, List, Tuple, Optional
 
 from mentpy.mbqc.mbqcircuit import MBQCircuit
 
 
@@ -76,20 +81,20 @@
         ----------
         angle: float
             The angle of measurement.
         """
         pass
 
     @abc.abstractmethod
-    def run(self, parameters: List[float], **kwargs) -> Tuple[List[int], np.ndarray]:
+    def run(self, angles: List[float], **kwargs) -> Tuple[List[int], np.ndarray]:
         """Measures the state of the system.
 
         Parameters
         ----------
-        parameters: List[float]
+        angles: List[float]
             The parameters of the MBQC circuit (if any).
         """
         pass
 
     @abc.abstractmethod
     def reset(self, input_state=None):
         """Resets the simulator to the initial state."""
```

### Comparing `mentpy-0.1.0a8/mentpy/simulators/np_simulator_dm.py` & `mentpy-0.1.0a9/mentpy/simulators/np_simulator_sv.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,78 @@
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
+"""A vector state simulator that uses numpy to simulate the quantum circuit."""
+
 from typing import Union, List, Tuple, Optional
 
 import numpy as np
 import math
 import networkx as nx
 
-from mentpy.operators import Ment, ControlledMent
+from mentpy.operators import Ment
 from mentpy.mbqc.mbqcircuit import MBQCircuit
 from mentpy.simulators.base_simulator import BaseSimulator
 
+from mentpy.operators import gates
+import mentpy.calculator as calc
+
+
+__all__ = ["NumpySimulatorSV"]
+
 # COMMON GATES
 H = np.array([[1, 1], [1, -1]]) / np.sqrt(2)
 S = np.array([[1, 0], [0, 1j]])
 Pi8 = np.array([[1, 0], [0, np.exp(1j * np.pi / 4)]])
 sx = np.array([[0, 1], [1, 0]])
 sz = np.array([[1, 0], [0, -1]])
 
 # COMMON QUANTUM STATES
 q_zero = np.array([1, 0])
 qubit_plus = H @ q_zero
 
 
-class NumpySimulatorDM(BaseSimulator):
-    """A density matrix simulator that uses numpy to simulate the quantum circuit."""
+class NumpySimulatorSV(BaseSimulator):
+    """A vector state simulator that uses numpy to simulate the quantum circuit."""
 
-    # TODO: CALCULATE OPTIMAL WINDOW SIZE AUTOMATICALLY
     def __init__(
         self, mbqcircuit: MBQCircuit, input_state: np.ndarray = None, **kwargs
     ) -> None:
         super().__init__(mbqcircuit, input_state)
 
         self.window_size = kwargs.pop("window_size", 1)
         self.schedule = kwargs.pop("schedule", None)
         self.force0 = kwargs.pop("force0", True)
+
         self.dev_mode = kwargs.pop("dev_mode", False)
         self.wires = kwargs.pop("wires", None)
 
         if not self.force0:
             raise NotImplementedError("Numpy simulator does not support force0=False.")
 
+        # Only support XY Measurements
+        for node in mbqcircuit.graph.nodes:
+            if mbqcircuit[node] is not None:
+                if mbqcircuit[node].plane not in ["X", "Y", "XY"]:
+                    raise ValueError(
+                        f"Node {node} has plane {mbqcircuit[node].plane}, but only XY plane is supported."
+                    )
+
         # TODO: FIND SCHEDULE IF NOT PROVIDED
         if self.schedule is not None:
             self.schedule_measure = [
-                i for i in self.schedule if i not in mbqcircuit.quantum_output_nodes
+                i for i in self.schedule if i not in mbqcircuit.output_nodes
             ]
         elif mbqcircuit.measurement_order is not None:
             # remove output nodes from the measurement order
             self.schedule_measure = [
                 i
                 for i in mbqcircuit.measurement_order
-                if i not in mbqcircuit.quantum_output_nodes
+                if i not in mbqcircuit.output_nodes
             ]
             self.schedule = mbqcircuit.measurement_order
             if self.window_size == 1 and mbqcircuit.flow is not None:
                 self.window_size = len(mbqcircuit.input_nodes) + 1
         else:
             raise ValueError(
                 "Schedule must be provided for numpy simulator as the MBQCircuit does not have a flow."
@@ -79,15 +99,15 @@
             )
 
         self.current_measurement = 0
 
         for i in range(self.window_size - n_qubits_input):
             self.input_state = np.kron(self.input_state, qubit_plus)
 
-        self.qstate = self.pure2density(self.input_state)
+        self.qstate = self.input_state
         # get subgraph of the first window_size nodes
         self.subgraph = self.mbqcircuit.graph.subgraph(
             self.schedule[: self.window_size]
         )
 
         self.initial_czs = np.eye(2**self.window_size)
 
@@ -97,20 +117,19 @@
         # apply cz gates to neighboring qubits
         for node in self.subgraph.nodes:
             for neighbour in self.subgraph.neighbors(node):
                 # avoid repeated application of cz gates
                 if node < neighbour:
                     indx = self.current_simulated_nodes().index(node)
                     indy = self.current_simulated_nodes().index(neighbour)
-                    cz = self.controlled_z(indx, indy, self.window_size)
+                    cz = gates.controlled_z(indx, indy, self.window_size)
                     # self.qstate = cz @ self.qstate @ np.conj(cz).T
                     self.initial_czs = cz @ self.initial_czs
 
-        self.qstate = self.initial_czs @ self.qstate @ np.conj(self.initial_czs).T
-        self.outcomes = {}
+        self.qstate = self.initial_czs @ self.qstate
 
     def current_simulated_nodes(self) -> List[int]:
         """Returns the nodes that are currently simulated."""
         if not self.dev_mode:
             return self.schedule[
                 self.current_measurement : self.current_measurement + self.window_size
             ]
@@ -138,15 +157,15 @@
         neighs = self.neighbors_in_wire(node)
         future_neighs = []
         for neigh in neighs:
             if neigh > node:
                 future_neighs.append(neigh)
         return future_neighs
 
-    def measure(self, angle: float, mode="sample") -> Tuple:
+    def measure(self, angle: float) -> Tuple:
         if self.current_measurement >= len(self.schedule_measure):
             raise ValueError("No more measurements to be done.")
 
         if not self.dev_mode:
             current_ment = self.mbqcircuit[
                 self.schedule_measure[self.current_measurement]
             ].copy()
@@ -163,24 +182,19 @@
                     cond = futnods[0] in self.current_simulated_nodes()
                 if cond:
                     current_ment = self.mbqcircuit[node].copy()
                     indx = self.current_simulated_nodes().index(node)
                     break
 
         self.qstate, outcome = self.measure_ment(
-            current_ment, angle, indx, force0=self.force0, mode=mode
+            current_ment, angle, indx, force0=self.force0
         )
-        # check if qstate has nan
-        if np.isnan(self.qstate).any():
-            raise ValueError(
-                "qstate has nan, you might want to increase the window size"
-            )
-        self.current_measurement += 1
 
-        self.qstate = self.partial_trace(self.qstate, [indx])
+        self.current_measurement += 1
+        self.qstate = calc.partial_trace(self.qstate, [indx])
 
         if self.dev_mode:
             # remove qubit at indx from current_simulated_nodes
             self._current_simulated_nodes = [
                 i for i in self._current_simulated_nodes if i != node
             ]
             if self.current_measurement + self.window_size <= len(
@@ -189,96 +203,102 @@
                 self._current_simulated_nodes.append(
                     self.schedule[self.current_measurement + self.window_size - 1]
                 )
 
         if self.current_measurement + self.window_size <= len(
             self.mbqcircuit.graph.nodes
         ):
-            self.qstate = np.kron(self.qstate, self.pure2density(qubit_plus))
+            self.qstate = np.kron(self.qstate, qubit_plus)
+
             new_qubit = self.current_simulated_nodes()[-1]
 
             # get neighbours of new qubit
             neighbours = nx.neighbors(self.mbqcircuit.graph, new_qubit)
 
             # do cz between new qubit and neighbours
             indx_new = self.current_simulated_nodes().index(new_qubit)
             for neighbour in neighbours:
                 if neighbour in self.current_simulated_nodes():
                     indxn = self.current_simulated_nodes().index(neighbour)
-                    cz = self.controlled_z(indxn, indx_new, self.window_size)
-                    self.qstate = cz @ self.qstate @ np.conj(cz.T)
+                    cz = gates.controlled_z(indxn, indx_new, self.window_size)
+                    self.qstate = cz @ self.qstate
 
         return self.qstate, outcome
 
     def run(
-        self, angles: List[float], mode="sample", input_state=None
+        self, angles: List[float], output_form="dm", **kwargs
     ) -> Tuple[List[int], np.ndarray]:
-        """Measures the quantum state in the given pattern."""
-        if input_state is not None:
-            self.reset(input_state=input_state)
+        """Measures the quantum state in the given pattern.
+
+        Args:
+            angles (List[float]): List of angles to be used for the measurements.
+            output_form (str): Output form of the quantum state. Can be 'dm' for density matrix or 'sv' for statevector.
+        """
+        if kwargs.get("input_state") is not None:
+            self.reset(input_state=kwargs.get("input_state"))
 
         if len(angles) != len(self.mbqcircuit.trainable_nodes):
             raise ValueError(
                 f"Number of angles ({len(angles)}) does not match number of trainable nodes ({len(self.mbqcircuit.trainable_nodes)})."
             )
 
         if not self.dev_mode:
             for i in self.schedule_measure:
                 if i in self.mbqcircuit.trainable_nodes:
                     angle = angles[self.mbqcircuit.trainable_nodes.index(i)]
                 else:
                     angle = self.mbqcircuit[i].angle
 
-                self.qstate, outcome = self.measure(angle, mode)
+                self.qstate, outcome = self.measure(angle)
                 self.outcomes[i] = outcome
 
         elif self.dev_mode:
             while self.current_measurement < len(self.schedule_measure):
                 for node in self.current_simulated_nodes():
                     cond = False
                     futnods = self.future_neighbors_in_wire(node)
                     if len(futnods) == 0:
                         cond = True
                     else:
                         cond = futnods[0] in self.current_simulated_nodes()
                     if cond:
-                        # current_ment = self.mbqcircuit[node].copy()
-                        # indx = self.current_simulated_nodes().index(node)
+                        current_ment = self.mbqcircuit[node].copy()
+                        indx = self.current_simulated_nodes().index(node)
                         break
 
                 if cond == False:
                     raise ValueError("WTF")
                 if node in self.mbqcircuit.trainable_nodes:
                     angle = angles[self.mbqcircuit.trainable_nodes.index(node)]
-                    if isinstance(self.mbqcircuit[node], ControlledMent):
-                        cond_angle = self.mbqcircuit[node].angle(self.outcomes) or angle
-                        angle = cond_angle
-                elif isinstance(self.mbqcircuit[node], Ment):
+                else:
                     angle = self.mbqcircuit[node].angle
 
-                self.qstate, outcome = self.measure(angle, mode)
+                self.qstate, outcome = self.measure(angle)
                 self.outcomes[node] = outcome
 
-        current_output_order = [
-            i for i in self.schedule if i not in self.schedule_measure
-        ]
+        # check if output nodes have a measurement, if so, measure them
+        for i in self.mbqcircuit.output_nodes:
+            if isinstance(self.mbqcircuit[i], Ment):
+                self.qstate, outcome = self.measure_ment(
+                    self.mbqcircuit[i], self.mbqcircuit[i].angle, i, force0=self.force0
+                )
+                self.outcomes[i] = outcome
+
+        current_output_order = self.current_simulated_nodes()
         if self.mbqcircuit.quantum_output_nodes != current_output_order:
             self.qstate = self.reorder_qubits(
-                self.qstate, current_output_order, self.mbqcircuit.quantum_output_nodes
+                self.qstate, current_output_order, self.mbqcircuit.output_nodes
             )
 
-        # # check if output nodes have a measurement, if so, measure them
-        # for i in self.mbqcircuit.output_nodes:
-        #     if isinstance(self.mbqcircuit[i], Ment):
-        #         self.qstate, outcome = self.measure_ment(
-        #             self.mbqcircuit[i], self.mbqcircuit[i].angle, i, force0=self.force0
-        #         )
-        #         self.outcomes[i] = outcome
-
-        return self.qstate
+        if output_form.lower() == "dm" or output_form.lower() == "densitymatrix":
+            return np.outer(self.qstate, np.conj(self.qstate).T)
+        elif output_form.lower() == "sv" or output_form.lower() == "statevector":
+            return self.qstate
+        else:
+            raise ValueError(f"Output form {output_form} is not supported.")
 
     def reset(self, input_state: np.ndarray = None):
         """Resets the simulator to the initial state."""
         self.current_measurement = 0
 
         if input_state is not None:
             input_state = self.reorder_qubits(
@@ -286,202 +306,61 @@
                 self.mbqcircuit.input_nodes,
                 self.schedule[: len(self.mbqcircuit.input_nodes)],
             )
             self.input_state = input_state
             for i in range(self.window_size - len(self.mbqcircuit.input_nodes)):
                 self.input_state = np.kron(self.input_state, qubit_plus)
 
-        self.qstate = self.pure2density(self.input_state)
+        self.qstate = self.input_state
+
+        self.qstate = self.initial_czs @ self.qstate
 
-        self.qstate = self.initial_czs @ self.qstate @ np.conj(self.initial_czs).T
         self.outcomes = {}
 
         if self.dev_mode:
             self._current_simulated_nodes = self.schedule[0 : self.window_size]
 
-    def arbitrary_qubit_gate(self, u, i, n):
-        """
-        Single qubit gate u acting on qubit i
-        n is the number of qubits
-        """
-        op = 1
-        for k in range(0, n):
-            if k == i:
-                op = np.kron(op, u)
-            else:
-                op = np.kron(op, np.eye(2))
-        return op
-
-    def swap_ij(self, i, j, n):
-        """
-        Swaps qubit i with qubit j
-        """
-        assert i < n and j < n
-        op1, op2, op3, op4 = np.ones(4)
-        for k in range(n):
-            if k == i or k == j:
-                op1 = np.kron(
-                    op1, np.kron(np.array([[1], [0]]).T, np.array([[1], [0]]))
-                )
-                op4 = np.kron(
-                    op4, np.kron(np.array([[0], [1]]).T, np.array([[0], [1]]))
-                )
-            else:
-                op1 = np.kron(op1, np.eye(2))
-                op4 = np.kron(op4, np.eye(2))
-
-            if k == i:
-                op2 = np.kron(
-                    op2, np.kron(np.array([[1], [0]]).T, np.array([[0], [1]]))
-                )
-                op3 = np.kron(
-                    op3, np.kron(np.array([[0], [1]]).T, np.array([[1], [0]]))
-                )
-            elif k == j:
-                op2 = np.kron(
-                    op2, np.kron(np.array([[0], [1]]).T, np.array([[1], [0]]))
-                )
-                op3 = np.kron(
-                    op3, np.kron(np.array([[1], [0]]).T, np.array([[0], [1]]))
-                )
-            else:
-                op2 = np.kron(op2, np.eye(2))
-                op3 = np.kron(op3, np.eye(2))
-        return op1 + op2 + op3 + op4
-
-    def partial_trace(self, rho, indices):
-        """
-        Partial trace of state rho over some indices
-        """
-        x, y = rho.shape
-        n = int(math.log(x, 2))
-        r = len(indices)
-        sigma = np.zeros((int(x / (2**r)), int(y / (2**r))))
-        for m in range(0, 2**r):
-            qubits = format(m, "0" + f"{r}" + "b")
-            ptrace = 1
-            for k in range(0, n):
-                if k in indices:
-                    idx = indices.index(k)
-                    if qubits[idx] == "0":
-                        ptrace = np.kron(ptrace, np.array([[1], [0]]))
-                    elif qubits[idx] == "1":
-                        ptrace = np.kron(ptrace, np.array([[0], [1]]))
-                else:
-                    ptrace = np.kron(ptrace, np.eye(2))
-            sigma = sigma + np.conjugate(ptrace.T) @ rho @ (ptrace)
-        return sigma
-
-    def measure_ment(self, ment: Ment, angle, i, force0=False, mode="sample"):
+    def measure_ment(self, ment: Ment, angle, i, force0=False):
         """
         Measures a ment
         """
+        if ment.plane not in ["X", "Y", "XY"]:
+            raise ValueError(
+                f"Plane {ment.plane} is not supported for state vector numpy simulator."
+            )
 
         op = ment.matrix(angle, self.outcomes)
         if op is None:
             raise ValueError(f"Ment has no matrix representation at qubit {i}")
 
         p0, p1 = ment.get_povm(angle, self.outcomes)
-        p0_extended = self.arbitrary_qubit_gate(
-            p0, i, self.current_number_simulated_nodes()
-        )
-        p1_extended = self.arbitrary_qubit_gate(
+        p1_extended = gates.arbitrary_qubit_gate(
             p1, i, self.current_number_simulated_nodes()
         )
+        p0_extended = gates.arbitrary_qubit_gate(
+            p0, i, self.current_number_simulated_nodes()
+        )
 
-        prob0 = np.real(np.trace(self.qstate @ p0_extended))
-        prob1 = np.real(np.trace(self.qstate @ p1_extended))
+        prob0 = np.dot(np.conj(self.qstate), p0_extended @ self.qstate)
+        prob1 = np.dot(np.conj(self.qstate), p1_extended @ self.qstate)
 
-        COND = (mode == "expectation" or mode == "exp") and ment.plane == "Z"
+        if not force0:
+            outcome = np.random.choice([0, 1], p=[prob0, prob1] / (prob0 + prob1))
+        else:
+            outcome = 0
 
-        if not force0 or ment.plane == "Z":
-            if COND:
-                outcome = prob1 / (prob0 + prob1)
-            else:
-                outcome = np.random.choice([0, 1], p=[prob0, prob1] / (prob0 + prob1))
+        if outcome == 0:
+            self.qstate = p0_extended @ self.qstate
+            self.qstate /= np.linalg.norm(self.qstate)
         else:
-            if prob0 < 1e-4:
-                outcome = 1  # important when measuring Z's -- should make pretty
-            else:
-                outcome = 0
-
-        if not COND:
-            if outcome == 0:
-                self.qstate = p0_extended @ self.qstate @ np.conj(p0_extended).T / prob0
-            else:
-                self.qstate = p1_extended @ self.qstate @ np.conj(p1_extended).T / prob1
+            self.qstate = p1_extended @ self.qstate
+            self.qstate /= np.linalg.norm(self.qstate)
 
         return self.qstate, outcome
 
-    def controlled_z(self, i, j, n):
-        """
-        Controlled z gate between qubits i and j.
-        n is the total number of qubits
-        """
-        assert i < n and j < n
-        op1, op2 = 1, 2
-        for k in range(0, n):
-            op1 = np.kron(op1, np.eye(2))
-            if k in [i, j]:
-                op2 = np.kron(
-                    op2,
-                    np.kron(np.conjugate(np.array([[0], [1]]).T), np.array([[0], [1]])),
-                )
-            else:
-                op2 = np.kron(op2, np.eye(2))
-        return op1 - op2
-
-    def cnot_ij(self, i, j, n):
-        """
-        CNOT gate with
-        j: target qubit
-        n: number of qubits
-        """
-        op1, op2, op3, op4 = np.ones(4)
-        for k in range(1, n + 1):
-            if k == i or k == j:
-                op1 = np.kron(
-                    op1, np.kron(np.array([[1], [0]]).T, np.array([[1], [0]]))
-                )
-            else:
-                op1 = np.kron(op1, np.eye(2))
-            if k == i:
-                op2 = np.kron(
-                    op2, np.kron(np.array([[1], [0]]).T, np.array([[1], [0]]))
-                )
-                op3 = np.kron(
-                    op3, np.kron(np.array([[0], [1]]).T, np.array([[0], [1]]))
-                )
-                op4 = np.kron(
-                    op4, np.kron(np.array([[0], [1]]).T, np.array([[0], [1]]))
-                )
-            elif k == j:
-                op2 = np.kron(
-                    op2, np.kron(np.array([[0], [1]]).T, np.array([[0], [1]]))
-                )
-                op3 = np.kron(
-                    op3, np.kron(np.array([[1], [0]]).T, np.array([[0], [1]]))
-                )
-                op4 = np.kron(
-                    op4, np.kron(np.array([[0], [1]]).T, np.array([[1], [0]]))
-                )
-            else:
-                op2 = np.kron(op2, np.eye(2))
-                op3 = np.kron(op3, np.eye(2))
-                op4 = np.kron(op4, np.eye(2))
-
-        return op1 + op2 + op3 + op4
-
-    def pure2density(self, psi):
-        """
-        Input: quantum state
-        Output: corresponding density matrix
-        """
-        return np.outer(psi, np.conj(psi).T)
-
     def find_swaps(self, source, target):
         assert set(source) == set(
             target
         ), f"Both lists must have the same elements, but source={source} and target={target}"
 
         swaps = []
         source = list(source)  # Make a copy to avoid modifying the original list
@@ -495,19 +374,11 @@
         return swaps
 
     def reorder_qubits(self, state, current_order, target_order):
         """
         Reorders the qubits in the given order.
         """
         new_state = state.copy()
-        type_state = "dm"
-        if len(new_state.shape) == 1:
-            type_state = "pure"
-
         swaps = self.find_swaps(current_order, target_order)
         for i, j in swaps:
-            swap_op = self.swap_ij(i, j, len(current_order))
-            if type_state == "pure":
-                new_state = swap_op @ new_state
-            else:
-                new_state = swap_op @ new_state @ np.conj(swap_op).T
+            new_state = gates.swap_ij(i, j, len(current_order)) @ new_state
         return new_state
```

### Comparing `mentpy-0.1.0a8/mentpy/simulators/np_simulator_sv.py` & `mentpy-0.1.0a9/mentpy/simulators/np_simulator_dm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,64 @@
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
+"""A density matrix simulator that uses numpy to simulate the quantum circuit."""
+
 from typing import Union, List, Tuple, Optional
 
 import numpy as np
 import math
 import networkx as nx
 
-from mentpy.operators import Ment
+from mentpy.operators import Ment, ControlledMent
 from mentpy.mbqc.mbqcircuit import MBQCircuit
 from mentpy.simulators.base_simulator import BaseSimulator
 
-# COMMON GATES
-H = np.array([[1, 1], [1, -1]]) / np.sqrt(2)
-S = np.array([[1, 0], [0, 1j]])
-Pi8 = np.array([[1, 0], [0, np.exp(1j * np.pi / 4)]])
-sx = np.array([[0, 1], [1, 0]])
-sz = np.array([[1, 0], [0, -1]])
+from mentpy.operators import gates
+
+import mentpy.calculator as calc
+
+__all__ = ["NumpySimulatorDM"]
+
 
 # COMMON QUANTUM STATES
 q_zero = np.array([1, 0])
-qubit_plus = H @ q_zero
+qubit_plus = gates.HGate @ q_zero
 
 
-class NumpySimulatorSV(BaseSimulator):
-    """A vector state simulator that uses numpy to simulate the quantum circuit."""
+class NumpySimulatorDM(BaseSimulator):
+    """A density matrix simulator that uses numpy to simulate the quantum circuit."""
 
+    # TODO: CALCULATE OPTIMAL WINDOW SIZE AUTOMATICALLY
     def __init__(
         self, mbqcircuit: MBQCircuit, input_state: np.ndarray = None, **kwargs
     ) -> None:
         super().__init__(mbqcircuit, input_state)
 
         self.window_size = kwargs.pop("window_size", 1)
         self.schedule = kwargs.pop("schedule", None)
         self.force0 = kwargs.pop("force0", True)
-
         self.dev_mode = kwargs.pop("dev_mode", False)
         self.wires = kwargs.pop("wires", None)
 
         if not self.force0:
             raise NotImplementedError("Numpy simulator does not support force0=False.")
 
-        # Only support XY Measurements
-        for node in mbqcircuit.graph.nodes:
-            if mbqcircuit[node] is not None:
-                if mbqcircuit[node].plane not in ["X", "Y", "XY"]:
-                    raise ValueError(
-                        f"Node {node} has plane {mbqcircuit[node].plane}, but only XY plane is supported."
-                    )
-
         # TODO: FIND SCHEDULE IF NOT PROVIDED
         if self.schedule is not None:
             self.schedule_measure = [
-                i for i in self.schedule if i not in mbqcircuit.output_nodes
+                i for i in self.schedule if i not in mbqcircuit.quantum_output_nodes
             ]
         elif mbqcircuit.measurement_order is not None:
             # remove output nodes from the measurement order
             self.schedule_measure = [
                 i
                 for i in mbqcircuit.measurement_order
-                if i not in mbqcircuit.output_nodes
+                if i not in mbqcircuit.quantum_output_nodes
             ]
             self.schedule = mbqcircuit.measurement_order
             if self.window_size == 1 and mbqcircuit.flow is not None:
                 self.window_size = len(mbqcircuit.input_nodes) + 1
         else:
             raise ValueError(
                 "Schedule must be provided for numpy simulator as the MBQCircuit does not have a flow."
@@ -87,15 +85,15 @@
             )
 
         self.current_measurement = 0
 
         for i in range(self.window_size - n_qubits_input):
             self.input_state = np.kron(self.input_state, qubit_plus)
 
-        self.qstate = self.input_state
+        self.qstate = calc.pure2density(self.input_state)
         # get subgraph of the first window_size nodes
         self.subgraph = self.mbqcircuit.graph.subgraph(
             self.schedule[: self.window_size]
         )
 
         self.initial_czs = np.eye(2**self.window_size)
 
@@ -105,19 +103,20 @@
         # apply cz gates to neighboring qubits
         for node in self.subgraph.nodes:
             for neighbour in self.subgraph.neighbors(node):
                 # avoid repeated application of cz gates
                 if node < neighbour:
                     indx = self.current_simulated_nodes().index(node)
                     indy = self.current_simulated_nodes().index(neighbour)
-                    cz = self.controlled_z(indx, indy, self.window_size)
+                    cz = gates.controlled_z(indx, indy, self.window_size)
                     # self.qstate = cz @ self.qstate @ np.conj(cz).T
                     self.initial_czs = cz @ self.initial_czs
 
-        self.qstate = self.initial_czs @ self.qstate
+        self.qstate = self.initial_czs @ self.qstate @ np.conj(self.initial_czs).T
+        self.outcomes = {}
 
     def current_simulated_nodes(self) -> List[int]:
         """Returns the nodes that are currently simulated."""
         if not self.dev_mode:
             return self.schedule[
                 self.current_measurement : self.current_measurement + self.window_size
             ]
@@ -145,15 +144,15 @@
         neighs = self.neighbors_in_wire(node)
         future_neighs = []
         for neigh in neighs:
             if neigh > node:
                 future_neighs.append(neigh)
         return future_neighs
 
-    def measure(self, angle: float) -> Tuple:
+    def measure(self, angle: float, mode="sample") -> Tuple:
         if self.current_measurement >= len(self.schedule_measure):
             raise ValueError("No more measurements to be done.")
 
         if not self.dev_mode:
             current_ment = self.mbqcircuit[
                 self.schedule_measure[self.current_measurement]
             ].copy()
@@ -170,19 +169,24 @@
                     cond = futnods[0] in self.current_simulated_nodes()
                 if cond:
                     current_ment = self.mbqcircuit[node].copy()
                     indx = self.current_simulated_nodes().index(node)
                     break
 
         self.qstate, outcome = self.measure_ment(
-            current_ment, angle, indx, force0=self.force0
+            current_ment, angle, indx, force0=self.force0, mode=mode
         )
-
+        # check if qstate has nan
+        if np.isnan(self.qstate).any():
+            raise ValueError(
+                "qstate has nan, you might want to increase the window size"
+            )
         self.current_measurement += 1
-        self.qstate = self.partial_trace_pure_state(self.qstate, [indx])
+
+        self.qstate = calc.partial_trace(self.qstate, [indx])
 
         if self.dev_mode:
             # remove qubit at indx from current_simulated_nodes
             self._current_simulated_nodes = [
                 i for i in self._current_simulated_nodes if i != node
             ]
             if self.current_measurement + self.window_size <= len(
@@ -191,102 +195,96 @@
                 self._current_simulated_nodes.append(
                     self.schedule[self.current_measurement + self.window_size - 1]
                 )
 
         if self.current_measurement + self.window_size <= len(
             self.mbqcircuit.graph.nodes
         ):
-            self.qstate = np.kron(self.qstate, qubit_plus)
-
+            self.qstate = np.kron(self.qstate, calc.pure2density(qubit_plus))
             new_qubit = self.current_simulated_nodes()[-1]
 
             # get neighbours of new qubit
             neighbours = nx.neighbors(self.mbqcircuit.graph, new_qubit)
 
             # do cz between new qubit and neighbours
             indx_new = self.current_simulated_nodes().index(new_qubit)
             for neighbour in neighbours:
                 if neighbour in self.current_simulated_nodes():
                     indxn = self.current_simulated_nodes().index(neighbour)
-                    cz = self.controlled_z(indxn, indx_new, self.window_size)
-                    self.qstate = cz @ self.qstate
+                    cz = gates.controlled_z(indxn, indx_new, self.window_size)
+                    self.qstate = cz @ self.qstate @ np.conj(cz.T)
 
         return self.qstate, outcome
 
     def run(
-        self, angles: List[float], output_form="dm", **kwargs
+        self, angles: List[float], mode="sample", input_state=None
     ) -> Tuple[List[int], np.ndarray]:
-        """Measures the quantum state in the given pattern.
-
-        Args:
-            angles (List[float]): List of angles to be used for the measurements.
-            output_form (str): Output form of the quantum state. Can be 'dm' for density matrix or 'sv' for statevector.
-        """
-        if kwargs.get("input_state") is not None:
-            self.reset(input_state=kwargs.get("input_state"))
+        """Measures the quantum state in the given pattern."""
+        if input_state is not None:
+            self.reset(input_state=input_state)
 
         if len(angles) != len(self.mbqcircuit.trainable_nodes):
             raise ValueError(
                 f"Number of angles ({len(angles)}) does not match number of trainable nodes ({len(self.mbqcircuit.trainable_nodes)})."
             )
 
         if not self.dev_mode:
             for i in self.schedule_measure:
                 if i in self.mbqcircuit.trainable_nodes:
                     angle = angles[self.mbqcircuit.trainable_nodes.index(i)]
                 else:
                     angle = self.mbqcircuit[i].angle
 
-                self.qstate, outcome = self.measure(angle)
+                self.qstate, outcome = self.measure(angle, mode)
                 self.outcomes[i] = outcome
 
         elif self.dev_mode:
             while self.current_measurement < len(self.schedule_measure):
                 for node in self.current_simulated_nodes():
                     cond = False
                     futnods = self.future_neighbors_in_wire(node)
                     if len(futnods) == 0:
                         cond = True
                     else:
                         cond = futnods[0] in self.current_simulated_nodes()
                     if cond:
-                        current_ment = self.mbqcircuit[node].copy()
-                        indx = self.current_simulated_nodes().index(node)
+                        # current_ment = self.mbqcircuit[node].copy()
+                        # indx = self.current_simulated_nodes().index(node)
                         break
 
                 if cond == False:
                     raise ValueError("WTF")
                 if node in self.mbqcircuit.trainable_nodes:
                     angle = angles[self.mbqcircuit.trainable_nodes.index(node)]
-                else:
+                    if isinstance(self.mbqcircuit[node], ControlledMent):
+                        cond_angle = self.mbqcircuit[node].angle(self.outcomes) or angle
+                        angle = cond_angle
+                elif isinstance(self.mbqcircuit[node], Ment):
                     angle = self.mbqcircuit[node].angle
 
-                self.qstate, outcome = self.measure(angle)
+                self.qstate, outcome = self.measure(angle, mode)
                 self.outcomes[node] = outcome
 
-        # check if output nodes have a measurement, if so, measure them
-        for i in self.mbqcircuit.output_nodes:
-            if isinstance(self.mbqcircuit[i], Ment):
-                self.qstate, outcome = self.measure_ment(
-                    self.mbqcircuit[i], self.mbqcircuit[i].angle, i, force0=self.force0
-                )
-                self.outcomes[i] = outcome
-
-        current_output_order = self.current_simulated_nodes()
+        current_output_order = [
+            i for i in self.schedule if i not in self.schedule_measure
+        ]
         if self.mbqcircuit.quantum_output_nodes != current_output_order:
             self.qstate = self.reorder_qubits(
-                self.qstate, current_output_order, self.mbqcircuit.output_nodes
+                self.qstate, current_output_order, self.mbqcircuit.quantum_output_nodes
             )
 
-        if output_form.lower() == "dm" or output_form.lower() == "densitymatrix":
-            return np.outer(self.qstate, np.conj(self.qstate).T)
-        elif output_form.lower() == "sv" or output_form.lower() == "statevector":
-            return self.qstate
-        else:
-            raise ValueError(f"Output form {output_form} is not supported.")
+        # # check if output nodes have a measurement, if so, measure them
+        # for i in self.mbqcircuit.output_nodes:
+        #     if isinstance(self.mbqcircuit[i], Ment):
+        #         self.qstate, outcome = self.measure_ment(
+        #             self.mbqcircuit[i], self.mbqcircuit[i].angle, i, force0=self.force0
+        #         )
+        #         self.outcomes[i] = outcome
+
+        return self.qstate
 
     def reset(self, input_state: np.ndarray = None):
         """Resets the simulator to the initial state."""
         self.current_measurement = 0
 
         if input_state is not None:
             input_state = self.reorder_qubits(
@@ -294,200 +292,62 @@
                 self.mbqcircuit.input_nodes,
                 self.schedule[: len(self.mbqcircuit.input_nodes)],
             )
             self.input_state = input_state
             for i in range(self.window_size - len(self.mbqcircuit.input_nodes)):
                 self.input_state = np.kron(self.input_state, qubit_plus)
 
-        self.qstate = self.input_state
-
-        self.qstate = self.initial_czs @ self.qstate
+        self.qstate = calc.pure2density(self.input_state)
 
+        self.qstate = self.initial_czs @ self.qstate @ np.conj(self.initial_czs).T
         self.outcomes = {}
 
         if self.dev_mode:
             self._current_simulated_nodes = self.schedule[0 : self.window_size]
 
-    def arbitrary_qubit_gate(self, u, i, n):
-        """
-        Single qubit gate u acting on qubit i
-        n is the number of qubits
-        """
-        op = 1
-        for k in range(0, n):
-            if k == i:
-                op = np.kron(op, u)
-            else:
-                op = np.kron(op, np.eye(2))
-        return op
-
-    def swap_ij(self, i, j, n):
-        """
-        Swaps qubit i with qubit j
-        """
-        assert i < n and j < n
-        op1, op2, op3, op4 = np.ones(4)
-        for k in range(n):
-            if k == i or k == j:
-                op1 = np.kron(
-                    op1, np.kron(np.array([[1], [0]]).T, np.array([[1], [0]]))
-                )
-                op4 = np.kron(
-                    op4, np.kron(np.array([[0], [1]]).T, np.array([[0], [1]]))
-                )
-            else:
-                op1 = np.kron(op1, np.eye(2))
-                op4 = np.kron(op4, np.eye(2))
-
-            if k == i:
-                op2 = np.kron(
-                    op2, np.kron(np.array([[1], [0]]).T, np.array([[0], [1]]))
-                )
-                op3 = np.kron(
-                    op3, np.kron(np.array([[0], [1]]).T, np.array([[1], [0]]))
-                )
-            elif k == j:
-                op2 = np.kron(
-                    op2, np.kron(np.array([[0], [1]]).T, np.array([[1], [0]]))
-                )
-                op3 = np.kron(
-                    op3, np.kron(np.array([[1], [0]]).T, np.array([[0], [1]]))
-                )
-            else:
-                op2 = np.kron(op2, np.eye(2))
-                op3 = np.kron(op3, np.eye(2))
-        return op1 + op2 + op3 + op4
-
-    def partial_trace_pure_state(self, psi, indices_to_trace):
-        num_qubits = int(np.log2(psi.shape[0]))
-
-        remaining_qubits = sorted(set(range(num_qubits)) - set(indices_to_trace))
-        num_remaining_qubits = len(remaining_qubits)
-
-        # Calculate the initial shape of the tensor product
-        initial_shape = [2] * num_qubits
-
-        # Reshape the state vector into a tensor
-        tensor = psi.reshape(initial_shape)
-
-        # Transpose the tensor to move the qubits to trace to the end
-        tensor = tensor.transpose(remaining_qubits + indices_to_trace)
-
-        # Calculate the final shape after tracing
-        final_shape = [2] * num_remaining_qubits
-
-        # Perform the partial trace by summing over the traced qubits
-        traced_tensor = tensor.reshape(final_shape + [-1]).sum(
-            axis=tuple(range(-len(indices_to_trace), 0))
-        )
-
-        # Reshape to a vector
-        traced_tensor = traced_tensor.reshape(-1)
-
-        # Normalize the result
-        traced_tensor /= np.linalg.norm(traced_tensor)
-
-        return traced_tensor
-
-    def measure_ment(self, ment: Ment, angle, i, force0=False):
+    def measure_ment(self, ment: Ment, angle, i, force0=False, mode="sample"):
         """
         Measures a ment
         """
-        if ment.plane not in ["X", "Y", "XY"]:
-            raise ValueError(
-                f"Plane {ment.plane} is not supported for state vector numpy simulator."
-            )
 
         op = ment.matrix(angle, self.outcomes)
         if op is None:
             raise ValueError(f"Ment has no matrix representation at qubit {i}")
 
         p0, p1 = ment.get_povm(angle, self.outcomes)
-        p1_extended = self.arbitrary_qubit_gate(
-            p1, i, self.current_number_simulated_nodes()
-        )
-        p0_extended = self.arbitrary_qubit_gate(
+        p0_extended = gates.arbitrary_qubit_gate(
             p0, i, self.current_number_simulated_nodes()
         )
+        p1_extended = gates.arbitrary_qubit_gate(
+            p1, i, self.current_number_simulated_nodes()
+        )
 
-        prob0 = np.dot(np.conj(self.qstate), p0_extended @ self.qstate)
-        prob1 = np.dot(np.conj(self.qstate), p1_extended @ self.qstate)
+        prob0 = np.real(np.trace(self.qstate @ p0_extended))
+        prob1 = np.real(np.trace(self.qstate @ p1_extended))
 
-        if not force0:
-            outcome = np.random.choice([0, 1], p=[prob0, prob1] / (prob0 + prob1))
-        else:
-            outcome = 0
+        COND = (mode == "expectation" or mode == "exp") and ment.plane == "Z"
 
-        if outcome == 0:
-            self.qstate = p0_extended @ self.qstate
-            self.qstate /= np.linalg.norm(self.qstate)
+        if not force0 or ment.plane == "Z":
+            if COND:
+                outcome = prob1 / (prob0 + prob1)
+            else:
+                outcome = np.random.choice([0, 1], p=[prob0, prob1] / (prob0 + prob1))
         else:
-            self.qstate = p1_extended @ self.qstate
-            self.qstate /= np.linalg.norm(self.qstate)
-
-        return self.qstate, outcome
-
-    def controlled_z(self, i, j, n):
-        """
-        Controlled z gate between qubits i and j.
-        n is the total number of qubits
-        """
-        assert i < n and j < n, f"{i} or {j} is larger than {n}"
-        op1, op2 = 1, 2
-        for k in range(0, n):
-            op1 = np.kron(op1, np.eye(2))
-            if k in [i, j]:
-                op2 = np.kron(
-                    op2,
-                    np.kron(np.conjugate(np.array([[0], [1]]).T), np.array([[0], [1]])),
-                )
+            if prob0 < 1e-4:
+                outcome = 1  # important when measuring Z's -- should make pretty
             else:
-                op2 = np.kron(op2, np.eye(2))
-        return op1 - op2
+                outcome = 0
 
-    def cnot_ij(self, i, j, n):
-        """
-        CNOT gate with
-        j: target qubit
-        n: number of qubits
-        """
-        op1, op2, op3, op4 = np.ones(4)
-        for k in range(1, n + 1):
-            if k == i or k == j:
-                op1 = np.kron(
-                    op1, np.kron(np.array([[1], [0]]).T, np.array([[1], [0]]))
-                )
+        if not COND:
+            if outcome == 0:
+                self.qstate = p0_extended @ self.qstate @ np.conj(p0_extended).T / prob0
             else:
-                op1 = np.kron(op1, np.eye(2))
-            if k == i:
-                op2 = np.kron(
-                    op2, np.kron(np.array([[1], [0]]).T, np.array([[1], [0]]))
-                )
-                op3 = np.kron(
-                    op3, np.kron(np.array([[0], [1]]).T, np.array([[0], [1]]))
-                )
-                op4 = np.kron(
-                    op4, np.kron(np.array([[0], [1]]).T, np.array([[0], [1]]))
-                )
-            elif k == j:
-                op2 = np.kron(
-                    op2, np.kron(np.array([[0], [1]]).T, np.array([[0], [1]]))
-                )
-                op3 = np.kron(
-                    op3, np.kron(np.array([[1], [0]]).T, np.array([[0], [1]]))
-                )
-                op4 = np.kron(
-                    op4, np.kron(np.array([[0], [1]]).T, np.array([[1], [0]]))
-                )
-            else:
-                op2 = np.kron(op2, np.eye(2))
-                op3 = np.kron(op3, np.eye(2))
-                op4 = np.kron(op4, np.eye(2))
+                self.qstate = p1_extended @ self.qstate @ np.conj(p1_extended).T / prob1
 
-        return op1 + op2 + op3 + op4
+        return self.qstate, outcome
 
     def find_swaps(self, source, target):
         assert set(source) == set(
             target
         ), f"Both lists must have the same elements, but source={source} and target={target}"
 
         swaps = []
@@ -502,11 +362,19 @@
         return swaps
 
     def reorder_qubits(self, state, current_order, target_order):
         """
         Reorders the qubits in the given order.
         """
         new_state = state.copy()
+        type_state = "dm"
+        if len(new_state.shape) == 1:
+            type_state = "pure"
+
         swaps = self.find_swaps(current_order, target_order)
         for i, j in swaps:
-            new_state = self.swap_ij(i, j, len(current_order)) @ new_state
+            swap_op = gates.swap_ij(i, j, len(current_order))
+            if type_state == "pure":
+                new_state = swap_op @ new_state
+            else:
+                new_state = swap_op @ new_state @ np.conj(swap_op).T
         return new_state
```

### Comparing `mentpy-0.1.0a8/mentpy/simulators/pattern_simulator.py` & `mentpy-0.1.0a9/mentpy/simulators/pattern_simulator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
+"""Simulator for measuring patterns of MBQC circuits."""
+
 from typing import Union, List, Tuple, Optional
 import numpy as np
 
 from mentpy.mbqc.mbqcircuit import MBQCircuit
 from mentpy.simulators.base_simulator import BaseSimulator
 from mentpy.simulators.pennylane_simulator import *
 from mentpy.simulators.np_simulator_dm import *
 from mentpy.simulators.np_simulator_sv import *
 
-# from mentpy.simulators.cirq_simulator import *
-# from mentpy.simulators.qiskit_simulator import *
-
 __all__ = ["PatternSimulator"]
 
 
 class PatternSimulator:
     """Simulator for measuring patterns of MBQC circuits.
 
     Parameters
@@ -38,16 +41,14 @@
         input_state: np.ndarray = None,
         backend="pennylane",
         *args,
         **kwargs,
     ) -> None:
         supported_backends = {
             "pennylane": PennylaneSimulator,
-            # "cirq": CirqSimulator,
-            # "qiskit": QiskitSimulator,
             "numpy-dm": NumpySimulatorDM,
             "numpy-sv": NumpySimulatorSV,
         }
 
         backend = backend.lower()
         if backend not in supported_backends:
             raise ValueError(
```

### Comparing `mentpy-0.1.0a8/mentpy/simulators/pennylane_simulator.py` & `mentpy-0.1.0a9/mentpy/simulators/pennylane_simulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
+"""PennyLane simulator for MBQC circuits."""
+
 from typing import Union, List, Tuple, Optional
 
 import numpy as np
 
 from mentpy.simulators.base_simulator import BaseSimulator
 from mentpy.mbqc.mbqcircuit import MBQCircuit
```

### Comparing `mentpy-0.1.0a8/mentpy/utils/expressivity.py` & `mentpy-0.1.0a9/mentpy/utils/expressivity.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
+"""A module to study the expressivity of a given MBQC circuit."""
 import numpy as np
-import cirq
 import networkx as nx
 
 from scipy.spatial import distance
 from scipy.special import kl_div, rel_entr
 
 import pennylane as qml
 
@@ -100,24 +104,24 @@
             random_pattern = (
                 2 * np.pi * np.random.rand(pattern_simulator.max_measure_number)
             )
             final_state = qmlcircuit(random_pattern, output="density")
             fid = qml.math.fidelity(np.kron(random_st.T, random_st), final_state)
             fidelities.append(fid)
 
-    elif backend == "cirq":
-        for random_st in random_input_states:
-            random_pattern = (
-                2 * np.pi * np.random.rand(pattern_simulator.max_measure_number)
-            )
-            pattern_simulator.reset(input_state=random_st)
-
-            _ = pattern_simulator.measure_pattern(random_pattern)
-            final_state = pattern_simulator.current_sim_state
-            fidelities.append(cirq.fidelity(random_st, final_state))
+    # elif backend == "cirq":
+    #     for random_st in random_input_states:
+    #         random_pattern = (
+    #             2 * np.pi * np.random.rand(pattern_simulator.max_measure_number)
+    #         )
+    #         pattern_simulator.reset(input_state=random_st)
+
+    #         _ = pattern_simulator.measure_pattern(random_pattern)
+    #         final_state = pattern_simulator.current_sim_state
+    #         fidelities.append(cirq.fidelity(random_st, final_state))
 
     else:
         print(f"Unsupported backend {backend}")
 
     return fidelities
```

### Comparing `mentpy-0.1.0a8/mentpy/utils/flow_space.py` & `mentpy-0.1.0a9/mentpy/utils/flow_space.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
+"""A module to study graphs with flow."""
 from mentpy.mbqc import MBQCircuit
 
 import networkx as nx
 import itertools
 
 
 class FlowSpace:
```

### Comparing `mentpy-0.1.0a8/mentpy/utils/generate_data.py` & `mentpy-0.1.0a9/mentpy/utils/generate_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,40 @@
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
+"""A module for generating random quantum data."""
 import numpy as np
 import scipy
-import cirq
+
+from functools import reduce
 
 from mentpy import MBQCircuit
+from mentpy.operators import gates
 
 
 def _generate_haar_random_state(n_qubits: int) -> np.ndarray:
     r"""Makes one Haar random state over n_qubits"""
 
-    zero_list = n_qubits * [cirq.KET_ZERO.state_vector()]
-    ket_zeros = cirq.kron(*zero_list)
-    haar_random_u = cirq.testing.random_special_unitary(dim=int(2**n_qubits))
+    zero_list = n_qubits * [np.array([1, 0])]
+    ket_zeros = reduce(np.kron, zero_list).reshape((1, 2**n_qubits))
+    haar_random_u = gates.random_su(n_qubits)
     return (haar_random_u @ ket_zeros.T).T[0]
 
 
 def generate_haar_random_states(n_qubits: int, n_samples: int = 1) -> np.ndarray:
     r"""Makes one Haar random state over n_qubits"""
 
     if n_samples == 1:
         return _generate_haar_random_state(n_qubits)
     else:
         return [_generate_haar_random_state(n_qubits) for _ in range(n_samples)]
 
 
-def random_special_unitary(n_qubits: int):
-    """Returns a random special unitary in ``n_qubits`` sampled from the Haar distribution."""
-    return cirq.testing.random_special_unitary(dim=int(2**n_qubits))
-
-
-def random_train_test_states_unitary(
+def generate_random_dataset(
     unitary: np.ndarray, n_samples: int, test_size: float = 0.3
 ) -> tuple:
     r"Return random training and test data (input, target) for a given unitary gate ``unitary``."
     n_qubits = int(np.log2(unitary.shape[0]))
     random_inputs = generate_haar_random_states(n_qubits, n_samples=n_samples)
     random_targets = [(unitary @ st.T).T for st in random_inputs]
     return train_test_split(random_inputs, random_targets, test_size=test_size)
@@ -68,15 +70,15 @@
 
 
 def randomUnitary_closetoid(dim, t, n):
     """Returns a random unitary matrix close to the identity matrix"""
     return brownian_circuit(dim, n, np.sqrt(1 / (n * dim)) * 2 * np.pi * t)
 
 
-def random_train_test_states_unitary_noise(
+def generate_random_dataset_noisy(
     unitary: np.ndarray,
     n_samples: int,
     noise_level: float = 0.0,
     noise_type="brownian",
     test_size: float = 0.3,
 ) -> tuple:
     r"""Return random training data (input, target) for a given unitary gate ``unitary`` with
```

### Comparing `mentpy-0.1.0a8/mentpy/utils/lc_equivalence.py` & `mentpy-0.1.0a9/mentpy/utils/lc_equivalence.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a8/mentpy/utils/lie_algebra.py` & `mentpy-0.1.0a9/mentpy/utils/lie_algebra.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
+"""A module for calculating the Lie algebra of a given MBQC circuit"""
 from itertools import combinations
 
 import numpy as np
 from mentpy import MBQCircuit, PauliOp
 import galois
 import copy
```

### Comparing `mentpy-0.1.0a8/mentpy.egg-info/SOURCES.txt` & `mentpy-0.1.0a9/mentpy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 LICENSE
 README.md
-setup.py
+pyproject.toml
 mentpy/__init__.py
 mentpy.egg-info/PKG-INFO
 mentpy.egg-info/SOURCES.txt
 mentpy.egg-info/dependency_links.txt
 mentpy.egg-info/requires.txt
 mentpy.egg-info/top_level.txt
 mentpy/calculator/__init__.py
 mentpy/calculator/borrows.py
 mentpy/calculator/linalg2.py
-mentpy/calculator/states.py
+mentpy/calculator/state_ops.py
 mentpy/gradients/__init__.py
 mentpy/gradients/_finite_difference.py
 mentpy/gradients/_parameter_shift.py
 mentpy/gradients/grad.py
 mentpy/mbqc/__init__.py
 mentpy/mbqc/flow.py
 mentpy/mbqc/mbqcircuit.py
 mentpy/mbqc/templates.py
+mentpy/mbqc/view.py
 mentpy/mbqc/states/__init__.py
 mentpy/mbqc/states/aklt.py
 mentpy/mbqc/states/cluster.py
 mentpy/mbqc/states/graphstate.py
 mentpy/noise/__init__.py
 mentpy/noise/base_noise.py
 mentpy/operators/__init__.py
@@ -34,23 +35,19 @@
 mentpy/optimizers/adam.py
 mentpy/optimizers/base_optimizer.py
 mentpy/optimizers/bp_tools.py
 mentpy/optimizers/rcd.py
 mentpy/optimizers/sgd.py
 mentpy/simulators/__init__.py
 mentpy/simulators/base_simulator.py
-mentpy/simulators/cirq_simulator.py
 mentpy/simulators/np_simulator_dm.py
 mentpy/simulators/np_simulator_sv.py
 mentpy/simulators/pattern_simulator.py
 mentpy/simulators/pennylane_simulator.py
-mentpy/simulators/qiskit_simulators.py
 mentpy/utils/__init__.py
 mentpy/utils/expressivity.py
 mentpy/utils/flow_space.py
 mentpy/utils/generate_data.py
 mentpy/utils/lc_equivalence.py
 mentpy/utils/lie_algebra.py
-tests/test_flow.py
-tests/test_graph_state.py
-tests/test_mbqc_templates.py
+tests/test_calculator.py
 tests/test_simulators.py
```

### Comparing `mentpy-0.1.0a8/tests/test_simulators.py` & `mentpy-0.1.0a9/tests/test_simulators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Copyright (C) [2023] Luis Mantilla
+#
+# This program is released under the GNU GPL v3.0 or later.
+# See <https://www.gnu.org/licenses/> for details.
+"""Tests for the simulator module."""
 import pytest
 import numpy as np
 import mentpy as mp
 
 all_backends = ["numpy-dm", "numpy-sv", "pennylane"]
```


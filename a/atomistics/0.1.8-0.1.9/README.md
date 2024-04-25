# Comparing `tmp/atomistics-0.1.8.tar.gz` & `tmp/atomistics-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomistics-0.1.8.tar", last modified: Mon Nov 27 14:30:51 2023, max compression
+gzip compressed data, was "atomistics-0.1.9.tar", last modified: Tue Nov 28 09:15:43 2023, max compression
```

## Comparing `atomistics-0.1.8.tar` & `atomistics-0.1.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:30:51.081577 atomistics-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2023-11-27 14:29:40.000000 atomistics-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-27 14:29:40.000000 atomistics-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14646 2023-11-27 14:30:51.081577 atomistics-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11330 2023-11-27 14:29:40.000000 atomistics-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:30:51.073577 atomistics-0.1.8/atomistics/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-11-27 14:30:51.081577 atomistics-0.1.8/atomistics/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:30:51.073577 atomistics-0.1.8/atomistics/calculators/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/calculators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/calculators/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/calculators/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:30:51.073577 atomistics-0.1.8/atomistics/calculators/lammps/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/calculators/lammps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/calculators/lammps/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10295 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/calculators/lammps/potential.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/calculators/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:30:51.073577 atomistics-0.1.8/atomistics/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/shared/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:30:51.073577 atomistics-0.1.8/atomistics/shared/thermo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/shared/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/shared/thermo/debye.py
--rw-r--r--   0 runner    (1001) docker     (127)    11893 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/shared/thermo/thermo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:30:51.073577 atomistics-0.1.8/atomistics/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:30:51.073577 atomistics-0.1.8/atomistics/workflows/elastic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/workflows/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/workflows/elastic/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/workflows/elastic/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:30:51.073577 atomistics-0.1.8/atomistics/workflows/evcurve/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/workflows/evcurve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13422 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/workflows/evcurve/fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/workflows/evcurve/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:30:51.073577 atomistics-0.1.8/atomistics/workflows/langevin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/workflows/langevin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/workflows/langevin/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:30:51.077577 atomistics-0.1.8/atomistics/workflows/phonons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/workflows/phonons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/workflows/phonons/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/workflows/phonons/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/workflows/phonons/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:30:51.077577 atomistics-0.1.8/atomistics/workflows/quasiharmonic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/workflows/quasiharmonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/workflows/quasiharmonic/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:30:51.077577 atomistics-0.1.8/atomistics/workflows/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/workflows/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/workflows/shared/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:30:51.077577 atomistics-0.1.8/atomistics/workflows/structure_optimization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/workflows/structure_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-11-27 14:29:40.000000 atomistics-0.1.8/atomistics/workflows/structure_optimization/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:30:51.073577 atomistics-0.1.8/atomistics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14646 2023-11-27 14:30:51.000000 atomistics-0.1.8/atomistics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2023-11-27 14:30:51.000000 atomistics-0.1.8/atomistics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 14:30:51.000000 atomistics-0.1.8/atomistics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-11-27 14:30:51.000000 atomistics-0.1.8/atomistics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-27 14:30:51.000000 atomistics-0.1.8/atomistics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2023-11-27 14:30:49.000000 atomistics-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 14:30:51.081577 atomistics-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-11-27 14:29:40.000000 atomistics-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:30:51.077577 atomistics-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      924 2023-11-27 14:29:40.000000 atomistics-0.1.8/tests/test_elastic_emt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2023-11-27 14:29:40.000000 atomistics-0.1.8/tests/test_elastic_gpaw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2023-11-27 14:29:40.000000 atomistics-0.1.8/tests/test_elastic_lammps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2023-11-27 14:29:40.000000 atomistics-0.1.8/tests/test_evcurve_abinit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2023-11-27 14:29:40.000000 atomistics-0.1.8/tests/test_evcurve_emt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2023-11-27 14:29:40.000000 atomistics-0.1.8/tests/test_evcurve_gpaw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2023-11-27 14:29:40.000000 atomistics-0.1.8/tests/test_evcurve_lammps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2023-11-27 14:29:40.000000 atomistics-0.1.8/tests/test_evcurve_qe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2023-11-27 14:29:40.000000 atomistics-0.1.8/tests/test_evcurve_siesta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-11-27 14:29:40.000000 atomistics-0.1.8/tests/test_lammps_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2023-11-27 14:29:40.000000 atomistics-0.1.8/tests/test_langevin_lammps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-11-27 14:29:40.000000 atomistics-0.1.8/tests/test_optimize_positions_emt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2023-11-27 14:29:40.000000 atomistics-0.1.8/tests/test_optimize_positions_lammps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2023-11-27 14:29:40.000000 atomistics-0.1.8/tests/test_phonons_emt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-11-27 14:29:40.000000 atomistics-0.1.8/tests/test_phonons_gpaw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2023-11-27 14:29:40.000000 atomistics-0.1.8/tests/test_phonons_lammps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-11-27 14:29:40.000000 atomistics-0.1.8/tests/test_quasiharmonic_emt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2023-11-27 14:29:40.000000 atomistics-0.1.8/tests/test_quasiharmonic_lammps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:15:43.082852 atomistics-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2023-11-28 09:14:28.000000 atomistics-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-28 09:14:28.000000 atomistics-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14646 2023-11-28 09:15:43.082852 atomistics-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11330 2023-11-28 09:14:28.000000 atomistics-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:15:43.070852 atomistics-0.1.9/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2023-11-28 09:15:43.082852 atomistics-0.1.9/atomistics/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:15:43.074852 atomistics-0.1.9/atomistics/calculators/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/calculators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/calculators/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/calculators/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:15:43.074852 atomistics-0.1.9/atomistics/calculators/lammps/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/calculators/lammps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5769 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/calculators/lammps/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10295 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/calculators/lammps/potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/calculators/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:15:43.074852 atomistics-0.1.9/atomistics/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/shared/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:15:43.074852 atomistics-0.1.9/atomistics/shared/thermo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/shared/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/shared/thermo/debye.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11893 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/shared/thermo/thermo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:15:43.074852 atomistics-0.1.9/atomistics/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:15:43.074852 atomistics-0.1.9/atomistics/workflows/elastic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/workflows/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/workflows/elastic/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/workflows/elastic/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:15:43.074852 atomistics-0.1.9/atomistics/workflows/evcurve/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/workflows/evcurve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13422 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/workflows/evcurve/fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/workflows/evcurve/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:15:43.074852 atomistics-0.1.9/atomistics/workflows/langevin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/workflows/langevin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/workflows/langevin/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:15:43.078852 atomistics-0.1.9/atomistics/workflows/phonons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/workflows/phonons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/workflows/phonons/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/workflows/phonons/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/workflows/phonons/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:15:43.078852 atomistics-0.1.9/atomistics/workflows/quasiharmonic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/workflows/quasiharmonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/workflows/quasiharmonic/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:15:43.078852 atomistics-0.1.9/atomistics/workflows/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/workflows/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/workflows/shared/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:15:43.078852 atomistics-0.1.9/atomistics/workflows/structure_optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/workflows/structure_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2023-11-28 09:14:28.000000 atomistics-0.1.9/atomistics/workflows/structure_optimization/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:15:43.074852 atomistics-0.1.9/atomistics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14646 2023-11-28 09:15:43.000000 atomistics-0.1.9/atomistics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2023-11-28 09:15:43.000000 atomistics-0.1.9/atomistics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 09:15:43.000000 atomistics-0.1.9/atomistics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2023-11-28 09:15:43.000000 atomistics-0.1.9/atomistics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-28 09:15:43.000000 atomistics-0.1.9/atomistics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2023-11-28 09:15:41.000000 atomistics-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-28 09:15:43.082852 atomistics-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2023-11-28 09:14:28.000000 atomistics-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:15:43.082852 atomistics-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2023-11-28 09:14:28.000000 atomistics-0.1.9/tests/test_elastic_emt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2023-11-28 09:14:28.000000 atomistics-0.1.9/tests/test_elastic_gpaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2023-11-28 09:14:28.000000 atomistics-0.1.9/tests/test_elastic_lammps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2023-11-28 09:14:28.000000 atomistics-0.1.9/tests/test_evcurve_abinit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2023-11-28 09:14:28.000000 atomistics-0.1.9/tests/test_evcurve_emt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2023-11-28 09:14:28.000000 atomistics-0.1.9/tests/test_evcurve_gpaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2023-11-28 09:14:28.000000 atomistics-0.1.9/tests/test_evcurve_lammps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2023-11-28 09:14:28.000000 atomistics-0.1.9/tests/test_evcurve_qe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2023-11-28 09:14:28.000000 atomistics-0.1.9/tests/test_evcurve_siesta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-11-28 09:14:28.000000 atomistics-0.1.9/tests/test_lammps_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2023-11-28 09:14:28.000000 atomistics-0.1.9/tests/test_langevin_lammps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-11-28 09:14:28.000000 atomistics-0.1.9/tests/test_optimize_positions_emt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2023-11-28 09:14:28.000000 atomistics-0.1.9/tests/test_optimize_positions_lammps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2023-11-28 09:14:28.000000 atomistics-0.1.9/tests/test_phonons_emt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-11-28 09:14:28.000000 atomistics-0.1.9/tests/test_phonons_gpaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2023-11-28 09:14:28.000000 atomistics-0.1.9/tests/test_phonons_lammps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-11-28 09:14:28.000000 atomistics-0.1.9/tests/test_quasiharmonic_emt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2023-11-28 09:14:28.000000 atomistics-0.1.9/tests/test_quasiharmonic_lammps.py
```

### Comparing `atomistics-0.1.8/LICENSE` & `atomistics-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/PKG-INFO` & `atomistics-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomistics
-Version: 0.1.8
+Version: 0.1.9
 Summary: Interfaces for atomistic simulation codes and workflows
 Author-email: Jan Janssen <janssen@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, pyiron
         All rights reserved.
         
@@ -52,19 +52,19 @@
 Requires-Dist: ase==3.22.1
 Requires-Dist: numpy<=1.26.2,>=1.23.5
 Requires-Dist: scipy<=1.11.4,>=1.11.1
 Requires-Dist: spglib<=2.1.0,>=2.0.2
 Provides-Extra: phonopy
 Requires-Dist: phonopy==2.20.0; extra == "phonopy"
 Requires-Dist: seekpath<=2.1.0,>=1.9.0; extra == "phonopy"
-Requires-Dist: structuretoolkit<=0.0.12,>=0.0.10; extra == "phonopy"
+Requires-Dist: structuretoolkit<=0.0.15,>=0.0.10; extra == "phonopy"
 Provides-Extra: gpaw
 Requires-Dist: gpaw<=23.9.1,>=20.1.0; extra == "gpaw"
 Provides-Extra: lammps
-Requires-Dist: pylammpsmpi<=0.2.6,>=0.2.1; extra == "lammps"
+Requires-Dist: pylammpsmpi<=0.2.9,>=0.2.1; extra == "lammps"
 Requires-Dist: jinja2<=3.1.2,>=2.11.3; extra == "lammps"
 Requires-Dist: pandas<=2.1.3,>=1.5.3; extra == "lammps"
 
 # atomistics - Interfaces for atomistic simulation codes and workflows
 [![Unittest](https://github.com/pyiron/atomistics/actions/workflows/unittests.yml/badge.svg)](https://github.com/pyiron/atomistics/actions/workflows/unittests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/pyiron/atomistics/badge.svg?branch=main)](https://coveralls.io/github/pyiron/atomistics?branch=main)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pyiron/atomistics/HEAD)
```

### Comparing `atomistics-0.1.8/README.md` & `atomistics-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/atomistics/calculators/ase.py` & `atomistics-0.1.9/atomistics/calculators/ase.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/atomistics/calculators/interface.py` & `atomistics-0.1.9/atomistics/calculators/interface.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/atomistics/calculators/lammps/calculator.py` & `atomistics-0.1.9/atomistics/calculators/lammps/calculator.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/atomistics/calculators/lammps/potential.py` & `atomistics-0.1.9/atomistics/calculators/lammps/potential.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/atomistics/calculators/wrapper.py` & `atomistics-0.1.9/atomistics/calculators/wrapper.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/atomistics/shared/thermo/debye.py` & `atomistics-0.1.9/atomistics/shared/thermo/debye.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/atomistics/shared/thermo/thermo.py` & `atomistics-0.1.9/atomistics/shared/thermo/thermo.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/atomistics/workflows/__init__.py` & `atomistics-0.1.9/atomistics/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/atomistics/workflows/elastic/symmetry.py` & `atomistics-0.1.9/atomistics/workflows/elastic/symmetry.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/atomistics/workflows/elastic/workflow.py` & `atomistics-0.1.9/atomistics/workflows/elastic/workflow.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/atomistics/workflows/evcurve/fit.py` & `atomistics-0.1.9/atomistics/workflows/evcurve/fit.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/atomistics/workflows/evcurve/workflow.py` & `atomistics-0.1.9/atomistics/workflows/evcurve/workflow.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/atomistics/workflows/langevin/workflow.py` & `atomistics-0.1.9/atomistics/workflows/langevin/workflow.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/atomistics/workflows/phonons/helper.py` & `atomistics-0.1.9/atomistics/workflows/phonons/helper.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/atomistics/workflows/phonons/workflow.py` & `atomistics-0.1.9/atomistics/workflows/phonons/workflow.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/atomistics/workflows/quasiharmonic/workflow.py` & `atomistics-0.1.9/atomistics/workflows/quasiharmonic/workflow.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/atomistics.egg-info/PKG-INFO` & `atomistics-0.1.9/atomistics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomistics
-Version: 0.1.8
+Version: 0.1.9
 Summary: Interfaces for atomistic simulation codes and workflows
 Author-email: Jan Janssen <janssen@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, pyiron
         All rights reserved.
         
@@ -52,19 +52,19 @@
 Requires-Dist: ase==3.22.1
 Requires-Dist: numpy<=1.26.2,>=1.23.5
 Requires-Dist: scipy<=1.11.4,>=1.11.1
 Requires-Dist: spglib<=2.1.0,>=2.0.2
 Provides-Extra: phonopy
 Requires-Dist: phonopy==2.20.0; extra == "phonopy"
 Requires-Dist: seekpath<=2.1.0,>=1.9.0; extra == "phonopy"
-Requires-Dist: structuretoolkit<=0.0.12,>=0.0.10; extra == "phonopy"
+Requires-Dist: structuretoolkit<=0.0.15,>=0.0.10; extra == "phonopy"
 Provides-Extra: gpaw
 Requires-Dist: gpaw<=23.9.1,>=20.1.0; extra == "gpaw"
 Provides-Extra: lammps
-Requires-Dist: pylammpsmpi<=0.2.6,>=0.2.1; extra == "lammps"
+Requires-Dist: pylammpsmpi<=0.2.9,>=0.2.1; extra == "lammps"
 Requires-Dist: jinja2<=3.1.2,>=2.11.3; extra == "lammps"
 Requires-Dist: pandas<=2.1.3,>=1.5.3; extra == "lammps"
 
 # atomistics - Interfaces for atomistic simulation codes and workflows
 [![Unittest](https://github.com/pyiron/atomistics/actions/workflows/unittests.yml/badge.svg)](https://github.com/pyiron/atomistics/actions/workflows/unittests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/pyiron/atomistics/badge.svg?branch=main)](https://coveralls.io/github/pyiron/atomistics?branch=main)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pyiron/atomistics/HEAD)
```

### Comparing `atomistics-0.1.8/atomistics.egg-info/SOURCES.txt` & `atomistics-0.1.9/atomistics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/pyproject.toml` & `atomistics-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -37,21 +37,21 @@
 Documentation = "https://atomistics.readthedocs.io"
 Repository = "https://github.com/pyiron/atomistics"
 
 [project.optional-dependencies]
 phonopy = [
     "phonopy==2.20.0",
     "seekpath>=1.9.0,<=2.1.0",
-    "structuretoolkit>=0.0.10,<=0.0.12",
+    "structuretoolkit>=0.0.10,<=0.0.15",
 ]
 gpaw = [
     "gpaw>=20.1.0,<=23.9.1",
 ]
 lammps = [
-    "pylammpsmpi>=0.2.1,<=0.2.6",
+    "pylammpsmpi>=0.2.1,<=0.2.9",
     "jinja2>=2.11.3,<=3.1.2",
     "pandas>=1.5.3,<=2.1.3",
 ]
 
 [tool.setuptools.packages.find]
 include = ["atomistics*"]
```

### Comparing `atomistics-0.1.8/tests/test_elastic_emt.py` & `atomistics-0.1.9/tests/test_elastic_emt.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/tests/test_elastic_gpaw.py` & `atomistics-0.1.9/tests/test_elastic_gpaw.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/tests/test_elastic_lammps.py` & `atomistics-0.1.9/tests/test_elastic_lammps.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/tests/test_evcurve_abinit.py` & `atomistics-0.1.9/tests/test_evcurve_abinit.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/tests/test_evcurve_emt.py` & `atomistics-0.1.9/tests/test_evcurve_emt.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/tests/test_evcurve_gpaw.py` & `atomistics-0.1.9/tests/test_evcurve_gpaw.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/tests/test_evcurve_lammps.py` & `atomistics-0.1.9/tests/test_evcurve_lammps.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/tests/test_evcurve_qe.py` & `atomistics-0.1.9/tests/test_evcurve_qe.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/tests/test_evcurve_siesta.py` & `atomistics-0.1.9/tests/test_evcurve_siesta.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/tests/test_lammps_calculator.py` & `atomistics-0.1.9/tests/test_lammps_calculator.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/tests/test_langevin_lammps.py` & `atomistics-0.1.9/tests/test_langevin_lammps.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/tests/test_optimize_positions_emt.py` & `atomistics-0.1.9/tests/test_optimize_positions_emt.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/tests/test_optimize_positions_lammps.py` & `atomistics-0.1.9/tests/test_optimize_positions_lammps.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/tests/test_phonons_emt.py` & `atomistics-0.1.9/tests/test_phonons_emt.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/tests/test_phonons_gpaw.py` & `atomistics-0.1.9/tests/test_phonons_gpaw.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/tests/test_phonons_lammps.py` & `atomistics-0.1.9/tests/test_phonons_lammps.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/tests/test_quasiharmonic_emt.py` & `atomistics-0.1.9/tests/test_quasiharmonic_emt.py`

 * *Files identical despite different names*

### Comparing `atomistics-0.1.8/tests/test_quasiharmonic_lammps.py` & `atomistics-0.1.9/tests/test_quasiharmonic_lammps.py`

 * *Files identical despite different names*


# Comparing `tmp/fenics-ufl-2023.2.0.tar.gz` & `tmp/fenics_ufl-2024.1.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenics-ufl-2023.2.0.tar", last modified: Mon Nov 20 15:40:49 2023, max compression
+gzip compressed data, was "fenics_ufl-2024.1.0.post0.tar", last modified: Thu Apr 25 08:20:43 2024, max compression
```

## Comparing `fenics-ufl-2023.2.0.tar` & `fenics_ufl-2024.1.0.post0.tar`

### file list

```diff
@@ -1,269 +1,252 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:40:49.698580 fenics-ufl-2023.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7639 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)    16564 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ChangeLog.rst
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2023-11-20 15:40:49.698580 fenics-ufl-2023.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:40:49.666580 fenics-ufl-2023.2.0/demo/
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/Constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/ConvectionJacobi.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/ConvectionJacobi2.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/ConvectionVector.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/Elasticity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/EnergyNorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/Equation.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/ExplicitConvection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/FEEC.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/FunctionOperators.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/H1norm.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/HarmonicMap.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/HarmonicMap2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/Heat.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/HornSchunck.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/HyperElasticity.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/HyperElasticity1D.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/L2norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/Mass.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/MassAD.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/MixedElasticity.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/MixedMixedElement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/MixedPoisson.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/MixedPoisson2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/NavierStokes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/NeumannProblem.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/NonlinearPoisson.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/P5tet.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/P5tri.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/Poisson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/PoissonDG.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/PoissonSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/PowAD.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/ProjectionSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/QuadratureElement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/RestrictedElement.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/Stiffness.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/StiffnessAD.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/Stokes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/StokesEquation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/SubDomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/SubDomains.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/TensorWeightedPoisson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/VectorLaplaceGradCurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/demo/_TensorProductElement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:40:49.654580 fenics-ufl-2023.2.0/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:40:49.654580 fenics-ufl-2023.2.0/doc/man/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:40:49.666580 fenics-ufl-2023.2.0/doc/man/man1/
--rw-r--r--   0 runner    (1001) docker     (127)      809 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/man/man1/ufl-analyse.1.gz
--rw-r--r--   0 runner    (1001) docker     (127)      957 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/man/man1/ufl-convert.1.gz
--rw-r--r--   0 runner    (1001) docker     (127)      596 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/man/man1/ufl-version.1.gz
--rw-r--r--   0 runner    (1001) docker     (127)      654 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/man/man1/ufl2py.1.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:40:49.666580 fenics-ufl-2023.2.0/doc/sphinx/
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      607 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/README
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:40:49.666580 fenics-ufl-2023.2.0/doc/sphinx/source/
--rw-r--r--   0 runner    (1001) docker     (127)     9313 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:40:49.666580 fenics-ufl-2023.2.0/doc/sphinx/source/manual/
--rw-r--r--   0 runner    (1001) docker     (127)    15582 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/source/manual/algorithms.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16051 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/source/manual/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)    52067 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/source/manual/form_language.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/source/manual/internal_representation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/source/manual/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/source/manual/user_manual.rst
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/source/manual.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:40:49.670580 fenics-ufl-2023.2.0/doc/sphinx/source/releases/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/source/releases/next.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/source/releases/v1.6.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/source/releases/v2016.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/source/releases/v2016.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/source/releases/v2017.1.0.post1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      739 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/source/releases/v2017.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/source/releases/v2017.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/source/releases/v2018.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      483 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/source/releases/v2019.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/doc/sphinx/source/releases.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:40:49.670580 fenics-ufl-2023.2.0/fenics_ufl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2023-11-20 15:40:49.000000 fenics-ufl-2023.2.0/fenics_ufl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6321 2023-11-20 15:40:49.000000 fenics-ufl-2023.2.0/fenics_ufl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-20 15:40:49.000000 fenics-ufl-2023.2.0/fenics_ufl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-20 15:40:49.000000 fenics-ufl-2023.2.0/fenics_ufl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-11-20 15:40:49.000000 fenics-ufl-2023.2.0/fenics_ufl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-11-20 15:40:49.000000 fenics-ufl-2023.2.0/fenics_ufl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2023-11-20 15:40:49.698580 fenics-ufl-2023.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:40:49.678580 fenics-ufl-2023.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/mockobjects.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4542 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_algorithms.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      684 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_analyse_demos.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3378 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_apply_algebra_lowering.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12884 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_apply_function_pullbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2137 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_apply_restrictions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3184 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_arithmetic.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20967 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_automatic_differentiation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13842 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_book_snippets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_cell.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2541 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_change_to_local.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5907 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_change_to_reference_frame.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1418 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_check_arities.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17100 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_classcoverage.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5938 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_complex.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4370 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_conditionals.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5692 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_degree_estimation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21205 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_derivative.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3586 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_diff.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8353 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (127)     8722 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_duals.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8461 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_elements.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3233 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_equals.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9128 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_evaluate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9532 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_expand_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)    15030 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_external_operator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12272 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_ffcforms.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5057 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_form.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4012 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_grad.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1644 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_illegal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1653 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_indexing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8190 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_interpolate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2081 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_lhs_rhs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3818 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_literals.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6495 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_mixed_function_space.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6546 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_new_ad.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16230 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7971 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_piecewise_checks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1005 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_reference_shapes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15780 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_scratch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18177 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_signature.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4024 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_simplify.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9254 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_sobolevspace.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3045 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_split.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3463 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_strip_forms.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4888 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_tensoralgebra.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4712 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/test/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:40:49.686580 fenics-ufl-2023.2.0/ufl/
--rw-r--r--   0 runner    (1001) docker     (127)    11082 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8040 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/adjoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    14446 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algebra.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:40:49.690580 fenics-ufl-2023.2.0/ufl/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/ad.py
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4495 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/apply_algebra_lowering.py
--rw-r--r--   0 runner    (1001) docker     (127)    64324 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/apply_derivatives.py
--rw-r--r--   0 runner    (1001) docker     (127)     7419 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/apply_function_pullbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    17595 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/apply_geometry_lowering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/apply_integral_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     9265 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/apply_restrictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/balancing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/change_to_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     7339 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/check_arities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/check_restrictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/comparison_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    17412 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/compute_form_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/coordinate_derivative_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14374 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/domain_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    11974 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/estimate_degrees.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/expand_compounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     7423 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/expand_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/formdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/formfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/formsplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16640 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/formtransformations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/map_integrands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/remove_complex_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/renumbering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/replace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/replace_derivative_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5820 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/signature.py
--rw-r--r--   0 runner    (1001) docker     (127)     5303 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/strip_terminal_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7971 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/algorithms/traversal.py
--rw-r--r--   0 runner    (1001) docker     (127)    10849 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/averaging.py
--rw-r--r--   0 runner    (1001) docker     (127)    18230 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7874 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/coefficient.py
--rw-r--r--   0 runner    (1001) docker     (127)    14598 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/compound_expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11527 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)    14772 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/constantvalue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:40:49.694580 fenics-ufl-2023.2.0/ufl/core/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7406 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/core/base_form_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/core/compute_expr_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)    14694 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/core/expr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/core/external_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/core/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7268 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/core/multiindex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/core/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/core/terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/core/ufl_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    17136 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/core/ufl_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:40:49.694580 fenics-ufl-2023.2.0/ufl/corealg/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/corealg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/corealg/map_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/corealg/multifunction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/corealg/traversal.py
--rw-r--r--   0 runner    (1001) docker     (127)    20298 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/differentiation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14196 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/duals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/equation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/exprcontainers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/exprequals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11490 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/exproperators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:40:49.694580 fenics-ufl-2023.2.0/ufl/finiteelement/
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/finiteelement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/finiteelement/brokenelement.py
--rw-r--r--   0 runner    (1001) docker     (127)    21316 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/finiteelement/elementlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/finiteelement/enrichedelement.py
--rw-r--r--   0 runner    (1001) docker     (127)    10055 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/finiteelement/finiteelement.py
--rw-r--r--   0 runner    (1001) docker     (127)     8177 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/finiteelement/finiteelementbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/finiteelement/hdivcurl.py
--rw-r--r--   0 runner    (1001) docker     (127)    19968 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/finiteelement/mixedelement.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/finiteelement/restrictedelement.py
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/finiteelement/tensorproductelement.py
--rw-r--r--   0 runner    (1001) docker     (127)    34021 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/form.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:40:49.694580 fenics-ufl-2023.2.0/ufl/formatting/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21871 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/formatting/ufl2unicode.py
--rw-r--r--   0 runner    (1001) docker     (127)    17620 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/formoperators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9553 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/functionspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    24445 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6817 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/index_combination_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/indexed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/indexsum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/integral.py
--rw-r--r--   0 runner    (1001) docker     (127)    14060 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/mathfunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    18693 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    17158 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/permutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/precedence.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/referencevalue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/restriction.py
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/sobolevspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/split_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/tensoralgebra.py
--rw-r--r--   0 runner    (1001) docker     (127)    14929 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/tensors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 15:40:49.698580 fenics-ufl-2023.2.0/ufl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/utils/counted.py
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/utils/indexflattening.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/utils/sequences.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/utils/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/utils/stacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2023-11-20 15:40:40.000000 fenics-ufl-2023.2.0/ufl/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:20:43.920341 fenics_ufl-2024.1.0.post0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-25 08:20:43.920341 fenics_ufl-2024.1.0.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:20:43.888341 fenics_ufl-2024.1.0.post0/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/Constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/ConvectionJacobi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/ConvectionJacobi2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/ConvectionVector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/Elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/EnergyNorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/Equation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/ExplicitConvection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/FunctionOperators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/H1norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/HarmonicMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/HarmonicMap2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/Heat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/HornSchunck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/HyperElasticity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/HyperElasticity1D.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/L2norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/Mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/MassAD.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/MixedElasticity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/MixedMixedElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/MixedPoisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/MixedPoisson2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/NavierStokes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/NeumannProblem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/NonlinearPoisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/P5tet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/P5tri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/Poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/PoissonDG.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/PoissonSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/PowAD.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/ProjectionSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/QuadratureElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/Stiffness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/StiffnessAD.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/Stokes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/StokesEquation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/SubDomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/SubDomains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/TensorWeightedPoisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/VectorLaplaceGradCurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/demo/_TensorProductElement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:20:43.880341 fenics_ufl-2024.1.0.post0/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:20:43.880341 fenics_ufl-2024.1.0.post0/doc/man/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:20:43.888341 fenics_ufl-2024.1.0.post0/doc/man/man1/
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/man/man1/ufl-analyse.1.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/man/man1/ufl-convert.1.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/man/man1/ufl-version.1.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/man/man1/ufl2py.1.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:20:43.892341 fenics_ufl-2024.1.0.post0/doc/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/README
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:20:43.892341 fenics_ufl-2024.1.0.post0/doc/sphinx/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:20:43.892341 fenics_ufl-2024.1.0.post0/doc/sphinx/source/manual/
+-rw-r--r--   0 runner    (1001) docker     (127)    15582 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/source/manual/algorithms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16051 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/source/manual/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    52067 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/source/manual/form_language.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/source/manual/internal_representation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/source/manual/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/source/manual/user_manual.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/source/manual.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:20:43.892341 fenics_ufl-2024.1.0.post0/doc/sphinx/source/releases/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/source/releases/next.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/source/releases/v1.6.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/source/releases/v2016.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/source/releases/v2016.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/source/releases/v2017.1.0.post1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/source/releases/v2017.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/source/releases/v2017.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/source/releases/v2018.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/source/releases/v2019.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/doc/sphinx/source/releases.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:20:43.920341 fenics_ufl-2024.1.0.post0/fenics_ufl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-25 08:20:43.000000 fenics_ufl-2024.1.0.post0/fenics_ufl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-25 08:20:43.000000 fenics_ufl-2024.1.0.post0/fenics_ufl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:20:43.000000 fenics_ufl-2024.1.0.post0/fenics_ufl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-25 08:20:43.000000 fenics_ufl-2024.1.0.post0/fenics_ufl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-25 08:20:43.000000 fenics_ufl-2024.1.0.post0/fenics_ufl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:20:43.920341 fenics_ufl-2024.1.0.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:20:43.904341 fenics_ufl-2024.1.0.post0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/mockobjects.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4796 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_algorithms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      672 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_analyse_demos.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4156 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_apply_algebra_lowering.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16047 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_apply_function_pullbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2408 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_apply_restrictions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3452 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_arithmetic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21884 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_automatic_differentiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_cell.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2799 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_change_to_local.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6338 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_change_to_reference_frame.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1762 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_check_arities.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17739 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_classcoverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6539 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_complex.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4552 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_conditionals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5049 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_degree_estimation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23444 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_derivative.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3820 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13409 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_duals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3763 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_equals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9957 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_evaluate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10098 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_expand_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15391 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_external_operator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13494 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_ffcforms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5580 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_form.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1822 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_illegal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1786 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_indexing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9308 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_interpolate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2402 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_lhs_rhs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3851 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_literals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6659 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_mixed_function_space.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7119 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_new_ad.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17988 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10246 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_piecewise_checks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2031 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_reference_shapes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16319 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_scratch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21257 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_signature.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4509 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_simplify.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5296 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_sobolevspace.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3366 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_split.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4184 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_strip_forms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5123 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_tensoralgebra.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4824 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/test/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:20:43.908341 fenics_ufl-2024.1.0.post0/ufl/
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14235 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algebra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:20:43.916341 fenics_ufl-2024.1.0.post0/ufl/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/apply_algebra_lowering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64677 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/apply_derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/apply_function_pullbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17564 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/apply_geometry_lowering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/apply_integral_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/apply_restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/balancing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/change_to_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/check_arities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/check_restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/comparison_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17213 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/compute_form_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/coordinate_derivative_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14700 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/domain_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/estimate_degrees.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/expand_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/formdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/formfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/formsplitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16653 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/formtransformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/map_integrands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/remove_complex_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/renumbering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/replace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/replace_derivative_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/strip_terminal_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/algorithms/traversal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/averaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/compound_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14901 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/constantvalue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:20:43.916341 fenics_ufl-2024.1.0.post0/ufl/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/core/base_form_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/core/compute_expr_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14465 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/core/expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/core/external_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/core/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/core/multiindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/core/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/core/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/core/ufl_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16097 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/core/ufl_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:20:43.916341 fenics_ufl-2024.1.0.post0/ufl/corealg/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/corealg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/corealg/map_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/corealg/multifunction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/corealg/traversal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19698 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/differentiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8749 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/duals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/equation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/exprcontainers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/exprequals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11578 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/exproperators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14145 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/finiteelement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32680 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/form.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:20:43.916341 fenics_ufl-2024.1.0.post0/ufl/formatting/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21814 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/formatting/ufl2unicode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17547 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/formoperators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/functionspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24675 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/index_combination_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/indexed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/indexsum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/integral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14075 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/mathfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18862 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17730 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/permutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/precedence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19237 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/pullback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/referencevalue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/restriction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/sobolevspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/split_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/tensoralgebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15025 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/tensors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:20:43.920341 fenics_ufl-2024.1.0.post0/ufl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/utils/counted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/utils/indexflattening.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/utils/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/utils/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/utils/stacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-25 08:20:37.000000 fenics_ufl-2024.1.0.post0/ufl/variable.py
```

### Comparing `fenics-ufl-2023.2.0/AUTHORS` & `fenics_ufl-2024.1.0.post0/AUTHORS`

 * *Files 8% similar despite different names*

```diff
@@ -27,7 +27,8 @@
   | Maximilian Albert     <maximilian.albert@gmail.com>
   | Corrado Maurini       <corrado.maurini@upmc.fr>
   | Jack S. Hale          <mail@jackhale.co.uk>
   | Tuomas Airaksinen     <tuomas.airaksinen@gmail.com>
   | Nacime Bouziani       <nacime.bouziani@gmail.com>
   | Reuben W. Hill        <reuben.hill10@imperial.ac.uk>
   | Nacime Bouziani       <n.bouziani18@imperial.ac.uk>
+  | Matthew Scroggs       <matthew.scroggs.14@ucl.ac.uk>
```

### Comparing `fenics-ufl-2023.2.0/COPYING` & `fenics_ufl-2024.1.0.post0/COPYING`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/COPYING.LESSER` & `fenics_ufl-2024.1.0.post0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/PKG-INFO` & `fenics_ufl-2024.1.0.post0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,93 +1,67 @@
 Metadata-Version: 2.1
 Name: fenics-ufl
-Version: 2023.2.0
+Version: 2024.1.0.post0
 Summary: Unified Form Language
-Home-page: https://github.com/FEniCS/ufl
-Author: FEniCS Project Contributors
-Maintainer: FEniCS Project Steering Council
-License: LGPL-3.0-or-later
-Project-URL: Homepage, https://fenicsproject.org
-Project-URL: Documentation, https://fenics.readthedocs.io/projects/ufl
-Project-URL: Issues, https://github.com/FEniCS/ufl/issues
-Project-URL: Funding, https://numfocus.org/donate
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
+Author: UFL contributors
+Maintainer: FEniCS Steering Council
+Maintainer-email: fenics-steering-council@googlegroups.com
+Project-URL: homepage, https://fenicsproject.org
+Project-URL: repository, https://github.com/fenics/ufl.git
+Project-URL: documentation, https://docs.fenicsproject.org
+Project-URL: issues, https://github.com/FEniCS/ufl/issues
+Project-URL: funding, https://numfocus.org/donate
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
 License-File: AUTHORS
 Requires-Dist: numpy
+Provides-Extra: lint
+Requires-Dist: ruff; extra == "lint"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
-Provides-Extra: lint
-Requires-Dist: flake8; extra == "lint"
-Requires-Dist: pydocstyle[toml]; extra == "lint"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: ci
-Requires-Dist: coverage; extra == "ci"
 Requires-Dist: coveralls; extra == "ci"
+Requires-Dist: coverage; extra == "ci"
 Requires-Dist: pytest-cov; extra == "ci"
 Requires-Dist: pytest-xdist; extra == "ci"
 Requires-Dist: fenics-ufl[docs]; extra == "ci"
 Requires-Dist: fenics-ufl[lint]; extra == "ci"
 Requires-Dist: fenics-ufl[test]; extra == "ci"
 
-===========================
-UFL - Unified Form Language
-===========================
+# UFL - Unified Form Language
 
 The Unified Form Language (UFL) is a domain specific language for
 declaration of finite element discretizations of variational forms. More
 precisely, it defines a flexible interface for choosing finite element
 spaces and defining expressions for weak forms in a notation close to
 mathematical notation.
 
 UFL is part of the FEniCS Project. For more information, visit
 https://www.fenicsproject.org
 
-.. image:: https://github.com/FEniCS/ufl/workflows/UFL%20CI/badge.svg
-   :target: https://github.com/FEniCS/ufl/workflows/UFL%20CI
-.. image:: https://coveralls.io/repos/github/FEniCS/ufl/badge.svg?branch=master
-   :target: https://coveralls.io/github/FEniCS/ufl?branch=master
-   :alt: Coverage Status
-.. image:: https://readthedocs.org/projects/fenics-ufl/badge/?version=latest
-   :target: https://fenics.readthedocs.io/projects/ufl/en/latest/?badge=latest
-   :alt: Documentation Status
-
-Documentation
-=============
-
-Documentation can be viewed at https://fenics-ufl.readthedocs.org/.
-
-License
-=======
-
-  This program is free software: you can redistribute it and/or modify
-  it under the terms of the GNU Lesser General Public License as published by
-  the Free Software Foundation, either version 3 of the License, or
-  (at your option) any later version.
-
-  This program is distributed in the hope that it will be useful,
-  but WITHOUT ANY WARRANTY; without even the implied warranty of
-  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-  GNU Lesser General Public License for more details.
+[![UFL CI](https://github.com/FEniCS/ufl/workflows/UFL%20CI/badge.svg)](https://github.com/FEniCS/ufl/workflows/UFL%20CI)
+[![Coverage Status](https://coveralls.io/repos/github/FEniCS/ufl/badge.svg?branch=master)](https://coveralls.io/github/FEniCS/ufl?branch=master)
+
+## Documentation
+
+Documentation can be viewed at https://docs.fenicsproject.org
+
+## License
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU Lesser General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+GNU Lesser General Public License for more details.
 
-  You should have received a copy of the GNU Lesser General Public License
-  along with this program. If not, see <https://www.gnu.org/licenses/>.
+You should have received a copy of the GNU Lesser General Public License
+along with this program. If not, see <https://www.gnu.org/licenses/>.
```

### Comparing `fenics-ufl-2023.2.0/README.rst` & `fenics_ufl-2024.1.0.post0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,33 @@
-===========================
-UFL - Unified Form Language
-===========================
+# UFL - Unified Form Language
 
 The Unified Form Language (UFL) is a domain specific language for
 declaration of finite element discretizations of variational forms. More
 precisely, it defines a flexible interface for choosing finite element
 spaces and defining expressions for weak forms in a notation close to
 mathematical notation.
 
 UFL is part of the FEniCS Project. For more information, visit
 https://www.fenicsproject.org
 
-.. image:: https://github.com/FEniCS/ufl/workflows/UFL%20CI/badge.svg
-   :target: https://github.com/FEniCS/ufl/workflows/UFL%20CI
-.. image:: https://coveralls.io/repos/github/FEniCS/ufl/badge.svg?branch=master
-   :target: https://coveralls.io/github/FEniCS/ufl?branch=master
-   :alt: Coverage Status
-.. image:: https://readthedocs.org/projects/fenics-ufl/badge/?version=latest
-   :target: https://fenics.readthedocs.io/projects/ufl/en/latest/?badge=latest
-   :alt: Documentation Status
-
-Documentation
-=============
-
-Documentation can be viewed at https://fenics-ufl.readthedocs.org/.
-
-License
-=======
-
-  This program is free software: you can redistribute it and/or modify
-  it under the terms of the GNU Lesser General Public License as published by
-  the Free Software Foundation, either version 3 of the License, or
-  (at your option) any later version.
-
-  This program is distributed in the hope that it will be useful,
-  but WITHOUT ANY WARRANTY; without even the implied warranty of
-  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-  GNU Lesser General Public License for more details.
+[![UFL CI](https://github.com/FEniCS/ufl/workflows/UFL%20CI/badge.svg)](https://github.com/FEniCS/ufl/workflows/UFL%20CI)
+[![Coverage Status](https://coveralls.io/repos/github/FEniCS/ufl/badge.svg?branch=master)](https://coveralls.io/github/FEniCS/ufl?branch=master)
 
-  You should have received a copy of the GNU Lesser General Public License
-  along with this program. If not, see <https://www.gnu.org/licenses/>.
+## Documentation
+
+Documentation can be viewed at https://docs.fenicsproject.org
+
+## License
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU Lesser General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+GNU Lesser General Public License for more details.
+
+You should have received a copy of the GNU Lesser General Public License
+along with this program. If not, see <https://www.gnu.org/licenses/>.
```

### Comparing `fenics-ufl-2023.2.0/demo/Constant.py` & `fenics_ufl-2024.1.0.post0/demo/Constant.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,24 +14,39 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with UFL. If not, see <http://www.gnu.org/licenses/>.
 #
 # Modified by Martin Sandve Alnes, 2009
 #
 # Test form for scalar and vector constants.
-from ufl import (Coefficient, Constant, FiniteElement, FunctionSpace, Mesh, TestFunction, TrialFunction, VectorConstant,
-                 VectorElement, dot, dx, grad, inner, triangle)
+from ufl import (
+    Coefficient,
+    Constant,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TrialFunction,
+    VectorConstant,
+    dot,
+    dx,
+    grad,
+    inner,
+    triangle,
+)
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 cell = triangle
-element = FiniteElement("Lagrange", cell, 1)
-domain = Mesh(VectorElement("Lagrange", cell, 1))
+element = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
 space = FunctionSpace(domain, element)
 
 v = TestFunction(space)
 u = TrialFunction(space)
 f = Coefficient(space)
 
-c = Constant(space)
-d = VectorConstant(space)
+c = Constant(domain)
+d = VectorConstant(domain)
 
 a = c * dot(grad(v), grad(u)) * dx
 L = inner(d, grad(v)) * dx
```

### Comparing `fenics-ufl-2023.2.0/demo/EnergyNorm.py` & `fenics_ufl-2024.1.0.post0/demo/P5tet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2005-2007 Anders Logg
+# Copyright (C) 2006-2007 Anders Logg
 #
 # This file is part of UFL.
 #
 # UFL is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,17 +11,14 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with UFL. If not, see <http://www.gnu.org/licenses/>.
 #
-# This example demonstrates how to define a functional, here
-# the energy norm (squared) for a reaction-diffusion problem.
-from ufl import Coefficient, FiniteElement, FunctionSpace, Mesh, VectorElement, dot, dx, grad, tetrahedron
+# A fifth degree Lagrange finite element on a tetrahedron
+from ufl import tetrahedron
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
-element = FiniteElement("Lagrange", tetrahedron, 1)
-domain = Mesh(VectorElement("Lagrange", tetrahedron, 1))
-space = FunctionSpace(domain, element)
-
-v = Coefficient(space)
-a = (v * v + dot(grad(v), grad(v))) * dx
+element = FiniteElement("Lagrange", tetrahedron, 5, (), identity_pullback, H1)
```

### Comparing `fenics-ufl-2023.2.0/demo/Equation.py` & `fenics_ufl-2024.1.0.post0/demo/Stokes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2007 Anders Logg
+# Copyright (C) 2005-2007 Anders Logg
 #
 # This file is part of UFL.
 #
 # UFL is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,43 +11,44 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with UFL. If not, see <http://www.gnu.org/licenses/>.
 #
-# Specification of a system F(v, u) = 0 and extraction of
-# the bilinear and linear forms a and L for the left- and
-# right-hand sides:
-#
-#   F(v, u) = a(v, u) - L(v) = 0
-#
-# The example below demonstrates the specification of the
-# linear system for a cG(1)/Crank-Nicholson time step for
-# the heat equation.
-#
-# The below formulation is equivalent to writing
-#
-#  a = v*u*dx + 0.5*k*dot(grad(v), grad(u))*dx
-#  L = v*u0*dx - 0.5*k*dot(grad(v), grad(u0))*dx
-#
-# but instead of manually shuffling terms not including
-# the unknown u to the right-hand side, all terms may
-# be listed on one line and left- and right-hand sides
-# extracted by lhs() and rhs().
-from ufl import (Coefficient, FiniteElement, FunctionSpace, Mesh, TestFunction, TrialFunction, VectorElement, dot, dx,
-                 grad, lhs, rhs, triangle)
-
-element = FiniteElement("Lagrange", triangle, 1)
-domain = Mesh(VectorElement("Lagrange", triangle, 1))
-space = FunctionSpace(domain, element)
+# Modified by: Martin Sandve Alnes (2009)
+# Date: 2009-03-02
+#
+# The bilinear form a(v, u) and Linear form L(v) for the Stokes
+# equations using a mixed formulation (Taylor-Hood elements).
+from ufl import (
+    Coefficient,
+    FunctionSpace,
+    Mesh,
+    TestFunctions,
+    TrialFunctions,
+    div,
+    dot,
+    dx,
+    grad,
+    inner,
+    triangle,
+)
+from ufl.finiteelement import FiniteElement, MixedElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
-k = 0.1
+cell = triangle
+P2 = FiniteElement("Lagrange", cell, 2, (2,), identity_pullback, H1)
+P1 = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+TH = MixedElement([P2, P1])
+domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
+space = FunctionSpace(domain, TH)
+p2_space = FunctionSpace(domain, P2)
 
-v = TestFunction(space)
-u = TrialFunction(space)
-u0 = Coefficient(space)
+(v, q) = TestFunctions(space)
+(u, p) = TrialFunctions(space)
 
-F = v * (u - u0) * dx + k * dot(grad(v), grad(0.5 * (u0 + u))) * dx
+f = Coefficient(p2_space)
 
-a = lhs(F)
-L = rhs(F)
+a = (inner(grad(v), grad(u)) - div(v) * p + q * div(u)) * dx
+L = dot(v, f) * dx
```

### Comparing `fenics-ufl-2023.2.0/demo/FEEC.py` & `fenics_ufl-2024.1.0.post0/demo/QuadratureElement.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2010 Marie Rognes
+# Copyright (C) 2008 Kristian B. Oelgaard
 #
 # This file is part of UFL.
 #
 # UFL is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -10,47 +10,51 @@
 # UFL is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with UFL. If not, see <http://www.gnu.org/licenses/>.
-
-"""
-This demo illustrates the FEEC notation
-
-  V = FiniteElement("P Lambda", cell, r, k)
-  V = FiniteElement("P- Lambda", cell, r, k)
-
-and their aliases.
-"""
-from ufl import (FiniteElement, FunctionSpace, Mesh, TestFunction, TestFunctions, TrialFunction, TrialFunctions,
-                 VectorElement, dx)
-from ufl import exterior_derivative as d
-from ufl import inner, interval, tetrahedron, triangle
-
-cells = [interval, triangle, tetrahedron]
-r = 1
-
-for cell in cells:
-    for family in ["P Lambda", "P- Lambda"]:
-        tdim = cell.topological_dimension()
-        for k in range(0, tdim + 1):
-
-            # Testing exterior derivative
-            V = FiniteElement(family, cell, r, form_degree=k)
-            domain = Mesh(VectorElement("Lagrange", cell, 1))
-            space = FunctionSpace(domain, V)
-            v = TestFunction(space)
-            u = TrialFunction(space)
-
-            a = inner(d(u), d(v)) * dx
-
-            # Testing mixed formulation of Hodge Laplace
-            if k > 0 and k < tdim + 1:
-                S = FiniteElement(family, cell, r, form_degree=k - 1)
-                W = S * V
-                mixed_space = FunctionSpace(domain, W)
-                (sigma, u) = TrialFunctions(mixed_space)
-                (tau, v) = TestFunctions(mixed_space)
-
-                a = (inner(sigma, tau) - inner(d(tau), u) + inner(d(sigma), v) + inner(d(u), d(v))) * dx
+#
+# First added:  2008-03-31
+# Last changed: 2008-03-31
+#
+# The linearised bilinear form a(u,v) and linear form L(v) for
+# the nonlinear equation - div (1+u) grad u = f (non-linear Poisson)
+from ufl import (
+    Coefficient,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TrialFunction,
+    dot,
+    dx,
+    grad,
+    i,
+    triangle,
+)
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
+
+element = FiniteElement("Lagrange", triangle, 2, (), identity_pullback, H1)
+domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
+space = FunctionSpace(domain, element)
+
+QE = FiniteElement("Quadrature", triangle, 2, (), identity_pullback, H1)
+sig = FiniteElement("Quadrature", triangle, 1, (2,), identity_pullback, H1)
+
+qe_space = FunctionSpace(domain, QE)
+sig_space = FunctionSpace(domain, sig)
+
+v = TestFunction(space)
+u = TrialFunction(space)
+u0 = Coefficient(space)
+C = Coefficient(qe_space)
+sig0 = Coefficient(sig_space)
+f = Coefficient(space)
+
+a = (
+    v.dx(i) * C * u.dx(i) * dx(metadata={"quadrature_degree": 2})
+    + v.dx(i) * 2 * u0 * u * u0.dx(i) * dx
+)
+L = v * f * dx - dot(grad(v), sig0) * dx(metadata={"quadrature_degree": 1})
```

### Comparing `fenics-ufl-2023.2.0/demo/FunctionOperators.py` & `fenics_ufl-2024.1.0.post0/demo/FunctionOperators.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,20 +12,37 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with UFL. If not, see <http://www.gnu.org/licenses/>.
 #
 # Test form for operators on Coefficients.
-from ufl import (Coefficient, FiniteElement, FunctionSpace, Mesh, TestFunction, TrialFunction, VectorElement, dot, dx,
-                 grad, max_value, sqrt, triangle)
+from ufl import (
+    Coefficient,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TrialFunction,
+    dot,
+    dx,
+    grad,
+    max_value,
+    sqrt,
+    triangle,
+)
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
-element = FiniteElement("Lagrange", triangle, 1)
-domain = Mesh(VectorElement("Lagrange", triangle, 1))
+element = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
 space = FunctionSpace(domain, element)
 
 v = TestFunction(space)
 u = TrialFunction(space)
 f = Coefficient(space)
 g = Coefficient(space)
 
-a = sqrt(1 / max_value(1 / f, -1 / f)) * sqrt(g) * dot(grad(v), grad(u)) * dx + v * u * sqrt(f * g) * g * dx
+a = (
+    sqrt(1 / max_value(1 / f, -1 / f)) * sqrt(g) * dot(grad(v), grad(u)) * dx
+    + v * u * sqrt(f * g) * g * dx
+)
```

### Comparing `fenics-ufl-2023.2.0/demo/HarmonicMap.py` & `fenics_ufl-2024.1.0.post0/demo/HarmonicMap.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #
 # Harmonic map demo using separate coefficients x and y.
 # Author: Martin Alnes
 # Date: 2009-04-09
 #
-from ufl import (Coefficient, FiniteElement, FunctionSpace, Mesh, VectorElement, derivative, dot, dx, grad, inner,
-                 triangle)
+from ufl import Coefficient, FunctionSpace, Mesh, derivative, dot, dx, grad, inner, triangle
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 cell = triangle
-X = VectorElement("Lagrange", cell, 1)
-Y = FiniteElement("Lagrange", cell, 1)
-domain = Mesh(VectorElement("Lagrange", cell, 1))
+X = FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1)
+Y = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
 X_space = FunctionSpace(domain, X)
 Y_space = FunctionSpace(domain, Y)
 
 x = Coefficient(X_space)
 y = Coefficient(Y_space)
 
 L = inner(grad(x), grad(x)) * dx + dot(x, x) * y * dx
```

### Comparing `fenics-ufl-2023.2.0/demo/Heat.py` & `fenics_ufl-2024.1.0.post0/demo/Heat.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,24 +16,37 @@
 # along with UFL. If not, see <http://www.gnu.org/licenses/>.
 #
 # Modified by Martin Sandve Alnes, 2009
 #
 # The bilinear form a(v, u1) and linear form L(v) for
 # one backward Euler step with the heat equation.
 #
-from ufl import (Coefficient, Constant, FiniteElement, FunctionSpace, Mesh, TestFunction, TrialFunction, VectorElement,
-                 dot, dx, grad, triangle)
+from ufl import (
+    Coefficient,
+    Constant,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TrialFunction,
+    dot,
+    dx,
+    grad,
+    triangle,
+)
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 cell = triangle
-element = FiniteElement("Lagrange", cell, 1)
-domain = Mesh(VectorElement("Lagrange", cell, 1))
+element = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
 space = FunctionSpace(domain, element)
 
 v = TestFunction(space)  # Test function
 u1 = TrialFunction(space)  # Value at t_n
-u0 = Coefficient(space)      # Value at t_n-1
-c = Coefficient(space)      # Heat conductivity
-f = Coefficient(space)      # Heat source
-k = Constant(domain)         # Time step
+u0 = Coefficient(space)  # Value at t_n-1
+c = Coefficient(space)  # Heat conductivity
+f = Coefficient(space)  # Heat source
+k = Constant(domain)  # Time step
 
 a = v * u1 * dx + k * c * dot(grad(v), grad(u1)) * dx
 L = v * u0 * dx + k * v * f * dx
```

### Comparing `fenics-ufl-2023.2.0/demo/Mass.py` & `fenics_ufl-2024.1.0.post0/demo/P5tri.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2004-2007 Anders Logg
+# Copyright (C) 2006-2007 Anders Logg
 #
 # This file is part of UFL.
 #
 # UFL is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,22 +11,14 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with UFL. If not, see <http://www.gnu.org/licenses/>.
 #
-# Modified by Martin Sandve Alnes, 2009
-#
-# Last changed: 2009-03-02
-#
-# The bilinear form for a mass matrix.
-from ufl import FiniteElement, FunctionSpace, Mesh, TestFunction, TrialFunction, VectorElement, dx, triangle
-
-element = FiniteElement("Lagrange", triangle, 1)
-domain = Mesh(VectorElement("Lagrange", triangle, 1))
-space = FunctionSpace(domain, element)
-
-u = TrialFunction(space)
-v = TestFunction(space)
+# A fifth degree Lagrange finite element on a triangle
+from ufl import triangle
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
-a = v * u * dx
+element = FiniteElement("Lagrange", triangle, 5, (), identity_pullback, H1)
```

### Comparing `fenics-ufl-2023.2.0/demo/MixedElasticity.py` & `fenics_ufl-2024.1.0.post0/demo/MixedElasticity.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,44 +13,57 @@
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with UFL. If not, see <http://www.gnu.org/licenses/>.
 #
 # First added:  2008-10-03
 # Last changed: 2011-07-22
-from ufl import (FunctionSpace, Mesh, MixedElement, TestFunctions, TrialFunctions, VectorElement, as_vector, div, dot,
-                 dx, inner, skew, tetrahedron, tr)
+from ufl import (
+    FunctionSpace,
+    Mesh,
+    TestFunctions,
+    TrialFunctions,
+    as_vector,
+    div,
+    dot,
+    dx,
+    inner,
+    skew,
+    tetrahedron,
+    tr,
+)
+from ufl.finiteelement import FiniteElement, MixedElement
+from ufl.pullback import contravariant_piola, identity_pullback
+from ufl.sobolevspace import H1, L2, HDiv
 
 
 def skw(tau):
     """Define vectorized skew operator"""
     sk = 2 * skew(tau)
     return as_vector((sk[0, 1], sk[0, 2], sk[1, 2]))
 
 
 cell = tetrahedron
 n = 3
 
 # Finite element exterior calculus syntax
 r = 1
-S = VectorElement("P Lambda", cell, r, form_degree=n - 1)
-V = VectorElement("P Lambda", cell, r - 1, form_degree=n)
-Q = VectorElement("P Lambda", cell, r - 1, form_degree=n)
-
-# Alternative syntax:
-# S = VectorElement("BDM", cell, r)
-# V = VectorElement("Discontinuous Lagrange", cell, r-1)
-# Q = VectorElement("Discontinuous Lagrange", cell, r-1)
+S = FiniteElement("vector BDM", cell, r, (3, 3), contravariant_piola, HDiv)
+V = FiniteElement("Discontinuous Lagrange", cell, r - 1, (3,), identity_pullback, L2)
+Q = FiniteElement("Discontinuous Lagrange", cell, r - 1, (3,), identity_pullback, L2)
 
-W = MixedElement(S, V, Q)
+W = MixedElement([S, V, Q])
 
-domain = Mesh(VectorElement("Lagrange", cell, 1))
+domain = Mesh(FiniteElement("Lagrange", cell, 1, (3,), identity_pullback, H1))
 space = FunctionSpace(domain, W)
 
 (sigma, u, gamma) = TrialFunctions(space)
 (tau, v, eta) = TestFunctions(space)
 
 a = (
-    inner(sigma, tau) - tr(sigma) * tr(tau) + dot(
-        div(tau), u
-    ) - dot(div(sigma), v) + inner(skw(tau), gamma) + inner(skw(sigma), eta)
+    inner(sigma, tau)
+    - tr(sigma) * tr(tau)
+    + dot(div(tau), u)
+    - dot(div(sigma), v)
+    + inner(skw(tau), gamma)
+    + inner(skw(sigma), eta)
 ) * dx
```

### Comparing `fenics-ufl-2023.2.0/demo/MixedPoisson.py` & `fenics_ufl-2024.1.0.post0/demo/PoissonSystem.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2006-2009 Anders Logg and Marie Rognes
+# Copyright (C) 2005-2007 Anders Logg
 #
 # This file is part of UFL.
 #
 # UFL is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,34 +11,40 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with UFL. If not, see <http://www.gnu.org/licenses/>.
 #
-# Modified by Martin Sandve Alnes, 2009
+# Modified by: Martin Sandve Alnes, 2009
 #
-# Last changed: 2009-01-12
+# Last changed: 2009-03-02
 #
 # The bilinear form a(v, u) and linear form L(v) for
-# a mixed formulation of Poisson's equation with BDM
-# (Brezzi-Douglas-Marini) elements.
-#
-from ufl import (Coefficient, FiniteElement, FunctionSpace, Mesh, TestFunctions, TrialFunctions, VectorElement, div,
-                 dot, dx, triangle)
+# Poisson's equation in system form (vector-valued).
+from ufl import (
+    Coefficient,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TrialFunction,
+    dot,
+    dx,
+    grad,
+    inner,
+    triangle,
+)
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 cell = triangle
-BDM1 = FiniteElement("Brezzi-Douglas-Marini", cell, 1)
-DG0 = FiniteElement("Discontinuous Lagrange", cell, 0)
-
-element = BDM1 * DG0
-domain = Mesh(VectorElement("Lagrange", cell, 1))
+element = FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1)
+domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
 space = FunctionSpace(domain, element)
-dg0_space = FunctionSpace(domain, DG0)
-
-(tau, w) = TestFunctions(space)
-(sigma, u) = TrialFunctions(space)
 
-f = Coefficient(dg0_space)
+v = TestFunction(space)
+u = TrialFunction(space)
+f = Coefficient(space)
 
-a = (dot(tau, sigma) - div(tau) * u + w * div(sigma)) * dx
-L = w * f * dx
+a = inner(grad(v), grad(u)) * dx
+L = dot(v, f) * dx
```

### Comparing `fenics-ufl-2023.2.0/demo/NavierStokes.py` & `fenics_ufl-2024.1.0.post0/demo/Mass.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,26 +11,25 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with UFL. If not, see <http://www.gnu.org/licenses/>.
 #
-# Modified by Martin Sandve Alnes
+# Modified by Martin Sandve Alnes, 2009
 #
 # Last changed: 2009-03-02
 #
-# The bilinear form for the nonlinear term in the
-# Navier-Stokes equations with fixed convective velocity.
-from ufl import Coefficient, FunctionSpace, Mesh, TestFunction, TrialFunction, VectorElement, dot, dx, grad, tetrahedron
+# The bilinear form for a mass matrix.
+from ufl import FunctionSpace, Mesh, TestFunction, TrialFunction, dx, triangle
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
-cell = tetrahedron
-element = VectorElement("Lagrange", cell, 1)
-domain = Mesh(VectorElement("Lagrange", cell, 1))
+element = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
 space = FunctionSpace(domain, element)
 
-v = TestFunction(space)
 u = TrialFunction(space)
-w = Coefficient(space)
+v = TestFunction(space)
 
-Du = grad(u)
-a = dot(dot(w, Du), v) * dx
+a = v * u * dx
```

### Comparing `fenics-ufl-2023.2.0/demo/NeumannProblem.py` & `fenics_ufl-2024.1.0.post0/demo/Poisson.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright (C) 2006-2007 Anders Logg
+# -*- coding: utf-8 -*-
+# Copyright (C) 2004-2008 Anders Logg
 #
 # This file is part of UFL.
 #
 # UFL is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,23 +12,37 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with UFL. If not, see <http://www.gnu.org/licenses/>.
 #
-# The bilinear form a(v, u) and linear form L(v) for
-# Poisson's equation with Neumann boundary conditions.
-from ufl import (Coefficient, FunctionSpace, Mesh, TestFunction, TrialFunction, VectorElement, ds, dx, grad, inner,
-                 triangle)
+# Modified by Martin Sandve Alnæs, 2009
+#
+# Last changed: 2009-03-02
+#
+# The bilinear form a(v, u) and linear form L(v) for Poisson's equation.
+from ufl import (
+    Coefficient,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TrialFunction,
+    dx,
+    grad,
+    inner,
+    triangle,
+)
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
-element = VectorElement("Lagrange", triangle, 1)
-domain = Mesh(VectorElement("Lagrange", triangle, 1))
+element = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
 space = FunctionSpace(domain, element)
 
-v = TestFunction(space)
 u = TrialFunction(space)
+v = TestFunction(space)
 f = Coefficient(space)
-g = Coefficient(space)
 
-a = inner(grad(v), grad(u)) * dx
-L = inner(v, f) * dx + inner(v, g) * ds
+a = inner(grad(v), grad(u)) * dx(degree=1)
+L = v * f * dx(degree=2)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fenics-ufl-2023.2.0/demo/P5tet.py` & `fenics_ufl-2024.1.0.post0/demo/EnergyNorm.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2006-2007 Anders Logg
+# Copyright (C) 2005-2007 Anders Logg
 #
 # This file is part of UFL.
 #
 # UFL is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,11 +11,20 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with UFL. If not, see <http://www.gnu.org/licenses/>.
 #
-# A fifth degree Lagrange finite element on a tetrahedron
-from ufl import FiniteElement, tetrahedron
+# This example demonstrates how to define a functional, here
+# the energy norm (squared) for a reaction-diffusion problem.
+from ufl import Coefficient, FunctionSpace, Mesh, dot, dx, grad, tetrahedron
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
-element = FiniteElement("Lagrange", tetrahedron, 5)
+element = FiniteElement("Lagrange", tetrahedron, 1, (), identity_pullback, H1)
+domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
+space = FunctionSpace(domain, element)
+
+v = Coefficient(space)
+a = (v * v + dot(grad(v), grad(v))) * dx
```

### Comparing `fenics-ufl-2023.2.0/demo/Poisson.py` & `fenics_ufl-2024.1.0.post0/demo/SubDomain.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# -*- coding: utf-8 -*-
-# Copyright (C) 2004-2008 Anders Logg
+# Copyright (C) 2008 Anders Logg
 #
 # This file is part of UFL.
 #
 # UFL is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -12,25 +11,23 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with UFL. If not, see <http://www.gnu.org/licenses/>.
 #
-# Modified by Martin Sandve Alnæs, 2009
-#
-# Last changed: 2009-03-02
-#
-# The bilinear form a(v, u) and linear form L(v) for Poisson's equation.
-from ufl import (Coefficient, FiniteElement, FunctionSpace, Mesh, TestFunction, TrialFunction, VectorElement, dx, grad,
-                 inner, triangle)
+# This example illustrates how to define a form over a
+# given subdomain of a mesh, in this case a functional.
+from ufl import Coefficient, FunctionSpace, Mesh, TestFunction, TrialFunction, ds, dx, tetrahedron
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
-element = FiniteElement("Lagrange", triangle, 1)
-domain = Mesh(VectorElement("Lagrange", triangle, 1))
+element = FiniteElement("Lagrange", tetrahedron, 1, (), identity_pullback, H1)
+domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
 space = FunctionSpace(domain, element)
 
-u = TrialFunction(space)
 v = TestFunction(space)
+u = TrialFunction(space)
 f = Coefficient(space)
 
-a = inner(grad(v), grad(u)) * dx(degree=1)
-L = v * f * dx(degree=2)
+M = f * dx(2) + f * ds(5)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fenics-ufl-2023.2.0/demo/PoissonDG.py` & `fenics_ufl-2024.1.0.post0/demo/PoissonDG.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,36 +17,57 @@
 #
 # First added:  2006-12-05
 # Last changed: 2007-07-15
 #
 # The bilinear form a(v, u) and linear form L(v) for
 # Poisson's equation in a discontinuous Galerkin (DG)
 # formulation.
-from ufl import (Coefficient, Constant, FacetNormal, FiniteElement, FunctionSpace, Mesh, TestFunction, TrialFunction,
-                 VectorElement, avg, dot, dS, ds, dx, grad, inner, jump, triangle)
+from ufl import (
+    Coefficient,
+    Constant,
+    FacetNormal,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TrialFunction,
+    avg,
+    dot,
+    dS,
+    ds,
+    dx,
+    grad,
+    inner,
+    jump,
+    triangle,
+)
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1, L2
 
 cell = triangle
-element = FiniteElement("Discontinuous Lagrange", cell, 1)
-domain = Mesh(VectorElement("Lagrange", cell, 1))
+element = FiniteElement("Discontinuous Lagrange", cell, 1, (), identity_pullback, L2)
+domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
 space = FunctionSpace(domain, element)
 
 v = TestFunction(space)
 u = TrialFunction(space)
 f = Coefficient(space)
 
 n = FacetNormal(domain)
 h = Constant(domain)
 
 gN = Coefficient(space)
 
 alpha = 4.0
 gamma = 8.0
 
-a = inner(grad(v), grad(u)) * dx \
-    - inner(avg(grad(v)), jump(u, n)) * dS \
-    - inner(jump(v, n), avg(grad(u))) * dS \
-    + alpha / h('+') * dot(jump(v, n), jump(u, n)) * dS \
-    - inner(grad(v), u * n) * ds \
-    - inner(v * n, grad(u)) * ds \
+a = (
+    inner(grad(v), grad(u)) * dx
+    - inner(avg(grad(v)), jump(u, n)) * dS
+    - inner(jump(v, n), avg(grad(u))) * dS
+    + alpha / h("+") * dot(jump(v, n), jump(u, n)) * dS
+    - inner(grad(v), u * n) * ds
+    - inner(v * n, grad(u)) * ds
     + gamma / h * v * u * ds
+)
 
 L = v * f * dx + v * gN * ds
```

### Comparing `fenics-ufl-2023.2.0/demo/PoissonSystem.py` & `fenics_ufl-2024.1.0.post0/demo/NavierStokes.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2005-2007 Anders Logg
+# Copyright (C) 2004-2007 Anders Logg
 #
 # This file is part of UFL.
 #
 # UFL is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,27 +11,39 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with UFL. If not, see <http://www.gnu.org/licenses/>.
 #
-# Modified by: Martin Sandve Alnes, 2009
+# Modified by Martin Sandve Alnes
 #
 # Last changed: 2009-03-02
 #
-# The bilinear form a(v, u) and linear form L(v) for
-# Poisson's equation in system form (vector-valued).
-from ufl import (Coefficient, FunctionSpace, Mesh, TestFunction, TrialFunction, VectorElement, dot, dx, grad, inner,
-                 triangle)
+# The bilinear form for the nonlinear term in the
+# Navier-Stokes equations with fixed convective velocity.
+from ufl import (
+    Coefficient,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TrialFunction,
+    dot,
+    dx,
+    grad,
+    tetrahedron,
+)
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
-cell = triangle
-element = VectorElement("Lagrange", cell, 1)
-domain = Mesh(VectorElement("Lagrange", cell, 1))
+cell = tetrahedron
+element = FiniteElement("Lagrange", cell, 1, (3,), identity_pullback, H1)
+domain = Mesh(FiniteElement("Lagrange", cell, 1, (3,), identity_pullback, H1))
 space = FunctionSpace(domain, element)
 
 v = TestFunction(space)
 u = TrialFunction(space)
-f = Coefficient(space)
+w = Coefficient(space)
 
-a = inner(grad(v), grad(u)) * dx
-L = dot(v, f) * dx
+Du = grad(u)
+a = dot(dot(w, Du), v) * dx
```

### Comparing `fenics-ufl-2023.2.0/demo/QuadratureElement.py` & `fenics_ufl-2024.1.0.post0/demo/_TensorProductElement.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2008 Kristian B. Oelgaard
+# Copyright (C) 2012 Marie E. Rognes (meg@simula.no)
 #
 # This file is part of UFL.
 #
 # UFL is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,34 +11,41 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with UFL. If not, see <http://www.gnu.org/licenses/>.
 #
-# First added:  2008-03-31
-# Last changed: 2008-03-31
-#
-# The linearised bilinear form a(u,v) and linear form L(v) for
-# the nonlinear equation - div (1+u) grad u = f (non-linear Poisson)
-from ufl import (Coefficient, FiniteElement, FunctionSpace, Mesh, TestFunction, TrialFunction, VectorElement, dot, dx,
-                 grad, i, triangle)
+# First added:  2012-08-16
+# Last changed: 2012-08-16
+from ufl import (
+    FunctionSpace,
+    Mesh,
+    TensorProductElement,
+    TestFunction,
+    TrialFunction,
+    dx,
+    interval,
+    tetrahedron,
+    triangle,
+)
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1, L2
 
-element = FiniteElement("Lagrange", triangle, 2)
-domain = Mesh(VectorElement("Lagrange", triangle, 1))
-space = FunctionSpace(domain, element)
+V0 = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+V1 = FiniteElement("DG", interval, 0, (), identity_pullback, L2)
+V2 = FiniteElement("DG", tetrahedron, 0, (), identity_pullback, L2)
 
-QE = FiniteElement("Quadrature", triangle, 2, quad_scheme="default")
-sig = VectorElement("Quadrature", triangle, 1, quad_scheme="default")
+V = TensorProductElement(V0, V1, V2)
 
-qe_space = FunctionSpace(domain, QE)
-sig_space = FunctionSpace(domain, sig)
+c0 = FiniteElement("CG", triangle, 1)
+c1 = FiniteElement("CG", interval, 1)
+c2 = FiniteElement("CG", tetrahedron, 1)
+domain = Mesh(TensorProductElement(c0, c1, c2))
+space = FunctionSpace(domain, V)
 
-v = TestFunction(space)
 u = TrialFunction(space)
-u0 = Coefficient(space)
-C = Coefficient(qe_space)
-sig0 = Coefficient(sig_space)
-f = Coefficient(space)
+v = TestFunction(space)
 
-a = v.dx(i) * C * u.dx(i) * dx(metadata={"quadrature_degree": 2}) + v.dx(i) * 2 * u0 * u * u0.dx(i) * dx
-L = v * f * dx - dot(grad(v), sig0) * dx(metadata={"quadrature_degree": 1})
+dxxx = dx * dx * dx
+a = u * v * dxxx
```

### Comparing `fenics-ufl-2023.2.0/demo/RestrictedElement.py` & `fenics_ufl-2024.1.0.post0/demo/SubDomains.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2009 Kristian B. Oelgaard
+# Copyright (C) 2008 Anders Logg and Kristian B. Oelgaard
 #
 # This file is part of UFL.
 #
 # UFL is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,19 +11,29 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with UFL. If not, see <http://www.gnu.org/licenses/>.
 #
-# Restriction of a finite element.
-# The below syntax show how one can restrict a higher order Lagrange element
-# to only take into account those DOFs that live on the facets.
-from ufl import FiniteElement, FunctionSpace, Mesh, TestFunction, TrialFunction, VectorElement, avg, dS, ds, triangle
+# This simple example illustrates how forms can be defined on different sub domains.
+# It is supported for all three integral types.
+from ufl import FunctionSpace, Mesh, TestFunction, TrialFunction, dS, ds, dx, tetrahedron
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
-# Restricted element
-CG_R = FiniteElement("Lagrange", triangle, 4)["facet"]
-domain = Mesh(VectorElement("Lagrange", triangle, 1))
-space = FunctionSpace(domain, CG_R)
-u_r = TrialFunction(space)
-v_r = TestFunction(space)
-a = avg(v_r) * avg(u_r) * dS + v_r * u_r * ds
+element = FiniteElement("Lagrange", tetrahedron, 1, (), identity_pullback, H1)
+domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
+space = FunctionSpace(domain, element)
+
+v = TestFunction(space)
+u = TrialFunction(space)
+
+a = (
+    v * u * dx(0)
+    + 10.0 * v * u * dx(1)
+    + v * u * ds(0)
+    + 2.0 * v * u * ds(1)
+    + v("+") * u("+") * dS(0)
+    + 4.3 * v("+") * u("+") * dS(1)
+)
```

### Comparing `fenics-ufl-2023.2.0/demo/Stokes.py` & `fenics_ufl-2024.1.0.post0/demo/StokesEquation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2005-2007 Anders Logg
+# Copyright (C) 2005-2009 Anders Logg and Harish Narayanan
 #
 # This file is part of UFL.
 #
 # UFL is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,30 +11,46 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with UFL. If not, see <http://www.gnu.org/licenses/>.
 #
-# Modified by: Martin Sandve Alnes (2009)
-# Date: 2009-03-02
-#
 # The bilinear form a(v, u) and Linear form L(v) for the Stokes
-# equations using a mixed formulation (Taylor-Hood elements).
-from ufl import (Coefficient, FiniteElement, FunctionSpace, Mesh, TestFunctions, TrialFunctions, VectorElement, div,
-                 dot, dx, grad, inner, triangle)
+# equations using a mixed formulation (Taylor-Hood elements) in
+# combination with the lhs() and rhs() operators to extract the
+# bilinear and linear forms from an expression F = 0.
+from ufl import (
+    Coefficient,
+    FunctionSpace,
+    Mesh,
+    TestFunctions,
+    TrialFunctions,
+    div,
+    dot,
+    dx,
+    grad,
+    inner,
+    lhs,
+    rhs,
+    triangle,
+)
+from ufl.finiteelement import FiniteElement, MixedElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 cell = triangle
-P2 = VectorElement("Lagrange", cell, 2)
-P1 = FiniteElement("Lagrange", cell, 1)
-TH = P2 * P1
-domain = Mesh(VectorElement("Lagrange", cell, 1))
+P2 = FiniteElement("Lagrange", cell, 2, (2,), identity_pullback, H1)
+P1 = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+TH = MixedElement([P2, P1])
+domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
 space = FunctionSpace(domain, TH)
 p2_space = FunctionSpace(domain, P2)
 
 (v, q) = TestFunctions(space)
 (u, p) = TrialFunctions(space)
 
 f = Coefficient(p2_space)
 
-a = (inner(grad(v), grad(u)) - div(v) * p + q * div(u)) * dx
-L = dot(v, f) * dx
+F = (inner(grad(v), grad(u)) - div(v) * p + q * div(u)) * dx - dot(v, f) * dx
+a = lhs(F)
+L = rhs(F)
```

### Comparing `fenics-ufl-2023.2.0/demo/StokesEquation.py` & `fenics_ufl-2024.1.0.post0/demo/TensorWeightedPoisson.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2005-2009 Anders Logg and Harish Narayanan
+# Copyright (C) 2005-2007 Anders Logg
 #
 # This file is part of UFL.
 #
 # UFL is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,30 +11,35 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with UFL. If not, see <http://www.gnu.org/licenses/>.
 #
-# The bilinear form a(v, u) and Linear form L(v) for the Stokes
-# equations using a mixed formulation (Taylor-Hood elements) in
-# combination with the lhs() and rhs() operators to extract the
-# bilinear and linear forms from an expression F = 0.
-from ufl import (Coefficient, FiniteElement, FunctionSpace, Mesh, TestFunctions, TrialFunctions, VectorElement, div,
-                 dot, dx, grad, inner, lhs, rhs, triangle)
+# The bilinear form a(v, u) and linear form L(v) for
+# tensor-weighted Poisson's equation.
+from ufl import (
+    Coefficient,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TrialFunction,
+    dx,
+    grad,
+    inner,
+    triangle,
+)
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1, L2
 
-cell = triangle
-P2 = VectorElement("Lagrange", cell, 2)
-P1 = FiniteElement("Lagrange", cell, 1)
-TH = P2 * P1
-domain = Mesh(VectorElement("Lagrange", cell, 1))
-space = FunctionSpace(domain, TH)
-p2_space = FunctionSpace(domain, P2)
+P1 = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+P0 = FiniteElement("Discontinuous Lagrange", triangle, 0, (2, 2), identity_pullback, L2)
+domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
+p1_space = FunctionSpace(domain, P1)
+p0_space = FunctionSpace(domain, P0)
 
-(v, q) = TestFunctions(space)
-(u, p) = TrialFunctions(space)
+v = TestFunction(p1_space)
+u = TrialFunction(p1_space)
+C = Coefficient(p0_space)
 
-f = Coefficient(p2_space)
-
-F = (inner(grad(v), grad(u)) - div(v) * p + q * div(u)) * dx - dot(v, f) * dx
-a = lhs(F)
-L = rhs(F)
+a = inner(grad(v), C * grad(u)) * dx
```

### Comparing `fenics-ufl-2023.2.0/demo/SubDomain.py` & `fenics_ufl-2024.1.0.post0/demo/NeumannProblem.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2008 Anders Logg
+# Copyright (C) 2006-2007 Anders Logg
 #
 # This file is part of UFL.
 #
 # UFL is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,21 +11,36 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with UFL. If not, see <http://www.gnu.org/licenses/>.
 #
-# This example illustrates how to define a form over a
-# given subdomain of a mesh, in this case a functional.
-from ufl import (Coefficient, FiniteElement, FunctionSpace, Mesh, TestFunction, TrialFunction, VectorElement, ds, dx,
-                 tetrahedron)
+# The bilinear form a(v, u) and linear form L(v) for
+# Poisson's equation with Neumann boundary conditions.
+from ufl import (
+    Coefficient,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TrialFunction,
+    ds,
+    dx,
+    grad,
+    inner,
+    triangle,
+)
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
-element = FiniteElement("CG", tetrahedron, 1)
-domain = Mesh(VectorElement("Lagrange", tetrahedron, 1))
+element = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
 space = FunctionSpace(domain, element)
 
 v = TestFunction(space)
 u = TrialFunction(space)
 f = Coefficient(space)
+g = Coefficient(space)
 
-M = f * dx(2) + f * ds(5)
+a = inner(grad(v), grad(u)) * dx
+L = inner(v, f) * dx + inner(v, g) * ds
```

### Comparing `fenics-ufl-2023.2.0/demo/TensorWeightedPoisson.py` & `fenics_ufl-2024.1.0.post0/demo/MixedPoisson.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2005-2007 Anders Logg
+# Copyright (C) 2006-2009 Anders Logg and Marie Rognes
 #
 # This file is part of UFL.
 #
 # UFL is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,23 +11,46 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with UFL. If not, see <http://www.gnu.org/licenses/>.
 #
+# Modified by Martin Sandve Alnes, 2009
+#
+# Last changed: 2009-01-12
+#
 # The bilinear form a(v, u) and linear form L(v) for
-# tensor-weighted Poisson's equation.
-from ufl import (Coefficient, FiniteElement, FunctionSpace, Mesh, TensorElement, TestFunction, TrialFunction,
-                 VectorElement, dx, grad, inner, triangle)
+# a mixed formulation of Poisson's equation with BDM
+# (Brezzi-Douglas-Marini) elements.
+#
+from ufl import (
+    Coefficient,
+    FunctionSpace,
+    Mesh,
+    TestFunctions,
+    TrialFunctions,
+    div,
+    dot,
+    dx,
+    triangle,
+)
+from ufl.finiteelement import FiniteElement, MixedElement
+from ufl.pullback import contravariant_piola, identity_pullback
+from ufl.sobolevspace import H1, HDiv
+
+cell = triangle
+BDM1 = FiniteElement("Brezzi-Douglas-Marini", cell, 1, (2,), contravariant_piola, HDiv)
+DG0 = FiniteElement("Discontinuous Lagrange", cell, 0, (), identity_pullback, H1)
+
+element = MixedElement([BDM1, DG0])
+domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
+space = FunctionSpace(domain, element)
+dg0_space = FunctionSpace(domain, DG0)
 
-P1 = FiniteElement("Lagrange", triangle, 1)
-P0 = TensorElement("Discontinuous Lagrange", triangle, 0, shape=(2, 2))
-domain = Mesh(VectorElement("Lagrange", triangle, 1))
-p1_space = FunctionSpace(domain, P1)
-p0_space = FunctionSpace(domain, P0)
+(tau, w) = TestFunctions(space)
+(sigma, u) = TrialFunctions(space)
 
-v = TestFunction(p1_space)
-u = TrialFunction(p1_space)
-C = Coefficient(p0_space)
+f = Coefficient(dg0_space)
 
-a = inner(grad(v), C * grad(u)) * dx
+a = (dot(tau, sigma) - div(tau) * u + w * div(sigma)) * dx
+L = w * f * dx
```

### Comparing `fenics-ufl-2023.2.0/doc/man/man1/ufl-analyse.1.gz` & `fenics_ufl-2024.1.0.post0/doc/man/man1/ufl-analyse.1.gz`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/doc/man/man1/ufl-convert.1.gz` & `fenics_ufl-2024.1.0.post0/doc/man/man1/ufl-convert.1.gz`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/doc/man/man1/ufl-version.1.gz` & `fenics_ufl-2024.1.0.post0/doc/man/man1/ufl-version.1.gz`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/doc/man/man1/ufl2py.1.gz` & `fenics_ufl-2024.1.0.post0/doc/man/man1/ufl2py.1.gz`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/doc/sphinx/Makefile` & `fenics_ufl-2024.1.0.post0/doc/sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/doc/sphinx/README` & `fenics_ufl-2024.1.0.post0/doc/sphinx/README`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/doc/sphinx/source/conf.py` & `fenics_ufl-2024.1.0.post0/doc/sphinx/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,271 +14,278 @@
 
 import datetime
 import importlib.metadata
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-#sys.path.insert(0, os.path.abspath('.'))
+# sys.path.insert(0, os.path.abspath('.'))
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
-#needs_sphinx = '1.0'
+# needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.doctest',
-    'sphinx.ext.coverage',
-    'sphinx.ext.mathjax',
-    'sphinx.ext.viewcode',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.doctest",
+    "sphinx.ext.coverage",
+    "sphinx.ext.mathjax",
+    "sphinx.ext.viewcode",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
-#source_encoding = 'utf-8-sig'
+# source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'Unified Form Language (UFL)'
+project = "Unified Form Language (UFL)"
 this_year = datetime.date.today().year
-copyright = u'%s, FEniCS Project' % this_year
-author = u'FEniCS Project'
+copyright = "%s, FEniCS Project" % this_year
+author = "FEniCS Project"
 
 version = importlib.metadata.version("fenics-ufl")
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 exclude_patterns = []
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
-#default_role = None
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
-#keep_warnings = False
+# keep_warnings = False
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-#html_theme = 'alabaster'
+# html_theme = 'alabaster'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+# html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
+# html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-#html_title = None
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+# html_logo = None
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = None
+# html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 # html_static_path = ['_static']
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
-#html_extra_path = []
+# html_extra_path = []
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
+# html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
+# html_sidebars = {}
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_domain_indices = True
+# html_domain_indices = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
+# html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-#html_show_sphinx = True
+# html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-#html_show_copyright = True
+# html_show_copyright = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = None
+# html_file_suffix = None
 
 # Language to be used for generating the HTML full-text search index.
 # Sphinx supports the following languages:
 #   'da', 'de', 'en', 'es', 'fi', 'fr', 'hu', 'it', 'ja'
 #   'nl', 'no', 'pt', 'ro', 'ru', 'sv', 'tr'
-#html_search_language = 'en'
+# html_search_language = 'en'
 
 # A dictionary with options for the search language support, empty by default.
 # Now only 'ja' uses this config value
-#html_search_options = {'type': 'default'}
+# html_search_options = {'type': 'default'}
 
 # The name of a javascript file (relative to the configuration directory) that
 # implements a search results scorer. If empty, the default will be used.
-#html_search_scorer = 'scorer.js'
+# html_search_scorer = 'scorer.js'
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'UnifiedFormLanguageUFLdoc'
+htmlhelp_basename = "UnifiedFormLanguageUFLdoc"
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
-# The paper size ('letterpaper' or 'a4paper').
-#'papersize': 'letterpaper',
-
-# The font size ('10pt', '11pt' or '12pt').
-#'pointsize': '10pt',
-
-# Additional stuff for the LaTeX preamble.
-#'preamble': '',
-
-# Latex figure (float) alignment
-#'figure_align': 'htbp',
+    # The paper size ('letterpaper' or 'a4paper').
+    #'papersize': 'letterpaper',
+    # The font size ('10pt', '11pt' or '12pt').
+    #'pointsize': '10pt',
+    # Additional stuff for the LaTeX preamble.
+    #'preamble': '',
+    # Latex figure (float) alignment
+    #'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-  (master_doc, 'UnifiedFormLanguageUFL.tex', u'Unified Form Language (UFL) Documentation',
-   u'FEniCS Project', 'manual'),
+    (
+        master_doc,
+        "UnifiedFormLanguageUFL.tex",
+        "Unified Form Language (UFL) Documentation",
+        "FEniCS Project",
+        "manual",
+    ),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
-#latex_logo = None
+# latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
-#latex_use_parts = False
+# latex_use_parts = False
 
 # If true, show page references after internal links.
-#latex_show_pagerefs = False
+# latex_show_pagerefs = False
 
 # If true, show URL addresses after external links.
-#latex_show_urls = False
+# latex_show_urls = False
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_domain_indices = True
+# latex_domain_indices = True
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    (master_doc, 'unifiedformlanguageufl', u'Unified Form Language (UFL) Documentation',
-     [author], 1)
+    (master_doc, "unifiedformlanguageufl", "Unified Form Language (UFL) Documentation", [author], 1)
 ]
 
 # If true, show URL addresses after external links.
-#man_show_urls = False
+# man_show_urls = False
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-  (master_doc, 'UnifiedFormLanguageUFL', u'Unified Form Language (UFL) Documentation',
-   author, 'UnifiedFormLanguageUFL', 'One line description of project.',
-   'Miscellaneous'),
+    (
+        master_doc,
+        "UnifiedFormLanguageUFL",
+        "Unified Form Language (UFL) Documentation",
+        author,
+        "UnifiedFormLanguageUFL",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
 
 # Documents to append as an appendix to all manuals.
-#texinfo_appendices = []
+# texinfo_appendices = []
 
 # If false, no module index is generated.
-#texinfo_domain_indices = True
+# texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
-#texinfo_show_urls = 'footnote'
+# texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
-#texinfo_no_detailmenu = False
+# texinfo_no_detailmenu = False
```

### Comparing `fenics-ufl-2023.2.0/doc/sphinx/source/index.rst` & `fenics_ufl-2024.1.0.post0/doc/sphinx/source/index.rst`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/doc/sphinx/source/installation.rst` & `fenics_ufl-2024.1.0.post0/doc/sphinx/source/installation.rst`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/doc/sphinx/source/manual/algorithms.rst` & `fenics_ufl-2024.1.0.post0/doc/sphinx/source/manual/algorithms.rst`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/doc/sphinx/source/manual/examples.rst` & `fenics_ufl-2024.1.0.post0/doc/sphinx/source/manual/examples.rst`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/doc/sphinx/source/manual/form_language.rst` & `fenics_ufl-2024.1.0.post0/doc/sphinx/source/manual/form_language.rst`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/doc/sphinx/source/manual/internal_representation.rst` & `fenics_ufl-2024.1.0.post0/doc/sphinx/source/manual/internal_representation.rst`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/doc/sphinx/source/manual/introduction.rst` & `fenics_ufl-2024.1.0.post0/doc/sphinx/source/manual/introduction.rst`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/doc/sphinx/source/releases/next.rst` & `fenics_ufl-2024.1.0.post0/doc/sphinx/source/releases/next.rst`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/doc/sphinx/source/releases/v1.6.0.rst` & `fenics_ufl-2024.1.0.post0/doc/sphinx/source/releases/v1.6.0.rst`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/doc/sphinx/source/releases/v2016.1.0.rst` & `fenics_ufl-2024.1.0.post0/doc/sphinx/source/releases/v2016.1.0.rst`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/doc/sphinx/source/releases/v2016.2.0.rst` & `fenics_ufl-2024.1.0.post0/doc/sphinx/source/releases/v2016.2.0.rst`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/doc/sphinx/source/releases/v2017.1.0.rst` & `fenics_ufl-2024.1.0.post0/doc/sphinx/source/releases/v2017.1.0.rst`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/doc/sphinx/source/releases/v2017.2.0.rst` & `fenics_ufl-2024.1.0.post0/doc/sphinx/source/releases/v2017.2.0.rst`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/fenics_ufl.egg-info/PKG-INFO` & `fenics_ufl-2024.1.0.post0/fenics_ufl.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,93 +1,67 @@
 Metadata-Version: 2.1
 Name: fenics-ufl
-Version: 2023.2.0
+Version: 2024.1.0.post0
 Summary: Unified Form Language
-Home-page: https://github.com/FEniCS/ufl
-Author: FEniCS Project Contributors
-Maintainer: FEniCS Project Steering Council
-License: LGPL-3.0-or-later
-Project-URL: Homepage, https://fenicsproject.org
-Project-URL: Documentation, https://fenics.readthedocs.io/projects/ufl
-Project-URL: Issues, https://github.com/FEniCS/ufl/issues
-Project-URL: Funding, https://numfocus.org/donate
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
+Author: UFL contributors
+Maintainer: FEniCS Steering Council
+Maintainer-email: fenics-steering-council@googlegroups.com
+Project-URL: homepage, https://fenicsproject.org
+Project-URL: repository, https://github.com/fenics/ufl.git
+Project-URL: documentation, https://docs.fenicsproject.org
+Project-URL: issues, https://github.com/FEniCS/ufl/issues
+Project-URL: funding, https://numfocus.org/donate
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
 License-File: AUTHORS
 Requires-Dist: numpy
+Provides-Extra: lint
+Requires-Dist: ruff; extra == "lint"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
-Provides-Extra: lint
-Requires-Dist: flake8; extra == "lint"
-Requires-Dist: pydocstyle[toml]; extra == "lint"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: ci
-Requires-Dist: coverage; extra == "ci"
 Requires-Dist: coveralls; extra == "ci"
+Requires-Dist: coverage; extra == "ci"
 Requires-Dist: pytest-cov; extra == "ci"
 Requires-Dist: pytest-xdist; extra == "ci"
 Requires-Dist: fenics-ufl[docs]; extra == "ci"
 Requires-Dist: fenics-ufl[lint]; extra == "ci"
 Requires-Dist: fenics-ufl[test]; extra == "ci"
 
-===========================
-UFL - Unified Form Language
-===========================
+# UFL - Unified Form Language
 
 The Unified Form Language (UFL) is a domain specific language for
 declaration of finite element discretizations of variational forms. More
 precisely, it defines a flexible interface for choosing finite element
 spaces and defining expressions for weak forms in a notation close to
 mathematical notation.
 
 UFL is part of the FEniCS Project. For more information, visit
 https://www.fenicsproject.org
 
-.. image:: https://github.com/FEniCS/ufl/workflows/UFL%20CI/badge.svg
-   :target: https://github.com/FEniCS/ufl/workflows/UFL%20CI
-.. image:: https://coveralls.io/repos/github/FEniCS/ufl/badge.svg?branch=master
-   :target: https://coveralls.io/github/FEniCS/ufl?branch=master
-   :alt: Coverage Status
-.. image:: https://readthedocs.org/projects/fenics-ufl/badge/?version=latest
-   :target: https://fenics.readthedocs.io/projects/ufl/en/latest/?badge=latest
-   :alt: Documentation Status
-
-Documentation
-=============
-
-Documentation can be viewed at https://fenics-ufl.readthedocs.org/.
-
-License
-=======
-
-  This program is free software: you can redistribute it and/or modify
-  it under the terms of the GNU Lesser General Public License as published by
-  the Free Software Foundation, either version 3 of the License, or
-  (at your option) any later version.
-
-  This program is distributed in the hope that it will be useful,
-  but WITHOUT ANY WARRANTY; without even the implied warranty of
-  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-  GNU Lesser General Public License for more details.
+[![UFL CI](https://github.com/FEniCS/ufl/workflows/UFL%20CI/badge.svg)](https://github.com/FEniCS/ufl/workflows/UFL%20CI)
+[![Coverage Status](https://coveralls.io/repos/github/FEniCS/ufl/badge.svg?branch=master)](https://coveralls.io/github/FEniCS/ufl?branch=master)
+
+## Documentation
+
+Documentation can be viewed at https://docs.fenicsproject.org
+
+## License
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU Lesser General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+GNU Lesser General Public License for more details.
 
-  You should have received a copy of the GNU Lesser General Public License
-  along with this program. If not, see <https://www.gnu.org/licenses/>.
+You should have received a copy of the GNU Lesser General Public License
+along with this program. If not, see <https://www.gnu.org/licenses/>.
```

### Comparing `fenics-ufl-2023.2.0/fenics_ufl.egg-info/SOURCES.txt` & `fenics_ufl-2024.1.0.post0/fenics_ufl.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 AUTHORS
 COPYING
 COPYING.LESSER
-ChangeLog.rst
 MANIFEST.in
-README.rst
+README.md
 pyproject.toml
-setup.cfg
 demo/Constant.py
 demo/ConvectionJacobi.py
 demo/ConvectionJacobi2.py
 demo/ConvectionVector.py
 demo/Elasticity.py
 demo/EnergyNorm.py
 demo/Equation.py
 demo/ExplicitConvection.py
-demo/FEEC.py
 demo/FunctionOperators.py
 demo/H1norm.py
 demo/HarmonicMap.py
 demo/HarmonicMap2.py
 demo/Heat.py
 demo/HornSchunck.py
 demo/HyperElasticity.py
@@ -37,15 +34,14 @@
 demo/P5tri.py
 demo/Poisson.py
 demo/PoissonDG.py
 demo/PoissonSystem.py
 demo/PowAD.py
 demo/ProjectionSystem.py
 demo/QuadratureElement.py
-demo/RestrictedElement.py
 demo/Stiffness.py
 demo/StiffnessAD.py
 demo/Stokes.py
 demo/StokesEquation.py
 demo/SubDomain.py
 demo/SubDomains.py
 demo/TensorWeightedPoisson.py
@@ -77,47 +73,43 @@
 doc/sphinx/source/releases/v2017.1.0.rst
 doc/sphinx/source/releases/v2017.2.0.rst
 doc/sphinx/source/releases/v2018.1.0.rst
 doc/sphinx/source/releases/v2019.1.0.rst
 fenics_ufl.egg-info/PKG-INFO
 fenics_ufl.egg-info/SOURCES.txt
 fenics_ufl.egg-info/dependency_links.txt
-fenics_ufl.egg-info/not-zip-safe
 fenics_ufl.egg-info/requires.txt
 fenics_ufl.egg-info/top_level.txt
 test/conftest.py
 test/mockobjects.py
 test/test_algorithms.py
 test/test_analyse_demos.py
 test/test_apply_algebra_lowering.py
 test/test_apply_function_pullbacks.py
 test/test_apply_restrictions.py
 test/test_arithmetic.py
 test/test_automatic_differentiation.py
-test/test_book_snippets.py
 test/test_cell.py
 test/test_change_to_local.py
 test/test_change_to_reference_frame.py
 test/test_check_arities.py
 test/test_classcoverage.py
 test/test_complex.py
 test/test_conditionals.py
 test/test_degree_estimation.py
 test/test_derivative.py
 test/test_diff.py
 test/test_domains.py
 test/test_duals.py
-test/test_elements.py
 test/test_equals.py
 test/test_evaluate.py
 test/test_expand_indices.py
 test/test_external_operator.py
 test/test_ffcforms.py
 test/test_form.py
-test/test_grad.py
 test/test_illegal.py
 test/test_indexing.py
 test/test_indices.py
 test/test_interpolate.py
 test/test_lhs_rhs.py
 test/test_literals.py
 test/test_measures.py
@@ -152,14 +144,15 @@
 ufl/differentiation.py
 ufl/domain.py
 ufl/duals.py
 ufl/equation.py
 ufl/exprcontainers.py
 ufl/exprequals.py
 ufl/exproperators.py
+ufl/finiteelement.py
 ufl/form.py
 ufl/formoperators.py
 ufl/functionspace.py
 ufl/geometry.py
 ufl/index_combination_utils.py
 ufl/indexed.py
 ufl/indexsum.py
@@ -168,14 +161,15 @@
 ufl/matrix.py
 ufl/measure.py
 ufl/objects.py
 ufl/operators.py
 ufl/permutation.py
 ufl/precedence.py
 ufl/protocols.py
+ufl/pullback.py
 ufl/referencevalue.py
 ufl/restriction.py
 ufl/sobolevspace.py
 ufl/sorting.py
 ufl/split_functions.py
 ufl/tensoralgebra.py
 ufl/tensors.py
@@ -195,15 +189,14 @@
 ufl/algorithms/check_restrictions.py
 ufl/algorithms/checks.py
 ufl/algorithms/comparison_checker.py
 ufl/algorithms/compute_form_data.py
 ufl/algorithms/coordinate_derivative_helpers.py
 ufl/algorithms/domain_analysis.py
 ufl/algorithms/estimate_degrees.py
-ufl/algorithms/expand_compounds.py
 ufl/algorithms/expand_indices.py
 ufl/algorithms/formdata.py
 ufl/algorithms/formfiles.py
 ufl/algorithms/formsplitter.py
 ufl/algorithms/formtransformations.py
 ufl/algorithms/map_integrands.py
 ufl/algorithms/remove_complex_nodes.py
@@ -225,24 +218,14 @@
 ufl/core/terminal.py
 ufl/core/ufl_id.py
 ufl/core/ufl_type.py
 ufl/corealg/__init__.py
 ufl/corealg/map_dag.py
 ufl/corealg/multifunction.py
 ufl/corealg/traversal.py
-ufl/finiteelement/__init__.py
-ufl/finiteelement/brokenelement.py
-ufl/finiteelement/elementlist.py
-ufl/finiteelement/enrichedelement.py
-ufl/finiteelement/finiteelement.py
-ufl/finiteelement/finiteelementbase.py
-ufl/finiteelement/hdivcurl.py
-ufl/finiteelement/mixedelement.py
-ufl/finiteelement/restrictedelement.py
-ufl/finiteelement/tensorproductelement.py
 ufl/formatting/__init__.py
 ufl/formatting/ufl2unicode.py
 ufl/utils/__init__.py
 ufl/utils/counted.py
 ufl/utils/formatting.py
 ufl/utils/indexflattening.py
 ufl/utils/sequences.py
```

### Comparing `fenics-ufl-2023.2.0/test/conftest.py` & `fenics_ufl-2024.1.0.post0/test/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import ufl
 from ufl import as_ufl, dx, inner
 from ufl.algorithms import compute_form_data
 
 
 class Tester:
-
     def assertTrue(self, a):
         assert a
 
     def assertFalse(self, a):
         assert not a
 
     def assertEqual(self, a, b):
```

### Comparing `fenics-ufl-2023.2.0/test/mockobjects.py` & `fenics_ufl-2024.1.0.post0/test/mockobjects.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from ufl import Measure, Mesh, triangle
 
 
 class MockMesh:
-
     def __init__(self, ufl_id):
         self._ufl_id = ufl_id
 
     def ufl_id(self):
         return self._ufl_id
 
     def ufl_domain(self):
         return Mesh(triangle, ufl_id=self.ufl_id(), cargo=self)
 
-    def ufl_measure(self, integral_type="dx", subdomain_id="everywhere", metadata=None, subdomain_data=None):
-        return Measure(integral_type, subdomain_id=subdomain_id, metadata=metadata, domain=self,
-                       subdomain_data=subdomain_data)
+    def ufl_measure(
+        self, integral_type="dx", subdomain_id="everywhere", metadata=None, subdomain_data=None
+    ):
+        return Measure(
+            integral_type,
+            subdomain_id=subdomain_id,
+            metadata=metadata,
+            domain=self,
+            subdomain_data=subdomain_data,
+        )
 
 
 class MockMeshFunction:
     """Mock class for the pydolfin compatibility hack for domain data with [] syntax."""
 
     def __init__(self, ufl_id, mesh):
         self._mesh = mesh
@@ -28,9 +34,13 @@
         return self._ufl_id
 
     def mesh(self):
         return self._mesh
 
     def ufl_measure(self, integral_type=None, subdomain_id="everywhere", metadata=None):
         return Measure(
-            integral_type, subdomain_id=subdomain_id, metadata=metadata,
-            domain=self.mesh(), subdomain_data=self)
+            integral_type,
+            subdomain_id=subdomain_id,
+            metadata=metadata,
+            domain=self.mesh(),
+            subdomain_data=self,
+        )
```

### Comparing `fenics-ufl-2023.2.0/test/test_algorithms.py` & `fenics_ufl-2024.1.0.post0/test/test_algorithms.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,57 +2,86 @@
 __date__ = "2008-03-12 -- 2009-01-28"
 
 # Modified by Anders Logg, 2008
 # Modified by Garth N. Wells, 2009
 
 import pytest
 
-from ufl import (Argument, Coefficient, FacetNormal, FiniteElement, FunctionSpace, Mesh, TestFunction, TrialFunction,
-                 VectorElement, adjoint, div, dot, ds, dx, grad, inner, triangle)
-from ufl.algorithms import (expand_derivatives, expand_indices, extract_arguments, extract_coefficients,
-                            extract_elements, extract_unique_elements)
-from ufl.corealg.traversal import post_traversal, pre_traversal, unique_post_traversal, unique_pre_traversal
+from ufl import (
+    Argument,
+    Coefficient,
+    FacetNormal,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TrialFunction,
+    adjoint,
+    div,
+    dot,
+    ds,
+    dx,
+    grad,
+    inner,
+    triangle,
+)
+from ufl.algorithms import (
+    expand_derivatives,
+    expand_indices,
+    extract_arguments,
+    extract_coefficients,
+    extract_elements,
+    extract_unique_elements,
+)
+from ufl.corealg.traversal import (
+    post_traversal,
+    pre_traversal,
+    unique_post_traversal,
+    unique_pre_traversal,
+)
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 # TODO: add more tests, covering all utility algorithms
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def element():
-    return FiniteElement("CG", triangle, 1)
+    return FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def domain():
-    return Mesh(VectorElement("CG", triangle, 1))
+    return Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def space(element, domain):
     return FunctionSpace(domain, element)
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def arguments(space):
     v = TestFunction(space)
     u = TrialFunction(space)
     return (v, u)
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def coefficients(space):
     c = Coefficient(space)
     f = Coefficient(space)
     return (c, f)
 
 
 @pytest.fixture
-def forms(arguments, coefficients, space):
+def forms(arguments, coefficients, domain):
     v, u = arguments
     c, f = coefficients
-    n = FacetNormal(space)
+    n = FacetNormal(domain)
     a = u * v * dx
     L = f * v * dx
     b = u * v * dx(0) + inner(c * grad(u), grad(v)) * dx(1) + dot(n, grad(u)) * v * ds + f * v * dx
     return (a, L, b)
 
 
 def test_extract_arguments_vs_fixture(arguments, forms):
@@ -60,36 +89,34 @@
     assert tuple(arguments[:1]) == tuple(extract_arguments(forms[1]))
 
 
 def test_extract_coefficients_vs_fixture(coefficients, forms):
     assert coefficients == tuple(extract_coefficients(forms[2]))
 
 
-def test_extract_elements_and_extract_unique_elements(forms, domain):
+def test_extract_elements_and_extract_unique_elements(forms, element, domain):
     b = forms[2]
     integrals = b.integrals_by_type("cell")
     integrals[0].integrand()
 
-    element1 = FiniteElement("CG", triangle, 1)
-    element2 = FiniteElement("CG", triangle, 1)
+    element1 = element
+    element2 = element
 
     space1 = FunctionSpace(domain, element1)
     space2 = FunctionSpace(domain, element2)
 
     v = TestFunction(space1)
     u = TrialFunction(space2)
 
     a = u * v * dx
     assert extract_elements(a) == (element1, element2)
     assert extract_unique_elements(a) == (element1,)
 
 
-def test_pre_and_post_traversal(domain):
-    element = FiniteElement("CG", "triangle", 1)
-    space = FunctionSpace(domain, element)
+def test_pre_and_post_traversal(space):
     v = TestFunction(space)
     f = Coefficient(space)
     g = Coefficient(space)
     p1 = f * v
     p2 = g * v
     s = p1 + p2
 
@@ -99,57 +126,59 @@
     assert list(pre_traversal(s)) == [s, p2, g, v, p1, f, v]
     assert list(post_traversal(s)) == [g, v, p2, f, v, p1, s]
     assert list(unique_pre_traversal(s)) == [s, p2, g, v, p1, f]
     assert list(unique_post_traversal(s)) == [v, f, p1, g, p2, s]
 
 
 def test_expand_indices(domain):
-    element = FiniteElement("Lagrange", triangle, 2)
+    element = FiniteElement("Lagrange", triangle, 2, (), identity_pullback, H1)
     space = FunctionSpace(domain, element)
     v = TestFunction(space)
     u = TrialFunction(space)
 
     def evaluate(form):
-        return form.cell_integral()[0].integrand()((), {v: 3, u: 5})  # TODO: How to define values of derivatives?
+        return form.cell_integral()[0].integrand()(
+            (), {v: 3, u: 5}
+        )  # TODO: How to define values of derivatives?
 
     a = div(grad(v)) * u * dx
     # a1 = evaluate(a)
     a = expand_derivatives(a)
     # a2 = evaluate(a)
     a = expand_indices(a)
     # a3 = evaluate(a)
     # TODO: Compare a1, a2, a3
     # TODO: Test something more
 
 
 def test_adjoint(domain):
     cell = triangle
 
-    V1 = FiniteElement("CG", cell, 1)
-    V2 = FiniteElement("CG", cell, 2)
+    V1 = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    V2 = FiniteElement("Lagrange", cell, 2, (), identity_pullback, H1)
 
     s1 = FunctionSpace(domain, V1)
     s2 = FunctionSpace(domain, V2)
 
     u = TrialFunction(s1)
     v = TestFunction(s2)
     assert u.number() > v.number()
 
     u2 = Argument(s1, 2)
     v2 = Argument(s2, 3)
     assert u2.number() < v2.number()
 
     a = u * v * dx
-    a_arg_degrees = [arg.ufl_element().degree() for arg in extract_arguments(a)]
+    a_arg_degrees = [arg.ufl_element().embedded_superdegree for arg in extract_arguments(a)]
     assert a_arg_degrees == [2, 1]
 
     b = adjoint(a)
-    b_arg_degrees = [arg.ufl_element().degree() for arg in extract_arguments(b)]
+    b_arg_degrees = [arg.ufl_element().embedded_superdegree for arg in extract_arguments(b)]
     assert b_arg_degrees == [1, 2]
 
     c = adjoint(a, (u2, v2))
-    c_arg_degrees = [arg.ufl_element().degree() for arg in extract_arguments(c)]
+    c_arg_degrees = [arg.ufl_element().embedded_superdegree for arg in extract_arguments(c)]
     assert c_arg_degrees == [1, 2]
 
     d = adjoint(b)
-    d_arg_degrees = [arg.ufl_element().degree() for arg in extract_arguments(d)]
+    d_arg_degrees = [arg.ufl_element().embedded_superdegree for arg in extract_arguments(d)]
     assert d_arg_degrees == [2, 1]
```

### Comparing `fenics-ufl-2023.2.0/test/test_analyse_demos.py` & `fenics_ufl-2024.1.0.post0/test/test_analyse_demos.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 from ufl.algorithms import load_ufl_file, validate_form
 
 demodir = os.path.abspath(os.path.join(os.path.dirname(__file__), "..", "demo"))
 
 
 def get_demo_filenames():
     filenames = sorted(
-        set(glob(os.path.join(demodir, "*.py")))
-        - set(glob(os.path.join(demodir, "_*.py")))
-        )
+        set(glob(os.path.join(demodir, "*.py"))) - set(glob(os.path.join(demodir, "_*.py")))
+    )
     return filenames
 
 
 @pytest.mark.parametrize("filename", get_demo_filenames())
 def test_demo_files(filename):
     "Check each form in each file with validate_form."
     data = load_ufl_file(filename)
```

### Comparing `fenics-ufl-2023.2.0/test/test_apply_function_pullbacks.py` & `fenics_ufl-2024.1.0.post0/test/test_apply_function_pullbacks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,88 @@
-import numpy
+import numpy as np
 
-from ufl import (Cell, Coefficient, FiniteElement, FunctionSpace, Mesh, TensorElement, VectorElement, as_tensor,
-                 as_vector, dx, indices, triangle)
-from ufl.algorithms.apply_function_pullbacks import apply_single_function_pullbacks
+from ufl import Cell, Coefficient, FunctionSpace, Mesh, as_tensor, as_vector, dx, indices, triangle
 from ufl.algorithms.renumbering import renumber_indices
 from ufl.classes import Jacobian, JacobianDeterminant, JacobianInverse, ReferenceValue
+from ufl.finiteelement import FiniteElement, MixedElement, SymmetricElement
+from ufl.pullback import (
+    contravariant_piola,
+    covariant_piola,
+    double_contravariant_piola,
+    double_covariant_piola,
+    identity_pullback,
+    l2_piola,
+)
+from ufl.sobolevspace import H1, L2, HCurl, HDiv, HDivDiv, HEin
 
 
 def check_single_function_pullback(g, mappings):
     expected = mappings[g]
-    actual = apply_single_function_pullbacks(ReferenceValue(g), g.ufl_element())
+    actual = g.ufl_element().pullback.apply(ReferenceValue(g))
     assert expected.ufl_shape == actual.ufl_shape
-    for idx in numpy.ndindex(actual.ufl_shape):
+    for idx in np.ndindex(actual.ufl_shape):
         rexp = renumber_indices(expected[idx])
         ract = renumber_indices(actual[idx])
         if not rexp == ract:
             print()
             print("In check_single_function_pullback:")
             print("input:")
             print(repr(g))
             print("expected:")
             print(str(rexp))
             print("actual:")
             print(str(ract))
             print("signatures:")
-            print((expected**2*dx).signature())
-            print((actual**2*dx).signature())
+            print((expected**2 * dx).signature())
+            print((actual**2 * dx).signature())
             print()
         assert ract == rexp
 
 
 def test_apply_single_function_pullbacks_triangle3d():
-    triangle3d = Cell("triangle", geometric_dimension=3)
-    cell = triangle3d
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
-
-    UL2 = FiniteElement("DG L2", cell, 1)
-    U0 = FiniteElement("DG", cell, 0)
-    U = FiniteElement("CG", cell, 1)
-    V = VectorElement("CG", cell, 1)
-    Vd = FiniteElement("RT", cell, 1)
-    Vc = FiniteElement("N1curl", cell, 1)
-    T = TensorElement("CG", cell, 1)
-    S = TensorElement("CG", cell, 1, symmetry=True)
-    COV2T = FiniteElement("Regge", cell, 0)   # (0, 2)-symmetric tensors
-    CONTRA2T = FiniteElement("HHJ", cell, 0)  # (2, 0)-symmetric tensors
-
-    Uml2 = UL2*UL2
-    Um = U*U
-    Vm = U*V
-    Vdm = V*Vd
-    Vcm = Vd*Vc
-    Tm = Vc*T
-    Sm = T*S
+    cell = Cell("triangle")
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (3,), identity_pullback, H1))
 
-    Vd0 = Vd*U0  # case from failing ffc demo
+    UL2 = FiniteElement("Discontinuous Lagrange", cell, 1, (), l2_piola, L2)
+    U0 = FiniteElement("Discontinuous Lagrange", cell, 0, (), identity_pullback, L2)
+    U = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    V = FiniteElement("Lagrange", cell, 1, (3,), identity_pullback, H1)
+    Vd = FiniteElement("Raviart-Thomas", cell, 1, (2,), contravariant_piola, HDiv)
+    Vc = FiniteElement("N1curl", cell, 1, (2,), covariant_piola, HCurl)
+    T = FiniteElement("Lagrange", cell, 1, (3, 3), identity_pullback, H1)
+    S = SymmetricElement(
+        {
+            (0, 0): 0,
+            (1, 0): 1,
+            (2, 0): 2,
+            (0, 1): 1,
+            (1, 1): 3,
+            (2, 1): 4,
+            (0, 2): 2,
+            (1, 2): 4,
+            (2, 2): 5,
+        },
+        [FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1) for _ in range(6)],
+    )
+    # (0, 2)-symmetric tensors
+    COV2T = FiniteElement("Regge", cell, 0, (2, 2), double_covariant_piola, HEin)
+    # (2, 0)-symmetric tensors
+    CONTRA2T = FiniteElement("HHJ", cell, 0, (2, 2), double_contravariant_piola, HDivDiv)
+
+    Uml2 = MixedElement([UL2, UL2])
+    Um = MixedElement([U, U])
+    Vm = MixedElement([U, V])
+    Vdm = MixedElement([V, Vd])
+    Vcm = MixedElement([Vd, Vc])
+    Tm = MixedElement([Vc, T])
+    Sm = MixedElement([T, S])
 
-    W = S*T*Vc*Vd*V*U
+    Vd0 = MixedElement([Vd, U0])  # case from failing ffc demo
+
+    W = MixedElement([S, T, Vc, Vd, V, U])
 
     ul2 = Coefficient(FunctionSpace(domain, UL2))
     u = Coefficient(FunctionSpace(domain, U))
     v = Coefficient(FunctionSpace(domain, V))
     vd = Coefficient(FunctionSpace(domain, Vd))
     vc = Coefficient(FunctionSpace(domain, Vc))
     t = Coefficient(FunctionSpace(domain, T))
@@ -113,98 +135,152 @@
     J = Jacobian(domain)
     detJ = JacobianDeterminant(domain)
     Jinv = JacobianInverse(domain)
     # o = CellOrientation(domain)
     i, j, k, l = indices(4)  # noqa: E741
 
     # Contravariant H(div) Piola mapping:
-    M_hdiv = ((1.0/detJ) * J)  # Not applying cell orientation here
+    M_hdiv = (1.0 / detJ) * J  # Not applying cell orientation here
     # Covariant H(curl) Piola mapping: Jinv.T
 
     mappings = {
         # Simple elements should get a simple representation
         ul2: rul2 / detJ,
         u: ru,
         v: rv,
-        vd: as_vector(M_hdiv[i, j]*rvd[j], i),
-        vc: as_vector(Jinv[j, i]*rvc[j], i),
+        vd: as_vector(M_hdiv[i, j] * rvd[j], i),
+        vc: as_vector(Jinv[j, i] * rvc[j], i),
         t: rt,
-        s: as_tensor([[rs[0], rs[1], rs[2]],
-                      [rs[1], rs[3], rs[4]],
-                      [rs[2], rs[4], rs[5]]]),
+        s: as_tensor([[rs[0], rs[1], rs[2]], [rs[1], rs[3], rs[4]], [rs[2], rs[4], rs[5]]]),
         cov2t: as_tensor(Jinv[k, i] * rcov2t[k, l] * Jinv[l, j], (i, j)),
-        contra2t: as_tensor((1.0 / detJ)**2
-                            * J[i, k] * rcontra2t[k, l] * J[j, l], (i, j)),
+        contra2t: as_tensor((1.0 / detJ) ** 2 * J[i, k] * rcontra2t[k, l] * J[j, l], (i, j)),
         # Mixed elements become a bit more complicated
         uml2: as_vector([ruml2[0] / detJ, ruml2[1] / detJ]),
         um: rum,
         vm: rvm,
-        vdm: as_vector([
-            # V
-            rvdm[0],
-            rvdm[1],
-            rvdm[2],
-            # Vd
-            *(as_tensor(M_hdiv[i, j]*as_vector([rvdm[3], rvdm[4]])[j], (i,))[n]
-              for n in range(3))
-        ]), vcm: as_vector([
-            # Vd
-            *(as_tensor(M_hdiv[i, j]*as_vector([rvcm[0], rvcm[1]])[j], (i,))[n]
-              for n in range(3)),
-            # Vc
-            *(as_tensor(Jinv[i, j]*as_vector([rvcm[2], rvcm[3]])[i], (j,))[n]
-              for n in range(3))
-        ]), tm: as_vector([
-            # Vc
-            *(as_tensor(Jinv[i, j]*as_vector([rtm[0], rtm[1]])[i], (j,))[n]
-              for n in range(3)),
-            # T
-            rtm[2], rtm[3], rtm[4],
-            rtm[5], rtm[6], rtm[7],
-            rtm[8], rtm[9], rtm[10],
-        ]), sm: as_vector([
-            # T
-            rsm[0], rsm[1], rsm[2],
-            rsm[3], rsm[4], rsm[5],
-            rsm[6], rsm[7], rsm[8],
-            # S
-            rsm[9], rsm[10], rsm[11],
-            rsm[10], rsm[12], rsm[13],
-            rsm[11], rsm[13], rsm[14],
-        ]),
+        vdm: as_vector(
+            [
+                # V
+                rvdm[0],
+                rvdm[1],
+                rvdm[2],
+                # Vd
+                *(
+                    as_tensor(M_hdiv[i, j] * as_vector([rvdm[3], rvdm[4]])[j], (i,))[n]
+                    for n in range(3)
+                ),
+            ]
+        ),
+        vcm: as_vector(
+            [
+                # Vd
+                *(
+                    as_tensor(M_hdiv[i, j] * as_vector([rvcm[0], rvcm[1]])[j], (i,))[n]
+                    for n in range(3)
+                ),
+                # Vc
+                *(
+                    as_tensor(Jinv[i, j] * as_vector([rvcm[2], rvcm[3]])[i], (j,))[n]
+                    for n in range(3)
+                ),
+            ]
+        ),
+        tm: as_vector(
+            [
+                # Vc
+                *(
+                    as_tensor(Jinv[i, j] * as_vector([rtm[0], rtm[1]])[i], (j,))[n]
+                    for n in range(3)
+                ),
+                # T
+                rtm[2],
+                rtm[3],
+                rtm[4],
+                rtm[5],
+                rtm[6],
+                rtm[7],
+                rtm[8],
+                rtm[9],
+                rtm[10],
+            ]
+        ),
+        sm: as_vector(
+            [
+                # T
+                rsm[0],
+                rsm[1],
+                rsm[2],
+                rsm[3],
+                rsm[4],
+                rsm[5],
+                rsm[6],
+                rsm[7],
+                rsm[8],
+                # S
+                rsm[9],
+                rsm[10],
+                rsm[11],
+                rsm[10],
+                rsm[12],
+                rsm[13],
+                rsm[11],
+                rsm[13],
+                rsm[14],
+            ]
+        ),
         # Case from failing ffc demo:
-        vd0m: as_vector([
-            M_hdiv[0, j]*as_vector([rvd0m[0], rvd0m[1]])[j],
-            M_hdiv[1, j]*as_vector([rvd0m[0], rvd0m[1]])[j],
-            M_hdiv[2, j]*as_vector([rvd0m[0], rvd0m[1]])[j],
-            rvd0m[2]
-        ]),
+        vd0m: as_vector(
+            [
+                M_hdiv[0, j] * as_vector([rvd0m[0], rvd0m[1]])[j],
+                M_hdiv[1, j] * as_vector([rvd0m[0], rvd0m[1]])[j],
+                M_hdiv[2, j] * as_vector([rvd0m[0], rvd0m[1]])[j],
+                rvd0m[2],
+            ]
+        ),
         # This combines it all:
-        w: as_vector([
-            # S
-            rw[0], rw[1], rw[2],
-            rw[1], rw[3], rw[4],
-            rw[2], rw[4], rw[5],
-            # T
-            rw[6], rw[7], rw[8],
-            rw[9], rw[10], rw[11],
-            rw[12], rw[13], rw[14],
-            # Vc
-            *(as_tensor(Jinv[i, j]*as_vector([rw[15], rw[16]])[i], (j,))[n]
-              for n in range(3)),
-            # Vd
-            *(as_tensor(M_hdiv[i, j]*as_vector([rw[17], rw[18]])[j], (i,))[n]
-              for n in range(3)),
-            # V
-            rw[19],
-            rw[20],
-            rw[21],
-            # U
-            rw[22],
-        ]),
+        w: as_vector(
+            [
+                # S
+                rw[0],
+                rw[1],
+                rw[2],
+                rw[1],
+                rw[3],
+                rw[4],
+                rw[2],
+                rw[4],
+                rw[5],
+                # T
+                rw[6],
+                rw[7],
+                rw[8],
+                rw[9],
+                rw[10],
+                rw[11],
+                rw[12],
+                rw[13],
+                rw[14],
+                # Vc
+                *(
+                    as_tensor(Jinv[i, j] * as_vector([rw[15], rw[16]])[i], (j,))[n]
+                    for n in range(3)
+                ),
+                # Vd
+                *(
+                    as_tensor(M_hdiv[i, j] * as_vector([rw[17], rw[18]])[j], (i,))[n]
+                    for n in range(3)
+                ),
+                # V
+                rw[19],
+                rw[20],
+                rw[21],
+                # U
+                rw[22],
+            ]
+        ),
     }
 
     # Check functions of various elements outside a mixed context
     check_single_function_pullback(ul2, mappings)
     check_single_function_pullback(u, mappings)
     check_single_function_pullback(v, mappings)
     check_single_function_pullback(vd, mappings)
@@ -225,33 +301,36 @@
 
     # Check the ridiculous mixed element W combining it all
     check_single_function_pullback(w, mappings)
 
 
 def test_apply_single_function_pullbacks_triangle():
     cell = triangle
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
 
-    Ul2 = FiniteElement("DG L2", cell, 1)
-    U = FiniteElement("CG", cell, 1)
-    V = VectorElement("CG", cell, 1)
-    Vd = FiniteElement("RT", cell, 1)
-    Vc = FiniteElement("N1curl", cell, 1)
-    T = TensorElement("CG", cell, 1)
-    S = TensorElement("CG", cell, 1, symmetry=True)
-
-    Uml2 = Ul2*Ul2
-    Um = U*U
-    Vm = U*V
-    Vdm = V*Vd
-    Vcm = Vd*Vc
-    Tm = Vc*T
-    Sm = T*S
+    Ul2 = FiniteElement("Discontinuous Lagrange", cell, 1, (), l2_piola, L2)
+    U = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    V = FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1)
+    Vd = FiniteElement("Raviart-Thomas", cell, 1, (2,), contravariant_piola, HDiv)
+    Vc = FiniteElement("N1curl", cell, 1, (2,), covariant_piola, HCurl)
+    T = FiniteElement("Lagrange", cell, 1, (2, 2), identity_pullback, H1)
+    S = SymmetricElement(
+        {(0, 0): 0, (0, 1): 1, (1, 0): 1, (1, 1): 2},
+        [FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1) for i in range(3)],
+    )
+
+    Uml2 = MixedElement([Ul2, Ul2])
+    Um = MixedElement([U, U])
+    Vm = MixedElement([U, V])
+    Vdm = MixedElement([V, Vd])
+    Vcm = MixedElement([Vd, Vc])
+    Tm = MixedElement([Vc, T])
+    Sm = MixedElement([T, S])
 
-    W = S*T*Vc*Vd*V*U
+    W = MixedElement([S, T, Vc, Vd, V, U])
 
     ul2 = Coefficient(FunctionSpace(domain, Ul2))
     u = Coefficient(FunctionSpace(domain, U))
     v = Coefficient(FunctionSpace(domain, V))
     vd = Coefficient(FunctionSpace(domain, Vd))
     vc = Coefficient(FunctionSpace(domain, Vc))
     t = Coefficient(FunctionSpace(domain, T))
@@ -293,82 +372,111 @@
     # Geometric quantities we need:
     J = Jacobian(domain)
     detJ = JacobianDeterminant(domain)
     Jinv = JacobianInverse(domain)
     i, j, k, l = indices(4)  # noqa: E741
 
     # Contravariant H(div) Piola mapping:
-    M_hdiv = (1.0/detJ) * J
+    M_hdiv = (1.0 / detJ) * J
     # Covariant H(curl) Piola mapping: Jinv.T
 
     mappings = {
         # Simple elements should get a simple representation
         ul2: rul2 / detJ,
         u: ru,
         v: rv,
-        vd: as_vector(M_hdiv[i, j]*rvd[j], i),
-        vc: as_vector(Jinv[j, i]*rvc[j], i),
+        vd: as_vector(M_hdiv[i, j] * rvd[j], i),
+        vc: as_vector(Jinv[j, i] * rvc[j], i),
         t: rt,
         s: as_tensor([[rs[0], rs[1]], [rs[1], rs[2]]]),
         # Mixed elements become a bit more complicated
         uml2: as_vector([ruml2[0] / detJ, ruml2[1] / detJ]),
         um: rum,
         vm: rvm,
-        vdm: as_vector([
-            # V
-            rvdm[0],
-            rvdm[1],
-            # Vd
-            *(as_tensor(M_hdiv[i, j]*as_vector([rvdm[2], rvdm[3]])[j], (i,))[n]
-              for n in range(2)),
-        ]),
-        vcm: as_vector([
-            # Vd
-            *(as_tensor(M_hdiv[i, j]*as_vector([rvcm[0], rvcm[1]])[j], (i,))[n]
-              for n in range(2)),
-            # Vc
-            *(as_tensor(Jinv[i, j]*as_vector([rvcm[2], rvcm[3]])[i], (j,))[n]
-              for n in range(2)),
-        ]),
-        tm: as_vector([
-            # Vc
-            *(as_tensor(Jinv[i, j]*as_vector([rtm[0], rtm[1]])[i], (j,))[n]
-              for n in range(2)),
-            # T
-            rtm[2], rtm[3],
-            rtm[4], rtm[5],
-        ]),
-        sm: as_vector([
-            # T
-            rsm[0], rsm[1],
-            rsm[2], rsm[3],
-            # S
-            rsm[4], rsm[5],
-            rsm[5], rsm[6],
-        ]),
+        vdm: as_vector(
+            [
+                # V
+                rvdm[0],
+                rvdm[1],
+                # Vd
+                *(
+                    as_tensor(M_hdiv[i, j] * as_vector([rvdm[2], rvdm[3]])[j], (i,))[n]
+                    for n in range(2)
+                ),
+            ]
+        ),
+        vcm: as_vector(
+            [
+                # Vd
+                *(
+                    as_tensor(M_hdiv[i, j] * as_vector([rvcm[0], rvcm[1]])[j], (i,))[n]
+                    for n in range(2)
+                ),
+                # Vc
+                *(
+                    as_tensor(Jinv[i, j] * as_vector([rvcm[2], rvcm[3]])[i], (j,))[n]
+                    for n in range(2)
+                ),
+            ]
+        ),
+        tm: as_vector(
+            [
+                # Vc
+                *(
+                    as_tensor(Jinv[i, j] * as_vector([rtm[0], rtm[1]])[i], (j,))[n]
+                    for n in range(2)
+                ),
+                # T
+                rtm[2],
+                rtm[3],
+                rtm[4],
+                rtm[5],
+            ]
+        ),
+        sm: as_vector(
+            [
+                # T
+                rsm[0],
+                rsm[1],
+                rsm[2],
+                rsm[3],
+                # S
+                rsm[4],
+                rsm[5],
+                rsm[5],
+                rsm[6],
+            ]
+        ),
         # This combines it all:
-        w: as_vector([
-            # S
-            rw[0], rw[1],
-            rw[1], rw[2],
-            # T
-            rw[3], rw[4],
-            rw[5], rw[6],
-            # Vc
-            *(as_tensor(Jinv[i, j]*as_vector([rw[7], rw[8]])[i], (j,))[n]
-              for n in range(2)),
-            # Vd
-            *(as_tensor(M_hdiv[i, j]*as_vector([rw[9], rw[10]])[j], (i,))[n]
-              for n in range(2)),
-            # V
-            rw[11],
-            rw[12],
-            # U
-            rw[13],
-        ]),
+        w: as_vector(
+            [
+                # S
+                rw[0],
+                rw[1],
+                rw[1],
+                rw[2],
+                # T
+                rw[3],
+                rw[4],
+                rw[5],
+                rw[6],
+                # Vc
+                *(as_tensor(Jinv[i, j] * as_vector([rw[7], rw[8]])[i], (j,))[n] for n in range(2)),
+                # Vd
+                *(
+                    as_tensor(M_hdiv[i, j] * as_vector([rw[9], rw[10]])[j], (i,))[n]
+                    for n in range(2)
+                ),
+                # V
+                rw[11],
+                rw[12],
+                # U
+                rw[13],
+            ]
+        ),
     }
 
     # Check functions of various elements outside a mixed context
     check_single_function_pullback(ul2, mappings)
     check_single_function_pullback(u, mappings)
     check_single_function_pullback(v, mappings)
     check_single_function_pullback(vd, mappings)
```

### Comparing `fenics-ufl-2023.2.0/test/test_apply_restrictions.py` & `fenics_ufl-2024.1.0.post0/test/test_apply_restrictions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 from pytest import raises
 
-from ufl import (Coefficient, FacetNormal, FiniteElement, FunctionSpace, Mesh, SpatialCoordinate, VectorElement,
-                 as_tensor, grad, i, triangle)
+from ufl import (
+    Coefficient,
+    FacetNormal,
+    FunctionSpace,
+    Mesh,
+    SpatialCoordinate,
+    as_tensor,
+    grad,
+    i,
+    triangle,
+)
 from ufl.algorithms.apply_restrictions import apply_default_restrictions, apply_restrictions
 from ufl.algorithms.renumbering import renumber_indices
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1, L2
 
 
 def test_apply_restrictions():
     cell = triangle
-    V0 = FiniteElement("DG", cell, 0)
-    V1 = FiniteElement("Lagrange", cell, 1)
-    V2 = FiniteElement("Lagrange", cell, 2)
+    V0 = FiniteElement("Discontinuous Lagrange", cell, 0, (), identity_pullback, L2)
+    V1 = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    V2 = FiniteElement("Lagrange", cell, 2, (), identity_pullback, H1)
 
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     v0_space = FunctionSpace(domain, V0)
     v1_space = FunctionSpace(domain, V1)
     v2_space = FunctionSpace(domain, V2)
 
     f0 = Coefficient(v0_space)
     f = Coefficient(v1_space)
     g = Coefficient(v2_space)
@@ -25,27 +37,30 @@
 
     assert raises(BaseException, lambda: apply_restrictions(f0))
     assert raises(BaseException, lambda: apply_restrictions(grad(f)))
     assert raises(BaseException, lambda: apply_restrictions(n))
 
     # Continuous function gets default restriction if none
     # provided otherwise the user choice is respected
-    assert apply_restrictions(f) == f('+')
-    assert apply_restrictions(f('-')) == f('-')
-    assert apply_restrictions(f('+')) == f('+')
+    assert apply_restrictions(f) == f("+")
+    assert apply_restrictions(f("-")) == f("-")
+    assert apply_restrictions(f("+")) == f("+")
 
     # Propagation to terminals
-    assert apply_restrictions((f + f0)('+')) == f('+') + f0('+')
+    assert apply_restrictions((f + f0)("+")) == f("+") + f0("+")
 
     # Propagation stops at grad
-    assert apply_restrictions(grad(f)('-')) == grad(f)('-')
-    assert apply_restrictions((grad(f)**2)('+')) == grad(f)('+')**2
-    assert apply_restrictions((grad(f) + grad(g))('-')) == (grad(f)('-') + grad(g)('-'))
+    assert apply_restrictions(grad(f)("-")) == grad(f)("-")
+    assert apply_restrictions((grad(f) ** 2)("+")) == grad(f)("+") ** 2
+    assert apply_restrictions((grad(f) + grad(g))("-")) == (grad(f)("-") + grad(g)("-"))
 
     # x is the same from both sides but computed from one of them
-    assert apply_default_restrictions(x) == x('+')
+    assert apply_default_restrictions(x) == x("+")
 
     # n on a linear mesh is opposite pointing from the other side
-    assert apply_restrictions(n('+')) == n('+')
-    assert renumber_indices(apply_restrictions(n('-'))) == renumber_indices(as_tensor(-1*n('+')[i], i))
-    # This would be nicer, but -f is translated to -1*f which is translated to as_tensor(-1*f[i], i).
-    # assert apply_restrictions(n('-')) == -n('+')
+    assert apply_restrictions(n("+")) == n("+")
+    assert renumber_indices(apply_restrictions(n("-"))) == renumber_indices(
+        as_tensor(-1 * n("+")[i], i)
+    )
+    # This would be nicer, but -f is translated to -1*f which is
+    # translated to as_tensor(-1*f[i], i). assert
+    # apply_restrictions(n('-')) == -n('+')
```

### Comparing `fenics-ufl-2023.2.0/test/test_arithmetic.py` & `fenics_ufl-2024.1.0.post0/test/test_arithmetic.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,25 @@
-from ufl import (Identity, Mesh, SpatialCoordinate, VectorElement, as_matrix, as_ufl, as_vector, elem_div, elem_mult,
-                 elem_op, sin, tetrahedron, triangle)
+from ufl import (
+    Identity,
+    Mesh,
+    SpatialCoordinate,
+    as_matrix,
+    as_ufl,
+    as_vector,
+    elem_div,
+    elem_mult,
+    elem_op,
+    sin,
+    tetrahedron,
+    triangle,
+)
 from ufl.classes import ComplexValue, Division, FloatValue, IntValue
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 
 def test_scalar_casting(self):
     f = as_ufl(2.0)
     r = as_ufl(4)
     c = as_ufl(1 + 2j)
     self.assertIsInstance(f, FloatValue)
@@ -12,21 +27,21 @@
     self.assertIsInstance(c, ComplexValue)
     assert float(f) == 2.0
     assert int(r) == 4
     assert complex(c) == 1.0 + 2.0j
 
 
 def test_ufl_float_division(self):
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     d = SpatialCoordinate(domain)[0] / 10.0  # TODO: Use mock instead of x
     self.assertIsInstance(d, Division)
 
 
 def test_float_ufl_division(self):
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     d = 3.14 / SpatialCoordinate(domain)[0]  # TODO: Use mock instead of x
     self.assertIsInstance(d, Division)
 
 
 def test_float_division(self):
     d = as_ufl(20.0) / 10.0
     self.assertIsInstance(d, FloatValue)
@@ -61,39 +76,40 @@
 
     v = as_vector((1, 2, 3))
     u = as_vector((4, 5, 6))
     self.assertEqual(elem_mult(v, u), as_vector((4, 10, 18)))
 
 
 def test_elem_mult_on_matrices(self):
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
 
     A = as_matrix(((1, 2), (3, 4)))
     B = as_matrix(((4, 5), (6, 7)))
     self.assertEqual(elem_mult(A, B), as_matrix(((4, 10), (18, 28))))
 
     x, y = SpatialCoordinate(domain)
     A = as_matrix(((x, y), (3, 4)))
     B = as_matrix(((4, 5), (y, x)))
-    self.assertEqual(elem_mult(A, B), as_matrix(((4*x, 5*y), (3*y, 4*x))))
+    self.assertEqual(elem_mult(A, B), as_matrix(((4 * x, 5 * y), (3 * y, 4 * x))))
 
     x, y = SpatialCoordinate(domain)
     A = as_matrix(((x, y), (3, 4)))
     B = Identity(2)
     self.assertEqual(elem_mult(A, B), as_matrix(((x, 0), (0, 4))))
 
 
 def test_elem_div(self):
-    domain = Mesh(VectorElement("Lagrange", tetrahedron, 1))
+    domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
     x, y, z = SpatialCoordinate(domain)
     A = as_matrix(((x, y, z), (3, 4, 5)))
     B = as_matrix(((7, 8, 9), (z, x, y)))
-    self.assertEqual(elem_div(A, B), as_matrix(((x/7, y/8, z/9), (3/z, 4/x, 5/y))))
+    self.assertEqual(elem_div(A, B), as_matrix(((x / 7, y / 8, z / 9), (3 / z, 4 / x, 5 / y))))
 
 
 def test_elem_op(self):
-    domain = Mesh(VectorElement("Lagrange", tetrahedron, 1))
+    domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
     x, y, z = SpatialCoordinate(domain)
     A = as_matrix(((x, y, z), (3, 4, 5)))
-    self.assertEqual(elem_op(sin, A), as_matrix(((sin(x), sin(y), sin(z)),
-                                                 (sin(3), sin(4), sin(5)))))
+    self.assertEqual(
+        elem_op(sin, A), as_matrix(((sin(x), sin(y), sin(z)), (sin(3), sin(4), sin(5))))
+    )
     self.assertEqual(elem_op(sin, A).dx(0).ufl_shape, (2, 3))
```

### Comparing `fenics-ufl-2023.2.0/test/test_automatic_differentiation.py` & `fenics_ufl-2024.1.0.post0/test/test_automatic_differentiation.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,33 +3,98 @@
 These tests should cover the behaviour of the automatic differentiation
 algorithm at a technical level, and are thus implementation specific.
 Other tests check for mathematical correctness of diff and derivative.
 """
 
 import pytest
 
-from ufl import (And, Argument, CellDiameter, CellVolume, Circumradius, Coefficient, Constant, FacetArea, FacetNormal,
-                 FiniteElement, FunctionSpace, Identity, Jacobian, JacobianDeterminant, JacobianInverse,
-                 MaxCellEdgeLength, MaxFacetEdgeLength, Mesh, MinCellEdgeLength, MinFacetEdgeLength, Not, Or,
-                 PermutationSymbol, SpatialCoordinate, TensorElement, VectorElement, acos, as_matrix, as_tensor, as_ufl,
-                 as_vector, asin, atan, bessel_I, bessel_J, bessel_K, bessel_Y, cofac, conditional, cos, cross,
-                 derivative, det, dev, diff, dot, eq, erf, exp, ge, grad, gt, indices, inner, interval, inv, le, ln, lt,
-                 ne, outer, replace, sin, skew, sqrt, sym, tan, tetrahedron, tr, triangle, variable)
+from ufl import (
+    And,
+    Argument,
+    CellDiameter,
+    CellVolume,
+    Circumradius,
+    Coefficient,
+    Constant,
+    FacetArea,
+    FacetNormal,
+    FunctionSpace,
+    Identity,
+    Jacobian,
+    JacobianDeterminant,
+    JacobianInverse,
+    MaxCellEdgeLength,
+    MaxFacetEdgeLength,
+    Mesh,
+    MinCellEdgeLength,
+    MinFacetEdgeLength,
+    Not,
+    Or,
+    PermutationSymbol,
+    SpatialCoordinate,
+    acos,
+    as_matrix,
+    as_tensor,
+    as_ufl,
+    as_vector,
+    asin,
+    atan,
+    bessel_I,
+    bessel_J,
+    bessel_K,
+    bessel_Y,
+    cofac,
+    conditional,
+    cos,
+    cross,
+    derivative,
+    det,
+    dev,
+    diff,
+    dot,
+    eq,
+    erf,
+    exp,
+    ge,
+    grad,
+    gt,
+    indices,
+    inner,
+    interval,
+    inv,
+    le,
+    ln,
+    lt,
+    ne,
+    outer,
+    replace,
+    sin,
+    skew,
+    sqrt,
+    sym,
+    tan,
+    tetrahedron,
+    tr,
+    triangle,
+    variable,
+)
 from ufl.algorithms import expand_derivatives
 from ufl.conditional import Conditional
 from ufl.corealg.traversal import unique_post_traversal
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1, L2
 
 
 class ExpressionCollection(object):
-
     def __init__(self, cell):
         self.cell = cell
-        domain = Mesh(VectorElement("Lagrange", cell, 1))
+        d = cell.topological_dimension()
+        domain = Mesh(FiniteElement("Lagrange", cell, 1, (d,), identity_pullback, H1))
 
-        d = cell.geometric_dimension()
         x = SpatialCoordinate(domain)
         n = FacetNormal(domain)
         c = CellVolume(domain)
         R = Circumradius(domain)
         h = CellDiameter(domain)
         f = FacetArea(domain)
         # s = CellSurfaceArea(domain)
@@ -41,154 +106,194 @@
         detJ = JacobianDeterminant(domain)
         invJ = JacobianInverse(domain)
         # FIXME: Add all new geometry types here!
 
         ident = Identity(d)
         eps = PermutationSymbol(d)
 
-        U = FiniteElement("U", cell, None)
-        V = VectorElement("U", cell, None)
-        W = TensorElement("U", cell, None)
+        U = FiniteElement("Undefined", cell, None, (), identity_pullback, L2)
+        V = FiniteElement("Undefined", cell, None, (d,), identity_pullback, L2)
+        W = FiniteElement("Undefined", cell, None, (d, d), identity_pullback, L2)
 
         u_space = FunctionSpace(domain, U)
         v_space = FunctionSpace(domain, V)
         w_space = FunctionSpace(domain, W)
 
         u = Coefficient(u_space)
         v = Coefficient(v_space)
         w = Coefficient(w_space)
         du = Argument(u_space, 0)
         dv = Argument(v_space, 1)
         dw = Argument(w_space, 2)
 
         class ObjectCollection(object):
             pass
+
         self.shared_objects = ObjectCollection()
         for key, value in list(locals().items()):
             setattr(self.shared_objects, key, value)
 
         self.literals = list(map(as_ufl, [0, 1, 3.14, ident, eps]))
         self.geometry = [x, n, c, R, h, f, mince, maxce, minfe, maxfe, J, detJ, invJ]
         self.functions = [u, du, v, dv, w, dw]
 
         self.terminals = []
         self.terminals += self.literals
         self.terminals += self.geometry
         self.terminals += self.functions
 
-        self.algebra = ([
-            u*2, v*2, w*2,
-            u+2*u, v+2*v, w+2*w,
-            2/u, u/2, v/2, w/2,
-            u**3, 3**u,
-        ])
-        self.mathfunctions = ([
-            abs(u), sqrt(u), exp(u), ln(u),
-            cos(u), sin(u), tan(u), acos(u), asin(u), atan(u),
-            erf(u), bessel_I(1, u), bessel_J(1, u), bessel_K(1, u), bessel_Y(1, u),
-        ])
-        self.variables = ([
-            variable(u), variable(v), variable(w),
-            variable(w*u), 3*variable(w*u),
-        ])
+        self.algebra = [
+            u * 2,
+            v * 2,
+            w * 2,
+            u + 2 * u,
+            v + 2 * v,
+            w + 2 * w,
+            2 / u,
+            u / 2,
+            v / 2,
+            w / 2,
+            u**3,
+            3**u,
+        ]
+        self.mathfunctions = [
+            abs(u),
+            sqrt(u),
+            exp(u),
+            ln(u),
+            cos(u),
+            sin(u),
+            tan(u),
+            acos(u),
+            asin(u),
+            atan(u),
+            erf(u),
+            bessel_I(1, u),
+            bessel_J(1, u),
+            bessel_K(1, u),
+            bessel_Y(1, u),
+        ]
+        self.variables = [
+            variable(u),
+            variable(v),
+            variable(w),
+            variable(w * u),
+            3 * variable(w * u),
+        ]
 
         if d == 1:
             w2 = as_matrix(((u**2,),))
         if d == 2:
-            w2 = as_matrix(((u**2, u**3),
-                            (u**4, u**5)))
+            w2 = as_matrix(((u**2, u**3), (u**4, u**5)))
         if d == 3:
-            w2 = as_matrix(((u**2, u**3, u**4),
-                            (u**4, u**5, u**6),
-                            (u**6, u**7, u**8)))
+            w2 = as_matrix(((u**2, u**3, u**4), (u**4, u**5, u**6), (u**6, u**7, u**8)))
 
         # Indexed,  ListTensor, ComponentTensor, IndexSum
         i, j, k, l = indices(4)  # noqa: E741
-        self.indexing = ([
-                v[0], w[d-1, 0], v[i], w[i, j],
-                v[:], w[0, :], w[:, 0],
-                v[...], w[0, ...], w[..., 0],
-                v[i]*v[j], w[i, 0]*v[j], w[d-1, j]*v[i],
-                v[i]*v[i], w[i, 0]*w[0, i], v[i]*w[0, i],
-                v[j]*w[d-1, j], w[i, i], w[i, j]*w[j, i],
-                as_tensor(v[i]*w[k, 0], (k, i)),
-                as_tensor(v[i]*w[k, 0], (k, i))[:, l],
-                as_tensor(w[i, j]*w[k, l], (k, j, l, i)),
-                as_tensor(w[i, j]*w[k, l], (k, j, l, i))[0, 0, 0, 0],
-                as_vector((u, 2, 3)),
-                as_matrix(((u**2, u**3), (u**4, u**5))),
-                as_vector((u, 2, 3))[i],
-                w2[i, j]*w[i, j],
-        ])
-        self.conditionals = ([
+        self.indexing = [
+            v[0],
+            w[d - 1, 0],
+            v[i],
+            w[i, j],
+            v[:],
+            w[0, :],
+            w[:, 0],
+            v[...],
+            w[0, ...],
+            w[..., 0],
+            v[i] * v[j],
+            w[i, 0] * v[j],
+            w[d - 1, j] * v[i],
+            v[i] * v[i],
+            w[i, 0] * w[0, i],
+            v[i] * w[0, i],
+            v[j] * w[d - 1, j],
+            w[i, i],
+            w[i, j] * w[j, i],
+            as_tensor(v[i] * w[k, 0], (k, i)),
+            as_tensor(v[i] * w[k, 0], (k, i))[:, l],
+            as_tensor(w[i, j] * w[k, l], (k, j, l, i)),
+            as_tensor(w[i, j] * w[k, l], (k, j, l, i))[0, 0, 0, 0],
+            as_vector((u, 2, 3)),
+            as_matrix(((u**2, u**3), (u**4, u**5))),
+            as_vector((u, 2, 3))[i],
+            w2[i, j] * w[i, j],
+        ]
+        self.conditionals = [
             conditional(le(u, 1.0), 1, 0),
             conditional(eq(3.0, u), 1, 0),
             conditional(ne(sin(u), cos(u)), 1, 0),
             conditional(lt(sin(u), cos(u)), 1, 0),
             conditional(ge(sin(u), cos(u)), 1, 0),
             conditional(gt(sin(u), cos(u)), 1, 0),
             conditional(And(lt(u, 3), gt(u, 1)), 1, 0),
             conditional(Or(lt(u, 3), gt(u, 1)), 1, 0),
             conditional(Not(ge(u, 0.0)), 1, 0),
             conditional(le(u, 0.0), 1, 2),
             conditional(Not(ge(u, 0.0)), 1, 2),
             conditional(And(Not(ge(u, 0.0)), lt(u, 1.0)), 1, 2),
             conditional(le(u, 0.0), u**3, ln(u)),
-        ])
-        self.restrictions = [u('+'), u('-'), v('+'), v('-'), w('+'), w('-')]
+        ]
+        self.restrictions = [u("+"), u("-"), v("+"), v("-"), w("+"), w("-")]
         if d > 1:
             i, j = indices(2)
-            self.restrictions += ([
-                v('+')[i]*v('+')[i],
-                v[i]('+')*v[i]('+'),
-                (v[i]*v[i])('+'),
-                (v[i]*v[j])('+')*w[i, j]('+'),
-            ])
+            self.restrictions += [
+                v("+")[i] * v("+")[i],
+                v[i]("+") * v[i]("+"),
+                (v[i] * v[i])("+"),
+                (v[i] * v[j])("+") * w[i, j]("+"),
+            ]
 
         self.noncompounds = []
         self.noncompounds += self.algebra
         self.noncompounds += self.mathfunctions
         self.noncompounds += self.variables
         self.noncompounds += self.indexing
         self.noncompounds += self.conditionals
         self.noncompounds += self.restrictions
 
         if d == 1:
             self.tensorproducts = []
         else:
-            self.tensorproducts = ([
+            self.tensorproducts = [
                 dot(v, v),
                 dot(v, w),
                 dot(w, w),
                 inner(v, v),
                 inner(w, w),
                 outer(v, v),
                 outer(w, v),
                 outer(v, w),
                 outer(w, w),
-            ])
+            ]
 
         if d == 1:
             self.tensoralgebra = []
         else:
-            self.tensoralgebra = ([
-                w.T, sym(w), skew(w), dev(w),
-                det(w), tr(w), cofac(w), inv(w),
-            ])
+            self.tensoralgebra = [
+                w.T,
+                sym(w),
+                skew(w),
+                dev(w),
+                det(w),
+                tr(w),
+                cofac(w),
+                inv(w),
+            ]
 
         if d != 3:
             self.crossproducts = []
         else:
-            self.crossproducts = ([
+            self.crossproducts = [
                 cross(v, v),
-                cross(v, 2*v),
+                cross(v, 2 * v),
                 cross(v, w[0, :]),
                 cross(v, w[:, 1]),
                 cross(w[:, 0], v),
-            ])
+            ]
 
         self.compounds = []
         self.compounds += self.tensorproducts
         self.compounds += self.tensoralgebra
         self.compounds += self.crossproducts
 
         self.all_expressions = []
@@ -213,39 +318,44 @@
     if alt == 0:
         return expand_derivatives(expr)
     elif alt == 1:
         return expand_derivatives(
             expr,
             apply_expand_compounds_before=True,
             apply_expand_compounds_after=False,
-            use_alternative_wrapper_algorithm=True)
+            use_alternative_wrapper_algorithm=True,
+        )
     elif alt == 2:
         return expand_derivatives(
             expr,
             apply_expand_compounds_before=False,
             apply_expand_compounds_after=True,
-            use_alternative_wrapper_algorithm=False)
+            use_alternative_wrapper_algorithm=False,
+        )
     elif alt == 3:
         return expand_derivatives(
             expr,
             apply_expand_compounds_before=False,
             apply_expand_compounds_after=False,
-            use_alternative_wrapper_algorithm=False)
+            use_alternative_wrapper_algorithm=False,
+        )
     elif alt == 4:
         return expand_derivatives(
             expr,
             apply_expand_compounds_before=False,
             apply_expand_compounds_after=False,
-            use_alternative_wrapper_algorithm=True)
+            use_alternative_wrapper_algorithm=True,
+        )
     elif alt == 5:
         return expand_derivatives(
             expr,
             apply_expand_compounds_before=False,
             apply_expand_compounds_after=False,
-            use_alternative_wrapper_algorithm=False)
+            use_alternative_wrapper_algorithm=False,
+        )
 
 
 def _test_no_derivatives_no_change(self, collection):
     for expr in collection:
         before = expr
         after = ad_algorithm(before)
         # print '\n', str(before), '\n', str(after), '\n'
@@ -270,15 +380,17 @@
 
 
 def test_no_derivatives_no_change(self, d_expr):
     d, ex = d_expr
     _test_no_derivatives_no_change(self, ex.noncompounds)
 
 
-def xtest_compounds_no_derivatives_no_change(self, d_expr):  # This test fails with expand_compounds enabled
+def xtest_compounds_no_derivatives_no_change(
+    self, d_expr
+):  # This test fails with expand_compounds enabled
     d, ex = d_expr
     _test_no_derivatives_no_change(self, ex.compounds)
 
 
 def test_zero_derivatives_of_terminals_produce_the_right_types_and_shapes(self, d_expr):
     d, ex = d_expr
     _test_zero_derivatives_of_terminals_produce_the_right_types_and_shapes(self, ex)
@@ -291,21 +403,21 @@
     v = Coefficient(collection.shared_objects.v_space)
     w = Coefficient(collection.shared_objects.w_space)
 
     for t in collection.terminals:
         for var in (u, v, w):
             before = derivative(t, var)  # This will often get preliminary simplified to zero
             after = ad_algorithm(before)
-            expected = 0*t
+            expected = 0 * t
             # print '\n', str(expected), '\n', str(after), '\n', str(before), '\n'
             assert after == expected
 
-            before = derivative(c*t, var)  # This will usually not get simplified to zero
+            before = derivative(c * t, var)  # This will usually not get simplified to zero
             after = ad_algorithm(before)
-            expected = 0*t
+            expected = 0 * t
             # print '\n', str(expected), '\n', str(after), '\n', str(before), '\n'
             assert after == expected
 
 
 def test_zero_diffs_of_terminals_produce_the_right_types_and_shapes(self, d_expr):
     d, ex = d_expr
     _test_zero_diffs_of_terminals_produce_the_right_types_and_shapes(self, ex)
@@ -321,21 +433,21 @@
     vu = variable(u)
     vv = variable(v)
     vw = variable(w)
     for t in collection.terminals:
         for var in (vu, vv, vw):
             before = diff(t, var)  # This will often get preliminary simplified to zero
             after = ad_algorithm(before)
-            expected = 0*outer(t, var)
+            expected = 0 * outer(t, var)
             # print '\n', str(expected), '\n', str(after), '\n', str(before), '\n'
             assert after == expected
 
-            before = diff(c*t, var)  # This will usually not get simplified to zero
+            before = diff(c * t, var)  # This will usually not get simplified to zero
             after = ad_algorithm(before)
-            expected = 0*outer(t, var)
+            expected = 0 * outer(t, var)
             # print '\n', str(expected), '\n', str(after), '\n', str(before), '\n'
             assert after == expected
 
 
 def test_zero_derivatives_of_noncompounds_produce_the_right_types_and_shapes(self, d_expr):
     d, ex = d_expr
     _test_zero_derivatives_of_noncompounds_produce_the_right_types_and_shapes(self, ex)
@@ -349,30 +461,30 @@
     w = Coefficient(collection.shared_objects.w_space)
 
     # for t in chain(collection.noncompounds, collection.compounds):
     # debug = True
     for t in collection.noncompounds:
         for var in (u, v, w):
             if debug:
-                print('\n', 'shapes:   ', t.ufl_shape, var.ufl_shape, '\n')
+                print("\n", "shapes:   ", t.ufl_shape, var.ufl_shape, "\n")
             if debug:
-                print('\n', 't:        ', str(t), '\n')
+                print("\n", "t:        ", str(t), "\n")
             if debug:
-                print('\n', 't ind:    ', str(t.ufl_free_indices), '\n')
+                print("\n", "t ind:    ", str(t.ufl_free_indices), "\n")
             if debug:
-                print('\n', 'var:      ', str(var), '\n')
+                print("\n", "var:      ", str(var), "\n")
             before = derivative(t, var)
             if debug:
-                print('\n', 'before:   ', str(before), '\n')
+                print("\n", "before:   ", str(before), "\n")
             after = ad_algorithm(before)
             if debug:
-                print('\n', 'after:    ', str(after), '\n')
-            expected = 0*t
+                print("\n", "after:    ", str(after), "\n")
+            expected = 0 * t
             if debug:
-                print('\n', 'expected: ', str(expected), '\n')
+                print("\n", "expected: ", str(expected), "\n")
             assert after == expected
 
 
 def test_zero_diffs_of_noncompounds_produce_the_right_types_and_shapes(self, d_expr):
     d, ex = d_expr
     _test_zero_diffs_of_noncompounds_produce_the_right_types_and_shapes(self, ex)
 
@@ -389,21 +501,21 @@
     vw = variable(w)
 
     # for t in chain(collection.noncompounds, collection.compounds):
     for t in collection.noncompounds:
         for var in (vu, vv, vw):
             before = diff(t, var)
             if debug:
-                print('\n', 'before:   ', str(before), '\n')
+                print("\n", "before:   ", str(before), "\n")
             after = ad_algorithm(before)
             if debug:
-                print('\n', 'after:    ', str(after), '\n')
-            expected = 0*outer(t, var)
+                print("\n", "after:    ", str(after), "\n")
+            expected = 0 * outer(t, var)
             if debug:
-                print('\n', 'expected: ', str(expected), '\n')
+                print("\n", "expected: ", str(expected), "\n")
             # print '\n', str(expected), '\n', str(after), '\n', str(before), '\n'
             assert after == expected
 
 
 def test_nonzero_derivatives_of_noncompounds_produce_the_right_types_and_shapes(self, d_expr):
     d, ex = d_expr
     _test_nonzero_derivatives_of_noncompounds_produce_the_right_types_and_shapes(self, ex)
@@ -422,24 +534,24 @@
             # Include d/dx [z ? y: x] but not d/dx [x ? f: z]
             if isinstance(t, Conditional) and (var in unique_post_traversal(t.ufl_operands[0])):
                 if debug:
                     print(("Depends on %s :: %s" % (str(var), str(t))))
                 continue
 
             if debug:
-                print(('\n', '...:   ', t.ufl_shape, var.ufl_shape, '\n'))
+                print(("\n", "...:   ", t.ufl_shape, var.ufl_shape, "\n"))
             before = derivative(t, var)
             if debug:
-                print(('\n', 'before:   ', str(before), '\n'))
+                print(("\n", "before:   ", str(before), "\n"))
             after = ad_algorithm(before)
             if debug:
-                print(('\n', 'after:    ', str(after), '\n'))
-            expected_shape = 0*t
+                print(("\n", "after:    ", str(after), "\n"))
+            expected_shape = 0 * t
             if debug:
-                print(('\n', 'expected_shape: ', str(expected_shape), '\n'))
+                print(("\n", "expected_shape: ", str(expected_shape), "\n"))
             # print '\n', str(expected_shape), '\n', str(after), '\n', str(before), '\n'
 
             if var in unique_post_traversal(t):
                 self.assertEqualTotalShape(after, expected_shape)
                 self.assertNotEqual(after, expected_shape)
             else:
                 assert after == expected_shape
@@ -468,21 +580,21 @@
             if isinstance(t, Conditional) and (var in unique_post_traversal(t.ufl_operands[0])):
                 if debug:
                     print(("Depends on %s :: %s" % (str(var), str(t))))
                 continue
 
             before = diff(t, var)
             if debug:
-                print(('\n', 'before:   ', str(before), '\n'))
+                print(("\n", "before:   ", str(before), "\n"))
             after = ad_algorithm(before)
             if debug:
-                print(('\n', 'after:    ', str(after), '\n'))
-            expected_shape = 0*outer(t, var)  # expected shape, not necessarily value
+                print(("\n", "after:    ", str(after), "\n"))
+            expected_shape = 0 * outer(t, var)  # expected shape, not necessarily value
             if debug:
-                print(('\n', 'expected_shape: ', str(expected_shape), '\n'))
+                print(("\n", "expected_shape: ", str(expected_shape), "\n"))
             # print '\n', str(expected_shape), '\n', str(after), '\n', str(before), '\n'
 
             if var in unique_post_traversal(t):
                 self.assertEqualTotalShape(after, expected_shape)
                 self.assertNotEqual(after, expected_shape)
             else:
                 assert after == expected_shape
@@ -495,16 +607,16 @@
     v = collection.shared_objects.v
     w = collection.shared_objects.w
     for f in (u, v, w):
         before = grad(f)
         after = ad_algorithm(before)
 
         if before.ufl_shape != after.ufl_shape:
-            print(('\n', 'shapes:', before.ufl_shape, after.ufl_shape))
-            print(('\n', str(before), '\n', str(after), '\n'))
+            print(("\n", "shapes:", before.ufl_shape, after.ufl_shape))
+            print(("\n", str(before), "\n", str(after), "\n"))
 
         self.assertEqualTotalShape(before, after)
         if f is u:  # Differing by being wrapped in indexing types
             assert before == after
 
         before = grad(grad(f))
         after = ad_algorithm(before)
@@ -536,28 +648,28 @@
 
         before = derivative(grad(grad(grad(f))), f)
         after = ad_algorithm(before)
         self.assertEqualTotalShape(before, after)
         # assert after == expected
         if 0:
             print()
-            print(('B', f, "::", before))
-            print(('A', f, "::", after))
+            print(("B", f, "::", before))
+            print(("A", f, "::", after))
 
 
 def xtest_derivative_grad_coeff_with_variation_components(self, d_expr):
     d, collection = d_expr
 
     v = collection.shared_objects.v
     w = collection.shared_objects.w
     dv = collection.shared_objects.dv
     dw = collection.shared_objects.dw
     for g, dg in ((v, dv), (w, dw)):
         # Pick a single component
-        ii = (0,)*(len(g.ufl_shape))
+        ii = (0,) * (len(g.ufl_shape))
         f = g[ii]
         df = dg[ii]
 
         before = derivative(grad(g), f, df)
         after = ad_algorithm(before)
         self.assertEqualTotalShape(before, after)
         # assert after == expected
@@ -569,9 +681,9 @@
 
         before = derivative(grad(grad(grad(g))), f, df)
         after = ad_algorithm(before)
         self.assertEqualTotalShape(before, after)
         # assert after == expected
         if 0:
             print()
-            print(('B', f, "::", before))
-            print(('A', f, "::", after))
+            print(("B", f, "::", before))
+            print(("A", f, "::", after))
```

### Comparing `fenics-ufl-2023.2.0/test/test_cell.py` & `fenics_ufl-2024.1.0.post0/test/test_cell.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,8 +81,7 @@
 
 
 def test_tensorproductcell():
     orig = ufl.TensorProductCell(ufl.interval, ufl.interval)
     cell = orig.reconstruct()
     assert cell.sub_cells() == orig.sub_cells()
     assert cell.topological_dimension() == orig.topological_dimension()
-    assert cell.geometric_dimension() == orig.geometric_dimension()
```

### Comparing `fenics-ufl-2023.2.0/test/test_change_to_local.py` & `fenics_ufl-2024.1.0.post0/test/test_change_to_local.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """Tests of the change to local representaiton algorithms."""
 
-from ufl import Coefficient, FiniteElement, FunctionSpace, Mesh, VectorElement, as_tensor, grad, indices, triangle
+from ufl import Coefficient, FunctionSpace, Mesh, as_tensor, grad, indices, triangle
 from ufl.algorithms import change_to_reference_grad
 from ufl.algorithms.renumbering import renumber_indices
 from ufl.classes import JacobianInverse, ReferenceGrad
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 
 def test_change_to_reference_grad():
     cell = triangle
-    domain = Mesh(cell)
-    U = FunctionSpace(domain, FiniteElement("CG", cell, 1))
-    V = FunctionSpace(domain, VectorElement("CG", cell, 1))
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
+    U = FunctionSpace(domain, FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1))
+    V = FunctionSpace(domain, FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     u = Coefficient(U)
     v = Coefficient(V)
     Jinv = JacobianInverse(domain)
     i, j, k = indices(3)
     q, r, s = indices(3)
-    t, = indices(1)
+    (t,) = indices(1)
 
     # Single grad change on a scalar function
     expr = grad(u)
     actual = change_to_reference_grad(expr)
     expected = as_tensor(Jinv[k, i] * ReferenceGrad(u)[k], (i,))
     assert renumber_indices(actual) == renumber_indices(expected)
 
@@ -29,34 +32,40 @@
     actual = change_to_reference_grad(expr)
     expected = as_tensor(Jinv[k, j] * ReferenceGrad(v)[i, k], (i, j))
     assert renumber_indices(actual) == renumber_indices(expected)
 
     # Multiple grads should work fine for affine domains:
     expr = grad(grad(u))
     actual = change_to_reference_grad(expr)
-    expected = as_tensor(
-        Jinv[s, j] * (Jinv[r, i] * ReferenceGrad(ReferenceGrad(u))[r, s]), (i, j))
+    expected = as_tensor(Jinv[s, j] * (Jinv[r, i] * ReferenceGrad(ReferenceGrad(u))[r, s]), (i, j))
     assert renumber_indices(actual) == renumber_indices(expected)
 
     expr = grad(grad(grad(u)))
     actual = change_to_reference_grad(expr)
     expected = as_tensor(
-        Jinv[s, k] * (Jinv[r, j] * (Jinv[q, i] * ReferenceGrad(ReferenceGrad(ReferenceGrad(u)))[q, r, s])), (i, j, k))
+        Jinv[s, k]
+        * (Jinv[r, j] * (Jinv[q, i] * ReferenceGrad(ReferenceGrad(ReferenceGrad(u)))[q, r, s])),
+        (i, j, k),
+    )
     assert renumber_indices(actual) == renumber_indices(expected)
 
     # Multiple grads on a vector valued function
     expr = grad(grad(v))
     actual = change_to_reference_grad(expr)
     expected = as_tensor(
-        Jinv[s, j] * (Jinv[r, i] * ReferenceGrad(ReferenceGrad(v))[t, r, s]), (t, i, j))
+        Jinv[s, j] * (Jinv[r, i] * ReferenceGrad(ReferenceGrad(v))[t, r, s]), (t, i, j)
+    )
     assert renumber_indices(actual) == renumber_indices(expected)
 
     expr = grad(grad(grad(v)))
     actual = change_to_reference_grad(expr)
-    expected = as_tensor(Jinv[s, k] * (Jinv[r, j] * (
-        Jinv[q, i] * ReferenceGrad(ReferenceGrad(ReferenceGrad(v)))[t, q, r, s])), (t, i, j, k))
+    expected = as_tensor(
+        Jinv[s, k]
+        * (Jinv[r, j] * (Jinv[q, i] * ReferenceGrad(ReferenceGrad(ReferenceGrad(v)))[t, q, r, s])),
+        (t, i, j, k),
+    )
     assert renumber_indices(actual) == renumber_indices(expected)
 
     # print tree_format(expected)
     # print tree_format(actual)
     # print tree_format(renumber_indices(actual))
     # print tree_format(renumber_indices(expected))
```

### Comparing `fenics-ufl-2023.2.0/test/test_change_to_reference_frame.py` & `fenics_ufl-2024.1.0.post0/test/test_change_to_reference_frame.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 """Tests of the change to reference frame algorithm."""
 
-from ufl import Coefficient, FiniteElement, FunctionSpace, Mesh, TensorElement, VectorElement, triangle
+from ufl import Coefficient, FunctionSpace, Mesh, triangle
 from ufl.classes import Expr, ReferenceValue
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import contravariant_piola, identity_pullback
+from ufl.sobolevspace import H1, HDiv
 
 
 def change_to_reference_frame(expr):
     assert isinstance(expr, Expr)
     return ReferenceValue(expr)
 
 
 def test_change_unmapped_form_arguments_to_reference_frame():
-    U = FiniteElement("CG", triangle, 1)
-    V = VectorElement("CG", triangle, 1)
-    T = TensorElement("CG", triangle, 1)
+    U = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    V = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    T = FiniteElement("Lagrange", triangle, 1, (2, 2), identity_pullback, H1)
 
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     u_space = FunctionSpace(domain, U)
     v_space = FunctionSpace(domain, V)
     t_space = FunctionSpace(domain, T)
 
     expr = Coefficient(u_space)
     assert change_to_reference_frame(expr) == ReferenceValue(expr)
     expr = Coefficient(v_space)
     assert change_to_reference_frame(expr) == ReferenceValue(expr)
     expr = Coefficient(t_space)
     assert change_to_reference_frame(expr) == ReferenceValue(expr)
 
 
 def test_change_hdiv_form_arguments_to_reference_frame():
-    V = FiniteElement("RT", triangle, 1)
+    V = FiniteElement("Raviart-Thomas", triangle, 1, (2,), contravariant_piola, HDiv)
 
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     v_space = FunctionSpace(domain, V)
 
     expr = Coefficient(v_space)
     assert change_to_reference_frame(expr) == ReferenceValue(expr)
 
 
 def test_change_hcurl_form_arguments_to_reference_frame():
-    V = FiniteElement("RT", triangle, 1)
+    V = FiniteElement("Raviart-Thomas", triangle, 1, (2,), contravariant_piola, HDiv)
 
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     v_space = FunctionSpace(domain, V)
 
     expr = Coefficient(v_space)
     assert change_to_reference_frame(expr) == ReferenceValue(expr)
 
-    '''
+    """
     # user input
     grad(f + g)('+')
     # change to reference frame
     -> (K*rgrad(rv(M)*rv(f) + rv(M)*rv(g)))('+')
     # apply derivatives
     -> (K*(rv(M)*rgrad(rv(f)) + rv(M)*rgrad(rv(g))))('+')
     # apply restrictions
@@ -114,34 +117,35 @@
     t = terminal | restricted(terminal)  # choice of terminal
     r = rval(t) | rgrad(r)               # in reference frame: value or n-gradient
     g = t | grad(g)                      # in global frame: value or n-gradient
     v = r | g                            # value in either frame
     e = v | cell_avg(v) | facet_avg(v) | at_cell_midpoint(v) | at_facet_midpoint(v)
                                          # evaluated at point or averaged over cell entity
     m = e | indexed(e)                   # scalar component of
-    '''
+    """
 
 
-'''
+"""
 New form preprocessing pipeline:
 
 Preferably introduce these changes:
 1) Create new FormArgument Expression without element or domain
 2) Create new FormArgument Constant without domain
 3) Drop replace
 --> but just applying replace first is fine
 
 i) group and join integrals by (domain, type, subdomain_id),
 ii) process integrands:
     a) apply_coefficient_completion # replace coefficients to ensure proper elements and domains
     b) lower_compound_operators # expand_compounds
     c) change_to_reference_frame # change f->rv(f), m->M*rv(m),
                                           grad(f)->K*rgrad(rv(f)),
-                                          grad(grad(f))->K*rgrad(K*rgrad(rv(f))), grad(expr)->K*rgrad(expr)
+                                          grad(grad(f))->K*rgrad(K*rgrad(rv(f))),
+                                                grad(expr)->K*rgrad(expr)
                                  # if grad(expr)->K*rgrad(expr) should be valid,
                                    then rgrad must be applicable to quite generic expressions
     d) apply_derivatives         # one possibility is to add an apply_mapped_derivatives AD
                                    algorithm which includes mappings
     e) apply_geometry_lowering
     f) apply_restrictions # requiring grad(f)('+') instead of grad(f('+')) would simplify a lot...
 iii) extract final metadata about elements and coefficient ordering
-'''
+"""
```

### Comparing `fenics-ufl-2023.2.0/test/test_classcoverage.py` & `fenics_ufl-2024.1.0.post0/test/test_classcoverage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,131 @@
 __authors__ = "Martin Sandve Alnæs"
 __date__ = "2008-09-06 -- 2009-02-10"
 
 import ufl
-from ufl import *  # noqa: F403, F401
-from ufl import (And, Argument, CellDiameter, CellVolume, Circumradius, Coefficient, Constant, FacetArea, FacetNormal,
-                 FiniteElement, FunctionSpace, Identity, Jacobian, JacobianDeterminant, JacobianInverse,
-                 MaxFacetEdgeLength, Mesh, MinFacetEdgeLength, MixedElement, Not, Or, PermutationSymbol,
-                 SpatialCoordinate, TensorConstant, TensorElement, VectorConstant, VectorElement, acos, action,
-                 as_matrix, as_tensor, as_ufl, as_vector, asin, atan, cell_avg, cofac, conditional, cos, cosh, cross,
-                 curl, derivative, det, dev, diff, div, dot, ds, dS, dx, eq, exp, facet_avg, ge, grad, gt, i, inner,
-                 inv, j, k, l, le, ln, lt, nabla_div, nabla_grad, ne, outer, rot, sin, sinh, skew, sqrt, sym, tan, tanh,
-                 tetrahedron, tr, transpose, triangle, variable)
-from ufl.algorithms import *  # noqa: F403, F401
-from ufl.classes import *  # noqa: F403, F401
-from ufl.classes import (Acos, Asin, Atan, CellCoordinate, Cos, Cosh, Exp, Expr, FacetJacobian,
-                         FacetJacobianDeterminant, FacetJacobianInverse, FloatValue, IntValue, Ln, Outer, Sin, Sinh,
-                         Sqrt, Tan, Tanh, all_ufl_classes)
+from ufl import *  # noqa: F403
+from ufl import (
+    And,
+    Argument,
+    CellDiameter,
+    CellVolume,
+    Circumradius,
+    Coefficient,
+    Constant,
+    FacetArea,
+    FacetNormal,
+    FunctionSpace,
+    Identity,
+    Jacobian,
+    JacobianDeterminant,
+    JacobianInverse,
+    MaxFacetEdgeLength,
+    Mesh,
+    MinFacetEdgeLength,
+    Not,
+    Or,
+    PermutationSymbol,
+    SpatialCoordinate,
+    TensorConstant,
+    VectorConstant,
+    acos,
+    action,
+    as_matrix,
+    as_tensor,
+    as_ufl,
+    as_vector,
+    asin,
+    atan,
+    cell_avg,
+    cofac,
+    conditional,
+    cos,
+    cosh,
+    cross,
+    curl,
+    derivative,
+    det,
+    dev,
+    diff,
+    div,
+    dot,
+    dS,
+    ds,
+    dx,
+    eq,
+    exp,
+    facet_avg,
+    ge,
+    grad,
+    gt,
+    i,
+    inner,
+    inv,
+    j,
+    k,
+    l,
+    le,
+    ln,
+    lt,
+    nabla_div,
+    nabla_grad,
+    ne,
+    outer,
+    rot,
+    sin,
+    sinh,
+    skew,
+    sqrt,
+    sym,
+    tan,
+    tanh,
+    tetrahedron,
+    tr,
+    transpose,
+    triangle,
+    variable,
+)
+from ufl.algorithms import *  # noqa: F403
+from ufl.classes import *  # noqa: F403
+from ufl.classes import (
+    Acos,
+    Asin,
+    Atan,
+    CellCoordinate,
+    Cos,
+    Cosh,
+    Exp,
+    Expr,
+    FacetJacobian,
+    FacetJacobianDeterminant,
+    FacetJacobianInverse,
+    FloatValue,
+    IntValue,
+    Ln,
+    Outer,
+    Sin,
+    Sinh,
+    Sqrt,
+    Tan,
+    Tanh,
+    all_ufl_classes,
+)
+from ufl.finiteelement import FiniteElement, MixedElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 has_repr = set()
 has_dict = set()
 
 
 def _test_object(a, shape, free_indices):
     # Check if instances of this type has certain memory consuming members
-    if hasattr(a, '_repr'):
+    if hasattr(a, "_repr"):
         has_repr.add(a.__class__.__name__)
-    if hasattr(a, '__dict__'):
+    if hasattr(a, "__dict__"):
         has_dict.add(a.__class__.__name__)
 
     # Test reproduction via repr string
     r = repr(a)
     e = eval(r, globals())
     assert hash(a) == hash(e)
 
@@ -54,17 +150,17 @@
             print(("sh:", sh))
             print(("shape:", shape))
         assert sh == shape
 
 
 def _test_object2(a):
     # Check if instances of this type has certain memory consuming members
-    if hasattr(a, '_repr'):
+    if hasattr(a, "_repr"):
         has_repr.add(a.__class__.__name__)
-    if hasattr(a, '__dict__'):
+    if hasattr(a, "__dict__"):
         has_dict.add(a.__class__.__name__)
 
     # Test reproduction via repr string
     r = repr(a)
     e = eval(r, globals())
     assert hash(a) == hash(e)
 
@@ -86,39 +182,39 @@
     "Verify that ufl.classes exports all Expr subclasses."
     all_expr_classes = []
     for m in list(vars(ufl).values()):
         if isinstance(m, type(ufl)):
             for c in list(vars(m).values()):
                 if isinstance(c, type) and issubclass(c, Expr):
                     all_expr_classes.append(c)
-    missing_classes = set(c.__name__ for c in all_expr_classes)\
-        - set(c.__name__ for c in all_ufl_classes)
+    missing_classes = set(c.__name__ for c in all_expr_classes) - set(
+        c.__name__ for c in all_ufl_classes
+    )
     if missing_classes:
         print("The following subclasses of Expr were not exported from ufl.classes:")
         print(("\n".join(sorted(missing_classes))))
     assert missing_classes == set()
 
 
 def testAll(self):
-
     Expr.ufl_enable_profiling()
 
     # --- Elements:
     cell = triangle
-    dim = cell.geometric_dimension()
+    dim = 2
 
-    e0 = FiniteElement("CG", cell, 1)
-    e1 = VectorElement("CG", cell, 1)
-    e2 = TensorElement("CG", cell, 1)
-    e3 = MixedElement(e0, e1, e2)
+    e0 = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    e1 = FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1)
+    e2 = FiniteElement("Lagrange", cell, 1, (2, 2), identity_pullback, H1)
+    e3 = MixedElement([e0, e1, e2])
 
-    e13D = VectorElement("CG", tetrahedron, 1)
+    e13D = FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1)
 
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
-    domain3D = Mesh(VectorElement("Lagrange", tetrahedron, 1))
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (dim,), identity_pullback, H1))
+    domain3D = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
     e0_space = FunctionSpace(domain, e0)
     e1_space = FunctionSpace(domain, e1)
     e2_space = FunctionSpace(domain, e2)
     e3_space = FunctionSpace(domain, e3)
     e13d_space = FunctionSpace(domain3D, e13D)
 
     # --- Terminals:
@@ -130,25 +226,25 @@
     v1 = Argument(e1_space, 5)
     v2 = Argument(e2_space, 6)
     v3 = Argument(e3_space, 7)
 
     _test_object(v0, (), ())
     _test_object(v1, (dim,), ())
     _test_object(v2, (dim, dim), ())
-    _test_object(v3, (dim*dim+dim+1,), ())
+    _test_object(v3, (1 + dim + dim**2,), ())
 
     f0 = Coefficient(e0_space)
     f1 = Coefficient(e1_space)
     f2 = Coefficient(e2_space)
     f3 = Coefficient(e3_space)
 
     _test_object(f0, (), ())
     _test_object(f1, (dim,), ())
     _test_object(f2, (dim, dim), ())
-    _test_object(f3, (dim*dim+dim+1,), ())
+    _test_object(f3, (1 + dim + dim**2,), ())
 
     c = Constant(domain)
     _test_object(c, (), ())
 
     c = VectorConstant(domain)
     _test_object(c, (dim,), ())
 
@@ -187,19 +283,19 @@
     _test_object(g, (dim, dim), ())
     g = JacobianDeterminant(domain)
     _test_object(g, (), ())
     g = JacobianInverse(domain)
     _test_object(g, (dim, dim), ())
 
     g = FacetJacobian(domain)
-    _test_object(g, (dim, dim-1), ())
+    _test_object(g, (dim, dim - 1), ())
     g = FacetJacobianDeterminant(domain)
     _test_object(g, (), ())
     g = FacetJacobianInverse(domain)
-    _test_object(g, (dim-1, dim), ())
+    _test_object(g, (dim - 1, dim), ())
 
     g = FacetNormal(domain)
     _test_object(g, (dim,), ())
     # g = CellNormal(domain)
     # _test_object(g, (dim,), ())
 
     g = CellVolume(domain)
@@ -223,23 +319,23 @@
     a = variable(v0)
     _test_object(a, (), ())
     a = variable(v1)
     _test_object(a, (dim,), ())
     a = variable(v2)
     _test_object(a, (dim, dim), ())
     a = variable(v3)
-    _test_object(a, (dim*dim+dim+1,), ())
+    _test_object(a, (1 + dim + dim**2,), ())
     a = variable(f0)
     _test_object(a, (), ())
     a = variable(f1)
     _test_object(a, (dim,), ())
     a = variable(f2)
     _test_object(a, (dim, dim), ())
     a = variable(f3)
-    _test_object(a, (dim*dim+dim+1,), ())
+    _test_object(a, (1 + dim + dim**2,), ())
 
     # a = MultiIndex()
 
     # --- Non-terminals:
 
     # a = Indexed()
     a = v2[i, j]
@@ -284,98 +380,96 @@
     a = v0 + f0 + v0
     _test_object(a, (), ())
     a = v1 + f1 + v1
     _test_object(a, (dim,), ())
     a = v2 + f2 + v2
     _test_object(a, (dim, dim), ())
     # a = Product()
-    a = 3*v0*(2.0*v0)*f0*(v0*3.0)
+    a = 3 * v0 * (2.0 * v0) * f0 * (v0 * 3.0)
     _test_object(a, (), ())
     # a = Division()
     a = v0 / 2.0
     _test_object(a, (), ())
     a = v0 / f0
     _test_object(a, (), ())
     a = v0 / (f0 + 7)
     _test_object(a, (), ())
     # a = Power()
     a = f0**3
     _test_object(a, (), ())
-    a = (f0*2)**1.23
+    a = (f0 * 2) ** 1.23
     _test_object(a, (), ())
 
     # a = ListTensor()
-    a = as_vector([1.0, 2.0*f0, f0**2])
+    a = as_vector([1.0, 2.0 * f0, f0**2])
     _test_object(a, (3,), ())
-    a = as_matrix([[1.0, 2.0*f0, f0**2],
-                   [1.0, 2.0*f0, f0**2]])
+    a = as_matrix([[1.0, 2.0 * f0, f0**2], [1.0, 2.0 * f0, f0**2]])
     _test_object(a, (2, 3), ())
-    a = as_tensor([[[0.00, 0.01, 0.02],
-                    [0.10, 0.11, 0.12]],
-                   [[1.00, 1.01, 1.02],
-                    [1.10, 1.11, 1.12]]])
+    a = as_tensor(
+        [[[0.00, 0.01, 0.02], [0.10, 0.11, 0.12]], [[1.00, 1.01, 1.02], [1.10, 1.11, 1.12]]]
+    )
     _test_object(a, (2, 2, 3), ())
 
     # a = ComponentTensor()
-    a = as_vector(v1[i]*f1[j], i)
+    a = as_vector(v1[i] * f1[j], i)
     _test_object(a, (dim,), (j,))
-    a = as_matrix(v1[i]*f1[j], (j, i))
+    a = as_matrix(v1[i] * f1[j], (j, i))
     _test_object(a, (dim, dim), ())
-    a = as_tensor(v1[i]*f1[j], (i, j))
+    a = as_tensor(v1[i] * f1[j], (i, j))
     _test_object(a, (dim, dim), ())
-    a = as_tensor(v2[i, j]*f2[j, k], (i, k))
+    a = as_tensor(v2[i, j] * f2[j, k], (i, k))
     _test_object(a, (dim, dim), ())
 
     a = dev(v2)
     _test_object(a, (dim, dim), ())
     a = dev(f2)
     _test_object(a, (dim, dim), ())
-    a = dev(f2*f0+v2*3)
+    a = dev(f2 * f0 + v2 * 3)
     _test_object(a, (dim, dim), ())
 
     a = sym(v2)
     _test_object(a, (dim, dim), ())
     a = sym(f2)
     _test_object(a, (dim, dim), ())
-    a = sym(f2*f0+v2*3)
+    a = sym(f2 * f0 + v2 * 3)
     _test_object(a, (dim, dim), ())
 
     a = skew(v2)
     _test_object(a, (dim, dim), ())
     a = skew(f2)
     _test_object(a, (dim, dim), ())
-    a = skew(f2*f0+v2*3)
+    a = skew(f2 * f0 + v2 * 3)
     _test_object(a, (dim, dim), ())
 
     a = v2.T
     _test_object(a, (dim, dim), ())
     a = f2.T
     _test_object(a, (dim, dim), ())
-    a = transpose(f2*f0+v2*3)
+    a = transpose(f2 * f0 + v2 * 3)
     _test_object(a, (dim, dim), ())
 
     a = det(v2)
     _test_object(a, (), ())
     a = det(f2)
     _test_object(a, (), ())
-    a = det(f2*f0+v2*3)
+    a = det(f2 * f0 + v2 * 3)
     _test_object(a, (), ())
 
     a = tr(v2)
     _test_object(a, (), ())
     a = tr(f2)
     _test_object(a, (), ())
-    a = tr(f2*f0+v2*3)
+    a = tr(f2 * f0 + v2 * 3)
     _test_object(a, (), ())
 
     a = cofac(v2)
     _test_object(a, (dim, dim), ())
     a = cofac(f2)
     _test_object(a, (dim, dim), ())
-    a = cofac(f2*f0+v2*3)
+    a = cofac(f2 * f0 + v2 * 3)
     _test_object(a, (dim, dim), ())
 
     cond1 = le(f0, 1.0)
     cond2 = eq(3.0, f0)
     cond3 = ne(sin(f0), cos(f0))
     cond4 = lt(sin(f0), cos(f0))
     cond5 = ge(sin(f0), cos(f0))
@@ -462,24 +556,31 @@
     _test_object(a, (), (i,))
     a = f0.dx(i, j, 1)
     _test_object(a, (), (i, j))
 
     s0 = variable(f0)
     s1 = variable(f1)
     s2 = variable(f2)
-    f = dot(s0*s1, s2)
+    f = dot(s0 * s1, s2)
     _test_object(s0, (), ())
     _test_object(s1, (dim,), ())
     _test_object(s2, (dim, dim), ())
     _test_object(f, (dim,), ())
 
     a = diff(f, s0)
     _test_object(a, (dim,), ())
     a = diff(f, s1)
-    _test_object(a, (dim, dim,), ())
+    _test_object(
+        a,
+        (
+            dim,
+            dim,
+        ),
+        (),
+    )
     a = diff(f, s2)
     _test_object(a, (dim, dim, dim), ())
 
     a = div(v1)
     _test_object(a, (), ())
     a = div(f1)
     _test_object(a, (), ())
@@ -494,17 +595,17 @@
     _test_object(a, (dim,), ())
     a = grad(f0)
     _test_object(a, (dim,), ())
     a = grad(v1)
     _test_object(a, (dim, dim), ())
     a = grad(f1)
     _test_object(a, (dim, dim), ())
-    a = grad(f0*v0)
+    a = grad(f0 * v0)
     _test_object(a, (dim,), ())
-    a = grad(f0*v1)
+    a = grad(f0 * v1)
     _test_object(a, (dim, dim), ())
 
     a = nabla_div(v1)
     _test_object(a, (), ())
     a = nabla_div(f1)
     _test_object(a, (), ())
     a = nabla_div(v2)
@@ -518,40 +619,40 @@
     _test_object(a, (dim,), ())
     a = nabla_grad(f0)
     _test_object(a, (dim,), ())
     a = nabla_grad(v1)
     _test_object(a, (dim, dim), ())
     a = nabla_grad(f1)
     _test_object(a, (dim, dim), ())
-    a = nabla_grad(f0*v0)
+    a = nabla_grad(f0 * v0)
     _test_object(a, (dim,), ())
-    a = nabla_grad(f0*v1)
+    a = nabla_grad(f0 * v1)
     _test_object(a, (dim, dim), ())
 
     a = curl(v13D)
     _test_object(a, (3,), ())
     a = curl(f13D)
     _test_object(a, (3,), ())
     a = rot(v1)
     _test_object(a, (), ())
     a = rot(f1)
     _test_object(a, (), ())
 
     # a = PositiveRestricted(v0)
     # _test_object(a, (), ())
-    a = v0('+')
+    a = v0("+")
     _test_object(a, (), ())
-    a = v0('+')*f0
+    a = v0("+") * f0
     _test_object(a, (), ())
 
     # a = NegativeRestricted(v0)
     # _test_object(a, (), ())
-    a = v0('-')
+    a = v0("-")
     _test_object(a, (), ())
-    a = v0('-') + f0
+    a = v0("-") + f0
     _test_object(a, (), ())
 
     a = cell_avg(v0)
     _test_object(a, (), ())
     a = facet_avg(v0)
     _test_object(a, (), ())
     a = cell_avg(v1)
@@ -561,55 +662,55 @@
     a = cell_avg(v1)[i]
     _test_object(a, (), (i,))
     a = facet_avg(v1)[i]
     _test_object(a, (), (i,))
 
     # --- Integrals:
 
-    a = v0*dx
+    a = v0 * dx
     _test_form(a)
-    a = v0*dx(0)
+    a = v0 * dx(0)
     _test_form(a)
-    a = v0*dx(1)
+    a = v0 * dx(1)
     _test_form(a)
-    a = v0*ds
+    a = v0 * ds
     _test_form(a)
-    a = v0*ds(0)
+    a = v0 * ds(0)
     _test_form(a)
-    a = v0*ds(1)
+    a = v0 * ds(1)
     _test_form(a)
-    a = v0*dS
+    a = v0 * dS
     _test_form(a)
-    a = v0*dS(0)
+    a = v0 * dS(0)
     _test_form(a)
-    a = v0*dS(1)
+    a = v0 * dS(1)
     _test_form(a)
 
-    a = v0*dot(v1, f1)*dx
+    a = v0 * dot(v1, f1) * dx
     _test_form(a)
-    a = v0*dot(v1, f1)*dx(0)
+    a = v0 * dot(v1, f1) * dx(0)
     _test_form(a)
-    a = v0*dot(v1, f1)*dx(1)
+    a = v0 * dot(v1, f1) * dx(1)
     _test_form(a)
-    a = v0*dot(v1, f1)*ds
+    a = v0 * dot(v1, f1) * ds
     _test_form(a)
-    a = v0*dot(v1, f1)*ds(0)
+    a = v0 * dot(v1, f1) * ds(0)
     _test_form(a)
-    a = v0*dot(v1, f1)*ds(1)
+    a = v0 * dot(v1, f1) * ds(1)
     _test_form(a)
-    a = v0*dot(v1, f1)*dS
+    a = v0 * dot(v1, f1) * dS
     _test_form(a)
-    a = v0*dot(v1, f1)*dS(0)
+    a = v0 * dot(v1, f1) * dS(0)
     _test_form(a)
-    a = v0*dot(v1, f1)*dS(1)
+    a = v0 * dot(v1, f1) * dS(1)
     _test_form(a)
 
     # --- Form transformations:
 
-    a = f0*v0*dx + f0*v0*dot(f1, v1)*dx
+    a = f0 * v0 * dx + f0 * v0 * dot(f1, v1) * dx
     # b = lhs(a) # TODO
     # c = rhs(a) # TODO
     d = derivative(a, f1, v1)
     f = action(d)
     # e = action(b)
 
     # --- Check which classes have been created
```

### Comparing `fenics-ufl-2023.2.0/test/test_complex.py` & `fenics_ufl-2024.1.0.post0/test/test_complex.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,136 @@
 import cmath
 
 import pytest
 
-from ufl import (Coefficient, FiniteElement, FunctionSpace, Mesh, TestFunction, TrialFunction, VectorElement, as_tensor,
-                 as_ufl, atan, conditional, conj, cos, cosh, dot, dx, exp, ge, grad, gt, imag, inner, le, ln, lt,
-                 max_value, min_value, outer, real, sin, sqrt, triangle)
+from ufl import (
+    Coefficient,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TrialFunction,
+    as_tensor,
+    as_ufl,
+    atan,
+    conditional,
+    conj,
+    cos,
+    cosh,
+    dot,
+    dx,
+    exp,
+    ge,
+    grad,
+    gt,
+    imag,
+    inner,
+    le,
+    ln,
+    lt,
+    max_value,
+    min_value,
+    outer,
+    real,
+    sin,
+    sqrt,
+    triangle,
+)
 from ufl.algebra import Conj, Imag, Real
 from ufl.algorithms import estimate_total_polynomial_degree
 from ufl.algorithms.apply_algebra_lowering import apply_algebra_lowering
 from ufl.algorithms.comparison_checker import ComplexComparisonError, do_comparison_check
 from ufl.algorithms.formtransformations import compute_form_adjoint
 from ufl.algorithms.remove_complex_nodes import remove_complex_nodes
 from ufl.constantvalue import ComplexValue, Zero
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 
 def test_conj(self):
-    z1 = ComplexValue(1+2j)
-    z2 = ComplexValue(1-2j)
+    z1 = ComplexValue(1 + 2j)
+    z2 = ComplexValue(1 - 2j)
 
     assert z1 == Conj(z2)
     assert z2 == Conj(z1)
 
 
 def test_real(self):
     z0 = Zero()
     z1 = as_ufl(1.0)
     z2 = ComplexValue(1j)
-    z3 = ComplexValue(1+1j)
+    z3 = ComplexValue(1 + 1j)
     assert Real(z1) == z1
     assert Real(z3) == z1
     assert Real(z2) == z0
 
 
 def test_imag(self):
     z0 = Zero()
     z1 = as_ufl(1.0)
     z2 = as_ufl(1j)
-    z3 = ComplexValue(1+1j)
+    z3 = ComplexValue(1 + 1j)
 
     assert Imag(z2) == z1
     assert Imag(z3) == z1
     assert Imag(z1) == z0
 
 
 def test_compute_form_adjoint(self):
     cell = triangle
-    element = FiniteElement('Lagrange', cell, 1)
-    domain = Mesh(VectorElement('Lagrange', cell, 1))
+    element = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     u = TrialFunction(space)
     v = TestFunction(space)
 
     a = inner(grad(u), grad(v)) * dx
 
     assert compute_form_adjoint(a) == conj(inner(grad(v), grad(u))) * dx
 
 
 def test_complex_algebra(self):
     z1 = ComplexValue(1j)
-    z2 = ComplexValue(1+1j)
+    z2 = ComplexValue(1 + 1j)
 
-    # Remember that ufl.algebra functions return ComplexValues, but ufl.mathfunctions return complex Python scalar
-    # Any operations with a ComplexValue and a complex Python scalar promote to ComplexValue
-    assert z1*z2 == ComplexValue(-1+1j)
-    assert z2/z1 == ComplexValue(1-1j)
-    assert pow(z2, z1) == ComplexValue((1+1j)**1j)
-    assert sqrt(z2) * as_ufl(1) == ComplexValue(cmath.sqrt(1+1j))
+    # Remember that ufl.algebra functions return ComplexValues, but
+    # ufl.mathfunctions return complex Python scalar
+    # Any operations with a ComplexValue and a complex Python scalar
+    # promote to ComplexValue
+    assert z1 * z2 == ComplexValue(-1 + 1j)
+    assert z2 / z1 == ComplexValue(1 - 1j)
+    assert pow(z2, z1) == ComplexValue((1 + 1j) ** 1j)
+    assert sqrt(z2) * as_ufl(1) == ComplexValue(cmath.sqrt(1 + 1j))
     assert (sin(z2) + cosh(z2) - atan(z2)) * z1 == ComplexValue(
-        (cmath.sin(1+1j) + cmath.cosh(1+1j) - cmath.atan(1+1j))*1j)
-    assert (abs(z2) - ln(z2))/exp(z1) == ComplexValue((abs(1+1j) - cmath.log(1+1j))/cmath.exp(1j))
+        (cmath.sin(1 + 1j) + cmath.cosh(1 + 1j) - cmath.atan(1 + 1j)) * 1j
+    )
+    assert (abs(z2) - ln(z2)) / exp(z1) == ComplexValue(
+        (abs(1 + 1j) - cmath.log(1 + 1j)) / cmath.exp(1j)
+    )
 
 
 def test_automatic_simplification(self):
     cell = triangle
-    element = FiniteElement("Lagrange", cell, 1)
-    domain = Mesh(VectorElement('Lagrange', cell, 1))
+    element = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
 
     assert inner(u, v) == u * conj(v)
     assert dot(u, v) == u * v
     assert outer(u, v) == conj(u) * v
 
 
 def test_apply_algebra_lowering_complex(self):
     cell = triangle
-    element = FiniteElement("Lagrange", cell, 1)
-    domain = Mesh(VectorElement('Lagrange', cell, 1))
+    element = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
 
     gv = grad(v)
     gu = grad(u)
@@ -108,44 +145,46 @@
     lowered_a_index = lowered_a.index()
     lowered_b_index = lowered_b.index()
     lowered_c_indices = lowered_c.indices()
 
     assert lowered_a == gu[lowered_a_index] * gv[lowered_a_index]
     assert lowered_b == gv[lowered_b_index] * conj(gu[lowered_b_index])
     assert lowered_c == as_tensor(
-        conj(gu[lowered_c_indices[0]]) * gv[lowered_c_indices[1]], (lowered_c_indices[0],) + (lowered_c_indices[1],))
+        conj(gu[lowered_c_indices[0]]) * gv[lowered_c_indices[1]],
+        (lowered_c_indices[0],) + (lowered_c_indices[1],),
+    )
 
 
 def test_remove_complex_nodes(self):
     cell = triangle
-    element = FiniteElement("Lagrange", cell, 1)
-    domain = Mesh(VectorElement('Lagrange', cell, 1))
+    element = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     u = TrialFunction(space)
     v = TestFunction(space)
     f = Coefficient(space)
 
     a = conj(v)
     b = real(u)
     c = imag(f)
-    d = conj(real(v))*imag(conj(u))
+    d = conj(real(v)) * imag(conj(u))
 
     assert remove_complex_nodes(a) == v
     assert remove_complex_nodes(b) == u
     with pytest.raises(BaseException):
         remove_complex_nodes(c)
     with pytest.raises(BaseException):
         remove_complex_nodes(d)
 
 
 def test_comparison_checker(self):
     cell = triangle
-    element = FiniteElement("Lagrange", cell, 1)
-    domain = Mesh(VectorElement('Lagrange', cell, 1))
+    element = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     u = TrialFunction(space)
     v = TestFunction(space)
 
     a = conditional(ge(abs(u), imag(v)), u, v)
     b = conditional(le(sqrt(abs(u)), imag(v)), as_ufl(1), as_ufl(1j))
@@ -164,16 +203,16 @@
     assert do_comparison_check(e) == max_value(real(as_ufl(0)), real(real(u)))
     assert do_comparison_check(f) == min_value(real(sin(u)), real(cos(v)))
     assert do_comparison_check(g) == min_value(real(sin(pow(u, 3))), real(cos(abs(v))))
 
 
 def test_complex_degree_handling(self):
     cell = triangle
-    element = FiniteElement("Lagrange", cell, 3)
-    domain = Mesh(VectorElement('Lagrange', cell, 1))
+    element = FiniteElement("Lagrange", cell, 3, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
 
     a = conj(v)
     b = imag(v)
     c = real(v)
```

### Comparing `fenics-ufl-2023.2.0/test/test_conditionals.py` & `fenics_ufl-2024.1.0.post0/test/test_conditionals.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 __authors__ = "Martin Sandve Alnæs"
 __date__ = "2008-08-20 -- 2012-11-30"
 
 import pytest
 
-from ufl import (Coefficient, FiniteElement, FunctionSpace, Mesh, VectorElement, conditional, eq, ge, gt, le, lt, ne,
-                 triangle)
+from ufl import Coefficient, FunctionSpace, Mesh, conditional, eq, ge, gt, le, lt, ne, triangle
 from ufl.classes import EQ, GE, GT, LE, LT, NE
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 
 @pytest.fixture
 def f():
-    element = FiniteElement("Lagrange", triangle, 1)
-    domain = Mesh(VectorElement('Lagrange', triangle, 1))
+    element = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     return Coefficient(space)
 
 
 @pytest.fixture
 def g():
-    element = FiniteElement("Lagrange", triangle, 1)
-    domain = Mesh(VectorElement('Lagrange', triangle, 1))
+    element = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     return Coefficient(space)
 
 
 def test_conditional_does_not_allow_bool_condition(f, g):
     # The reason for this test is that it protects from the case
     # conditional(a == b, t, f) in which a == b means comparing representations
```

### Comparing `fenics-ufl-2023.2.0/test/test_derivative.py` & `fenics_ufl-2024.1.0.post0/test/test_derivative.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,85 @@
 __authors__ = "Martin Sandve Alnæs"
 __date__ = "2009-02-17 -- 2009-02-17"
 
 from itertools import chain
 
-from ufl import (CellDiameter, CellVolume, Circumradius, Coefficient, Constant, FacetArea, FacetNormal, FiniteElement,
-                 FunctionSpace, Identity, Index, Jacobian, JacobianInverse, Mesh, SpatialCoordinate, TensorElement,
-                 TestFunction, TrialFunction, VectorElement, acos, as_matrix, as_tensor, as_vector, asin, atan,
-                 conditional, cos, derivative, diff, dot, dx, exp, i, indices, inner, interval, j, k, ln, lt,
-                 nabla_grad, outer, quadrilateral, replace, sign, sin, split, sqrt, tan, tetrahedron, triangle,
-                 variable, zero)
+from ufl import (
+    CellDiameter,
+    CellVolume,
+    Circumradius,
+    Coefficient,
+    Constant,
+    FacetArea,
+    FacetNormal,
+    FunctionSpace,
+    Identity,
+    Index,
+    Jacobian,
+    JacobianInverse,
+    Mesh,
+    SpatialCoordinate,
+    TestFunction,
+    TrialFunction,
+    acos,
+    as_matrix,
+    as_tensor,
+    as_vector,
+    asin,
+    atan,
+    conditional,
+    cos,
+    derivative,
+    diff,
+    dot,
+    dx,
+    exp,
+    i,
+    indices,
+    inner,
+    interval,
+    j,
+    k,
+    ln,
+    lt,
+    nabla_grad,
+    outer,
+    quadrilateral,
+    replace,
+    sign,
+    sin,
+    split,
+    sqrt,
+    tan,
+    tetrahedron,
+    triangle,
+    variable,
+    zero,
+)
 from ufl.algorithms import compute_form_data, expand_indices, strip_variables
 from ufl.algorithms.apply_algebra_lowering import apply_algebra_lowering
 from ufl.algorithms.apply_derivatives import apply_derivatives
 from ufl.algorithms.apply_geometry_lowering import apply_geometry_lowering
 from ufl.classes import Indexed, MultiIndex, ReferenceGrad
 from ufl.constantvalue import as_ufl
 from ufl.domain import extract_unique_domain
+from ufl.finiteelement import FiniteElement, MixedElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1, L2
 
 
 def assertEqualBySampling(actual, expected):
-    ad = compute_form_data(actual*dx)
+    ad = compute_form_data(actual * dx)
     a = ad.preprocessed_form.integrals_by_type("cell")[0].integrand()
-    bd = compute_form_data(expected*dx)
+    bd = compute_form_data(expected * dx)
     b = bd.preprocessed_form.integrals_by_type("cell")[0].integrand()
 
-    assert ([ad.function_replace_map[ac] for ac in ad.reduced_coefficients]
-            == [bd.function_replace_map[bc] for bc in bd.reduced_coefficients])
+    assert [ad.function_replace_map[ac] for ac in ad.reduced_coefficients] == [
+        bd.function_replace_map[bc] for bc in bd.reduced_coefficients
+    ]
 
     n = ad.num_coefficients
 
     def make_value(c):
         if isinstance(c, Coefficient):
             z = 0.3
             m = c.count()
@@ -39,24 +89,32 @@
         if c.ufl_shape == ():
             return z * (0.1 + 0.9 * m / n)
         elif len(c.ufl_shape) == 1:
             return tuple((z * (j + 0.1 + 0.9 * m / n) for j in range(c.ufl_shape[0])))
         else:
             raise NotImplementedError("Tensor valued expressions not supported here.")
 
-    amapping = dict((c, make_value(c)) for c in chain(ad.original_form.coefficients(), ad.original_form.arguments()))
-    bmapping = dict((c, make_value(c)) for c in chain(bd.original_form.coefficients(), bd.original_form.arguments()))
-    acell = extract_unique_domain(actual).ufl_cell()
-    bcell = extract_unique_domain(expected).ufl_cell()
+    amapping = dict(
+        (c, make_value(c))
+        for c in chain(ad.original_form.coefficients(), ad.original_form.arguments())
+    )
+    bmapping = dict(
+        (c, make_value(c))
+        for c in chain(bd.original_form.coefficients(), bd.original_form.arguments())
+    )
+    adomain = extract_unique_domain(actual)
+    bdomain = extract_unique_domain(expected)
+    acell = adomain.ufl_cell()
+    bcell = bdomain.ufl_cell()
     assert acell == bcell
-    if acell.geometric_dimension() == 1:
+    if adomain.geometric_dimension() == 1:
         x = (0.3,)
-    elif acell.geometric_dimension() == 2:
+    elif adomain.geometric_dimension() == 2:
         x = (0.3, 0.4)
-    elif acell.geometric_dimension() == 3:
+    elif adomain.geometric_dimension() == 3:
         x = (0.3, 0.4, 0.5)
     av = a(x, amapping)
     bv = b(x, bmapping)
 
     if not av == bv:
         print("Tried to sample expressions to compare but failed:")
         print()
@@ -68,16 +126,16 @@
         print()
 
     assert av == bv
 
 
 def _test(self, f, df):
     cell = triangle
-    element = FiniteElement("CG", cell, 1)
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    element = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
     w = Coefficient(space)
     xv = (0.3, 0.7)
     uv = 7.0
@@ -89,531 +147,630 @@
 
     dfv1 = derivative(f(w), w, v)
     dfv2 = df(w, v)
     dfv1 = dfv1(x, mapping)
     dfv2 = dfv2(x, mapping)
     assert dfv1 == dfv2
 
-    dfv1 = derivative(f(7*w), w, v)
-    dfv2 = 7*df(7*w, v)
+    dfv1 = derivative(f(7 * w), w, v)
+    dfv2 = 7 * df(7 * w, v)
     dfv1 = dfv1(x, mapping)
     dfv2 = dfv2(x, mapping)
     assert dfv1 == dfv2
 
+
 # --- Literals
 
 
 def testScalarLiteral(self):
-    def f(w): return as_ufl(1)
+    def f(w):
+        return as_ufl(1)
+
+    def df(w, v):
+        return zero()
 
-    def df(w, v): return zero()
     _test(self, f, df)
 
 
 def testIdentityLiteral(self):
-    def f(w): return Identity(2)[i, i]
+    def f(w):
+        return Identity(2)[i, i]
+
+    def df(w, v):
+        return zero()
 
-    def df(w, v): return zero()
     _test(self, f, df)
 
+
 # --- Form arguments
 
 
 def testCoefficient(self):
-    def f(w): return w
+    def f(w):
+        return w
+
+    def df(w, v):
+        return v
 
-    def df(w, v): return v
     _test(self, f, df)
 
 
 def testArgument(self):
-    def f(w): return TestFunction(FunctionSpace(Mesh(VectorElement("Lagrange", triangle, 1)),
-                                                FiniteElement("CG", triangle, 1)))
+    def f(w):
+        return TestFunction(
+            FunctionSpace(
+                Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)),
+                FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1),
+            )
+        )
+
+    def df(w, v):
+        return zero()
 
-    def df(w, v): return zero()
     _test(self, f, df)
 
+
 # --- Geometry
 
 
 def testSpatialCoordinate(self):
-    def f(w): return SpatialCoordinate(Mesh(VectorElement("Lagrange", triangle, 1)))[0]
+    def f(w):
+        return SpatialCoordinate(
+            Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
+        )[0]
+
+    def df(w, v):
+        return zero()
 
-    def df(w, v): return zero()
     _test(self, f, df)
 
 
 def testFacetNormal(self):
-    def f(w): return FacetNormal(Mesh(VectorElement("Lagrange", triangle, 1)))[0]
+    def f(w):
+        return FacetNormal(
+            Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
+        )[0]
 
-    def df(w, v): return zero()
-    _test(self, f, df)
+    def df(w, v):
+        return zero()
 
-# def testCellSurfaceArea(self):
-#    def f(w):     return CellSurfaceArea(Mesh(VectorElement("Lagrange", triangle, 1)))
-#    def df(w, v): return zero()
-#    _test(self, f, df)
+    _test(self, f, df)
 
 
 def testFacetArea(self):
-    def f(w): return FacetArea(Mesh(VectorElement("Lagrange", triangle, 1)))
+    def f(w):
+        return FacetArea(Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)))
+
+    def df(w, v):
+        return zero()
 
-    def df(w, v): return zero()
     _test(self, f, df)
 
 
 def testCellDiameter(self):
-    def f(w): return CellDiameter(Mesh(VectorElement("Lagrange", triangle, 1)))
+    def f(w):
+        return CellDiameter(
+            Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
+        )
+
+    def df(w, v):
+        return zero()
 
-    def df(w, v): return zero()
     _test(self, f, df)
 
 
 def testCircumradius(self):
-    def f(w): return Circumradius(Mesh(VectorElement("Lagrange", triangle, 1)))
+    def f(w):
+        return Circumradius(
+            Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
+        )
+
+    def df(w, v):
+        return zero()
 
-    def df(w, v): return zero()
     _test(self, f, df)
 
 
 def testCellVolume(self):
-    def f(w): return CellVolume(Mesh(VectorElement("Lagrange", triangle, 1)))
+    def f(w):
+        return CellVolume(Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)))
+
+    def df(w, v):
+        return zero()
 
-    def df(w, v): return zero()
     _test(self, f, df)
 
+
 # --- Basic operators
 
 
 def testSum(self):
-    def f(w): return w + 1
+    def f(w):
+        return w + 1
+
+    def df(w, v):
+        return v
 
-    def df(w, v): return v
     _test(self, f, df)
 
 
 def testProduct(self):
-    def f(w): return 3*w
+    def f(w):
+        return 3 * w
+
+    def df(w, v):
+        return 3 * v
 
-    def df(w, v): return 3*v
     _test(self, f, df)
 
 
 def testPower(self):
-    def f(w): return w**3
+    def f(w):
+        return w**3
+
+    def df(w, v):
+        return 3 * w**2 * v
 
-    def df(w, v): return 3*w**2*v
     _test(self, f, df)
 
 
 def testDivision(self):
-    def f(w): return w / 3.0
+    def f(w):
+        return w / 3.0
+
+    def df(w, v):
+        return v / 3.0
 
-    def df(w, v): return v / 3.0
     _test(self, f, df)
 
 
 def testDivision2(self):
-    def f(w): return 3.0 / w
+    def f(w):
+        return 3.0 / w
+
+    def df(w, v):
+        return -3.0 * v / w**2
 
-    def df(w, v): return -3.0 * v / w**2
     _test(self, f, df)
 
 
 def testExp(self):
-    def f(w): return exp(w)
+    def f(w):
+        return exp(w)
+
+    def df(w, v):
+        return v * exp(w)
 
-    def df(w, v): return v*exp(w)
     _test(self, f, df)
 
 
 def testLn(self):
-    def f(w): return ln(w)
+    def f(w):
+        return ln(w)
+
+    def df(w, v):
+        return v / w
 
-    def df(w, v): return v / w
     _test(self, f, df)
 
 
 def testCos(self):
-    def f(w): return cos(w)
+    def f(w):
+        return cos(w)
+
+    def df(w, v):
+        return -v * sin(w)
 
-    def df(w, v): return -v*sin(w)
     _test(self, f, df)
 
 
 def testSin(self):
-    def f(w): return sin(w)
+    def f(w):
+        return sin(w)
+
+    def df(w, v):
+        return v * cos(w)
 
-    def df(w, v): return v*cos(w)
     _test(self, f, df)
 
 
 def testTan(self):
-    def f(w): return tan(w)
+    def f(w):
+        return tan(w)
+
+    def df(w, v):
+        return v * 2.0 / (cos(2.0 * w) + 1.0)
 
-    def df(w, v): return v*2.0/(cos(2.0*w) + 1.0)
     _test(self, f, df)
 
 
 def testAcos(self):
-    def f(w): return acos(w/1000)
+    def f(w):
+        return acos(w / 1000)
+
+    def df(w, v):
+        return -(v / 1000) / sqrt(1.0 - (w / 1000) ** 2)
 
-    def df(w, v): return -(v/1000)/sqrt(1.0 - (w/1000)**2)
     _test(self, f, df)
 
 
 def testAsin(self):
-    def f(w): return asin(w/1000)
+    def f(w):
+        return asin(w / 1000)
+
+    def df(w, v):
+        return (v / 1000) / sqrt(1.0 - (w / 1000) ** 2)
 
-    def df(w, v): return (v/1000)/sqrt(1.0 - (w/1000)**2)
     _test(self, f, df)
 
 
 def testAtan(self):
-    def f(w): return atan(w)
+    def f(w):
+        return atan(w)
+
+    def df(w, v):
+        return v / (1.0 + w**2)
 
-    def df(w, v): return v/(1.0 + w**2)
     _test(self, f, df)
 
+
 # FIXME: Add the new erf and bessel_*
 
 # --- Abs and conditionals
 
 
 def testAbs(self):
-    def f(w): return abs(w)
+    def f(w):
+        return abs(w)
+
+    def df(w, v):
+        return sign(w) * v
 
-    def df(w, v): return sign(w)*v
     _test(self, f, df)
 
 
 def testConditional(self):  # This will fail without bugfix in derivative
-    def cond(w): return lt(w, 1.0)
+    def cond(w):
+        return lt(w, 1.0)
+
+    def f(w):
+        return conditional(cond(w), 2 * w, 3 * w)
 
-    def f(w): return conditional(cond(w), 2*w, 3*w)
+    def df(w, v):
+        return conditional(cond(w), 1, 0) * 2 * v + conditional(cond(w), 0, 1) * 3 * v
 
-    def df(w, v): return (conditional(cond(w), 1, 0) * 2*v +
-                          conditional(cond(w), 0, 1) * 3*v)
     _test(self, f, df)
 
+
 # --- Tensor algebra basics
 
 
 def testIndexSum(self):
     def f(w):
         # 3*w + 4*w**2 + 5*w**3
         a = as_vector((w, w**2, w**3))
         b = as_vector((3, 4, 5))
-        i, = indices(1)
-        return a[i]*b[i]
+        (i,) = indices(1)
+        return a[i] * b[i]
+
+    def df(w, v):
+        return 3 * v + 4 * 2 * w * v + 5 * 3 * w**2 * v
 
-    def df(w, v): return 3*v + 4*2*w*v + 5*3*w**2*v
     _test(self, f, df)
 
 
 def testListTensor(self):
     v = variable(as_ufl(42))
-    f = as_tensor((
-        ((0, 0), (0, 0)),
-        ((v, 2*v), (0, 0)),
-        ((v**2, 1), (2, v/2)),
-    ))
+    f = as_tensor(
+        (
+            ((0, 0), (0, 0)),
+            ((v, 2 * v), (0, 0)),
+            ((v**2, 1), (2, v / 2)),
+        )
+    )
     assert f.ufl_shape == (3, 2, 2)
-    g = as_tensor((
-        ((0, 0), (0, 0)),
-        ((1, 2), (0, 0)),
-        ((84, 0), (0, 0.5)),
-    ))
+    g = as_tensor(
+        (
+            ((0, 0), (0, 0)),
+            ((1, 2), (0, 0)),
+            ((84, 0), (0, 0.5)),
+        )
+    )
     assert g.ufl_shape == (3, 2, 2)
     dfv = diff(f, v)
     x = None
     for a in range(3):
         for b in range(2):
             for c in range(2):
                 self.assertEqual(dfv[a, b, c](x), g[a, b, c](x))
 
+
 # --- Coefficient and argument input configurations
 
 
 def test_single_scalar_coefficient_derivative(self):
     cell = triangle
-    V = FiniteElement("CG", cell, 1)
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    V = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, V)
     u = Coefficient(space)
     v = TestFunction(space)
-    a = 3*u**2
+    a = 3 * u**2
     b = derivative(a, u, v)
-    self.assertEqualAfterPreprocessing(b, 3*(u*(2*v)))
+    self.assertEqualAfterPreprocessing(b, 3 * (u * (2 * v)))
 
 
 def test_single_vector_coefficient_derivative(self):
     cell = triangle
-    V = VectorElement("CG", cell, 1)
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    V = FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, V)
     u = Coefficient(space)
     v = TestFunction(space)
-    a = 3*dot(u, u)
+    a = 3 * dot(u, u)
     actual = derivative(a, u, v)
-    expected = 3*(2*(u[i]*v[i]))
+    expected = 3 * (2 * (u[i] * v[i]))
     assertEqualBySampling(actual, expected)
 
 
 def test_multiple_coefficient_derivative(self):
     cell = triangle
-    V = FiniteElement("CG", cell, 1)
-    W = VectorElement("CG", cell, 1)
-    M = V*W
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    V = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    W = FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1)
+    M = MixedElement([V, W])
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     v_space = FunctionSpace(domain, V)
     w_space = FunctionSpace(domain, W)
     m_space = FunctionSpace(domain, M)
     uv = Coefficient(v_space)
     uw = Coefficient(w_space)
     v = TestFunction(m_space)
     vv, vw = split(v)
 
-    a = sin(uv)*dot(uw, uw)
+    a = sin(uv) * dot(uw, uw)
 
     actual = derivative(a, (uv, uw), split(v))
-    expected = cos(uv)*vv * (uw[i]*uw[i]) + (uw[j]*vw[j])*2 * sin(uv)
+    expected = cos(uv) * vv * (uw[i] * uw[i]) + (uw[j] * vw[j]) * 2 * sin(uv)
     assertEqualBySampling(actual, expected)
 
     actual = derivative(a, (uv, uw), v)
-    expected = cos(uv)*vv * (uw[i]*uw[i]) + (uw[j]*vw[j])*2 * sin(uv)
+    expected = cos(uv) * vv * (uw[i] * uw[i]) + (uw[j] * vw[j]) * 2 * sin(uv)
     assertEqualBySampling(actual, expected)
 
 
 def test_indexed_coefficient_derivative(self):
     cell = triangle
-    ident = Identity(cell.geometric_dimension())
-    V = FiniteElement("CG", cell, 1)
-    W = VectorElement("CG", cell, 1)
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    ident = Identity(2)
+    V = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    W = FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     v_space = FunctionSpace(domain, V)
     w_space = FunctionSpace(domain, W)
     u = Coefficient(w_space)
     v = TestFunction(v_space)
 
     w = dot(u, nabla_grad(u))
     # a = dot(w, w)
-    a = (u[i]*u[k].dx(i)) * w[k]
+    a = (u[i] * u[k].dx(i)) * w[k]
 
     actual = derivative(a, u[0], v)
 
-    dw = v*u[k].dx(0) + u[i]*ident[0, k]*v.dx(i)
+    dw = v * u[k].dx(0) + u[i] * ident[0, k] * v.dx(i)
     expected = 2 * w[k] * dw
 
     assertEqualBySampling(actual, expected)
 
 
 def test_multiple_indexed_coefficient_derivative(self):
     cell = tetrahedron
-    V = FiniteElement("CG", cell, 1)
-    V2 = V*V
-    W = VectorElement("CG", cell, 1)
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    V = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    V2 = MixedElement([V, V])
+    W = FiniteElement("Lagrange", cell, 1, (3,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (3,), identity_pullback, H1))
     v2_space = FunctionSpace(domain, V2)
     w_space = FunctionSpace(domain, W)
     u = Coefficient(w_space)
     w = Coefficient(w_space)
     v = TestFunction(v2_space)
     vu, vw = split(v)
 
-    actual = derivative(cos(u[i]*w[i]), (u[2], w[1]), (vu, vw))
-    expected = -sin(u[i]*w[i])*(vu*w[2] + u[1]*vw)
+    actual = derivative(cos(u[i] * w[i]), (u[2], w[1]), (vu, vw))
+    expected = -sin(u[i] * w[i]) * (vu * w[2] + u[1] * vw)
 
     assertEqualBySampling(actual, expected)
 
 
 def test_segregated_derivative_of_convection(self):
     cell = tetrahedron
-    V = FiniteElement("CG", cell, 1)
-    W = VectorElement("CG", cell, 1)
+    V = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    W = FiniteElement("Lagrange", cell, 1, (3,), identity_pullback, H1)
 
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (3,), identity_pullback, H1))
     v_space = FunctionSpace(domain, V)
     w_space = FunctionSpace(domain, W)
 
     u = Coefficient(w_space)
     v = Coefficient(w_space)
     du = TrialFunction(v_space)
     dv = TestFunction(v_space)
 
     L = dot(dot(u, nabla_grad(u)), v)
 
     Lv = {}
     Lvu = {}
-    for a in range(cell.geometric_dimension()):
+    for a in range(3):
         Lv[a] = derivative(L, v[a], dv)
-        for b in range(cell.geometric_dimension()):
+        for b in range(3):
             Lvu[a, b] = derivative(Lv[a], u[b], du)
 
-    for a in range(cell.geometric_dimension()):
-        for b in range(cell.geometric_dimension()):
-            form = Lvu[a, b]*dx
+    for a in range(3):
+        for b in range(3):
+            form = Lvu[a, b] * dx
             fd = compute_form_data(form)
             pf = fd.preprocessed_form
             expand_indices(pf)
 
     k = Index()
-    for a in range(cell.geometric_dimension()):
-        for b in range(cell.geometric_dimension()):
+    for a in range(3):
+        for b in range(3):
             actual = Lvu[a, b]
-            expected = du*u[a].dx(b)*dv + u[k]*du.dx(k)*dv
+            expected = du * u[a].dx(b) * dv + u[k] * du.dx(k) * dv
             assertEqualBySampling(actual, expected)
 
+
 # --- User provided derivatives of coefficients
 
 
 def test_coefficient_derivatives(self):
-    V = FiniteElement("Lagrange", triangle, 1)
+    V = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
 
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, V)
 
     dv = TestFunction(space)
 
     f = Coefficient(space, count=0)
     g = Coefficient(space, count=1)
     df = Coefficient(space, count=2)
     dg = Coefficient(space, count=3)
     u = Coefficient(space, count=4)
     cd = {f: df, g: dg}
 
     integrand = inner(f, g)
-    expected = (df*dv)*g + f*(dg*dv)
+    expected = (df * dv) * g + f * (dg * dv)
 
-    F = integrand*dx
+    F = integrand * dx
     J = derivative(F, u, dv, cd)
     fd = compute_form_data(J)
     actual = fd.preprocessed_form.integrals()[0].integrand()
-    assert (actual*dx).signature() == (expected*dx).signature()
+    assert (actual * dx).signature() == (expected * dx).signature()
     self.assertEqual(replace(actual, fd.function_replace_map), expected)
 
 
 def test_vector_coefficient_scalar_derivatives(self):
-    V = FiniteElement("Lagrange", triangle, 1)
-    VV = VectorElement("Lagrange", triangle, 1)
+    V = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    VV = FiniteElement("vector Lagrange", triangle, 1, (2,), identity_pullback, H1)
 
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     v_space = FunctionSpace(domain, V)
     vv_space = FunctionSpace(domain, VV)
 
     dv = TestFunction(v_space)
 
     df = Coefficient(vv_space, count=0)
     g = Coefficient(vv_space, count=1)
     f = Coefficient(vv_space, count=2)
     u = Coefficient(v_space, count=3)
     cd = {f: df}
 
     integrand = inner(f, g)
 
     i0, i1, i2, i3, i4 = [Index(count=c) for c in range(5)]
-    expected = as_tensor(df[i1]*dv, (i1,))[i0]*g[i0]
+    expected = as_tensor(df[i1] * dv, (i1,))[i0] * g[i0]
 
-    F = integrand*dx
+    F = integrand * dx
     J = derivative(F, u, dv, cd)
     fd = compute_form_data(J)
     actual = fd.preprocessed_form.integrals()[0].integrand()
-    assert (actual*dx).signature() == (expected*dx).signature()
+    assert (actual * dx).signature() == (expected * dx).signature()
 
 
 def test_vector_coefficient_derivatives(self):
-    V = VectorElement("Lagrange", triangle, 1)
-    VV = TensorElement("Lagrange", triangle, 1)
+    V = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    VV = FiniteElement("Lagrange", triangle, 1, (2, 2), identity_pullback, H1)
 
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     v_space = FunctionSpace(domain, V)
     vv_space = FunctionSpace(domain, VV)
 
     dv = TestFunction(v_space)
 
     df = Coefficient(vv_space, count=0)
     g = Coefficient(v_space, count=1)
     f = Coefficient(v_space, count=2)
     u = Coefficient(v_space, count=3)
     cd = {f: df}
 
     integrand = inner(f, g)
 
     i0, i1, i2, i3, i4 = [Index(count=c) for c in range(5)]
-    expected = as_tensor(df[i2, i1]*dv[i1], (i2,))[i0]*g[i0]
+    expected = as_tensor(df[i2, i1] * dv[i1], (i2,))[i0] * g[i0]
 
-    F = integrand*dx
+    F = integrand * dx
     J = derivative(F, u, dv, cd)
     fd = compute_form_data(J)
     actual = fd.preprocessed_form.integrals()[0].integrand()
-    assert (actual*dx).signature() == (expected*dx).signature()
+    assert (actual * dx).signature() == (expected * dx).signature()
     # self.assertEqual(replace(actual, fd.function_replace_map), expected)
 
 
 def test_vector_coefficient_derivatives_of_product(self):
-    V = VectorElement("Lagrange", triangle, 1)
-    VV = TensorElement("Lagrange", triangle, 1)
+    V = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    VV = FiniteElement("Lagrange", triangle, 1, (2, 2), identity_pullback, H1)
 
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     v_space = FunctionSpace(domain, V)
     vv_space = FunctionSpace(domain, VV)
 
     dv = TestFunction(v_space)
 
     df = Coefficient(vv_space, count=0)
     g = Coefficient(v_space, count=1)
     dg = Coefficient(vv_space, count=2)
     f = Coefficient(v_space, count=3)
     u = Coefficient(v_space, count=4)
     cd = {f: df, g: dg}
 
-    integrand = f[i]*g[i]
+    integrand = f[i] * g[i]
 
     i0, i1, i2, i3, i4 = [Index(count=c) for c in range(5)]
-    expected = as_tensor(df[i2, i1]*dv[i1], (i2,))[i0]*g[i0] +\
-        f[i0]*as_tensor(dg[i4, i3]*dv[i3], (i4,))[i0]
+    expected = (
+        as_tensor(df[i2, i1] * dv[i1], (i2,))[i0] * g[i0]
+        + f[i0] * as_tensor(dg[i4, i3] * dv[i3], (i4,))[i0]
+    )
 
-    F = integrand*dx
+    F = integrand * dx
     J = derivative(F, u, dv, cd)
     fd = compute_form_data(J)
     actual = fd.preprocessed_form.integrals()[0].integrand()
 
     # Tricky case! These are equal in representation except
     # that the outermost sum/indexsum are swapped.
     # Sampling the expressions instead of comparing representations.
     x = (0, 0)
     funcs = {dv: (13, 14), f: (1, 2), g: (3, 4), df: ((5, 6), (7, 8)), dg: ((9, 10), (11, 12))}
     self.assertEqual(replace(actual, fd.function_replace_map)(x, funcs), expected(x, funcs))
 
     # TODO: Add tests covering more cases, in particular mixed stuff
 
+
 # --- Some actual forms
 
 
 def testHyperElasticity(self):
     cell = interval
-    element = FiniteElement("CG", cell, 2)
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    element = FiniteElement("Lagrange", cell, 2, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (1,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     w = Coefficient(space)
     v = TestFunction(space)
     u = TrialFunction(space)
     b = Constant(domain)
     K = Constant(domain)
 
     dw = w.dx(0)
     dv = v.dx(0)
     du = v.dx(0)
 
     E = dw + dw**2 / 2
     E = variable(E)
-    Q = b*E**2
-    psi = K*(exp(Q)-1)
+    Q = b * E**2
+    psi = K * (exp(Q) - 1)
 
-    f = psi*dx
+    f = psi * dx
     F = derivative(f, w, v)
     J = derivative(F, w, u)
 
     form_data_f = compute_form_data(f)
     form_data_F = compute_form_data(F)
     form_data_J = compute_form_data(J)
 
@@ -623,26 +780,26 @@
 
     f_expression = strip_variables(f.integrals_by_type("cell")[0].integrand())
     F_expression = strip_variables(F.integrals_by_type("cell")[0].integrand())
     J_expression = strip_variables(J.integrals_by_type("cell")[0].integrand())
 
     # classes = set(c.__class__ for c in post_traversal(f_expression))
 
-    Kv = .2
-    bv = .3
-    dw = .5
-    dv = .7
-    du = .11
-    E = dw + dw**2 / 2.
-    Q = bv*E**2
+    Kv = 0.2
+    bv = 0.3
+    dw = 0.5
+    dv = 0.7
+    du = 0.11
+    E = dw + dw**2 / 2.0
+    Q = bv * E**2
     expQ = float(exp(Q))
-    psi = Kv*(expQ-1)
+    psi = Kv * (expQ - 1)
     fv = psi
-    Fv = 2*Kv*bv*E*(1+dw)*expQ*dv
-    Jv = 2*Kv*bv*expQ*dv*du*(E + (1+dw)**2*(2*bv*E**2 + 1))
+    Fv = 2 * Kv * bv * E * (1 + dw) * expQ * dv
+    Jv = 2 * Kv * bv * expQ * dv * du * (E + (1 + dw) ** 2 * (2 * bv * E**2 + 1))
 
     def Nv(x, derivatives):
         assert derivatives == (0,)
         return dv
 
     def Nu(x, derivatives):
         assert derivatives == (0,)
@@ -652,122 +809,119 @@
         assert derivatives == (0,)
         return dw
 
     mapping = {K: Kv, b: bv, w: Nw}
     fv2 = f_expression((0,), mapping)
     self.assertAlmostEqual(fv, fv2)
 
-    v, = form_data_F.original_form.arguments()
+    (v,) = form_data_F.original_form.arguments()
     mapping = {K: Kv, b: bv, v: Nv, w: Nw}
     Fv2 = F_expression((0,), mapping)
     self.assertAlmostEqual(Fv, Fv2)
 
     v, u = form_data_J.original_form.arguments()
     mapping = {K: Kv, b: bv, v: Nv, u: Nu, w: Nw}
     Jv2 = J_expression((0,), mapping)
     self.assertAlmostEqual(Jv, Jv2)
 
 
 def test_mass_derived_from_functional(self):
     cell = triangle
-    V = FiniteElement("CG", cell, 1)
+    V = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
 
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, V)
 
     v = TestFunction(space)
     u = TrialFunction(space)
     w = Coefficient(space)
 
-    f = (w**2/2)*dx
-    L = w*v*dx
-    a = u*v*dx  # noqa: F841
+    f = (w**2 / 2) * dx
+    L = w * v * dx
+    # a = u*v*dx
     F = derivative(f, w, v)
-    J1 = derivative(L, w, u)  # noqa: F841
-    J2 = derivative(F, w, u)  # noqa: F841
+    derivative(L, w, u)
+    derivative(F, w, u)
     # TODO: assert something
 
+
 # --- Interaction with replace
 
 
 def test_derivative_replace_works_together(self):
     cell = triangle
-    V = FiniteElement("CG", cell, 1)
+    V = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
 
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, V)
 
     v = TestFunction(space)
     u = TrialFunction(space)
     f = Coefficient(space)
     g = Coefficient(space)
 
-    M = cos(f)*sin(g)
+    M = cos(f) * sin(g)
     F = derivative(M, f, v)
     J = derivative(F, f, u)
     JR = replace(J, {f: g})
 
-    F2 = -sin(f)*v*sin(g)
-    J2 = -cos(f)*u*v*sin(g)
-    JR2 = -cos(g)*u*v*sin(g)
+    F2 = -sin(f) * v * sin(g)
+    J2 = -cos(f) * u * v * sin(g)
+    JR2 = -cos(g) * u * v * sin(g)
 
     assertEqualBySampling(F, F2)
     assertEqualBySampling(J, J2)
     assertEqualBySampling(JR, JR2)
 
 
 def test_index_simplification_handles_repeated_indices(self):
-    mesh = Mesh(VectorElement("P", quadrilateral, 1))
-    V = FunctionSpace(mesh, TensorElement("DQ", quadrilateral, 0))
+    mesh = Mesh(FiniteElement("Lagrange", quadrilateral, 1, (2,), identity_pullback, H1))
+    V = FunctionSpace(mesh, FiniteElement("DQ", quadrilateral, 0, (2, 2), identity_pullback, L2))
     K = JacobianInverse(mesh)
     G = outer(Identity(2), Identity(2))
-    i, j, k, l, m, n = indices(6)
-    A = as_tensor(K[m, i] * K[n, j] * G[i, j, k, l], (m, n, k, l))
+    i, j, k, L, m, n = indices(6)
+    A = as_tensor(K[m, i] * K[n, j] * G[i, j, k, L], (m, n, k, L))
     i, j = indices(2)
     # Can't use A[i, i, j, j] because UFL automagically index-sums
     # repeated indices in the __getitem__ call.
     Adiag = Indexed(A, MultiIndex((i, i, j, j)))
     A = as_tensor(Adiag, (i, j))
     v = TestFunction(V)
-    f = inner(A, v)*dx
+    f = inner(A, v) * dx
     fd = compute_form_data(f, do_apply_geometry_lowering=True)
-    integral, = fd.preprocessed_form.integrals()
+    (integral,) = fd.preprocessed_form.integrals()
     assert integral.integrand().ufl_free_indices == ()
 
 
 def test_index_simplification_reference_grad(self):
-    mesh = Mesh(VectorElement("P", quadrilateral, 1))
-    i, = indices(1)
+    mesh = Mesh(FiniteElement("Lagrange", quadrilateral, 1, (2,), identity_pullback, H1))
+    (i,) = indices(1)
     A = as_tensor(Indexed(Jacobian(mesh), MultiIndex((i, i))), (i,))
-    expr = apply_derivatives(apply_geometry_lowering(
-        apply_algebra_lowering(A[0])))
+    expr = apply_derivatives(apply_geometry_lowering(apply_algebra_lowering(A[0])))
     assert expr == ReferenceGrad(SpatialCoordinate(mesh))[0, 0]
     assert expr.ufl_free_indices == ()
     assert expr.ufl_shape == ()
 
 
 # --- Scratch space
 
+
 def test_foobar(self):
-    element = VectorElement("Lagrange", triangle, 1)
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    element = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     v = TestFunction(space)
-
     du = TrialFunction(space)
-
     U = Coefficient(space)
 
     def planarGrad(u):
-        return as_matrix([[u[0].dx(0), 0, u[0].dx(1)],
-                          [0, 0, 0],
-                          [u[1].dx(0), 0, u[1].dx(1)]])
+        return as_matrix([[u[0].dx(0), 0, u[0].dx(1)], [0, 0, 0], [u[1].dx(0), 0, u[1].dx(1)]])
 
     def epsilon(u):
-        return 0.5*(planarGrad(u)+planarGrad(u).T)
+        return 0.5 * (planarGrad(u) + planarGrad(u).T)
 
     def NS_a(u, v):
         return inner(epsilon(u), epsilon(v))
 
-    L = NS_a(U, v)*dx
-    a = derivative(L, U, du)  # noqa: F841
+    L = NS_a(U, v) * dx
+    _ = derivative(L, U, du)
     # TODO: assert something
```

### Comparing `fenics-ufl-2023.2.0/test/test_diff.py` & `fenics_ufl-2024.1.0.post0/test/test_diff.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,34 @@
 __authors__ = "Martin Sandve Alnæs"
 __date__ = "2009-02-17 -- 2014-10-14"
 
 import pytest
 
-from ufl import (Coefficient, FiniteElement, FunctionSpace, Mesh, SpatialCoordinate, VectorElement, as_vector, atan,
-                 cos, diff, exp, indices, ln, sin, tan, triangle, variable)
+from ufl import (
+    Coefficient,
+    FunctionSpace,
+    Mesh,
+    SpatialCoordinate,
+    as_vector,
+    atan,
+    cos,
+    diff,
+    exp,
+    indices,
+    ln,
+    sin,
+    tan,
+    triangle,
+    variable,
+)
 from ufl.algorithms import expand_derivatives
 from ufl.constantvalue import as_ufl
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 
 def get_variables():
     xv = None
     vv = 5.0
     return (xv, variable(vv))
 
@@ -39,106 +57,118 @@
 
 def testVariable(v):
     def f(v):
         return v
 
     def df(v):
         return as_ufl(1)
+
     _test(f, df)
 
 
 def testSum(v):
     def f(v):
         return v + 1
 
     def df(v):
         return as_ufl(1)
+
     _test(f, df)
 
 
 def testProduct(v):
     def f(v):
         return 3 * v
 
     def df(v):
         return as_ufl(3)
+
     _test(f, df)
 
 
 def testPower(v):
     def f(v):
-        return v ** 3
+        return v**3
 
     def df(v):
-        return 3 * v ** 2
+        return 3 * v**2
+
     _test(f, df)
 
 
 def testDivision(v):
     def f(v):
         return v / 3.0
 
     def df(v):
         return as_ufl(1.0 / 3.0)
+
     _test(f, df)
 
 
 def testDivision2(v):
     def f(v):
         return 3.0 / v
 
     def df(v):
-        return -3.0 / v ** 2
+        return -3.0 / v**2
+
     _test(f, df)
 
 
 def testExp(v):
     def f(v):
         return exp(v)
 
     def df(v):
         return exp(v)
+
     _test(f, df)
 
 
 def testLn(v):
     def f(v):
         return ln(v)
 
     def df(v):
         return 1.0 / v
+
     _test(f, df)
 
 
 def testSin(v):
     def f(v):
         return sin(v)
 
     def df(v):
         return cos(v)
+
     _test(f, df)
 
 
 def testCos(v):
     def f(v):
         return cos(v)
 
     def df(v):
         return -sin(v)
+
     _test(f, df)
 
 
 def testTan(v):
     def f(v):
         return tan(v)
 
     def df(v):
         return 2.0 / (cos(2.0 * v) + 1.0)
+
     _test(f, df)
 
+
 # TODO: Check the following tests. They run into strange math domain errors.
 # def testAsin(v):
 #    def f(v):  return asin(v)
 #    def df(v): return 1/sqrt(1.0 - v**2)
 #    _test(f, df)
 
 # def testAcos(v):
@@ -148,52 +178,55 @@
 
 
 def testAtan(v):
     def f(v):
         return atan(v)
 
     def df(v):
-        return 1 / (1.0 + v ** 2)
+        return 1 / (1.0 + v**2)
+
     _test(f, df)
 
 
 def testIndexSum(v):
     def f(v):
         # 3*v + 4*v**2 + 5*v**3
-        a = as_vector((v, v ** 2, v ** 3))
+        a = as_vector((v, v**2, v**3))
         b = as_vector((3, 4, 5))
-        i, = indices(1)
+        (i,) = indices(1)
         return a[i] * b[i]
 
     def df(v):
-        return 3 + 4 * 2 * v + 5 * 3 * v ** 2
+        return 3 + 4 * 2 * v + 5 * 3 * v**2
+
     _test(f, df)
 
 
 def testCoefficient():
-    coord_elem = VectorElement("P", triangle, 1, dim=3)
+    coord_elem = FiniteElement("Lagrange", triangle, 1, (3,), identity_pullback, H1)
     mesh = Mesh(coord_elem)
-    V = FunctionSpace(mesh, FiniteElement("P", triangle, 1))
+    V = FunctionSpace(mesh, FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1))
     v = Coefficient(V)
-    assert round(expand_derivatives(diff(v, v))-1.0, 7) == 0
+    assert round(expand_derivatives(diff(v, v)) - 1.0, 7) == 0
 
 
 def testDiffX():
     cell = triangle
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     x = SpatialCoordinate(domain)
     f = x[0] ** 2 * x[1] ** 2
-    i, = indices(1)
+    (i,) = indices(1)
     df1 = diff(f, x)
     df2 = as_vector(f.dx(i), i)
 
     xv = (2, 3)
     df10 = df1[0](xv)
     df11 = df1[1](xv)
     df20 = df2[0](xv)
     df21 = df2[1](xv)
     assert round(df10 - df20, 7) == 0
     assert round(df11 - df21, 7) == 0
     assert round(df10 - 2 * 2 * 9, 7) == 0
     assert round(df11 - 2 * 4 * 3, 7) == 0
 
+
 # TODO: More tests involving wrapper types and indices
```

### Comparing `fenics-ufl-2023.2.0/test/test_duals.py` & `fenics_ufl-2024.1.0.post0/test/test_duals.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,53 @@
 __authors__ = "India Marsden"
 __date__ = "2020-12-28"
 
 import pytest
 
-from ufl import (Action, Adjoint, Argument, Coargument, Coefficient, Cofunction, FiniteElement, FormSum, FunctionSpace,
-                 Matrix, Mesh, MixedFunctionSpace, TestFunction, TrialFunction, VectorElement, action, adjoint,
-                 derivative, dx, inner, interval, tetrahedron, triangle)
+from ufl import (
+    Action,
+    Adjoint,
+    Argument,
+    Coargument,
+    Coefficient,
+    Cofunction,
+    FormSum,
+    FunctionSpace,
+    Matrix,
+    Mesh,
+    MixedFunctionSpace,
+    TestFunction,
+    TrialFunction,
+    action,
+    adjoint,
+    derivative,
+    dx,
+    inner,
+    interval,
+    tetrahedron,
+    triangle,
+)
 from ufl.algorithms.ad import expand_derivatives
 from ufl.constantvalue import Zero
 from ufl.duals import is_dual, is_primal
+from ufl.finiteelement import FiniteElement
 from ufl.form import ZeroBaseForm
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 
 def test_mixed_functionspace(self):
     # Domains
-    domain_3d = Mesh(VectorElement("Lagrange", tetrahedron, 1))
-    domain_2d = Mesh(VectorElement("Lagrange", triangle, 1))
-    domain_1d = Mesh(VectorElement("Lagrange", interval, 1))
+    domain_3d = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
+    domain_2d = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
+    domain_1d = Mesh(FiniteElement("Lagrange", interval, 1, (1,), identity_pullback, H1))
     # Finite elements
-    f_1d = FiniteElement("CG", interval, 1)
-    f_2d = FiniteElement("CG", triangle, 1)
-    f_3d = FiniteElement("CG", tetrahedron, 1)
+    f_1d = FiniteElement("Lagrange", interval, 1, (), identity_pullback, H1)
+    f_2d = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    f_3d = FiniteElement("Lagrange", tetrahedron, 1, (), identity_pullback, H1)
     # Function spaces
     V_3d = FunctionSpace(domain_3d, f_3d)
     V_2d = FunctionSpace(domain_2d, f_2d)
     V_1d = FunctionSpace(domain_1d, f_1d)
 
     # MixedFunctionSpace = V_3d x V_2d x V_1d
     V = MixedFunctionSpace(V_3d, V_2d, V_1d)
@@ -43,16 +66,16 @@
 
     assert is_dual(V_dual)
     assert not is_dual(V)
     assert is_dual(V_mixed_dual)
 
 
 def test_dual_coefficients():
-    domain_2d = Mesh(VectorElement("Lagrange", triangle, 1))
-    f_2d = FiniteElement("CG", triangle, 1)
+    domain_2d = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
+    f_2d = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
     V = FunctionSpace(domain_2d, f_2d)
     V_dual = V.dual()
 
     v = Coefficient(V, count=1)
     u = Coefficient(V_dual, count=1)
     w = Cofunction(V_dual)
 
@@ -66,16 +89,16 @@
     assert not is_primal(w)
 
     with pytest.raises(ValueError):
         Cofunction(V)
 
 
 def test_dual_arguments():
-    domain_2d = Mesh(VectorElement("Lagrange", triangle, 1))
-    f_2d = FiniteElement("CG", triangle, 1)
+    domain_2d = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
+    f_2d = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
     V = FunctionSpace(domain_2d, f_2d)
     V_dual = V.dual()
 
     v = Argument(V, 1)
     u = Argument(V_dual, 2)
     w = Coargument(V_dual, 3)
 
@@ -89,19 +112,22 @@
     assert not is_primal(w)
 
     with pytest.raises(ValueError):
         Coargument(V, 4)
 
 
 def test_addition():
-    domain_2d = Mesh(VectorElement("Lagrange", triangle, 1))
-    f_2d = FiniteElement("CG", triangle, 1)
+    domain_2d = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
+    f_2d = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
     V = FunctionSpace(domain_2d, f_2d)
     V_dual = V.dual()
 
+    fvector_2d = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    W = FunctionSpace(domain_2d, fvector_2d)
+
     u = TrialFunction(V)
     v = TestFunction(V)
 
     # linear 1-form
     L = v * dx
     a = Cofunction(V_dual)
     res = L + a
@@ -125,18 +151,23 @@
     res += a
     assert res == a
     # Check __neg__
     res = L
     res -= ZeroBaseForm((v,))
     assert res == L
 
+    # Simplification with respect to ufl.Zero
+    a_W = Matrix(W, W)
+    res = a_W + Zero(W.value_shape)
+    assert res == a_W
+
 
 def test_scalar_mult():
-    domain_2d = Mesh(VectorElement("Lagrange", triangle, 1))
-    f_2d = FiniteElement("CG", triangle, 1)
+    domain_2d = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
+    f_2d = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
     V = FunctionSpace(domain_2d, f_2d)
     V_dual = V.dual()
 
     # linear 1-form
     a = Cofunction(V_dual)
     res = 2 * a
     assert isinstance(res, FormSum)
@@ -145,16 +176,16 @@
     a = Matrix(V, V)
     res = 2 * a
     assert isinstance(res, FormSum)
     assert res
 
 
 def test_adjoint():
-    domain_2d = Mesh(VectorElement("Lagrange", triangle, 1))
-    f_2d = FiniteElement("CG", triangle, 1)
+    domain_2d = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
+    f_2d = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
     V = FunctionSpace(domain_2d, f_2d)
     a = Matrix(V, V)
 
     adj = adjoint(a)
     res = 2 * adj
     assert isinstance(res, FormSum)
     assert res
@@ -164,19 +195,19 @@
     assert isinstance(res.components()[0], Adjoint)
 
     # Adjoint(Adjoint(.)) = Id
     assert adjoint(adj) == a
 
 
 def test_action():
-    domain_2d = Mesh(VectorElement("Lagrange", triangle, 1))
-    f_2d = FiniteElement("CG", triangle, 1)
+    domain_2d = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
+    f_2d = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
     V = FunctionSpace(domain_2d, f_2d)
-    domain_1d = Mesh(VectorElement("Lagrange", interval, 1))
-    f_1d = FiniteElement("CG", interval, 1)
+    domain_1d = Mesh(FiniteElement("Lagrange", interval, 1, (1,), identity_pullback, H1))
+    f_1d = FiniteElement("Lagrange", interval, 1, (), identity_pullback, H1)
     U = FunctionSpace(domain_1d, f_1d)
 
     a = Matrix(V, U)
     b = Matrix(V, U.dual())
     u = Coefficient(U)
     u_a = Argument(U, 0)
     v = Coefficient(V)
@@ -215,39 +246,43 @@
     res = action(b + b2, ustar)
     assert res == Action(b, ustar) + Action(b2, ustar)
 
     a2 = Matrix(V, U)
     u2 = Coefficient(U)
     u3 = Coefficient(U)
     # Check Action left-distributivity with Sum
-    # Add 3 Coefficients to check composition of Sum works fine since u + u2 + u3 => Sum(u, Sum(u2, u3))
+    # Add 3 Coefficients to check composition of Sum works fine since u
+    # + u2 + u3 => Sum(u, Sum(u2, u3))
     res = action(a, u + u2 + u3)
     assert res == Action(a, u3) + Action(a, u) + Action(a, u2)
     # Check Action right-distributivity with Sum
     res = action(a + a2, u)
     assert res == Action(a, u) + Action(a2, u)
 
 
 def test_differentiation():
-    domain_2d = Mesh(VectorElement("Lagrange", triangle, 1))
-    f_2d = FiniteElement("CG", triangle, 1)
+    domain_2d = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
+    f_2d = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
     V = FunctionSpace(domain_2d, f_2d)
-    domain_1d = Mesh(VectorElement("Lagrange", interval, 1))
-    f_1d = FiniteElement("CG", interval, 1)
+    domain_1d = Mesh(FiniteElement("Lagrange", interval, 1, (1,), identity_pullback, H1))
+    f_1d = FiniteElement("Lagrange", interval, 1, (), identity_pullback, H1)
     U = FunctionSpace(domain_1d, f_1d)
 
     u = Coefficient(U)
     v = Argument(U, 0)
     vstar = Argument(U.dual(), 0)
 
     # -- Cofunction -- #
     w = Cofunction(U.dual())
     dwdu = expand_derivatives(derivative(w, u))
     assert isinstance(dwdu, ZeroBaseForm)
-    assert dwdu.arguments() == (Argument(w.ufl_function_space().dual(), 0), Argument(u.ufl_function_space(), 1))
+    assert dwdu.arguments() == (
+        Argument(w.ufl_function_space().dual(), 0),
+        Argument(u.ufl_function_space(), 1),
+    )
     # Check compatibility with int/float
     assert dwdu == 0
 
     dwdw = expand_derivatives(derivative(w, w, vstar))
     assert dwdw == vstar
 
     dudw = expand_derivatives(derivative(u, w))
@@ -270,16 +305,18 @@
     assert dMdu.arguments() == M.arguments() + (Argument(u.ufl_function_space(), 2),)
     # Check compatibility with int/float
     assert dMdu == 0
 
     # -- Action -- #
     Ac = Action(w, u)
     dAcdu = derivative(Ac, u)
-    assert dAcdu == (action(adjoint(derivative(w, u), derivatives_expanded=True), u, derivatives_expanded=True)
-                     + action(w, derivative(u, u), derivatives_expanded=True))
+    assert dAcdu == (
+        action(adjoint(derivative(w, u), derivatives_expanded=True), u, derivatives_expanded=True)
+        + action(w, derivative(u, u), derivatives_expanded=True)
+    )
 
     dAcdu = expand_derivatives(dAcdu)
     # Since dw/du = 0
     assert dAcdu == Action(w, v)
 
     # -- Form sum -- #
     uhat = Argument(U, 1)
@@ -287,18 +324,29 @@
     Fs = M + inner(u * uhat, v) * dx
     dFsdu = expand_derivatives(derivative(Fs, u))
     # Distribute differentiation over FormSum components
     assert dFsdu == inner(what * uhat, v) * dx
 
 
 def test_zero_base_form_mult():
-    domain_2d = Mesh(VectorElement("Lagrange", triangle, 1))
-    f_2d = FiniteElement("CG", triangle, 1)
+    domain_2d = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
+    f_2d = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
     V = FunctionSpace(domain_2d, f_2d)
     v = Argument(V, 0)
     Z = ZeroBaseForm((v, v))
 
     u = Coefficient(V)
 
     Zu = Z * u
     assert Zu == action(Z, u)
     assert action(Zu, u) == ZeroBaseForm(())
+
+
+def test_base_form_call():
+    domain_2d = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
+    f_2d = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    V = FunctionSpace(domain_2d, f_2d)
+
+    # Check duality pairing
+    f = Coefficient(V)
+    c = Cofunction(V.dual())
+    assert c(f) == action(c, f)
```

### Comparing `fenics-ufl-2023.2.0/test/test_evaluate.py` & `fenics_ufl-2024.1.0.post0/test/test_evaluate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,46 @@
 __authors__ = "Martin Sandve Alnæs"
 __date__ = "2009-02-13 -- 2009-02-13"
 
 import math
 
-from ufl import (Argument, Coefficient, FiniteElement, FunctionSpace, Identity, Mesh, SpatialCoordinate, VectorElement,
-                 as_matrix, as_vector, cos, cross, det, dev, dot, exp, i, indices, inner, j, ln, outer, sin, skew, sqrt,
-                 sym, tan, tetrahedron, tr, triangle)
+from ufl import (
+    Argument,
+    Coefficient,
+    FunctionSpace,
+    Identity,
+    Mesh,
+    SpatialCoordinate,
+    as_matrix,
+    as_vector,
+    cos,
+    cross,
+    det,
+    dev,
+    dot,
+    exp,
+    i,
+    indices,
+    inner,
+    j,
+    ln,
+    outer,
+    sin,
+    skew,
+    sqrt,
+    sym,
+    tan,
+    tetrahedron,
+    tr,
+    triangle,
+)
 from ufl.constantvalue import as_ufl
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 
 def testScalars():
     s = as_ufl(123)
     e = s((5, 7))
     v = 123
     assert e == v
@@ -21,115 +51,117 @@
     e = s((5, 7))
     v = 0
     assert e == v
 
 
 def testIdentity():
     cell = triangle
-    ident = Identity(cell.geometric_dimension())
+    ident = Identity(cell.topological_dimension())
 
     s = 123 * ident[0, 0]
     e = s((5, 7))
     v = 123
     assert e == v
 
     s = 123 * ident[1, 0]
     e = s((5, 7))
     v = 0
     assert e == v
 
 
 def testCoords():
     cell = triangle
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     x = SpatialCoordinate(domain)
     s = x[0] + x[1]
     e = s((5, 7))
     v = 5 + 7
     assert e == v
 
 
 def testFunction1():
     cell = triangle
-    element = FiniteElement("CG", cell, 1)
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    element = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     f = Coefficient(space)
     s = 3 * f
     e = s((5, 7), {f: 123})
     v = 3 * 123
     assert e == v
 
 
 def testFunction2():
     cell = triangle
-    element = FiniteElement("CG", cell, 1)
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    element = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     f = Coefficient(space)
 
     def g(x):
         return x[0]
+
     s = 3 * f
     e = s((5, 7), {f: g})
     v = 3 * 5
     assert e == v
 
 
 def testArgument2():
     cell = triangle
-    element = FiniteElement("CG", cell, 1)
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    element = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     f = Argument(space, 2)
 
     def g(x):
         return x[0]
+
     s = 3 * f
     e = s((5, 7), {f: g})
     v = 3 * 5
     assert e == v
 
 
 def testAlgebra():
     cell = triangle
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     x = SpatialCoordinate(domain)
     s = 3 * (x[0] + x[1]) - 7 + x[0] ** (x[1] / 2)
     e = s((5, 7))
-    v = 3 * (5. + 7.) - 7 + 5. ** (7. / 2)
+    v = 3 * (5.0 + 7.0) - 7 + 5.0 ** (7.0 / 2)
     assert e == v
 
 
 def testIndexSum():
     cell = triangle
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     x = SpatialCoordinate(domain)
-    i, = indices(1)
+    (i,) = indices(1)
     s = x[i] * x[i]
     e = s((5, 7))
-    v = 5 ** 2 + 7 ** 2
+    v = 5**2 + 7**2
     assert e == v
 
 
 def testIndexSum2():
     cell = triangle
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     x = SpatialCoordinate(domain)
-    ident = Identity(cell.geometric_dimension())
+    ident = Identity(cell.topological_dimension())
     i, j = indices(2)
     s = (x[i] * x[j]) * ident[i, j]
     e = s((5, 7))
     # v = sum_i sum_j x_i x_j delta_ij = x_0 x_0 + x_1 x_1
-    v = 5 ** 2 + 7 ** 2
+    v = 5**2 + 7**2
     assert e == v
 
 
 def testMathFunctions():
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     x = SpatialCoordinate(domain)[0]
 
     s = sin(x)
     e = s((5, 7))
     v = math.sin(5)
     assert e == v
 
@@ -156,235 +188,225 @@
     s = sqrt(x)
     e = s((5, 7))
     v = math.sqrt(5)
     assert e == v
 
 
 def testListTensor():
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     x, y = SpatialCoordinate(domain)
 
     m = as_matrix([[x, y], [-y, -x]])
 
     s = m[0, 0] + m[1, 0] + m[0, 1] + m[1, 1]
     e = s((5, 7))
     v = 0
     assert e == v
 
     s = m[0, 0] * m[1, 0] * m[0, 1] * m[1, 1]
     e = s((5, 7))
-    v = 5 ** 2 * 7 ** 2
+    v = 5**2 * 7**2
     assert e == v
 
 
 def testComponentTensor1():
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     x = SpatialCoordinate(domain)
     m = as_vector(x[i], i)
 
     s = m[0] * m[1]
     e = s((5, 7))
     v = 5 * 7
     assert e == v
 
 
 def testComponentTensor2():
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     x = SpatialCoordinate(domain)
     xx = outer(x, x)
 
     m = as_matrix(xx[i, j], (i, j))
 
     s = m[0, 0] + m[1, 0] + m[0, 1] + m[1, 1]
     e = s((5, 7))
     v = 5 * 5 + 5 * 7 + 5 * 7 + 7 * 7
     assert e == v
 
 
 def testComponentTensor3():
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     x = SpatialCoordinate(domain)
     xx = outer(x, x)
 
     m = as_matrix(xx[i, j], (i, j))
 
     s = m[0, 0] * m[1, 0] * m[0, 1] * m[1, 1]
     e = s((5, 7))
     v = 5 * 5 * 5 * 7 * 5 * 7 * 7 * 7
     assert e == v
 
 
 def testCoefficient():
-    V = FiniteElement("CG", triangle, 1)
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    V = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, V)
     f = Coefficient(space)
-    e = f ** 2
+    e = f**2
 
     def eval_f(x):
         return x[0] * x[1] ** 2
-    assert e((3, 7), {f: eval_f}) == (3 * 7 ** 2) ** 2
+
+    assert e((3, 7), {f: eval_f}) == (3 * 7**2) ** 2
 
 
 def testCoefficientDerivative():
-    V = FiniteElement("CG", triangle, 1)
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    V = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, V)
     f = Coefficient(space)
     e = f.dx(0) ** 2 + f.dx(1) ** 2
 
     def eval_f(x, derivatives):
         if not derivatives:
             return eval_f.c * x[0] * x[1] ** 2
         # assume only first order derivative
-        d, = derivatives
+        (d,) = derivatives
         if d == 0:
             return eval_f.c * x[1] ** 2
         if d == 1:
             return eval_f.c * x[0] * 2 * x[1]
+
     # shows how to attach data to eval_f
     eval_f.c = 5
 
-    assert e((3, 7), {f: eval_f}) == (5 * 7 ** 2) ** 2 + (5 * 3 * 2 * 7) ** 2
+    assert e((3, 7), {f: eval_f}) == (5 * 7**2) ** 2 + (5 * 3 * 2 * 7) ** 2
 
 
 def test_dot():
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     x = SpatialCoordinate(domain)
     s = dot(x, 2 * x)
     e = s((5, 7))
     v = 2 * (5 * 5 + 7 * 7)
     assert e == v
 
 
 def test_inner():
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     x = SpatialCoordinate(domain)
     xx = as_matrix(((2 * x[0], 3 * x[0]), (2 * x[1], 3 * x[1])))
     s = inner(xx, 2 * xx)
     e = s((5, 7))
     v = 2 * ((5 * 2) ** 2 + (5 * 3) ** 2 + (7 * 2) ** 2 + (7 * 3) ** 2)
     assert e == v
 
 
 def test_outer():
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     x = SpatialCoordinate(domain)
     xx = outer(outer(x, x), as_vector((2, 3)))
     s = inner(xx, 2 * xx)
     e = s((5, 7))
-    v = 2 * (5 ** 2 + 7 ** 2) ** 2 * (2 ** 2 + 3 ** 2)
+    v = 2 * (5**2 + 7**2) ** 2 * (2**2 + 3**2)
     assert e == v
 
 
 def test_cross():
-    domain = Mesh(VectorElement("Lagrange", tetrahedron, 1))
+    domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
     x = SpatialCoordinate(domain)
     xv = (3, 5, 7)
 
     # Test cross product of triplets of orthogonal
     # vectors, where |a x b| = |a| |b|
     ts = [
-        [as_vector((x[0], 0, 0)),
-            as_vector((0, x[1], 0)),
-            as_vector((0, 0, x[2]))],
-        [as_vector((x[0], x[1], 0)),
-            as_vector((x[1], -x[0], 0)),
-            as_vector((0, 0, x[2]))],
-        [as_vector((0, x[0], x[1])),
-            as_vector((0, x[1], -x[0])),
-            as_vector((x[2], 0, 0))],
-        [as_vector((x[0], 0, x[1])),
-            as_vector((x[1], 0, -x[0])),
-            as_vector((0, x[2], 0))],
+        [as_vector((x[0], 0, 0)), as_vector((0, x[1], 0)), as_vector((0, 0, x[2]))],
+        [as_vector((x[0], x[1], 0)), as_vector((x[1], -x[0], 0)), as_vector((0, 0, x[2]))],
+        [as_vector((0, x[0], x[1])), as_vector((0, x[1], -x[0])), as_vector((x[2], 0, 0))],
+        [as_vector((x[0], 0, x[1])), as_vector((x[1], 0, -x[0])), as_vector((0, x[2], 0))],
     ]
     for t in ts:
         for a in range(3):
             for b in range(3):
                 cab = cross(t[a], t[b])
                 dab = dot(cab, cab)
                 eab = dab(xv)
                 tna = dot(t[a], t[a])(xv)
                 tnb = dot(t[b], t[b])(xv)
                 vab = tna * tnb if a != b else 0
                 assert eab == vab
 
 
 def xtest_dev():
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     x = SpatialCoordinate(domain)
     xv = (5, 7)
     xx = outer(x, x)
     s1 = dev(2 * xx)
     s2 = 2 * (xx - xx.T)  # FIXME
     e = inner(s1, s1)(xv)
     v = inner(s2, s2)(xv)
     assert e == v
 
 
 def test_skew():
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     x = SpatialCoordinate(domain)
     xv = (5, 7)
     xx = outer(x, x)
     s1 = skew(2 * xx)
-    s2 = (xx - xx.T)
+    s2 = xx - xx.T
     e = inner(s1, s1)(xv)
     v = inner(s2, s2)(xv)
     assert e == v
 
 
 def test_sym():
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     x = SpatialCoordinate(domain)
     xv = (5, 7)
     xx = outer(x, x)
     s1 = sym(2 * xx)
-    s2 = (xx + xx.T)
+    s2 = xx + xx.T
     e = inner(s1, s1)(xv)
     v = inner(s2, s2)(xv)
     assert e == v
 
 
 def test_tr():
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     x = SpatialCoordinate(domain)
     xv = (5, 7)
     xx = outer(x, x)
     s = tr(2 * xx)
     e = s(xv)
     v = 2 * sum(xv[i] ** 2 for i in (0, 1))
     assert e == v
 
 
 def test_det2D():
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     x = SpatialCoordinate(domain)
     xv = (5, 7)
     a, b = 6.5, -4
     xx = as_matrix(((x[0], x[1]), (a, b)))
     s = det(2 * xx)
     e = s(xv)
-    v = 2 ** 2 * (5 * b - 7 * a)
+    v = 2**2 * (5 * b - 7 * a)
     assert e == v
 
 
 def xtest_det3D():  # FIXME
     x = SpatialCoordinate(tetrahedron)
     xv = (5, 7, 9)
     a, b, c = 6.5, -4, 3
     d, e, f = 2, 3, 4
-    xx = as_matrix(((x[0], x[1], x[2]),
-                    (a, b, c),
-                    (d, e, f)))
+    xx = as_matrix(((x[0], x[1], x[2]), (a, b, c), (d, e, f)))
     s = det(2 * xx)
     e = s(xv)
-    v = 2 ** 3 * \
-        (xv[0] * (b * f - e * c) - xv[1] *
-         (a * f - c * d) + xv[2] * (a * e - b * d))
+    v = 2**3 * (xv[0] * (b * f - e * c) - xv[1] * (a * f - c * d) + xv[2] * (a * e - b * d))
     assert e == v
 
 
 def test_cofac():
     pass  # TODO
```

### Comparing `fenics-ufl-2023.2.0/test/test_expand_indices.py` & `fenics_ufl-2024.1.0.post0/test/test_expand_indices.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,31 +4,56 @@
 # Modified by Anders Logg, 2008
 # Modified by Garth N. Wells, 2009
 
 import math
 
 import pytest
 
-from ufl import (Coefficient, FiniteElement, FunctionSpace, Identity, Mesh, TensorElement, VectorElement, as_tensor,
-                 cos, det, div, dot, dx, exp, grad, i, inner, j, k, l, ln, nabla_div, nabla_grad, outer, sin, triangle)
+from ufl import (
+    Coefficient,
+    FunctionSpace,
+    Identity,
+    Mesh,
+    as_tensor,
+    cos,
+    det,
+    div,
+    dot,
+    dx,
+    exp,
+    grad,
+    i,
+    inner,
+    j,
+    k,
+    l,
+    ln,
+    nabla_div,
+    nabla_grad,
+    outer,
+    sin,
+    triangle,
+)
 from ufl.algorithms import compute_form_data, expand_derivatives, expand_indices
 from ufl.algorithms.renumbering import renumber_indices
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 # TODO: Test expand_indices2 throuroughly for correctness, then efficiency:
 # expand_indices, expand_indices2 = expand_indices2, expand_indices
 
 
 class Fixture:
-
     def __init__(self):
         cell = triangle
-        element = FiniteElement("Lagrange", cell, 1)
-        velement = VectorElement("Lagrange", cell, 1)
-        telement = TensorElement("Lagrange", cell, 1)
-        domain = Mesh(VectorElement("Lagrange", cell, 1))
+        element = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+        velement = FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1)
+        telement = FiniteElement("Lagrange", cell, 1, (2, 2), identity_pullback, H1)
+        domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
         space = FunctionSpace(domain, element)
         vspace = FunctionSpace(domain, velement)
         tspace = FunctionSpace(domain, telement)
         self.sf = Coefficient(space)
         self.sf2 = Coefficient(space)
         self.vf = Coefficient(vspace)
         self.tf = Coefficient(tspace)
@@ -106,30 +131,30 @@
 
         self.x = (1.23, 3.14)
         self.mapping = {self.sf: SF, self.sf2: SF2, self.vf: VF, self.tf: TF}
 
     def compare(self, f, value):
         debug = 0
         if debug:
-            print(('f', f))
+            print(("f", f))
         g = expand_derivatives(f)
         if debug:
-            print(('g', g))
+            print(("g", g))
         gv = g(self.x, self.mapping)
         assert abs(gv - value) < 1e-7
 
         g = expand_indices(g)
         if debug:
-            print(('g', g))
+            print(("g", g))
         gv = g(self.x, self.mapping)
         assert abs(gv - value) < 1e-7
 
         g = renumber_indices(g)
         if debug:
-            print(('g', g))
+            print(("g", g))
         gv = g(self.x, self.mapping)
         assert abs(gv - value) < 1e-7
 
 
 @pytest.fixture(scope="module")
 def fixt():
     # Workaround for quick pytest transition
@@ -142,83 +167,86 @@
     tf = fixt.tf
     compare = fixt.compare
 
     # Simple expressions with no indices or derivatives to expand
     compare(sf, 3)
     compare(sf + 1, 4)
     compare(sf - 2.5, 0.5)
-    compare(sf/2, 1.5)
-    compare(sf/0.5, 6)
+    compare(sf / 2, 1.5)
+    compare(sf / 0.5, 6)
     compare(sf**2, 9)
     compare(sf**0.5, 3**0.5)
     compare(sf**3, 27)
     compare(0.5**sf, 0.5**3)
-    compare(sf * (sf/6), 1.5)
+    compare(sf * (sf / 6), 1.5)
     compare(sin(sf), math.sin(3))
     compare(cos(sf), math.cos(3))
     compare(exp(sf), math.exp(3))
     compare(ln(sf), math.log(3))
 
     # Simple indexing
     compare(vf[0], 5)
     compare(vf[0] + 1, 6)
     compare(vf[0] - 2.5, 2.5)
-    compare(vf[0]/2, 2.5)
-    compare(vf[0]/0.5, 10)
-    compare(vf[0]**2, 25)
-    compare(vf[0]**0.5, 5**0.5)
-    compare(vf[0]**3, 125)
-    compare(0.5**vf[0], 0.5**5)
-    compare(vf[0] * (vf[0]/6), 5*(5./6))
+    compare(vf[0] / 2, 2.5)
+    compare(vf[0] / 0.5, 10)
+    compare(vf[0] ** 2, 25)
+    compare(vf[0] ** 0.5, 5**0.5)
+    compare(vf[0] ** 3, 125)
+    compare(0.5 ** vf[0], 0.5**5)
+    compare(vf[0] * (vf[0] / 6), 5 * (5.0 / 6))
     compare(sin(vf[0]), math.sin(5))
     compare(cos(vf[0]), math.cos(5))
     compare(exp(vf[0]), math.exp(5))
     compare(ln(vf[0]), math.log(5))
 
     # Double indexing
     compare(tf[1, 1], 19)
     compare(tf[1, 1] + 1, 20)
     compare(tf[1, 1] - 2.5, 16.5)
-    compare(tf[1, 1]/2, 9.5)
-    compare(tf[1, 1]/0.5, 38)
-    compare(tf[1, 1]**2, 19**2)
-    compare(tf[1, 1]**0.5, 19**0.5)
-    compare(tf[1, 1]**3, 19**3)
-    compare(0.5**tf[1, 1], 0.5**19)
-    compare(tf[1, 1] * (tf[1, 1]/6), 19*(19./6))
+    compare(tf[1, 1] / 2, 9.5)
+    compare(tf[1, 1] / 0.5, 38)
+    compare(tf[1, 1] ** 2, 19**2)
+    compare(tf[1, 1] ** 0.5, 19**0.5)
+    compare(tf[1, 1] ** 3, 19**3)
+    compare(0.5 ** tf[1, 1], 0.5**19)
+    compare(tf[1, 1] * (tf[1, 1] / 6), 19 * (19.0 / 6))
     compare(sin(tf[1, 1]), math.sin(19))
     compare(cos(tf[1, 1]), math.cos(19))
     compare(exp(tf[1, 1]), math.exp(19))
     compare(ln(tf[1, 1]), math.log(19))
 
 
 def test_expand_indices_index_sum(self, fixt):
     vf = fixt.vf
     tf = fixt.tf
     compare = fixt.compare
 
     # Basic index sums
-    compare(vf[i]*vf[i], 5*5+7*7)
-    compare(vf[j]*tf[i, j]*vf[i], 5*5*11 + 5*7*13 + 5*7*17 + 7*7*19)
-    compare(vf[j]*tf.T[j, i]*vf[i], 5*5*11 + 5*7*13 + 5*7*17 + 7*7*19)
+    compare(vf[i] * vf[i], 5 * 5 + 7 * 7)
+    compare(vf[j] * tf[i, j] * vf[i], 5 * 5 * 11 + 5 * 7 * 13 + 5 * 7 * 17 + 7 * 7 * 19)
+    compare(vf[j] * tf.T[j, i] * vf[i], 5 * 5 * 11 + 5 * 7 * 13 + 5 * 7 * 17 + 7 * 7 * 19)
     compare(tf[i, i], 11 + 19)
-    compare(tf[i, j]*(tf[j, i]+outer(vf, vf)[i, j]), (5*5+11)*11 + (7*5+17)*13 + (7*5+13)*17 + (7*7+19)*19)
+    compare(
+        tf[i, j] * (tf[j, i] + outer(vf, vf)[i, j]),
+        (5 * 5 + 11) * 11 + (7 * 5 + 17) * 13 + (7 * 5 + 13) * 17 + (7 * 7 + 19) * 19,
+    )
     compare(as_tensor(as_tensor(tf[i, j], (i, j))[k, l], (l, k))[i, i], 11 + 19)
 
 
 def test_expand_indices_derivatives(self, fixt):
     sf = fixt.sf
     vf = fixt.vf
     compare = fixt.compare
 
     # Basic derivatives
     compare(sf.dx(0), 0.3)
     compare(sf.dx(1), 0.31)
-    compare(sf.dx(i)*vf[i], 0.30*5 + 0.31*7)
-    compare(vf[j].dx(i)*vf[i].dx(j), 0.50*0.50 + 0.51*0.70 + 0.70*0.51 + 0.71*0.71)
+    compare(sf.dx(i) * vf[i], 0.30 * 5 + 0.31 * 7)
+    compare(vf[j].dx(i) * vf[i].dx(j), 0.50 * 0.50 + 0.51 * 0.70 + 0.70 * 0.51 + 0.71 * 0.71)
 
 
 def test_expand_indices_hyperelasticity(self, fixt):
     vf = fixt.vf
     compare = fixt.compare
 
     # Deformation gradient
@@ -233,46 +261,46 @@
     F11 = 1 + 0.71
     compare(F[0, 0], F00)
     compare(F[0, 1], F01)
     compare(F[1, 0], F10)
     compare(F[1, 1], F11)
 
     J = det(F)
-    compare(J, (1 + 0.50)*(1 + 0.71) - 0.70*0.51)
+    compare(J, (1 + 0.50) * (1 + 0.71) - 0.70 * 0.51)
 
     # Strain tensors
-    C = F.T*F
+    C = F.T * F
     # Cij = sum_k Fki Fkj
-    C00 = F00*F00 + F10*F10
-    C01 = F00*F01 + F10*F11
-    C10 = F01*F00 + F11*F10
-    C11 = F01*F01 + F11*F11
+    C00 = F00 * F00 + F10 * F10
+    C01 = F00 * F01 + F10 * F11
+    C10 = F01 * F00 + F11 * F10
+    C11 = F01 * F01 + F11 * F11
     compare(C[0, 0], C00)
     compare(C[0, 1], C01)
     compare(C[1, 0], C10)
     compare(C[1, 1], C11)
 
-    E = (C-ident)/2
-    E00 = (C00-1)/2
-    E01 = (C01)/2
-    E10 = (C10)/2
-    E11 = (C11-1)/2
+    E = (C - ident) / 2
+    E00 = (C00 - 1) / 2
+    E01 = (C01) / 2
+    E10 = (C10) / 2
+    E11 = (C11 - 1) / 2
     compare(E[0, 0], E00)
     compare(E[0, 1], E01)
     compare(E[1, 0], E10)
     compare(E[1, 1], E11)
 
     # Strain energy
     Q = inner(E, E)
     Qvalue = E00**2 + E01**2 + E10**2 + E11**2
     compare(Q, Qvalue)
 
     K = 0.5
-    psi = (K/2)*exp(Q)
-    compare(psi, 0.25*math.exp(Qvalue))
+    psi = (K / 2) * exp(Q)
+    compare(psi, 0.25 * math.exp(Qvalue))
 
 
 def test_expand_indices_div_grad(self, fixt):
     sf = fixt.sf
     sf2 = fixt.sf2
     vf = fixt.vf
     tf = fixt.tf
@@ -284,26 +312,29 @@
     a = div(grad(sf2))
     compare(a, 3.300 + 3.311)
 
     if 0:
         Dvf = grad(vf)
         Lvf = div(Dvf)
         Lvf2 = dot(Lvf, Lvf)
-        pp = compute_form_data(Lvf2*dx).preprocessed_form.integrals()[0].integrand()
-        print(('vf', vf.ufl_shape, str(vf)))
-        print(('Dvf', Dvf.ufl_shape, str(Dvf)))
-        print(('Lvf', Lvf.ufl_shape, str(Lvf)))
-        print(('Lvf2', Lvf2.ufl_shape, str(Lvf2)))
-        print(('pp', pp.ufl_shape, str(pp)))
+        pp = compute_form_data(Lvf2 * dx).preprocessed_form.integrals()[0].integrand()
+        print(("vf", vf.ufl_shape, str(vf)))
+        print(("Dvf", Dvf.ufl_shape, str(Dvf)))
+        print(("Lvf", Lvf.ufl_shape, str(Lvf)))
+        print(("Lvf2", Lvf2.ufl_shape, str(Lvf2)))
+        print(("pp", pp.ufl_shape, str(pp)))
 
     a = div(grad(vf))
-    compare(dot(a, a), (0.20+0.40)**2 + (0.21+0.41)**2)
+    compare(dot(a, a), (0.20 + 0.40) ** 2 + (0.21 + 0.41) ** 2)
 
     a = div(grad(tf))
-    compare(inner(a, a), (10.00+11.00)**2 + (10.01+11.01)**2 + (10.10+11.10)**2 + (10.11+11.11)**2)
+    compare(
+        inner(a, a),
+        (10.00 + 11.00) ** 2 + (10.01 + 11.01) ** 2 + (10.10 + 11.10) ** 2 + (10.11 + 11.11) ** 2,
+    )
 
 
 def test_expand_indices_nabla_div_grad(self, fixt):
     sf = fixt.sf
     sf2 = fixt.sf2
     vf = fixt.vf
     tf = fixt.tf
@@ -312,11 +343,14 @@
     a = nabla_div(nabla_grad(sf))
     compare(a, 0)
 
     a = nabla_div(nabla_grad(sf2))
     compare(a, 3.300 + 3.311)
 
     a = nabla_div(nabla_grad(vf))
-    compare(dot(a, a), (0.20+0.40)**2 + (0.21+0.41)**2)
+    compare(dot(a, a), (0.20 + 0.40) ** 2 + (0.21 + 0.41) ** 2)
 
     a = nabla_div(nabla_grad(tf))
-    compare(inner(a, a), (10.00+11.00)**2 + (10.01+11.01)**2 + (10.10+11.10)**2 + (10.11+11.11)**2)
+    compare(
+        inner(a, a),
+        (10.00 + 11.00) ** 2 + (10.01 + 11.01) ** 2 + (10.10 + 11.10) ** 2 + (10.11 + 11.11) ** 2,
+    )
```

### Comparing `fenics-ufl-2023.2.0/test/test_external_operator.py` & `fenics_ufl-2024.1.0.post0/test/test_external_operator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,62 @@
 """Test ExternalOperator object."""
 
 __authors__ = "Nacime Bouziani"
 __date__ = "2019-03-26"
 
 import pytest
 
-# This imports everything external code will see from ufl
-from ufl import (Action, Argument, Coefficient, Constant, FiniteElement, Form, FunctionSpace, Mesh, TestFunction,
-                 TrialFunction, VectorElement, action, adjoint, cos, derivative, dx, inner, sin, triangle)
+from ufl import (
+    Action,
+    Argument,
+    Coefficient,
+    Constant,
+    Form,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TrialFunction,
+    action,
+    adjoint,
+    cos,
+    derivative,
+    dx,
+    inner,
+    sin,
+    triangle,
+)
 from ufl.algorithms import expand_derivatives
 from ufl.algorithms.apply_derivatives import apply_derivatives
 from ufl.core.external_operator import ExternalOperator
+from ufl.finiteelement import FiniteElement
 from ufl.form import BaseForm
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 
 @pytest.fixture
 def domain_2d():
-    return Mesh(VectorElement("Lagrange", triangle, 1))
+    return Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
 
 
 @pytest.fixture
 def V1(domain_2d):
-    f1 = FiniteElement("CG", triangle, 1)
+    f1 = FiniteElement("CG", triangle, 1, (), identity_pullback, H1)
     return FunctionSpace(domain_2d, f1)
 
 
 @pytest.fixture
 def V2(domain_2d):
-    f1 = FiniteElement("CG", triangle, 2)
+    f1 = FiniteElement("CG", triangle, 2, (), identity_pullback, H1)
     return FunctionSpace(domain_2d, f1)
 
 
 @pytest.fixture
 def V3(domain_2d):
-    f1 = FiniteElement("CG", triangle, 3)
+    f1 = FiniteElement("CG", triangle, 3, (), identity_pullback, H1)
     return FunctionSpace(domain_2d, f1)
 
 
 def test_properties(V1):
     u = Coefficient(V1, count=0)
     r = Coefficient(V1, count=1)
 
@@ -56,49 +75,51 @@
     # Test __str__
     s = Coefficient(V1, count=2)
     t = Coefficient(V1, count=3)
     v0 = Argument(V1, 0)
     v1 = Argument(V1, 1)
 
     e = ExternalOperator(u, function_space=V1)
-    assert str(e) == 'e(w_0; v_0)'
+    assert str(e) == "e(w_0; v_0)"
 
     e = ExternalOperator(u, function_space=V1, derivatives=(1,))
-    assert str(e) == '∂e(w_0; v_0)/∂o1'
+    assert str(e) == "∂e(w_0; v_0)/∂o1"
 
-    e = ExternalOperator(u, r, 2 * s, t, function_space=V1, derivatives=(1, 0, 1, 2), argument_slots=(v0, v1))
-    assert str(e) == '∂e(w_0, w_1, 2 * w_2, w_3; v_1, v_0)/∂o1∂o3∂o4∂o4'
+    e = ExternalOperator(
+        u, r, 2 * s, t, function_space=V1, derivatives=(1, 0, 1, 2), argument_slots=(v0, v1)
+    )
+    assert str(e) == "∂e(w_0, w_1, 2 * w_2, w_3; v_1, v_0)/∂o1∂o3∂o4∂o4"
 
 
 def test_form(V1, V2):
     u = Coefficient(V1)
     m = Coefficient(V1)
     u_hat = TrialFunction(V1)
     v = TestFunction(V1)
 
     # F = N * v * dx
     N = ExternalOperator(u, m, function_space=V2)
     F = N * v * dx
     actual = derivative(F, u, u_hat)
 
-    vstar, = N.arguments()
+    (vstar,) = N.arguments()
     Nhat = TrialFunction(N.ufl_function_space())
 
     dNdu = N._ufl_expr_reconstruct_(u, m, derivatives=(1, 0), argument_slots=(vstar, u_hat))
     dFdN = Nhat * v * dx
     expected = Action(dFdN, dNdu)
 
     assert apply_derivatives(actual) == expected
 
     # F = N * u * v * dx
     N = ExternalOperator(u, m, function_space=V1)
     F = N * u * v * dx
     actual = derivative(F, u, u_hat)
 
-    vstar, = N.arguments()
+    (vstar,) = N.arguments()
     Nhat = TrialFunction(N.ufl_function_space())
 
     dNdu = N._ufl_expr_reconstruct_(u, m, derivatives=(1, 0), argument_slots=(vstar, u_hat))
     dFdu_partial = N * u_hat * v * dx
     dFdN = Nhat * u * v * dx
     expected = dFdu_partial + Action(dFdN, dNdu)
     assert apply_derivatives(actual) == expected
@@ -120,16 +141,16 @@
     assert N2.arguments() == N2.argument_slots()
 
     # Check coefficients
     assert N1.coefficients() == (u, m)
     assert N2.coefficients() == (s,)
 
     # Get v*
-    vstar_N1, = N1.arguments()
-    vstar_N2, = N2.arguments()
+    (vstar_N1,) = N1.arguments()
+    (vstar_N2,) = N2.arguments()
     assert vstar_N1.ufl_function_space().dual() == V1
     assert vstar_N2.ufl_function_space().dual() == V1
 
     u_hat = Argument(V1, 1)
     s_hat = Argument(V2, 1)
     w = Coefficient(V1)
     r = Coefficient(V2)
@@ -171,26 +192,31 @@
     assert dN1du_action.arguments() == (vstar_dN1du,)
 
     assert dN2du.arguments() == (vstar_dN2du, s_hat)
     assert dN2du_action.arguments() == (vstar_dN2du,)
 
     # Check argument slots
     assert dN1du.argument_slots() == (vstar_dN1du, u_hat)
-    assert dN2du.argument_slots() == (vstar_dN2du, - sin(s) * s_hat)
+    assert dN2du.argument_slots() == (vstar_dN2du, -sin(s) * s_hat)
 
 
 def test_extractions(domain_2d, V1):
-    from ufl.algorithms.analysis import (extract_arguments, extract_arguments_and_coefficients,
-                                         extract_base_form_operators, extract_coefficients, extract_constants)
+    from ufl.algorithms.analysis import (
+        extract_arguments,
+        extract_arguments_and_coefficients,
+        extract_base_form_operators,
+        extract_coefficients,
+        extract_constants,
+    )
 
     u = Coefficient(V1)
     c = Constant(domain_2d)
 
     e = ExternalOperator(u, c, function_space=V1)
-    vstar_e, = e.arguments()
+    (vstar_e,) = e.arguments()
 
     assert extract_coefficients(e) == [u]
     assert extract_arguments(e) == [vstar_e]
     assert extract_arguments_and_coefficients(e) == ([vstar_e], [u])
     assert extract_constants(e) == [c]
     assert extract_base_form_operators(e) == [e]
 
@@ -215,15 +241,15 @@
     assert extract_coefficients(F) == [u]
     assert extract_arguments(e) == [vstar_e, u_hat]
     assert extract_arguments_and_coefficients(e) == ([vstar_e, u_hat], [u])
     assert F.base_form_operators() == (e,)
 
     w = Coefficient(V1)
     e2 = ExternalOperator(w, e, function_space=V1)
-    vstar_e2, = e2.arguments()
+    (vstar_e2,) = e2.arguments()
 
     assert extract_coefficients(e2) == [u, w]
     assert extract_arguments(e2) == [vstar_e2, u_hat]
     assert extract_arguments_and_coefficients(e2) == ([vstar_e2, u_hat], [u, w])
     assert extract_base_form_operators(e2) == [e, e2]
 
     F = e2 * dx
@@ -236,46 +262,44 @@
 
 def get_external_operators(form_base):
     if isinstance(form_base, ExternalOperator):
         return (form_base,)
     elif isinstance(form_base, BaseForm):
         return form_base.base_form_operators()
     else:
-        raise ValueError('Expecting FormBase argument!')
+        raise ValueError("Expecting FormBase argument!")
 
 
 def test_adjoint_action_jacobian(V1, V2, V3):
-
     u = Coefficient(V1)
     m = Coefficient(V2)
 
     # N(u, m; v*)
     N = ExternalOperator(u, m, function_space=V3)
-    vstar_N, = N.arguments()
+    (vstar_N,) = N.arguments()
 
     # Arguments for the Gateaux-derivative
     def u_hat(number):
-        return Argument(V1, number)   # V1: degree 1 # dFdu.arguments()[-1]
+        return Argument(V1, number)  # V1: degree 1 # dFdu.arguments()[-1]
 
     def m_hat(number):
-        return Argument(V2, number)   # V2: degree 2 # dFdm.arguments()[-1]
+        return Argument(V2, number)  # V2: degree 2 # dFdm.arguments()[-1]
 
     def vstar_N(number):
         return Argument(V3.dual(), number)  # V3: degree 3
 
     # Coefficients for the action
     w = Coefficient(V1)  # for u
     p = Coefficient(V2)  # for m
 
     v2 = TestFunction(V2)
     v3 = TestFunction(V3)
     form_base_expressions = (N * dx, N * v2 * dx, N * v3 * dx)  # , N)
 
     for F in form_base_expressions:
-
         # Get test function
         v_F = F.arguments() if isinstance(F, Form) else ()
         # If we have a 0-form with an ExternalOperator: e.g. F = N * dx
         # => F.arguments() = (), because of form composition.
         # But we still need to make arguments with number 1 (i.e. n_arg = 1)
         # since at the external operator level, argument numbering is based on
         # the external operator arguments and not on the outer form arguments.
@@ -325,15 +349,14 @@
             action_dFdm_adj = action(dFdm_adj, q)
 
             assert action_dFdu_adj.arguments() == (u_hat(n_arg),)
             assert action_dFdm_adj.arguments() == (m_hat(n_arg),)
 
 
 def test_multiple_external_operators(V1, V2):
-
     u = Coefficient(V1)
     m = Coefficient(V1)
     w = Coefficient(V2)
 
     v = TestFunction(V1)
     v_hat = TrialFunction(V1)
     w_hat = TrialFunction(V2)
@@ -358,22 +381,26 @@
     F = (inner(N1, v) + inner(N2, v) + inner(N3, v)) * dx
 
     # dFdu = Action(dFdN1, dN1du) + Action(dFdN3, dN3du)
     dFdu = expand_derivatives(derivative(F, u))
     dFdN1 = inner(v_hat, v) * dx
     dFdN2 = inner(w_hat, v) * dx
     dFdN3 = inner(v_hat, v) * dx
-    dN1du = N1._ufl_expr_reconstruct_(u, m, derivatives=(1, 0), argument_slots=N1.arguments() + (v_hat,))
+    dN1du = N1._ufl_expr_reconstruct_(
+        u, m, derivatives=(1, 0), argument_slots=N1.arguments() + (v_hat,)
+    )
     dN3du = N3._ufl_expr_reconstruct_(u, derivatives=(1,), argument_slots=N3.arguments() + (v_hat,))
 
     assert dFdu == Action(dFdN1, dN1du) + Action(dFdN3, dN3du)
 
     # dFdm = Action(dFdN1, dN1dm)
     dFdm = expand_derivatives(derivative(F, m))
-    dN1dm = N1._ufl_expr_reconstruct_(u, m, derivatives=(0, 1), argument_slots=N1.arguments() + (v_hat,))
+    dN1dm = N1._ufl_expr_reconstruct_(
+        u, m, derivatives=(0, 1), argument_slots=N1.arguments() + (v_hat,)
+    )
 
     assert dFdm == Action(dFdN1, dN1dm)
 
     # dFdw = Action(dFdN2, dN2dw)
     dFdw = expand_derivatives(derivative(F, w))
     dN2dw = N2._ufl_expr_reconstruct_(w, derivatives=(1,), argument_slots=N2.arguments() + (w_hat,))
 
@@ -391,39 +418,48 @@
     #
     # Using the fact that Action is distributive, we have:
     #
     # dFdu = Action(∂F/∂N4, ∂N4/∂u) +
     #         Action(∂F/∂N4, Action(∂N4/∂N1, dN1/du))
     dFdu = expand_derivatives(derivative(F, u))
     dFdN4_partial = inner(v_hat, v) * dx
-    dN4dN1_partial = N4._ufl_expr_reconstruct_(N1, u, derivatives=(1, 0), argument_slots=N4.arguments() + (v_hat,))
-    dN4du_partial = N4._ufl_expr_reconstruct_(N1, u, derivatives=(0, 1), argument_slots=N4.arguments() + (v_hat,))
-
-    assert dFdu == Action(dFdN4_partial, Action(dN4dN1_partial, dN1du)) + Action(dFdN4_partial, dN4du_partial)
+    dN4dN1_partial = N4._ufl_expr_reconstruct_(
+        N1, u, derivatives=(1, 0), argument_slots=N4.arguments() + (v_hat,)
+    )
+    dN4du_partial = N4._ufl_expr_reconstruct_(
+        N1, u, derivatives=(0, 1), argument_slots=N4.arguments() + (v_hat,)
+    )
+
+    assert dFdu == Action(dFdN4_partial, Action(dN4dN1_partial, dN1du)) + Action(
+        dFdN4_partial, dN4du_partial
+    )
 
     # dFdm = Action(∂F/∂N4, Action(∂N4/∂N1, dN1/dm))
     dFdm = expand_derivatives(derivative(F, m))
 
     assert dFdm == Action(dFdN4_partial, Action(dN4dN1_partial, dN1dm))
 
-    # --- F = < N1(u, m; v*), v > + <N2(w; v*), v> + <N3(u; v*), v> + < N4(N1(u, m), u; v*), v > --- #
+    # --- F = < N1(u, m; v*), v > + <N2(w; v*), v> + <N3(u; v*), v> + <
+    # N4(N1(u, m), u; v*), v > --- #
 
     F = (inner(N1, v) + inner(N2, v) + inner(N3, v) + inner(N4, v)) * dx
 
     dFdu = expand_derivatives(derivative(F, u))
     assert dFdu == Action(dFdN1, dN1du) + Action(dFdN3, dN3du) + Action(
-        dFdN4_partial, Action(dN4dN1_partial, dN1du)) + Action(dFdN4_partial, dN4du_partial)
+        dFdN4_partial, Action(dN4dN1_partial, dN1du)
+    ) + Action(dFdN4_partial, dN4du_partial)
 
     dFdm = expand_derivatives(derivative(F, m))
     assert dFdm == Action(dFdN1, dN1dm) + Action(dFdN4_partial, Action(dN4dN1_partial, dN1dm))
 
     dFdw = expand_derivatives(derivative(F, w))
     assert dFdw == Action(dFdN2, dN2dw)
 
-    # --- F = < N5(N4(N1(u, m), u), u; v*), v > + < N1(u, m; v*), v > + < u * N5(N4(N1(u, m), u), u; v*), v >--- #
+    # --- F = < N5(N4(N1(u, m), u), u; v*), v > + < N1(u, m; v*), v > +
+    # < u * N5(N4(N1(u, m), u), u; v*), v >--- #
 
     F = (inner(N5, v) + inner(N1, v) + inner(u * N5, v)) * dx
 
     # dFdu = ∂F/∂u + Action(∂F/∂N1, dN1/du) + Action(∂F/∂N4, dN4/du) + Action(∂F/∂N5, dN5/du)
     #
     # where:
     #  - ∂F/∂u = inner(w * N5, v) * dx
@@ -433,14 +469,21 @@
     #  - dN5/du = ∂N5/∂u + Action(∂N5/∂N4, dN4/du)
     #           = ∂N5/∂u + Action(∂N5/∂N4, ∂N4/∂u) + Action(∂N5/∂N4, Action(∂N4/∂N1, dN1/du))
     # with w = TrialFunction(V1)
     w = TrialFunction(V1)
     dFdu_partial = inner(w * N5, v) * dx
     dFdN1_partial = inner(w, v) * dx
     dFdN5_partial = (inner(w, v) + inner(u * w, v)) * dx
-    dN5dN4_partial = N5._ufl_expr_reconstruct_(N4, u, derivatives=(1, 0), argument_slots=N4.arguments() + (w,))
-    dN5du_partial = N5._ufl_expr_reconstruct_(N4, u, derivatives=(0, 1), argument_slots=N4.arguments() + (w,))
-    dN5du = Action(dN5dN4_partial, Action(dN4dN1_partial, dN1du)) + Action(
-        dN5dN4_partial, dN4du_partial) + dN5du_partial
+    dN5dN4_partial = N5._ufl_expr_reconstruct_(
+        N4, u, derivatives=(1, 0), argument_slots=N4.arguments() + (w,)
+    )
+    dN5du_partial = N5._ufl_expr_reconstruct_(
+        N4, u, derivatives=(0, 1), argument_slots=N4.arguments() + (w,)
+    )
+    dN5du = (
+        Action(dN5dN4_partial, Action(dN4dN1_partial, dN1du))
+        + Action(dN5dN4_partial, dN4du_partial)
+        + dN5du_partial
+    )
 
     dFdu = expand_derivatives(derivative(F, u))
     assert dFdu == dFdu_partial + Action(dFdN1_partial, dN1du) + Action(dFdN5_partial, dN5du)
```

### Comparing `fenics-ufl-2023.2.0/test/test_ffcforms.py` & `fenics_ufl-2024.1.0.post0/test/test_ffcforms.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,213 +9,232 @@
 __date__ = "2008-04-09 -- 2008-09-26"
 __copyright__ = "Copyright (C) 2008 Anders Logg et al."
 __license__ = "GNU GPL version 3 or any later version"
 
 # Examples copied from the FFC demo directory, examples contributed
 # by Johan Jansson, Kristian Oelgaard, Marie Rognes, and Garth Wells.
 
-from ufl import (Coefficient, Constant, Dx, FacetNormal, FiniteElement, FunctionSpace, Mesh, TensorElement,
-                 TestFunction, TestFunctions, TrialFunction, TrialFunctions, VectorConstant, VectorElement, avg, curl,
-                 div, dot, ds, dS, dx, grad, i, inner, j, jump, lhs, rhs, sqrt, tetrahedron, triangle)
+from ufl import (
+    Coefficient,
+    Constant,
+    Dx,
+    FacetNormal,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TestFunctions,
+    TrialFunction,
+    TrialFunctions,
+    VectorConstant,
+    avg,
+    curl,
+    div,
+    dot,
+    dS,
+    ds,
+    dx,
+    grad,
+    i,
+    inner,
+    j,
+    jump,
+    lhs,
+    rhs,
+    sqrt,
+    tetrahedron,
+    triangle,
+)
+from ufl.finiteelement import FiniteElement, MixedElement
+from ufl.pullback import contravariant_piola, covariant_piola, identity_pullback
+from ufl.sobolevspace import H1, L2, HCurl, HDiv
 
 
 def testConstant():
-    element = FiniteElement("Lagrange", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
 
     c = Constant(domain)
     d = VectorConstant(domain)
 
-    a = c * dot(grad(v), grad(u)) * dx  # noqa: F841
+    _ = c * dot(grad(v), grad(u)) * dx
 
     # FFC notation: L = dot(d, grad(v))*dx
-    L = inner(d, grad(v)) * dx  # noqa: F841
+    _ = inner(d, grad(v)) * dx
 
 
 def testElasticity():
-    element = VectorElement("Lagrange", "tetrahedron", 1)
-    domain = Mesh(VectorElement("Lagrange", "tetrahedron", 1))
+    element = FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
 
     def eps(v):
         # FFC notation: return grad(v) + transp(grad(v))
         return grad(v) + (grad(v)).T
 
     # FFC notation: a = 0.25*dot(eps(v), eps(u))*dx
-    a = 0.25 * inner(eps(v), eps(u)) * dx  # noqa: F841
+    _ = 0.25 * inner(eps(v), eps(u)) * dx
 
 
 def testEnergyNorm():
-    element = FiniteElement("Lagrange", "tetrahedron", 1)
-    domain = Mesh(VectorElement("Lagrange", "tetrahedron", 1))
+    element = FiniteElement("Lagrange", tetrahedron, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = Coefficient(space)
-    a = (v * v + dot(grad(v), grad(v))) * dx  # noqa: F841
+    _ = (v * v + dot(grad(v), grad(v))) * dx
 
 
 def testEquation():
-    element = FiniteElement("Lagrange", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     k = 0.1
 
     v = TestFunction(space)
     u = TrialFunction(space)
     u0 = Coefficient(space)
 
     F = v * (u - u0) * dx + k * dot(grad(v), grad(0.5 * (u0 + u))) * dx
 
-    a = lhs(F)  # noqa: F841
-    L = rhs(F)  # noqa: F841
+    _ = lhs(F)
+    _ = rhs(F)
 
 
 def testFunctionOperators():
-    element = FiniteElement("Lagrange", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
     f = Coefficient(space)
     g = Coefficient(space)
 
     # FFC notation: a = sqrt(1/modulus(1/f))*sqrt(g)*dot(grad(v), grad(u))*dx
     # + v*u*sqrt(f*g)*g*dx
-    a = sqrt(1 / abs(1 / f)) * sqrt(g) * dot(grad(v), grad(u)) * dx + v * u * sqrt(f * g) * g * dx  # noqa: F841
+    _ = sqrt(1 / abs(1 / f)) * sqrt(g) * dot(grad(v), grad(u)) * dx + v * u * sqrt(f * g) * g * dx
 
 
 def testHeat():
-    element = FiniteElement("Lagrange", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u1 = TrialFunction(space)
     u0 = Coefficient(space)
     c = Coefficient(space)
     f = Coefficient(space)
     k = Constant(domain)
 
-    a = v * u1 * dx + k * c * dot(grad(v), grad(u1)) * dx  # noqa: F841
-    L = v * u0 * dx + k * v * f * dx  # noqa: F841
+    _ = v * u1 * dx + k * c * dot(grad(v), grad(u1)) * dx
+    _ = v * u0 * dx + k * v * f * dx
 
 
 def testMass():
-    element = FiniteElement("Lagrange", "tetrahedron", 3)
-    domain = Mesh(VectorElement("Lagrange", "tetrahedron", 1))
+    element = FiniteElement("Lagrange", tetrahedron, 3, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
-
     v = TestFunction(space)
     u = TrialFunction(space)
-
-    a = v * u * dx  # noqa: F841
+    _ = v * u * dx
 
 
 def testMixedMixedElement():
-    P3 = FiniteElement("Lagrange", "triangle", 3)
-
-    element = (P3 * P3) * (P3 * P3)  # noqa: F841
+    P3 = FiniteElement("Lagrange", triangle, 3, (), identity_pullback, H1)
+    MixedElement([[P3, P3], [P3, P3]])
 
 
 def testMixedPoisson():
     q = 1
+    BDM = FiniteElement("Brezzi-Douglas-Marini", triangle, q, (2,), contravariant_piola, HDiv)
+    DG = FiniteElement("Discontinuous Lagrange", triangle, q - 1, (), identity_pullback, L2)
 
-    BDM = FiniteElement("Brezzi-Douglas-Marini", "triangle", q)
-    DG = FiniteElement("Discontinuous Lagrange", "triangle", q - 1)
-
-    mixed_element = BDM * DG
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    mixed_element = MixedElement([BDM, DG])
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, mixed_element)
 
     (tau, w) = TestFunctions(space)
     (sigma, u) = TrialFunctions(space)
-
     f = Coefficient(FunctionSpace(domain, DG))
-
-    a = (dot(tau, sigma) - div(tau) * u + w * div(sigma)) * dx  # noqa: F841
-    L = w * f * dx  # noqa: F841
+    _ = (dot(tau, sigma) - div(tau) * u + w * div(sigma)) * dx
+    _ = w * f * dx
 
 
 def testNavierStokes():
-    element = VectorElement("Lagrange", "tetrahedron", 1)
-    domain = Mesh(VectorElement("Lagrange", "tetrahedron", 1))
+    element = FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
-
     w = Coefficient(space)
 
     # FFC notation: a = v[i]*w[j]*D(u[i], j)*dx
-    a = v[i] * w[j] * Dx(u[i], j) * dx  # noqa: F841
+    _ = v[i] * w[j] * Dx(u[i], j) * dx
 
 
 def testNeumannProblem():
-    element = VectorElement("Lagrange", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
     f = Coefficient(space)
     g = Coefficient(space)
 
     # FFC notation: a = dot(grad(v), grad(u))*dx
-    a = inner(grad(v), grad(u)) * dx  # noqa: F841
+    _ = inner(grad(v), grad(u)) * dx
 
     # FFC notation: L = dot(v, f)*dx + dot(v, g)*ds
-    L = inner(v, f) * dx + inner(v, g) * ds  # noqa: F841
+    _ = inner(v, f) * dx + inner(v, g) * ds
 
 
 def testOptimization():
-    element = FiniteElement("Lagrange", "triangle", 3)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 3, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
-
     v = TestFunction(space)
     u = TrialFunction(space)
     f = Coefficient(space)
-
-    a = dot(grad(v), grad(u)) * dx  # noqa: F841
-    L = v * f * dx  # noqa: F841
+    _ = dot(grad(v), grad(u)) * dx
+    _ = v * f * dx
 
 
 def testP5tet():
-    element = FiniteElement("Lagrange", tetrahedron, 5)  # noqa: F841
+    FiniteElement("Lagrange", tetrahedron, 5, (), identity_pullback, H1)
 
 
 def testP5tri():
-    element = FiniteElement("Lagrange", triangle, 5)  # noqa: F841
+    FiniteElement("Lagrange", triangle, 5, (), identity_pullback, H1)
 
 
 def testPoissonDG():
-    element = FiniteElement("Discontinuous Lagrange", triangle, 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Discontinuous Lagrange", triangle, 1, (), identity_pullback, L2)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
     f = Coefficient(space)
-
     n = FacetNormal(domain)
 
     # FFC notation: h = MeshSize(domain), not supported by UFL
     h = Constant(domain)
 
     gN = Coefficient(space)
-
     alpha = 4.0
     gamma = 8.0
 
     # FFC notation
     # a = dot(grad(v), grad(u))*dx \
     #    - dot(avg(grad(v)), jump(u, n))*dS \
     #    - dot(jump(v, n), avg(grad(u)))*dS \
@@ -223,194 +242,192 @@
     #    - dot(grad(v), mult(u,n))*ds \
     #    - dot(mult(v,n), grad(u))*ds \
     #    + gamma/h*v*u*ds
 
     a = inner(grad(v), grad(u)) * dx
     a -= inner(avg(grad(v)), jump(u, n)) * dS
     a -= inner(jump(v, n), avg(grad(u))) * dS
-    a += alpha / h('+') * dot(jump(v, n), jump(u, n)) * dS
+    a += alpha / h("+") * dot(jump(v, n), jump(u, n)) * dS
     a -= inner(grad(v), u * n) * ds
     a -= inner(u * n, grad(u)) * ds
     a += gamma / h * v * u * ds
 
-    L = v * f * dx + v * gN * ds  # noqa: F841
+    _ = v * f * dx + v * gN * ds
 
 
 def testPoisson():
-    element = FiniteElement("Lagrange", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
     f = Coefficient(space)
 
     # Note: inner() also works
-    a = dot(grad(v), grad(u)) * dx  # noqa: F841
-    L = v * f * dx  # noqa: F841
+    _ = dot(grad(v), grad(u)) * dx
+    _ = v * f * dx
 
 
 def testPoissonSystem():
-    element = VectorElement("Lagrange", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
     f = Coefficient(space)
 
     # FFC notation: a = dot(grad(v), grad(u))*dx
-    a = inner(grad(v), grad(u)) * dx  # noqa: F841
+    _ = inner(grad(v), grad(u)) * dx
 
     # FFC notation: L = dot(v, f)*dx
-    L = inner(v, f) * dx  # noqa: F841
+    _ = inner(v, f) * dx
 
 
 def testProjection():
     # Projections are not supported by UFL and have been broken
     # in FFC for a while. For DOLFIN, the current (global) L^2
     # projection can be extended to handle also local projections.
 
-    P1 = FiniteElement("Lagrange", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    P1 = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, P1)
-
-    v = TestFunction(space)  # noqa: F841
-    f = Coefficient(space)  # noqa: F841
+    _ = TestFunction(space)
+    _ = Coefficient(space)
 
     # pi0 = Projection(P0)
     # pi1 = Projection(P1)
     # pi2 = Projection(P2)
     #
     # a = v*(pi0(f) + pi1(f) + pi2(f))*dx
 
 
 def testQuadratureElement():
-    element = FiniteElement("Lagrange", "triangle", 2)
+    element = FiniteElement("Lagrange", triangle, 2, (), identity_pullback, H1)
 
     # FFC notation:
-    # QE = QuadratureElement("triangle", 3)
-    # sig = VectorQuadratureElement("triangle", 3)
+    # QE = QuadratureElement(triangle, 3)
+    # sig = VectorQuadratureElement(triangle, 3)
 
-    QE = FiniteElement("Quadrature", "triangle", 3)
-    sig = VectorElement("Quadrature", "triangle", 3)
+    QE = FiniteElement("Quadrature", triangle, 3, (), identity_pullback, L2)
+    sig = FiniteElement("Quadrature", triangle, 3, (2,), identity_pullback, L2)
 
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
     u0 = Coefficient(space)
     C = Coefficient(FunctionSpace(domain, QE))
     sig0 = Coefficient(FunctionSpace(domain, sig))
     f = Coefficient(space)
 
-    a = v.dx(i) * C * u.dx(i) * dx + v.dx(i) * 2 * u0 * u * u0.dx(i) * dx  # noqa: F841
-    L = v * f * dx - dot(grad(v), sig0) * dx  # noqa: F841
+    _ = v.dx(i) * C * u.dx(i) * dx + v.dx(i) * 2 * u0 * u * u0.dx(i) * dx
+    _ = v * f * dx - dot(grad(v), sig0) * dx
 
 
 def testStokes():
     # UFLException: Shape mismatch in sum.
 
-    P2 = VectorElement("Lagrange", "triangle", 2)
-    P1 = FiniteElement("Lagrange", "triangle", 1)
-    TH = P2 * P1
+    P2 = FiniteElement("Lagrange", triangle, 2, (2,), identity_pullback, H1)
+    P1 = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    TH = MixedElement([P2, P1])
 
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     th_space = FunctionSpace(domain, TH)
     p2_space = FunctionSpace(domain, P2)
 
     (v, q) = TestFunctions(th_space)
     (u, p) = TrialFunctions(th_space)
-
     f = Coefficient(p2_space)
 
     # FFC notation:
     # a = (dot(grad(v), grad(u)) - div(v)*p + q*div(u))*dx
-    a = (inner(grad(v), grad(u)) - div(v) * p + q * div(u)) * dx  # noqa: F841
-
-    L = dot(v, f) * dx  # noqa: F841
+    _ = (inner(grad(v), grad(u)) - div(v) * p + q * div(u)) * dx
+    _ = dot(v, f) * dx
 
 
 def testSubDomain():
-    element = FiniteElement("CG", "tetrahedron", 1)
-    domain = Mesh(VectorElement("Lagrange", "tetrahedron", 1))
+    element = FiniteElement("Lagrange", tetrahedron, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
-
     f = Coefficient(space)
-
-    M = f * dx(2) + f * ds(5)  # noqa: F841
+    _ = f * dx(2) + f * ds(5)
 
 
 def testSubDomains():
-    element = FiniteElement("CG", "tetrahedron", 1)
-    domain = Mesh(VectorElement("Lagrange", "tetrahedron", 1))
+    element = FiniteElement("Lagrange", tetrahedron, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
-
     a = v * u * dx(0) + 10.0 * v * u * dx(1) + v * u * ds(0) + 2.0 * v * u * ds(1)
-    a += v('+') * u('+') * dS(0) + 4.3 * v('+') * u('+') * dS(1)
+    a += v("+") * u("+") * dS(0) + 4.3 * v("+") * u("+") * dS(1)
 
 
 def testTensorWeightedPoisson():
     # FFC notation:
-    # P1 = FiniteElement("Lagrange", "triangle", 1)
-    # P0 = FiniteElement("Discontinuous Lagrange", "triangle", 0)
+    # P1 = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    # P0 = FiniteElement("Discontinuous Lagrange", triangle, 0, (), identity_pullback, L2)
     #
     # v = TestFunction(P1)
     # u = TrialFunction(P1)
     # f = Coefficient(P1)
     #
     # c00 = Coefficient(P0)
     # c01 = Coefficient(P0)
     # c10 = Coefficient(P0)
     # c11 = Coefficient(P0)
     #
     # C = [[c00, c01], [c10, c11]]
     #
     # a = dot(grad(v), mult(C, grad(u)))*dx
 
-    P1 = FiniteElement("Lagrange", "triangle", 1)
-    P0 = TensorElement("Discontinuous Lagrange", "triangle", 0, shape=(2, 2))
+    P1 = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    P0 = FiniteElement("Discontinuous Lagrange", triangle, 0, (2, 2), identity_pullback, L2)
 
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     p1_space = FunctionSpace(domain, P1)
     p0_space = FunctionSpace(domain, P0)
 
     v = TestFunction(p1_space)
     u = TrialFunction(p1_space)
     C = Coefficient(p0_space)
-
-    a = inner(grad(v), C * grad(u)) * dx  # noqa: F841
+    _ = inner(grad(v), C * grad(u)) * dx
 
 
 def testVectorLaplaceGradCurl():
     def HodgeLaplaceGradCurl(space, fspace):
         (tau, v) = TestFunctions(space)
         (sigma, u) = TrialFunctions(space)
         f = Coefficient(fspace)
 
         # FFC notation: a = (dot(tau, sigma) - dot(grad(tau), u) + dot(v,
         # grad(sigma)) + dot(curl(v), curl(u)))*dx
-        a = (inner(tau, sigma) - inner(grad(tau), u) +
-             inner(v, grad(sigma)) + inner(curl(v), curl(u))) * dx
+        a = (
+            inner(tau, sigma)
+            - inner(grad(tau), u)
+            + inner(v, grad(sigma))
+            + inner(curl(v), curl(u))
+        ) * dx
 
         # FFC notation: L = dot(v, f)*dx
         L = inner(v, f) * dx
 
         return [a, L]
 
-    shape = "tetrahedron"
+    shape = tetrahedron
     order = 1
 
-    GRAD = FiniteElement("Lagrange", shape, order)
+    GRAD = FiniteElement("Lagrange", shape, order, (), identity_pullback, H1)
 
     # FFC notation: CURL = FiniteElement("Nedelec", shape, order-1)
-    CURL = FiniteElement("N1curl", shape, order)
+    CURL = FiniteElement("N1curl", shape, order, (3,), covariant_piola, HCurl)
 
-    VectorLagrange = VectorElement("Lagrange", shape, order + 1)
-    domain = Mesh(VectorElement("Lagrange", shape, 1))
+    VectorLagrange = FiniteElement("Lagrange", shape, order + 1, (3,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", shape, 1, (3,), identity_pullback, H1))
 
-    [a, L] = HodgeLaplaceGradCurl(FunctionSpace(domain, GRAD * CURL),
-                                  FunctionSpace(domain, VectorLagrange))
+    [a, L] = HodgeLaplaceGradCurl(
+        FunctionSpace(domain, MixedElement([GRAD, CURL])), FunctionSpace(domain, VectorLagrange)
+    )
```

### Comparing `fenics-ufl-2023.2.0/test/test_form.py` & `fenics_ufl-2024.1.0.post0/test/test_form.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,81 +1,100 @@
 import pytest
 
-from ufl import (Coefficient, Cofunction, FiniteElement, Form, FormSum, FunctionSpace, Mesh, SpatialCoordinate,
-                 TestFunction, TrialFunction, VectorElement, dot, ds, dx, grad, inner, nabla_grad, triangle)
+from ufl import (
+    Coefficient,
+    Cofunction,
+    Form,
+    FormSum,
+    FunctionSpace,
+    Mesh,
+    SpatialCoordinate,
+    TestFunction,
+    TrialFunction,
+    dot,
+    ds,
+    dx,
+    grad,
+    inner,
+    nabla_grad,
+    triangle,
+)
+from ufl.finiteelement import FiniteElement
 from ufl.form import BaseForm
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 
 @pytest.fixture
 def element():
     cell = triangle
-    element = FiniteElement("Lagrange", cell, 1)
+    element = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
     return element
 
 
 @pytest.fixture
 def domain():
     cell = triangle
-    return Mesh(VectorElement("Lagrange", cell, 1))
+    return Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
 
 
 @pytest.fixture
 def mass(domain):
     cell = triangle
-    element = FiniteElement("Lagrange", cell, 1)
+    element = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
     space = FunctionSpace(domain, element)
     v = TestFunction(space)
     u = TrialFunction(space)
     return u * v * dx
 
 
 @pytest.fixture
 def stiffness(domain):
     cell = triangle
-    element = FiniteElement("Lagrange", cell, 1)
+    element = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
     space = FunctionSpace(domain, element)
     v = TestFunction(space)
     u = TrialFunction(space)
     return inner(grad(u), grad(v)) * dx
 
 
 @pytest.fixture
 def convection(domain):
     cell = triangle
-    element = VectorElement("Lagrange", cell, 1)
+    element = FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1)
     space = FunctionSpace(domain, element)
     v = TestFunction(space)
     u = TrialFunction(space)
     w = Coefficient(space)
     return dot(dot(w, nabla_grad(u)), v) * dx
 
 
 @pytest.fixture
 def load(domain):
     cell = triangle
-    element = FiniteElement("Lagrange", cell, 1)
+    element = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
     space = FunctionSpace(domain, element)
     f = Coefficient(space)
     v = TestFunction(space)
     return f * v * dx
 
 
 @pytest.fixture
 def boundary_load(domain):
     cell = triangle
-    element = FiniteElement("Lagrange", cell, 1)
+    element = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
     space = FunctionSpace(domain, element)
     f = Coefficient(space)
     v = TestFunction(space)
     return f * v * ds
 
 
 def test_form_arguments(mass, stiffness, convection, load):
     v, u = mass.arguments()
-    f, = load.coefficients()
+    (f,) = load.coefficients()
 
     assert v.number() == 0
     assert u.number() == 1
     assert stiffness.arguments() == (v, u)
     assert load.arguments() == (v,)
 
     assert (v * dx).arguments() == (v,)
@@ -96,16 +115,16 @@
     assert (g * dx + f * ds).coefficients() == (f, g)
     assert (g * dx(1) + f * dx(2)).coefficients() == (f, g)
     assert (g * v * dx + f * v * dx(2)).coefficients() == (f, g)
 
 
 def test_form_domains():
     cell = triangle
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
-    element = FiniteElement("Lagrange", cell, 1)
+    element = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     V = FunctionSpace(domain, element)
 
     v = TestFunction(V)
     f = Coefficient(V)
     x = SpatialCoordinate(domain)[0]
 
     assert (x * dx).ufl_domains() == (domain,)
@@ -128,49 +147,50 @@
     assert mass.integrals_by_type("exterior_facet") == ()
     assert isinstance(boundary_load.integrals_by_type("cell"), tuple)
     assert len(boundary_load.integrals_by_type("cell")) == 0
     assert len(boundary_load.integrals_by_type("exterior_facet")) == 1
 
 
 def test_form_call():
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
-    element = FiniteElement("Lagrange", triangle, 1)
+    element = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     V = FunctionSpace(domain, element)
     v = TestFunction(V)
     u = TrialFunction(V)
     f = Coefficient(V)
     g = Coefficient(V)
-    a = g*inner(grad(v), grad(u))*dx
+    a = g * inner(grad(v), grad(u)) * dx
     M = a(f, f, coefficients={g: 1})
-    assert M == grad(f)**2*dx
+    assert M == grad(f) ** 2 * dx
 
     import sys
+
     if sys.version_info.major >= 3 and sys.version_info.minor >= 5:
-        a = u*v*dx
+        a = u * v * dx
         M = eval("(a @ f) @ g")
-        assert M == g*f*dx
+        assert M == g * f * dx
 
 
 def test_formsum(mass):
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
-    element = FiniteElement("Lagrange", triangle, 1)
+    element = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     V = FunctionSpace(domain, element)
     v = Cofunction(V.dual())
 
     assert v + mass
     assert mass + v
-    assert isinstance((mass+v), FormSum)
+    assert isinstance((mass + v), FormSum)
 
     assert len((mass + v + v).components()) == 3
     # Variational forms are summed appropriately
     assert len((mass + v + mass).components()) == 2
 
     assert v - mass
     assert mass - v
-    assert isinstance((mass+v), FormSum)
+    assert isinstance((mass + v), FormSum)
 
     assert -v
     assert isinstance(-v, BaseForm)
     assert (-v).weights()[0] == -1
 
     assert 2 * v
     assert isinstance(2 * v, BaseForm)
```

### Comparing `fenics-ufl-2023.2.0/test/test_illegal.py` & `fenics_ufl-2024.1.0.post0/test/test_illegal.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import pytest
 
-from ufl import Argument, Coefficient, FiniteElement, FunctionSpace, Mesh, VectorElement
+from ufl import Argument, Coefficient, FunctionSpace, Mesh, triangle
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 # TODO: Add more illegal expressions to check!
 
 
 @pytest.fixture
 def selement():
-    return FiniteElement("Lagrange", "triangle", 1)
+    return FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
 
 
 @pytest.fixture
 def velement():
-    return VectorElement("Lagrange", "triangle", 1)
+    return FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
 
 
 @pytest.fixture
 def domain():
-    return Mesh(VectorElement("Lagrange", "triangle", 1))
+    return Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
 
 
 @pytest.fixture
 def sspace(domain, selement):
     return FunctionSpace(domain, selement)
```

### Comparing `fenics-ufl-2023.2.0/test/test_indexing.py` & `fenics_ufl-2024.1.0.post0/test/test_indexing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import pytest
 
-from ufl import Index, Mesh, SpatialCoordinate, VectorElement, outer, triangle
+from ufl import Index, Mesh, SpatialCoordinate, outer, triangle
 from ufl.classes import FixedIndex, Indexed, MultiIndex, Outer, Zero
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 
 @pytest.fixture
 def domain():
-    return Mesh(VectorElement("Lagrange", triangle, 1))
+    return Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
 
 
 @pytest.fixture
 def x1(domain):
     x = SpatialCoordinate(domain)
     return x
```

### Comparing `fenics-ufl-2023.2.0/test/test_indices.py` & `fenics_ufl-2024.1.0.post0/test/test_indices.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,86 +1,110 @@
 import pytest
 
-from ufl import (Argument, Coefficient, FunctionSpace, Mesh, TensorElement, TestFunction, TrialFunction, VectorElement,
-                 as_matrix, as_tensor, as_vector, cos, dx, exp, i, indices, j, k, l, outer, sin, triangle)
+from ufl import (
+    Argument,
+    Coefficient,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TrialFunction,
+    as_matrix,
+    as_tensor,
+    as_vector,
+    cos,
+    dx,
+    exp,
+    i,
+    indices,
+    j,
+    k,
+    l,
+    outer,
+    sin,
+    triangle,
+)
 from ufl.classes import IndexSum
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
-# TODO: add more expressions to test as many possible combinations of index notation as feasible...
+# TODO: add more expressions to test as many possible combinations of
+# index notation as feasible...
 
 
 def test_vector_indices(self):
-    element = VectorElement("CG", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     u = Argument(space, 2)
     f = Coefficient(space)
-    u[i]*f[i]*dx
-    u[j]*f[j]*dx
+    u[i] * f[i] * dx
+    u[j] * f[j] * dx
 
 
 def test_tensor_indices(self):
-    element = TensorElement("CG", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (2, 2), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     u = Argument(space, 2)
     f = Coefficient(space)
-    u[i, j]*f[i, j]*dx
-    u[j, i]*f[i, j]*dx
-    u[j, i]*f[j, i]*dx
+    u[i, j] * f[i, j] * dx
+    u[j, i] * f[i, j] * dx
+    u[j, i] * f[j, i] * dx
     with pytest.raises(BaseException):
-        (u[i, i]+f[j, i])*dx
+        (u[i, i] + f[j, i]) * dx
 
 
 def test_indexed_sum1(self):
-    element = VectorElement("CG", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     u = Argument(space, 2)
     f = Coefficient(space)
-    a = u[i]+f[i]
+    a = u[i] + f[i]
     with pytest.raises(BaseException):
-        a*dx
+        a * dx
 
 
 def test_indexed_sum2(self):
-    element = VectorElement("CG", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     v = Argument(space, 2)
     u = Argument(space, 3)
     f = Coefficient(space)
-    a = u[j]+f[j]+v[j]+2*v[j]+exp(u[i]*u[i])/2*f[j]
+    a = u[j] + f[j] + v[j] + 2 * v[j] + exp(u[i] * u[i]) / 2 * f[j]
     with pytest.raises(BaseException):
-        a*dx
+        a * dx
 
 
 def test_indexed_sum3(self):
-    element = VectorElement("CG", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     u = Argument(space, 2)
     f = Coefficient(space)
     with pytest.raises(BaseException):
-        u[i]+f[j]
+        u[i] + f[j]
 
 
 def test_indexed_function1(self):
-    element = VectorElement("CG", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     v = Argument(space, 2)
     u = Argument(space, 3)
     f = Coefficient(space)
-    aarg = (u[i]+f[i])*v[i]
-    exp(aarg)*dx
+    aarg = (u[i] + f[i]) * v[i]
+    exp(aarg) * dx
 
 
 def test_indexed_function2(self):
-    element = VectorElement("CG", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     v = Argument(space, 2)
     u = Argument(space, 3)
     f = Coefficient(space)
     bfun = cos(f[0])
     left = u[i] + f[i]
     right = v[i] * bfun
@@ -88,27 +112,27 @@
     assert left.ufl_free_indices[0] == i.count()
     assert len(right.ufl_free_indices) == 1
     assert right.ufl_free_indices[0] == i.count()
     left * right * dx
 
 
 def test_indexed_function3(self):
-    element = VectorElement("CG", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     Argument(space, 2)
     u = Argument(space, 3)
     f = Coefficient(space)
     with pytest.raises(BaseException):
-        sin(u[i] + f[i])*dx
+        sin(u[i] + f[i]) * dx
 
 
 def test_vector_from_indices(self):
-    element = VectorElement("CG", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     v = TestFunction(space)
     u = TrialFunction(space)
 
     # legal
     vv = as_vector(u[i], i)
     uu = as_vector(v[j], j)
@@ -117,77 +141,77 @@
     assert len(vv.ufl_shape) == 1
     assert len(uu.ufl_shape) == 1
     assert len(w.ufl_shape) == 1
     assert len(ww.ufl_shape) == 1
 
 
 def test_matrix_from_indices(self):
-    element = VectorElement("CG", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     v = TestFunction(space)
     u = TrialFunction(space)
 
-    A = as_matrix(u[i]*v[j], (i, j))
-    B = as_matrix(v[k]*v[k]*u[i]*v[j], (j, i))
+    A = as_matrix(u[i] * v[j], (i, j))
+    B = as_matrix(v[k] * v[k] * u[i] * v[j], (j, i))
     C = A + A
     C = B + B
     D = A + B
     assert len(A.ufl_shape) == 2
     assert len(B.ufl_shape) == 2
     assert len(C.ufl_shape) == 2
     assert len(D.ufl_shape) == 2
 
 
 def test_vector_from_list(self):
-    element = VectorElement("CG", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     v = TestFunction(space)
     u = TrialFunction(space)
 
     # create vector from list
     vv = as_vector([u[0], v[0]])
     ww = vv + vv
     assert len(vv.ufl_shape) == 1
     assert len(ww.ufl_shape) == 1
 
 
 def test_matrix_from_list(self):
-    element = VectorElement("CG", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     v = TestFunction(space)
     u = TrialFunction(space)
 
     # create matrix from list
     A = as_matrix([[u[0], u[1]], [v[0], v[1]]])
     # create matrix from indices
-    B = as_matrix((v[k]*v[k]) * u[i]*v[j], (j, i))
+    B = as_matrix((v[k] * v[k]) * u[i] * v[j], (j, i))
     # Test addition
     C = A + A
     C = B + B
     D = A + B
     assert len(A.ufl_shape) == 2
     assert len(B.ufl_shape) == 2
     assert len(C.ufl_shape) == 2
     assert len(D.ufl_shape) == 2
 
 
 def test_tensor(self):
-    element = VectorElement("CG", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     v = TestFunction(space)
     u = TrialFunction(space)
     f = Coefficient(space)
     g = Coefficient(space)
 
     # define the components of a fourth order tensor
-    Cijkl = u[i]*v[j]*f[k]*g[l]
+    Cijkl = u[i] * v[j] * f[k] * g[l]
     assert len(Cijkl.ufl_shape) == 0
     assert set(Cijkl.ufl_free_indices) == {i.count(), j.count(), k.count(), l.count()}
 
     # make it a tensor
     C = as_tensor(Cijkl, (i, j, k, l))
     assert len(C.ufl_shape) == 4
     self.assertSameIndices(C, ())
@@ -198,28 +222,28 @@
     self.assertSameIndices(A, ())
     A = C[:, :, i, j]
     assert len(A.ufl_shape) == 2
     assert set(A.ufl_free_indices) == {i.count(), j.count()}
 
     # legal?
     vv = as_vector([u[i], v[i]])
-    f[i]*vv  # this is well defined: ww = sum_i <f_i*u_i, f_i*v_i>
+    f[i] * vv  # this is well defined: ww = sum_i <f_i*u_i, f_i*v_i>
 
     # illegal
     with pytest.raises(BaseException):
         as_vector([u[i], v[j]])
 
     # illegal
     with pytest.raises(BaseException):
         as_matrix([[u[0], u[1]], [v[0]]])
 
 
 def test_indexed(self):
-    element = VectorElement("CG", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     v = TestFunction(space)
     u = TrialFunction(space)
     Coefficient(space)
     i, j, k, l = indices(4)  # noqa: E741
 
     a = v[i]
@@ -231,33 +255,33 @@
     a = outer(v, u)[i, i]
     self.assertSameIndices(a, ())
     self.assertIsInstance(a, IndexSum)
 
 
 def test_spatial_derivative(self):
     cell = triangle
-    element = VectorElement("CG", cell, 1)
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    element = FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     v = TestFunction(space)
     u = TrialFunction(space)
     i, j, k, l = indices(4)  # noqa: E741
-    d = cell.geometric_dimension()
+    d = 2
 
     a = v[i].dx(i)
     self.assertSameIndices(a, ())
     self.assertIsInstance(a, IndexSum)
     assert a.ufl_shape == ()
 
     a = v[i].dx(j)
     self.assertSameIndices(a, (i, j))
     self.assertNotIsInstance(a, IndexSum)
     assert a.ufl_shape == ()
 
-    a = (v[i]*u[j]).dx(i, j)
+    a = (v[i] * u[j]).dx(i, j)
     self.assertSameIndices(a, ())
     self.assertIsInstance(a, IndexSum)
     assert a.ufl_shape == ()
 
     a = v.dx(i, j)
     # self.assertSameIndices(a, (i,j))
     assert set(a.ufl_free_indices) == {j.count(), i.count()}
@@ -265,15 +289,15 @@
     assert a.ufl_shape == (d,)
 
     a = v[i].dx(0)
     self.assertSameIndices(a, (i,))
     self.assertNotIsInstance(a, IndexSum)
     assert a.ufl_shape == ()
 
-    a = (v[i]*u[j]).dx(0, 1)
+    a = (v[i] * u[j]).dx(0, 1)
     assert set(a.ufl_free_indices) == {i.count(), j.count()}
     self.assertNotIsInstance(a, IndexSum)
     assert a.ufl_shape == ()
 
     a = v.dx(i)[i]
     self.assertSameIndices(a, ())
     self.assertIsInstance(a, IndexSum)
```

### Comparing `fenics-ufl-2023.2.0/test/test_interpolate.py` & `fenics_ufl-2024.1.0.post0/test/test_interpolate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,64 @@
 """Test Interpolate object."""
 
 __authors__ = "Nacime Bouziani"
 __date__ = "2021-11-19"
 
 import pytest
 
-from ufl import (Action, Adjoint, Argument, Coefficient, FiniteElement, FunctionSpace, Mesh, TestFunction,
-                 TrialFunction, VectorElement, action, adjoint, derivative, dx, grad, inner, replace, triangle)
+from ufl import (
+    Action,
+    Adjoint,
+    Argument,
+    Coefficient,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TrialFunction,
+    action,
+    adjoint,
+    derivative,
+    dx,
+    grad,
+    inner,
+    replace,
+    triangle,
+)
 from ufl.algorithms.ad import expand_derivatives
-from ufl.algorithms.analysis import (extract_arguments, extract_arguments_and_coefficients, extract_base_form_operators,
-                                     extract_coefficients)
+from ufl.algorithms.analysis import (
+    extract_arguments,
+    extract_arguments_and_coefficients,
+    extract_base_form_operators,
+    extract_coefficients,
+)
 from ufl.algorithms.expand_indices import expand_indices
 from ufl.core.interpolate import Interpolate
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 
 @pytest.fixture
 def domain_2d():
-    return Mesh(VectorElement("Lagrange", triangle, 1))
+    return Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
 
 
 @pytest.fixture
 def V1(domain_2d):
-    f1 = FiniteElement("CG", triangle, 1)
+    f1 = FiniteElement("CG", triangle, 1, (), identity_pullback, H1)
     return FunctionSpace(domain_2d, f1)
 
 
 @pytest.fixture
 def V2(domain_2d):
-    f1 = FiniteElement("CG", triangle, 2)
+    f1 = FiniteElement("CG", triangle, 2, (), identity_pullback, H1)
     return FunctionSpace(domain_2d, f1)
 
 
 def test_symbolic(V1, V2):
-
     # Set dual of V2
     V2_dual = V2.dual()
 
     u = Coefficient(V1)
     vstar = Argument(V2_dual, 0)
     Iu = Interpolate(u, vstar)
 
@@ -44,15 +66,14 @@
     assert Iu.ufl_function_space() == V2
     assert Iu.argument_slots() == (vstar, u)
     assert Iu.arguments() == (vstar,)
     assert Iu.ufl_operands == (u,)
 
 
 def test_action_adjoint(V1, V2):
-
     # Set dual of V2
     V2_dual = V2.dual()
     vstar = Argument(V2_dual, 0)
 
     u = Coefficient(V1)
     Iu = Interpolate(u, vstar)
 
@@ -71,15 +92,14 @@
     assert action(F, Iu) == Iu * v * dx
 
     # -- Adjoint -- #
     adjoint(Iv) == Adjoint(Iv)
 
 
 def test_differentiation(V1, V2):
-
     u = Coefficient(V1)
     v = TestFunction(V1)
 
     # Define Interpolate
     Iu = Interpolate(u, V2)
 
     # -- Differentiate: Interpolate(u, V2) -- #
@@ -126,15 +146,14 @@
     dFdw = expand_derivatives(derivative(F, w, Ihat))
 
     # Need to expand indices to be able to match equal (different MultiIndex used for both).
     assert expand_indices(dFdIu) == expand_indices(dFdw)
 
 
 def test_extract_base_form_operators(V1, V2):
-
     u = Coefficient(V1)
     uhat = TrialFunction(V1)
     vstar = Argument(V2.dual(), 0)
 
     # -- Interpolate(u, V2) -- #
     Iu = Interpolate(u, V2)
     assert extract_arguments(Iu) == [vstar]
```

### Comparing `fenics-ufl-2023.2.0/test/test_lhs_rhs.py` & `fenics_ufl-2024.1.0.post0/test/test_lhs_rhs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,37 @@
 __authors__ = "Marie E. Rognes"
 
 # First added: 2011-11-09
 # Last changed: 2011-11-09
 
-from ufl import (Argument, Coefficient, Constant, FiniteElement, FunctionSpace, Mesh, TestFunction, TrialFunction,
-                 VectorElement, action, derivative, ds, dS, dx, exp, interval, system)
+from ufl import (
+    Argument,
+    Coefficient,
+    Constant,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TrialFunction,
+    action,
+    derivative,
+    dS,
+    ds,
+    dx,
+    exp,
+    interval,
+    system,
+)
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 
 def test_lhs_rhs_simple():
-    V = FiniteElement("CG", interval, 1)
-    domain = Mesh(VectorElement("Lagrange", interval, 1))
+    V = FiniteElement("Lagrange", interval, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", interval, 1, (1,), identity_pullback, H1))
     space = FunctionSpace(domain, V)
     v = TestFunction(space)
     u = TrialFunction(space)
     w = Argument(space, 2)  # This was 0, not sure why
     f = Coefficient(space)
 
     F0 = f * u * v * w * dx
@@ -33,33 +51,33 @@
 
     F3 = action(F2, f)
     a, L = system(F3)
     assert len(L.integrals()) == 1
 
 
 def test_lhs_rhs_derivatives():
-    V = FiniteElement("CG", interval, 1)
-    domain = Mesh(VectorElement("Lagrange", interval, 1))
+    V = FiniteElement("Lagrange", interval, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", interval, 1, (1,), identity_pullback, H1))
     space = FunctionSpace(domain, V)
     v = TestFunction(space)
     u = TrialFunction(space)
     f = Coefficient(space)
 
-    F0 = exp(f) * u * v * dx + v * dx + f * v * ds + exp(f)('+') * v * dS
+    F0 = exp(f) * u * v * dx + v * dx + f * v * ds + exp(f)("+") * v * dS
     a, L = system(F0)
     assert len(a.integrals()) == 1
     assert len(L.integrals()) == 3
 
     derivative(F0, f)
     a, L = system(F0)
 
 
 def test_lhs_rhs_slightly_obscure():
-    V = FiniteElement("CG", interval, 1)
-    domain = Mesh(VectorElement("Lagrange", interval, 1))
+    V = FiniteElement("Lagrange", interval, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", interval, 1, (1,), identity_pullback, H1))
     space = FunctionSpace(domain, V)
     u = TrialFunction(space)
     w = Argument(space, 2)
     f = Constant(domain)
 
     # FIXME:
     # ufl.algorithsm.formtransformations.compute_form_with_arity
```

### Comparing `fenics-ufl-2023.2.0/test/test_literals.py` & `fenics_ufl-2024.1.0.post0/test/test_literals.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     assert z1 == z1
     assert int(z1) == 0
     assert float(z1) == 0.0
     assert complex(z1) == 0.0 + 0.0j
     self.assertNotEqual(z1, 1.0)
     self.assertFalse(z1)
 
-    # If zero() == 0 is to be allowed, it must not have the same hash or it will collide with 0 as key in dicts...
+    # If zero() == 0 is to be allowed, it must not have the same hash or
+    # it will collide with 0 as key in dicts...
     self.assertNotEqual(hash(z1), hash(0.0))
     self.assertNotEqual(hash(z1), hash(0))
 
 
 def test_float(self):
     f1 = as_ufl(1)
     f2 = as_ufl(1.0)
@@ -73,15 +74,15 @@
 
 
 def test_scalar_sums(self):
     n = 10
     s = [as_ufl(i) for i in range(n)]
 
     for i in range(n):
-        self.assertNotEqual(s[i], i+1)
+        self.assertNotEqual(s[i], i + 1)
 
     for i in range(n):
         assert s[i] == i
 
     for i in range(n):
         assert 0 + s[i] == i
 
@@ -94,52 +95,53 @@
     for i in range(n):
         assert 1 + s[i] - 1 == i
 
     assert s[1] + s[1] == 2
     assert s[1] + s[2] == 3
     assert s[1] + s[2] + s[3] == s[6]
     assert s[5] - s[2] == 3
-    assert 1*s[5] == 5
-    assert 2*s[5] == 10
-    assert s[6]/3 == 2
+    assert 1 * s[5] == 5
+    assert 2 * s[5] == 10
+    assert s[6] / 3 == 2
 
 
 def test_identity(self):
     pass  # FIXME
 
 
 def test_permutation_symbol_3(self):
     e = PermutationSymbol(3)
     assert e.ufl_shape == (3, 3, 3)
     assert eval(repr(e)) == e
     for i in range(3):
         for j in range(3):
             for k in range(3):
-                value = (j-i)*(k-i)*(k-j)/2
+                value = (j - i) * (k - i) * (k - j) / 2
                 self.assertEqual(e[i, j, k], value)
     i, j, k = indices(3)
     self.assertIsInstance(e[i, j, k], Indexed)
     x = (0, 0, 0)
     self.assertEqual((e[i, j, k] * e[i, j, k])(x), 6)
 
 
 def test_permutation_symbol_n(self):
     for n in range(2, 5):  # tested with upper limit 7, but evaluation is a bit slow then
         e = PermutationSymbol(n)
-        assert e.ufl_shape == (n,)*n
+        assert e.ufl_shape == (n,) * n
         assert eval(repr(e)) == e
 
         ii = indices(n)
-        x = (0,)*n
-        nfac = product(m for m in range(1, n+1))
+        x = (0,) * n
+        nfac = product(m for m in range(1, n + 1))
         assert (e[ii] * e[ii])(x) == nfac
 
 
 def test_unit_dyads(self):
     from ufl.tensors import unit_matrices, unit_vectors
+
     ei, ej = unit_vectors(2)
     self.assertEqual(as_vector((1, 0)), ei)
     self.assertEqual(as_vector((0, 1)), ej)
     eii, eij, eji, ejj = unit_matrices(2)
     self.assertEqual(as_matrix(((1, 0), (0, 0))), eii)
     self.assertEqual(as_matrix(((0, 1), (0, 0))), eij)
     self.assertEqual(as_matrix(((0, 0), (1, 0))), eji)
```

### Comparing `fenics-ufl-2023.2.0/test/test_measures.py` & `fenics_ufl-2024.1.0.post0/test/test_measures.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """Tests of the various ways Measure objects can be created and used."""
 
 from mockobjects import MockMesh, MockMeshFunction
 
-from ufl import Cell, Coefficient, FiniteElement, FunctionSpace, Measure, Mesh, as_ufl, dC, dI, dO, triangle
+from ufl import Cell, Coefficient, FunctionSpace, Measure, Mesh, as_ufl, dC, dI, dO, triangle
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 
 def test_construct_forms_from_default_measures():
     # Create defaults:
     dx = Measure("dx")
     # dE = Measure("dE")
 
@@ -53,45 +56,42 @@
 
     # Check that defaults are set properly
     assert dx.ufl_domain() is None
     assert dx.metadata() == {}
 
     # Check that we can create a basic form with default measure
     one = as_ufl(1)
-    one * dx(Mesh(triangle))
+    one * dx(Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)))
 
 
 def test_foo():
-
     # Define a manifold domain, allows checking gdim/tdim mixup errors
     gdim = 3
     tdim = 2
-    cell = Cell("triangle", gdim)
+    cell = Cell("triangle")
     mymesh = MockMesh(9)
-    mydomain = Mesh(cell, ufl_id=9, cargo=mymesh)
+    mydomain = Mesh(
+        FiniteElement("Lagrange", cell, 1, (gdim,), identity_pullback, H1), ufl_id=9, cargo=mymesh
+    )
 
     assert cell.topological_dimension() == tdim
-    assert cell.geometric_dimension() == gdim
     assert cell.cellname() == "triangle"
     assert mydomain.topological_dimension() == tdim
     assert mydomain.geometric_dimension() == gdim
     assert mydomain.ufl_cell() == cell
     assert mydomain.ufl_id() == 9
     assert mydomain.ufl_cargo() == mymesh
 
     # Define a coefficient for use in tests below
-    V = FunctionSpace(mydomain, FiniteElement("CG", cell, 1))
+    V = FunctionSpace(mydomain, FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1))
     f = Coefficient(V)
 
     # Test definition of a custom measure with explicit parameters
     metadata = {"opt": True}
-    mydx = Measure("dx",
-                   domain=mydomain,
-                   subdomain_id=3,
-                   metadata=metadata)
+    mydx = Measure("dx", domain=mydomain, subdomain_id=3, metadata=metadata)
     assert mydx.ufl_domain().ufl_id() == mydomain.ufl_id()
     assert mydx.metadata() == metadata
     M = f * mydx
 
     # Compatibility:
     dx = Measure("dx")
     # domain=None,
@@ -113,15 +113,15 @@
     # Check that original dx is untouched
     assert dx.ufl_domain() is None
     assert dx.subdomain_id() == "everywhere"
 
     # Set subdomain_id to (2,3), still no domain set
     dx23 = dx((2, 3))
     assert dx23.ufl_domain() is None
-    assert dx23.subdomain_id(), (2 == 3)
+    assert dx23.subdomain_id(), 2 == 3
 
     # Map metadata to metadata, ffc interprets as before
     dxm = dx(metadata={"dummy": 123})
     # assert dxm.metadata() == {"dummy":123}
     assert dxm.metadata() == {"dummy": 123}  # Deprecated, TODO: Remove
 
     assert dxm.ufl_domain() is None
@@ -154,37 +154,37 @@
     assert dSd.ufl_domain() is None
     assert dxd.subdomain_data() is cell_domains
     assert dsd.subdomain_data() is exterior_facet_domains
     assert dSd.subdomain_data() is interior_facet_domains
 
     # Create some forms with these measures (used in checks below):
     Mx = f * dxd
-    Ms = f ** 2 * dsd
-    MS = f('+') * dSd
-    M = f * dxd + f ** 2 * dsd + f('+') * dSd
+    Ms = f**2 * dsd
+    MS = f("+") * dSd
+    M = f * dxd + f**2 * dsd + f("+") * dSd
 
     # Test extracting domain data from a form for each measure:
-    domain, = Mx.ufl_domains()
+    (domain,) = Mx.ufl_domains()
     assert domain.ufl_id() == mydomain.ufl_id()
     assert domain.ufl_cargo() == mymesh
     assert len(Mx.subdomain_data()[mydomain]["cell"]) == 1
     assert Mx.subdomain_data()[mydomain]["cell"][0] == cell_domains
 
-    domain, = Ms.ufl_domains()
+    (domain,) = Ms.ufl_domains()
     assert domain.ufl_cargo() == mymesh
     assert len(Ms.subdomain_data()[mydomain]["exterior_facet"]) == 1
     assert Ms.subdomain_data()[mydomain]["exterior_facet"][0] == exterior_facet_domains
 
-    domain, = MS.ufl_domains()
+    (domain,) = MS.ufl_domains()
     assert domain.ufl_cargo() == mymesh
     assert len(MS.subdomain_data()[mydomain]["interior_facet"]) == 1
     assert MS.subdomain_data()[mydomain]["interior_facet"][0] == interior_facet_domains
 
     # Test joining of these domains in a single form
-    domain, = M.ufl_domains()
+    (domain,) = M.ufl_domains()
     assert domain.ufl_cargo() == mymesh
     assert len(M.subdomain_data()[mydomain]["cell"]) == 1
     assert M.subdomain_data()[mydomain]["cell"][0] == cell_domains
     assert len(M.subdomain_data()[mydomain]["exterior_facet"]) == 1
     assert M.subdomain_data()[mydomain]["exterior_facet"][0] == exterior_facet_domains
     assert len(M.subdomain_data()[mydomain]["interior_facet"]) == 1
     assert M.subdomain_data()[mydomain]["interior_facet"][0] == interior_facet_domains
```

### Comparing `fenics-ufl-2023.2.0/test/test_new_ad.py` & `fenics_ufl-2024.1.0.post0/test/test_new_ad.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,56 @@
-from ufl import (CellVolume, Coefficient, Constant, FacetNormal, FiniteElement, FunctionSpace, Identity, Mesh,
-                 SpatialCoordinate, TestFunction, VectorConstant, VectorElement, as_ufl, cos, derivative, diff, exp,
-                 grad, ln, sin, tan, triangle, variable, zero)
-from ufl.algorithms.apply_derivatives import GenericDerivativeRuleset, GradRuleset, apply_derivatives
+from ufl import (
+    CellVolume,
+    Coefficient,
+    Constant,
+    FacetNormal,
+    FunctionSpace,
+    Identity,
+    Mesh,
+    SpatialCoordinate,
+    TestFunction,
+    VectorConstant,
+    as_ufl,
+    cos,
+    derivative,
+    diff,
+    exp,
+    grad,
+    ln,
+    sin,
+    tan,
+    triangle,
+    variable,
+    zero,
+)
+from ufl.algorithms.apply_derivatives import (
+    GenericDerivativeRuleset,
+    GradRuleset,
+    apply_derivatives,
+)
 from ufl.algorithms.renumbering import renumber_indices
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1, L2
 
 # Note: the old tests in test_automatic_differentiation.py are a bit messy
 #       but still cover many things that are not in here yet.
 
 
 # FIXME: Write UNIT tests for all terminal derivatives!
 # FIXME: Write UNIT tests for operator derivatives!
 
 
 def test_apply_derivatives_doesnt_change_expression_without_derivatives():
     cell = triangle
-    d = cell.geometric_dimension()
-    V0 = FiniteElement("DG", cell, 0)
-    V1 = FiniteElement("Lagrange", cell, 1)
+    d = 2
+    V0 = FiniteElement("Discontinuous Lagrange", cell, 0, (), identity_pullback, L2)
+    V1 = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
 
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (d,), identity_pullback, H1))
     v0_space = FunctionSpace(domain, V0)
     v1_space = FunctionSpace(domain, V1)
 
     # Literals
     z = zero((3, 2))
     one = as_ufl(1)
     two = as_ufl(2.0)
@@ -43,54 +71,54 @@
     # Coefficients
     f0 = Coefficient(v0_space)
     f1 = Coefficient(v1_space)
     coefficients = [f0, f1]
 
     # Expressions
     e0 = f0 + f1
-    e1 = v0 * (f1/3 - f0**2)
+    e1 = v0 * (f1 / 3 - f0**2)
     e2 = exp(sin(cos(tan(ln(x[0])))))
     expressions = [e0, e1, e2]
 
     # Check that all are unchanged
     for expr in literals + geometry + arguments + coefficients + expressions:
         # Note the use of "is" here instead of ==, this property
         # is important for efficiency and memory usage
         assert apply_derivatives(expr) is expr
 
 
 def test_literal_derivatives_are_zero():
     cell = triangle
-    d = cell.geometric_dimension()
+    d = 2
 
     # Literals
     one = as_ufl(1)
     two = as_ufl(2.0)
     ident = Identity(d)
     literals = [one, two, ident]
 
     # Generic ruleset handles literals directly:
     for lit in literals:
-        for sh in [(), (d,), (d, d+1)]:
+        for sh in [(), (d,), (d, d + 1)]:
             assert GenericDerivativeRuleset(sh)(lit) == zero(lit.ufl_shape + sh)
 
     # Variables
     v0 = variable(one)
     v1 = variable(zero((d,)))
     v2 = variable(ident)
     variables = [v0, v1, v2]
 
     # Test literals via apply_derivatives and variable ruleset:
     for lit in literals:
         for v in variables:
             assert apply_derivatives(diff(lit, v)) == zero(lit.ufl_shape + v.ufl_shape)
 
-    V0 = FiniteElement("DG", cell, 0)
-    V1 = FiniteElement("Lagrange", cell, 1)
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    V0 = FiniteElement("Discontinuous Lagrange", cell, 0, (), identity_pullback, L2)
+    V1 = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (d,), identity_pullback, H1))
     v0_space = FunctionSpace(domain, V0)
     v1_space = FunctionSpace(domain, V1)
     u0 = Coefficient(v0_space)
     u1 = Coefficient(v1_space)
     v0 = TestFunction(v0_space)
     v1 = TestFunction(v1_space)
     args = [(u0, v0), (u1, v1)]
@@ -103,24 +131,24 @@
     # Test grad ruleset directly since grad(literal) is invalid:
     assert GradRuleset(d)(one) == zero((d,))
     assert GradRuleset(d)(one) == zero((d,))
 
 
 def test_grad_ruleset():
     cell = triangle
-    d = cell.geometric_dimension()
+    d = 2
 
-    V0 = FiniteElement("DG", cell, 0)
-    V1 = FiniteElement("Lagrange", cell, 1)
-    V2 = FiniteElement("Lagrange", cell, 2)
-    W0 = VectorElement("DG", cell, 0)
-    W1 = VectorElement("Lagrange", cell, 1)
-    W2 = VectorElement("Lagrange", cell, 2)
+    V0 = FiniteElement("Discontinuous Lagrange", cell, 0, (), identity_pullback, L2)
+    V1 = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    V2 = FiniteElement("Lagrange", cell, 2, (), identity_pullback, H1)
+    W0 = FiniteElement("Discontinuous Lagrange", cell, 0, (2,), identity_pullback, L2)
+    W1 = FiniteElement("Lagrange", cell, 1, (d,), identity_pullback, H1)
+    W2 = FiniteElement("Lagrange", cell, 2, (d,), identity_pullback, H1)
 
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (d,), identity_pullback, H1))
     v0_space = FunctionSpace(domain, V0)
     v1_space = FunctionSpace(domain, V1)
     v2_space = FunctionSpace(domain, V2)
     w0_space = FunctionSpace(domain, W0)
     w1_space = FunctionSpace(domain, W1)
     w2_space = FunctionSpace(domain, W2)
 
@@ -190,18 +218,22 @@
     assert rules(grad(vf2)) == grad(grad(vf2))
 
     # Indexed coefficients
     assert renumber_indices(apply_derivatives(grad(vf2[0]))) == renumber_indices(grad(vf2)[0, :])
     assert renumber_indices(apply_derivatives(grad(vf2[1])[0])) == renumber_indices(grad(vf2)[1, 0])
 
     # Grad of gradually more complex expressions
-    assert apply_derivatives(grad(2*f0)) == zero((d,))
-    assert renumber_indices(apply_derivatives(grad(2*f1))) == renumber_indices(2*grad(f1))
-    assert renumber_indices(apply_derivatives(grad(sin(f1)))) == renumber_indices(cos(f1) * grad(f1))
-    assert renumber_indices(apply_derivatives(grad(cos(f1)))) == renumber_indices(-sin(f1) * grad(f1))
+    assert apply_derivatives(grad(2 * f0)) == zero((d,))
+    assert renumber_indices(apply_derivatives(grad(2 * f1))) == renumber_indices(2 * grad(f1))
+    assert renumber_indices(apply_derivatives(grad(sin(f1)))) == renumber_indices(
+        cos(f1) * grad(f1)
+    )
+    assert renumber_indices(apply_derivatives(grad(cos(f1)))) == renumber_indices(
+        -sin(f1) * grad(f1)
+    )
 
 
 def test_variable_ruleset():
     pass
 
 
 def test_gateaux_ruleset():
```

### Comparing `fenics-ufl-2023.2.0/test/test_pickle.py` & `fenics_ufl-2024.1.0.post0/test/test_pickle.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,25 +6,56 @@
 __license__ = "GNU GPL version 3 or any later version"
 
 # Examples copied from the FFC demo directory, examples contributed
 # by Johan Jansson, Kristian Oelgaard, Marie Rognes, and Garth Wells.
 
 import pickle
 
-from ufl import (Coefficient, Constant, Dx, FacetNormal, FiniteElement, FunctionSpace, Identity, Mesh, TensorElement,
-                 TestFunction, TestFunctions, TrialFunction, TrialFunctions, VectorConstant, VectorElement, avg, curl,
-                 div, dot, dS, ds, dx, grad, i, inner, j, jump, lhs, rhs, sqrt, tetrahedron, triangle)
+from ufl import (
+    Coefficient,
+    Constant,
+    Dx,
+    FacetNormal,
+    FunctionSpace,
+    Identity,
+    Mesh,
+    TestFunction,
+    TestFunctions,
+    TrialFunction,
+    TrialFunctions,
+    VectorConstant,
+    avg,
+    curl,
+    div,
+    dot,
+    dS,
+    ds,
+    dx,
+    grad,
+    i,
+    inner,
+    j,
+    jump,
+    lhs,
+    rhs,
+    sqrt,
+    tetrahedron,
+    triangle,
+)
 from ufl.algorithms import compute_form_data
+from ufl.finiteelement import FiniteElement, MixedElement
+from ufl.pullback import contravariant_piola, covariant_piola, identity_pullback
+from ufl.sobolevspace import H1, L2, HCurl, HDiv
 
 p = pickle.HIGHEST_PROTOCOL
 
 
 def testConstant():
-    element = FiniteElement("Lagrange", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
 
     c = Constant(domain)
     d = VectorConstant(domain)
@@ -40,16 +71,16 @@
     L_restore = pickle.loads(L_pickle)
 
     assert a.signature() == a_restore.signature()
     assert L.signature() == L_restore.signature()
 
 
 def testElasticity():
-    element = VectorElement("Lagrange", "tetrahedron", 1)
-    domain = Mesh(VectorElement("Lagrange", "tetrahedron", 1))
+    element = FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
 
     def eps(v):
         # FFC notation: return grad(v) + transp(grad(v))
@@ -61,30 +92,30 @@
     a_pickle = pickle.dumps(a, p)
     a_restore = pickle.loads(a_pickle)
 
     assert a.signature() == a_restore.signature()
 
 
 def testEnergyNorm():
-    element = FiniteElement("Lagrange", "tetrahedron", 1)
-    domain = Mesh(VectorElement("Lagrange", "tetrahedron", 1))
+    element = FiniteElement("Lagrange", tetrahedron, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = Coefficient(space)
     a = (v * v + dot(grad(v), grad(v))) * dx
 
     a_pickle = pickle.dumps(a, p)
     a_restore = pickle.loads(a_pickle)
 
     assert a.signature() == a_restore.signature()
 
 
 def testEquation():
-    element = FiniteElement("Lagrange", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     k = 0.1
 
     v = TestFunction(space)
     u = TrialFunction(space)
     u0 = Coefficient(space)
@@ -100,37 +131,36 @@
     L_restore = pickle.loads(L_pickle)
 
     assert a.signature() == a_restore.signature()
     assert L.signature() == L_restore.signature()
 
 
 def testFunctionOperators():
-    element = FiniteElement("Lagrange", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
     f = Coefficient(space)
     g = Coefficient(space)
 
     # FFC notation: a = sqrt(1/modulus(1/f))*sqrt(g)*dot(grad(v), grad(u))*dx
     # + v*u*sqrt(f*g)*g*dx
-    a = sqrt(1 / abs(1 / f)) * sqrt(g) * \
-        dot(grad(v), grad(u)) * dx + v * u * sqrt(f * g) * g * dx
+    a = sqrt(1 / abs(1 / f)) * sqrt(g) * dot(grad(v), grad(u)) * dx + v * u * sqrt(f * g) * g * dx
 
     a_pickle = pickle.dumps(a, p)
     a_restore = pickle.loads(a_pickle)
 
     assert a.signature() == a_restore.signature()
 
 
 def testHeat():
-    element = FiniteElement("Lagrange", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u1 = TrialFunction(space)
     u0 = Coefficient(space)
     c = Coefficient(space)
     f = Coefficient(space)
@@ -145,48 +175,48 @@
     L_restore = pickle.loads(L_pickle)
 
     assert a.signature() == a_restore.signature()
     assert L.signature() == L_restore.signature()
 
 
 def testMass():
-    element = FiniteElement("Lagrange", "tetrahedron", 3)
-    domain = Mesh(VectorElement("Lagrange", "tetrahedron", 1))
+    element = FiniteElement("Lagrange", tetrahedron, 3, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
 
     a = v * u * dx
 
     a_pickle = pickle.dumps(a, p)
     a_restore = pickle.loads(a_pickle)
 
     assert a.signature() == a_restore.signature()
 
 
 def testMixedMixedElement():
-    P3 = FiniteElement("Lagrange", "triangle", 3)
+    P3 = FiniteElement("Lagrange", triangle, 3, (), identity_pullback, H1)
 
-    element = (P3 * P3) * (P3 * P3)
+    element = MixedElement([[P3, P3], [P3, P3]])
 
     element_pickle = pickle.dumps(element, p)
     element_restore = pickle.loads(element_pickle)
 
     assert element == element_restore
 
 
 def testMixedPoisson():
     q = 1
 
-    BDM = FiniteElement("Brezzi-Douglas-Marini", "triangle", q)
-    DG = FiniteElement("Discontinuous Lagrange", "triangle", q - 1)
+    BDM = FiniteElement("Brezzi-Douglas-Marini", triangle, q, (2,), contravariant_piola, HDiv)
+    DG = FiniteElement("Discontinuous Lagrange", triangle, q - 1, (), identity_pullback, L2)
 
-    mixed_element = BDM * DG
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    mixed_element = MixedElement([BDM, DG])
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     mixed_space = FunctionSpace(domain, mixed_element)
     dg_space = FunctionSpace(domain, DG)
 
     (tau, w) = TestFunctions(mixed_space)
     (sigma, u) = TrialFunctions(mixed_space)
 
     f = Coefficient(dg_space)
@@ -200,16 +230,16 @@
     L_restore = pickle.loads(L_pickle)
 
     assert a.signature() == a_restore.signature()
     assert L.signature() == L_restore.signature()
 
 
 def testNavierStokes():
-    element = VectorElement("Lagrange", "tetrahedron", 1)
-    domain = Mesh(VectorElement("Lagrange", "tetrahedron", 1))
+    element = FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
 
     w = Coefficient(space)
 
@@ -219,16 +249,16 @@
     a_pickle = pickle.dumps(a, p)
     a_restore = pickle.loads(a_pickle)
 
     assert a.signature() == a_restore.signature()
 
 
 def testNeumannProblem():
-    element = VectorElement("Lagrange", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
     f = Coefficient(space)
     g = Coefficient(space)
 
@@ -244,16 +274,16 @@
     L_restore = pickle.loads(L_pickle)
 
     assert a.signature() == a_restore.signature()
     assert L.signature() == L_restore.signature()
 
 
 def testOptimization():
-    element = FiniteElement("Lagrange", "triangle", 3)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 3, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
     f = Coefficient(space)
 
     a = dot(grad(v), grad(u)) * dx
@@ -265,32 +295,32 @@
     L_restore = pickle.loads(L_pickle)
 
     assert a.signature() == a_restore.signature()
     assert L.signature() == L_restore.signature()
 
 
 def testP5tet():
-    element = FiniteElement("Lagrange", tetrahedron, 5)
+    element = FiniteElement("Lagrange", tetrahedron, 5, (), identity_pullback, H1)
 
     element_pickle = pickle.dumps(element, p)
     element_restore = pickle.loads(element_pickle)
 
     assert element == element_restore
 
 
 def testP5tri():
-    element = FiniteElement("Lagrange", triangle, 5)
+    element = FiniteElement("Lagrange", triangle, 5, (), identity_pullback, H1)
 
     element_pickle = pickle.dumps(element, p)
     pickle.loads(element_pickle)
 
 
 def testPoissonDG():
-    element = FiniteElement("Discontinuous Lagrange", triangle, 1)
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    element = FiniteElement("Discontinuous Lagrange", triangle, 1, (), identity_pullback, L2)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
     f = Coefficient(space)
 
     n = FacetNormal(domain)
@@ -308,36 +338,38 @@
     #    - dot(avg(grad(v)), jump(u, n))*dS \
     #    - dot(jump(v, n), avg(grad(u)))*dS \
     #    + alpha/h('+')*dot(jump(v, n), jump(u, n))*dS \
     #    - dot(grad(v), mult(u,n))*ds \
     #    - dot(mult(v,n), grad(u))*ds \
     #    + gamma/h*v*u*ds
 
-    a = inner(grad(v), grad(u)) * dx \
-        - inner(avg(grad(v)), jump(u, n)) * dS \
-        - inner(jump(v, n), avg(grad(u))) * dS \
-        + alpha / h('+') * dot(jump(v, n), jump(u, n)) * dS \
-        - inner(grad(v), u * n) * ds \
-        - inner(u * n, grad(u)) * ds \
+    a = (
+        inner(grad(v), grad(u)) * dx
+        - inner(avg(grad(v)), jump(u, n)) * dS
+        - inner(jump(v, n), avg(grad(u))) * dS
+        + alpha / h("+") * dot(jump(v, n), jump(u, n)) * dS
+        - inner(grad(v), u * n) * ds
+        - inner(u * n, grad(u)) * ds
         + gamma / h * v * u * ds
+    )
 
     L = v * f * dx + v * gN * ds
 
     a_pickle = pickle.dumps(a, p)
     a_restore = pickle.loads(a_pickle)
     L_pickle = pickle.dumps(L, p)
     L_restore = pickle.loads(L_pickle)
 
     assert a.signature() == a_restore.signature()
     assert L.signature() == L_restore.signature()
 
 
 def testPoisson():
-    element = FiniteElement("Lagrange", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
     f = Coefficient(space)
 
     # Note: inner() also works
@@ -350,16 +382,16 @@
     L_restore = pickle.loads(L_pickle)
 
     assert a.signature() == a_restore.signature()
     assert L.signature() == L_restore.signature()
 
 
 def testPoissonSystem():
-    element = VectorElement("Lagrange", "triangle", 1)
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    element = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
     f = Coefficient(space)
 
     # FFC notation: a = dot(grad(v), grad(u))*dx
@@ -374,24 +406,24 @@
     L_restore = pickle.loads(L_pickle)
 
     assert a.signature() == a_restore.signature()
     assert L.signature() == L_restore.signature()
 
 
 def testQuadratureElement():
-    element = FiniteElement("Lagrange", "triangle", 2)
+    element = FiniteElement("Lagrange", triangle, 2, (), identity_pullback, H1)
 
     # FFC notation:
-    # QE = QuadratureElement("triangle", 3)
-    # sig = VectorQuadratureElement("triangle", 3)
+    # QE = QuadratureElement(triangle, 3)
+    # sig = VectorQuadratureElement(triangle, 3)
 
-    QE = FiniteElement("Quadrature", "triangle", 3)
-    sig = VectorElement("Quadrature", "triangle", 3)
+    QE = FiniteElement("Quadrature", triangle, 3, (), identity_pullback, L2)
+    sig = FiniteElement("Quadrature", triangle, 3, (2,), identity_pullback, L2)
 
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
     qe_space = FunctionSpace(domain, QE)
     sig_space = FunctionSpace(domain, sig)
 
     v = TestFunction(space)
     u = TrialFunction(space)
     u0 = Coefficient(space)
@@ -410,19 +442,19 @@
     assert a.signature() == a_restore.signature()
     assert L.signature() == L_restore.signature()
 
 
 def testStokes():
     # UFLException: Shape mismatch in sum.
 
-    P2 = VectorElement("Lagrange", "triangle", 2)
-    P1 = FiniteElement("Lagrange", "triangle", 1)
-    TH = P2 * P1
+    P2 = FiniteElement("Lagrange", triangle, 2, (2,), identity_pullback, H1)
+    P1 = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    TH = MixedElement([P2, P1])
 
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     th_space = FunctionSpace(domain, TH)
     p2_space = FunctionSpace(domain, P2)
 
     (v, q) = TestFunctions(th_space)
     (u, r) = TrialFunctions(th_space)
 
     f = Coefficient(p2_space)
@@ -439,67 +471,73 @@
     L_restore = pickle.loads(L_pickle)
 
     assert a.signature() == a_restore.signature()
     assert L.signature() == L_restore.signature()
 
 
 def testSubDomain():
-    element = FiniteElement("CG", "tetrahedron", 1)
-    domain = Mesh(VectorElement("Lagrange", "tetrahedron", 1))
+    element = FiniteElement("Lagrange", tetrahedron, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     f = Coefficient(space)
 
     M = f * dx(2) + f * ds(5)
 
     M_pickle = pickle.dumps(M, p)
     M_restore = pickle.loads(M_pickle)
 
     assert M.signature() == M_restore.signature()
 
 
 def testSubDomains():
-    element = FiniteElement("CG", "tetrahedron", 1)
-    domain = Mesh(VectorElement("Lagrange", "tetrahedron", 1))
+    element = FiniteElement("Lagrange", tetrahedron, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
 
-    a = v * u * dx(0) + 10.0 * v * u * dx(1) + v * u * ds(0) + 2.0 * v * u * \
-        ds(1) + v('+') * u('+') * dS(0) + 4.3 * v('+') * u('+') * dS(1)
+    a = (
+        v * u * dx(0)
+        + 10.0 * v * u * dx(1)
+        + v * u * ds(0)
+        + 2.0 * v * u * ds(1)
+        + v("+") * u("+") * dS(0)
+        + 4.3 * v("+") * u("+") * dS(1)
+    )
 
     a_pickle = pickle.dumps(a, p)
     a_restore = pickle.loads(a_pickle)
 
     assert a.signature() == a_restore.signature()
 
 
 def testTensorWeightedPoisson():
     # FFC notation:
-    # P1 = FiniteElement("Lagrange", "triangle", 1)
-    # P0 = FiniteElement("Discontinuous Lagrange", "triangle", 0)
+    # P1 = FiniteElement("Lagrange", triangle, 1)
+    # P0 = FiniteElement("Discontinuous Lagrange", triangle, 0)
     #
     # v = TestFunction(P1)
     # u = TrialFunction(P1)
     # f = Coefficient(P1)
     #
     # c00 = Coefficient(P0)
     # c01 = Coefficient(P0)
     # c10 = Coefficient(P0)
     # c11 = Coefficient(P0)
     #
     # C = [[c00, c01], [c10, c11]]
     #
     # a = dot(grad(v), mult(C, grad(u)))*dx
 
-    P1 = FiniteElement("Lagrange", "triangle", 1)
-    P0 = TensorElement("Discontinuous Lagrange", "triangle", 0, shape=(2, 2))
+    P1 = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    P0 = FiniteElement("Discontinuous Lagrange", triangle, 0, (2, 2), identity_pullback, L2)
 
-    domain = Mesh(VectorElement("Lagrange", "triangle", 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     p1_space = FunctionSpace(domain, P1)
     p0_space = FunctionSpace(domain, P0)
 
     v = TestFunction(p1_space)
     u = TrialFunction(p1_space)
     C = Coefficient(p0_space)
 
@@ -515,34 +553,40 @@
     def HodgeLaplaceGradCurl(space, fspace):
         (tau, v) = TestFunctions(space)
         (sigma, u) = TrialFunctions(space)
         f = Coefficient(fspace)
 
         # FFC notation: a = (dot(tau, sigma) - dot(grad(tau), u) + dot(v,
         # grad(sigma)) + dot(curl(v), curl(u)))*dx
-        a = (inner(tau, sigma) - inner(grad(tau), u) +
-             inner(v, grad(sigma)) + inner(curl(v), curl(u))) * dx
+        a = (
+            inner(tau, sigma)
+            - inner(grad(tau), u)
+            + inner(v, grad(sigma))
+            + inner(curl(v), curl(u))
+        ) * dx
 
         # FFC notation: L = dot(v, f)*dx
         L = inner(v, f) * dx
 
         return [a, L]
 
-    shape = "tetrahedron"
+    shape = tetrahedron
     order = 1
 
-    GRAD = FiniteElement("Lagrange", shape, order)
+    GRAD = FiniteElement("Lagrange", shape, order, (), identity_pullback, H1)
 
     # FFC notation: CURL = FiniteElement("Nedelec", shape, order-1)
-    CURL = FiniteElement("N1curl", shape, order)
+    CURL = FiniteElement("N1curl", shape, order, (3,), covariant_piola, HCurl)
 
-    VectorLagrange = VectorElement("Lagrange", shape, order + 1)
-    domain = Mesh(VectorElement("Lagrange", shape, 1))
+    VectorLagrange = FiniteElement("Lagrange", shape, order + 1, (3,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", shape, 1, (3,), identity_pullback, H1))
 
-    [a, L] = HodgeLaplaceGradCurl(FunctionSpace(domain, GRAD * CURL), FunctionSpace(domain, VectorLagrange))
+    [a, L] = HodgeLaplaceGradCurl(
+        FunctionSpace(domain, MixedElement([GRAD, CURL])), FunctionSpace(domain, VectorLagrange)
+    )
 
     a_pickle = pickle.dumps(a, p)
     a_restore = pickle.loads(a_pickle)
     L_pickle = pickle.dumps(L, p)
     L_restore = pickle.loads(L_pickle)
 
     assert a.signature() == a_restore.signature()
@@ -553,16 +597,16 @@
     i = Identity(2)
     i_pickle = pickle.dumps(i, p)
     i_restore = pickle.loads(i_pickle)
     assert i == i_restore
 
 
 def testFormData():
-    element = FiniteElement("Lagrange", "tetrahedron", 3)
-    domain = Mesh(VectorElement("Lagrange", "tetrahedron", 1))
+    element = FiniteElement("Lagrange", tetrahedron, 3, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
     space = FunctionSpace(domain, element)
 
     v = TestFunction(space)
     u = TrialFunction(space)
 
     a = v * u * dx
```

### Comparing `fenics-ufl-2023.2.0/test/test_scratch.py` & `fenics_ufl-2024.1.0.post0/test/test_scratch.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,61 +4,77 @@
 Begin by copying this file to a filename matching test_*.py.
 The tests in the file will then automatically be run by ./test.py.
 Next look at the TODO markers below for places to edit.
 """
 
 import warnings
 
-from ufl import (Coefficient, FiniteElement, FunctionSpace, Identity, Mesh, TensorElement, TestFunction, VectorElement,
-                 as_matrix, as_tensor, as_vector, dx, grad, indices, inner, outer, triangle)
+from ufl import (
+    Coefficient,
+    FunctionSpace,
+    Identity,
+    Mesh,
+    TestFunction,
+    as_matrix,
+    as_tensor,
+    as_vector,
+    dx,
+    grad,
+    indices,
+    inner,
+    outer,
+    triangle,
+)
 from ufl.classes import FixedIndex, FormArgument, Grad, Indexed, ListTensor, Zero
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 from ufl.tensors import as_scalar, unit_indexed_tensor, unwrap_list_tensor
 
 
 class MockForwardAD:
-
     def __init__(self):
         self._w = ()
         self._v = ()
 
         class Obj:
-
             def __init__(self):
                 self._data = {}
+
         self._cd = Obj()
 
     def grad(self, g):
         # If we hit this type, it has already been propagated
         # to a coefficient (or grad of a coefficient), # FIXME: Assert this!
         # so we need to take the gradient of the variation or return zero.
         # Complications occur when dealing with derivatives w.r.t. single components...
 
         # Figure out how many gradients are around the inner terminal
         ngrads = 0
         o = g
         while isinstance(o, Grad):
-            o, = o.ufl_operands
+            (o,) = o.ufl_operands
             ngrads += 1
         if not isinstance(o, FormArgument):
             raise ValueError("Expecting gradient of a FormArgument, not %s" % repr(o))
 
         def apply_grads(f):
             if not isinstance(f, FormArgument):
-                print((','*60))
+                print(("," * 60))
                 print(f)
                 print(o)
                 print(g)
-                print((','*60))
+                print(("," * 60))
                 raise ValueError("What?")
             for i in range(ngrads):
                 f = Grad(f)
             return f
 
         # Find o among all w without any indexing, which makes this easy
-        for (w, v) in zip(self._w, self._v):
+        for w, v in zip(self._w, self._v):
             if o == w and isinstance(v, FormArgument):
                 # Case: d/dt [w + t v]
                 return (g, apply_grads(v))
 
         # If o is not among coefficient derivatives, return do/dw=0
         gprimesum = Zero(g.ufl_shape)
 
@@ -78,26 +94,25 @@
                 raise ValueError("Expecting only fixed indices in variation.")
             return vval, vcomp
 
         def compute_gprimeterm(ngrads, vval, vcomp, wshape, wcomp):
             # Apply gradients directly to argument vval,
             # and get the right indexed scalar component(s)
             kk = indices(ngrads)
-            Dvkk = apply_grads(vval)[vcomp+kk]
+            Dvkk = apply_grads(vval)[vcomp + kk]
             # Place scalar component(s) Dvkk into the right tensor positions
             if wshape:
                 Ejj, jj = unit_indexed_tensor(wshape, wcomp)
             else:
                 Ejj, jj = 1, ()
-            gprimeterm = as_tensor(Ejj*Dvkk, jj+kk)
+            gprimeterm = as_tensor(Ejj * Dvkk, jj + kk)
             return gprimeterm
 
         # Accumulate contributions from variations in different components
-        for (w, v) in zip(self._w, self._v):
-
+        for w, v in zip(self._w, self._v):
             # Analyse differentiation variable coefficient
             if isinstance(w, FormArgument):
                 if not w == o:
                     continue
                 wshape = w.ufl_shape
 
                 if isinstance(v, FormArgument):
@@ -105,26 +120,30 @@
                     return (g, apply_grads(v))
 
                 elif isinstance(v, ListTensor):
                     # Case: d/dt [w + t <...,v,...>]
                     for wcomp, vsub in unwrap_list_tensor(v):
                         if not isinstance(vsub, Zero):
                             vval, vcomp = analyse_variation_argument(vsub)
-                            gprimesum = gprimesum + compute_gprimeterm(ngrads, vval, vcomp, wshape, wcomp)
+                            gprimesum = gprimesum + compute_gprimeterm(
+                                ngrads, vval, vcomp, wshape, wcomp
+                            )
 
                 else:
                     if wshape != ():
                         raise ValueError("Expecting scalar coefficient in this branch.")
                     # Case: d/dt [w + t v[...]]
                     wval, wcomp = w, ()
 
                     vval, vcomp = analyse_variation_argument(v)
                     gprimesum = gprimesum + compute_gprimeterm(ngrads, vval, vcomp, wshape, wcomp)
 
-            elif isinstance(w, Indexed):  # This path is tested in unit tests, but not actually used?
+            elif isinstance(
+                w, Indexed
+            ):  # This path is tested in unit tests, but not actually used?
                 # Case: d/dt [w[...] + t v[...]]
                 # Case: d/dt [w[...] + t v]
                 wval, wcomp = w.ufl_operands
                 if not wval == o:
                     continue
                 assert isinstance(wval, FormArgument)
                 if not all(isinstance(k, FixedIndex) for k in wcomp):
@@ -147,28 +166,30 @@
                     #       It may be good to have for debugging...
                     warnings.warn("Assuming d{%s}/d{%s} = 0." % (o, self._w))
             else:
                 # Make sure we have a tuple to match the self._v tuple
                 if not isinstance(oprimes, tuple):
                     oprimes = (oprimes,)
                     if len(oprimes) != len(self._v):
-                        raise ValueError("Got a tuple of arguments, "
-                                         "expecting a matching tuple of coefficient derivatives.")
+                        raise ValueError(
+                            "Got a tuple of arguments, "
+                            "expecting a matching tuple of coefficient derivatives."
+                        )
 
                 # Compute dg/dw_j = dg/dw_h : v.
                 # Since we may actually have a tuple of oprimes and vs in a
                 # 'mixed' space, sum over them all to get the complete inner
                 # product. Using indices to define a non-compound inner product.
-                for (oprime, v) in zip(oprimes, self._v):
+                for oprime, v in zip(oprimes, self._v):
                     raise ValueError("FIXME: Figure out how to do this with ngrads")
                     so, oi = as_scalar(oprime)
                     rv = len(v.ufl_shape)
                     oi1 = oi[:-rv]
                     oi2 = oi[-rv:]
-                    prod = so*v[oi2]
+                    prod = so * v[oi2]
                     if oi1:
                         gprimesum += as_tensor(prod, oi1)
                     else:
                         gprimesum += prod
 
         return (g, gprimesum)
 
@@ -178,44 +199,49 @@
     E3_1, ii = unit_indexed_tensor((3,), (1,))
     E22_10, ii = unit_indexed_tensor((2, 2), (1, 0))
     # TODO: Evaluate and assert values
 
 
 def test_unwrap_list_tensor(self):
     lt = as_tensor((1, 2))
-    expected = [((0,), 1),
-                ((1,), 2), ]
+    expected = [
+        ((0,), 1),
+        ((1,), 2),
+    ]
     comp = unwrap_list_tensor(lt)
     assert comp == expected
 
     lt = as_tensor(((1, 2), (3, 4)))
-    expected = [((0, 0), 1),
-                ((0, 1), 2),
-                ((1, 0), 3),
-                ((1, 1), 4), ]
+    expected = [
+        ((0, 0), 1),
+        ((0, 1), 2),
+        ((1, 0), 3),
+        ((1, 1), 4),
+    ]
     comp = unwrap_list_tensor(lt)
     assert comp == expected
 
-    lt = as_tensor((((1, 2), (3, 4)),
-                    ((11, 12), (13, 14))))
-    expected = [((0, 0, 0), 1),
-                ((0, 0, 1), 2),
-                ((0, 1, 0), 3),
-                ((0, 1, 1), 4),
-                ((1, 0, 0), 11),
-                ((1, 0, 1), 12),
-                ((1, 1, 0), 13),
-                ((1, 1, 1), 14), ]
+    lt = as_tensor((((1, 2), (3, 4)), ((11, 12), (13, 14))))
+    expected = [
+        ((0, 0, 0), 1),
+        ((0, 0, 1), 2),
+        ((0, 1, 0), 3),
+        ((0, 1, 1), 4),
+        ((1, 0, 0), 11),
+        ((1, 0, 1), 12),
+        ((1, 1, 0), 13),
+        ((1, 1, 1), 14),
+    ]
     comp = unwrap_list_tensor(lt)
     assert comp == expected
 
 
 def test__forward_coefficient_ad__grad_of_scalar_coefficient(self):
-    U = FiniteElement("CG", triangle, 1)
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    U = FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, U)
     u = Coefficient(space)
     du = TestFunction(space)
 
     mad = MockForwardAD()
     mad._w = (u,)
     mad._v = (du,)
@@ -232,16 +258,16 @@
     df = grad(grad(du))
     g, dg = mad.grad(f)
     assert g == f
     assert dg == df
 
 
 def test__forward_coefficient_ad__grad_of_vector_coefficient(self):
-    V = VectorElement("CG", triangle, 1)
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    V = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, V)
     v = Coefficient(space)
     dv = TestFunction(space)
 
     mad = MockForwardAD()
     mad._w = (v,)
     mad._v = (dv,)
@@ -258,130 +284,134 @@
     df = grad(grad(dv))
     g, dg = mad.grad(f)
     assert g == f
     assert dg == df
 
 
 def test__forward_coefficient_ad__grad_of_vector_coefficient__with_component_variation(self):
-    V = VectorElement("CG", triangle, 1)
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    V = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, V)
     v = Coefficient(space)
     dv = TestFunction(space)
 
     mad = MockForwardAD()
 
     # Component of variation:
     # grad(grad(c))[0,...] -> grad(grad(dc))[1,...]
     mad._w = (v[0],)
     mad._v = (dv[1],)
     f = grad(v)
     df = grad(as_vector((dv[1], 0)))  # Mathematically this would be the natural result
     j, k = indices(2)
-    df = as_tensor(Identity(2)[0, j]*grad(dv)[1, k], (j, k))  # Actual representation should have grad right next to dv
+    df = as_tensor(
+        Identity(2)[0, j] * grad(dv)[1, k], (j, k)
+    )  # Actual representation should have grad right next to dv
     g, dg = mad.grad(f)
     if 0:
-        print(('\nf    ', f))
-        print(('df   ', df))
-        print(('g    ', g))
-        print(('dg   ', dg))
+        print(("\nf    ", f))
+        print(("df   ", df))
+        print(("g    ", g))
+        print(("dg   ", dg))
     assert f.ufl_shape == df.ufl_shape
     assert g.ufl_shape == f.ufl_shape
     assert dg.ufl_shape == df.ufl_shape
     assert g == f
-    self.assertEqual((inner(dg, dg)*dx).signature(),
-                     (inner(df, df)*dx).signature())
+    self.assertEqual((inner(dg, dg) * dx).signature(), (inner(df, df) * dx).signature())
     # assert dg == df # Expected to fail because of different index numbering
 
     # Multiple components of variation:
     # grad(grad(c))[0,1,:,:] -> grad(grad(dc))[1,0,:,:]
     mad._w = (v[0], v[1])
     mad._v = (dv[1], dv[0])
     f = grad(v)
     # Mathematically this would be the natural result:
     df = grad(as_vector((dv[1], dv[0])))
     # Actual representation should have grad right next to dv:
     j0, k0 = indices(2)
     j1, k1 = indices(2)  # Using j0,k0 for both terms gives different signature
-    df = (as_tensor(Identity(2)[0, j0]*grad(dv)[1, k0], (j0, k0))
-          + as_tensor(Identity(2)[1, j1]*grad(dv)[0, k1], (j1, k1)))
-    g, dg = mad.grad(f)
-    print(('\nf    ', f))
-    print(('df   ', df))
-    print(('g    ', g))
-    print(('dg   ', dg))
+    df = as_tensor(Identity(2)[0, j0] * grad(dv)[1, k0], (j0, k0)) + as_tensor(
+        Identity(2)[1, j1] * grad(dv)[0, k1], (j1, k1)
+    )
+    g, dg = mad.grad(f)
+    print(("\nf    ", f))
+    print(("df   ", df))
+    print(("g    ", g))
+    print(("dg   ", dg))
     assert f.ufl_shape == df.ufl_shape
     assert g.ufl_shape == f.ufl_shape
     assert dg.ufl_shape == df.ufl_shape
     assert g == f
-    self.assertEqual((inner(dg, dg)*dx).signature(),
-                     (inner(df, df)*dx).signature())
+    self.assertEqual((inner(dg, dg) * dx).signature(), (inner(df, df) * dx).signature())
     # assert dg == df # Expected to fail because of different index numbering
 
 
-def test__forward_coefficient_ad__grad_of_vector_coefficient__with_component_variation_in_list(self):
-    V = VectorElement("CG", triangle, 1)
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+def test__forward_coefficient_ad__grad_of_vector_coefficient__with_component_variation_in_list(
+    self,
+):
+    V = FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, V)
     v = Coefficient(space)
     dv = TestFunction(space)
 
     mad = MockForwardAD()
 
     # Component of variation:
     # grad(grad(c))[0,...] -> grad(grad(dc))[1,...]
     mad._w = (v,)
     mad._v = (as_vector((dv[1], 0)),)
     f = grad(v)
     df = grad(as_vector((dv[1], 0)))  # Mathematically this would be the natural result
     j, k = indices(2)
-    df = as_tensor(Identity(2)[0, j]*grad(dv)[1, k], (j, k))  # Actual representation should have grad right next to dv
+    df = as_tensor(
+        Identity(2)[0, j] * grad(dv)[1, k], (j, k)
+    )  # Actual representation should have grad right next to dv
     g, dg = mad.grad(f)
     if 0:
-        print(('\nf    ', f))
-        print(('df   ', df))
-        print(('g    ', g))
-        print(('dg   ', dg))
+        print(("\nf    ", f))
+        print(("df   ", df))
+        print(("g    ", g))
+        print(("dg   ", dg))
     assert f.ufl_shape == df.ufl_shape
     assert g.ufl_shape == f.ufl_shape
     assert dg.ufl_shape == df.ufl_shape
     assert g == f
-    self.assertEqual((inner(dg, dg)*dx).signature(),
-                     (inner(df, df)*dx).signature())
+    self.assertEqual((inner(dg, dg) * dx).signature(), (inner(df, df) * dx).signature())
     # assert dg == df # Expected to fail because of different index numbering
 
     # Multiple components of variation:
     # grad(grad(c))[0,1,:,:] -> grad(grad(dc))[1,0,:,:]
-    mad._w = (v, )
+    mad._w = (v,)
     mad._v = (as_vector((dv[1], dv[0])),)
     f = grad(v)
     # Mathematically this would be the natural result:
     df = grad(as_vector((dv[1], dv[0])))
     # Actual representation should have grad right next to dv:
     j0, k0 = indices(2)
     j1, k1 = indices(2)  # Using j0,k0 for both terms gives different signature
-    df = (as_tensor(Identity(2)[0, j0]*grad(dv)[1, k0], (j0, k0))
-          + as_tensor(Identity(2)[1, j1]*grad(dv)[0, k1], (j1, k1)))
-    g, dg = mad.grad(f)
-    print(('\nf    ', f))
-    print(('df   ', df))
-    print(('g    ', g))
-    print(('dg   ', dg))
+    df = as_tensor(Identity(2)[0, j0] * grad(dv)[1, k0], (j0, k0)) + as_tensor(
+        Identity(2)[1, j1] * grad(dv)[0, k1], (j1, k1)
+    )
+    g, dg = mad.grad(f)
+    print(("\nf    ", f))
+    print(("df   ", df))
+    print(("g    ", g))
+    print(("dg   ", dg))
     assert f.ufl_shape == df.ufl_shape
     assert g.ufl_shape == f.ufl_shape
     assert dg.ufl_shape == df.ufl_shape
     assert g == f
-    self.assertEqual((inner(dg, dg)*dx).signature(),
-                     (inner(df, df)*dx).signature())
+    self.assertEqual((inner(dg, dg) * dx).signature(), (inner(df, df) * dx).signature())
     # assert dg == df # Expected to fail because of different index numbering
 
 
 def test__forward_coefficient_ad__grad_of_tensor_coefficient(self):
-    W = TensorElement("CG", triangle, 1)
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    W = FiniteElement("Lagrange", triangle, 1, (2, 2), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, W)
     w = Coefficient(space)
     dw = TestFunction(space)
 
     mad = MockForwardAD()
     mad._w = (w,)
     mad._v = (dw,)
@@ -398,16 +428,16 @@
     df = grad(grad(dw))
     g, dg = mad.grad(f)
     assert g == f
     assert dg == df
 
 
 def test__forward_coefficient_ad__grad_of_tensor_coefficient__with_component_variation(self):
-    W = TensorElement("CG", triangle, 1)
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    W = FiniteElement("Lagrange", triangle, 1, (2, 2), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, W)
     w = Coefficient(space)
     dw = TestFunction(space)
 
     mad = MockForwardAD()
 
     # Component of variation:
@@ -417,21 +447,20 @@
     mad._w = (w[wc],)
     mad._v = (dw[dwc],)
     f = grad(w)
     df = grad(as_matrix(((0, 0), (dw[dwc], 0))))  # Mathematically this is it.
     i, j, k = indices(3)
     E = outer(Identity(2)[wc[0], i], Identity(2)[wc[1], j])
     Ddw = grad(dw)[dwc + (k,)]
-    df = as_tensor(E*Ddw, (i, j, k))  # Actual representation should have grad next to dv
+    df = as_tensor(E * Ddw, (i, j, k))  # Actual representation should have grad next to dv
     g, dg = mad.grad(f)
     if 0:
-        print(('\nf    ', f))
-        print(('df   ', df))
-        print(('g    ', g))
-        print(('dg   ', dg))
+        print(("\nf    ", f))
+        print(("df   ", df))
+        print(("g    ", g))
+        print(("dg   ", dg))
     assert f.ufl_shape == df.ufl_shape
     assert g.ufl_shape == f.ufl_shape
     assert dg.ufl_shape == df.ufl_shape
     assert g == f
-    self.assertEqual((inner(dg, dg)*dx).signature(),
-                     (inner(df, df)*dx).signature())
+    self.assertEqual((inner(dg, dg) * dx).signature(), (inner(df, df) * dx).signature())
     # assert dg == df # Expected to fail because of different index numbering
```

### Comparing `fenics-ufl-2023.2.0/test/test_signature.py` & `fenics_ufl-2024.1.0.post0/test/test_signature.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,56 @@
 """Test the computation of form signatures."""
 
-from ufl import (Argument, CellDiameter, CellVolume, Circumradius, Coefficient, FacetArea, FacetNormal, FiniteElement,
-                 FunctionSpace, Identity, Mesh, SpatialCoordinate, TensorElement, TestFunction, VectorElement,
-                 as_vector, diff, dot, ds, dx, hexahedron, indices, inner, interval, quadrilateral, tetrahedron,
-                 triangle, variable)
+from ufl import (
+    Argument,
+    CellDiameter,
+    CellVolume,
+    Circumradius,
+    Coefficient,
+    FacetArea,
+    FacetNormal,
+    FunctionSpace,
+    Identity,
+    Mesh,
+    SpatialCoordinate,
+    TestFunction,
+    as_vector,
+    diff,
+    dot,
+    ds,
+    dx,
+    hexahedron,
+    indices,
+    inner,
+    interval,
+    quadrilateral,
+    tetrahedron,
+    triangle,
+    variable,
+)
 from ufl.algorithms.signature import compute_multiindex_hashdata, compute_terminal_hashdata
 from ufl.classes import FixedIndex, MultiIndex
+from ufl.finiteelement import FiniteElement, SymmetricElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1, L2
 
 # TODO: Test compute_terminal_hashdata
 #   TODO: Check that form argument counts only affect the sig by their relative ordering
 #   TODO: Check that all other relevant terminal propeties affect the terminal_hashdata
 
 # TODO: Test that operator types affect the sig
 # TODO: Test that we do not get collisions for some large sets of generated forms
 # TODO: How do we know that we have tested the signature reliably enough?
 
 
 def domain_numbering(*cells):
     renumbering = {}
     for i, cell in enumerate(cells):
-        domain = Mesh(VectorElement("Lagrange", cell, 1), ufl_id=i)
+        d = cell.topological_dimension()
+        domain = Mesh(FiniteElement("Lagrange", cell, 1, (d,), identity_pullback, H1), ufl_id=i)
         renumbering[domain] = i
     return renumbering
 
 
 def compute_unique_terminal_hashdatas(hashdatas):
     count = 0
     data = set()
@@ -53,20 +80,22 @@
 def test_terminal_hashdata_depends_on_literals(self):
     reprs = set()
     hashes = set()
 
     def forms():
         i, j = indices(2)
         for d, cell in [(2, triangle), (3, tetrahedron)]:
-            domain = Mesh(VectorElement("Lagrange", cell, 1), ufl_id=d-2)
+            domain = Mesh(
+                FiniteElement("Lagrange", cell, 1, (d,), identity_pullback, H1), ufl_id=d - 2
+            )
             x = SpatialCoordinate(domain)
             ident = Identity(d)
             for fv in (1.1, 2.2):
                 for iv in (5, 7):
-                    expr = (ident[0, j]*(fv*x[j]))**iv
+                    expr = (ident[0, j] * (fv * x[j])) ** iv
 
                     reprs.add(repr(expr))
                     hashes.add(hash(expr))
                     yield compute_terminal_hashdata(expr, {domain: 0})
 
     c, d, r, h = compute_unique_terminal_hashdatas(forms())
     assert c == 8
@@ -81,70 +110,103 @@
     reprs = set()
     hashes = set()
 
     def forms():
         i, j = indices(2)
         cells = (triangle, tetrahedron)
         for i, cell in enumerate(cells):
-            domain = Mesh(VectorElement("Lagrange", cell, 1), ufl_id=i)
+            d = cell.topological_dimension()
+            domain = Mesh(FiniteElement("Lagrange", cell, 1, (d,), identity_pullback, H1), ufl_id=i)
 
-            d = cell.geometric_dimension()
             x = SpatialCoordinate(domain)
             n = FacetNormal(domain)
             h = CellDiameter(domain)
             r = Circumradius(domain)
             a = FacetArea(domain)
             # s = CellSurfaceArea(domain)
             v = CellVolume(domain)
             ident = Identity(d)
 
             ws = (x, n)
             qs = (h, r, a, v)  # , s)
             for w in ws:
                 for q in qs:
-                    expr = (ident[0, j]*(q*w[j]))
+                    expr = ident[0, j] * (q * w[j])
 
                     reprs.add(repr(expr))
                     hashes.add(hash(expr))
                     yield compute_terminal_hashdata(expr, domain_numbering(*cells))
 
     c, d, r, h = compute_unique_terminal_hashdatas(forms())
-    assert c == 2*4*2  # len(ws)*len(qs)*len(cells)
+    assert c == 2 * 4 * 2  # len(ws)*len(qs)*len(cells)
     assert d == c
     assert r == c
     assert h == c
     assert len(reprs) == c
     assert len(hashes) == c
 
 
 def test_terminal_hashdata_depends_on_form_argument_properties(self):
     reprs = set()
     hashes = set()
-    nelm = 6
+    nelm = 5
     nreps = 2
 
     # Data
     cells = (triangle, tetrahedron)
     degrees = (1, 2)
-    families = ("CG", "Lagrange", "DG")
+    families = (("Lagrange", H1), ("Lagrange", H1), ("Discontinuous Lagrange", L2))
 
     def forms():
         for rep in range(nreps):
             for i, cell in enumerate(cells):
-                d = cell.geometric_dimension()
-                domain = Mesh(VectorElement("Lagrange", cell, 1), ufl_id=i)
+                d = cell.topological_dimension()
+                domain = Mesh(
+                    FiniteElement("Lagrange", cell, 1, (d,), identity_pullback, H1), ufl_id=i
+                )
                 for degree in degrees:
-                    for family in families:
-                        V = FiniteElement(family, cell, degree)
-                        W = VectorElement(family, cell, degree)
-                        W2 = VectorElement(family, cell, degree, dim=d+1)
-                        T = TensorElement(family, cell, degree)
-                        S = TensorElement(family, cell, degree, symmetry=True)
-                        S2 = TensorElement(family, cell, degree, shape=(d, d), symmetry={(0, 0): (1, 1)})
-                        elements = [V, W, W2, T, S, S2]
+                    for family, sobolev in families:
+                        V = FiniteElement(family, cell, degree, (), identity_pullback, sobolev)
+                        W = FiniteElement(family, cell, degree, (d,), identity_pullback, sobolev)
+                        W2 = FiniteElement(
+                            family, cell, degree, (d + 1,), identity_pullback, sobolev
+                        )
+                        T = FiniteElement(family, cell, degree, (d, d), identity_pullback, sobolev)
+                        if d == 2:
+                            S = SymmetricElement(
+                                {(0, 0): 0, (0, 1): 1, (1, 0): 1, (1, 1): 2},
+                                [
+                                    FiniteElement(
+                                        family, cell, degree, (), identity_pullback, sobolev
+                                    )
+                                    for _ in range(3)
+                                ],
+                            )
+                        else:
+                            assert d == 3
+                            S = SymmetricElement(
+                                {
+                                    (0, 0): 0,
+                                    (0, 1): 1,
+                                    (0, 2): 2,
+                                    (1, 0): 1,
+                                    (1, 1): 3,
+                                    (1, 2): 4,
+                                    (2, 0): 2,
+                                    (2, 1): 4,
+                                    (2, 2): 5,
+                                },
+                                [
+                                    FiniteElement(
+                                        family, cell, degree, (), identity_pullback, sobolev
+                                    )
+                                    for _ in range(6)
+                                ],
+                            )
+                        elements = [V, W, W2, T, S]
                         assert len(elements) == nelm
 
                         for H in elements[:nelm]:
                             space = FunctionSpace(domain, H)
                             # Keep number and count fixed, we're not testing that here
                             a = Argument(space, number=1)
                             c = Coefficient(space, count=1)
@@ -154,19 +216,18 @@
                                 expr = inner(f, f)
 
                                 reprs.add(repr(expr))
                                 hashes.add(hash(expr))
                                 yield compute_terminal_hashdata(expr, renumbering)
 
     c, d, r, h = compute_unique_terminal_hashdatas(forms())
-    c1 = nreps * len(cells) * len(degrees) * len(families) * nelm * 2  # Number of cases with repetitions
+    c1 = nreps * len(cells) * len(degrees) * len(families) * nelm * 2
     assert c == c1
 
-    c0 = len(cells) * len(degrees) * (len(families)-1) * nelm * 2  # Number of unique cases, "CG" == "Lagrange"
-    # c0 = len(cells) * len(degrees) * (len(families)) * nelm * 2 # Number of unique cases, "CG" != "Lagrange"
+    c0 = len(cells) * len(degrees) * (len(families) - 1) * nelm * 2
     assert d == c0
     assert r == c0
     assert h == c0
     assert len(reprs) == c0
     assert len(hashes) == c0
 
 
@@ -177,20 +238,23 @@
     cells = (interval, triangle, hexahedron)
     assert len(counts) == 7
     nreps = 1
 
     def forms():
         for rep in range(nreps):
             for i, cell in enumerate(cells):
-                domain = Mesh(VectorElement("Lagrange", cell, 1), ufl_id=i)
+                d = cell.topological_dimension()
+                domain = Mesh(
+                    FiniteElement("Lagrange", cell, 1, (d,), identity_pullback, H1), ufl_id=i
+                )
                 for k in counts:
-                    V = FiniteElement("CG", cell, 2)
+                    V = FiniteElement("Lagrange", cell, 2, (), identity_pullback, H1)
                     space = FunctionSpace(domain, V)
                     f = Coefficient(space, count=k)
-                    g = Coefficient(space, count=k+2)
+                    g = Coefficient(space, count=k + 2)
                     expr = inner(f, g)
 
                     renumbering = domain_numbering(*cells)
                     renumbering[f] = 0
                     renumbering[g] = 1
 
                     reprs.add(repr(expr))
@@ -215,28 +279,33 @@
     counts = list(range(4))
     cells = (interval, triangle, hexahedron)
     nreps = 2
 
     def forms():
         for rep in range(nreps):
             for i, cell in enumerate(cells):
-                domain = Mesh(VectorElement("Lagrange", cell, 1), ufl_id=i)
+                d = cell.topological_dimension()
+                domain = Mesh(
+                    FiniteElement("Lagrange", cell, 1, (d,), identity_pullback, H1), ufl_id=i
+                )
                 for k in counts:
-                    V = FiniteElement("CG", cell, 2)
+                    V = FiniteElement("Lagrange", cell, 2, (), identity_pullback, H1)
                     space = FunctionSpace(domain, V)
                     f = Argument(space, k)
-                    g = Argument(space, k+2)
+                    g = Argument(space, k + 2)
                     expr = inner(f, g)
 
                     reprs.add(repr(expr))
                     hashes.add(hash(expr))
                     yield compute_terminal_hashdata(expr, domain_numbering(*cells))
 
     c, d, r, h = compute_unique_terminal_hashdatas(forms())
-    c0 = len(cells) * len(counts)  # Number of actually unique cases from a code generation perspective
+    c0 = len(cells) * len(
+        counts
+    )  # Number of actually unique cases from a code generation perspective
     c1 = 1 * c0  # Number of unique cases from a symbolic representation perspective
     assert len(reprs) == c1
     assert len(hashes) == c1
     self.assertEqual(c, nreps * c1)  # number of inner loop executions in forms() above
     assert d == c0
     assert r == c0
     assert h == c0
@@ -244,15 +313,16 @@
 
 def test_domain_signature_data_does_not_depend_on_domain_label_value(self):
     cells = [triangle, tetrahedron, hexahedron]
     s0s = set()
     s1s = set()
     s2s = set()
     for i, cell in enumerate(cells):
-        domain = VectorElement("Lagrange", cell, 1)
+        d = cell.topological_dimension()
+        domain = FiniteElement("Lagrange", cell, 1, (d,), identity_pullback, H1)
         d0 = Mesh(domain)
         d1 = Mesh(domain, ufl_id=1)
         d2 = Mesh(domain, ufl_id=2)
         s0 = d0._ufl_signature_data_({d0: 0})
         s1 = d1._ufl_signature_data_({d1: 0})
         s2 = d2._ufl_signature_data_({d2: 0})
         assert s0 == s1
@@ -266,22 +336,34 @@
 
 
 def test_terminal_hashdata_does_not_depend_on_domain_label_value(self):
     reprs = set()
     hashes = set()
     ufl_ids = [1, 2]
     cells = [triangle, quadrilateral]
-    domains = [Mesh(cell, ufl_id=ufl_id) for cell in cells for ufl_id in ufl_ids]
+    domains = [
+        Mesh(
+            FiniteElement(
+                "Lagrange", cell, 1, (cell.topological_dimension(),), identity_pullback, H1
+            ),
+            ufl_id=ufl_id,
+        )
+        for cell in cells
+        for ufl_id in ufl_ids
+    ]
     nreps = 2
     num_exprs = 2
 
     def forms():
         for rep in range(nreps):
             for domain in domains:
-                V = FunctionSpace(domain, FiniteElement("CG", domain.ufl_cell(), 2))
+                V = FunctionSpace(
+                    domain,
+                    FiniteElement("Lagrange", domain.ufl_cell(), 2, (), identity_pullback, H1),
+                )
                 f = Coefficient(V, count=0)
                 v = TestFunction(V)
                 x = SpatialCoordinate(domain)
                 n = FacetNormal(domain)
                 exprs = [inner(x, n), inner(f, v)]
                 assert num_exprs == len(exprs)  # Assumed in checks below
 
@@ -290,16 +372,20 @@
 
                 for expr in exprs:
                     reprs.add(repr(expr))
                     hashes.add(hash(expr))
                     yield compute_terminal_hashdata(expr, renumbering)
 
     c, d, r, h = compute_unique_terminal_hashdatas(forms())
-    c0 = num_exprs * len(cells)  # Number of actually unique cases from a code generation perspective
-    c1 = num_exprs * len(domains)  # Number of unique cases from a symbolic representation perspective
+    c0 = num_exprs * len(
+        cells
+    )  # Number of actually unique cases from a code generation perspective
+    c1 = num_exprs * len(
+        domains
+    )  # Number of unique cases from a symbolic representation perspective
     assert len(reprs) == c1
     assert len(hashes) == c1
     self.assertEqual(c, nreps * c1)  # number of inner loop executions in forms() above
     assert d == c0
     assert r == c0
     assert h == c0
 
@@ -328,17 +414,17 @@
                 expr = MultiIndex(jj)
                 reprs.add(repr(expr))
                 hashes.add(hash(expr))
                 yield compute_multiindex_hashdata(expr, {})
 
     c, d, r, h = compute_unique_multiindex_hashdatas(hashdatas())
     assert c == 9
-    assert d == 9-1  # (1,0 is repeated, therefore -1)
-    assert len(reprs) == 9-1
-    assert len(hashes) == 9-1
+    assert d == 9 - 1  # (1,0 is repeated, therefore -1)
+    assert len(reprs) == 9 - 1
+    assert len(hashes) == 9 - 1
 
 
 def test_multiindex_hashdata_does_not_depend_on_counts(self):
     reprs = set()
     hashes = set()
 
     def hashdatas():
@@ -351,50 +437,54 @@
                 ijs.append((i, j))
                 ijs.append((j, i))
         for ij in ijs:
             expr = MultiIndex(ij)
             reprs.add(repr(expr))
             hashes.add(hash(expr))
             yield compute_multiindex_hashdata(expr, {})
+
     c, d, r, h = compute_unique_multiindex_hashdatas(hashdatas())
-    assert c == 3+9+9
-    assert d == 1+1
-    assert len(reprs) == 3+9+9
-    assert len(hashes) == 3+9+9
+    assert c == 3 + 9 + 9
+    assert d == 1 + 1
+    assert len(reprs) == 3 + 9 + 9
+    assert len(hashes) == 3 + 9 + 9
 
 
 def test_multiindex_hashdata_depends_on_the_order_indices_are_observed(self):
     reprs = set()
     hashes = set()
     nrep = 3
 
     def hashdatas():
         for rep in range(nrep):
-            # Resetting index_numbering for each repetition,
-            # resulting in hashdata staying the same for
-            # each repetition but repr and hashes changing
-            # because new indices are created each repetition.
+            # Resetting index_numbering for each repetition, resulting
+            # in hashdata staying the same for each repetition but repr
+            # and hashes changing because new indices are created each
+            # repetition.
             index_numbering = {}
             i, j, k, l = indices(4)  # noqa: E741
-            for expr in (MultiIndex((i,)),
-                         MultiIndex((i,)),  # r
-                         MultiIndex((i, j)),
-                         MultiIndex((j, i)),
-                         MultiIndex((i, j)),  # r
-                         MultiIndex((i, j, k)),
-                         MultiIndex((k, j, i)),
-                         MultiIndex((j, i))):  # r
+            for expr in (
+                MultiIndex((i,)),
+                MultiIndex((i,)),  # r
+                MultiIndex((i, j)),
+                MultiIndex((j, i)),
+                MultiIndex((i, j)),  # r
+                MultiIndex((i, j, k)),
+                MultiIndex((k, j, i)),
+                MultiIndex((j, i)),
+            ):  # r
                 reprs.add(repr(expr))
                 hashes.add(hash(expr))
                 yield compute_multiindex_hashdata(expr, index_numbering)
+
     c, d, r, h = compute_unique_multiindex_hashdatas(hashdatas())
-    assert c == nrep*8
+    assert c == nrep * 8
     assert d == 5
-    assert len(reprs) == nrep*5
-    assert len(hashes) == nrep*5
+    assert len(reprs) == nrep * 5
+    assert len(hashes) == nrep * 5
 
 
 def check_unique_signatures(forms):
     count = 0
     sigs = set()
     sigs2 = set()
     hashes = set()
@@ -412,94 +502,104 @@
     assert len(sigs2) == count
     assert len(reprs) == count
     assert len(hashes) == count
 
 
 def test_signature_is_affected_by_element_properties(self):
     def forms():
-        for family in ("CG", "DG"):
+        for family, sobolev in (("Lagrange", H1), ("Discontinuous Lagrange", L2)):
             for cell in (triangle, tetrahedron, quadrilateral):
-                domain = Mesh(VectorElement("Lagrange", cell, 1))
+                d = cell.topological_dimension()
+                domain = Mesh(FiniteElement("Lagrange", cell, 1, (d,), identity_pullback, H1))
                 for degree in (1, 2):
-                    V = FiniteElement(family, cell, degree)
+                    V = FiniteElement(family, cell, degree, (), identity_pullback, sobolev)
                     space = FunctionSpace(domain, V)
                     u = Coefficient(space)
                     v = TestFunction(space)
                     x = SpatialCoordinate(domain)
-                    w = as_vector([v]*x.ufl_shape[0])
-                    f = dot(w, u*x)
-                    a = f*dx
+                    w = as_vector([v] * x.ufl_shape[0])
+                    f = dot(w, u * x)
+                    a = f * dx
                     yield a
+
     check_unique_signatures(forms())
 
 
 def test_signature_is_affected_by_domains(self):
     def forms():
         for cell in (triangle, tetrahedron):
-            domain = Mesh(VectorElement("Lagrange", cell, 1))
+            d = cell.topological_dimension()
+            domain = Mesh(FiniteElement("Lagrange", cell, 1, (d,), identity_pullback, H1))
             for di in (1, 2):
                 for dj in (1, 2):
                     for dk in (1, 2):
-                        V = FiniteElement("CG", cell, 1)
+                        V = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
                         space = FunctionSpace(domain, V)
                         u = Coefficient(space)
-                        a = u*dx(di) + 2*u*dx(dj) + 3*u*ds(dk)
+                        a = u * dx(di) + 2 * u * dx(dj) + 3 * u * ds(dk)
                         yield a
+
     check_unique_signatures(forms())
 
 
 def test_signature_of_forms_with_diff(self):
     def forms():
         for i, cell in enumerate([triangle, tetrahedron]):
-            domain = Mesh(VectorElement("Lagrange", cell, 1), ufl_id=i)
+            d = cell.topological_dimension()
+            domain = Mesh(FiniteElement("Lagrange", cell, 1, (d,), identity_pullback, H1), ufl_id=i)
             for k in (1, 2, 3):
-                V = FiniteElement("CG", cell, 1)
-                W = VectorElement("CG", cell, 1)
+                d = cell.topological_dimension()
+                V = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+                W = FiniteElement("Lagrange", cell, 1, (d,), identity_pullback, H1)
                 v_space = FunctionSpace(domain, V)
                 w_space = FunctionSpace(domain, W)
                 u = Coefficient(v_space)
                 w = Coefficient(w_space)
                 vu = variable(u)
                 vw = variable(w)
-                f = vu*dot(vw, vu**k*vw)
+                f = vu * dot(vw, vu**k * vw)
                 g = diff(f, vu)
                 h = dot(diff(f, vw), FacetNormal(domain))
-                a = f*dx(1) + g*dx(2) + h*ds(0)
+                a = f * dx(1) + g * dx(2) + h * ds(0)
                 yield a
+
     check_unique_signatures(forms())
 
 
 def test_signature_of_form_depend_on_coefficient_numbering_across_integrals(self):
     cell = triangle
-    V = FiniteElement("CG", cell, 1)
-    domain = Mesh(VectorElement("Lagrange", cell, 1))
+    V = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+    domain = Mesh(FiniteElement("Lagrange", cell, 1, (2,), identity_pullback, H1))
     space = FunctionSpace(domain, V)
     f = Coefficient(space)
     g = Coefficient(space)
-    M1 = f*dx(0) + g*dx(1)
-    M2 = g*dx(0) + f*dx(1)
-    M3 = g*dx(0) + g*dx(1)
+    M1 = f * dx(0) + g * dx(1)
+    M2 = g * dx(0) + f * dx(1)
+    M3 = g * dx(0) + g * dx(1)
     self.assertTrue(M1.signature() != M2.signature())
     self.assertTrue(M1.signature() != M3.signature())
     self.assertTrue(M2.signature() != M3.signature())
 
 
 def test_signature_of_forms_change_with_operators(self):
     def forms():
         for cell in (triangle, tetrahedron):
-            V = FiniteElement("CG", cell, 1)
-            domain = Mesh(VectorElement("Lagrange", cell, 1))
+            d = cell.topological_dimension()
+            V = FiniteElement("Lagrange", cell, 1, (), identity_pullback, H1)
+            domain = Mesh(FiniteElement("Lagrange", cell, 1, (d,), identity_pullback, H1))
             space = FunctionSpace(domain, V)
             u = Coefficient(space)
             v = Coefficient(space)
-            fs = [(u*v)+(u/v),
-                  (u+v)+(u/v),
-                  (u+v)*(u/v),
-                  (u*v)*(u*v),
-                  (u+v)*(u*v),  # (!) same
-                  # (u*v)*(u+v), # (!) same
-                  (u*v)+(u+v),
-                  ]
+            fs = [
+                (u * v) + (u / v),
+                (u + v) + (u / v),
+                (u + v) * (u / v),
+                (u * v) * (u * v),
+                (u + v) * (u * v),  # H1 same
+                # (u*v)*(u+v), # H1 same
+                (u * v) + (u + v),
+            ]
             for f in fs:
-                a = f*dx
+                a = f * dx
                 yield a
+
     check_unique_signatures(forms())
```

### Comparing `fenics-ufl-2023.2.0/test/test_str.py` & `fenics_ufl-2024.1.0.post0/test/test_str.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,117 +1,142 @@
-from ufl import (CellDiameter, CellVolume, Circumradius, FacetArea, FacetNormal, FiniteElement, FunctionSpace, Index,
-                 Mesh, SpatialCoordinate, TestFunction, TrialFunction, VectorElement, as_matrix, as_ufl, as_vector,
-                 quadrilateral, tetrahedron, triangle)
+from ufl import (
+    CellDiameter,
+    CellVolume,
+    Circumradius,
+    FacetArea,
+    FacetNormal,
+    FunctionSpace,
+    Index,
+    Mesh,
+    SpatialCoordinate,
+    TestFunction,
+    TrialFunction,
+    as_matrix,
+    as_ufl,
+    as_vector,
+    quadrilateral,
+    tetrahedron,
+    triangle,
+)
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 
 def test_str_int_value(self):
     assert str(as_ufl(3)) == "3"
 
 
 def test_str_float_value(self):
     assert str(as_ufl(3.14)) == "3.14"
 
 
 def test_str_zero(self):
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     x = SpatialCoordinate(domain)
     assert str(as_ufl(0)) == "0"
-    assert str(0*x) == "0 (shape (2,))"
-    assert str(0*x*x[Index(42)]) == "0 (shape (2,), index labels (42,))"
+    assert str(0 * x) == "0 (shape (2,))"
+    assert str(0 * x * x[Index(42)]) == "0 (shape (2,), index labels (42,))"
 
 
 def test_str_index(self):
     assert str(Index(3)) == "i_3"
     assert str(Index(42)) == "i_{42}"
 
 
 def test_str_coordinate(self):
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     assert str(SpatialCoordinate(domain)) == "x"
     assert str(SpatialCoordinate(domain)[0]) == "x[0]"
 
 
 def test_str_normal(self):
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     assert str(FacetNormal(domain)) == "n"
     assert str(FacetNormal(domain)[0]) == "n[0]"
 
 
 def test_str_circumradius(self):
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     assert str(Circumradius(domain)) == "circumradius"
 
 
 def test_str_diameter(self):
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     assert str(CellDiameter(domain)) == "diameter"
 
 
 def test_str_facetarea(self):
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     assert str(FacetArea(domain)) == "facetarea"
 
 
 def test_str_volume(self):
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     assert str(CellVolume(domain)) == "volume"
 
 
 def test_str_scalar_argument(self):
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
-    v = TestFunction(FunctionSpace(domain, FiniteElement("CG", triangle, 1)))
-    u = TrialFunction(FunctionSpace(domain, FiniteElement("CG", triangle, 1)))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
+    v = TestFunction(
+        FunctionSpace(domain, FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1))
+    )
+    u = TrialFunction(
+        FunctionSpace(domain, FiniteElement("Lagrange", triangle, 1, (), identity_pullback, H1))
+    )
     assert str(v) == "v_0"
     assert str(u) == "v_1"
 
 
 # def test_str_vector_argument(self): # FIXME
 
 # def test_str_scalar_coefficient(self): # FIXME
 
 # def test_str_vector_coefficient(self): # FIXME
 
 
 def test_str_list_vector():
-    domain = Mesh(VectorElement("Lagrange", tetrahedron, 1))
+    domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
     x, y, z = SpatialCoordinate(domain)
     v = as_vector((x, y, z))
     assert str(v) == ("[%s, %s, %s]" % (x, y, z))
 
 
 def test_str_list_vector_with_zero():
-    domain = Mesh(VectorElement("Lagrange", tetrahedron, 1))
+    domain = Mesh(FiniteElement("Lagrange", tetrahedron, 1, (3,), identity_pullback, H1))
     x, y, z = SpatialCoordinate(domain)
     v = as_vector((x, 0, 0))
     assert str(v) == ("[%s, 0, 0]" % (x,))
 
 
 def test_str_list_matrix():
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     x, y = SpatialCoordinate(domain)
-    v = as_matrix(((2*x, 3*y),
-                   (4*x, 5*y)))
-    a = str(2*x)
-    b = str(3*y)
-    c = str(4*x)
-    d = str(5*y)
+    v = as_matrix(((2 * x, 3 * y), (4 * x, 5 * y)))
+    a = str(2 * x)
+    b = str(3 * y)
+    c = str(4 * x)
+    d = str(5 * y)
     assert str(v) == ("[\n  [%s, %s],\n  [%s, %s]\n]" % (a, b, c, d))
 
 
 def test_str_list_matrix_with_zero():
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     x, y = SpatialCoordinate(domain)
-    v = as_matrix(((2*x, 3*y),
-                   (0, 0)))
-    a = str(2*x)
-    b = str(3*y)
+    v = as_matrix(((2 * x, 3 * y), (0, 0)))
+    a = str(2 * x)
+    b = str(3 * y)
     c = str(as_vector((0, 0)))
     assert str(v) == ("[\n  [%s, %s],\n%s\n]" % (a, b, c))
 
 
 # FIXME: Add more tests for tensors collapsing
 #        partly or completely into Zero!
 
 
 def test_str_element():
-    elem = FiniteElement("Q", quadrilateral, 1)
+    elem = FiniteElement("Q", quadrilateral, 1, (), identity_pullback, H1)
+    assert (
+        repr(elem)
+        == 'ufl.finiteelement.FiniteElement("Q", quadrilateral, 1, (), IdentityPullback(), H1)'
+    )
     assert str(elem) == "<Q1 on a quadrilateral>"
```

### Comparing `fenics-ufl-2023.2.0/test/test_tensoralgebra.py` & `fenics_ufl-2024.1.0.post0/test/test_tensoralgebra.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,39 @@
 """Test tensor algebra operators."""
 
 import pytest
 
-from ufl import (FacetNormal, Mesh, VectorElement, as_matrix, as_tensor, as_vector, cofac, cross, det, dev, diag,
-                 diag_vector, dot, inner, inv, outer, perp, skew, sym, tr, transpose, triangle, zero)
+from ufl import (
+    FacetNormal,
+    Mesh,
+    as_matrix,
+    as_tensor,
+    as_vector,
+    cofac,
+    cross,
+    det,
+    dev,
+    diag,
+    diag_vector,
+    dot,
+    inner,
+    inv,
+    outer,
+    perp,
+    skew,
+    sym,
+    tr,
+    transpose,
+    triangle,
+    zero,
+)
 from ufl.algorithms.remove_complex_nodes import remove_complex_nodes
+from ufl.finiteelement import FiniteElement
+from ufl.pullback import identity_pullback
+from ufl.sobolevspace import H1
 
 
 @pytest.fixture(scope="module")
 def A():
     return as_matrix([[2, 3], [4, 5]])
 
 
@@ -36,61 +61,60 @@
     assert B2 == B
     assert u2 == u
     assert v2 == v
 
 
 def test_outer(self, A, B, u, v):
     C = outer(u, v)
-    D = as_matrix([[10*30, 10*40], [20*30, 20*40]])
+    D = as_matrix([[10 * 30, 10 * 40], [20 * 30, 20 * 40]])
     self.assertEqualValues(C, D)
 
     C = outer(A, v)
     A, v = A, v
     dims = (0, 1)
-    D = as_tensor([[[A[i, j]*v[k] for k in dims] for j in dims] for i in dims])
+    D = as_tensor([[[A[i, j] * v[k] for k in dims] for j in dims] for i in dims])
     self.assertEqualValues(C, D)
 
     # TODO: Test other ranks
 
 
 def test_inner(self, A, B, u, v):
     C = inner(A, B)
-    D = 2*6 + 3*7 + 4*8 + 5*9
+    D = 2 * 6 + 3 * 7 + 4 * 8 + 5 * 9
     self.assertEqualValues(C, D)
 
     C = inner(u, v)
-    D = 10*30 + 20*40
+    D = 10 * 30 + 20 * 40
     self.assertEqualValues(C, D)
 
 
 def test_pow2_inner(self, A, u):
-    domain = Mesh(VectorElement("Lagrange", triangle, 1))
+    domain = Mesh(FiniteElement("Lagrange", triangle, 1, (2,), identity_pullback, H1))
     f = FacetNormal(domain)[0]
-    f2 = f*f
+    f2 = f * f
     assert f2 == remove_complex_nodes(inner(f, f))
 
     u2 = u**2
     assert u2 == remove_complex_nodes(inner(u, u))
 
     A2 = A**2
     assert A2 == remove_complex_nodes(inner(A, A))
 
     # Only tensor**2 notation is supported:
     self.assertRaises(BaseException, lambda: A**3)
 
 
 def test_dot(self, A, B, u, v):
     C = dot(u, v)
-    D = 10*30 + 20*40
+    D = 10 * 30 + 20 * 40
     self.assertEqualValues(C, D)
 
     C = dot(A, B)
     dims = (0, 1)
-    D = as_matrix([[sum(A[i, k]*B[k, j] for k in dims)
-                    for j in dims] for i in dims])
+    D = as_matrix([[sum(A[i, k] * B[k, j] for k in dims) for j in dims] for i in dims])
     self.assertEqualValues(C, D)
 
 
 def test_cross(self):
     u = as_vector([3, 3, 3])
     v = as_vector([2, 2, 2])
     C = cross(u, v)
@@ -124,29 +148,29 @@
     u = as_matrix([[1, 3], [0, 4]])  # Matrix instead of vector
     with pytest.raises(ValueError):
         v = perp(u)
 
 
 def xtest_dev(self, A):
     C = dev(A)
-    D = 0*C  # FIXME: Add expected value here
+    D = 0 * C  # FIXME: Add expected value here
     self.assertEqualValues(C, D)
 
 
 def test_skew(self, A):
     C = skew(A)
     A, dims = A, (0, 1)
-    D = 0.5*as_matrix([[A[i, j] - A[j, i] for j in dims] for i in dims])
+    D = 0.5 * as_matrix([[A[i, j] - A[j, i] for j in dims] for i in dims])
     self.assertEqualValues(C, D)
 
 
 def test_sym(self, A):
     C = sym(A)
     A, dims = A, (0, 1)
-    D = 0.5*as_matrix([[A[i, j] + A[j, i] for j in dims] for i in dims])
+    D = 0.5 * as_matrix([[A[i, j] + A[j, i] for j in dims] for i in dims])
     self.assertEqualValues(C, D)
 
 
 def test_transpose(self, A):
     C = transpose(A)
     dims = (0, 1)
     D = as_matrix([[A[j, i] for j in dims] for i in dims])
@@ -178,23 +202,23 @@
     D = sum(A[i, i] for i in dims)
     self.assertEqualValues(C, D)
 
 
 def test_det(self, A):
     dims = (0, 1)
     C = det(A)
-    D = sum((-A[i, 0]*A[0, i] if i != 0 else A[i-1, -1]*A[i, 0]) for i in dims)
+    D = sum((-A[i, 0] * A[0, i] if i != 0 else A[i - 1, -1] * A[i, 0]) for i in dims)
     self.assertEqualValues(C, D)
 
 
 def test_cofac(self, A):
     C = cofac(A)
     D = as_matrix([[(-A[i, j] if i != j else A[i, j]) for j in (-1, 0)] for i in (-1, 0)])
     self.assertEqualValues(C, D)
 
 
 def xtest_inv(self, A):
     # FIXME: Test fails probably due to integer division
     C = inv(A)
-    detA = sum((-A[i, 0]*A[0, i] if i != 0 else A[i-1, -1]*A[i, 0]) for i in (0, 1))
+    detA = sum((-A[i, 0] * A[0, i] if i != 0 else A[i - 1, -1] * A[i, 0]) for i in (0, 1))
     D = as_matrix([[(-A[i, j] if i != j else A[i, j]) for j in (-1, 0)] for i in (-1, 0)]) / detA
     self.assertEqualValues(C, D)
```

### Comparing `fenics-ufl-2023.2.0/test/test_utilities.py` & `fenics_ufl-2024.1.0.post0/test/test_utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,30 +27,42 @@
     assert 0 == flatten_multiindex((), shape_to_strides(()))
     assert 0 == flatten_multiindex((0,), shape_to_strides((2,)))
     assert 1 == flatten_multiindex((1,), shape_to_strides((2,)))
     assert 3 == flatten_multiindex((1, 1), shape_to_strides((2, 2)))
     for i in range(5):
         for j in range(3):
             for k in range(2):
-                assert 15*k+5*j+i == flatten_multiindex((k, j, i), shape_to_strides((2, 3, 5)))
+                assert 15 * k + 5 * j + i == flatten_multiindex(
+                    (k, j, i), shape_to_strides((2, 3, 5))
+                )
 
 
 def test_component_numbering():
     from ufl.permutation import build_component_numbering
+
     sh = (2, 2)
     sm = {(1, 0): (0, 1)}
     v, s = build_component_numbering(sh, sm)
     assert v == {(0, 1): 1, (1, 0): 1, (0, 0): 0, (1, 1): 2}
     assert s == [(0, 0), (0, 1), (1, 1)]
 
     sh = (3, 3)
     sm = {(1, 0): (0, 1), (2, 0): (0, 2), (2, 1): (1, 2)}
     v, s = build_component_numbering(sh, sm)
-    assert v == {(0, 1): 1, (1, 2): 4, (0, 0): 0, (2, 1): 4, (1, 1): 3,
-                 (2, 0): 2, (2, 2): 5, (1, 0): 1, (0, 2): 2}
+    assert v == {
+        (0, 1): 1,
+        (1, 2): 4,
+        (0, 0): 0,
+        (2, 1): 4,
+        (1, 1): 3,
+        (2, 0): 2,
+        (2, 2): 5,
+        (1, 0): 1,
+        (0, 2): 2,
+    }
     assert s == [(0, 0), (0, 1), (0, 2), (1, 1), (1, 2), (2, 2)]
 
 
 def test_index_flattening():
     from ufl.utils.indexflattening import flatten_multiindex, shape_to_strides, unflatten_index
 
     # Scalar shape
@@ -139,19 +151,20 @@
         c = (k,)
         # get flat index:
         i = flatten_multiindex(c, shape_to_strides(mixed_shape))
         # remove offset:
         i -= 0
         # map back to tensor component:
         c2 = unflatten_index(i, shape_to_strides(ts))
-        assert (k//2, k % 2) == c2
+        assert (k // 2, k % 2) == c2
 
 
 def test_stackdict():
     from ufl.utils.stacks import StackDict
+
     d = StackDict(a=1)
     assert d["a"] == 1
     d.push("a", 2)
     assert d["a"] == 2
     d.push("a", 3)
     d.push("b", 9)
     assert d["a"] == 3
```

### Comparing `fenics-ufl-2023.2.0/ufl/action.py` & `fenics_ufl-2024.1.0.post0/ufl/action.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Nacime Bouziani, 2021-2022.
 
-from ufl.form import BaseForm, FormSum, Form, ZeroBaseForm
-from ufl.core.ufl_type import ufl_type
+from itertools import chain
+
 from ufl.algebra import Sum
-from ufl.constantvalue import Zero
 from ufl.argument import Argument, Coargument
 from ufl.coefficient import BaseCoefficient, Coefficient, Cofunction
-from ufl.differentiation import CoefficientDerivative
+from ufl.constantvalue import Zero
 from ufl.core.base_form_operator import BaseFormOperator
+from ufl.core.ufl_type import ufl_type
+from ufl.differentiation import CoefficientDerivative
+from ufl.form import BaseForm, Form, FormSum, ZeroBaseForm
 from ufl.matrix import Matrix
 
 # --- The Action class represents the action of a numerical object that needs
 #     to be computed at assembly time ---
 
 
 @ufl_type()
@@ -39,15 +41,16 @@
         "_left",
         "_right",
         "ufl_operands",
         "_repr",
         "_arguments",
         "_coefficients",
         "_domains",
-        "_hash")
+        "_hash",
+    )
 
     def __new__(cls, *args, **kw):
         """Create a new Action."""
         left, right = args
 
         # Check trivial case
         if left == 0 or right == 0:
@@ -65,20 +68,18 @@
         if isinstance(left, (Coargument, Argument)):
             return right
         if isinstance(right, (Coargument, Argument)):
             return left
 
         if isinstance(left, (FormSum, Sum)):
             # Action distributes over sums on the LHS
-            return FormSum(*[(Action(component, right), 1)
-                             for component in left.ufl_operands])
+            return FormSum(*[(Action(component, right), 1) for component in left.ufl_operands])
         if isinstance(right, (FormSum, Sum)):
             # Action also distributes over sums on the RHS
-            return FormSum(*[(Action(left, component), 1)
-                             for component in right.ufl_operands])
+            return FormSum(*[(Action(left, component), 1) for component in right.ufl_operands])
 
         return super(Action, cls).__new__(cls)
 
     def __init__(self, left, right):
         """Initialise."""
         BaseForm.__init__(self)
 
@@ -92,16 +93,15 @@
 
         self._repr = "Action(%s, %s)" % (repr(self._left), repr(self._right))
         self._hash = None
 
     def ufl_function_spaces(self):
         """Get the tuple of function spaces of the underlying form."""
         if isinstance(self._right, Form):
-            return self._left.ufl_function_spaces()[:-1] \
-                + self._right.ufl_function_spaces()[1:]
+            return self._left.ufl_function_spaces()[:-1] + self._right.ufl_function_spaces()[1:]
         elif isinstance(self._right, Coefficient):
             return self._left.ufl_function_spaces()[:-1]
 
     def left(self):
         """Get left."""
         return self._left
 
@@ -116,16 +116,19 @@
         Argument of the right operand are consumed by the action.
         """
         self._arguments, self._coefficients = _get_action_form_arguments(self._left, self._right)
 
     def _analyze_domains(self):
         """Analyze which domains can be found in Action."""
         from ufl.domain import join_domains
-        # Collect unique domains
-        self._domains = join_domains([e.ufl_domain() for e in self.ufl_operands])
+
+        # Collect domains
+        self._domains = join_domains(
+            chain.from_iterable(e.ufl_domains() for e in self.ufl_operands)
+        )
 
     def equals(self, other):
         """Check if two Actions are equal."""
         if type(other) is not Action:
             return False
         if self is other:
             return True
@@ -151,45 +154,48 @@
 def _check_function_spaces(left, right):
     """Check if the function spaces of left and right match."""
     if isinstance(right, CoefficientDerivative):
         # Action differentiation pushes differentiation through
         # right as a consequence of Leibniz formula.
         right, *_ = right.ufl_operands
 
-    # `left` can also be a Coefficient in V (= V**), e.g. `action(Coefficient(V), Cofunction(V.dual()))`.
+    # `left` can also be a Coefficient in V (= V**), e.g.
+    # `action(Coefficient(V), Cofunction(V.dual()))`.
     left_arg = left.arguments()[-1] if not isinstance(left, Coefficient) else left
     if isinstance(right, (Form, Action, Matrix, ZeroBaseForm)):
         if left_arg.ufl_function_space().dual() != right.arguments()[0].ufl_function_space():
             raise TypeError("Incompatible function spaces in Action")
     elif isinstance(right, (Coefficient, Cofunction, Argument, BaseFormOperator)):
         if left_arg.ufl_function_space() != right.ufl_function_space():
-
             raise TypeError("Incompatible function spaces in Action")
     # `Zero` doesn't contain any information about the function space.
-    # -> Not a problem since Action will get simplified with a `ZeroBaseForm`
-    #    which won't take into account the arguments on the right because of argument contraction.
+    # -> Not a problem since Action will get simplified with a
+    #    `ZeroBaseForm` which won't take into account the arguments on
+    #    the right because of argument contraction.
     # This occurs for:
     # `derivative(Action(A, B), u)` with B is an `Expr` such that dB/du == 0
     # -> `derivative(B, u)` becomes `Zero` when expanding derivatives since B is an Expr.
     elif not isinstance(right, Zero):
         raise TypeError("Incompatible argument in Action: %s" % type(right))
 
 
 def _get_action_form_arguments(left, right):
     """Perform argument contraction to work out the arguments of Action."""
     coefficients = ()
-    # `left` can also be a Coefficient in V (= V**), e.g. `action(Coefficient(V), Cofunction(V.dual()))`.
+    # `left` can also be a Coefficient in V (= V**), e.g.
+    # `action(Coefficient(V), Cofunction(V.dual()))`.
     left_args = left.arguments()[:-1] if not isinstance(left, Coefficient) else ()
     if isinstance(right, BaseForm):
         arguments = left_args + right.arguments()[1:]
         coefficients += right.coefficients()
     elif isinstance(right, CoefficientDerivative):
         # Action differentiation pushes differentiation through
         # right as a consequence of Leibniz formula.
         from ufl.algorithms.analysis import extract_arguments_and_coefficients
+
         right_args, right_coeffs = extract_arguments_and_coefficients(right)
         arguments = left_args + tuple(right_args)
         coefficients += tuple(right_coeffs)
     elif isinstance(right, (BaseCoefficient, Zero)):
         arguments = left_args
         # When right is ufl.Zero, Action gets simplified so updating
         # coefficients here doesn't matter
```

### Comparing `fenics-ufl-2023.2.0/ufl/adjoint.py` & `fenics_ufl-2024.1.0.post0/ufl/adjoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Nacime Bouziani, 2021-2022.
 
-from ufl.form import BaseForm, FormSum, ZeroBaseForm
 from ufl.argument import Coargument
 from ufl.core.ufl_type import ufl_type
+from ufl.form import BaseForm, FormSum, ZeroBaseForm
+
 # --- The Adjoint class represents the adjoint of a numerical object that
 #     needs to be computed at assembly time ---
 
 
 @ufl_type()
 class Adjoint(BaseForm):
     """UFL base form type: represents the adjoint of an object.
@@ -27,37 +28,40 @@
     __slots__ = (
         "_form",
         "_repr",
         "_arguments",
         "_coefficients",
         "_domains",
         "ufl_operands",
-        "_hash")
+        "_hash",
+    )
 
     def __new__(cls, *args, **kw):
         """Create a new Adjoint."""
         form = args[0]
         # Check trivial case: This is not a ufl.Zero but a ZeroBaseForm!
         if form == 0:
             # Swap the arguments
             return ZeroBaseForm(form.arguments()[::-1])
 
         if isinstance(form, Adjoint):
             return form._form
         elif isinstance(form, FormSum):
             # Adjoint distributes over sums
-            return FormSum(*[(Adjoint(component), 1)
-                             for component in form.components()])
+            return FormSum(*[(Adjoint(component), 1) for component in form.components()])
         elif isinstance(form, Coargument):
-            # The adjoint of a coargument `c: V* -> V*` is the identity matrix mapping from V to V (i.e. V x V* -> R).
-            # Equivalently, the adjoint of `c` is its first argument, which is a ufl.Argument defined on the
-            # primal space of `c`.
+            # The adjoint of a coargument `c: V* -> V*` is the identity
+            # matrix mapping from V to V (i.e. V x V* -> R).
+            # Equivalently, the adjoint of `c` is its first argument,
+            # which is a ufl.Argument defined on the primal space of
+            # `c`.
             primal_arg, _ = form.arguments()
-            # Returning the primal argument avoids explicit argument reconstruction, making it
-            # a robust strategy for handling subclasses of `ufl.Coargument`.
+            # Returning the primal argument avoids explicit argument
+            # reconstruction, making it a robust strategy for handling
+            # subclasses of `ufl.Coargument`.
             return primal_arg
 
         return super(Adjoint, cls).__new__(cls)
 
     def __init__(self, form):
         """Initialise."""
         BaseForm.__init__(self)
@@ -83,25 +87,27 @@
         """The arguments of adjoint are the reverse of the form arguments."""
         self._arguments = self._form.arguments()[::-1]
         self._coefficients = self._form.coefficients()
 
     def _analyze_domains(self):
         """Analyze which domains can be found in Adjoint."""
         from ufl.domain import join_domains
+
         # Collect unique domains
         self._domains = join_domains([e.ufl_domain() for e in self.ufl_operands])
 
     def equals(self, other):
         """Check if two Adjoints are equal."""
         if type(other) is not Adjoint:
             return False
         if self is other:
             return True
-        # Make sure we are returning a boolean as the equality can result in a `ufl.Equation`
-        # if the underlying objects are `ufl.BaseForm`.
+        # Make sure we are returning a boolean as the equality can
+        # result in a `ufl.Equation` if the underlying objects are
+        # `ufl.BaseForm`.
         return bool(self._form == other._form)
 
     def __str__(self):
         """Format as a string."""
         return f"Adjoint({self._form})"
 
     def __repr__(self):
```

### Comparing `fenics-ufl-2023.2.0/ufl/algebra.py` & `fenics_ufl-2024.1.0.post0/ufl/algebra.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,33 @@
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Anders Logg, 2008
 
-from ufl.core.ufl_type import ufl_type
+from ufl.checks import is_true_ufl_scalar, is_ufl_scalar
+from ufl.constantvalue import ComplexValue, IntValue, ScalarValue, Zero, as_ufl, zero
 from ufl.core.expr import ufl_err_str
 from ufl.core.operator import Operator
-from ufl.constantvalue import Zero, zero, ScalarValue, IntValue, ComplexValue, as_ufl
-from ufl.checks import is_ufl_scalar, is_true_ufl_scalar
+from ufl.core.ufl_type import ufl_type
 from ufl.index_combination_utils import merge_unique_indices
-from ufl.sorting import sorted_expr
 from ufl.precedence import parstr
+from ufl.sorting import sorted_expr
 
 # --- Algebraic operators ---
 
 
-@ufl_type(num_ops=2,
-          inherit_shape_from_operand=0, inherit_indices_from_operand=0,
-          binop="__add__", rbinop="__radd__")
+@ufl_type(
+    num_ops=2,
+    inherit_shape_from_operand=0,
+    inherit_indices_from_operand=0,
+    binop="__add__",
+    rbinop="__radd__",
+)
 class Sum(Operator):
     """Sum."""
 
     __slots__ = ()
 
     def __new__(cls, a, b):
         """Create a new Sum."""
@@ -83,48 +87,50 @@
 
     def __init__(self, a, b):
         """Initialise."""
         Operator.__init__(self)
 
     def evaluate(self, x, mapping, component, index_values):
         """Evaluate."""
-        return sum(o.evaluate(x, mapping, component,
-                              index_values) for o in self.ufl_operands)
+        return sum(o.evaluate(x, mapping, component, index_values) for o in self.ufl_operands)
 
     def __str__(self):
         """Format as a string."""
         return " + ".join([parstr(o, self) for o in self.ufl_operands])
 
 
-@ufl_type(num_ops=2,
-          binop="__mul__", rbinop="__rmul__")
+@ufl_type(num_ops=2, binop="__mul__", rbinop="__rmul__")
 class Product(Operator):
     """The product of two or more UFL objects."""
 
     __slots__ = ("ufl_free_indices", "ufl_index_dimensions")
 
     def __new__(cls, a, b):
         """Create a new product."""
         # Conversion
         a = as_ufl(a)
         b = as_ufl(b)
 
         # Type checking
         # Make sure everything is scalar
         if a.ufl_shape or b.ufl_shape:
-            raise ValueError("Product can only represent products of scalars, "
-                             f"got\n    {ufl_err_str(a)}\nand\n    {ufl_err_str(b)}")
+            raise ValueError(
+                "Product can only represent products of scalars, "
+                f"got\n    {ufl_err_str(a)}\nand\n    {ufl_err_str(b)}"
+            )
 
         # Simplification
         if isinstance(a, Zero) or isinstance(b, Zero):
             # Got any zeros? Return zero.
-            fi, fid = merge_unique_indices(a.ufl_free_indices,
-                                           a.ufl_index_dimensions,
-                                           b.ufl_free_indices,
-                                           b.ufl_index_dimensions)
+            fi, fid = merge_unique_indices(
+                a.ufl_free_indices,
+                a.ufl_index_dimensions,
+                b.ufl_free_indices,
+                b.ufl_index_dimensions,
+            )
             return Zero((), fi, fid)
         sa = isinstance(a, ScalarValue)
         sb = isinstance(b, ScalarValue)
         if sa and sb:  # const * const = const
             # FIXME: Handle free indices like with zero? I think
             # IntValue may be index annotated now?
             return as_ufl(a._value * b._value)
@@ -150,18 +156,17 @@
         return self
 
     def _init(self, a, b):
         """Constructor, called by __new__ with already checked arguments."""
         self.ufl_operands = (a, b)
 
         # Extract indices
-        fi, fid = merge_unique_indices(a.ufl_free_indices,
-                                       a.ufl_index_dimensions,
-                                       b.ufl_free_indices,
-                                       b.ufl_index_dimensions)
+        fi, fid = merge_unique_indices(
+            a.ufl_free_indices, a.ufl_index_dimensions, b.ufl_free_indices, b.ufl_index_dimensions
+        )
         self.ufl_free_indices = fi
         self.ufl_index_dimensions = fid
 
     def __init__(self, a, b):
         """Initialise."""
         Operator.__init__(self)
 
@@ -169,32 +174,32 @@
 
     def evaluate(self, x, mapping, component, index_values):
         """Evaluate."""
         ops = self.ufl_operands
         sh = self.ufl_shape
         if sh:
             if sh != ops[-1].ufl_shape:
-                raise ValueError("Expecting nonscalar product operand to be the last by convention.")
+                raise ValueError(
+                    "Expecting nonscalar product operand to be the last by convention."
+                )
             tmp = ops[-1].evaluate(x, mapping, component, index_values)
             ops = ops[:-1]
         else:
             tmp = 1
         for o in ops:
             tmp *= o.evaluate(x, mapping, (), index_values)
         return tmp
 
     def __str__(self):
         """Format as a string."""
         a, b = self.ufl_operands
         return " * ".join((parstr(a, self), parstr(b, self)))
 
 
-@ufl_type(num_ops=2,
-          inherit_indices_from_operand=0,
-          binop="__div__", rbinop="__rdiv__")
+@ufl_type(num_ops=2, inherit_indices_from_operand=0, binop="__div__", rbinop="__rdiv__")
 class Division(Operator):
     """Division."""
 
     __slots__ = ()
 
     def __new__(cls, a, b):
         """Create a new Division."""
@@ -256,17 +261,15 @@
         return e
 
     def __str__(self):
         """Format as a string."""
         return f"{parstr(self.ufl_operands[0], self)} / {parstr(self.ufl_operands[1], self)}"
 
 
-@ufl_type(num_ops=2,
-          inherit_indices_from_operand=0,
-          binop="__pow__", rbinop="__rpow__")
+@ufl_type(num_ops=2, inherit_indices_from_operand=0, binop="__pow__", rbinop="__rpow__")
 class Power(Operator):
     """Power."""
 
     __slots__ = ()
 
     def __new__(cls, a, b):
         """Create new Power."""
@@ -278,15 +281,15 @@
         if not is_true_ufl_scalar(a):
             raise ValueError(f"Cannot take the power of a non-scalar expression {ufl_err_str(a)}.")
         if not is_true_ufl_scalar(b):
             raise ValueError(f"Cannot raise an expression to a non-scalar power {ufl_err_str(b)}.")
 
         # Simplification
         if isinstance(a, ScalarValue) and isinstance(b, ScalarValue):
-            return as_ufl(a._value ** b._value)
+            return as_ufl(a._value**b._value)
         if isinstance(b, Zero):
             return IntValue(1)
         if isinstance(a, Zero) and isinstance(b, ScalarValue):
             if isinstance(b, ComplexValue):
                 raise ValueError("Cannot raise zero to a complex power.")
             bf = float(b)
             if bf < 0:
@@ -320,17 +323,15 @@
 
     def __str__(self):
         """Format as a string."""
         a, b = self.ufl_operands
         return f"{parstr(a, self)} ** {parstr(b, self)}"
 
 
-@ufl_type(num_ops=1,
-          inherit_shape_from_operand=0, inherit_indices_from_operand=0,
-          unop="__abs__")
+@ufl_type(num_ops=1, inherit_shape_from_operand=0, inherit_indices_from_operand=0, unop="__abs__")
 class Abs(Operator):
     """Absolute value."""
 
     __slots__ = ()
 
     def __new__(cls, a):
         """Create a new Abs."""
@@ -353,20 +354,19 @@
     def evaluate(self, x, mapping, component, index_values):
         """Evaluate."""
         a = self.ufl_operands[0].evaluate(x, mapping, component, index_values)
         return abs(a)
 
     def __str__(self):
         """Format as a string."""
-        a, = self.ufl_operands
+        (a,) = self.ufl_operands
         return f"|{parstr(a, self)}|"
 
 
-@ufl_type(num_ops=1,
-          inherit_shape_from_operand=0, inherit_indices_from_operand=0)
+@ufl_type(num_ops=1, inherit_shape_from_operand=0, inherit_indices_from_operand=0)
 class Conj(Operator):
     """Complex conjugate."""
 
     __slots__ = ()
 
     def __new__(cls, a):
         """Creatr a new Conj."""
@@ -389,20 +389,19 @@
     def evaluate(self, x, mapping, component, index_values):
         """Evaluate."""
         a = self.ufl_operands[0].evaluate(x, mapping, component, index_values)
         return a.conjugate()
 
     def __str__(self):
         """Format as a string."""
-        a, = self.ufl_operands
+        (a,) = self.ufl_operands
         return f"conj({parstr(a, self)})"
 
 
-@ufl_type(num_ops=1,
-          inherit_shape_from_operand=0, inherit_indices_from_operand=0)
+@ufl_type(num_ops=1, inherit_shape_from_operand=0, inherit_indices_from_operand=0)
 class Real(Operator):
     """Real part."""
 
     __slots__ = ()
 
     def __new__(cls, a):
         """Create a new Real."""
@@ -427,20 +426,19 @@
     def evaluate(self, x, mapping, component, index_values):
         """Evaluate."""
         a = self.ufl_operands[0].evaluate(x, mapping, component, index_values)
         return a.real
 
     def __str__(self):
         """Format as a string."""
-        a, = self.ufl_operands
+        (a,) = self.ufl_operands
         return f"Re[{parstr(a, self)}]"
 
 
-@ufl_type(num_ops=1,
-          inherit_shape_from_operand=0, inherit_indices_from_operand=0)
+@ufl_type(num_ops=1, inherit_shape_from_operand=0, inherit_indices_from_operand=0)
 class Imag(Operator):
     """Imaginary part."""
 
     __slots__ = ()
 
     def __new__(cls, a):
         """Create a new Imag."""
@@ -463,9 +461,9 @@
     def evaluate(self, x, mapping, component, index_values):
         """Evaluate."""
         a = self.ufl_operands[0].evaluate(x, mapping, component, index_values)
         return a.imag
 
     def __str__(self):
         """Format as a string."""
-        a, = self.ufl_operands
+        (a,) = self.ufl_operands
         return f"Im[{parstr(a, self)}]"
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/ad.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/ad.py`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/analysis.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-"""Utility algorithms for inspection of and information extraction from UFL objects in various ways."""
+"""Utility algorithms for inspection of and information extraction from UFL objects."""
 
 # Copyright (C) 2008-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Anders Logg, 2009-2010.
 # Modified by Johan Hake, 2010.
 
 from itertools import chain
 
-from ufl.utils.sorting import sorted_by_count, topological_sorting
-
-from ufl.core.terminal import Terminal
-from ufl.core.base_form_operator import BaseFormOperator
+from ufl.algorithms.traversal import iter_expressions
 from ufl.argument import BaseArgument, Coargument
 from ufl.coefficient import BaseCoefficient
 from ufl.constant import Constant
+from ufl.core.base_form_operator import BaseFormOperator
+from ufl.core.terminal import Terminal
+from ufl.corealg.traversal import traverse_unique_terminals, unique_pre_traversal
 from ufl.form import BaseForm, Form
-from ufl.algorithms.traversal import iter_expressions
-from ufl.corealg.traversal import unique_pre_traversal, traverse_unique_terminals
-
+from ufl.utils.sorting import sorted_by_count, topological_sorting
 
 # TODO: Some of these can possibly be optimised by implementing
 # inlined stack based traversal algorithms
 
+
 def _sorted_by_number_and_part(seq):
     """Sort items by number and part."""
     return sorted(seq, key=lambda x: (x.number(), x.part()))
 
 
 def unique_tuple(objects):
     """Return tuple of unique objects, preserving initial ordering."""
@@ -40,14 +39,15 @@
             handled.add(obj)
             unique_objects.append(obj)
     return tuple(unique_objects)
 
 
 # --- Utilities to extract information from an expression ---
 
+
 def extract_type(a, ufl_types):
     """Build a set of all objects found in a whose class is in ufl_types.
 
     Args:
         a: A BaseForm, Integral or Expr
         ufl_types: A list of UFL types
 
@@ -73,41 +73,51 @@
         coeff_types = tuple(t for t in ufl_types if issubclass(t, BaseCoefficient))
         if coeff_types:
             objects.update([e for e in a.coefficients() if isinstance(e, coeff_types)])
         return objects
 
     if all(issubclass(t, Terminal) for t in ufl_types):
         # Optimization
-        objects = set(o for e in iter_expressions(a)
-                      for o in traverse_unique_terminals(e)
-                      if any(isinstance(o, t) for t in ufl_types))
+        objects = set(
+            o
+            for e in iter_expressions(a)
+            for o in traverse_unique_terminals(e)
+            if any(isinstance(o, t) for t in ufl_types)
+        )
     else:
-        objects = set(o for e in iter_expressions(a)
-                      for o in unique_pre_traversal(e)
-                      if any(isinstance(o, t) for t in ufl_types))
+        objects = set(
+            o
+            for e in iter_expressions(a)
+            for o in unique_pre_traversal(e)
+            if any(isinstance(o, t) for t in ufl_types)
+        )
 
-    # Need to extract objects contained in base form operators whose type is in ufl_types
+    # Need to extract objects contained in base form operators whose
+    # type is in ufl_types
     base_form_ops = set(e for e in objects if isinstance(e, BaseFormOperator))
     ufl_types_no_args = tuple(t for t in ufl_types if not issubclass(t, BaseArgument))
     base_form_objects = ()
     for o in base_form_ops:
         # This accounts for having BaseFormOperator in Forms: if N is a BaseFormOperator
         # `N(u; v*) * v * dx` <=> `action(v1 * v * dx, N(...; v*))`
         # where `v`, `v1` are `Argument`s and `v*` a `Coargument`.
         for ai in tuple(arg for arg in o.argument_slots(isinstance(a, Form))):
-            # Extracting BaseArguments of an object of which a Coargument is an argument,
-            # then we just return the dual argument of the Coargument and not its primal argument.
+            # Extracting BaseArguments of an object of which a
+            # Coargument is an argument, then we just return the dual
+            # argument of the Coargument and not its primal argument.
             if isinstance(ai, Coargument):
                 new_types = tuple(Coargument if t is BaseArgument else t for t in ufl_types)
                 base_form_objects += tuple(extract_type(ai, new_types))
             else:
                 base_form_objects += tuple(extract_type(ai, ufl_types))
-        # Look for BaseArguments in BaseFormOperator's argument slots only since that's where they are by definition.
-        # Don't look into operands, which is convenient for external operator composition, e.g. N1(N2; v*)
-        # where N2 is seen as an operator and not a form.
+        # Look for BaseArguments in BaseFormOperator's argument slots
+        # only since that's where they are by definition. Don't look
+        # into operands, which is convenient for external operator
+        # composition, e.g. N1(N2; v*) where N2 is seen as an operator
+        # and not a form.
         slots = o.ufl_operands
         for ai in slots:
             base_form_objects += tuple(extract_type(ai, ufl_types_no_args))
     objects.update(base_form_objects)
 
     # `Remove BaseFormOperator` objects if there were initially not in `ufl_types`
     if remove_base_form_ops:
@@ -204,22 +214,24 @@
 
     # Build number,part: instance mappings, should be one to one
     bfnp = dict((f, (f.number(), f.part())) for f in arguments)
     if len(bfnp) != len(set(bfnp.values())):
         raise ValueError(
             "Found different Arguments with same number and part.\n"
             "Did you combine test or trial functions from different spaces?\n"
-            "The Arguments found are:\n" + "\n".join(f"  {a}" for a in arguments))
+            "The Arguments found are:\n" + "\n".join(f"  {a}" for a in arguments)
+        )
 
     # Build count: instance mappings, should be one to one
     fcounts = dict((f, f.count()) for f in coefficients)
     if len(fcounts) != len(set(fcounts.values())):
         raise ValueError(
             "Found different coefficients with same counts.\n"
-            "The arguments found are:\n" + "\n".join(f"  {c}" for c in coefficients))
+            "The arguments found are:\n" + "\n".join(f"  {c}" for c in coefficients)
+        )
 
     # Passed checks, so we can safely sort the instances by count
     arguments = _sorted_by_number_and_part(arguments)
     coefficients = sorted_by_count(coefficients)
 
     return arguments, coefficients
 
@@ -233,15 +245,15 @@
 def extract_unique_elements(form):
     """Build sorted tuple of all unique elements used in form."""
     return unique_tuple(extract_elements(form))
 
 
 def extract_sub_elements(elements):
     """Build sorted tuple of all sub elements (including parent element)."""
-    sub_elements = tuple(chain(*[e.sub_elements() for e in elements]))
+    sub_elements = tuple(chain(*[e.sub_elements for e in elements]))
     if not sub_elements:
         return tuple(elements)
     return tuple(elements) + extract_sub_elements(sub_elements)
 
 
 def sort_elements(elements):
     """Sort elements.
@@ -249,20 +261,20 @@
     A sort is performed so that any sub elements appear before the
     corresponding mixed elements. This is useful when sub elements
     need to be defined before the corresponding mixed elements.
 
     The ordering is based on sorting a directed acyclic graph.
     """
     # Set nodes
-    nodes = sorted(elements)
+    nodes = list(elements)
 
     # Set edges
     edges = dict((node, []) for node in nodes)
     for element in elements:
-        for sub_element in element.sub_elements():
+        for sub_element in element.sub_elements:
             edges[element].append(sub_element)
 
     # Sort graph
     sorted_elements = topological_sorting(nodes, edges)
 
     # Reverse list of elements
     sorted_elements.reverse()
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/apply_algebra_lowering.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/apply_algebra_lowering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-"""Algorithm for expanding compound expressions into equivalent representations using basic operators."""
+"""Algorithm for expanding compound expressions."""
 
 # Copyright (C) 2008-2016 Martin Sandve Alnæs and Anders Logg
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Anders Logg, 2009-2010
 
-from ufl.classes import Product, Grad, Conj
-from ufl.core.multiindex import indices, Index
-from ufl.tensors import as_tensor, as_matrix, as_vector
-
-from ufl.compound_expressions import deviatoric_expr, determinant_expr, cofactor_expr, inverse_expr
-
-from ufl.corealg.multifunction import MultiFunction
 from ufl.algorithms.map_integrands import map_integrand_dags
+from ufl.classes import Conj, Grad, Product
+from ufl.compound_expressions import cofactor_expr, determinant_expr, deviatoric_expr, inverse_expr
+from ufl.core.multiindex import Index, indices
+from ufl.corealg.multifunction import MultiFunction
+from ufl.tensors import as_matrix, as_tensor, as_vector
 
 
 class LowerCompoundAlgebra(MultiFunction):
     """Expands high level compound operators to equivalent representations using basic operators."""
 
     def __init__(self):
         """Initialize."""
@@ -51,16 +49,18 @@
     def sym(self, o, A):
         """Lower a sym."""
         i, j = indices(2)
         return as_matrix((A[i, j] + A[j, i]) / 2, (i, j))
 
     def cross(self, o, a, b):
         """Lower a cross."""
+
         def c(i, j):
             return Product(a[i], b[j]) - Product(a[j], b[i])
+
         return as_vector((c(1, 2), c(2, 0), c(0, 1)))
 
     def perp(self, o, a):
         """Lower a perp."""
         return as_vector([-a[1], a[0]])
 
     def dot(self, o, a, b):
@@ -123,20 +123,22 @@
         else:
             j = Index()
             ii = tuple(indices(len(sh)))
             return as_tensor(a[ii].dx(j), (j,) + ii)
 
     def curl(self, o, a):
         """Lower a curl."""
+
         # o = curl a = "[a.dx(1), -a.dx(0)]"            if a.ufl_shape == ()
         # o = curl a = "cross(nabla, (a0, a1, 0))[2]" if a.ufl_shape == (2,)
         # o = curl a = "cross(nabla, a)"              if a.ufl_shape == (3,)
         def c(i, j):
             """A component of curl."""
             return a[j].dx(i) - a[i].dx(j)
+
         sh = a.ufl_shape
         if sh == ():
             return as_vector((a.dx(1), -a.dx(0)))
         if sh == (2,):
             return c(0, 1)
         if sh == (3,):
             return as_vector((c(1, 2), c(2, 0), c(0, 1)))
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/apply_derivatives.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/apply_derivatives.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,84 @@
-"""This module contains the apply_derivatives algorithm which computes the derivatives of a form of expression."""
+"""Apply derivatives algorithm which computes the derivatives of a form of expression."""
 
 # Copyright (C) 2008-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
 import warnings
 from collections import defaultdict
 from math import pi
 
+from ufl.action import Action
 from ufl.algorithms.analysis import extract_arguments
 from ufl.algorithms.map_integrands import map_integrand_dags
 from ufl.algorithms.replace_derivative_nodes import replace_derivative_nodes
+from ufl.argument import BaseArgument
 from ufl.checks import is_cellwise_constant
-from ufl.classes import (Coefficient, ComponentTensor, Conj, ConstantValue,
-                         ExprList, ExprMapping, FloatValue, FormArgument, Grad,
-                         Identity, Imag, Indexed, IndexSum, JacobianInverse,
-                         ListTensor, Product, Real, ReferenceGrad,
-                         ReferenceValue, SpatialCoordinate, Sum, Variable,
-                         Zero)
+from ufl.classes import (
+    Coefficient,
+    ComponentTensor,
+    Conj,
+    ConstantValue,
+    ExprList,
+    ExprMapping,
+    FloatValue,
+    FormArgument,
+    Grad,
+    Identity,
+    Imag,
+    Indexed,
+    IndexSum,
+    JacobianInverse,
+    ListTensor,
+    Product,
+    Real,
+    ReferenceGrad,
+    ReferenceValue,
+    SpatialCoordinate,
+    Sum,
+    Variable,
+    Zero,
+)
 from ufl.constantvalue import is_true_ufl_scalar, is_ufl_scalar
+from ufl.core.base_form_operator import BaseFormOperator
 from ufl.core.expr import ufl_err_str
 from ufl.core.multiindex import FixedIndex, MultiIndex, indices
 from ufl.core.terminal import Terminal
 from ufl.corealg.map_dag import map_expr_dag
 from ufl.corealg.multifunction import MultiFunction
-from ufl.differentiation import CoordinateDerivative, BaseFormCoordinateDerivative, BaseFormOperatorDerivative
+from ufl.differentiation import (
+    BaseFormCoordinateDerivative,
+    BaseFormOperatorDerivative,
+    CoordinateDerivative,
+)
 from ufl.domain import extract_unique_domain
-from ufl.operators import (bessel_I, bessel_J, bessel_K, bessel_Y, cell_avg,
-                           conditional, cos, cosh, exp, facet_avg, ln, sign,
-                           sin, sinh, sqrt)
-from ufl.tensors import (as_scalar, as_scalars, as_tensor, unit_indexed_tensor,
-                         unwrap_list_tensor)
-
-from ufl.argument import BaseArgument
-from ufl.action import Action
 from ufl.form import Form, ZeroBaseForm
-from ufl.core.base_form_operator import BaseFormOperator
+from ufl.operators import (
+    bessel_I,
+    bessel_J,
+    bessel_K,
+    bessel_Y,
+    cell_avg,
+    conditional,
+    cos,
+    cosh,
+    exp,
+    facet_avg,
+    ln,
+    sign,
+    sin,
+    sinh,
+    sqrt,
+)
+from ufl.pullback import CustomPullback, PhysicalPullback
+from ufl.tensors import as_scalar, as_scalars, as_tensor, unit_indexed_tensor, unwrap_list_tensor
+
 # TODO: Add more rulesets?
 # - DivRuleset
 # - CurlRuleset
 # - ReferenceGradRuleset
 # - ReferenceDivRuleset
 
 
@@ -53,49 +90,58 @@
         MultiFunction.__init__(self)
         self._var_shape = var_shape
 
     # --- Error checking for missing handlers and unexpected types
 
     def expr(self, o):
         """Raise error."""
-        raise ValueError(f"Missing differentiation handler for type {o._ufl_class_.__name__}. "
-                         "Have you added a new type?")
+        raise ValueError(
+            f"Missing differentiation handler for type {o._ufl_class_.__name__}. "
+            "Have you added a new type?"
+        )
 
     def unexpected(self, o):
         """Raise error about unexpected type."""
         raise ValueError(f"Unexpected type {o._ufl_class_.__name__} in AD rules.")
 
     def override(self, o):
         """Raise error about overriding."""
-        raise ValueError(f"Type {o._ufl_class_.__name__} must be overridden in specialized AD rule set.")
+        raise ValueError(
+            f"Type {o._ufl_class_.__name__} must be overridden in specialized AD rule set."
+        )
 
     def derivative(self, o):
         """Raise error."""
-        raise ValueError(f"Unhandled derivative type {o._ufl_class_.__name__}, nested differentiation has failed.")
+        raise ValueError(
+            f"Unhandled derivative type {o._ufl_class_.__name__}, "
+            "nested differentiation has failed."
+        )
 
     # --- Some types just don't have any derivative, this is just to
     # --- make algorithm structure generic
 
     def non_differentiable_terminal(self, o):
         """Return the non-differentiated object.
 
-        Labels and indices are not differentiable: it's convenient to return the non-differentiated object.
+        Labels and indices are not differentiable: it's convenient to
+        return the non-differentiated object.
         """
         return o
+
     label = non_differentiable_terminal
     multi_index = non_differentiable_terminal
 
     # --- Helper functions for creating zeros with the right shapes
 
     def independent_terminal(self, o):
-        """Return a zero with the right shape for terminals independent of differentiation variable."""
+        """A zero with correct shape for terminals independent of diff. variable."""
         return Zero(o.ufl_shape + self._var_shape)
 
     def independent_operator(self, o):
-        """Return a zero with the right shape and indices for operators independent of differentiation variable."""
+        """A zero with correct shape and indices for operators independent of diff. variable."""
         return Zero(o.ufl_shape + self._var_shape, o.ufl_free_indices, o.ufl_index_dimensions)
 
     # --- All derivatives need to define grad and averaging
 
     grad = override
     cell_avg = override
     facet_avg = override
@@ -276,19 +322,21 @@
         # do/df  = g * f**(g-1) = g / f * o
         # do/dg  = ln(f) * f**g = ln(f) * o
         # do/df * df + do/dg * dg = o * (g / f * df + ln(f) * dg)
 
         if isinstance(gp, Zero):
             # This probably produces better results for the common
             # case of f**constant
-            op = fp * g * f**(g - 1)
+            op = fp * g * f ** (g - 1)
         else:
             # Note: This produces expressions like (1/w)*w**5 instead of w**4
             # op = o * (fp * g / f + gp * ln(f)) # This reuses o
-            op = f**(g - 1) * (g * fp + f * ln(f) * gp)  # This gives better accuracy in dolfin integration test
+            op = f ** (g - 1) * (
+                g * fp + f * ln(f) * gp
+            )  # This gives better accuracy in dolfin integration test
 
         # Example: d/dx[x**(x**3)]:
         # f = x
         # g = x**3
         # df = 1
         # dg = 3*x**2
         # op1 = o * (fp * g / f + gp * ln(f))
@@ -296,15 +344,15 @@
         # op2 = f**(g-1) * (g*fp + f*ln(f)*gp)
         #     = x**(x**3-1) * (x**3 + x*3*x**2*ln(x))
 
         return op
 
     def abs(self, o, df):
         """Differentiate an abs."""
-        f, = o.ufl_operands
+        (f,) = o.ufl_operands
         # return conditional(eq(f, 0), 0, Product(sign(f), df)) abs is
         # not complex differentiable, so we workaround the case of a
         # real F in complex mode by defensively casting to real inside
         # the sign.
         return sign(Real(f)) * df
 
     # --- Complex algebra
@@ -323,135 +371,144 @@
 
     # --- Mathfunctions
 
     def math_function(self, o, df):
         """Differentiate a math_function."""
         # FIXME: Introduce a UserOperator type instead of this hack
         # and define user derivative() function properly
-        if hasattr(o, 'derivative'):
-            f, = o.ufl_operands
+        if hasattr(o, "derivative"):
+            (f,) = o.ufl_operands
             return df * o.derivative()
         raise ValueError("Unknown math function.")
 
     def sqrt(self, o, fp):
         """Differentiate a sqrt."""
         return fp / (2 * o)
 
     def exp(self, o, fp):
         """Differentiate an exp."""
         return fp * o
 
     def ln(self, o, fp):
         """Differentiate a ln."""
-        f, = o.ufl_operands
+        (f,) = o.ufl_operands
         if isinstance(f, Zero):
             raise ZeroDivisionError()
         return fp / f
 
     def cos(self, o, fp):
         """Differentiate a cos."""
-        f, = o.ufl_operands
+        (f,) = o.ufl_operands
         return fp * -sin(f)
 
     def sin(self, o, fp):
         """Differentiate a sin."""
-        f, = o.ufl_operands
+        (f,) = o.ufl_operands
         return fp * cos(f)
 
     def tan(self, o, fp):
         """Differentiate a tan."""
-        f, = o.ufl_operands
+        (f,) = o.ufl_operands
         return 2.0 * fp / (cos(2.0 * f) + 1.0)
 
     def cosh(self, o, fp):
         """Differentiate a cosh."""
-        f, = o.ufl_operands
+        (f,) = o.ufl_operands
         return fp * sinh(f)
 
     def sinh(self, o, fp):
         """Differentiate a sinh."""
-        f, = o.ufl_operands
+        (f,) = o.ufl_operands
         return fp * cosh(f)
 
     def tanh(self, o, fp):
         """Differentiate a tanh."""
-        f, = o.ufl_operands
+        (f,) = o.ufl_operands
 
         def sech(y):
             return (2.0 * cosh(y)) / (cosh(2.0 * y) + 1.0)
-        return fp * sech(f)**2
+
+        return fp * sech(f) ** 2
 
     def acos(self, o, fp):
         """Differentiate an acos."""
-        f, = o.ufl_operands
+        (f,) = o.ufl_operands
         return -fp / sqrt(1.0 - f**2)
 
     def asin(self, o, fp):
         """Differentiate an asin."""
-        f, = o.ufl_operands
+        (f,) = o.ufl_operands
         return fp / sqrt(1.0 - f**2)
 
     def atan(self, o, fp):
         """Differentiate an atan."""
-        f, = o.ufl_operands
+        (f,) = o.ufl_operands
         return fp / (1.0 + f**2)
 
     def atan2(self, o, fp, gp):
         """Differentiate an atan2."""
         f, g = o.ufl_operands
         return (g * fp - f * gp) / (f**2 + g**2)
 
     def erf(self, o, fp):
         """Differentiate an erf."""
-        f, = o.ufl_operands
-        return fp * (2.0 / sqrt(pi) * exp(-f**2))
+        (f,) = o.ufl_operands
+        return fp * (2.0 / sqrt(pi) * exp(-(f**2)))
 
     # --- Bessel functions
 
     def bessel_j(self, o, nup, fp):
         """Differentiate a bessel_j."""
         nu, f = o.ufl_operands
         if not (nup is None or isinstance(nup, Zero)):
-            raise NotImplementedError("Differentiation of bessel function w.r.t. nu is not supported.")
+            raise NotImplementedError(
+                "Differentiation of bessel function w.r.t. nu is not supported."
+            )
 
         if isinstance(nu, Zero):
             op = -bessel_J(1, f)
         else:
             op = 0.5 * (bessel_J(nu - 1, f) - bessel_J(nu + 1, f))
         return op * fp
 
     def bessel_y(self, o, nup, fp):
         """Differentiate a bessel_y."""
         nu, f = o.ufl_operands
         if not (nup is None or isinstance(nup, Zero)):
-            raise NotImplementedError("Differentiation of bessel function w.r.t. nu is not supported.")
+            raise NotImplementedError(
+                "Differentiation of bessel function w.r.t. nu is not supported."
+            )
 
         if isinstance(nu, Zero):
             op = -bessel_Y(1, f)
         else:
             op = 0.5 * (bessel_Y(nu - 1, f) - bessel_Y(nu + 1, f))
         return op * fp
 
     def bessel_i(self, o, nup, fp):
         """Differentiate a bessel_i."""
         nu, f = o.ufl_operands
         if not (nup is None or isinstance(nup, Zero)):
-            raise NotImplementedError("Differentiation of bessel function w.r.t. nu is not supported.")
+            raise NotImplementedError(
+                "Differentiation of bessel function w.r.t. nu is not supported."
+            )
 
         if isinstance(nu, Zero):
             op = bessel_I(1, f)
         else:
             op = 0.5 * (bessel_I(nu - 1, f) + bessel_I(nu + 1, f))
         return op * fp
 
     def bessel_k(self, o, nup, fp):
         """Differentiate a bessel_k."""
         nu, f = o.ufl_operands
         if not (nup is None or isinstance(nup, Zero)):
-            raise NotImplementedError("Differentiation of bessel function w.r.t. nu is not supported.")
+            raise NotImplementedError(
+                "Differentiation of bessel function w.r.t. nu is not supported."
+            )
 
         if isinstance(nu, Zero):
             op = -bessel_K(1, f)
         else:
             op = -0.5 * (bessel_K(nu - 1, f) + bessel_K(nu + 1, f))
         return op * fp
 
@@ -568,15 +625,16 @@
 
     # --- Specialized rules for form arguments
 
     def base_form_operator(self, o):
         """Differentiate a base_form_operator."""
         # Push the grad through the operator is not legal in most cases:
         #    -> Not enouth regularity for chain rule to hold!
-        # By the time we evaluate `grad(o)`, the operator `o` will have been assembled and substituted by its output.
+        # By the time we evaluate `grad(o)`, the operator `o` will have
+        # been assembled and substituted by its output.
         return Grad(o)
 
     def coefficient(self, o):
         """Differentiate a coefficient."""
         if is_cellwise_constant(o):
             return self.independent_terminal(o)
         return Grad(o)
@@ -593,15 +651,15 @@
 
     # --- Rules for values or derivatives in reference frame
 
     def reference_value(self, o):
         """Differentiate a reference_value."""
         # grad(o) == grad(rv(f)) -> K_ji*rgrad(rv(f))_rj
         f = o.ufl_operands[0]
-        if f.ufl_element().mapping() == "physical":
+        if isinstance(f.ufl_element().pullback, PhysicalPullback):
             # TODO: Do we need to be more careful for immersed things?
             return ReferenceGrad(o)
 
         if not f._ufl_is_terminal_:
             raise ValueError("ReferenceValue can only wrap a terminal")
         domain = extract_unique_domain(f)
         K = JacobianInverse(domain)
@@ -609,15 +667,17 @@
         return Do
 
     def reference_grad(self, o):
         """Differentiate a reference_grad."""
         # grad(o) == grad(rgrad(rv(f))) -> K_ji*rgrad(rgrad(rv(f)))_rj
         f = o.ufl_operands[0]
 
-        valid_operand = f._ufl_is_in_reference_frame_ or isinstance(f, (JacobianInverse, SpatialCoordinate))
+        valid_operand = f._ufl_is_in_reference_frame_ or isinstance(
+            f, (JacobianInverse, SpatialCoordinate)
+        )
         if not valid_operand:
             raise ValueError("ReferenceGrad can only wrap a reference frame type!")
         domain = extract_unique_domain(f)
         K = JacobianInverse(domain)
         Do = grad_to_reference_grad(o, K)
         return Do
 
@@ -664,18 +724,18 @@
     # grad(o) == K_ji rgrad(o)_rj
     Do = as_tensor(K[j, i] * ReferenceGrad(o)[r + (j,)], r + (i,))
     return Do
 
 
 class ReferenceGradRuleset(GenericDerivativeRuleset):
     """Apply the reference grad derivative."""
+
     def __init__(self, topological_dimension):
         """Initialise."""
-        GenericDerivativeRuleset.__init__(self,
-                                          var_shape=(topological_dimension,))
+        GenericDerivativeRuleset.__init__(self, var_shape=(topological_dimension,))
         self._Id = Identity(topological_dimension)
 
     # --- Specialized rules for geometric quantities
 
     def geometric_quantity(self, o):
         """Differentiate a geometric_quantity.
 
@@ -722,33 +782,35 @@
         """Differentiate an argument."""
         raise ValueError("Argument should be wrapped in ReferenceValue by now")
 
     # --- Nesting of gradients
 
     def grad(self, o):
         """Differentiate a grad."""
-        raise ValueError(f"Grad should have been transformed by this point, but got {type(o).__name__}.")
+        raise ValueError(
+            f"Grad should have been transformed by this point, but got {type(o).__name__}."
+        )
 
     def reference_grad(self, o):
         """Differentiate a reference_grad.
 
         Represent ref_grad(ref_grad(f)) as RefGrad(RefGrad(f)).
         """
         # Check that o is a "differential terminal"
-        if not isinstance(o.ufl_operands[0],
-                          (ReferenceGrad, ReferenceValue, Terminal)):
+        if not isinstance(o.ufl_operands[0], (ReferenceGrad, ReferenceValue, Terminal)):
             raise ValueError("Expecting only grads applied to a terminal.")
         return ReferenceGrad(o)
 
     cell_avg = GenericDerivativeRuleset.independent_operator
     facet_avg = GenericDerivativeRuleset.independent_operator
 
 
 class VariableRuleset(GenericDerivativeRuleset):
     """Differentiate with respect to a variable."""
+
     def __init__(self, var):
         """Initialise."""
         GenericDerivativeRuleset.__init__(self, var_shape=var.ufl_shape)
         if var.ufl_free_indices:
             raise ValueError("Differentiation variable cannot have free indices.")
         self._variable = var
         self._Id = self._make_identity(self._var_shape)
@@ -785,17 +847,14 @@
 
     # Explicitly defining dg/dw == 0
     geometric_quantity = GenericDerivativeRuleset.independent_terminal
 
     # Explicitly defining da/dw == 0
     argument = GenericDerivativeRuleset.independent_terminal
 
-    # def _argument(self, o):
-    #    return AnnotatedZero(o.ufl_shape + self._var_shape, arguments=(o,))  # TODO: Missing this type
-
     def coefficient(self, o):
         """Differentiate a coefficient.
 
         df/dv = Id if v is f else 0.
 
         Note that if v = variable(f), df/dv is still 0,
         but if v == f, i.e. isinstance(v, Coefficient) == True,
@@ -832,34 +891,34 @@
     # --- Rules for values or derivatives in reference frame
 
     def reference_value(self, o):
         """Differentiate a reference_value."""
         # d/dv(o) == d/dv(rv(f)) = 0 if v is not f, or rv(dv/df)
         v = self._variable
         if isinstance(v, Coefficient) and o.ufl_operands[0] == v:
-            if v.ufl_element().mapping() != "identity":
+            if not v.ufl_element().pullback.is_identity:
                 # FIXME: This is a bit tricky, instead of Identity it is
                 #   actually inverse(transform), or we should rather not
                 #   convert to reference frame in the first place
                 raise ValueError(
                     "Missing implementation: To handle derivatives of rv(f) w.r.t. f for "
-                    "mapped elements, rewriting to reference frame should not happen first...")
+                    "mapped elements, rewriting to reference frame should not happen first..."
+                )
             # dv/dv = identity of rank 2*rank(v)
             return self._Id
         else:
             # df/v = 0
             return self.independent_terminal(o)
 
     def reference_grad(self, o):
         """Differentiate a reference_grad.
 
         Variable derivative of a gradient of a terminal must be 0.
         """
-        if not isinstance(o.ufl_operands[0],
-                          (ReferenceGrad, ReferenceValue)):
+        if not isinstance(o.ufl_operands[0], (ReferenceGrad, ReferenceValue)):
             raise ValueError("Unexpected argument to reference_grad.")
         return self.independent_terminal(o)
 
     cell_avg = GenericDerivativeRuleset.independent_operator
     facet_avg = GenericDerivativeRuleset.independent_operator
 
 
@@ -942,15 +1001,18 @@
             # shape(dfdu) == shape(f) + shape(v)
             # shape(f) == shape(g) == shape(dfdu : v)
 
             # Make sure we have a tuple to match the self._v tuple
             if not isinstance(dos, tuple):
                 dos = (dos,)
             if len(dos) != len(self._v):
-                raise ValueError("Got a tuple of arguments, expecting a matching tuple of coefficient derivatives.")
+                raise ValueError(
+                    "Got a tuple of arguments, expecting a "
+                    "matching tuple of coefficient derivatives."
+                )
             dosum = Zero(o.ufl_shape)
             for do, v in zip(dos, self._v):
                 so, oi = as_scalar(do)
                 rv = len(oi) - len(v.ufl_shape)
                 oi1 = oi[:rv]
                 oi2 = oi[rv:]
                 prod = so * v[oi2]
@@ -958,15 +1020,17 @@
                     dosum += as_tensor(prod, oi1)
                 else:
                     dosum += prod
             return dosum
 
     def reference_value(self, o):
         """Differentiate a reference_value."""
-        raise NotImplementedError("Currently no support for ReferenceValue in CoefficientDerivative.")
+        raise NotImplementedError(
+            "Currently no support for ReferenceValue in CoefficientDerivative."
+        )
         # TODO: This is implementable for regular derivative(M(f),f,v)
         #       but too messy if customized coefficient derivative
         #       relations are given by the user.  We would only need
         #       this to allow the user to write
         #       derivative(...ReferenceValue...,...).
         # f, = o.ufl_operands
         # if not f._ufl_is_terminal_:
@@ -976,15 +1040,17 @@
         #     # FIXME: requires that v is an Argument with the same element mapping!
         #     return ReferenceValue(v)
         # else:
         #     return self.independent_terminal(o)
 
     def reference_grad(self, o):
         """Differentiate a reference_grad."""
-        raise NotImplementedError("Currently no support for ReferenceGrad in CoefficientDerivative.")
+        raise NotImplementedError(
+            "Currently no support for ReferenceGrad in CoefficientDerivative."
+        )
         # TODO: This is implementable for regular derivative(M(f),f,v)
         #       but too messy if customized coefficient derivative
         #       relations are given by the user.  We would only need
         #       this to allow the user to write
         #       derivative(...ReferenceValue...,...).
 
     def grad(self, g):
@@ -995,28 +1061,28 @@
         # return zero.  Complications occur when dealing with
         # derivatives w.r.t. single components...
 
         # Figure out how many gradients are around the inner terminal
         ngrads = 0
         o = g
         while isinstance(o, Grad):
-            o, = o.ufl_operands
+            (o,) = o.ufl_operands
             ngrads += 1
         # `grad(N)` where N is a BaseFormOperator is treated as if `N` was a Coefficient.
         if not isinstance(o, (FormArgument, BaseFormOperator)):
             raise ValueError(f"Expecting gradient of a FormArgument, not {ufl_err_str(o)}.")
 
         def apply_grads(f):
             for i in range(ngrads):
                 f = Grad(f)
             return f
 
         # Find o among all w without any indexing, which makes this
         # easy
-        for (w, v) in zip(self._w, self._v):
+        for w, v in zip(self._w, self._v):
             if o == w and isinstance(v, FormArgument):
                 # Case: d/dt [w + t v]
                 return apply_grads(v)
 
         # If o is not among coefficient derivatives, return do/dw=0
         gprimesum = Zero(g.ufl_shape)
 
@@ -1048,16 +1114,15 @@
             else:
                 Ejj, jj = 1, ()
             gprimeterm = as_tensor(Ejj * Dvkk, jj + kk)
             return gprimeterm
 
         # Accumulate contributions from variations in different
         # components
-        for (w, v) in zip(self._w, self._v):
-
+        for w, v in zip(self._w, self._v):
             # -- Analyse differentiation variable coefficient -- #
 
             # Can differentiate a Form wrt a BaseFormOperator
             if isinstance(w, (FormArgument, BaseFormOperator)):
                 if not w == o:
                     continue
                 wshape = w.ufl_shape
@@ -1067,28 +1132,30 @@
                     return apply_grads(v)
 
                 elif isinstance(v, ListTensor):
                     # Case: d/dt [w + t <...,v,...>]
                     for wcomp, vsub in unwrap_list_tensor(v):
                         if not isinstance(vsub, Zero):
                             vval, vcomp = analyse_variation_argument(vsub)
-                            gprimesum = gprimesum + compute_gprimeterm(ngrads, vval, vcomp, wshape, wcomp)
+                            gprimesum = gprimesum + compute_gprimeterm(
+                                ngrads, vval, vcomp, wshape, wcomp
+                            )
 
                 else:
                     if wshape != ():
                         raise ValueError("Expecting scalar coefficient in this branch.")
                     # Case: d/dt [w + t v[...]]
                     wval, wcomp = w, ()
 
                     vval, vcomp = analyse_variation_argument(v)
-                    gprimesum = gprimesum + compute_gprimeterm(ngrads, vval,
-                                                               vcomp, wshape,
-                                                               wcomp)
+                    gprimesum = gprimesum + compute_gprimeterm(ngrads, vval, vcomp, wshape, wcomp)
 
-            elif isinstance(w, Indexed):  # This path is tested in unit tests, but not actually used?
+            elif isinstance(
+                w, Indexed
+            ):  # This path is tested in unit tests, but not actually used?
                 # Case: d/dt [w[...] + t v[...]]
                 # Case: d/dt [w[...] + t v]
                 wval, wcomp = w.ufl_operands
                 if not wval == o:
                     continue
                 assert isinstance(wval, FormArgument)
                 if not all(isinstance(k, FixedIndex) for k in wcomp):
@@ -1115,22 +1182,23 @@
             else:
                 # Make sure we have a tuple to match the self._v tuple
                 if not isinstance(oprimes, tuple):
                     oprimes = (oprimes,)
                     if len(oprimes) != len(self._v):
                         raise ValueError(
                             "Got a tuple of arguments, expecting a"
-                            " matching tuple of coefficient derivatives.")
+                            " matching tuple of coefficient derivatives."
+                        )
 
                 # Compute dg/dw_j = dg/dw_h : v.
                 # Since we may actually have a tuple of oprimes and vs
                 # in a 'mixed' space, sum over them all to get the
                 # complete inner product. Using indices to define a
                 # non-compound inner product.
-                for (oprime, v) in zip(oprimes, self._v):
+                for oprime, v in zip(oprimes, self._v):
                     raise NotImplementedError("FIXME: Figure out how to do this with ngrads")
                     so, oi = as_scalar(oprime)
                     rv = len(v.ufl_shape)
                     oi1 = oi[:-rv]
                     oi2 = oi[-rv:]
                     prod = so * v[oi2]
                     if oi1:
@@ -1144,16 +1212,18 @@
         """Differentiate a coordinate_derivative."""
         o = o.ufl_operands
         return CoordinateDerivative(map_expr_dag(self, o[0]), o[1], o[2], o[3])
 
     def base_form_operator(self, o, *dfs):
         """Differentiate a base_form_operator.
 
-        If d_coeff = 0 => BaseFormOperator's derivative is taken wrt a variable => we call the appropriate handler.
-        Otherwise => differentiation done wrt the BaseFormOperator (dF/dN[Nhat]) => we treat o as a Coefficient.
+        If d_coeff = 0 => BaseFormOperator's derivative is taken wrt a
+        variable => we call the appropriate handler. Otherwise =>
+        differentiation done wrt the BaseFormOperator (dF/dN[Nhat]) =>
+        we treat o as a Coefficient.
         """
         d_coeff = self.coefficient(o)
         # It also handles the non-scalar case
         if d_coeff == 0:
             self.pending_operations += (o,)
         return d_coeff
 
@@ -1178,43 +1248,53 @@
             # Convert ufl.Zero into ZeroBaseForm
             return ZeroBaseForm(o.arguments() + self._v)
         return dc
 
     def matrix(self, M):
         """Differentiate a matrix."""
         # Matrix rule: D_w[v](M) = v if M == w else 0
-        # We can't differentiate wrt a matrix so always return zero in the appropriate space
+        # We can't differentiate wrt a matrix so always return zero in
+        # the appropriate space
         return ZeroBaseForm(M.arguments() + self._v)
 
 
 class BaseFormOperatorDerivativeRuleset(GateauxDerivativeRuleset):
     """Apply AFD (Automatic Functional Differentiation) to BaseFormOperator.
 
     Implements rules for the Gateaux derivative D_w[v](...) defined as
     D_w[v](B) = d/dtau B(w+tau v)|tau=0 where B is a ufl.BaseFormOperator.
     """
 
     def __init__(self, coefficients, arguments, coefficient_derivatives, pending_operations):
         """Initialise."""
-        GateauxDerivativeRuleset.__init__(self, coefficients, arguments, coefficient_derivatives, pending_operations)
+        GateauxDerivativeRuleset.__init__(
+            self, coefficients, arguments, coefficient_derivatives, pending_operations
+        )
 
     def pending_operations_recording(base_form_operator_handler):
         """Decorate a function to record pending operations."""
+
         def wrapper(self, base_form_op, *dfs):
             """Decorate."""
-            # Get the outer `BaseFormOperator` expression, i.e. the operator that is being differentiated.
+            # Get the outer `BaseFormOperator` expression, i.e. the
+            # operator that is being differentiated.
             expression = self.pending_operations.expression
-            # If the base form operator we observe is different from the outer `BaseFormOperator`:
-            # -> Record that `BaseFormOperator` so that `d(expression)/d(base_form_op)` can then be computed later.
+            # If the base form operator we observe is different from the
+            # outer `BaseFormOperator`:
+            # -> Record that `BaseFormOperator` so that
+            # `d(expression)/d(base_form_op)` can then be computed
+            # later.
             # Else:
-            # -> Compute the Gateaux derivative of `base_form_ops` by calling the appropriate handler.
+            # -> Compute the Gateaux derivative of `base_form_ops` by
+            # calling the appropriate handler.
             if expression != base_form_op:
                 self.pending_operations += (base_form_op,)
                 return self.coefficient(base_form_op)
             return base_form_operator_handler(self, base_form_op, *dfs)
+
         return wrapper
 
     @pending_operations_recording
     def interpolate(self, i_op, dw):
         """Differentiate an interpolate."""
         # Interpolate rule: D_w[v](i_op(w, v*)) = i_op(v, v*), by linearity of Interpolate!
         if not dw:
@@ -1232,24 +1312,30 @@
             derivatives = tuple(dj + int(i == j) for j, dj in enumerate(N.derivatives))
             if len(extract_arguments(df)) != 0:
                 # Handle the symbolic differentiation of external operators.
                 # This bit returns:
                 #
                 #   `\sum_{i} dNdOi(..., Oi, ...; DOi(u)[v], ..., v*)`
                 #
-                # where we differentate wrt u, Oi is the i-th operand, N(..., Oi, ...; ..., v*) an ExternalOperator
-                # and v the direction (Argument). dNdOi(..., Oi, ...; DOi(u)[v]) is an ExternalOperator
-                # representing the Gateaux-derivative of N. For example:
+                # where we differentate wrt u, Oi is the i-th operand,
+                # N(..., Oi, ...; ..., v*) an ExternalOperator and v the
+                # direction (Argument). dNdOi(..., Oi, ...; DOi(u)[v])
+                # is an ExternalOperator representing the
+                # Gateaux-derivative of N. For example:
                 #  -> From N(u) = u**2, we get `dNdu(u; uhat, v*) = 2 * u * uhat`.
                 new_args = N.argument_slots() + (df,)
-                extop = N._ufl_expr_reconstruct_(*N.ufl_operands, derivatives=derivatives, argument_slots=new_args)
+                extop = N._ufl_expr_reconstruct_(
+                    *N.ufl_operands, derivatives=derivatives, argument_slots=new_args
+                )
             elif df == 0:
                 extop = Zero(N.ufl_shape)
             else:
-                raise NotImplementedError('Frechet derivative of external operators need to be provided!')
+                raise NotImplementedError(
+                    "Frechet derivative of external operators need to be provided!"
+                )
             result += (extop,)
         return sum(result)
 
 
 class DerivativeRuleDispatcher(MultiFunction):
     """Dispatch a derivative rule."""
 
@@ -1274,95 +1360,95 @@
 
     ufl_type = MultiFunction.reuse_if_untouched
 
     def grad(self, o, f):
         """Apply to a grad."""
         rules = GradRuleset(o.ufl_shape[-1])
         key = (GradRuleset, o.ufl_shape[-1])
-        return map_expr_dag(rules, f,
-                            vcache=self.vcaches[key],
-                            rcache=self.rcaches[key])
+        return map_expr_dag(rules, f, vcache=self.vcaches[key], rcache=self.rcaches[key])
 
     def reference_grad(self, o, f):
         """Apply to a reference_grad."""
         rules = ReferenceGradRuleset(o.ufl_shape[-1])  # FIXME: Look over this and test better.
         key = (ReferenceGradRuleset, o.ufl_shape[-1])
-        return map_expr_dag(rules, f,
-                            vcache=self.vcaches[key],
-                            rcache=self.rcaches[key])
+        return map_expr_dag(rules, f, vcache=self.vcaches[key], rcache=self.rcaches[key])
 
     def variable_derivative(self, o, f, dummy_v):
         """Apply to a variable_derivative."""
         op = o.ufl_operands[1]
         rules = VariableRuleset(op)
         key = (VariableRuleset, op)
-        return map_expr_dag(rules, f,
-                            vcache=self.vcaches[key],
-                            rcache=self.rcaches[key])
+        return map_expr_dag(rules, f, vcache=self.vcaches[key], rcache=self.rcaches[key])
 
     def coefficient_derivative(self, o, f, dummy_w, dummy_v, dummy_cd):
         """Apply to a coefficient_derivative."""
         dummy, w, v, cd = o.ufl_operands
-        pending_operations = BaseFormOperatorDerivativeRecorder(f, w, arguments=v, coefficient_derivatives=cd)
+        pending_operations = BaseFormOperatorDerivativeRecorder(
+            f, w, arguments=v, coefficient_derivatives=cd
+        )
         rules = GateauxDerivativeRuleset(w, v, cd, pending_operations)
         key = (GateauxDerivativeRuleset, w, v, cd)
-        # We need to go through the dag first to record the pending operations
-        mapped_expr = map_expr_dag(rules, f,
-                                   vcache=self.vcaches[key],
-                                   rcache=self.rcaches[key])
-        # Need to account for pending operations that have been stored in other integrands
+        # We need to go through the dag first to record the pending
+        # operations
+        mapped_expr = map_expr_dag(rules, f, vcache=self.vcaches[key], rcache=self.rcaches[key])
+        # Need to account for pending operations that have been stored
+        # in other integrands
         self.pending_operations += pending_operations
         return mapped_expr
 
     def base_form_operator_derivative(self, o, f, dummy_w, dummy_v, dummy_cd):
         """Apply to a base_form_operator_derivative."""
         dummy, w, v, cd = o.ufl_operands
-        pending_operations = BaseFormOperatorDerivativeRecorder(f, w, arguments=v, coefficient_derivatives=cd)
+        pending_operations = BaseFormOperatorDerivativeRecorder(
+            f, w, arguments=v, coefficient_derivatives=cd
+        )
         rules = BaseFormOperatorDerivativeRuleset(w, v, cd, pending_operations=pending_operations)
         key = (BaseFormOperatorDerivativeRuleset, w, v, cd)
         if isinstance(f, ZeroBaseForm):
-            arg, = v.ufl_operands
+            (arg,) = v.ufl_operands
             arguments = f.arguments()
             # derivative(F, u, du) with `du` a Coefficient
             # is equivalent to taking the action of the derivative.
             # In that case, we don't add arguments to `ZeroBaseForm`.
             if isinstance(arg, BaseArgument):
                 arguments += (arg,)
             return ZeroBaseForm(arguments)
         # We need to go through the dag first to record the pending operations
-        mapped_expr = map_expr_dag(rules, f,
-                                   vcache=self.vcaches[key],
-                                   rcache=self.rcaches[key])
+        mapped_expr = map_expr_dag(rules, f, vcache=self.vcaches[key], rcache=self.rcaches[key])
 
         mapped_f = rules.coefficient(f)
         if mapped_f != 0:
             # If dN/dN needs to return an Argument in N space
             # with N a BaseFormOperator.
             return mapped_f
         # Need to account for pending operations that have been stored in other integrands
         self.pending_operations += pending_operations
         return mapped_expr
 
     def coordinate_derivative(self, o, f, dummy_w, dummy_v, dummy_cd):
         """Apply to a coordinate_derivative."""
         o_ = o.ufl_operands
         key = (CoordinateDerivative, o_[0])
-        return CoordinateDerivative(map_expr_dag(self, o_[0],
-                                                 vcache=self.vcaches[key],
-                                                 rcache=self.rcaches[key]),
-                                    o_[1], o_[2], o_[3])
+        return CoordinateDerivative(
+            map_expr_dag(self, o_[0], vcache=self.vcaches[key], rcache=self.rcaches[key]),
+            o_[1],
+            o_[2],
+            o_[3],
+        )
 
     def base_form_coordinate_derivative(self, o, f, dummy_w, dummy_v, dummy_cd):
         """Apply to a base_form_coordinate_derivative."""
         o_ = o.ufl_operands
         key = (BaseFormCoordinateDerivative, o_[0])
-        return BaseFormCoordinateDerivative(map_expr_dag(self, o_[0],
-                                                         vcache=self.vcaches[key],
-                                                         rcache=self.rcaches[key]),
-                                            o_[1], o_[2], o_[3])
+        return BaseFormCoordinateDerivative(
+            map_expr_dag(self, o_[0], vcache=self.vcaches[key], rcache=self.rcaches[key]),
+            o_[1],
+            o_[2],
+            o_[3],
+        )
 
     def indexed(self, o, Ap, ii):  # TODO: (Partially) duplicated in generic rules
         """Apply to an indexed."""
         # Reuse if untouched
         if Ap is o.ufl_operands[0]:
             return o
 
@@ -1389,23 +1475,26 @@
             op = Indexed(Ap, MultiIndex(ii.indices() + kk))
             op = as_tensor(op, kk)
         else:
             op = Indexed(Ap, ii)
         return op
 
 
-class BaseFormOperatorDerivativeRecorder():
+class BaseFormOperatorDerivativeRecorder:
     """A derivative recorded for a base form operator."""
 
     def __init__(self, expression, var, **kwargs):
         """Initialise."""
         base_form_ops = kwargs.pop("base_form_ops", ())
 
-        if kwargs.keys() != {'arguments', 'coefficient_derivatives'}:
-            raise ValueError("Only `arguments` and `coefficient_derivatives` are allowed as derivative arguments.")
+        if kwargs.keys() != {"arguments", "coefficient_derivatives"}:
+            raise ValueError(
+                "Only `arguments` and `coefficient_derivatives` are "
+                "allowed as derivative arguments."
+            )
 
         self.expression = expression
         self.var = var
         self.der_kwargs = kwargs
         self.base_form_ops = base_form_ops
 
     def __len__(self):
@@ -1418,26 +1507,31 @@
 
     def __add__(self, other):
         """Add."""
         if isinstance(other, (list, tuple)):
             base_form_ops = self.base_form_ops + other
         elif isinstance(other, BaseFormOperatorDerivativeRecorder):
             if self.der_kwargs != other.der_kwargs:
-                raise ValueError(f"Derivative arguments must match when summing {type(self).__name__} objects.")
+                raise ValueError(
+                    f"Derivative arguments must match when summing {type(self).__name__} objects."
+                )
             base_form_ops = self.base_form_ops + other.base_form_ops
         else:
-            raise NotImplementedError(f"Sum of {type(self)} and {type(other)} objects is not supported.")
-
-        return BaseFormOperatorDerivativeRecorder(self.expression, self.var,
-                                                  base_form_ops=base_form_ops,
-                                                  **self.der_kwargs)
+            raise NotImplementedError(
+                f"Sum of {type(self)} and {type(other)} objects is not supported."
+            )
+
+        return BaseFormOperatorDerivativeRecorder(
+            self.expression, self.var, base_form_ops=base_form_ops, **self.der_kwargs
+        )
 
     def __radd__(self, other):
         """Add."""
-        # Recording order doesn't matter as collected `BaseFormOperator`s are sorted later on.
+        # Recording order doesn't matter as collected
+        # `BaseFormOperator`s are sorted later on.
         return self.__add__(other)
 
     def __iadd__(self, other):
         """Add."""
         if isinstance(other, (list, tuple)):
             self.base_form_ops += other
         elif isinstance(other, BaseFormOperatorDerivativeRecorder):
@@ -1457,16 +1551,18 @@
         A differentiated expression
     """
     # Notation: Let `var` be the thing we are differentating with respect to.
 
     rules = DerivativeRuleDispatcher()
 
     # If we hit a base form operator (bfo), then if `var` is:
-    #    - a BaseFormOperator → Return `d(expression)/dw` where `w` is the coefficient produced by the bfo `var`.
-    #    - else → Record the bfo on the MultiFunction object and returns 0.
+    #    - a BaseFormOperator → Return `d(expression)/dw` where `w` is
+    #      the coefficient produced by the bfo `var`.
+    #    - else → Record the bfo on the MultiFunction object and returns
+    #    - 0.
     # Example:
     #    → If derivative(F(u, N(u); v), u) was taken the following line would compute `∂F/∂u`.
     dexpression_dvar = map_integrand_dags(rules, expression)
 
     # Get the recorded delayed operations
     pending_operations = rules.pending_operations
     if not pending_operations:
@@ -1474,37 +1570,48 @@
 
     # Don't take into account empty Forms
     if not (isinstance(dexpression_dvar, Form) and len(dexpression_dvar.integrals()) == 0):
         dexpression_dvar = (dexpression_dvar,)
     else:
         dexpression_dvar = ()
 
-    # Retrieve the base form operators, var, and the argument and coefficient_derivatives for `derivative`
+    # Retrieve the base form operators, var, and the argument and
+    # coefficient_derivatives for `derivative`
     var = pending_operations.var
     base_form_ops = pending_operations.base_form_ops
     der_kwargs = pending_operations.der_kwargs
     for N in sorted(set(base_form_ops), key=lambda x: x.count()):
         # -- Replace dexpr/dvar by dexpr/dN -- #
-        # We don't use `apply_derivatives` since the differentiation is done via `\partial` and not `d`.
-        dexpr_dN = map_integrand_dags(rules, replace_derivative_nodes(expression, {var.ufl_operands[0]: N}))
+        # We don't use `apply_derivatives` since the differentiation is
+        # done via `\partial` and not `d`.
+        dexpr_dN = map_integrand_dags(
+            rules, replace_derivative_nodes(expression, {var.ufl_operands[0]: N})
+        )
         # -- Add the BaseFormOperatorDerivative node -- #
-        var_arg, = der_kwargs['arguments'].ufl_operands
-        cd = der_kwargs['coefficient_derivatives']
-        # Not always the case since `derivative`'s syntax enables one to use a Coefficient as the Gateaux direction
+        (var_arg,) = der_kwargs["arguments"].ufl_operands
+        cd = der_kwargs["coefficient_derivatives"]
+        # Not always the case since `derivative`'s syntax enables one to
+        # use a Coefficient as the Gateaux direction
         if isinstance(var_arg, BaseArgument):
-            # Construct the argument number based on the BaseFormOperator arguments instead of naively
-            # using `var_arg`. This is critical when BaseFormOperators are used inside 0-forms.
+            # Construct the argument number based on the
+            # BaseFormOperator arguments instead of naively using
+            # `var_arg`. This is critical when BaseFormOperators are
+            # used inside 0-forms.
             #
             # Example: F = 0.5 * u** 2 * dx + 0.5 * N(u; v*)** 2 * dx
             #    -> dFdu[vhat] = <u, vhat> + Action(<N(u; v*), v0>, dNdu(u; v1, v*))
-            # with `vhat` a 0-numbered argument, and where `v1` and `vhat` have the same function space but
-            # a different number. Here, applying `vhat` (`var_arg`) naively would result in `dNdu(u; vhat, v*)`,
-            # i.e. the 2-forms `dNdu` would have two 0-numbered arguments. Instead we increment the argument number
-            # of `vhat` to form `v1`.
-            var_arg = type(var_arg)(var_arg.ufl_function_space(), number=len(N.arguments()), part=var_arg.part())
+            # with `vhat` a 0-numbered argument, and where `v1` and
+            # `vhat` have the same function space but a different
+            # number. Here, applying `vhat` (`var_arg`) naively would
+            # result in `dNdu(u; vhat, v*)`, i.e. the 2-forms `dNdu`
+            # would have two 0-numbered arguments. Instead we increment
+            # the argument number of `vhat` to form `v1`.
+            var_arg = type(var_arg)(
+                var_arg.ufl_function_space(), number=len(N.arguments()), part=var_arg.part()
+            )
         dN_dvar = apply_derivatives(BaseFormOperatorDerivative(N, var, ExprList(var_arg), cd))
         # -- Sum the Action: dF/du = ∂F/∂u + \sum_{i=1,...} Action(∂F/∂Ni, dNi/du) -- #
         if not (isinstance(dexpr_dN, Form) and len(dexpr_dN.integrals()) == 0):
             # In this case: Action <=> ufl.action since `dN_var` has 2 arguments.
             # We use Action to handle the trivial case `dN_dvar` = 0.
             dexpression_dvar += (Action(dexpr_dN, dN_dvar),)
     return sum(dexpression_dvar)
@@ -1545,29 +1652,33 @@
     geometric_quantity = GenericDerivativeRuleset.independent_terminal
 
     # Explicitly defining da/dw == 0
     argument = GenericDerivativeRuleset.independent_terminal
 
     def coefficient(self, o):
         """Differentiate a coefficient."""
-        raise NotImplementedError("CoordinateDerivative of coefficient in physical space is not implemented.")
+        raise NotImplementedError(
+            "CoordinateDerivative of coefficient in physical space is not implemented."
+        )
 
     def grad(self, o):
         """Differentiate a grad."""
         raise NotImplementedError("CoordinateDerivative grad in physical space is not implemented.")
 
     def spatial_coordinate(self, o):
         """Differentiate a spatial_coordinate."""
         do = self._w2v.get(o)
         # d x /d x => Argument(x.function_space())
         if do is not None:
             return do
         else:
-            raise NotImplementedError("CoordinateDerivative found a SpatialCoordinate that is different "
-                                      "from the one being differentiated.")
+            raise NotImplementedError(
+                "CoordinateDerivative found a SpatialCoordinate that is different "
+                "from the one being differentiated."
+            )
 
     def reference_value(self, o):
         """Differentiate a reference_value."""
         do = self._cd.get(o)
         if do is not None:
             return do
         else:
@@ -1575,37 +1686,43 @@
 
     def reference_grad(self, g):
         """Differentiate a reference_grad."""
         # d (grad_X(...(x)) / dx => grad_X(...(Argument(x.function_space()))
         o = g
         ngrads = 0
         while isinstance(o, ReferenceGrad):
-            o, = o.ufl_operands
+            (o,) = o.ufl_operands
             ngrads += 1
         if not (isinstance(o, SpatialCoordinate) or isinstance(o.ufl_operands[0], FormArgument)):
             raise ValueError(f"Expecting gradient of a FormArgument, not {ufl_err_str(o)}")
 
         def apply_grads(f):
             for i in range(ngrads):
                 f = ReferenceGrad(f)
             return f
 
         # Find o among all w without any indexing, which makes this
         # easy
-        for (w, v) in zip(self._w, self._v):
-            if o == w and isinstance(v, ReferenceValue) and isinstance(v.ufl_operands[0], FormArgument):
+        for w, v in zip(self._w, self._v):
+            if (
+                o == w
+                and isinstance(v, ReferenceValue)
+                and isinstance(v.ufl_operands[0], FormArgument)
+            ):
                 # Case: d/dt [w + t v]
                 return apply_grads(v)
         return self.independent_terminal(o)
 
     def jacobian(self, o):
         """Differentiate a jacobian."""
         # d (grad_X(x))/d x => grad_X(Argument(x.function_space())
-        for (w, v) in zip(self._w, self._v):
-            if extract_unique_domain(o) == extract_unique_domain(w) and isinstance(v.ufl_operands[0], FormArgument):
+        for w, v in zip(self._w, self._v):
+            if extract_unique_domain(o) == extract_unique_domain(w) and isinstance(
+                v.ufl_operands[0], FormArgument
+            ):
                 return ReferenceGrad(v)
         return self.independent_terminal(o)
 
 
 class CoordinateDerivativeRuleDispatcher(MultiFunction):
     """Dispatcher."""
 
@@ -1636,18 +1753,20 @@
     def coefficient_derivative(self, o):
         """Apply to a coefficient_derivative."""
         return o
 
     def coordinate_derivative(self, o, f, w, v, cd):
         """Apply to a coordinate_derivative."""
         from ufl.algorithms import extract_unique_elements
+
         for space in extract_unique_elements(o):
-            if space.mapping() == "custom":
+            if isinstance(space.pullback, CustomPullback):
                 raise NotImplementedError(
-                    "CoordinateDerivative is not supported for elements with custom pull back.")
+                    "CoordinateDerivative is not supported for elements with custom pull back."
+                )
 
         _, w, v, cd = o.ufl_operands
         rules = CoordinateDerivativeRuleset(w, v, cd)
         key = (CoordinateDerivativeRuleset, w, v, cd)
         return map_expr_dag(rules, f, vcache=self.vcache[key], rcache=self.rcache[key])
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/apply_geometry_lowering.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/apply_geometry_lowering.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,34 +10,52 @@
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
 import warnings
 from functools import reduce
 from itertools import combinations
 
-from ufl.classes import (CellCoordinate, CellEdgeVectors, CellFacetJacobian,
-                         CellOrientation, CellOrigin, CellVertices, CellVolume,
-                         Expr, FacetEdgeVectors, FacetJacobian,
-                         FacetJacobianDeterminant, FloatValue, Form, Integral,
-                         Jacobian, JacobianDeterminant, JacobianInverse,
-                         MaxCellEdgeLength, ReferenceCellVolume,
-                         ReferenceFacetVolume, ReferenceGrad, ReferenceNormal,
-                         SpatialCoordinate)
+from ufl.classes import (
+    CellCoordinate,
+    CellEdgeVectors,
+    CellFacetJacobian,
+    CellOrientation,
+    CellOrigin,
+    CellVertices,
+    CellVolume,
+    Expr,
+    FacetEdgeVectors,
+    FacetJacobian,
+    FacetJacobianDeterminant,
+    FloatValue,
+    Form,
+    Integral,
+    Jacobian,
+    JacobianDeterminant,
+    JacobianInverse,
+    MaxCellEdgeLength,
+    ReferenceCellVolume,
+    ReferenceFacetVolume,
+    ReferenceGrad,
+    ReferenceNormal,
+    SpatialCoordinate,
+)
 from ufl.compound_expressions import cross_expr, determinant_expr, inverse_expr
 from ufl.core.multiindex import Index, indices
 from ufl.corealg.map_dag import map_expr_dag
 from ufl.corealg.multifunction import MultiFunction, memoized_handler
 from ufl.domain import extract_unique_domain
 from ufl.measure import custom_integral_types, point_integral_types
 from ufl.operators import conj, max_value, min_value, real, sqrt
 from ufl.tensors import as_tensor, as_vector
 
 
 class GeometryLoweringApplier(MultiFunction):
     """Geometry lowering."""
+
     def __init__(self, preserve_types=()):
         """Initialise."""
         MultiFunction.__init__(self)
         # Store preserve_types as boolean lookup table
         self._preserve_types = [False] * Expr._ufl_num_typecodes_
         for cls in preserve_types:
             self._preserve_types[cls._ufl_typecode_] = True
@@ -50,15 +68,15 @@
 
     @memoized_handler
     def jacobian(self, o):
         """Apply to jacobian."""
         if self._preserve_types[o._ufl_typecode_]:
             return o
         domain = extract_unique_domain(o)
-        if domain.ufl_coordinate_element().mapping() != "identity":
+        if not domain.ufl_coordinate_element().pullback.is_identity:
             raise ValueError("Piola mapped coordinates are not implemented.")
         # Note: No longer supporting domain.coordinates(), always
         # preserving SpatialCoordinate object.  However if Jacobians
         # are not preserved, using
         # ReferenceGrad(SpatialCoordinate(domain)) to represent them.
         x = self.spatial_coordinate(SpatialCoordinate(domain))
         return ReferenceGrad(x)
@@ -151,15 +169,15 @@
     def spatial_coordinate(self, o):
         """Apply to spatial_coordinate.
 
         Fall through to coordinate field of domain if it exists.
         """
         if self._preserve_types[o._ufl_typecode_]:
             return o
-        if extract_unique_domain(o).ufl_coordinate_element().mapping() != "identity":
+        if not extract_unique_domain(o).ufl_coordinate_element().pullback.is_identity:
             raise ValueError("Piola mapped coordinates are not implemented.")
         # No longer supporting domain.coordinates(), always preserving
         # SpatialCoordinate object.
         return o
 
     @memoized_handler
     def cell_coordinate(self, o):
@@ -180,16 +198,18 @@
 
     @memoized_handler
     def facet_cell_coordinate(self, o):
         """Apply to facet_cell_coordinate."""
         if self._preserve_types[o._ufl_typecode_]:
             return o
 
-        raise ValueError("Missing computation of facet reference coordinates "
-                         "from physical coordinates via mappings.")
+        raise ValueError(
+            "Missing computation of facet reference coordinates "
+            "from physical coordinates via mappings."
+        )
 
     @memoized_handler
     def cell_volume(self, o):
         """Apply to cell_volume."""
         if self._preserve_types[o._ufl_typecode_]:
             return o
 
@@ -256,15 +276,15 @@
         elif cellname == "tetrahedron":
             # la, lb, lc = lengths of the sides of an intermediate triangle
             # NOTE: Is here some hidden numbering assumption?
             la = elen[3] * elen[2]
             lb = elen[4] * elen[1]
             lc = elen[5] * elen[0]
             # p = perimeter
-            p = (la + lb + lc)
+            p = la + lb + lc
             # s = semiperimeter
             s = p / 2
             # area of intermediate triangle with Herons formula
             triangle_area = sqrt(s * (s - la) * (s - lb) * (s - lc))
             return triangle_area / (6.0 * cellvolume)
 
     @memoized_handler
@@ -280,15 +300,15 @@
     def _reduce_cell_edge_length(self, o, reduction_op):
         """Apply to _reduce_cell_edge_length."""
         if self._preserve_types[o._ufl_typecode_]:
             return o
 
         domain = extract_unique_domain(o)
 
-        if not domain.ufl_coordinate_element().degree() == 1:
+        if domain.ufl_coordinate_element().embedded_superdegree > 1:
             # Don't lower bendy cells, instead leave it to form compiler
             warnings.warn("Only know how to compute cell edge lengths of P1 or Q1 cell.")
             return o
 
         elif domain.ufl_cell().cellname() == "interval":
             # Interval optimization, square root not needed
             return self.cell_volume(CellVolume(domain))
@@ -305,15 +325,15 @@
     def cell_diameter(self, o):
         """Apply to cell_diameter."""
         if self._preserve_types[o._ufl_typecode_]:
             return o
 
         domain = extract_unique_domain(o)
 
-        if not domain.ufl_coordinate_element().degree() in {1, (1, 1)}:
+        if domain.ufl_coordinate_element().embedded_superdegree > 1:
             # Don't lower bendy cells, instead leave it to form compiler
             warnings.warn("Only know how to compute cell diameter of P1 or Q1 cell.")
             return o
 
         elif domain.is_piecewise_linear_simplex_domain():
             # Simplices
             return self.max_cell_edge_length(MaxCellEdgeLength(domain))
@@ -342,15 +362,15 @@
             return o
 
         domain = extract_unique_domain(o)
 
         if domain.ufl_cell().topological_dimension() < 3:
             raise ValueError("Facet edge lengths only make sense for topological dimension >= 3.")
 
-        elif not domain.ufl_coordinate_element().degree() == 1:
+        elif domain.ufl_coordinate_element().embedded_superdegree > 1:
             # Don't lower bendy cells, instead leave it to form compiler
             warnings.warn("Only know how to compute facet edge lengths of P1 or Q1 cell.")
             return o
 
         else:
             # P1 tetrahedron or Q1 hexahedron
             edges = FacetEdgeVectors(domain)
@@ -431,30 +451,33 @@
 
             # normalise
             i = Index()
             n = ndir / sqrt(ndir[i] * ndir[i])
             r = n
 
         if r.ufl_shape != o.ufl_shape:
-            raise ValueError(f"Inconsistent dimensions (in={o.ufl_shape[0]}, out={r.ufl_shape[0]}).")
+            raise ValueError(
+                f"Inconsistent dimensions (in={o.ufl_shape[0]}, out={r.ufl_shape[0]})."
+            )
         return r
 
 
 def apply_geometry_lowering(form, preserve_types=()):
     """Change GeometricQuantity objects in expression to the lowest level GeometricQuantity objects.
 
     Assumes the expression is preprocessed or at least that derivatives have been expanded.
 
     Args:
         form: An Expr or Form.
         preserve_types: Preserved types
     """
     if isinstance(form, Form):
-        newintegrals = [apply_geometry_lowering(integral, preserve_types)
-                        for integral in form.integrals()]
+        newintegrals = [
+            apply_geometry_lowering(integral, preserve_types) for integral in form.integrals()
+        ]
         return Form(newintegrals)
 
     elif isinstance(form, Integral):
         integral = form
         if integral.integral_type() in (custom_integral_types + point_integral_types):
             automatic_preserve_types = [SpatialCoordinate, Jacobian]
         else:
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/apply_integral_scaling.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/apply_integral_scaling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-"""Algorithm for replacing gradients in an expression with reference gradients and coordinate mappings."""
+"""Algorithm for replacing gradients in an expression."""
 
 # Copyright (C) 2013-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
-from ufl.classes import JacobianDeterminant, FacetJacobianDeterminant, QuadratureWeight, Form, Integral
-from ufl.measure import custom_integral_types, point_integral_types
-from ufl.differentiation import CoordinateDerivative
 from ufl.algorithms.apply_geometry_lowering import apply_geometry_lowering
 from ufl.algorithms.estimate_degrees import estimate_total_polynomial_degree
+from ufl.classes import (
+    FacetJacobianDeterminant,
+    Form,
+    Integral,
+    JacobianDeterminant,
+    QuadratureWeight,
+)
+from ufl.differentiation import CoordinateDerivative
+from ufl.measure import custom_integral_types, point_integral_types
 
 
 def compute_integrand_scaling_factor(integral):
     """Change integrand geometry to the right representations."""
     domain = integral.ufl_domain()
     integral_type = integral.integral_type()
     # co = CellOrientation(domain)
@@ -48,15 +54,15 @@
 
     elif integral_type.startswith("interior_facet"):
         if tdim > 1:
             # Scaling integral by facet jacobian determinant from one
             # side and quadrature weight
             detFJ = FacetJacobianDeterminant(domain)
             degree = estimate_total_polynomial_degree(apply_geometry_lowering(detFJ))
-            scale = detFJ('+') * weight
+            scale = detFJ("+") * weight
         else:
             # No need to scale 'integral' over a vertex
             scale = 1
 
     elif integral_type in custom_integral_types:
         # Scaling with custom weight, which includes eventual volume
         # scaling
@@ -73,16 +79,15 @@
 
 
 def apply_integral_scaling(form):
     """Multiply integrands by a factor to scale the integral to reference frame."""
     # TODO: Consider adding an in_reference_frame property to Integral
     #       and checking it here and setting it in the returned form
     if isinstance(form, Form):
-        newintegrals = [apply_integral_scaling(integral)
-                        for integral in form.integrals()]
+        newintegrals = [apply_integral_scaling(integral) for integral in form.integrals()]
         return Form(newintegrals)
 
     elif isinstance(form, Integral):
         integral = form
         integrand = integral.integrand()
         # Compute and apply integration scaling factor since we want to compute
         # coordinate derivatives at the end, the scaling factor has to be moved
@@ -103,15 +108,18 @@
                 new_degree = cur_degree + degree
         md["estimated_polynomial_degree"] = new_degree
 
         def scale_coordinate_derivative(o, scale):
             """Scale the coordinate derivative."""
             o_ = o.ufl_operands
             if isinstance(o, CoordinateDerivative):
-                return CoordinateDerivative(scale_coordinate_derivative(o_[0], scale), o_[1], o_[2], o_[3])
+                return CoordinateDerivative(
+                    scale_coordinate_derivative(o_[0], scale), o_[1], o_[2], o_[3]
+                )
             else:
                 return scale * o
+
         newintegrand = scale_coordinate_derivative(integrand, scale)
         return integral.reconstruct(integrand=newintegrand, metadata=md)
 
     else:
         raise ValueError(f"Invalid type {form.__class__.__name__}")
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/apply_restrictions.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/apply_restrictions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """Apply restrictions.
 
-This module contains the apply_restrictions algorithm which propagates restrictions in a form
-towards the terminals.
+This module contains the apply_restrictions algorithm which propagates
+restrictions in a form towards the terminals.
 """
 
 # Copyright (C) 2008-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
-
 from ufl.algorithms.map_integrands import map_integrand_dags
 from ufl.classes import Restricted
 from ufl.corealg.map_dag import map_expr_dag
 from ufl.corealg.multifunction import MultiFunction
 from ufl.domain import extract_unique_domain
 from ufl.measure import integral_type_to_measure_name
 from ufl.sobolevspace import H1
@@ -28,33 +27,36 @@
         MultiFunction.__init__(self)
         self.current_restriction = side
         self.default_restriction = "+"
         # Caches for propagating the restriction with map_expr_dag
         self.vcaches = {"+": {}, "-": {}}
         self.rcaches = {"+": {}, "-": {}}
         if self.current_restriction is None:
-            self._rp = {"+": RestrictionPropagator("+"),
-                        "-": RestrictionPropagator("-")}
+            self._rp = {"+": RestrictionPropagator("+"), "-": RestrictionPropagator("-")}
 
     def restricted(self, o):
         """When hitting a restricted quantity, visit child with a separate restriction algorithm."""
         # Assure that we have only two levels here, inside or outside
         # the Restricted node
         if self.current_restriction is not None:
             raise ValueError("Cannot restrict an expression twice.")
         # Configure a propagator for this side and apply to subtree
         side = o.side()
-        return map_expr_dag(self._rp[side], o.ufl_operands[0],
-                            vcache=self.vcaches[side],
-                            rcache=self.rcaches[side])
+        return map_expr_dag(
+            self._rp[side], o.ufl_operands[0], vcache=self.vcaches[side], rcache=self.rcaches[side]
+        )
 
     # --- Reusable rules
 
     def _ignore_restriction(self, o):
-        """Ignore current restriction, quantity is independent of side also from a computational point of view."""
+        """Ignore current restriction.
+
+        Quantity is independent of side also from a computational point
+        of view.
+        """
         return o
 
     def _require_restriction(self, o):
         """Restrict a discontinuous quantity to current side, require a side to be set."""
         if self.current_restriction is None:
             raise ValueError(f"Discontinuous type {o._ufl_class_.__name__} must be restricted.")
         return o(self.current_restriction)
@@ -95,15 +97,15 @@
 
     def variable(self, o, op, label):
         """Strip variable."""
         return op
 
     def reference_value(self, o):
         """Reference value of something follows same restriction rule as the underlying object."""
-        f, = o.ufl_operands
+        (f,) = o.ufl_operands
         assert f._ufl_is_terminal_
         g = self(f)
         if isinstance(g, Restricted):
             side = g.side()
             return o(side)
         else:
             return o
@@ -136,16 +138,16 @@
     # Assuming homogeoneous mesh
     reference_cell_volume = _ignore_restriction
     reference_facet_volume = _ignore_restriction
 
     def coefficient(self, o):
         """Restrict a coefficient.
 
-        Allow coefficients to be unrestricted (apply default if so) if the values are fully continuous
-        across the facet.
+        Allow coefficients to be unrestricted (apply default if so) if
+        the values are fully continuous across the facet.
         """
         if o.ufl_element() in H1:
             # If the coefficient _value_ is _fully_ continuous
             # It must still be computed from one of the sides, we just don't care which
             return self._default_restricted(o)
         else:
             return self._require_restriction(o)
@@ -153,15 +155,15 @@
     def facet_normal(self, o):
         """Restrict a facet_normal."""
         D = extract_unique_domain(o)
         e = D.ufl_coordinate_element()
         gd = D.geometric_dimension()
         td = D.topological_dimension()
 
-        if e._is_linear() and gd == td:
+        if e.embedded_superdegree <= 1 and e in H1 and gd == td:
             # For meshes with a continuous linear non-manifold
             # coordinate field, the facet normal from side - points in
             # the opposite direction of the one from side +.  We must
             # still require a side to be chosen by the user but
             # rewrite n- -> n+.  This is an optimization, possibly
             # premature, however it's more difficult to do at a later
             # stage.
@@ -170,32 +172,31 @@
             # For other meshes, we require a side to be
             # chosen by the user and respect that
             return self._require_restriction(o)
 
 
 def apply_restrictions(expression):
     """Propagate restriction nodes to wrap differential terminals directly."""
-    integral_types = [k for k in integral_type_to_measure_name.keys()
-                      if k.startswith("interior_facet")]
+    integral_types = [
+        k for k in integral_type_to_measure_name.keys() if k.startswith("interior_facet")
+    ]
     rules = RestrictionPropagator()
-    return map_integrand_dags(rules, expression,
-                              only_integral_type=integral_types)
+    return map_integrand_dags(rules, expression, only_integral_type=integral_types)
 
 
 class DefaultRestrictionApplier(MultiFunction):
     """Default restriction applier."""
 
     def __init__(self, side=None):
         """Initialise."""
         MultiFunction.__init__(self)
         self.current_restriction = side
         self.default_restriction = "+"
         if self.current_restriction is None:
-            self._rp = {"+": DefaultRestrictionApplier("+"),
-                        "-": DefaultRestrictionApplier("-")}
+            self._rp = {"+": DefaultRestrictionApplier("+"), "-": DefaultRestrictionApplier("-")}
 
     def terminal(self, o):
         """Apply to terminal."""
         # Most terminals are unchanged
         return o
 
     # Default: Operators should reconstruct only if subtrees are not touched
@@ -237,12 +238,12 @@
 
 
 def apply_default_restrictions(expression):
     """Some terminals can be restricted from either side.
 
     This applies a default restriction to such terminals if unrestricted.
     """
-    integral_types = [k for k in integral_type_to_measure_name.keys()
-                      if k.startswith("interior_facet")]
+    integral_types = [
+        k for k in integral_type_to_measure_name.keys() if k.startswith("interior_facet")
+    ]
     rules = DefaultRestrictionApplier()
-    return map_integrand_dags(rules, expression,
-                              only_integral_type=integral_types)
+    return map_integrand_dags(rules, expression, only_integral_type=integral_types)
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/balancing.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/balancing.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,28 +2,39 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2011-2017 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
-from ufl.classes import (CellAvg, FacetAvg, Grad, Indexed, NegativeRestricted,
-                         PositiveRestricted, ReferenceGrad, ReferenceValue)
+from ufl.classes import (
+    CellAvg,
+    FacetAvg,
+    Grad,
+    Indexed,
+    NegativeRestricted,
+    PositiveRestricted,
+    ReferenceGrad,
+    ReferenceValue,
+)
 from ufl.corealg.map_dag import map_expr_dag
 from ufl.corealg.multifunction import MultiFunction
 
 modifier_precedence = [
-    ReferenceValue, ReferenceGrad, Grad, CellAvg, FacetAvg, PositiveRestricted,
-    NegativeRestricted, Indexed
+    ReferenceValue,
+    ReferenceGrad,
+    Grad,
+    CellAvg,
+    FacetAvg,
+    PositiveRestricted,
+    NegativeRestricted,
+    Indexed,
 ]
 
-modifier_precedence = {
-    m._ufl_handler_name_: i
-    for i, m in enumerate(modifier_precedence)
-}
+modifier_precedence = {m._ufl_handler_name_: i for i, m in enumerate(modifier_precedence)}
 
 
 def balance_modified_terminal(expr):
     """Balance modified terminal."""
     # NB! Assuming e.g. grad(cell_avg(expr)) does not occur,
     # i.e. it is simplified to 0 immediately.
 
@@ -40,18 +51,17 @@
         assert expr._ufl_is_terminal_modifier_
         expr = expr.ufl_operands[0]
         layers.append(expr)
     assert layers[-1] is expr
     assert expr._ufl_is_terminal_
 
     # Apply modifiers in order
-    layers = sorted(
-        layers[:-1], key=lambda e: modifier_precedence[e._ufl_handler_name_])
+    layers = sorted(layers[:-1], key=lambda e: modifier_precedence[e._ufl_handler_name_])
     for op in layers:
-        ops = (expr, ) + op.ufl_operands[1:]
+        ops = (expr,) + op.ufl_operands[1:]
         expr = op._ufl_expr_reconstruct_(*ops)
 
     # Preserve id if nothing has changed
     return orig if expr == orig else expr
 
 
 class BalanceModifiers(MultiFunction):
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/change_to_reference.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/change_to_reference.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-"""Algorithm for replacing gradients in an expression with reference gradients and coordinate mappings."""
+"""Algorithm for replacing gradients in an expression."""
 
 # Copyright (C) 2008-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
-from ufl.core.multiindex import indices
-from ufl.corealg.multifunction import MultiFunction
-from ufl.corealg.map_dag import map_expr_dag
-
-from ufl.classes import ReferenceGrad, Grad, Restricted, ReferenceValue, JacobianInverse
-
-from ufl.tensors import as_tensor
-
 from ufl.algorithms.apply_function_pullbacks import apply_function_pullbacks
 from ufl.algorithms.apply_geometry_lowering import apply_geometry_lowering
 from ufl.checks import is_cellwise_constant
-
+from ufl.classes import Grad, JacobianInverse, ReferenceGrad, ReferenceValue, Restricted
+from ufl.core.multiindex import indices
+from ufl.corealg.map_dag import map_expr_dag
+from ufl.corealg.multifunction import MultiFunction
+from ufl.domain import extract_unique_domain
+from ufl.tensors import as_tensor
 
 """
 # Some notes:
-# Below, let v_i mean physical coordinate of vertex i and V_i mean the reference cell coordinate of the same vertex.
+# Below, let v_i mean physical coordinate of vertex i and V_i mean the
+reference cell coordinate of the same vertex.
 
 
-# Add a type for CellVertices? Note that vertices must be computed in linear cell cases!
-triangle_vertices[i,j] = component j of vertex i, following ufc numbering conventions
+# Add a type for CellVertices? Note that vertices must be computed in
+linear cell cases! triangle_vertices[i,j] = component j of vertex i,
+following ufc numbering conventions
 
 
-# DONE Add a type for CellEdgeLengths? Note that these are only easy to define in the linear cell case!
+# DONE Add a type for CellEdgeLengths? Note that these are only easy to
+define in the linear cell case!
 triangle_edge_lengths    = [v1v2, v0v2, v0v1] # shape (3,)
 tetrahedron_edge_lengths = [v0v1, v0v2, v0v3, v1v2, v1v3, v2v3] # shape (6,)
 
 
 # DONE Here's how to compute edge lengths from the Jacobian:
 J =[ [dx0/dX0, dx0/dX1],
      [dx1/dX0, dx1/dX1] ]
-# First compute the edge vector, which is constant for each edge: the vector from one vertex to the other
+# First compute the edge vector, which is constant for each edge: the
+vector from one vertex to the other
 reference_edge_vector_0 = V2 - V1 # Example! Add a type ReferenceEdgeVectors?
 # Then apply J to it and take the length of the resulting vector, this is generic for affine cells
 edge_length_i = || dot(J, reference_edge_vector_i) ||
 
 e2 = || J[:,0] . < 1, 0> || = || J[:,0] || = || dx/dX0 || = edge length of edge 2 (v0-v1)
 e1 = || J[:,1] . < 0, 1> || = || J[:,1] || = || dx/dX1 || = edge length of edge 1 (v0-v2)
 e0 = || J[:,:] . <-1, 1> || = || < J[0,1]-J[0,0], J[1,1]-J[1,0] > || = || dx/dX <-1,1> ||
@@ -120,44 +121,46 @@
         return o
 
     def grad(self, o):
         """Apply to grad."""
         # Peel off the Grads and count them, and get restriction if
         # it's between the grad and the terminal
         ngrads = 0
-        restricted = ''
+        restricted = ""
         rv = False
         while not o._ufl_is_terminal_:
             if isinstance(o, Grad):
-                o, = o.ufl_operands
+                (o,) = o.ufl_operands
                 ngrads += 1
             elif isinstance(o, Restricted):
                 restricted = o.side()
-                o, = o.ufl_operands
+                (o,) = o.ufl_operands
             elif isinstance(o, ReferenceValue):
                 rv = True
-                o, = o.ufl_operands
+                (o,) = o.ufl_operands
             else:
                 raise ValueError(f"Invalid type {o._ufl_class_.__name__}")
         f = o
         if rv:
             f = ReferenceValue(f)
 
         # Get domain and create Jacobian inverse object
-        domain = o.ufl_domain()
+        domain = extract_unique_domain(o)
         Jinv = JacobianInverse(domain)
 
         if is_cellwise_constant(Jinv):
             # Optimise slightly by turning Grad(Grad(...)) into
             # J^(-T)J^(-T)RefGrad(RefGrad(...))
             # rather than J^(-T)RefGrad(J^(-T)RefGrad(...))
 
             # Create some new indices
             ii = indices(len(f.ufl_shape))  # Indices to get to the scalar component of f
-            jj = indices(ngrads)  # Indices to sum over the local gradient axes with the inverse Jacobian
+            jj = indices(
+                ngrads
+            )  # Indices to sum over the local gradient axes with the inverse Jacobian
             kk = indices(ngrads)  # Indices for the leftover inverse Jacobian axes
 
             # Preserve restricted property
             if restricted:
                 Jinv = Jinv(restricted)
                 f = f(restricted)
 
@@ -181,15 +184,17 @@
             # Preserve restricted property
             if restricted:
                 Jinv = Jinv(restricted)
                 f = f(restricted)
 
             jinv_lgrad_f = f
             for foo in range(ngrads):
-                ii = indices(len(jinv_lgrad_f.ufl_shape))  # Indices to get to the scalar component of f
+                ii = indices(
+                    len(jinv_lgrad_f.ufl_shape)
+                )  # Indices to get to the scalar component of f
                 j, k = indices(2)
 
                 lgrad = ReferenceGrad(jinv_lgrad_f)
                 jinv_lgrad_f = Jinv[j, k] * lgrad[ii + (j,)]
 
                 # Wrap back in tensor shape, derivative axes at the end
                 jinv_lgrad_f = as_tensor(jinv_lgrad_f, ii + (k,))
@@ -198,21 +203,24 @@
 
     def reference_grad(self, o):
         """Apply to reference_grad."""
         raise ValueError("Not expecting reference grad while applying change to reference grad.")
 
     def coefficient_derivative(self, o):
         """Apply to coefficient_derivative."""
-        raise ValueError("Coefficient derivatives should be expanded before applying change to reference grad.")
+        raise ValueError(
+            "Coefficient derivatives should be expanded before applying change to reference grad."
+        )
 
 
 def change_to_reference_grad(e):
     """Change Grad objects in expression to products of JacobianInverse and ReferenceGrad.
 
-    Assumes the expression is preprocessed or at least that derivatives have been expanded.
+    Assumes the expression is preprocessed or at least that derivatives
+    have been expanded.
 
     Args:
         e: An Expr or Form.
     """
     mf = ChangeToReferenceGrad()
     return map_expr_dag(mf, e)
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/check_arities.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/check_arities.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Check arities."""
+
 from itertools import chain
 
-from ufl.corealg.traversal import traverse_unique_terminals
-from ufl.corealg.multifunction import MultiFunction
-from ufl.corealg.map_dag import map_expr_dag
 from ufl.classes import Argument, Zero
+from ufl.corealg.map_dag import map_expr_dag
+from ufl.corealg.multifunction import MultiFunction
+from ufl.corealg.traversal import traverse_unique_terminals
 
 
 class ArityMismatch(BaseException):
     """Arity mismatch exception."""
+
     pass
 
 
 def _afmt(atuple):
     """Return a string representation of an arity tuple."""
     return tuple(f"conj({arg})" if conj else str(arg) for arg, conj in atuple)
 
@@ -37,24 +39,28 @@
     def nonlinear_operator(self, o):
         """Apply to nonlinear_operator."""
         # Cutoff traversal by not having *ops in argument list of this
         # handler.  Traverse only the terminals under here the fastest
         # way we know of:
         for t in traverse_unique_terminals(o):
             if t._ufl_typecode_ == Argument._ufl_typecode_:
-                raise ArityMismatch(f"Applying nonlinear operator {o._ufl_class_.__name__} to "
-                                    f"expression depending on form argument {t}.")
+                raise ArityMismatch(
+                    f"Applying nonlinear operator {o._ufl_class_.__name__} to "
+                    f"expression depending on form argument {t}."
+                )
         return self._et
 
     expr = nonlinear_operator
 
     def sum(self, o, a, b):
         """Apply to sum."""
         if a != b:
-            raise ArityMismatch(f"Adding expressions with non-matching form arguments {_afmt(a)} vs {_afmt(b)}.")
+            raise ArityMismatch(
+                f"Adding expressions with non-matching form arguments {_afmt(a)} vs {_afmt(b)}."
+            )
         return a
 
     def division(self, o, a, b):
         """Apply to division."""
         if b:
             raise ArityMismatch(f"Cannot divide by form argument {b}.")
         return a
@@ -63,23 +69,27 @@
         """Apply to product."""
         if a and b:
             # Check that we don't have test*test, trial*trial, even
             # for different parts in a block system
             anumbers = set(x[0].number() for x in a)
             for x in b:
                 if x[0].number() in anumbers:
-                    raise ArityMismatch("Multiplying expressions with overlapping form argument number "
-                                        f"{x[0].number()}, argument is {_afmt(x)}.")
+                    raise ArityMismatch(
+                        "Multiplying expressions with overlapping form argument number "
+                        f"{x[0].number()}, argument is {_afmt(x)}."
+                    )
             # Combine argument lists
             c = tuple(sorted(set(a + b), key=lambda x: (x[0].number(), x[0].part())))
             # Check that we don't have any arguments shared between a
             # and b
             if len(c) != len(a) + len(b) or len(c) != len({x[0] for x in c}):
-                raise ArityMismatch("Multiplying expressions with overlapping form arguments "
-                                    f"{_afmt(a)} vs {_afmt(b)}.")
+                raise ArityMismatch(
+                    "Multiplying expressions with overlapping form arguments "
+                    f"{_afmt(a)} vs {_afmt(b)}."
+                )
             # It's fine for argument parts to overlap
             return c
         elif a:
             return a
         else:
             return b
 
@@ -135,16 +145,18 @@
             return b
         elif a == b:
             # Allow conditional(c, test, test)
             return a
         else:
             # Do not allow e.g. conditional(c, test, trial),
             # conditional(c, test, nonzeroconstant)
-            raise ArityMismatch("Conditional subexpressions with non-matching form arguments "
-                                f"{_afmt(a)} vs {_afmt(b)}.")
+            raise ArityMismatch(
+                "Conditional subexpressions with non-matching form arguments "
+                f"{_afmt(a)} vs {_afmt(b)}."
+            )
 
     def linear_indexed_type(self, o, a, i):
         """Apply to linear_indexed_type."""
         return a
 
     # All of these indexed thingies behave as a linear_indexed_type
     indexed = linear_indexed_type
@@ -157,28 +169,29 @@
         if args:
             # Check that each list tensor component has the same
             # argument numbers (ignoring parts)
             numbers = set(tuple(sorted(set(arg[0].number() for arg in op))) for op in ops)
             if () in numbers:  # Allow e.g. <v[0], 0, v[1]> but not <v[0], u[0]>
                 numbers.remove(())
             if len(numbers) > 1:
-                raise ArityMismatch("Listtensor components must depend on the same argument numbers, "
-                                    f"found {numbers}.")
+                raise ArityMismatch(
+                    "Listtensor components must depend on the same argument numbers, "
+                    f"found {numbers}."
+                )
 
             # Allow different parts with the same number
             return tuple(sorted(args, key=lambda x: (x[0].number(), x[0].part())))
         else:
             # No argument dependencies
             return self._et
 
 
 def check_integrand_arity(expr, arguments, complex_mode=False):
     """Check the arity of an integrand."""
-    arguments = tuple(sorted(set(arguments),
-                             key=lambda x: (x.number(), x.part())))
+    arguments = tuple(sorted(set(arguments), key=lambda x: (x.number(), x.part())))
     rules = ArityChecker(arguments)
     arg_tuples = map_expr_dag(rules, expr, compress=False)
     args = tuple(a[0] for a in arg_tuples)
     if args != arguments:
         raise ArityMismatch(f"Integrand arguments {args} differ from form arguments {arguments}.")
     if complex_mode:
         # Check that the test function is conjugated and that any
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/check_restrictions.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/check_restrictions.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 # Copyright (C) 2008-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
-from ufl.corealg.multifunction import MultiFunction
 from ufl.corealg.map_dag import map_expr_dag
+from ufl.corealg.multifunction import MultiFunction
 
 
 class RestrictionChecker(MultiFunction):
     """Restiction checker."""
 
     def __init__(self, require_restriction):
         """Initialise."""
@@ -24,15 +24,15 @@
         pass
 
     def restricted(self, o):
         """Apply to restricted."""
         if self.current_restriction is not None:
             raise ValueError("Not expecting twice restricted expression.")
         self.current_restriction = o._side
-        e, = o.ufl_operands
+        (e,) = o.ufl_operands
         self.visit(e)
         self.current_restriction = None
 
     def facet_normal(self, o):
         """Apply to facet_normal."""
         if self.require_restriction:
             if self.current_restriction is None:
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/checks.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/checks.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,46 +5,51 @@
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Anders Logg, 2008-2009.
 # Modified by Mehdi Nikbakht, 2010.
 
-# UFL classes
-from ufl.core.expr import ufl_err_str
-from ufl.form import Form
+from ufl.algorithms.check_restrictions import check_restrictions
+
+# UFL algorithms
+from ufl.algorithms.traversal import iter_expressions
 from ufl.argument import Argument
 from ufl.coefficient import Coefficient
 from ufl.constantvalue import is_true_ufl_scalar
 
-# UFL algorithms
-from ufl.algorithms.traversal import iter_expressions
+# UFL classes
+from ufl.core.expr import ufl_err_str
 from ufl.corealg.traversal import traverse_unique_terminals
-from ufl.algorithms.check_restrictions import check_restrictions
 from ufl.domain import extract_unique_domain
+from ufl.form import Form
 
 
-def validate_form(form):  # TODO: Can we make this return a list of errors instead of raising exception?
+def validate_form(
+    form,
+):  # TODO: Can we make this return a list of errors instead of raising exception?
     """Performs all implemented validations on a form. Raises exception if something fails."""
     errors = []
 
     if not isinstance(form, Form):
         raise ValueError(f"Validation failed, not a Form:\n{ufl_err_str(form)}")
 
     # FIXME: There's a bunch of other checks we should do here.
 
     # FIXME: Add back check for multilinearity
     # Check that form is multilinear
     # if not is_multilinear(form):
     #     errors.append("Form is not multilinear in arguments.")
 
     # FIXME DOMAIN: Add check for consistency between domains somehow
-    domains = set(extract_unique_domain(t)
-                  for e in iter_expressions(form)
-                  for t in traverse_unique_terminals(e)) - {None}
+    domains = set(
+        extract_unique_domain(t)
+        for e in iter_expressions(form)
+        for t in traverse_unique_terminals(e)
+    ) - {None}
     if not domains:
         errors.append("Missing domain definition in form.")
 
     # Check that cell is the same everywhere
     cells = set(dom.ufl_cell() for dom in domains) - {None}
     if not cells:
         errors.append("Missing cell definition in form.")
@@ -58,16 +63,15 @@
     for e in iter_expressions(form):
         for f in traverse_unique_terminals(e):
             if isinstance(f, Coefficient):
                 c = f.count()
                 if c in coefficients:
                     g = coefficients[c]
                     if f is not g:
-                        errors.append("Found different Coefficients with "
-                                      f"same count: {f} and {g}.")
+                        errors.append(f"Found different Coefficients with same count: {f} and {g}.")
                 else:
                     coefficients[c] = f
 
             elif isinstance(f, Argument):
                 n = f.number()
                 p = f.part()
                 if (n, p) in arguments:
@@ -98,8 +102,8 @@
         else:
             check_restrictions(integral.integrand(), False)
 
     # Raise exception with all error messages
     # TODO: Return errors list instead, need to collect messages from
     # all validations above first.
     if errors:
-        raise ValueError("Found errors in validation of form:\n" + '\n\n'.join(errors))
+        raise ValueError("Found errors in validation of form:\n" + "\n\n".join(errors))
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/comparison_checker.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/comparison_checker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Algorithm to check for 'comparison' nodes in a form when the user is in 'complex mode'."""
 
-from ufl.corealg.multifunction import MultiFunction
-from ufl.algorithms.map_integrands import map_integrand_dags
 from ufl.algebra import Real
-from ufl.constantvalue import RealValue, Zero
+from ufl.algorithms.map_integrands import map_integrand_dags
 from ufl.argument import Argument
+from ufl.constantvalue import RealValue, Zero
+from ufl.corealg.multifunction import MultiFunction
 from ufl.geometry import GeometricQuantity
 
 
 class CheckComparisons(MultiFunction):
     """Raises an error if comparisons are done with complex quantities.
 
     If quantities are real, adds the Real operator to the compared quantities.
@@ -79,57 +79,57 @@
             o = o._ufl_expr_reconstruct_(*map(Real, ops))
             self.nodetype[o] = "bool"
             return o
 
     def real(self, o, *ops):
         """Apply to real."""
         o = self.reuse_if_untouched(o, *ops)
-        self.nodetype[o] = 'real'
+        self.nodetype[o] = "real"
         return o
 
     def imag(self, o, *ops):
         """Apply to imag."""
         o = self.reuse_if_untouched(o, *ops)
-        self.nodetype[o] = 'real'
+        self.nodetype[o] = "real"
         return o
 
     def sqrt(self, o, *ops):
         """Apply to sqrt."""
         o = self.reuse_if_untouched(o, *ops)
-        self.nodetype[o] = 'complex'
+        self.nodetype[o] = "complex"
         return o
 
     def power(self, o, base, exponent):
         """Apply to power."""
         o = self.reuse_if_untouched(o, base, exponent)
         try:
             # Attempt to diagnose circumstances in which the result must be real.
             exponent = float(exponent)
-            if self.nodetype[base] == 'real' and int(exponent) == exponent:
-                self.nodetype[o] = 'real'
+            if self.nodetype[base] == "real" and int(exponent) == exponent:
+                self.nodetype[o] = "real"
                 return o
         except TypeError:
             pass
 
-        self.nodetype[o] = 'complex'
+        self.nodetype[o] = "complex"
         return o
 
     def abs(self, o, *ops):
         """Apply to abs."""
         o = self.reuse_if_untouched(o, *ops)
-        self.nodetype[o] = 'real'
+        self.nodetype[o] = "real"
         return o
 
     def terminal(self, term, *ops):
         """Apply to terminal."""
         # default terminals to complex, except the ones we *know* are real
         if isinstance(term, (RealValue, Zero, Argument, GeometricQuantity)):
-            self.nodetype[term] = 'real'
+            self.nodetype[term] = "real"
         else:
-            self.nodetype[term] = 'complex'
+            self.nodetype[term] = "complex"
         return term
 
     def indexed(self, o, expr, multiindex):
         """Apply to indexed."""
         o = self.reuse_if_untouched(o, expr, multiindex)
         self.nodetype[o] = self.nodetype[expr]
         return o
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/compute_form_data.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/compute_form_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,94 +1,95 @@
 """This module provides the compute_form_data function.
 
-Form compilers will typically call compute_form_dataprior to code generation to preprocess/simplify a
-raw input form given by a user.
+Form compilers will typically call compute_form_dataprior to code
+generation to preprocess/simplify a raw input form given by a user.
 """
 # Copyright (C) 2008-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
 from itertools import chain
 
-from ufl.utils.sequences import max_degree
-
-from ufl.classes import GeometricFacetQuantity, Coefficient, Form, FunctionSpace
-from ufl.corealg.traversal import traverse_unique_terminals
 from ufl.algorithms.analysis import extract_coefficients, extract_sub_elements, unique_tuple
-from ufl.algorithms.formdata import FormData
-from ufl.algorithms.formtransformations import compute_form_arities
-from ufl.algorithms.check_arities import check_form_arity
+from ufl.algorithms.apply_algebra_lowering import apply_algebra_lowering
+from ufl.algorithms.apply_derivatives import apply_coordinate_derivatives, apply_derivatives
 
 # These are the main symbolic processing steps:
 from ufl.algorithms.apply_function_pullbacks import apply_function_pullbacks
-from ufl.algorithms.apply_algebra_lowering import apply_algebra_lowering
-from ufl.algorithms.apply_derivatives import apply_derivatives, apply_coordinate_derivatives
-from ufl.algorithms.apply_integral_scaling import apply_integral_scaling
 from ufl.algorithms.apply_geometry_lowering import apply_geometry_lowering
-from ufl.algorithms.apply_restrictions import apply_restrictions, apply_default_restrictions
-from ufl.algorithms.estimate_degrees import estimate_total_polynomial_degree
-from ufl.algorithms.remove_complex_nodes import remove_complex_nodes
+from ufl.algorithms.apply_integral_scaling import apply_integral_scaling
+from ufl.algorithms.apply_restrictions import apply_default_restrictions, apply_restrictions
+from ufl.algorithms.check_arities import check_form_arity
 from ufl.algorithms.comparison_checker import do_comparison_check
 
 # See TODOs at the call sites of these below:
-from ufl.algorithms.domain_analysis import build_integral_data
-from ufl.algorithms.domain_analysis import reconstruct_form_from_integral_data
-from ufl.algorithms.domain_analysis import group_form_integrals
+from ufl.algorithms.domain_analysis import (
+    build_integral_data,
+    group_form_integrals,
+    reconstruct_form_from_integral_data,
+)
+from ufl.algorithms.estimate_degrees import estimate_total_polynomial_degree
+from ufl.algorithms.formdata import FormData
+from ufl.algorithms.formtransformations import compute_form_arities
+from ufl.algorithms.remove_complex_nodes import remove_complex_nodes
+from ufl.classes import Coefficient, Form, FunctionSpace, GeometricFacetQuantity
+from ufl.corealg.traversal import traverse_unique_terminals
+from ufl.domain import extract_unique_domain
+from ufl.utils.sequences import max_degree
 
 
 def _auto_select_degree(elements):
     """Automatically select degree for all elements of the form.
 
     This is be used in cases where the degree has not been specified by the user.
     This feature is used by DOLFIN to allow the specification of Expressions with
     undefined degrees.
     """
     # Use max degree of all elements, at least 1 (to work with
     # Lagrange elements)
-    return max_degree({e.degree() for e in elements} - {None} | {1})
+    return max_degree({e.embedded_superdegree for e in elements} - {None} | {1})
 
 
 def _compute_element_mapping(form):
     """Compute element mapping for element replacement."""
     # The element mapping is a slightly messy concept with two use
     # cases:
     # - Expression with missing cell or element TODO: Implement proper
     #   Expression handling in UFL and get rid of this
     # - Constant with missing cell TODO: Fix anything that needs to be
     #   worked around to drop this requirement
 
     # Extract all elements and include subelements of mixed elements
-    elements = [obj.ufl_element() for obj in chain(form.arguments(),
-                                                   form.coefficients())]
+    elements = [obj.ufl_element() for obj in chain(form.arguments(), form.coefficients())]
     elements = extract_sub_elements(elements)
 
     # Try to find a common degree for elements
     common_degree = _auto_select_degree(elements)
 
     # Compute element map
     element_mapping = {}
     for element in elements:
-
         # Flag for whether element needs to be reconstructed
         reconstruct = False
 
         # Set cell
-        cell = element.cell()
+        cell = element.cell
         if cell is None:
             domains = form.ufl_domains()
-            if not all(domains[0].ufl_cell() == d.ufl_cell()
-                       for d in domains):
-                raise ValueError("Cannot replace unknown element cell without unique common cell in form.")
+            if not all(domains[0].ufl_cell() == d.ufl_cell() for d in domains):
+                raise ValueError(
+                    "Cannot replace unknown element cell without unique common cell in form."
+                )
             cell = domains[0].ufl_cell()
             reconstruct = True
 
         # Set degree
-        degree = element.degree()
+        degree = element.embedded_superdegree
         if degree is None:
             degree = common_degree
             reconstruct = True
 
         # Reconstruct element and add to map
         if reconstruct:
             element_mapping[element] = element.reconstruct(cell=cell, degree=degree)
@@ -132,17 +133,16 @@
 
     self.unique_elements = unique_tuple(all_elements)
     self.unique_sub_elements = unique_tuple(all_sub_elements)
 
 
 def _check_elements(form_data):
     """Check elements."""
-    for element in chain(form_data.unique_elements,
-                         form_data.unique_sub_elements):
-        if element.cell() is None:
+    for element in chain(form_data.unique_elements, form_data.unique_sub_elements):
+        if element.cell is None:
             raise ValueError(f"Found element with undefined cell: {element}")
 
 
 def _check_facet_geometry(integral_data):
     """Check facet geometry."""
     for itg_data in integral_data:
         for itg in itg_data.integrals:
@@ -180,16 +180,17 @@
     for i, f in enumerate(coefficients):
         old_e = f.ufl_element()
         new_e = element_mapping.get(old_e, old_e)
         # XXX: This is a hack to ensure that if the original
         # coefficient had a domain, the new one does too.
         # This should be overhauled with requirement that Expressions
         # always have a domain.
-        if f.ufl_domain() is not None:
-            new_e = FunctionSpace(f.ufl_domain(), new_e)
+        domain = extract_unique_domain(f)
+        if domain is not None:
+            new_e = FunctionSpace(domain, new_e)
         new_f = Coefficient(new_e, count=i)
         new_coefficients.append(new_f)
         replace_map[f] = new_f
 
     return new_coefficients, replace_map
 
 
@@ -242,18 +243,23 @@
     # user-defined coefficient relations it just gets too messy
     form = apply_derivatives(form)
 
     return form
 
 
 def compute_form_data(
-    form, do_apply_function_pullbacks=False, do_apply_integral_scaling=False,
-    do_apply_geometry_lowering=False, preserve_geometry_types=(),
-    do_apply_default_restrictions=True, do_apply_restrictions=True,
-    do_estimate_degrees=True, do_append_everywhere_integrals=True,
+    form,
+    do_apply_function_pullbacks=False,
+    do_apply_integral_scaling=False,
+    do_apply_geometry_lowering=False,
+    preserve_geometry_types=(),
+    do_apply_default_restrictions=True,
+    do_apply_restrictions=True,
+    do_estimate_degrees=True,
+    do_append_everywhere_integrals=True,
     complex_mode=False,
 ):
     """Compute form data.
 
     The default arguments configured to behave the way old FFC expects.
     """
     # TODO: Move this to the constructor instead
@@ -271,16 +277,19 @@
 
     form = preprocess_form(form, complex_mode)
 
     # --- Group form integrals
     # TODO: Refactor this, it's rather opaque what this does
     # TODO: Is self.original_form.ufl_domains() right here?
     #       It will matter when we start including 'num_domains' in ufc form.
-    form = group_form_integrals(form, self.original_form.ufl_domains(),
-                                do_append_everywhere_integrals=do_append_everywhere_integrals)
+    form = group_form_integrals(
+        form,
+        self.original_form.ufl_domains(),
+        do_append_everywhere_integrals=do_append_everywhere_integrals,
+    )
 
     # Estimate polynomial degree of integrands now, before applying
     # any pullbacks and geometric lowering.  Otherwise quad degrees
     # blow up horrifically.
     if do_estimate_degrees:
         form = attach_estimated_degrees(form)
 
@@ -348,25 +357,26 @@
 
     # Figure out which coefficients from the original form are
     # actually used in any integral (Differentiation may reduce the
     # set of coefficients w.r.t. the original form)
     reduced_coefficients_set = set()
     for itg_data in self.integral_data:
         reduced_coefficients_set.update(itg_data.integral_coefficients)
-    self.reduced_coefficients = sorted(reduced_coefficients_set,
-                                       key=lambda c: c.count())
+    self.reduced_coefficients = sorted(reduced_coefficients_set, key=lambda c: c.count())
     self.num_coefficients = len(self.reduced_coefficients)
-    self.original_coefficient_positions = [i for i, c in enumerate(self.original_form.coefficients())
-                                           if c in self.reduced_coefficients]
+    self.original_coefficient_positions = [
+        i for i, c in enumerate(self.original_form.coefficients()) if c in self.reduced_coefficients
+    ]
 
     # Store back into integral data which form coefficients are used
     # by each integral
     for itg_data in self.integral_data:
-        itg_data.enabled_coefficients = [bool(coeff in itg_data.integral_coefficients)
-                                         for coeff in self.reduced_coefficients]
+        itg_data.enabled_coefficients = [
+            bool(coeff in itg_data.integral_coefficients) for coeff in self.reduced_coefficients
+        ]
 
     # --- Collect some trivial data
 
     # Get rank of form from argument list (assuming not a mixed arity form)
     self.rank = len(self.original_form.arguments())
 
     # Extract common geometric dimension (topological is not common!)
@@ -382,25 +392,27 @@
     # Expression-like functions that can be evaluated in quadrature
     # points.
     self.element_replace_map = _compute_element_mapping(self.original_form)
 
     # Mappings from elements and coefficients that reside in form to
     # objects with canonical numbering as well as completed cells and
     # elements
-    renumbered_coefficients, function_replace_map = \
-        _build_coefficient_replace_map(self.reduced_coefficients,
-                                       self.element_replace_map)
+    renumbered_coefficients, function_replace_map = _build_coefficient_replace_map(
+        self.reduced_coefficients, self.element_replace_map
+    )
     self.function_replace_map = function_replace_map
 
     # --- Store various lists of elements and sub elements (adds
     #     members to self)
-    _compute_form_data_elements(self,
-                                self.original_form.arguments(),
-                                renumbered_coefficients,
-                                self.original_form.ufl_domains())
+    _compute_form_data_elements(
+        self,
+        self.original_form.arguments(),
+        renumbered_coefficients,
+        self.original_form.ufl_domains(),
+    )
 
     # --- Store number of domains for integral types
     # TODO: Group this by domain first. For now keep a backwards
     # compatible data structure.
     self.max_subdomain_ids = _compute_max_subdomain_ids(self.integral_data)
 
     # --- Checks
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/coordinate_derivative_helpers.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/coordinate_derivative_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""This module provides the necessary tools to strip away and reattach coordinate derivatives.
+"""Tools to strip away and reattach coordinate derivatives.
 
 This is used in compute_form_data.
 """
 
 # Copyright (C) 2018 Florian Wechsung
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
-from ufl.differentiation import CoordinateDerivative
-from ufl.corealg.multifunction import MultiFunction
-from ufl.corealg.map_dag import map_expr_dags
 from ufl.classes import Integral
+from ufl.corealg.map_dag import map_expr_dags
+from ufl.corealg.multifunction import MultiFunction
+from ufl.differentiation import CoordinateDerivative
 
 
 class CoordinateDerivativeIsOutermostChecker(MultiFunction):
     """Traverses the tree to make sure that CoordinateDerivatives are only on the outside.
 
     The visitor returns False as long as no CoordinateDerivative has been seen.
     """
@@ -60,15 +60,18 @@
         integral = integrals
         integrand = integral.integrand()
         checker = CoordinateDerivativeIsOutermostChecker()
         map_expr_dags(checker, [integrand])
         coordinate_derivatives = []
 
         def take_top_coordinate_derivatives(o):
-            """Grab all coordinate derivatives and store them, so that we can apply them later again."""
+            """Get all coordinate derivatives and store them.
+
+            So we can apply them later again.
+            """
             o_ = o.ufl_operands
             if isinstance(o, CoordinateDerivative):
                 coordinate_derivatives.append((o_[1], o_[2], o_[3]))
                 return take_top_coordinate_derivatives(o_[0])
             else:
                 return o
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/domain_analysis.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/domain_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,42 +2,49 @@
 
 # Copyright (C) 2009-2016 Anders Logg and Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
+import numbers
+import typing
 from collections import defaultdict
 
 import ufl
-from ufl.integral import Integral
+from ufl.algorithms.coordinate_derivative_helpers import (
+    attach_coordinate_derivatives,
+    strip_coordinate_derivatives,
+)
 from ufl.form import Form
+from ufl.integral import Integral
 from ufl.protocols import id_or_none
 from ufl.sorting import cmp_expr, sorted_expr
 from ufl.utils.sorting import canonicalize_metadata, sorted_by_key
-from ufl.algorithms.coordinate_derivative_helpers import (
-    attach_coordinate_derivatives, strip_coordinate_derivatives)
-import numbers
-import typing
 
 
 class IntegralData(object):
     """Utility class.
 
-    This class has members (domain, integral_type, subdomain_id, integrals, metadata),
-    where metadata is an empty dictionary that may be used for
-    associating metadata with each object.
+    This class has members (domain, integral_type, subdomain_id,
+    integrals, metadata), where metadata is an empty dictionary that may
+    be used for associating metadata with each object.
     """
-    __slots__ = ('domain', 'integral_type', 'subdomain_id',
-                 'integrals', 'metadata',
-                 'integral_coefficients',
-                 'enabled_coefficients')
 
-    def __init__(self, domain, integral_type, subdomain_id, integrals,
-                 metadata):
+    __slots__ = (
+        "domain",
+        "integral_type",
+        "subdomain_id",
+        "integrals",
+        "metadata",
+        "integral_coefficients",
+        "enabled_coefficients",
+    )
+
+    def __init__(self, domain, integral_type, subdomain_id, integrals, metadata):
         """Initialise."""
         if 1 != len(set(itg.ufl_domain() for itg in integrals)):
             raise ValueError("Multiple domains mismatch in integral data.")
         if not all(integral_type == itg.integral_type() for itg in integrals):
             raise ValueError("Integral type mismatch in integral data.")
         if not all(subdomain_id == itg.subdomain_id() for itg in integrals):
             raise ValueError("Subdomain id mismatch in integral data.")
@@ -56,37 +63,44 @@
         # TODO: I think we can get rid of this with some refactoring
         # in ffc:
         self.metadata = metadata
 
     def __lt__(self, other):
         """Check if self is less than other."""
         # To preserve behaviour of extract_integral_data:
-        return (
-            self.integral_type, self.subdomain_id, self.integrals, self.metadata
-        ) < (
-            other.integral_type, other.subdomain_id, other.integrals, other.metadata
+        return (self.integral_type, self.subdomain_id, self.integrals, self.metadata) < (
+            other.integral_type,
+            other.subdomain_id,
+            other.integrals,
+            other.metadata,
         )
 
     def __eq__(self, other):
         """Check for equality."""
         # Currently only used for tests:
-        return (self.integral_type == other.integral_type and self.subdomain_id == other.subdomain_id and  # noqa: W504
-                self.integrals == other.integrals and self.metadata == other.metadata)
+        return (
+            self.integral_type == other.integral_type
+            and self.subdomain_id == other.subdomain_id
+            and self.integrals == other.integrals
+            and self.metadata == other.metadata
+        )
 
     def __str__(self):
         """Format as a string."""
-        s = f"IntegralData over domain({self.integral_type}, {self.subdomain_id}), with integrals:\n"
+        s = f"IntegralData over domain({self.integral_type}, {self.subdomain_id})"
+        s += " with integrals:\n"
         s += "\n\n".join(map(str, self.integrals))
         s += "\nand metadata:\n{metadata}"
         return s
 
 
 class ExprTupleKey(object):
     """Tuple comparison helper."""
-    __slots__ = ('x',)
+
+    __slots__ = ("x",)
 
     def __init__(self, x):
         """Initialise."""
         self.x = x
 
     def __lt__(self, other):
         """Check if self is less than other."""
@@ -138,22 +152,22 @@
         # TODO: Define list of valid strings somewhere more central
         return did
     else:
         raise ValueError(f"Invalid domain id {did}.")
 
 
 def rearrange_integrals_by_single_subdomains(
-    integrals: typing.List[Integral],
-    do_append_everywhere_integrals: bool
+    integrals: typing.List[Integral], do_append_everywhere_integrals: bool
 ) -> typing.Dict[int, typing.List[Integral]]:
     """Rearrange integrals over multiple subdomains to single subdomain integrals.
 
     Args:
         integrals: List of integrals
-        do_append_everywhere_integrals: Boolean indicating if integrals defined on the whole domain should
+        do_append_everywhere_integrals: Boolean indicating if integrals
+        defined on the whole domain should
             just be restricted to the set of input subdomain ids.
 
     Returns:
         The integrals reconstructed with single subdomain_id
     """
     # Split integrals into lists of everywhere and subdomain integrals
     everywhere_integrals = []
@@ -185,31 +199,33 @@
         otherwise_integrals.append(ev_itg.reconstruct(subdomain_id="otherwise"))
 
         # Restrict everywhere integral to each subdomain
         # and append to each integral list
         if do_append_everywhere_integrals:
             for subdomain_id in sorted(single_subdomain_integrals.keys()):
                 single_subdomain_integrals[subdomain_id].append(
-                    ev_itg.reconstruct(subdomain_id=subdomain_id))
+                    ev_itg.reconstruct(subdomain_id=subdomain_id)
+                )
 
     if otherwise_integrals:
         single_subdomain_integrals["otherwise"] = otherwise_integrals
 
     return single_subdomain_integrals
 
 
 def accumulate_integrands_with_same_metadata(integrals):
     """Accumulate integrands with the same metedata.
 
     Args:
         integrals: a list of integrals
 
     Returns:
-        A list of the form [(integrand0, metadata0), (integrand1, metadata1), ...]
-        where integrand0 < integrand1 by the canonical ufl expression ordering criteria.
+        A list of the form [(integrand0, metadata0), (integrand1,
+        metadata1), ...] where integrand0 < integrand1 by the canonical
+        ufl expression ordering criteria.
     """
     # Group integrals by compiler data hash
     by_cdid = {}
     for itg in integrals:
         cd = itg.metadata()
         cdid = hash(canonicalize_metadata(cd))
         if cdid not in by_cdid:
@@ -253,46 +269,59 @@
         integral_type = integral.integral_type()
         ufl_domain = integral.ufl_domain()
         metadata = integral.metadata()
         meta_hash = hash(canonicalize_metadata(metadata))
         subdomain_id = integral.subdomain_id()
         subdomain_data = id_or_none(integral.subdomain_data())
         if subdomain_id == "everywhere":
-            raise ValueError("'everywhere' not a valid subdomain id.  Did you forget to call group_form_integrals?")
-        unique_integrals[(integral_type, ufl_domain, meta_hash, integrand, subdomain_data)] += (subdomain_id,)
+            raise ValueError(
+                "'everywhere' not a valid subdomain id. "
+                "Did you forget to call group_form_integrals?"
+            )
+        unique_integrals[(integral_type, ufl_domain, meta_hash, integrand, subdomain_data)] += (
+            subdomain_id,
+        )
         metadata_table[(integral_type, ufl_domain, meta_hash, integrand, subdomain_data)] = metadata
 
     for integral_data, subdomain_ids in unique_integrals.items():
         (integral_type, ufl_domain, metadata, integrand, subdomain_data) = integral_data
 
-        integral = Integral(integrand, integral_type, ufl_domain, subdomain_ids,
-                            metadata_table[integral_data], subdomain_data)
+        integral = Integral(
+            integrand,
+            integral_type,
+            ufl_domain,
+            subdomain_ids,
+            metadata_table[integral_data],
+            subdomain_data,
+        )
         # Group for integral data (One integral data object for all
         # integrals with same domain, itype, (but possibly different metadata).
         itgs[(ufl_domain, integral_type, subdomain_ids)].append(integral)
 
     # Build list with canonical ordering, iteration over dicts
     # is not deterministic across python versions
     def keyfunc(item):
         (d, itype, sid), integrals = item
         sid_int = tuple(-1 if i == "otherwise" else i for i in sid)
-        return (d._ufl_sort_key_(), itype, (type(sid).__name__, ), sid_int)
+        return (d._ufl_sort_key_(), itype, (type(sid).__name__,), sid_int)
+
     integral_datas = []
     for (d, itype, sid), integrals in sorted(itgs.items(), key=keyfunc):
         integral_datas.append(IntegralData(d, itype, sid, integrals, {}))
     return integral_datas
 
 
 def group_form_integrals(form, domains, do_append_everywhere_integrals=True):
     """Group integrals by domain and type, performing canonical simplification.
 
     Args:
         form: the Form to group the integrals of.
         domains: an iterable of Domains.
-        do_append_everywhere_integrals: Boolean indicating if integrals defined on the whole domain should
+        do_append_everywhere_integrals: Boolean indicating if integrals
+        defined on the whole domain should
             just be restricted to the set of input subdomain ids.
 
     Returns:
         A new Form with gathered integrands.
     """
     # Group integrals by domain and type
     integrals_by_domain_and_type = group_integrals_by_domain_and_type(form.integrals(), domains)
@@ -306,48 +335,53 @@
                 continue
 
             # Group integrals by subdomain id, after splitting e.g.
             #   f*dx((1,2)) + g*dx((2,3)) -> f*dx(1) + (f+g)*dx(2) + g*dx(3)
             # (note: before this call, 'everywhere' is a valid subdomain_id,
             # and after this call, 'otherwise' is a valid subdomain_id)
             single_subdomain_integrals = rearrange_integrals_by_single_subdomains(
-                ddt_integrals, do_append_everywhere_integrals)
+                ddt_integrals, do_append_everywhere_integrals
+            )
 
             for subdomain_id, ss_integrals in sorted_by_key(single_subdomain_integrals):
-
                 # strip the coordinate derivatives from all integrals
                 # this yields a list of the form [(coordinate derivative, integral), ...]
                 stripped_integrals_and_coordderivs = strip_coordinate_derivatives(ss_integrals)
 
                 # now group the integrals by the coordinate derivative
                 def calc_hash(cd):
-                    return sum(sum(tuple_elem._ufl_compute_hash_()
-                                   for tuple_elem in tuple_) for tuple_ in cd)
+                    return sum(
+                        sum(tuple_elem._ufl_compute_hash_() for tuple_elem in tuple_)
+                        for tuple_ in cd
+                    )
+
                 coordderiv_integrals_dict = {}
                 for integral, coordderiv in stripped_integrals_and_coordderivs:
                     coordderivhash = calc_hash(coordderiv)
                     if coordderivhash in coordderiv_integrals_dict:
                         coordderiv_integrals_dict[coordderivhash][1].append(integral)
                     else:
                         coordderiv_integrals_dict[coordderivhash] = (coordderiv, [integral])
 
                 # cd_integrals_dict is now a dict of the form
                 # { hash: (CoordinateDerivative, [integral, integral, ...]), ... }
                 # we can now put the integrals back together and then afterwards
                 # apply the CoordinateDerivative again
 
                 for cdhash, samecd_integrals in sorted_by_key(coordderiv_integrals_dict):
-
                     # Accumulate integrands of integrals that share the
                     # same compiler data
-                    integrands_and_cds = accumulate_integrands_with_same_metadata(samecd_integrals[1])
+                    integrands_and_cds = accumulate_integrands_with_same_metadata(
+                        samecd_integrals[1]
+                    )
 
                     for integrand, metadata in integrands_and_cds:
-                        integral = Integral(integrand, integral_type, domain,
-                                            subdomain_id, metadata, None)
+                        integral = Integral(
+                            integrand, integral_type, domain, subdomain_id, metadata, None
+                        )
                         integral = attach_coordinate_derivatives(integral, samecd_integrals[0])
                         integrals.append(integral)
     return Form(integrals)
 
 
 def reconstruct_form_from_integral_data(integral_data):
     """Reconstruct a form from integral data."""
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/estimate_degrees.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/estimate_degrees.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Anders Logg, 2009-2010
 # Modified by Jan Blechta, 2012
 
 import warnings
 
-from ufl.corealg.multifunction import MultiFunction
 from ufl.checks import is_cellwise_constant
 from ufl.constantvalue import IntValue
 from ufl.corealg.map_dag import map_expr_dags
+from ufl.corealg.multifunction import MultiFunction
 from ufl.domain import extract_unique_domain
 from ufl.form import Form
 from ufl.integral import Integral
 
 
 class SumDegreeEstimator(MultiFunction):
     """Sum degree estimator.
@@ -42,64 +42,70 @@
     def constant(self, v):
         """Apply to constant."""
         return 0
 
     def geometric_quantity(self, v):
         """Apply to geometric_quantity.
 
-        Some geometric quantities are cellwise constant. Others are nonpolynomial and thus hard to estimate.
+        Some geometric quantities are cellwise constant. Others are
+        nonpolynomial and thus hard to estimate.
         """
         if is_cellwise_constant(v):
             return 0
         else:
             # As a heuristic, just returning domain degree to bump up degree somewhat
-            return extract_unique_domain(v).ufl_coordinate_element().degree()
+            return extract_unique_domain(v).ufl_coordinate_element().embedded_superdegree
 
     def spatial_coordinate(self, v):
         """Apply to spatial_coordinate.
 
         A coordinate provides additional degrees depending on coordinate field of domain.
         """
-        return extract_unique_domain(v).ufl_coordinate_element().degree()
+        return extract_unique_domain(v).ufl_coordinate_element().embedded_superdegree
 
     def cell_coordinate(self, v):
         """Apply to cell_coordinate.
 
         A coordinate provides one additional degree.
         """
         return 1
 
     def argument(self, v):
         """Apply to argument.
 
         A form argument provides a degree depending on the element,
         or the default degree if the element has no degree.
         """
-        return v.ufl_element().degree()  # FIXME: Use component to improve accuracy for mixed elements
+        return (
+            v.ufl_element().embedded_superdegree
+        )  # FIXME: Use component to improve accuracy for mixed elements
 
     def coefficient(self, v):
         """Apply to coefficient.
 
         A form argument provides a degree depending on the element,
         or the default degree if the element has no degree.
         """
         e = v.ufl_element()
         e = self.element_replace_map.get(e, e)
-        d = e.degree()  # FIXME: Use component to improve accuracy for mixed elements
+        d = e.embedded_superdegree  # FIXME: Use component to improve accuracy for mixed elements
         if d is None:
             d = self.default_degree
         return d
 
     def _reduce_degree(self, v, f):
         """Reduce the estimated degree by one.
 
         This is used when derivatives are taken. It does not reduce the degree when
         TensorProduct elements or quadrilateral elements are involved.
         """
-        if isinstance(f, int) and v.ufl_domain().ufl_cell().cellname() not in ["quadrilateral", "hexahedron"]:
+        if isinstance(f, int) and extract_unique_domain(v).ufl_cell().cellname() not in [
+            "quadrilateral",
+            "hexahedron",
+        ]:
             return max(f - 1, 0)
         else:
             return f
 
     def _add_degrees(self, v, *ops):
         """Apply to _add_degrees."""
         if any(isinstance(o, tuple) for o in ops):
@@ -280,41 +286,44 @@
 
     def atan2(self, v, a, b):
         """Apply to atan2.
 
         Using the heuristic:
         degree(atan2(const,const)) == 0
         degree(atan2(a,b)) == max(degree(a),degree(b))+2
-        which can be wildly inaccurate but at least gives a somewhat high integration degree.
+        which can be wildly inaccurate but at least gives a somewhat
+        high integration degree.
         """
         if a or b:
             return self._add_degrees(v, self._max_degrees(v, a, b), 2)
         else:
             return self._max_degrees(v, a, b)
 
     def math_function(self, v, a):
         """Apply to math_function.
 
         Using the heuristic:
         degree(sin(const)) == 0
         degree(sin(a)) == degree(a)+2
-        which can be wildly inaccurate but at least gives a somewhat high integration degree.
+        which can be wildly inaccurate but at least gives a somewhat
+        high integration degree.
         """
         if a:
             return self._add_degrees(v, a, 2)
         else:
             return a
 
     def bessel_function(self, v, nu, x):
         """Apply to bessel_function.
 
         Using the heuristic
         degree(bessel_*(const)) == 0
         degree(bessel_*(x)) == degree(x)+2
-        which can be wildly inaccurate but at least gives a somewhat high integration degree.
+        which can be wildly inaccurate but at least gives a somewhat
+        high integration degree.
         """
         if x:
             return self._add_degrees(v, x, 2)
         else:
             return x
 
     def condition(self, v, *args):
@@ -333,14 +342,15 @@
 
     def min_value(self, v, a, r):
         """Apply to min_value.
 
         Same as conditional.
         """
         return self._max_degrees(v, a, r)
+
     max_value = min_value
 
     def coordinate_derivative(self, v, integrand_degree, b, direction_degree, d):
         """Apply to coordinate_derivative.
 
         We use the heuristic that a shape derivative in direction V
         introduces terms V and grad(V) into the integrand. Hence we add the
@@ -353,25 +363,24 @@
         return self._max_degrees(v, *o)
 
     def expr_mapping(self, v, *o):
         """Apply to expr_mapping."""
         return self._max_degrees(v, *o)
 
 
-def estimate_total_polynomial_degree(e, default_degree=1,
-                                     element_replace_map={}):
+def estimate_total_polynomial_degree(e, default_degree=1, element_replace_map={}):
     """Estimate total polynomial degree of integrand.
 
     NB: Although some compound types are supported here,
     some derivatives and compounds must be preprocessed
     prior to degree estimation. In generic code, this algorithm
     should only be applied after preprocessing.
 
-    For coefficients defined on an element with unspecified degree (None),
-    the degree is set to the given default degree.
+    For coefficients defined on an element with unspecified degree
+    (None), the degree is set to the given default degree.
     """
     de = SumDegreeEstimator(default_degree, element_replace_map)
     if isinstance(e, Form):
         if not e.integrals():
             raise ValueError("Form has no integrals.")
         degrees = map_expr_dags(de, [it.integrand() for it in e.integrals()])
     elif isinstance(e, Integral):
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/expand_indices.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/expand_indices.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Anders Logg, 2009.
 
-from ufl.utils.stacks import Stack, StackDict
+from ufl.algorithms.transformer import ReuseTransformer, apply_transformer
 from ufl.classes import Terminal
 from ufl.constantvalue import Zero
-from ufl.core.multiindex import Index, FixedIndex, MultiIndex
+from ufl.core.multiindex import FixedIndex, Index, MultiIndex
 from ufl.differentiation import Grad
-from ufl.algorithms.transformer import ReuseTransformer, apply_transformer
+from ufl.utils.stacks import Stack, StackDict
 
 
 class IndexExpander(ReuseTransformer):
     """Index expander."""
 
     def __init__(self):
         """Initialise."""
@@ -54,18 +54,18 @@
 
             # Get component
             c = self.component()
             if r != len(c):
                 raise ValueError("Component size mismatch.")
 
             # Map it through an eventual symmetry mapping
-            s = e.symmetry()
-            c = s.get(c, c)
-            if r != len(c):
-                raise ValueError("Component size mismatch after symmetry mapping.")
+            if len(e.components) > 1:
+                c = min(i for i, j in e.components.items() if j == e.components[c])
+                if r != len(c):
+                    raise ValueError("Component size mismatch after symmetry mapping.")
 
             return x[c]
 
     def zero(self, x):
         """Apply to zero."""
         if len(x.ufl_shape) != len(self.component()):
             raise ValueError("Component size mismatch.")
@@ -129,15 +129,15 @@
 
         return self.reuse_if_possible(x, a, b)
 
     def index_sum(self, x):
         """Apply to index_sum."""
         ops = []
         summand, multiindex = x.ufl_operands
-        index, = multiindex
+        (index,) = multiindex
 
         # TODO: For the list tensor purging algorithm, do something like:
         # if index not in self._to_expand:
         #     return self.expr(x, *[self.visit(o) for o in x.ufl_operands])
 
         for value in range(x.dimension()):
             self._index2value.push(index, value)
@@ -218,15 +218,15 @@
         self._components.push(c1)
         r = self.visit(op)
         self._components.pop()
         return r
 
     def grad(self, x):
         """Apply to grad."""
-        f, = x.ufl_operands
+        (f,) = x.ufl_operands
         if not isinstance(f, (Terminal, Grad)):
             raise ValueError("Expecting expand_derivatives to have been applied.")
         # No need to visit child as long as it is on the form [Grad]([Grad](terminal))
         return x[self.component()]
 
 
 def expand_indices(e):
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/formdata.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/formdata.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,29 +4,31 @@
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Anders Logg, 2008.
 
-from ufl.utils.formatting import lstr, tstr, estr
+from ufl.utils.formatting import estr, lstr, tstr
 
 
 class FormData(object):
     """Class collecting various information extracted from a Form by calling preprocess."""
 
     def __init__(self):
         """Create empty form data for given form."""
 
     def __str__(self):
         """Return formatted summary of form data."""
         types = sorted(self.max_subdomain_ids.keys())
-        geometry = (("Geometric dimension", self.geometric_dimension), )
-        subdomains = tuple((f"Number of {integral_type} subdomains", self.max_subdomain_ids[integral_type])
-                           for integral_type in types)
+        geometry = (("Geometric dimension", self.geometric_dimension),)
+        subdomains = tuple(
+            (f"Number of {integral_type} subdomains", self.max_subdomain_ids[integral_type])
+            for integral_type in types
+        )
         functions = (
             # Arguments
             ("Rank", self.rank),
             ("Arguments", lstr(self.original_form.arguments())),
             # Coefficients
             ("Number of coefficients", self.num_coefficients),
             ("Coefficients", lstr(self.reduced_coefficients)),
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/formfiles.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/formfiles.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 #
 # Modified by Anders Logg, 2008-2009.
 # Modified by Marie E. Rognes, 2011.
 
 import io
 import os
 import re
-from ufl.utils.sorting import sorted_by_key
-from ufl.form import Form
-from ufl.finiteelement import FiniteElementBase
-from ufl.core.expr import Expr
-from ufl.constant import Constant
+
 from ufl.argument import Argument
 from ufl.coefficient import Coefficient
+from ufl.constant import Constant
+from ufl.core.expr import Expr
+from ufl.finiteelement import AbstractFiniteElement
+from ufl.form import Form
+from ufl.utils.sorting import sorted_by_key
 
 
 class FileData(object):
     """File data."""
 
     def __init__(self):
         """Initialise."""
@@ -32,16 +33,23 @@
         self.forms = []
         self.object_names = {}
         self.object_by_name = {}
         self.reserved_objects = {}
 
     def __bool__(self):
         """Convert to a bool."""
-        return bool(self.elements or self.coefficients or self.forms or self.expressions or  # noqa: W504
-                    self.object_names or self.object_by_name or self.reserved_objects)
+        return bool(
+            self.elements
+            or self.coefficients
+            or self.forms
+            or self.expressions
+            or self.object_names
+            or self.object_by_name
+            or self.reserved_objects
+        )
 
     __nonzero__ = __bool__
 
 
 def read_lines_decoded(fn):
     """Read decoded lines of a UFL file."""
     r = re.compile(b".*coding: *([^ ]+)")
@@ -54,17 +62,17 @@
     with io.open(fn, "rb") as f:
         lines = f.readlines()
 
     # Check for coding: in the first two lines
     for i in range(min(2, len(lines))):
         m = match(lines[i])
         if m:
-            encoding, = m.groups()
+            (encoding,) = m.groups()
             # Drop encoding line
-            lines = lines[:i] + lines[i + 1:]
+            lines = lines[:i] + lines[i + 1 :]
             break
     else:
         # Default to utf-8 (works for ascii files
         # as well, default for python files in py3)
         encoding = "utf-8"
 
     # Decode all lines
@@ -89,41 +97,44 @@
 
 
 def interpret_ufl_namespace(namespace):
     """Take a namespace dict from an executed ufl file and convert it to a FileData object."""
     # Object to hold all returned data
     ufd = FileData()
 
-    # Extract object names for Form, Coefficient and FiniteElementBase objects
+    # Extract object names for Form, Coefficient and AbstractFiniteElement objects
     # The use of id(obj) as key in object_names is necessary
     # because we need to distinguish between instances,
     # and not just between objects with different values.
     for name, value in sorted_by_key(namespace):
         # Store objects by reserved name OR instance id
         reserved_names = ("unknown",)  # Currently only one reserved name
         if name in reserved_names:
             # Store objects with reserved names
             ufd.reserved_objects[name] = value
             # FIXME: Remove after FFC is updated to use reserved_objects:
             ufd.object_names[name] = value
             ufd.object_by_name[name] = value
-        elif isinstance(value, (FiniteElementBase, Coefficient, Constant, Argument, Form, Expr)):
+        elif isinstance(
+            value, (AbstractFiniteElement, Coefficient, Constant, Argument, Form, Expr)
+        ):
             # Store instance <-> name mappings for important objects
             # without a reserved name
             ufd.object_names[id(value)] = name
             ufd.object_by_name[name] = value
 
     # Get list of exported forms
     forms = namespace.get("forms")
     if forms is None:
         # Get forms from object_by_name, which has already mapped
         # tuple->Form where needed
         def get_form(name):
             form = ufd.object_by_name.get(name)
             return form if isinstance(form, Form) else None
+
         a_form = get_form("a")
         L_form = get_form("L")
         M_form = get_form("M")
         forms = [a_form, L_form, M_form]
         # Add forms F and J if not "a" and "L" are used
         if a_form is None or L_form is None:
             F_form = get_form("F")
@@ -144,34 +155,40 @@
     if elements is None:
         elements = [ufd.object_by_name.get(name) for name in ("element",)]
         elements = [e for e in elements if e is not None]
     ufd.elements = elements
 
     # Validate types
     if not isinstance(ufd.elements, (list, tuple)):
-        raise ValueError(f"Expecting 'elements' to be a list or tuple, not '{type(ufd.elements)}''.")
-    if not all(isinstance(e, FiniteElementBase) for e in ufd.elements):
-        raise ValueError("Expecting 'elements' to be a list of FiniteElementBase instances.")
+        raise ValueError(
+            f"Expecting 'elements' to be a list or tuple, not '{type(ufd.elements)}''."
+        )
+    if not all(isinstance(e, AbstractFiniteElement) for e in ufd.elements):
+        raise ValueError("Expecting 'elements' to be a list of AbstractFiniteElement instances.")
 
     # Get list of exported coefficients
     functions = []
     ufd.coefficients = namespace.get("coefficients", functions)
 
     # Validate types
     if not isinstance(ufd.coefficients, (list, tuple)):
-        raise ValueError(f"Expecting 'coefficients' to be a list or tuple, not '{type(ufd.coefficients)}'.")
+        raise ValueError(
+            f"Expecting 'coefficients' to be a list or tuple, not '{type(ufd.coefficients)}'."
+        )
     if not all(isinstance(e, Coefficient) for e in ufd.coefficients):
         raise ValueError("Expecting 'coefficients' to be a list of Coefficient instances.")
 
     # Get list of exported expressions
     ufd.expressions = namespace.get("expressions", [])
 
     # Validate types
     if not isinstance(ufd.expressions, (list, tuple)):
-        raise ValueError(f"Expecting 'expressions' to be a list or tuple, not '{type(ufd.expressions)}'.")
+        raise ValueError(
+            f"Expecting 'expressions' to be a list or tuple, not '{type(ufd.expressions)}'."
+        )
     if not all(isinstance(e[0], Expr) for e in ufd.expressions):
         raise ValueError("Expecting 'expressions' to be a list of Expr instances.")
 
     # Return file data
     return ufd
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/formsplitter.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/formsplitter.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,71 +4,71 @@
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Cecile Daversin-Catty, 2018
 
-from ufl.corealg.multifunction import MultiFunction
 from ufl.algorithms.map_integrands import map_integrand_dags
-from ufl.constantvalue import Zero
-from ufl.tensors import as_vector
 from ufl.argument import Argument
+from ufl.constantvalue import Zero
+from ufl.corealg.multifunction import MultiFunction
 from ufl.functionspace import FunctionSpace
+from ufl.tensors import as_vector
 
 
 class FormSplitter(MultiFunction):
     """Form splitter."""
 
     def split(self, form, ix, iy=0):
         """Split."""
         # Remember which block to extract
         self.idx = [ix, iy]
         return map_integrand_dags(self, form)
 
     def argument(self, obj):
         """Apply to argument."""
-        if (obj.part() is not None):
+        if obj.part() is not None:
             # Mixed element built from MixedFunctionSpace,
             # whose sub-function spaces are indexed by obj.part()
             if len(obj.ufl_shape) == 0:
-                if (obj.part() == self.idx[obj.number()]):
+                if obj.part() == self.idx[obj.number()]:
                     return obj
                 else:
                     return Zero()
             else:
                 indices = [()]
                 for m in obj.ufl_shape:
                     indices = [(k + (j,)) for k in indices for j in range(m)]
 
-                if (obj.part() == self.idx[obj.number()]):
+                if obj.part() == self.idx[obj.number()]:
                     return as_vector([obj[j] for j in indices])
                 else:
                     return as_vector([Zero() for j in indices])
         else:
             # Mixed element built from MixedElement,
             # whose sub-elements need their function space to be created
             Q = obj.ufl_function_space()
             dom = Q.ufl_domain()
             sub_elements = obj.ufl_element().sub_elements()
 
             # If not a mixed element, do nothing
-            if (len(sub_elements) == 0):
+            if len(sub_elements) == 0:
                 return obj
 
             args = []
             for i, sub_elem in enumerate(sub_elements):
                 Q_i = FunctionSpace(dom, sub_elem)
                 a = Argument(Q_i, obj.number(), part=obj.part())
 
                 indices = [()]
                 for m in a.ufl_shape:
                     indices = [(k + (j,)) for k in indices for j in range(m)]
 
-                if (i == self.idx[obj.number()]):
+                if i == self.idx[obj.number()]:
                     args += [a[j] for j in indices]
                 else:
                     args += [Zero() for j in indices]
 
             return as_vector(args)
 
     def multi_index(self, obj):
@@ -86,15 +86,15 @@
 
     numbers = tuple(sorted(set(a.number() for a in arguments)))
     arity = len(numbers)
     parts = tuple(sorted(set(a.part() for a in arguments)))
     assert arity <= 2
 
     if arity == 0:
-        return (form, )
+        return (form,)
 
     for pi in parts:
         if arity > 1:
             for pj in parts:
                 f = fs.split(form, pi, pj)
                 if f.empty():
                     forms.append(None)
@@ -107,15 +107,15 @@
             else:
                 forms.append(f)
 
     try:
         forms_tuple = tuple(forms)
     except TypeError:
         # Only one form returned
-        forms_tuple = (forms, )
+        forms_tuple = (forms,)
 
     if i is not None:
         if arity > 1 and j is not None:
             return forms_tuple[i * len(parts) + j]
         else:
             return forms_tuple[i]
     else:
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/formtransformations.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/formtransformations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-"""This module defines utilities for transforming complete Forms into new related Forms."""
+"""Utilities for transforming complete Forms into new related Forms."""
 
 # Copyright (C) 2008-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Anders Logg, 2008-2009.
 # Modified by Garth N. Wells, 2010.
 # Modified by Marie E. Rognes, 2010.
 
 import warnings
 from logging import debug
 
-# All classes:
-from ufl.core.expr import ufl_err_str
-from ufl.argument import Argument
-from ufl.coefficient import Coefficient
-from ufl.constantvalue import Zero
 from ufl.algebra import Conj
 
 # Other algorithms:
 from ufl.algorithms.map_integrands import map_integrands
-from ufl.algorithms.transformer import Transformer
 from ufl.algorithms.replace import replace
+from ufl.algorithms.transformer import Transformer
+from ufl.argument import Argument
+from ufl.coefficient import Coefficient
+from ufl.constantvalue import Zero
+
+# All classes:
+from ufl.core.expr import ufl_err_str
 
 
 # FIXME: Don't use this below, it makes partextracter more expensive than necessary
 def _expr_has_terminal_types(expr, ufl_types):
     """Check if an expression has terminal types."""
     input = [expr]
     while input:
@@ -120,15 +121,14 @@
         """
         parts_that_provide = {}
 
         # 1. Skip terms that provide too much
         original_terms = x.ufl_operands
         assert len(original_terms) == 2
         for term in original_terms:
-
             # Visit this term in the sum
             part, term_provides = self.visit(term)
 
             # If this part is zero or it provides more than we want,
             # skip it
             if isinstance(part, Zero) or (term_provides - self._want):
                 continue
@@ -142,42 +142,40 @@
 
         # 2. If there are no remaining terms, return zero
         if not parts_that_provide:
             return (zero_expr(x), set())
 
         # 3. Return the terms that provide the biggest set
         most_provided = frozenset()
-        for (provideds, parts) in parts_that_provide.items():  # TODO: Just sort instead?
-
+        for provideds, parts in parts_that_provide.items():  # TODO: Just sort instead?
             # Throw error if size of sets are equal (and not zero)
             if len(provideds) == len(most_provided) and len(most_provided):
                 raise ValueError("Don't know what to do with sums with different Arguments.")
 
             if provideds > most_provided:
                 most_provided = provideds
 
         terms = parts_that_provide[most_provided]
         if len(terms) == 2:
             x = self.reuse_if_possible(x, *terms)
         else:
-            x, = terms
+            (x,) = terms
 
         return (x, most_provided)
 
     def product(self, x, *ops):
         """Apply to product.
 
         Note: Product is a visit-children-first handler. ops are
         the visited factors.
         """
         provides = set()
         factors = []
 
         for factor, factor_provides in ops:
-
             # If any factor is zero, return
             if isinstance(factor, Zero):
                 return (zero_expr(x), set())
 
             # Add factor to factors and extend provides
             factors.append(factor)
             provides = provides | factor_provides
@@ -199,15 +197,17 @@
     def division(self, x):
         """Return parts_of_numerator/denominator."""
         # Get numerator and denominator
         numerator, denominator = x.ufl_operands
 
         # Check for Arguments in the denominator
         if _expr_has_terminal_types(denominator, Argument):
-            raise ValueError(f"Found Argument in denominator of {ufl_err_str(x)}, this is an invalid expression.")
+            raise ValueError(
+                f"Found Argument in denominator of {ufl_err_str(x)}, this is an invalid expression."
+            )
 
         # Visit numerator
         numerator_parts, provides = self.visit(numerator)
 
         # If numerator is zero, return zero. (No need to check whether
         # it provides too much, already checked by visit.)
         if isinstance(numerator_parts, Zero):
@@ -278,26 +278,28 @@
         """Apply to list_tensor."""
         # list_tensor is a visit-children-first handler. ops contains
         # the visited operands with their provides. (It follows that
         # none of the visited operands provide more than wanted.)
 
         # Extract the most arguments provided by any of the components
         most_provides = ops[0][1]
-        for (component, provides) in ops:
-            if (provides - most_provides):
+        for component, provides in ops:
+            if provides - most_provides:
                 most_provides = provides
 
         # Check that all components either provide the same arguments
         # or vanish. (This check is here b/c it is not obvious what to
         # return if the components provide different arguments, at
         # least with the current transformer design.)
-        for (component, provides) in ops:
-            if (provides != most_provides and not isinstance(component, Zero)):
-                raise ValueError("PartExtracter does not know how to handle list_tensors with "
-                                 "non-zero components providing fewer arguments")
+        for component, provides in ops:
+            if provides != most_provides and not isinstance(component, Zero):
+                raise ValueError(
+                    "PartExtracter does not know how to handle list_tensors with "
+                    "non-zero components providing fewer arguments"
+                )
 
         # Return components
         components = [op[0] for op in ops]
         x = self.reuse_if_possible(x, *components)
 
         return (x, most_provides)
 
@@ -324,29 +326,29 @@
     pe = PartExtracter(sub_arguments)
 
     def _transform(e):
         e, provides = pe.visit(e)
         if provides == sub_arguments:
             return e
         return Zero()
+
     return map_integrands(_transform, form)
 
 
 def compute_form_arities(form):
     """Return set of arities of terms present in form."""
     # Extract all arguments present in form
     arguments = form.arguments()
 
     parts = [arg.part() for arg in arguments]
     if set(parts) - {None}:
         raise ValueError("compute_form_arities cannot handle parts.")
 
     arities = set()
     for arity in range(len(arguments) + 1):
-
         # Compute parts with arity "arity"
         parts = compute_form_with_arity(form, arity, arguments)
 
         # Register arity if "parts" does not vanish
         if parts and parts.integrals():
             arities.add(arity)
 
@@ -429,21 +431,25 @@
 
     if len(arguments) != 2:
         raise ValueError("Expecting bilinear form.")
     v, u = arguments
     U = u.ufl_function_space()
     V = v.ufl_function_space()
     if U != V:
-        raise ValueError(f"Expecting equal finite elements for test and trial functions, got '{U}' and '{V}'.")
+        raise ValueError(
+            f"Expecting equal finite elements for test and trial functions, got '{U}' and '{V}'."
+        )
     if coefficient is None:
         coefficient = Coefficient(V)
     else:
         if coefficient.ufl_function_space() != U:
-            raise ValueError("Trying to compute action of form on a "
-                  "coefficient in an incompatible element space.")
+            raise ValueError(
+                "Trying to compute action of form on a "
+                "coefficient in an incompatible element space."
+            )
     return action(action(form, coefficient), coefficient)
 
 
 def compute_form_adjoint(form, reordered_arguments=None):
     """Compute the adjoint of a bilinear form.
 
     This works simply by swapping the number and part of the two arguments,
@@ -459,18 +465,16 @@
         raise ValueError("Expecting bilinear form.")
 
     v, u = arguments
     if v.number() >= u.number():
         raise ValueError("Mistaken assumption in code!")
 
     if reordered_arguments is None:
-        reordered_u = Argument(u.ufl_function_space(), number=v.number(),
-                               part=v.part())
-        reordered_v = Argument(v.ufl_function_space(), number=u.number(),
-                               part=u.part())
+        reordered_u = Argument(u.ufl_function_space(), number=v.number(), part=v.part())
+        reordered_v = Argument(v.ufl_function_space(), number=u.number(), part=u.part())
     else:
         reordered_u, reordered_v = reordered_arguments
 
     if reordered_u.number() >= reordered_v.number():
         raise ValueError("Ordering of new arguments is the same as the old arguments!")
 
     if reordered_u.part() != v.part():
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/map_integrands.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/map_integrands.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,59 @@
-"""Basic algorithms for applying functions to subexpressions."""
+"""Basic algorithms for applying functions to sub-expressions."""
 
 # Copyright (C) 2008-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
 # NOTE: Placing this under algorithms/ because I want corealg/ to stay clean
 # as part of a careful refactoring process, and this file depends on ufl.form
 # which drags in a lot of stuff.
 
-from ufl.core.expr import Expr
-from ufl.corealg.map_dag import map_expr_dag
-from ufl.integral import Integral
-from ufl.form import Form, BaseForm, FormSum, ZeroBaseForm
 from ufl.action import Action
 from ufl.adjoint import Adjoint
 from ufl.constantvalue import Zero
+from ufl.core.expr import Expr
+from ufl.corealg.map_dag import map_expr_dag
+from ufl.form import BaseForm, Form, FormSum, ZeroBaseForm
+from ufl.integral import Integral
 
 
 def map_integrands(function, form, only_integral_type=None):
-    """Apply transform(expression) to each integrand expression in form, or to form if it is an Expr."""
+    """Map integrands.
+
+    Apply transform(expression) to each integrand expression in form, or
+    to form if it is an Expr.
+    """
     if isinstance(form, Form):
-        mapped_integrals = [map_integrands(function, itg, only_integral_type)
-                            for itg in form.integrals()]
-        nonzero_integrals = [itg for itg in mapped_integrals
-                             if not isinstance(itg.integrand(), Zero)]
+        mapped_integrals = [
+            map_integrands(function, itg, only_integral_type) for itg in form.integrals()
+        ]
+        nonzero_integrals = [
+            itg for itg in mapped_integrals if not isinstance(itg.integrand(), Zero)
+        ]
         return Form(nonzero_integrals)
     elif isinstance(form, Integral):
         itg = form
         if (only_integral_type is None) or (itg.integral_type() in only_integral_type):
             return itg.reconstruct(function(itg.integrand()))
         else:
             return itg
     elif isinstance(form, FormSum):
-        mapped_components = [map_integrands(function, component, only_integral_type)
-                             for component in form.components()]
-        nonzero_components = [(component, w) for component, w in zip(mapped_components, form.weights())
-                              # Catch ufl.Zero and ZeroBaseForm
-                              if component != 0]
+        mapped_components = [
+            map_integrands(function, component, only_integral_type)
+            for component in form.components()
+        ]
+        nonzero_components = [
+            (component, w)
+            for component, w in zip(mapped_components, form.weights())
+            # Catch ufl.Zero and ZeroBaseForm
+            if component != 0
+        ]
 
         # Simplify case with one nonzero component and the corresponding weight is 1
         if len(nonzero_components) == 1 and nonzero_components[0][1] == 1:
             return nonzero_components[0][0]
 
         if all(not isinstance(component, BaseForm) for component, _ in nonzero_components):
             # Simplification of `BaseForm` objects may turn `FormSum` into a sum of `Expr` objects
@@ -55,20 +66,23 @@
         return Adjoint(map_integrands(function, form._form, only_integral_type))
     elif isinstance(form, Action):
         left = map_integrands(function, form._left, only_integral_type)
         right = map_integrands(function, form._right, only_integral_type)
         # Zeros are caught inside `Action.__new__`
         return Action(left, right)
     elif isinstance(form, ZeroBaseForm):
-        arguments = tuple(map_integrands(function, arg, only_integral_type) for arg in form._arguments)
+        arguments = tuple(
+            map_integrands(function, arg, only_integral_type) for arg in form._arguments
+        )
         return ZeroBaseForm(arguments)
     elif isinstance(form, (Expr, BaseForm)):
         integrand = form
         return function(integrand)
     else:
         raise ValueError("Expecting Form, Integral or Expr.")
 
 
 def map_integrand_dags(function, form, only_integral_type=None, compress=True):
     """Map integrand dags."""
-    return map_integrands(lambda expr: map_expr_dag(function, expr, compress),
-                          form, only_integral_type)
+    return map_integrands(
+        lambda expr: map_expr_dag(function, expr, compress), form, only_integral_type
+    )
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/remove_complex_nodes.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/remove_complex_nodes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-"""Algorithm for removing conj, real, and imag nodes from a form for when the user is in 'real mode'."""
+"""Remove conj, real, and imag nodes from a form."""
 
-from ufl.corealg.multifunction import MultiFunction
-from ufl.constantvalue import ComplexValue
 from ufl.algorithms.map_integrands import map_integrand_dags
+from ufl.constantvalue import ComplexValue
+from ufl.corealg.multifunction import MultiFunction
 
 
 class ComplexNodeRemoval(MultiFunction):
     """Replaces complex operator nodes with their children."""
+
     expr = MultiFunction.reuse_if_untouched
 
     def conj(self, o, a):
         """Apply to conj."""
         return a
 
     def real(self, o, a):
@@ -20,20 +21,20 @@
     def imag(self, o, a):
         """Apply to imag."""
         raise ValueError("Unexpected imag in real expression.")
 
     def terminal(self, t, *ops):
         """Apply to terminal."""
         if isinstance(t, ComplexValue):
-            raise ValueError('Unexpected complex value in real expression.')
+            raise ValueError("Unexpected complex value in real expression.")
         else:
             return t
 
 
 def remove_complex_nodes(expr):
     """Replaces complex operator nodes with their children.
 
-    This is called during compute_form_data if the compiler wishes to compile
-    real-valued forms. In essence this strips all trace of complex
-    support from the preprocessed form.
+    This is called during compute_form_data if the compiler wishes to
+    compile real-valued forms. In essence this strips all trace of
+    complex support from the preprocessed form.
     """
     return map_integrand_dags(ComplexNodeRemoval(), expr)
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/renumbering.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/renumbering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Algorithms for renumbering of counted objects, currently variables and indices."""
 # Copyright (C) 2008-2016 Martin Sandve Alnæs and Anders Logg
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
-from ufl.core.expr import Expr
-from ufl.core.multiindex import Index, FixedIndex, MultiIndex
-from ufl.variable import Label, Variable
 from ufl.algorithms.transformer import ReuseTransformer, apply_transformer
 from ufl.classes import Zero
+from ufl.core.expr import Expr
+from ufl.core.multiindex import FixedIndex, Index, MultiIndex
+from ufl.variable import Label, Variable
 
 
 class VariableRenumberingTransformer(ReuseTransformer):
     """Variable renumbering transformer."""
 
     def __init__(self):
         """Initialise."""
@@ -31,15 +31,16 @@
             self.variable_map[l] = v
         return v
 
 
 class IndexRenumberingTransformer(VariableRenumberingTransformer):
     """Index renumbering transformer.
 
-    This is a poorly designed algorithm. It is used in some tests, please do not use for anything else.
+    This is a poorly designed algorithm. It is used in some tests,
+    please do not use for anything else.
     """
 
     def __init__(self):
         """Initialise."""
         VariableRenumberingTransformer.__init__(self)
         self.index_map = {}
 
@@ -75,9 +76,12 @@
     if isinstance(expr, Expr):
         num_free_indices = len(expr.ufl_free_indices)
 
     result = apply_transformer(expr, IndexRenumberingTransformer())
 
     if isinstance(expr, Expr):
         if num_free_indices != len(result.ufl_free_indices):
-            raise ValueError("The number of free indices left in expression should be invariant w.r.t. renumbering.")
+            raise ValueError(
+                "The number of free indices left in expression "
+                "should be invariant w.r.t. renumbering."
+            )
     return result
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/replace.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/replace.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Anders Logg, 2009-2010
 
-from ufl.classes import CoefficientDerivative, Interpolate, ExternalOperator, Form
+from ufl.algorithms.analysis import has_exact_type
+from ufl.algorithms.map_integrands import map_integrand_dags
+from ufl.classes import CoefficientDerivative, Form
 from ufl.constantvalue import as_ufl
+from ufl.core.external_operator import ExternalOperator
+from ufl.core.interpolate import Interpolate
 from ufl.corealg.multifunction import MultiFunction
-from ufl.algorithms.map_integrands import map_integrand_dags
-from ufl.algorithms.analysis import has_exact_type
 
 
 class Replacer(MultiFunction):
     """Replacer."""
 
     def __init__(self, mapping):
         """Initialize."""
@@ -27,15 +29,17 @@
         def get_shape(x):
             """Get the shape of an object."""
             if isinstance(x, Form):
                 return x.arguments()[0].ufl_shape
             return x.ufl_shape
 
         if not all(get_shape(k) == get_shape(v) for k, v in mapping.items()):
-            raise ValueError("Replacement expressions must have the same shape as what they replace.")
+            raise ValueError(
+                "Replacement expressions must have the same shape as what they replace."
+            )
 
     def ufl_type(self, o, *args):
         """Replace a ufl_type."""
         try:
             return self.mapping[o]
         except KeyError:
             return self.reuse_if_untouched(o, *args)
@@ -82,10 +86,11 @@
     # replace(derivative(f(g, h), g), {g: h})
     #
     # To fix this would require one to expand derivatives early (which
     # is not attractive), or make replace lazy too.
     if has_exact_type(e, CoefficientDerivative):
         # Hack to avoid circular dependencies
         from ufl.algorithms.ad import expand_derivatives
+
         e = expand_derivatives(e)
 
     return map_integrand_dags(Replacer(mapping2), e)
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/replace_derivative_nodes.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/replace_derivative_nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Algorithm for replacing derivative nodes in a BaseForm or Expr."""
 
 import ufl
-from ufl.corealg.multifunction import MultiFunction
-from ufl.algorithms.map_integrands import map_integrand_dags
 from ufl.algorithms.analysis import extract_arguments
-from ufl.tensors import ListTensor
+from ufl.algorithms.map_integrands import map_integrand_dags
 from ufl.constantvalue import as_ufl
+from ufl.corealg.multifunction import MultiFunction
+from ufl.tensors import ListTensor
 
 
 class DerivativeNodeReplacer(MultiFunction):
     """Replace derivative nodes with new derivative nodes."""
 
     def __init__(self, mapping, **derivative_kwargs):
         """Initialise."""
@@ -18,49 +18,52 @@
         self.der_kwargs = derivative_kwargs
 
     expr = MultiFunction.reuse_if_untouched
 
     def coefficient_derivative(self, cd, o, coefficients, arguments, coefficient_derivatives):
         """Apply to coefficient_derivative."""
         der_kwargs = self.der_kwargs
-        new_coefficients = tuple(self.mapping[c] if c in self.mapping.keys() else c for c in coefficients.ufl_operands)
+        new_coefficients = tuple(
+            self.mapping[c] if c in self.mapping.keys() else c for c in coefficients.ufl_operands
+        )
 
         # Ensure type compatibility for arguments!
-        if 'argument' not in der_kwargs.keys():
+        if "argument" not in der_kwargs.keys():
             # Argument's number/part can be retrieved from the former coefficient derivative.
             arguments = arguments.ufl_operands
             new_arguments = ()
             for c, a in zip(new_coefficients, arguments):
                 if isinstance(a, ListTensor):
-                    a, = extract_arguments(a)
+                    (a,) = extract_arguments(a)
                 new_arguments += (type(a)(c.ufl_function_space(), a.number(), a.part()),)
-            der_kwargs.update({'argument': new_arguments})
+            der_kwargs.update({"argument": new_arguments})
 
         return ufl.derivative(o, new_coefficients, **der_kwargs)
 
 
 def replace_derivative_nodes(expr, mapping, **derivative_kwargs):
     """Replaces derivative nodes.
 
     Replaces the variable with respect to which the derivative is taken.
     This is called during apply_derivatives to treat delayed derivatives.
 
-    Example: Let u be a Coefficient, N an ExternalOperator independent of u (i.e. N's operands don't depend on u),
-             and let uhat and Nhat be Arguments.
+    Example: Let u be a Coefficient, N an ExternalOperator independent
+        of u (i.e. N's operands don't depend on u),
+        and let uhat and Nhat be Arguments.
 
         F = u ** 2 * N * dx
         dFdu = derivative(F, u, uhat)
         dFdN = replace_derivative_nodes(dFdu, {u: N}, argument=Nhat)
 
         Then, by subsequently expanding the derivatives we have:
 
         dFdu -> 2 * u * uhat * N * dx
         dFdN -> u ** 2 * Nhat * dx
 
     Args:
         expr: An Expr or BaseForm.
         mapping: A dict with from:to replacements to perform.
-        derivative_kwargs: A dict containing the keyword arguments for derivative
-            (i.e. `argument` and `coefficient_derivatives`).
+        derivative_kwargs: A dict containing the keyword arguments for
+            derivative (i.e. `argument` and `coefficient_derivatives`).
     """
     mapping2 = dict((k, as_ufl(v)) for (k, v) in mapping.items())
     return map_integrand_dags(DerivativeNodeReplacer(mapping2, **derivative_kwargs), expr)
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/signature.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/signature.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,29 @@
 # Copyright (C) 2012-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
 import hashlib
-from ufl.classes import (Label,
-                         Index, MultiIndex,
-                         Coefficient, Argument,
-                         GeometricQuantity, ConstantValue, Constant,
-                         ExprList, ExprMapping)
-from ufl.corealg.traversal import traverse_unique_terminals, unique_post_traversal
+
 from ufl.algorithms.domain_analysis import canonicalize_metadata
+from ufl.classes import (
+    Argument,
+    Coefficient,
+    Constant,
+    ConstantValue,
+    ExprList,
+    ExprMapping,
+    GeometricQuantity,
+    Index,
+    Label,
+    MultiIndex,
+)
+from ufl.corealg.traversal import traverse_unique_terminals, unique_post_traversal
 
 
 def compute_multiindex_hashdata(expr, index_numbering):
     """Compute multiindex hashdata."""
     data = []
     for i in expr:
         if isinstance(i, Index):
@@ -41,15 +49,14 @@
     # Extract a unique numbering of free indices, as well as form
     # arguments, and just take repr of the rest of the terminals while
     # we're iterating over them
     terminal_hashdata = {}
     index_numbering = {}
     for expression in expressions:
         for expr in traverse_unique_terminals(expression):
-
             if isinstance(expr, MultiIndex):
                 # Indices need a canonical numbering for a stable
                 # signature, thus this algorithm
                 data = compute_multiindex_hashdata(expr, index_numbering)
 
             elif isinstance(expr, ConstantValue):
                 data = expr._ufl_signature_data_(renumbering)
@@ -129,16 +136,15 @@
     # replacement of functions and index labels.
     terminal_hashdata = compute_terminal_hashdata(integrands, renumbering)
 
     # Build hashdata for each integral
     hashdata = []
     for integral in integrals:
         # Compute hash data for expression, this is the expensive part
-        integrand_hashdata = compute_expression_hashdata(integral.integrand(),
-                                                         terminal_hashdata)
+        integrand_hashdata = compute_expression_hashdata(integral.integrand(), terminal_hashdata)
 
         domain_hashdata = integral.ufl_domain()._ufl_signature_data_(renumbering)
 
         # Collect all data about integral that should be reflected in
         # signature, including compiler data but not domain data,
         # because compiler data affects the way the integral is
         # compiled while domain data is only carried for convenience
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/strip_terminal_data.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/strip_terminal_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 """Algorithm for replacing form arguments with 'stripped' versions.
 
 In the stripped version, any data-carrying objects have been extracted to a mapping.
 """
 
-from ufl.classes import Form, Integral
-from ufl.classes import Argument, Coefficient, Constant
-from ufl.classes import FunctionSpace, TensorProductFunctionSpace, MixedFunctionSpace
-from ufl.classes import Mesh, MeshView, TensorProductMesh
 from ufl.algorithms.replace import replace
+from ufl.classes import (
+    Argument,
+    Coefficient,
+    Constant,
+    Form,
+    FunctionSpace,
+    Integral,
+    Mesh,
+    MeshView,
+    MixedFunctionSpace,
+    TensorProductFunctionSpace,
+)
 from ufl.corealg.map_dag import map_expr_dag
 from ufl.corealg.multifunction import MultiFunction
 
 
 class TerminalStripper(MultiFunction):
     """Terminal stripper."""
 
     def __init__(self):
         """Initialise."""
         super().__init__()
         self.mapping = {}
 
     def argument(self, o):
         """Apply to argument."""
-        o_new = Argument(strip_function_space(o.ufl_function_space()),
-                         o.number(), o.part())
+        o_new = Argument(strip_function_space(o.ufl_function_space()), o.number(), o.part())
         return self.mapping.setdefault(o, o_new)
 
     def coefficient(self, o):
         """Apply to coefficient."""
-        o_new = Coefficient(strip_function_space(o.ufl_function_space()),
-                            o.count())
+        o_new = Coefficient(strip_function_space(o.ufl_function_space()), o.count())
         return self.mapping.setdefault(o, o_new)
 
     def constant(self, o):
         """Apply to constant."""
-        o_new = Constant(strip_domain(o.ufl_domain()), o.ufl_shape,
-                         o.count())
+        o_new = Constant(strip_domain(o.ufl_domain()), o.ufl_shape, o.count())
         return self.mapping.setdefault(o, o_new)
 
     expr = MultiFunction.reuse_if_untouched
 
 
 def strip_terminal_data(o):
     """Return a new form where all terminals have been replaced by UFL-only equivalents.
@@ -100,16 +105,17 @@
     else:
         raise ValueError("Only Form or Integral inputs expected")
 
 
 def strip_function_space(function_space):
     """Return a new function space with all non-UFL information removed."""
     if isinstance(function_space, FunctionSpace):
-        return FunctionSpace(strip_domain(function_space.ufl_domain()),
-                             function_space.ufl_element())
+        return FunctionSpace(
+            strip_domain(function_space.ufl_domain()), function_space.ufl_element()
+        )
     elif isinstance(function_space, TensorProductFunctionSpace):
         subspaces = [strip_function_space(sub) for sub in function_space.ufl_sub_spaces()]
         return TensorProductFunctionSpace(*subspaces)
     elif isinstance(function_space, MixedFunctionSpace):
         subspaces = [strip_function_space(sub) for sub in function_space.ufl_sub_spaces()]
         return MixedFunctionSpace(*subspaces)
     else:
@@ -117,14 +123,12 @@
 
 
 def strip_domain(domain):
     """Return a new domain with all non-UFL information removed."""
     if isinstance(domain, Mesh):
         return Mesh(domain.ufl_coordinate_element(), domain.ufl_id())
     elif isinstance(domain, MeshView):
-        return MeshView(strip_domain(domain.ufl_mesh()),
-                        domain.topological_dimension(), domain.ufl_id())
-    elif isinstance(domain, TensorProductMesh):
-        meshes = [strip_domain(mesh) for mesh in domain.ufl_meshes()]
-        return TensorProductMesh(meshes, domain.ufl_id())
+        return MeshView(
+            strip_domain(domain.ufl_mesh()), domain.topological_dimension(), domain.ufl_id()
+        )
     else:
         raise NotImplementedError(f"{type(domain)} cannot be stripped")
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/transformer.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 class Transformer(object):
     """Transformer.
 
     Base class for a visitor-like algorithm design pattern used to
     transform expression trees from one representation to another.
     """
+
     _handlers_cache = {}
 
     def __init__(self, variable_cache=None):
         """Initialise."""
         if variable_cache is None:
             variable_cache = {}
         self._variable_cache = variable_cache
@@ -60,25 +61,24 @@
                     except AttributeError as attribute_error:
                         if type(classobject) is not UFLType:
                             raise attribute_error
                         # Default handler name for UFL types
                         handler_name = UFLType._ufl_handler_name_
                     function = getattr(self, handler_name, None)
                     if function:
-                        cache_data[
-                            classobject.
-                            _ufl_typecode_] = handler_name, is_post_handler(
-                                function)
+                        cache_data[classobject._ufl_typecode_] = (
+                            handler_name,
+                            is_post_handler(function),
+                        )
                         break
             Transformer._handlers_cache[type(self)] = cache_data
 
         # Build handler list for this particular class (get functions
         # bound to self)
-        self._handlers = [(getattr(self, name), post)
-                          for (name, post) in cache_data]
+        self._handlers = [(getattr(self, name), post) for (name, post) in cache_data]
         # Keep a stack of objects visit is called on, to ease
         # backtracking
         self._visit_stack = []
 
     def print_visit_stack(self):
         """Print visit stack."""
         print("/" * 80)
@@ -232,15 +232,18 @@
 
     def variable(self, o):
         """Visit a variable."""
         return self.visit(o.ufl_operands[0])
 
 
 def apply_transformer(e, transformer, integral_type=None):
-    """Apply transformer.visit(expression) to each integrand expression in form, or to form if it is an Expr."""
-    return map_integrands(lambda expr: transformer.visit(expr), e,
-                          integral_type)
+    """Apply transforms.
+
+    Apply transformer.visit(expression) to each integrand expression in
+    form, or to form if it is an Expr.
+    """
+    return map_integrands(lambda expr: transformer.visit(expr), e, integral_type)
 
 
 def strip_variables(e):
     """Replace all Variable instances with the expression they represent."""
     return apply_transformer(e, VariableStripper())
```

### Comparing `fenics-ufl-2023.2.0/ufl/algorithms/traversal.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/traversal.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,23 @@
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Anders Logg, 2008
 
-from ufl.core.expr import Expr
-from ufl.integral import Integral
 from ufl.action import Action
 from ufl.adjoint import Adjoint
-from ufl.form import Form, FormSum, BaseForm
-
+from ufl.core.expr import Expr
+from ufl.form import BaseForm, Form, FormSum
+from ufl.integral import Integral
 
-# --- Traversal utilities ---
 
 def iter_expressions(a):
-    """Utility function to handle Form, Integral and any Expr the same way when inspecting expressions.
+    """Handle Form, Integral and any Expr the same way when inspecting expressions.
 
     Returns an iterable over Expr instances:
     - a is an Expr: (a,)
     - a is an Integral:  the integrand expression of a
     - a is a  Form:      all integrand expressions of all integrals
     - a is a  FormSum:   the components of a
     - a is an Action:    the left and right component of a
```

### Comparing `fenics-ufl-2023.2.0/ufl/argument.py` & `fenics_ufl-2024.1.0.post0/ufl/argument.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,57 +10,47 @@
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Anders Logg, 2008-2009.
 # Modified by Massimiliano Leoni, 2016.
 # Modified by Cecile Daversin-Catty, 2018.
 # Modified by Ignacia Fierro-Piccardo 2023.
 
-import warnings
 import numbers
 
-from ufl.core.ufl_type import ufl_type
 from ufl.core.terminal import FormArgument
-from ufl.split_functions import split
-from ufl.finiteelement import FiniteElementBase
-from ufl.domain import default_domain
+from ufl.core.ufl_type import ufl_type
+from ufl.duals import is_dual, is_primal
 from ufl.form import BaseForm
-from ufl.functionspace import AbstractFunctionSpace, FunctionSpace, MixedFunctionSpace
-from ufl.duals import is_primal, is_dual
+from ufl.functionspace import AbstractFunctionSpace, MixedFunctionSpace
+from ufl.split_functions import split
 
 # Export list for ufl.classes (TODO: not actually classes: drop? these are in ufl.*)
 __all_classes__ = ["TestFunction", "TrialFunction", "TestFunctions", "TrialFunctions"]
 
 
 # --- Class representing an argument (basis function) in a form ---
 
+
 class BaseArgument(object):
     """UFL value: Representation of an argument to a form."""
 
     __slots__ = ()
     _ufl_is_abstract_ = True
 
     def __getnewargs__(self):
         """Get new args."""
         return (self._ufl_function_space, self._number, self._part)
 
     def __init__(self, function_space, number, part=None):
-        """initialise."""
-        if isinstance(function_space, FiniteElementBase):
-            # For legacy support for UFL files using cells, we map the cell to
-            # the default Mesh
-            element = function_space
-            domain = default_domain(element.cell())
-            function_space = FunctionSpace(domain, element)
-            warnings.warn("The use of FiniteElement as an input to Argument will be deprecated by December 2023. "
-                          "Please, use FunctionSpace instead", FutureWarning)
-        elif not isinstance(function_space, AbstractFunctionSpace):
-            raise ValueError("Expecting a FunctionSpace or FiniteElement.")
+        """Initialise."""
+        if not isinstance(function_space, AbstractFunctionSpace):
+            raise ValueError("Expecting a FunctionSpace.")
 
         self._ufl_function_space = function_space
-        self._ufl_shape = function_space.ufl_element().value_shape()
+        self._ufl_shape = function_space.value_shape
 
         if not isinstance(number, numbers.Integral):
             raise ValueError(f"Expecting an int for number, not {number}")
         if part is not None and not isinstance(part, numbers.Integral):
             raise ValueError(f"Expecting None or an int for part, not {part}")
         self._number = number
         self._part = part
@@ -101,15 +91,19 @@
         return False
 
     def ufl_domains(self):
         """Return UFL domains."""
         return self._ufl_function_space.ufl_domains()
 
     def _ufl_signature_data_(self, renumbering):
-        """Signature data for form arguments depend on the global numbering of the form arguments and domains."""
+        """Signature data.
+
+        Signature data for form arguments depend on the global numbering
+        of the form arguments and domains.
+        """
         fsdata = self._ufl_function_space._ufl_signature_data_(renumbering)
         return ("Argument", self._number, self._part, fsdata)
 
     def __str__(self):
         """Format as a string."""
         number = str(self._number)
         if len(number) == 1:
@@ -139,16 +133,18 @@
         with a different non-ufl payload, such as dolfin FunctionSpace
         with different mesh. This is necessary because arguments with the
         same element and argument number are always equal from a pure ufl
         point of view, e.g. TestFunction(V1) == TestFunction(V2) if V1 and V2
         are the same ufl element but different dolfin function spaces.
         """
         return (
-            type(self) is type(other) and self._number == other._number and  # noqa: W504
-            self._part == other._part and self._ufl_function_space == other._ufl_function_space
+            type(self) is type(other)
+            and self._number == other._number
+            and self._part == other._part
+            and self._ufl_function_space == other._ufl_function_space
         )
 
 
 @ufl_type()
 class Argument(FormArgument, BaseArgument):
     """UFL value: Representation of an argument to a form."""
 
@@ -176,15 +172,18 @@
 
     def __init__(self, function_space, number, part=None):
         """Initialise."""
         FormArgument.__init__(self)
         BaseArgument.__init__(self, function_space, number, part)
 
         self._repr = "Argument(%s, %s, %s)" % (
-            repr(self._ufl_function_space), repr(self._number), repr(self._part))
+            repr(self._ufl_function_space),
+            repr(self._number),
+            repr(self._part),
+        )
 
     def ufl_domains(self):
         """Return UFL domains."""
         return BaseArgument.ufl_domains(self)
 
     def __repr__(self):
         """Representation."""
@@ -200,51 +199,57 @@
         "_ufl_shape",
         "_arguments",
         "_coefficients",
         "ufl_operands",
         "_number",
         "_part",
         "_repr",
-        "_hash"
+        "_hash",
     )
 
     _primal = False
     _dual = True
 
     def __new__(cls, *args, **kw):
         """Create a new Coargument."""
         if args[0] and is_primal(args[0]):
-            raise ValueError("ufl.Coargument takes in a dual space! If you want to define an argument "
-                             "in the primal space you should use ufl.Argument.")
+            raise ValueError(
+                "ufl.Coargument takes in a dual space! If you want to define an argument "
+                "in the primal space you should use ufl.Argument."
+            )
         return super().__new__(cls)
 
     def __init__(self, function_space, number, part=None):
         """Initialise."""
         BaseArgument.__init__(self, function_space, number, part)
         BaseForm.__init__(self)
 
         self.ufl_operands = ()
         self._hash = None
         self._repr = "Coargument(%s, %s, %s)" % (
-            repr(self._ufl_function_space), repr(self._number), repr(self._part))
+            repr(self._ufl_function_space),
+            repr(self._number),
+            repr(self._part),
+        )
 
     def arguments(self, outer_form=None):
         """Return all Argument objects found in form."""
         if self._arguments is None:
             self._analyze_form_arguments(outer_form=outer_form)
         return self._arguments
 
     def _analyze_form_arguments(self, outer_form=None):
         """Analyze which Argument and Coefficient objects can be found in the form."""
         # Define canonical numbering of arguments and coefficients
         self._coefficients = ()
         # Coarguments map from V* to V*, i.e. V* -> V*, or equivalently V* x V -> R.
         # So they have one argument in the primal space and one in the dual space.
-        # However, when they are composed with linear forms with dual arguments, such as BaseFormOperators,
-        # the primal argument is discarded when analysing the argument as Coarguments.
+        # However, when they are composed with linear forms with dual
+        # arguments, such as BaseFormOperators, the primal argument is
+        # discarded when analysing the argument as Coarguments.
         if not outer_form:
             self._arguments = (Argument(self.ufl_function_space().dual(), 0), self)
         else:
             self._arguments = (self,)
 
     def ufl_domain(self):
         """Return the UFL domain."""
@@ -252,23 +257,24 @@
 
     def equals(self, other):
         """Check equality."""
         if type(other) is not Coargument:
             return False
         if self is other:
             return True
-        return (self._ufl_function_space == other._ufl_function_space and  # noqa: W504
-                self._number == other._number and self._part == other._part)
+        return (
+            self._ufl_function_space == other._ufl_function_space
+            and self._number == other._number
+            and self._part == other._part
+        )
 
     def __hash__(self):
         """Hash."""
-        return hash(("Coargument",
-                     hash(self._ufl_function_space),
-                     self._number,
-                     self._part))
+        return hash(("Coargument", hash(self._ufl_function_space), self._number, self._part))
+
 
 # --- Helper functions for pretty syntax ---
 
 
 def TestFunction(function_space, part=None):
     """UFL value: Create a test function argument to a form."""
     return Argument(function_space, 0, part)
@@ -277,33 +283,38 @@
 def TrialFunction(function_space, part=None):
     """UFL value: Create a trial function argument to a form."""
     return Argument(function_space, 1, part)
 
 
 # --- Helper functions for creating subfunctions on mixed elements ---
 
+
 def Arguments(function_space, number):
     """Create an Argument in a mixed space.
 
     Returns a tuple with the function components corresponding to the subelements.
     """
     if isinstance(function_space, MixedFunctionSpace):
-        return [Argument(function_space.ufl_sub_space(i), number, i)
-                for i in range(function_space.num_sub_spaces())]
+        return [
+            Argument(function_space.ufl_sub_space(i), number, i)
+            for i in range(function_space.num_sub_spaces())
+        ]
     else:
         return split(Argument(function_space, number))
 
 
 def TestFunctions(function_space):
     """Create a TestFunction in a mixed space.
 
-    Returns a tuple with the function components corresponding to the subelements.
+    Returns a tuple with the function components corresponding to the
+    subelements.
     """
     return Arguments(function_space, 0)
 
 
 def TrialFunctions(function_space):
     """Create a TrialFunction in a mixed space.
 
-    Returns a tuple with the function components corresponding to the subelements.
+    Returns a tuple with the function components corresponding to the
+    subelements.
     """
     return Arguments(function_space, 1)
```

### Comparing `fenics-ufl-2023.2.0/ufl/averaging.py` & `fenics_ufl-2024.1.0.post0/ufl/averaging.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 
 # Copyright (C) 2008-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
+from ufl.constantvalue import ConstantValue
 from ufl.core.operator import Operator
 from ufl.core.ufl_type import ufl_type
-from ufl.constantvalue import ConstantValue
 
 
-@ufl_type(inherit_shape_from_operand=0,
-          inherit_indices_from_operand=0,
-          num_ops=1,
-          is_evaluation=True)
+@ufl_type(
+    inherit_shape_from_operand=0, inherit_indices_from_operand=0, num_ops=1, is_evaluation=True
+)
 class CellAvg(Operator):
     """Cell average."""
 
     __slots__ = ()
 
     def __new__(cls, f):
         """Create a new CellAvg."""
@@ -33,26 +32,24 @@
     @property
     def ufl_shape(self):
         """Get the UFL shape."""
         return self.ufl_operands[0].ufl_shape
 
     def evaluate(self, x, mapping, component, index_values):
         """Performs an approximate symbolic evaluation, since we don't have a cell."""
-        return self.ufl_operands[0].evaluate(x, mapping, component,
-                                             index_values)
+        return self.ufl_operands[0].evaluate(x, mapping, component, index_values)
 
     def __str__(self):
         """Format as a string."""
         return f"cell_avg({self.ufl_operands[0]})"
 
 
-@ufl_type(inherit_shape_from_operand=0,
-          inherit_indices_from_operand=0,
-          num_ops=1,
-          is_evaluation=True)
+@ufl_type(
+    inherit_shape_from_operand=0, inherit_indices_from_operand=0, num_ops=1, is_evaluation=True
+)
 class FacetAvg(Operator):
     """Facet average."""
 
     __slots__ = ()
 
     def __new__(cls, f):
         """Create a new FacetAvg."""
```

### Comparing `fenics-ufl-2023.2.0/ufl/cell.py` & `fenics_ufl-2024.1.0.post0/ufl/cell.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,48 +3,48 @@
 # Copyright (C) 2008-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
 from __future__ import annotations
+
 import functools
 import numbers
 import typing
 import weakref
-
-from ufl.core.ufl_type import UFLObject
 from abc import abstractmethod
 
+from ufl.core.ufl_type import UFLObject
 
 __all_classes__ = ["AbstractCell", "Cell", "TensorProductCell"]
 
 
 class AbstractCell(UFLObject):
     """A base class for all cells."""
 
     @abstractmethod
     def topological_dimension(self) -> int:
         """Return the dimension of the topology of this cell."""
 
     @abstractmethod
-    def geometric_dimension(self) -> int:
-        """Return the dimension of the geometry of this cell."""
-
-    @abstractmethod
     def is_simplex(self) -> bool:
         """Return True if this is a simplex cell."""
 
     @abstractmethod
     def has_simplex_facets(self) -> bool:
         """Return True if all the facets of this cell are simplex cells."""
 
     @abstractmethod
     def _lt(self, other) -> bool:
-        """Define an arbitrarily chosen but fixed sort order for all instances of this type with the same dimensions."""
+        """Less than operator.
+
+        Define an arbitrarily chosen but fixed sort order for all
+        instances of this type with the same dimensions.
+        """
 
     @abstractmethod
     def num_sub_entities(self, dim: int) -> int:
         """Get the number of sub-entities of the given dimension."""
 
     @abstractmethod
     def sub_entities(self, dim: int) -> typing.Tuple[AbstractCell, ...]:
@@ -61,16 +61,16 @@
     @abstractmethod
     def reconstruct(self, **kwargs: typing.Any) -> Cell:
         """Reconstruct this cell, overwriting properties by those in kwargs."""
 
     def __lt__(self, other: AbstractCell) -> bool:
         """Define an arbitrarily chosen but fixed sort order for all cells."""
         if type(self) is type(other):
-            s = (self.geometric_dimension(), self.topological_dimension())
-            o = (other.geometric_dimension(), other.topological_dimension())
+            s = self.topological_dimension()
+            o = other.topological_dimension()
             if s != o:
                 return s < o
             return self._lt(other)
         else:
             if type(self).__name__ == type(other).__name__:
                 raise ValueError("Cannot order cell types with the same name")
             return type(self).__name__ < type(other).__name__
@@ -181,76 +181,108 @@
         Peaks are entities of dimension tdim-3.
         """
         tdim = self.topological_dimension()
         return self.sub_entity_types(tdim - 3)
 
 
 _sub_entity_celltypes = {
-    "vertex": [("vertex", )],
-    "interval": [tuple("vertex" for i in range(2)), ("interval", )],
-    "triangle": [tuple("vertex" for i in range(3)), tuple("interval" for i in range(3)), ("triangle", )],
-    "quadrilateral": [tuple("vertex" for i in range(4)), tuple("interval" for i in range(4)), ("quadrilateral", )],
-    "tetrahedron": [tuple("vertex" for i in range(4)), tuple("interval" for i in range(6)),
-                    tuple("triangle" for i in range(4)), ("tetrahedron", )],
-    "hexahedron": [tuple("vertex" for i in range(8)), tuple("interval" for i in range(12)),
-                   tuple("quadrilateral" for i in range(6)), ("hexahedron", )],
-    "prism": [tuple("vertex" for i in range(6)), tuple("interval" for i in range(9)),
-              ("triangle", "quadrilateral", "quadrilateral", "quadrilateral", "triangle"), ("prism", )],
-    "pyramid": [tuple("vertex" for i in range(5)), tuple("interval" for i in range(8)),
-                ("quadrilateral", "triangle", "triangle", "triangle", "triangle"), ("pyramid", )],
-    "pentatope": [tuple("vertex" for i in range(5)), tuple("interval" for i in range(10)),
-                  tuple("triangle" for i in range(10)), tuple("tetrahedron" for i in range(5)), ("pentatope", )],
-    "tesseract": [tuple("vertex" for i in range(16)), tuple("interval" for i in range(32)),
-                  tuple("quadrilateral" for i in range(24)), tuple("hexahedron" for i in range(8)), ("tesseract", )],
+    "vertex": [("vertex",)],
+    "interval": [tuple("vertex" for i in range(2)), ("interval",)],
+    "triangle": [
+        tuple("vertex" for i in range(3)),
+        tuple("interval" for i in range(3)),
+        ("triangle",),
+    ],
+    "quadrilateral": [
+        tuple("vertex" for i in range(4)),
+        tuple("interval" for i in range(4)),
+        ("quadrilateral",),
+    ],
+    "tetrahedron": [
+        tuple("vertex" for i in range(4)),
+        tuple("interval" for i in range(6)),
+        tuple("triangle" for i in range(4)),
+        ("tetrahedron",),
+    ],
+    "hexahedron": [
+        tuple("vertex" for i in range(8)),
+        tuple("interval" for i in range(12)),
+        tuple("quadrilateral" for i in range(6)),
+        ("hexahedron",),
+    ],
+    "prism": [
+        tuple("vertex" for i in range(6)),
+        tuple("interval" for i in range(9)),
+        ("triangle", "quadrilateral", "quadrilateral", "quadrilateral", "triangle"),
+        ("prism",),
+    ],
+    "pyramid": [
+        tuple("vertex" for i in range(5)),
+        tuple("interval" for i in range(8)),
+        ("quadrilateral", "triangle", "triangle", "triangle", "triangle"),
+        ("pyramid",),
+    ],
+    "pentatope": [
+        tuple("vertex" for i in range(5)),
+        tuple("interval" for i in range(10)),
+        tuple("triangle" for i in range(10)),
+        tuple("tetrahedron" for i in range(5)),
+        ("pentatope",),
+    ],
+    "tesseract": [
+        tuple("vertex" for i in range(16)),
+        tuple("interval" for i in range(32)),
+        tuple("quadrilateral" for i in range(24)),
+        tuple("hexahedron" for i in range(8)),
+        ("tesseract",),
+    ],
 }
 
 
 class Cell(AbstractCell):
     """Representation of a named finite element cell with known structure."""
-    __slots__ = ("_cellname", "_tdim", "_gdim", "_num_cell_entities", "_sub_entity_types",
-                 "_sub_entities", "_sub_entity_types")
 
-    def __init__(self, cellname: str, geometric_dimension: typing.Optional[int] = None):
+    __slots__ = (
+        "_cellname",
+        "_tdim",
+        "_num_cell_entities",
+        "_sub_entity_types",
+        "_sub_entities",
+        "_sub_entity_types",
+    )
+
+    def __init__(self, cellname: str):
         """Initialise.
 
         Args:
             cellname: Name of the cell
-            geometric_dimension: Geometric dimension
         """
         if cellname not in _sub_entity_celltypes:
             raise ValueError(f"Unsupported cell type: {cellname}")
 
         self._sub_entity_celltypes = _sub_entity_celltypes[cellname]
 
         self._cellname = cellname
         self._tdim = len(self._sub_entity_celltypes) - 1
-        self._gdim = self._tdim if geometric_dimension is None else geometric_dimension
 
         self._num_cell_entities = [len(i) for i in self._sub_entity_celltypes]
-        self._sub_entities = [tuple(Cell(t, self._gdim) for t in se_types)
-                              for se_types in self._sub_entity_celltypes[:-1]]
+        self._sub_entities = [
+            tuple(Cell(t) for t in se_types) for se_types in self._sub_entity_celltypes[:-1]
+        ]
         self._sub_entity_types = [tuple(set(i)) for i in self._sub_entities]
-        self._sub_entities.append((weakref.proxy(self), ))
-        self._sub_entity_types.append((weakref.proxy(self), ))
+        self._sub_entities.append((weakref.proxy(self),))
+        self._sub_entity_types.append((weakref.proxy(self),))
 
-        if not isinstance(self._gdim, numbers.Integral):
-            raise ValueError("Expecting integer geometric_dimension.")
         if not isinstance(self._tdim, numbers.Integral):
             raise ValueError("Expecting integer topological_dimension.")
-        if self._tdim > self._gdim:
-            raise ValueError("Topological dimension cannot be larger than geometric dimension.")
 
     def topological_dimension(self) -> int:
         """Return the dimension of the topology of this cell."""
         return self._tdim
 
-    def geometric_dimension(self) -> int:
-        """Return the dimension of the geometry of this cell."""
-        return self._gdim
-
     def is_simplex(self) -> bool:
         """Return True if this is a simplex cell."""
         return self._cellname in ["vertex", "interval", "triangle", "tetrahedron"]
 
     def has_simplex_facets(self) -> bool:
         """Return True if all the facets of this cell are simplex cells."""
         return self._cellname in ["interval", "triangle", "quadrilateral", "tetrahedron"]
@@ -287,77 +319,57 @@
 
     def cellname(self) -> str:
         """Return the cellname of the cell."""
         return self._cellname
 
     def __str__(self) -> str:
         """Format as a string."""
-        if self._gdim == self._tdim:
-            return self._cellname
-        else:
-            return f"{self._cellname}{self._gdim}D"
+        return self._cellname
 
     def __repr__(self) -> str:
         """Representation."""
-        if self._gdim == self._tdim:
-            return self._cellname
-        else:
-            return f"Cell({self._cellname}, {self._gdim})"
+        return self._cellname
 
     def _ufl_hash_data_(self) -> typing.Hashable:
         """UFL hash data."""
-        return (self._cellname, self._gdim)
+        return (self._cellname,)
 
     def reconstruct(self, **kwargs: typing.Any) -> Cell:
         """Reconstruct this cell, overwriting properties by those in kwargs."""
-        gdim = self._gdim
         for key, value in kwargs.items():
-            if key == "geometric_dimension":
-                gdim = value
-            else:
-                raise TypeError(f"reconstruct() got unexpected keyword argument '{key}'")
-        return Cell(self._cellname, geometric_dimension=gdim)
+            raise TypeError(f"reconstruct() got unexpected keyword argument '{key}'")
+        return Cell(self._cellname)
 
 
 class TensorProductCell(AbstractCell):
     """Tensor product cell."""
 
-    __slots__ = ("_cells", "_tdim", "_gdim")
+    __slots__ = ("_cells", "_tdim")
 
-    def __init__(self, *cells: Cell, geometric_dimension: typing.Optional[int] = None):
+    def __init__(self, *cells: Cell):
         """Initialise.
 
         Args:
             cells: Cells to take the tensor product of
-            geometric_dimension: Geometric dimension
         """
         self._cells = tuple(as_cell(cell) for cell in cells)
 
         self._tdim = sum([cell.topological_dimension() for cell in self._cells])
-        self._gdim = self._tdim if geometric_dimension is None else geometric_dimension
 
-        if not isinstance(self._gdim, numbers.Integral):
-            raise ValueError("Expecting integer geometric_dimension.")
         if not isinstance(self._tdim, numbers.Integral):
             raise ValueError("Expecting integer topological_dimension.")
-        if self._tdim > self._gdim:
-            raise ValueError("Topological dimension cannot be larger than geometric dimension.")
 
     def sub_cells(self) -> typing.List[AbstractCell]:
         """Return list of cell factors."""
         return self._cells
 
     def topological_dimension(self) -> int:
         """Return the dimension of the topology of this cell."""
         return self._tdim
 
-    def geometric_dimension(self) -> int:
-        """Return the dimension of the geometry of this cell."""
-        return self._gdim
-
     def is_simplex(self) -> bool:
         """Return True if this is a simplex cell."""
         if len(self._cells) == 1:
             return self._cells[0].is_simplex()
         return False
 
     def has_simplex_facets(self) -> bool:
@@ -371,103 +383,95 @@
     def num_sub_entities(self, dim: int) -> int:
         """Get the number of sub-entities of the given dimension."""
         if dim < 0 or dim > self._tdim:
             return 0
         if dim == 0:
             return functools.reduce(lambda x, y: x * y, [c.num_vertices() for c in self._cells])
         if dim == self._tdim - 1:
-            # Note: This is not the number of facets that the cell has, but I'm leaving it here for now
-            # to not change past behaviour
+            # Note: This is not the number of facets that the cell has,
+            # but I'm leaving it here for now to not change past
+            # behaviour
             return sum(c.num_facets() for c in self._cells if c.topological_dimension() > 0)
         if dim == self._tdim:
             return 1
         raise NotImplementedError(f"TensorProductCell.num_sub_entities({dim}) is not implemented.")
 
     def sub_entities(self, dim: int) -> typing.Tuple[AbstractCell, ...]:
         """Get the sub-entities of the given dimension."""
         if dim < 0 or dim > self._tdim:
             return []
         if dim == 0:
-            return [Cell("vertex", self._gdim) for i in range(self.num_sub_entities(0))]
+            return [Cell("vertex") for i in range(self.num_sub_entities(0))]
         if dim == self._tdim:
             return [self]
         raise NotImplementedError(f"TensorProductCell.sub_entities({dim}) is not implemented.")
 
     def sub_entity_types(self, dim: int) -> typing.Tuple[AbstractCell, ...]:
         """Get the unique sub-entity types of the given dimension."""
         if dim < 0 or dim > self._tdim:
             return []
         if dim == 0:
-            return [Cell("vertex", self._gdim)]
+            return [Cell("vertex")]
         if dim == self._tdim:
             return [self]
         raise NotImplementedError(f"TensorProductCell.sub_entities({dim}) is not implemented.")
 
     def _lt(self, other) -> bool:
         return self._ufl_hash_data_() < other._ufl_hash_data_()
 
     def cellname(self) -> str:
         """Return the cellname of the cell."""
         return " * ".join([cell.cellname() for cell in self._cells])
 
     def __str__(self) -> str:
         """Format as a string."""
-        s = "TensorProductCell("
-        s += ", ".join(f"{c!r}" for c in self._cells)
-        if self._tdim != self._gdim:
-            s += f", geometric_dimension={self._gdim}"
-        s += ")"
-        return s
+        return "TensorProductCell(" + ", ".join(f"{c!r}" for c in self._cells) + ")"
 
     def __repr__(self) -> str:
         """Representation."""
         return str(self)
 
     def _ufl_hash_data_(self) -> typing.Hashable:
         """UFL hash data."""
-        return tuple(c._ufl_hash_data_() for c in self._cells) + (self._gdim,)
+        return tuple(c._ufl_hash_data_() for c in self._cells)
 
     def reconstruct(self, **kwargs: typing.Any) -> Cell:
         """Reconstruct this cell, overwriting properties by those in kwargs."""
-        gdim = self._gdim
         for key, value in kwargs.items():
-            if key == "geometric_dimension":
-                gdim = value
-            else:
-                raise TypeError(f"reconstruct() got unexpected keyword argument '{key}'")
-        return TensorProductCell(*self._cells, geometric_dimension=gdim)
+            raise TypeError(f"reconstruct() got unexpected keyword argument '{key}'")
+        return TensorProductCell(*self._cells)
 
 
-def simplex(topological_dimension: int, geometric_dimension: typing.Optional[int] = None):
+def simplex(topological_dimension: int):
     """Return a simplex cell of the given dimension."""
     if topological_dimension == 0:
-        return Cell("vertex", geometric_dimension)
+        return Cell("vertex")
     if topological_dimension == 1:
-        return Cell("interval", geometric_dimension)
+        return Cell("interval")
     if topological_dimension == 2:
-        return Cell("triangle", geometric_dimension)
+        return Cell("triangle")
     if topological_dimension == 3:
-        return Cell("tetrahedron", geometric_dimension)
+        return Cell("tetrahedron")
     if topological_dimension == 4:
-        return Cell("pentatope", geometric_dimension)
+        return Cell("pentatope")
     raise ValueError(f"Unsupported topological dimension for simplex: {topological_dimension}")
 
 
-def hypercube(topological_dimension, geometric_dimension=None):
+def hypercube(topological_dimension: int):
     """Return a hypercube cell of the given dimension."""
     if topological_dimension == 0:
-        return Cell("vertex", geometric_dimension)
+        return Cell("vertex")
     if topological_dimension == 1:
-        return Cell("interval", geometric_dimension)
+        return Cell("interval")
     if topological_dimension == 2:
-        return Cell("quadrilateral", geometric_dimension)
+        return Cell("quadrilateral")
     if topological_dimension == 3:
-        return Cell("hexahedron", geometric_dimension)
+        return Cell("hexahedron")
     if topological_dimension == 4:
-        return Cell("tesseract", geometric_dimension)
+        return Cell("tesseract")
     raise ValueError(f"Unsupported topological dimension for hypercube: {topological_dimension}")
 
 
 def as_cell(cell: typing.Union[AbstractCell, str, typing.Tuple[AbstractCell, ...]]) -> AbstractCell:
     """Convert any valid object to a Cell or return cell if it is already a Cell.
 
     Allows an already valid cell, a known cellname string, or a tuple of cells for a product cell.
```

### Comparing `fenics-ufl-2023.2.0/ufl/checks.py` & `fenics_ufl-2024.1.0.post0/ufl/checks.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,71 +5,58 @@
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Anders Logg, 2008-2009
 
 from ufl.core.expr import Expr
+from ufl.core.terminal import FormArgument
 from ufl.corealg.traversal import traverse_unique_terminals
+from ufl.geometry import GeometricQuantity
+from ufl.sobolevspace import H1
 
 
 def is_python_scalar(expression):
     """Return True iff expression is of a Python scalar type."""
     return isinstance(expression, (int, float, complex))
 
 
 def is_ufl_scalar(expression):
     """Return True iff expression is scalar-valued, but possibly containing free indices."""
     return isinstance(expression, Expr) and not expression.ufl_shape
 
 
 def is_true_ufl_scalar(expression):
     """Return True iff expression is scalar-valued, with no free indices."""
-    return isinstance(expression, Expr) and not (expression.ufl_shape or expression.ufl_free_indices)
+    return isinstance(expression, Expr) and not (
+        expression.ufl_shape or expression.ufl_free_indices
+    )
 
 
 def is_cellwise_constant(expr):
     """Return whether expression is constant over a single cell."""
     # TODO: Implement more accurately considering e.g. derivatives?
-    return all(t.is_cellwise_constant() for t in traverse_unique_terminals(expr))
+    return all(e.is_cellwise_constant() for e in traverse_unique_terminals(expr))
 
 
-def is_globally_constant(expr):
-    """Check if an expression is globally constant.
+def is_scalar_constant_expression(expr):
+    """Check if an expression is a globally constant scalar expression."""
+    if is_python_scalar(expr):
+        return True
+    if expr.ufl_shape:
+        return False
 
-    This includes spatially independent constant coefficients that
-    are not known before assembly time.
-    """
     # TODO: This does not consider gradients of coefficients, so false
     # negatives are possible.
-    # from ufl.argument import Argument
-    # from ufl.coefficient import Coefficient
-    from ufl.core.terminal import FormArgument
-    from ufl.geometry import GeometricQuantity
     for e in traverse_unique_terminals(expr):
         # Return False if any single terminal is not constant
-        if e._ufl_is_literal_:
-            # Accept literals first, they are the most common
-            # terminals
-            continue
-        elif isinstance(e, FormArgument):
-            # Accept only Real valued Arguments and Coefficients
-            if e.ufl_element()._is_globally_constant():
-                continue
-            else:
+        if isinstance(e, FormArgument):
+            # Accept only globally constant Arguments and Coefficients
+            if e.ufl_element().embedded_superdegree > 0 or e.ufl_element() not in H1:
                 return False
         elif isinstance(e, GeometricQuantity):
             # Reject all geometric quantities, they all vary over
             # cells
             return False
 
     # All terminals passed constant check
     return True
-
-
-def is_scalar_constant_expression(expr):
-    """Check if an expression is a globally constant scalar expression."""
-    if is_python_scalar(expr):
-        return True
-    if expr.ufl_shape:
-        return False
-    return is_globally_constant(expr)
```

### Comparing `fenics-ufl-2023.2.0/ufl/classes.py` & `fenics_ufl-2024.1.0.post0/ufl/classes.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,50 +15,50 @@
 # Modified by Anders Logg, 2009.
 # Modified by Kristian B. Oelgaard, 2011
 # Modified by Andrew T. T. McRae, 2014
 
 # This will be populated part by part below
 __all__ = []
 
-
 # Import all submodules, triggering execution of the ufl_type class
 # decorator for each Expr class.
 
-# Base classes of Expr type hierarchy
-import ufl.core.expr
-import ufl.core.terminal
-import ufl.core.operator
-
-# Terminal types
-import ufl.constantvalue
+import ufl.algebra
 import ufl.argument
+import ufl.averaging
+import ufl.cell
 import ufl.coefficient
+import ufl.conditional
+import ufl.constantvalue
+import ufl.core.expr
+import ufl.core.multiindex
+import ufl.core.operator
+import ufl.core.terminal
+import ufl.differentiation
+import ufl.domain
+import ufl.equation
+import ufl.exprcontainers
+import ufl.finiteelement
+import ufl.form
+import ufl.functionspace
 import ufl.geometry
-
-# Operator types
-import ufl.averaging
 import ufl.indexed
 import ufl.indexsum
-import ufl.variable
-import ufl.tensors
-import ufl.algebra
-import ufl.tensoralgebra
+import ufl.integral
 import ufl.mathfunctions
-import ufl.differentiation
-import ufl.conditional
-import ufl.restriction
-import ufl.exprcontainers
+import ufl.measure
+import ufl.pullback
 import ufl.referencevalue
-
-# Make sure we import exproperators which attaches special functions
-# to Expr
+import ufl.restriction
+import ufl.sobolevspace
+import ufl.tensoralgebra
+import ufl.tensors
+import ufl.variable
 from ufl import exproperators as __exproperators
 
-# Make sure to import modules with new Expr subclasses here!
-
 # Collect all classes in sets automatically classified by some properties
 all_ufl_classes = set(ufl.core.expr.Expr._ufl_all_classes_)
 abstract_classes = set(c for c in all_ufl_classes if c._ufl_is_abstract_)
 ufl_classes = set(c for c in all_ufl_classes if not c._ufl_is_abstract_)
 terminal_classes = set(c for c in all_ufl_classes if c._ufl_is_terminal_)
 nonterminal_classes = set(c for c in all_ufl_classes if not c._ufl_is_terminal_)
 
@@ -84,44 +84,28 @@
 
 
 __all__ += populate_namespace_with_expr_classes(locals())
 
 
 # Semi-automated imports of non-expr classes:
 
+
 def populate_namespace_with_module_classes(mod, loc):
     """Export the classes that submodules list in __all_classes__."""
     names = mod.__all_classes__
     for name in names:
         loc[name] = getattr(mod, name)
     return names
 
 
-import ufl.cell  # noqa E401
 __all__ += populate_namespace_with_module_classes(ufl.cell, locals())
-
-import ufl.finiteelement  # noqa E401
 __all__ += populate_namespace_with_module_classes(ufl.finiteelement, locals())
-
-import ufl.domain  # noqa E401
 __all__ += populate_namespace_with_module_classes(ufl.domain, locals())
-
-import ufl.functionspace  # noqa E401
 __all__ += populate_namespace_with_module_classes(ufl.functionspace, locals())
-
-import ufl.core.multiindex  # noqa E401
 __all__ += populate_namespace_with_module_classes(ufl.core.multiindex, locals())
-
-import ufl.argument  # noqa E401
 __all__ += populate_namespace_with_module_classes(ufl.argument, locals())
-
-import ufl.measure  # noqa E401
 __all__ += populate_namespace_with_module_classes(ufl.measure, locals())
-
-import ufl.integral  # noqa E401
 __all__ += populate_namespace_with_module_classes(ufl.integral, locals())
-
-import ufl.form  # noqa E401
 __all__ += populate_namespace_with_module_classes(ufl.form, locals())
-
-import ufl.equation  # noqa E401
 __all__ += populate_namespace_with_module_classes(ufl.equation, locals())
+__all__ += populate_namespace_with_module_classes(ufl.pullback, locals())
+__all__ += populate_namespace_with_module_classes(ufl.sobolevspace, locals())
```

### Comparing `fenics-ufl-2023.2.0/ufl/coefficient.py` & `fenics_ufl-2024.1.0.post0/ufl/coefficient.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,23 @@
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Anders Logg, 2008-2009.
 # Modified by Massimiliano Leoni, 2016.
 # Modified by Cecile Daversin-Catty, 2018.
 # Modified by Ignacia Fierro-Piccardo 2023.
-import warnings
 
-from ufl.core.ufl_type import ufl_type
-from ufl.core.terminal import FormArgument
 from ufl.argument import Argument
-from ufl.finiteelement import FiniteElementBase
-from ufl.domain import default_domain
-from ufl.functionspace import AbstractFunctionSpace, FunctionSpace, MixedFunctionSpace
+from ufl.core.terminal import FormArgument
+from ufl.core.ufl_type import ufl_type
+from ufl.duals import is_dual, is_primal
 from ufl.form import BaseForm
+from ufl.functionspace import AbstractFunctionSpace, MixedFunctionSpace
 from ufl.split_functions import split
 from ufl.utils.counted import Counted
-from ufl.duals import is_primal, is_dual
-
 
 # --- The Coefficient class represents a coefficient in a form ---
 
 
 class BaseCoefficient(Counted):
     """UFL form argument type: Parent Representation of a form coefficient."""
 
@@ -41,30 +37,21 @@
         """Get new args."""
         return (self._ufl_function_space, self._count)
 
     def __init__(self, function_space, count=None):
         """Initalise."""
         Counted.__init__(self, count, Coefficient)
 
-        if isinstance(function_space, FiniteElementBase):
-            # For legacy support for .ufl files using cells, we map
-            # the cell to The Default Mesh
-            element = function_space
-            domain = default_domain(element.cell())
-            function_space = FunctionSpace(domain, element)
-            warnings.warn("The use of FiniteElement as an input to Coefficient will be deprecated by December 2023. "
-                          "Please, use FunctionSpace instead", FutureWarning)
-        elif not isinstance(function_space, AbstractFunctionSpace):
-            raise ValueError("Expecting a FunctionSpace or FiniteElement.")
+        if not isinstance(function_space, AbstractFunctionSpace):
+            raise ValueError("Expecting a FunctionSpace.")
 
         self._ufl_function_space = function_space
-        self._ufl_shape = function_space.ufl_element().value_shape()
+        self._ufl_shape = function_space.value_shape
 
-        self._repr = "BaseCoefficient(%s, %s)" % (
-            repr(self._ufl_function_space), repr(self._count))
+        self._repr = "BaseCoefficient(%s, %s)" % (repr(self._ufl_function_space), repr(self._count))
 
     @property
     def ufl_shape(self):
         """Return the associated UFL shape."""
         return self._ufl_shape
 
     def ufl_function_space(self):
@@ -84,15 +71,19 @@
         return self.ufl_element().is_cellwise_constant()
 
     def ufl_domains(self):
         """Return tuple of domains related to this terminal object."""
         return self._ufl_function_space.ufl_domains()
 
     def _ufl_signature_data_(self, renumbering):
-        """Signature data for form arguments depend on the global numbering of the form arguments and domains."""
+        """Signature data.
+
+        Signature data for form arguments depend on the global numbering
+        of the form arguments and domains.
+        """
         count = renumbering[self]
         fsdata = self._ufl_function_space._ufl_signature_data_(renumbering)
         return ("Coefficient", count, fsdata)
 
     def __str__(self):
         """Format as a string."""
         return f"w_{self._count}"
@@ -119,49 +110,50 @@
         "_counted_class",
         "_arguments",
         "_coefficients",
         "_ufl_function_space",
         "ufl_operands",
         "_repr",
         "_ufl_shape",
-        "_hash"
+        "_hash",
     )
     _primal = False
     _dual = True
 
+    __eq__ = BaseForm.__eq__
+
     def __new__(cls, *args, **kw):
         """Create a new Cofunction."""
         if args[0] and is_primal(args[0]):
-            raise ValueError("ufl.Cofunction takes in a dual space. If you want to define a coefficient "
-                             "in the primal space you should use ufl.Coefficient.")
+            raise ValueError(
+                "ufl.Cofunction takes in a dual space. If you want to define a coefficient "
+                "in the primal space you should use ufl.Coefficient."
+            )
         return super().__new__(cls)
 
     def __init__(self, function_space, count=None):
         """Initialise."""
         BaseCoefficient.__init__(self, function_space, count)
         BaseForm.__init__(self)
 
         self.ufl_operands = ()
         self._hash = None
-        self._repr = "Cofunction(%s, %s)" % (
-            repr(self._ufl_function_space), repr(self._count))
+        self._repr = "Cofunction(%s, %s)" % (repr(self._ufl_function_space), repr(self._count))
 
     def equals(self, other):
         """Check equality."""
         if type(other) is not Cofunction:
             return False
         if self is other:
             return True
         return self._count == other._count and self._ufl_function_space == other._ufl_function_space
 
     def __hash__(self):
         """Hash."""
-        return hash(("Cofunction",
-                     hash(self._ufl_function_space),
-                     self._count))
+        return hash(("Cofunction", hash(self._ufl_function_space), self._count))
 
     def _analyze_form_arguments(self):
         """Analyze which Argument and Coefficient objects can be found in the form."""
         # Define canonical numbering of arguments and coefficients
         # Cofunctions have one argument in primal space as they map from V to R.
         self._arguments = (Argument(self._ufl_function_space.dual(), 0),)
         self._coefficients = (self,)
@@ -186,16 +178,15 @@
         return super().__new__(cls)
 
     def __init__(self, function_space, count=None):
         """Initialise."""
         FormArgument.__init__(self)
         BaseCoefficient.__init__(self, function_space, count)
 
-        self._repr = "Coefficient(%s, %s)" % (
-            repr(self._ufl_function_space), repr(self._count))
+        self._repr = "Coefficient(%s, %s)" % (repr(self._ufl_function_space), repr(self._count))
 
     def ufl_domains(self):
         """Get the UFL domains."""
         return BaseCoefficient.ufl_domains(self)
 
     def __eq__(self, other):
         """Check equality."""
@@ -208,17 +199,20 @@
     def __repr__(self):
         """Representation."""
         return self._repr
 
 
 # --- Helper functions for subfunctions on mixed elements ---
 
+
 def Coefficients(function_space):
     """Create a Coefficient in a mixed space.
 
     Returns a tuple with the function components corresponding to the subelements.
     """
     if isinstance(function_space, MixedFunctionSpace):
-        return [Coefficient(fs) if is_primal(fs) else Cofunction(fs)
-                for fs in function_space.num_sub_spaces()]
+        return [
+            Coefficient(fs) if is_primal(fs) else Cofunction(fs)
+            for fs in function_space.num_sub_spaces()
+        ]
     else:
         return split(Coefficient(function_space))
```

### Comparing `fenics-ufl-2023.2.0/ufl/conditional.py` & `fenics_ufl-2024.1.0.post0/ufl/conditional.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
 import warnings
 
+from ufl.checks import is_true_ufl_scalar
+from ufl.constantvalue import as_ufl
 from ufl.core.expr import ufl_err_str
-from ufl.core.ufl_type import ufl_type
 from ufl.core.operator import Operator
-from ufl.constantvalue import as_ufl
-from ufl.precedence import parstr
+from ufl.core.ufl_type import ufl_type
 from ufl.exprequals import expr_equals
-from ufl.checks import is_true_ufl_scalar
+from ufl.precedence import parstr
 
 # --- Condition classes ---
 
 # TODO: Would be nice with some kind of type system to show that this
 # is a boolean type not a float type
 
 
@@ -39,32 +39,32 @@
     __nonzero__ = __bool__
 
 
 @ufl_type(is_abstract=True, num_ops=2)
 class BinaryCondition(Condition):
     """Binary condition."""
 
-    __slots__ = ('_name',)
+    __slots__ = ("_name",)
 
     def __init__(self, name, left, right):
         """Initialise."""
         left = as_ufl(left)
         right = as_ufl(right)
 
         Condition.__init__(self, (left, right))
 
         self._name = name
 
-        if name in ('!=', '=='):
+        if name in ("!=", "=="):
             # Since equals and not-equals are used for comparing
             # representations, we have to allow any shape here. The
             # scalar properties must be checked when used in
             # conditional instead!
             pass
-        elif name in ('&&', '||'):
+        elif name in ("&&", "||"):
             # Binary operators acting on boolean expressions allow
             # only conditions
             for arg in (left, right):
                 if not isinstance(arg, Condition):
                     raise ValueError(f"Expecting a Condition, not {ufl_err_str(arg)}.")
         else:
             # Binary operators acting on non-boolean expressions allow
@@ -72,16 +72,19 @@
             if left.ufl_shape != () or right.ufl_shape != ():
                 raise ValueError("Expecting scalar arguments.")
             if left.ufl_free_indices != () or right.ufl_free_indices != ():
                 raise ValueError("Expecting scalar arguments.")
 
     def __str__(self):
         """Format as a string."""
-        return "%s %s %s" % (parstr(self.ufl_operands[0], self),
-                             self._name, parstr(self.ufl_operands[1], self))
+        return "%s %s %s" % (
+            parstr(self.ufl_operands[0], self),
+            self._name,
+            parstr(self.ufl_operands[1], self),
+        )
 
 
 # Not associating with __eq__, the concept of equality with == is
 # reserved for object equivalence for use in set and dict.
 @ufl_type()
 class EQ(BinaryCondition):
     """Equality condition."""
@@ -250,43 +253,46 @@
         return bool(not a)
 
     def __str__(self):
         """Format as a string."""
         return "!(%s)" % (str(self.ufl_operands[0]),)
 
 
-@ufl_type(num_ops=3, inherit_shape_from_operand=1,
-          inherit_indices_from_operand=1)
+@ufl_type(num_ops=3, inherit_shape_from_operand=1, inherit_indices_from_operand=1)
 class Conditional(Operator):
     """Conditional expression.
 
     In C++ these take the format `(condition ? true_value : false_value)`.
     """
 
     __slots__ = ()
 
     def __init__(self, condition, true_value, false_value):
         """Initialise."""
         if not isinstance(condition, Condition):
-            raise ValueError("Expectiong condition as first argument.")
+            raise ValueError("Expecting condition as first argument.")
         true_value = as_ufl(true_value)
         false_value = as_ufl(false_value)
         tsh = true_value.ufl_shape
         fsh = false_value.ufl_shape
         if tsh != fsh:
             raise ValueError("Shape mismatch between conditional branches.")
         tfi = true_value.ufl_free_indices
         ffi = false_value.ufl_free_indices
         if tfi != ffi:
             raise ValueError("Free index mismatch between conditional branches.")
         if isinstance(condition, (EQ, NE)):
-            if not all((condition.ufl_operands[0].ufl_shape == (),
-                        condition.ufl_operands[0].ufl_free_indices == (),
-                        condition.ufl_operands[1].ufl_shape == (),
-                        condition.ufl_operands[1].ufl_free_indices == ())):
+            if not all(
+                (
+                    condition.ufl_operands[0].ufl_shape == (),
+                    condition.ufl_operands[0].ufl_free_indices == (),
+                    condition.ufl_operands[1].ufl_shape == (),
+                    condition.ufl_operands[1].ufl_free_indices == (),
+                )
+            ):
                 raise ValueError("Non-scalar == or != is not allowed.")
 
         Operator.__init__(self, (condition, true_value, false_value))
 
     def evaluate(self, x, mapping, component, index_values):
         """Evaluate."""
         c = self.ufl_operands[0].evaluate(x, mapping, component, index_values)
@@ -299,14 +305,15 @@
     def __str__(self):
         """Format as a string."""
         return "%s ? %s : %s" % tuple(parstr(o, self) for o in self.ufl_operands)
 
 
 # --- Specific functions higher level than a conditional ---
 
+
 @ufl_type(is_scalar=True, num_ops=1)
 class MinValue(Operator):
     """Take the minimum of two values."""
 
     __slots__ = ()
 
     def __init__(self, left, right):
@@ -319,15 +326,15 @@
         """Evaluate."""
         a, b = self.ufl_operands
         a = a.evaluate(x, mapping, component, index_values)
         b = b.evaluate(x, mapping, component, index_values)
         try:
             res = min(a, b)
         except ValueError:
-            warnings.warn('Value error in evaluation of min() of %s and %s.' % self.ufl_operands)
+            warnings.warn("Value error in evaluation of min() of %s and %s." % self.ufl_operands)
             raise
         return res
 
     def __str__(self):
         """Format as a string."""
         return "min_value(%s, %s)" % self.ufl_operands
 
@@ -348,14 +355,14 @@
         """Evaluate."""
         a, b = self.ufl_operands
         a = a.evaluate(x, mapping, component, index_values)
         b = b.evaluate(x, mapping, component, index_values)
         try:
             res = max(a, b)
         except ValueError:
-            warnings.warn('Value error in evaluation of max() of %s and %s.' % self.ufl_operands)
+            warnings.warn("Value error in evaluation of max() of %s and %s." % self.ufl_operands)
             raise
         return res
 
     def __str__(self):
         """Format as a string."""
         return "max_value(%s, %s)" % self.ufl_operands
```

### Comparing `fenics-ufl-2023.2.0/ufl/constant.py` & `fenics_ufl-2024.1.0.post0/ufl/constant.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-"""This module defines classes representing non-literal values which are constant with respect to a domain."""
+"""Support fpr non-literal values which are constant with respect to a domain."""
 
 # Copyright (C) 2019 Michal Habera
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
-from ufl.core.ufl_type import ufl_type
 from ufl.core.terminal import Terminal
+from ufl.core.ufl_type import ufl_type
 from ufl.domain import as_domain
 from ufl.utils.counted import Counted
 
 
 @ufl_type()
 class Constant(Terminal, Counted):
     """Constant."""
@@ -25,28 +25,29 @@
 
         self._ufl_domain = as_domain(domain)
         self._ufl_shape = shape
 
         # Repr string is build in such way, that reconstruction
         # with eval() is possible
         self._repr = "Constant({}, {}, {})".format(
-            repr(self._ufl_domain), repr(self._ufl_shape), repr(self._count))
+            repr(self._ufl_domain), repr(self._ufl_shape), repr(self._count)
+        )
 
     @property
     def ufl_shape(self):
         """Get the UFL shape."""
         return self._ufl_shape
 
     def ufl_domain(self):
         """Get the UFL domain."""
         return self._ufl_domain
 
     def ufl_domains(self):
         """Get the UFL domains."""
-        return (self.ufl_domain(), )
+        return (self.ufl_domain(),)
 
     def is_cellwise_constant(self):
         """Return True if the function is cellwise constant."""
         return True
 
     def __str__(self):
         """Format as a string."""
@@ -58,27 +59,34 @@
 
     def __eq__(self, other):
         """Check equality."""
         if not isinstance(other, Constant):
             return False
         if self is other:
             return True
-        return (self._count == other._count and self._ufl_domain == other._ufl_domain and   # noqa: W504
-                self._ufl_shape == self._ufl_shape)
+        return (
+            self._count == other._count
+            and self._ufl_domain == other._ufl_domain
+            and self._ufl_shape == self._ufl_shape
+        )
 
     def _ufl_signature_data_(self, renumbering):
         """Signature data for constant depends on renumbering."""
         return "Constant({}, {}, {})".format(
-            self._ufl_domain._ufl_signature_data_(renumbering), repr(self._ufl_shape),
-            repr(renumbering[self]))
+            self._ufl_domain._ufl_signature_data_(renumbering),
+            repr(self._ufl_shape),
+            repr(renumbering[self]),
+        )
 
 
 def VectorConstant(domain, count=None):
     """Vector constant."""
     domain = as_domain(domain)
-    return Constant(domain, shape=(domain.geometric_dimension(), ), count=count)
+    return Constant(domain, shape=(domain.geometric_dimension(),), count=count)
 
 
 def TensorConstant(domain, count=None):
     """Tensor constant."""
     domain = as_domain(domain)
-    return Constant(domain, shape=(domain.geometric_dimension(), domain.geometric_dimension()), count=count)
+    return Constant(
+        domain, shape=(domain.geometric_dimension(), domain.geometric_dimension()), count=count
+    )
```

### Comparing `fenics-ufl-2023.2.0/ufl/constantvalue.py` & `fenics_ufl-2024.1.0.post0/ufl/constantvalue.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,37 +8,37 @@
 #
 # Modified by Anders Logg, 2011.
 # Modified by Massimiliano Leoni, 2016.
 
 from math import atan2
 
 import ufl
+
+# --- Helper functions imported here for compatibility---
+from ufl.checks import is_python_scalar, is_true_ufl_scalar, is_ufl_scalar  # noqa: F401
 from ufl.core.expr import Expr
+from ufl.core.multiindex import FixedIndex, Index
 from ufl.core.terminal import Terminal
-from ufl.core.multiindex import Index, FixedIndex
 from ufl.core.ufl_type import ufl_type
 
-# --- Helper functions imported here for compatibility---
-from ufl.checks import is_python_scalar, is_ufl_scalar, is_true_ufl_scalar  # noqa: F401
-
-
 # Precision for float formatting
 precision = None
 
 
 def format_float(x):
     """Format float value based on global UFL precision."""
     if precision:
         return "{:.{prec}}".format(float(x), prec=precision)
     else:
         return "{}".format(float(x))
 
 
 # --- Base classes for constant types ---
 
+
 @ufl_type(is_abstract=True)
 class ConstantValue(Terminal):
     """Constant value."""
 
     __slots__ = ()
 
     def __init__(self):
@@ -97,24 +97,31 @@
             raise ValueError(f"Expecting tuple for free_indices, not {free_indices}.")
 
         self.ufl_shape = shape
         if not free_indices:
             self.ufl_free_indices = ()
             self.ufl_index_dimensions = ()
         elif all(isinstance(i, Index) for i in free_indices):  # Handle old input format
-            if not isinstance(index_dimensions, dict) and all(isinstance(i, Index) for i in index_dimensions.keys()):
+            if not isinstance(index_dimensions, dict) and all(
+                isinstance(i, Index) for i in index_dimensions.keys()
+            ):
                 raise ValueError(f"Expecting tuple of index dimensions, not {index_dimensions}")
             self.ufl_free_indices = tuple(sorted(i.count() for i in free_indices))
             self.ufl_index_dimensions = tuple(
-                d for i, d in sorted(index_dimensions.items(), key=lambda x: x[0].count()))
+                d for i, d in sorted(index_dimensions.items(), key=lambda x: x[0].count())
+            )
         else:  # Handle new input format
             if not all(isinstance(i, int) for i in free_indices):
                 raise ValueError(f"Expecting tuple of integer free index ids, not {free_indices}")
-            if not isinstance(index_dimensions, tuple) and all(isinstance(i, int) for i in index_dimensions):
-                raise ValueError(f"Expecting tuple of integer index dimensions, not {index_dimensions}")
+            if not isinstance(index_dimensions, tuple) and all(
+                isinstance(i, int) for i in index_dimensions
+            ):
+                raise ValueError(
+                    f"Expecting tuple of integer index dimensions, not {index_dimensions}"
+                )
 
             # Assuming sorted now to avoid this cost, enable for debugging:
             # if sorted(free_indices) != list(free_indices):
             #    raise ValueError("Expecting sorted input. Remove this check later for efficiency.")
 
             self.ufl_free_indices = free_indices
             self.ufl_index_dimensions = index_dimensions
@@ -134,25 +141,28 @@
         return "0 (shape %s, index labels %s)" % (self.ufl_shape, self.ufl_free_indices)
 
     def __repr__(self):
         """Representation."""
         r = "Zero(%s, %s, %s)" % (
             repr(self.ufl_shape),
             repr(self.ufl_free_indices),
-            repr(self.ufl_index_dimensions))
+            repr(self.ufl_index_dimensions),
+        )
         return r
 
     def __eq__(self, other):
         """Check equalty."""
         if isinstance(other, Zero):
             if self is other:
                 return True
-            return (self.ufl_shape == other.ufl_shape and  # noqa: W504
-                    self.ufl_free_indices == other.ufl_free_indices and  # noqa: W504
-                    self.ufl_index_dimensions == other.ufl_index_dimensions)
+            return (
+                self.ufl_shape == other.ufl_shape
+                and self.ufl_free_indices == other.ufl_free_indices
+                and self.ufl_index_dimensions == other.ufl_index_dimensions
+            )
         elif isinstance(other, (int, float)):
             return other == 0
         else:
             return False
 
     def __neg__(self):
         """Negate."""
@@ -187,14 +197,15 @@
         return Zero(shape[0])
     else:
         return Zero(shape)
 
 
 # --- Scalar value types ---
 
+
 @ufl_type(is_abstract=True, is_scalar=True)
 class ScalarValue(ConstantValue):
     """A constant scalar value."""
 
     __slots__ = ("_value",)
 
     def __init__(self, value):
@@ -343,14 +354,15 @@
         r = "%s(%s)" % (type(self).__name__, format_float(self._value))
         return r
 
 
 @ufl_type(wraps_type=int, is_literal=True)
 class IntValue(RealValue):
     """Representation of a constant scalar integer value."""
+
     __slots__ = ()
 
     _cache = {}
 
     def __getnewargs__(self):
         """Get new args."""
         return (self._value,)
@@ -385,17 +397,19 @@
         """Representation."""
         r = "%s(%s)" % (type(self).__name__, repr(self._value))
         return r
 
 
 # --- Identity matrix ---
 
+
 @ufl_type()
 class Identity(ConstantValue):
     """Representation of an identity matrix."""
+
     __slots__ = ("_dim", "ufl_shape")
 
     def __init__(self, dim):
         """Initialise."""
         ConstantValue.__init__(self)
         self._dim = dim
         self.ufl_shape = (dim, dim)
@@ -425,14 +439,15 @@
     def __eq__(self, other):
         """Check equalty."""
         return isinstance(other, Identity) and self._dim == other._dim
 
 
 # --- Permutation symbol ---
 
+
 @ufl_type()
 class PermutationSymbol(ConstantValue):
     """Representation of a permutation symbol.
 
     This is also known as the Levi-Civita symbol, antisymmetric symbol,
     or alternating symbol.
     """
@@ -495,8 +510,9 @@
         return ComplexValue(expression)
     elif isinstance(expression, float):
         return FloatValue(expression)
     elif isinstance(expression, int):
         return IntValue(expression)
     else:
         raise ValueError(
-            f"Invalid type conversion: {expression} can not be converted to any UFL type.")
+            f"Invalid type conversion: {expression} can not be converted to any UFL type."
+        )
```

### Comparing `fenics-ufl-2023.2.0/ufl/core/base_form_operator.py` & `fenics_ufl-2024.1.0.post0/ufl/core/base_form_operator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Base form operator.
 
-This module defines the BaseFormOperator class, which is the base class for objects that can be seen as forms
-and as operators such as ExternalOperator or Interpolate.
+This module defines the BaseFormOperator class, which is the base class
+for objects that can be seen as forms and as operators such as
+ExternalOperator or Interpolate.
 """
 
 # Copyright (C) 2019 Nacime Bouziani
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Nacime Bouziani, 2021-2022
 
 from collections import OrderedDict
 
 from ufl.argument import Argument, Coargument
+from ufl.constantvalue import as_ufl
 from ufl.core.operator import Operator
-from ufl.form import BaseForm
 from ufl.core.ufl_type import ufl_type
-from ufl.constantvalue import as_ufl
+from ufl.form import BaseForm
 from ufl.functionspace import AbstractFunctionSpace
 from ufl.utils.counted import Counted
 
 
 @ufl_type(num_ops="varying", is_differential=True)
 class BaseFormOperator(Operator, BaseForm, Counted):
     """Base form operator."""
@@ -32,17 +33,19 @@
     _ufl_noslots_ = True
 
     def __init__(self, *operands, function_space, derivatives=None, argument_slots=()):
         """Initialise.
 
         Args:
             operands: operands on which acts the operator.
-            function_space: the FunctionSpace or MixedFunctionSpace on which to build this Function.
-            derivatives: tuple specifiying the derivative multiindex.
-            argument_slots: tuple composed containing expressions with ufl.Argument or ufl.Coefficient objects.
+            function_space: the FunctionSpace or MixedFunctionSpace on
+                which to build this Function.
+            derivatives: tuple specifying the derivative multiindex.
+            argument_slots: tuple composed containing expressions with
+                ufl.Argument or ufl.Coefficient objects.
         """
         BaseForm.__init__(self)
         ufl_operands = tuple(map(as_ufl, operands))
         argument_slots = tuple(map(as_ufl, argument_slots))
         Operator.__init__(self, ufl_operands)
         Counted.__init__(self, counted_class=BaseFormOperator)
 
@@ -69,20 +72,22 @@
     # BaseFormOperators don't have free indices.
     ufl_free_indices = ()
     ufl_index_dimensions = ()
 
     def argument_slots(self, outer_form=False):
         """Returns a tuple of expressions containing argument and coefficient based expressions.
 
-        We get an argument uhat when we take the Gateaux derivative in the direction uhat:
-        d/du N(u; v*) = dNdu(u; uhat, v*) where uhat is a ufl.Argument and v* a ufl.Coargument
-        Applying the action replace the last argument by coefficient:
-        action(dNdu(u; uhat, v*), w) = dNdu(u; w, v*) where du is a ufl.Coefficient.
+        We get an argument uhat when we take the Gateaux derivative in
+        the direction uhat: d/du N(u; v*) = dNdu(u; uhat, v*) where uhat
+        is a ufl.Argument and v* a ufl.Coargument Applying the action
+        replace the last argument by coefficient: action(dNdu(u; uhat,
+        v*), w) = dNdu(u; w, v*) where du is a ufl.Coefficient.
         """
         from ufl.algorithms.analysis import extract_arguments
+
         if not outer_form:
             return self._argument_slots
         # Takes into account argument contraction when a base form operator is in an outer form:
         # For example:
         #   F = N(u; v*) * v * dx can be seen as Action(v1 * v * dx, N(u; v*))
         #   => F.arguments() should return (v,)!
         return tuple(a for a in self._argument_slots[1:] if len(extract_arguments(a)) != 0)
@@ -92,22 +97,27 @@
         if self._coefficients is None:
             self._analyze_form_arguments()
         return self._coefficients
 
     def _analyze_form_arguments(self):
         """Analyze which Argument and Coefficient objects can be found in the base form."""
         from ufl.algorithms.analysis import extract_arguments, extract_coefficients, extract_type
+
         dual_arg, *arguments = self.argument_slots()
-        # When coarguments are treated as BaseForms, they have two arguments (one primal and one dual)
-        # as they map from V* to V* => V* x V -> R. However, when they are treated as mere "arguments",
-        # the primal space argument is discarded and we only have the dual space argument (Coargument).
-        # This is the exact same situation than BaseFormOperator's arguments which are different depending on
-        # whether the BaseFormOperator is used in an outer form or not.
-        arguments = (tuple(extract_type(dual_arg, Coargument))
-                     + tuple(a for arg in arguments for a in extract_arguments(arg)))
+        # When coarguments are treated as BaseForms, they have two
+        # arguments (one primal and one dual) as they map from V* to V*
+        # => V* x V -> R. However, when they are treated as mere
+        # "arguments", the primal space argument is discarded and we
+        # only have the dual space argument (Coargument). This is the
+        # exact same situation than BaseFormOperator's arguments which
+        # are different depending on whether the BaseFormOperator is
+        # used in an outer form or not.
+        arguments = tuple(extract_type(dual_arg, Coargument)) + tuple(
+            a for arg in arguments for a in extract_arguments(arg)
+        )
         coefficients = tuple(c for op in self.ufl_operands for c in extract_coefficients(op))
         # Define canonical numbering of arguments and coefficients
         # 1) Need concept of order since we may have arguments with the same number
         #    because of form composition (`argument_slots(outer_form=True)`):
         #    Example: Let u \in V1 and N \in V2 and F = N(u; v*) * dx, then
         #    `derivative(F, u)` will contain dNdu(u; uhat, v*) with v* = Argument(0, V2)
         #    and uhat = Argument(0, V1) (since F.arguments() = ())
@@ -128,34 +138,41 @@
     def ufl_function_space(self):
         """Return the function space associated to the operator.
 
         I.e. return the dual of the base form operator's Coargument.
         """
         return self.arguments()[0]._ufl_function_space.dual()
 
-    def _ufl_expr_reconstruct_(self, *operands, function_space=None, derivatives=None, argument_slots=None):
+    def _ufl_expr_reconstruct_(
+        self, *operands, function_space=None, derivatives=None, argument_slots=None
+    ):
         """Return a new object of the same type with new operands."""
-        return type(self)(*operands, function_space=function_space or self.ufl_function_space(),
-                          derivatives=derivatives or self.derivatives,
-                          argument_slots=argument_slots or self.argument_slots())
+        return type(self)(
+            *operands,
+            function_space=function_space or self.ufl_function_space(),
+            derivatives=derivatives or self.derivatives,
+            argument_slots=argument_slots or self.argument_slots(),
+        )
 
     def __repr__(self):
         """Default repr string construction for base form operators."""
         r = f"{type(self).__name__}("
         r += ", ".join(repr(op) for op in self.ufl_operands)
         r += "; {self.ufl_function_space()!r}; "
         r += ", ".join(repr(arg) for arg in self.argument_slots())
         r += f"; derivatives={self.derivatives!r})"
         return r
 
     def __hash__(self):
         """Hash code for use in dicts."""
-        hashdata = (type(self),
-                    tuple(hash(op) for op in self.ufl_operands),
-                    tuple(hash(arg) for arg in self._argument_slots),
-                    self.derivatives,
-                    hash(self.ufl_function_space()))
+        hashdata = (
+            type(self),
+            tuple(hash(op) for op in self.ufl_operands),
+            tuple(hash(arg) for arg in self._argument_slots),
+            self.derivatives,
+            hash(self.ufl_function_space()),
+        )
         return hash(hashdata)
 
     def __eq__(self, other):
         """Check for equality."""
         raise NotImplementedError()
```

### Comparing `fenics-ufl-2023.2.0/ufl/core/compute_expr_hash.py` & `fenics_ufl-2024.1.0.post0/ufl/core/compute_expr_hash.py`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/ufl/core/expr.py` & `fenics_ufl-2024.1.0.post0/ufl/core/expr.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 # Modified by Massimiliano Leoni, 2016
 
 import warnings
 
 from ufl.core.ufl_type import UFLType, update_ufl_type_attributes
 
 
-# --- The base object for all UFL expression tree nodes ---
-
 class Expr(object, metaclass=UFLType):
     """Base class for all UFL expression types.
 
     *Instance properties*
         Every ``Expr`` instance will have certain properties.
         The most important ones are ``ufl_operands``, ``ufl_shape``,
         ``ufl_free_indices``, and ``ufl_index_dimensions`` properties.
@@ -167,55 +165,43 @@
     # --- All subclasses must define these object attributes ---
 
     # Each subclass of Expr is checked to have these properties in
     # ufl_type
     _ufl_required_properties_ = (
         # A tuple of operands, all of them Expr instances.
         "ufl_operands",
-
         # A tuple of ints, the value shape of the expression.
         "ufl_shape",
-
         # A tuple of free index counts.
         "ufl_free_indices",
-
         # A tuple providing the int dimension for each free index.
         "ufl_index_dimensions",
     )
 
     # Each subclass of Expr is checked to have these methods in
     # ufl_type
     # FIXME: Add more and enable all
     _ufl_required_methods_ = (
         # To compute the hash on demand, this method is called.
         "_ufl_compute_hash_",
-
         # The data returned from this method is used to compute the
         # signature of a form
         "_ufl_signature_data_",
-
         # The == operator must be implemented to compare for identical
         # representation, used by set() and dict(). The __hash__
         # operator is added by ufl_type.
         "__eq__",
-
         # To reconstruct an object of the same type with operands or
         # properties changed.
         "_ufl_expr_reconstruct_",  # Implemented in Operator and Terminal so this should never fail
-
         "ufl_domains",
         # "ufl_cell",
         # "ufl_domain",
-
         # "__str__",
         # "__repr__",
-
-        # TODO: Add checks for methods/properties of terminals only?
-        # Required for terminals:
-        # "is_cellwise_constant", # TODO: Rename to ufl_is_cellwise_constant?
     )
 
     # --- Global variables for collecting all types ---
 
     # A global dict mapping language_operator_name to the type it
     # produces
     _ufl_language_operators_ = {}
@@ -261,24 +247,30 @@
         """Return a new object of the same type with new operands."""
         raise NotImplementedError(self.__class__._ufl_expr_reconstruct_)
 
     # --- Functions for geometric properties of expression ---
 
     def ufl_domains(self):
         """Return all domains this expression is defined on."""
-        warnings.warn("Expr.ufl_domains() is deprecated, please "
-                      "use extract_domains(expr) instead.", DeprecationWarning)
+        warnings.warn(
+            "Expr.ufl_domains() is deprecated, please use extract_domains(expr) instead.",
+            DeprecationWarning,
+        )
         from ufl.domain import extract_domains
+
         return extract_domains(self)
 
     def ufl_domain(self):
         """Return the single unique domain this expression is defined on, or throw an error."""
-        warnings.warn("Expr.ufl_domain() is deprecated, please "
-                      "use extract_unique_domain(expr) instead.", DeprecationWarning)
+        warnings.warn(
+            "Expr.ufl_domain() is deprecated, please use extract_unique_domain(expr) instead.",
+            DeprecationWarning,
+        )
         from ufl.domain import extract_unique_domain
+
         return extract_unique_domain(self)
 
     # --- Functions for float evaluation ---
 
     def evaluate(self, x, mapping, component, index_values):
         """Evaluate expression at given coordinate with given values for terminals."""
         raise ValueError(f"Symbolic evaluation of {self._ufl_class_.__name__} not available.")
```

### Comparing `fenics-ufl-2023.2.0/ufl/core/external_operator.py` & `fenics_ufl-2024.1.0.post0/ufl/core/external_operator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """External operator.
 
-This module defines the ``ExternalOperator`` class, which symbolically represents operators that are not
-straightforwardly expressible in UFL. Subclasses of ``ExternalOperator`` must define
-how this operator should be evaluated as well as its derivatives from a given set of operands.
+This module defines the ``ExternalOperator`` class, which symbolically
+represents operators that are not straightforwardly expressible in UFL.
+Subclasses of ``ExternalOperator`` must define how this operator should
+be evaluated as well as its derivatives from a given set of operands.
 """
 # Copyright (C) 2019 Nacime Bouziani
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
@@ -25,75 +26,95 @@
     _ufl_noslots_ = True
 
     def __init__(self, *operands, function_space, derivatives=None, argument_slots=()):
         """Initialise.
 
         Args:
             operands: operands on which acts the ExternalOperator.
-            function_space: the FunctionSpace, or MixedFunctionSpace on which to build this Function.
-            derivatives: tuple specifiying the derivative multiindex.
-            argument_slots: tuple composed containing expressions with ufl.Argument or ufl.Coefficient objects.
+            function_space: the FunctionSpace, or MixedFunctionSpace on
+                which to build this Function.
+            derivatives: tuple specifying the derivative multiindex.
+                argument_slots: tuple composed containing expressions with
+                ufl.Argument or ufl.Coefficient objects.
+            argument_slots: TODO
         """
         # -- Derivatives -- #
         if derivatives is not None:
             if not isinstance(derivatives, tuple):
-                raise TypeError(f"Expecting a tuple for derivatives and not {derivatives}")
+                raise TypeError(f"Expecting a tuple for derivatives and not {derivatives}.")
             if not len(derivatives) == len(operands):
-                raise ValueError(f"Expecting a size of {len(operands)} for {derivatives}")
+                raise ValueError(f"Expecting a size of {len(operands)} for {derivatives}.")
             if not all(isinstance(d, int) for d in derivatives) or any(d < 0 for d in derivatives):
                 raise ValueError(
-                    f"Expecting a derivative multi-index with nonnegative indices and not {str(derivatives)}")
+                    "Expecting a derivative multi-index with nonnegative indices, "
+                    f"not {derivatives}."
+                )
         else:
             derivatives = (0,) * len(operands)
 
-        BaseFormOperator.__init__(self, *operands,
-                                  function_space=function_space,
-                                  derivatives=derivatives,
-                                  argument_slots=argument_slots)
+        BaseFormOperator.__init__(
+            self,
+            *operands,
+            function_space=function_space,
+            derivatives=derivatives,
+            argument_slots=argument_slots,
+        )
 
     def ufl_element(self):
         """Shortcut to get the finite element of the function space of the external operator."""
         # Useful when applying split on an ExternalOperator
         return self.arguments()[0].ufl_element()
 
     def grad(self):
         """Returns the symbolic grad of the external operator."""
-        # By default, differential rules produce `grad(assembled_o)` `where assembled_o`
-        # is the `Coefficient` resulting from assembling the external operator since
-        # the external operator may not be smooth enough for chain rule to hold.
-        # Symbolic gradient (`grad(ExternalOperator)`) depends on the operator considered
-        # and its implementation may be needed in some cases (e.g. convolution operator).
-        raise NotImplementedError('Symbolic gradient not defined for the external operator considered!')
+        # By default, differential rules produce `grad(assembled_o)`
+        # `where assembled_o` is the `Coefficient` resulting from
+        # assembling the external operator since the external operator
+        # may not be smooth enough for chain rule to hold. Symbolic
+        # gradient (`grad(ExternalOperator)`) depends on the operator
+        # considered and its implementation may be needed in some cases
+        # (e.g. convolution operator).
+        raise NotImplementedError(
+            "Symbolic gradient not defined for the external operator considered."
+        )
 
     def assemble(self, *args, **kwargs):
         """Assemble the external operator."""
-        raise NotImplementedError(f"Symbolic evaluation of {self._ufl_class_.__name__} not available.")
-
-    def _ufl_expr_reconstruct_(self, *operands, function_space=None, derivatives=None,
-                               argument_slots=None, add_kwargs={}):
+        raise NotImplementedError(
+            f"Symbolic evaluation of {self._ufl_class_.__name__} not available."
+        )
+
+    def _ufl_expr_reconstruct_(
+        self, *operands, function_space=None, derivatives=None, argument_slots=None, add_kwargs={}
+    ):
         """Return a new object of the same type with new operands."""
-        return type(self)(*operands, function_space=function_space or self.ufl_function_space(),
-                          derivatives=derivatives or self.derivatives,
-                          argument_slots=argument_slots or self.argument_slots(),
-                          **add_kwargs)
+        return type(self)(
+            *operands,
+            function_space=function_space or self.ufl_function_space(),
+            derivatives=derivatives or self.derivatives,
+            argument_slots=argument_slots or self.argument_slots(),
+            **add_kwargs,
+        )
 
     def __str__(self):
         """Default str string for ExternalOperator operators."""
-        d = '\N{PARTIAL DIFFERENTIAL}'
+        d = "\N{PARTIAL DIFFERENTIAL}"
         derivatives = self.derivatives
         d_ops = "".join(d + "o" + str(i + 1) for i, di in enumerate(derivatives) for j in range(di))
         e = "e("
         e += ", ".join(str(op) for op in self.ufl_operands)
         e += "; "
         e += ", ".join(str(arg) for arg in reversed(self.argument_slots()))
         e += ")"
         return d + e + "/" + d_ops if sum(derivatives) > 0 else e
 
     def __eq__(self, other):
         """Check for equality."""
         if self is other:
             return True
-        return (type(self) is type(other) and
-                all(a == b for a, b in zip(self.ufl_operands, other.ufl_operands)) and
-                all(a == b for a, b in zip(self._argument_slots, other._argument_slots)) and
-                self.derivatives == other.derivatives and
-                self.ufl_function_space() == other.ufl_function_space())
+        return (
+            type(self) is type(other)
+            and all(a == b for a, b in zip(self.ufl_operands, other.ufl_operands))
+            and all(a == b for a, b in zip(self._argument_slots, other._argument_slots))
+            and self.derivatives == other.derivatives
+            and self.ufl_function_space() == other.ufl_function_space()
+        )
```

### Comparing `fenics-ufl-2023.2.0/ufl/core/interpolate.py` & `fenics_ufl-2024.1.0.post0/ufl/core/interpolate.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Nacime Bouziani, 2021-2022
 
-from ufl.core.ufl_type import ufl_type
-from ufl.constantvalue import as_ufl
-from ufl.functionspace import AbstractFunctionSpace
-from ufl.argument import Coargument, Argument
+from ufl.argument import Argument, Coargument
 from ufl.coefficient import Cofunction
-from ufl.form import Form
+from ufl.constantvalue import as_ufl
 from ufl.core.base_form_operator import BaseFormOperator
+from ufl.core.ufl_type import ufl_type
 from ufl.duals import is_dual
+from ufl.form import Form
+from ufl.functionspace import AbstractFunctionSpace
 
 
 @ufl_type(num_ops="varying", is_differential=True)
 class Interpolate(BaseFormOperator):
     """Symbolic representation of the interpolation operator."""
 
     # Slots are disabled here because they cause trouble in PyDOLFIN
@@ -35,32 +35,35 @@
                 defined on the dual of the FunctionSpace to interpolate into.
         """
         # This check could be more rigorous.
         dual_args = (Coargument, Cofunction, Form)
 
         if isinstance(v, AbstractFunctionSpace):
             if is_dual(v):
-                raise ValueError('Expecting a primal function space.')
+                raise ValueError("Expecting a primal function space.")
             v = Argument(v.dual(), 0)
         elif not isinstance(v, dual_args):
-            raise ValueError("Expecting the second argument to be FunctionSpace, FiniteElement or dual.")
+            raise ValueError(
+                "Expecting the second argument to be FunctionSpace, FiniteElement or dual."
+            )
 
         expr = as_ufl(expr)
         if isinstance(expr, dual_args):
             raise ValueError("Expecting the first argument to be primal.")
 
         # Reversed order convention
         argument_slots = (v, expr)
         # Get the primal space (V** = V)
         vv = v if not isinstance(v, Form) else v.arguments()[0]
         function_space = vv.ufl_function_space().dual()
         # Set the operand as `expr` for DAG traversal purpose.
         operand = expr
-        BaseFormOperator.__init__(self, operand, function_space=function_space,
-                                  argument_slots=argument_slots)
+        BaseFormOperator.__init__(
+            self, operand, function_space=function_space, argument_slots=argument_slots
+        )
 
     def _ufl_expr_reconstruct_(self, expr, v=None, **add_kwargs):
         """Return a new object of the same type with new operands."""
         v = v or self.argument_slots()[0]
         return type(self)(expr, v, **add_kwargs)
 
     def __repr__(self):
@@ -77,17 +80,19 @@
         s += f"; {self.ufl_function_space()})"
         return s
 
     def __eq__(self, other):
         """Check for equality."""
         if self is other:
             return True
-        return (type(self) is type(other) and
-                all(a == b for a, b in zip(self._argument_slots, other._argument_slots)) and
-                self.ufl_function_space() == other.ufl_function_space())
+        return (
+            type(self) is type(other)
+            and all(a == b for a, b in zip(self._argument_slots, other._argument_slots))
+            and self.ufl_function_space() == other.ufl_function_space()
+        )
 
 
 # Helper function
 def interpolate(expr, v):
     """Create symbolic representation of the interpolation operator.
 
     Args:
```

### Comparing `fenics-ufl-2023.2.0/ufl/core/multiindex.py` & `fenics_ufl-2024.1.0.post0/ufl/core/multiindex.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,33 +4,34 @@
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Massimiliano Leoni, 2016.
 
-
-from ufl.utils.counted import Counted
-from ufl.core.ufl_type import ufl_type
 from ufl.core.terminal import Terminal
+from ufl.core.ufl_type import ufl_type
+from ufl.utils.counted import Counted
 
 # Export list for ufl.classes
 __all_classes__ = ["IndexBase", "FixedIndex", "Index"]
 
 
 class IndexBase(object):
     """Base class for all indices."""
+
     __slots__ = ()
 
     def __init__(self):
         """Initialise."""
 
 
 class FixedIndex(IndexBase):
     """UFL value: An index with a specific value assigned."""
+
     __slots__ = ("_value", "_hash")
 
     _cache = {}
 
     def __getnewargs__(self):
         """Get new args."""
         return (self._value,)
@@ -108,14 +109,15 @@
         """Return representation."""
         return f"Index({self._count})"
 
 
 @ufl_type()
 class MultiIndex(Terminal):
     """Represents a sequence of indices, either fixed or free."""
+
     __slots__ = ("_indices",)
 
     _cache = {}
 
     def __getnewargs__(self):
         """Get new args."""
         return (self._indices,)
@@ -160,16 +162,15 @@
 
     def _ufl_compute_hash_(self):
         """Compute UFL hash."""
         return hash(("MultiIndex",) + tuple(hash(ind) for ind in self._indices))
 
     def __eq__(self, other):
         """Check equality."""
-        return isinstance(other, MultiIndex) and \
-            self._indices == other._indices
+        return isinstance(other, MultiIndex) and self._indices == other._indices
 
     def evaluate(self, x, mapping, component, index_values):
         """Evaluate index."""
         # Build component from index values
         component = []
         for i in self._indices:
             if isinstance(i, FixedIndex):
```

### Comparing `fenics-ufl-2023.2.0/ufl/core/operator.py` & `fenics_ufl-2024.1.0.post0/ufl/core/operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Modified by Anders Logg, 2008
 # Modified by Massimiliano Leoni, 2016
 
 from ufl.core.expr import Expr
 from ufl.core.ufl_type import ufl_type
 
 
-# --- Base class for operator objects ---
-
 @ufl_type(is_abstract=True, is_terminal=False)
 class Operator(Expr):
     """Base class for all operators, i.e. non-terminal expression types."""
 
     __slots__ = ("ufl_operands",)
 
     def __init__(self, operands=None):
```

### Comparing `fenics-ufl-2023.2.0/ufl/core/terminal.py` & `fenics_ufl-2024.1.0.post0/ufl/core/terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,18 +50,20 @@
                     f = complex(self)
                 if derivatives:
                     f = 0.0
                 return f
             except Exception:
                 pass
             # If it has an ufl_evaluate function, call it
-            if hasattr(self, 'ufl_evaluate'):
+            if hasattr(self, "ufl_evaluate"):
                 return self.ufl_evaluate(x, component, derivatives)
             # Take component if any
-            warnings.warn(f"Couldn't map '{self}' to a float, returning ufl object without evaluation.")
+            warnings.warn(
+                f"Couldn't map '{self}' to a float, returning ufl object without evaluation."
+            )
             f = self
             if component:
                 f = f[component]
             return f
 
         # Found a callable in the mapping
         if callable(f):
@@ -89,15 +91,17 @@
     def __eq__(self, other):
         """Default comparison of terminals just compare repr strings."""
         return repr(self) == repr(other)
 
 
 # --- Subgroups of terminals ---
 
+
 @ufl_type(is_abstract=True)
 class FormArgument(Terminal):
     """An abstract class for a form argument (a thing in a primal finite element space)."""
+
     __slots__ = ()
 
     def __init__(self):
         """Initialise the form argument."""
         Terminal.__init__(self)
```

### Comparing `fenics-ufl-2023.2.0/ufl/core/ufl_id.py` & `fenics_ufl-2024.1.0.post0/ufl/core/ufl_id.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,16 +47,15 @@
         # Bind cls with closure here
 
         def init_ufl_id(self, ufl_id):
             if ufl_id is None:
                 ufl_id = cls._ufl_global_id
             cls._ufl_global_id = max(ufl_id, cls._ufl_global_id) + 1
             return ufl_id
+
         return init_ufl_id
 
     # Modify class:
-    if hasattr(cls, "__slots__"):
-        assert "_ufl_id" in cls.__slots__
     cls._ufl_global_id = 0
     cls.ufl_id = _get_ufl_id
     cls._init_ufl_id = _init_ufl_id(cls)
     return cls
```

### Comparing `fenics-ufl-2023.2.0/ufl/core/ufl_type.py` & `fenics_ufl-2024.1.0.post0/ufl/core/ufl_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Massimiliano Leoni, 2016
 # Modified by Matthew Scroggs, 2023
 
 from __future__ import annotations
+
 import typing
-import warnings
+from abc import ABC, abstractmethod
 
+import ufl.core as core
 from ufl.core.compute_expr_hash import compute_expr_hash
 from ufl.utils.formatting import camel2underscore
-from abc import ABC, abstractmethod
-# Avoid circular import
-import ufl.core as core
 
 
 class UFLObject(ABC):
     """A UFL Object."""
 
     @abstractmethod
     def _ufl_hash_data_(self) -> typing.Hashable:
@@ -43,55 +42,29 @@
         return type(self) is type(other) and self._ufl_hash_data_() == other._ufl_hash_data_()
 
     def __ne__(self, other):
         """Check inequality."""
         return not self.__eq__(other)
 
 
-def attach_operators_from_hash_data(cls):
-    """Class decorator to attach ``__hash__``, ``__eq__`` and ``__ne__`` implementations.
-
-    These are implemented in terms of a ``._ufl_hash_data()`` method on the class,
-    which should return a tuple or hashable and comparable data.
-    """
-    warnings.warn("attach_operators_from_hash_data deprecated, please use UFLObject instead.", DeprecationWarning)
-    assert hasattr(cls, "_ufl_hash_data_")
-
-    def __hash__(self):
-        """__hash__ implementation attached in attach_operators_from_hash_data."""
-        return hash(self._ufl_hash_data_())
-    cls.__hash__ = __hash__
-
-    def __eq__(self, other):
-        """__eq__ implementation attached in attach_operators_from_hash_data."""
-        return type(self) is type(other) and self._ufl_hash_data_() == other._ufl_hash_data_()
-    cls.__eq__ = __eq__
-
-    def __ne__(self, other):
-        """__ne__ implementation attached in attach_operators_from_hash_data."""
-        return not self.__eq__(other)
-    cls.__ne__ = __ne__
-
-    return cls
-
-
 def get_base_attr(cls, name):
     """Return first non-``None`` attribute of given name among base classes."""
     for base in cls.mro():
         if hasattr(base, name):
             attr = getattr(base, name)
             if attr is not None:
                 return attr
     return None
 
 
 def set_trait(cls, basename, value, inherit=False):
     """Assign a trait to class with namespacing ``_ufl_basename_`` applied.
 
-    If trait value is ``None``, optionally inherit it from the closest base class that has it.
+    If trait value is ``None``, optionally inherit it from the closest
+    base class that has it.
     """
     name = "_ufl_" + basename + "_"
     if value is None and inherit:
         value = get_base_attr(cls, name)
     setattr(cls, name, value)
 
 
@@ -112,51 +85,58 @@
         # Determine from base class
         return get_base_attr(cls, "_ufl_num_ops_")
 
 
 def check_is_terminal_consistency(cls):
     """Check for consistency in ``is_terminal`` trait among superclasses."""
     if cls._ufl_is_terminal_ is None:
-        msg = (f"Class {cls.__name__} has not specified the is_terminal trait."
-               " Did you forget to inherit from Terminal or Operator?")
+        msg = (
+            f"Class {cls.__name__} has not specified the is_terminal trait."
+            " Did you forget to inherit from Terminal or Operator?"
+        )
         raise TypeError(msg)
 
     base_is_terminal = get_base_attr(cls, "_ufl_is_terminal_")
     if base_is_terminal is not None and cls._ufl_is_terminal_ != base_is_terminal:
-        msg = (f"Conflicting given and automatic 'is_terminal' trait for class {cls.__name__}."
-               " Check if you meant to inherit from Terminal or Operator.")
+        msg = (
+            f"Conflicting given and automatic 'is_terminal' trait for class {cls.__name__}."
+            " Check if you meant to inherit from Terminal or Operator."
+        )
         raise TypeError(msg)
 
 
 def check_abstract_trait_consistency(cls):
     """Check that the first base classes up to ``Expr`` are other UFL types."""
     for base in cls.mro():
         if base is core.expr.Expr:
             break
         if not issubclass(base, core.expr.Expr) and base._ufl_is_abstract_:
-            msg = ("Base class {0.__name__} of class {1.__name__} "
-                   "is not an abstract subclass of {2.__name__}.")
+            msg = (
+                "Base class {0.__name__} of class {1.__name__} "
+                "is not an abstract subclass of {2.__name__}."
+            )
             raise TypeError(msg.format(base, cls, core.expr.Expr))
 
 
 def check_has_slots(cls):
     """Check if type has __slots__ unless it is marked as exception with _ufl_noslots_."""
     if "_ufl_noslots_" in cls.__dict__:
         return
 
     if "__slots__" not in cls.__dict__:
-        msg = ("Class {0.__name__} is missing the __slots__ "
-               "attribute and is not marked with _ufl_noslots_.")
+        msg = (
+            "Class {0.__name__} is missing the __slots__ "
+            "attribute and is not marked with _ufl_noslots_."
+        )
         raise TypeError(msg.format(cls))
 
     # Check base classes for __slots__ as well, skipping object which is the last one
     for base in cls.mro()[1:-1]:
         if "__slots__" not in base.__dict__:
-            msg = ("Class {0.__name__} is has a base class "
-                   "{1.__name__} with __slots__ missing.")
+            msg = "Class {0.__name__} is has a base class {1.__name__} with __slots__ missing."
             raise TypeError(msg.format(cls, base))
 
 
 def check_type_traits_consistency(cls):
     """Execute a variety of consistency checks on the ufl type traits."""
     # Check for consistency in global type collection sizes
     Expr = core.expr.Expr
@@ -226,30 +206,38 @@
         cls.ufl_free_indices = ()
         cls.ufl_index_dimensions = ()
 
     # Automate direct inheriting of shape and indices from one of the
     # operands.  This simplifies refactoring because a lot of types do
     # this.
     if inherit_shape_from_operand is not None:
+
         def _inherited_ufl_shape(self):
             return self.ufl_operands[inherit_shape_from_operand].ufl_shape
+
         cls.ufl_shape = property(_inherited_ufl_shape)
 
     if inherit_indices_from_operand is not None:
+
         def _inherited_ufl_free_indices(self):
             return self.ufl_operands[inherit_indices_from_operand].ufl_free_indices
 
         def _inherited_ufl_index_dimensions(self):
             return self.ufl_operands[inherit_indices_from_operand].ufl_index_dimensions
+
         cls.ufl_free_indices = property(_inherited_ufl_free_indices)
         cls.ufl_index_dimensions = property(_inherited_ufl_index_dimensions)
 
 
 def update_global_expr_attributes(cls):
-    """Update global ``Expr`` attributes, mainly by adding *cls* to global collections of ufl types."""
+    """Update global attributres.
+
+    Update global ``Expr`` attributes, mainly by adding *cls* to global
+    collections of ufl types.
+    """
     if cls._ufl_is_terminal_modifier_:
         core.expr.Expr._ufl_terminal_modifiers_.append(cls)
 
     # Add to collection of language operators.  This collection is
     # used later to populate the official language namespace.
     # TODO: I don't think this functionality is fully completed, check
     # it out later.
@@ -273,28 +261,42 @@
     # Append space for counting object creation and destriction of
     # this this type.
     UFLType._ufl_obj_init_counts_.append(0)
     UFLType._ufl_obj_del_counts_.append(0)
 
 
 def ufl_type(
-    is_abstract=False, is_terminal=None,  is_scalar=False, is_index_free=False, is_shaping=False,
-    is_literal=False, is_terminal_modifier=False, is_in_reference_frame=False, is_restriction=False,
-    is_evaluation=False, is_differential=None, use_default_hash=True, num_ops=None,
-    inherit_shape_from_operand=None, inherit_indices_from_operand=None, wraps_type=None, unop=None,
-    binop=None, rbinop=None
+    is_abstract=False,
+    is_terminal=None,
+    is_scalar=False,
+    is_index_free=False,
+    is_shaping=False,
+    is_literal=False,
+    is_terminal_modifier=False,
+    is_in_reference_frame=False,
+    is_restriction=False,
+    is_evaluation=False,
+    is_differential=None,
+    use_default_hash=True,
+    num_ops=None,
+    inherit_shape_from_operand=None,
+    inherit_indices_from_operand=None,
+    wraps_type=None,
+    unop=None,
+    binop=None,
+    rbinop=None,
 ):
-    """This decorator is to be applied to every subclass in the UFL ``Expr`` and ``BaseForm`` hierarchy.
+    """Decorator to apply to every subclass in the UFL ``Expr`` and ``BaseForm`` hierarchy.
 
-    This decorator contains a number of checks that are
-    intended to enforce uniform behaviour across UFL types.
+    This decorator contains a number of checks that are intended to
+    enforce uniform behaviour across UFL types.
 
-    The rationale behind the checks and the meaning of the
-    optional arguments should be sufficiently documented
-    in the source code below.
+    The rationale behind the checks and the meaning of the optional
+    arguments should be sufficiently documented in the source code
+    below.
     """
 
     def _ufl_type_decorator_(cls):
         """UFL type decorator."""
         # Update attributes for UFLType instances (BaseForm and Expr objects)
         update_ufl_type_attributes(cls)
         if not issubclass(cls, core.expr.Expr):
@@ -309,19 +311,17 @@
 
         # Store type traits
         cls._ufl_class_ = cls
         set_trait(cls, "is_abstract", is_abstract, inherit=False)
 
         set_trait(cls, "is_terminal", is_terminal, inherit=True)
         set_trait(cls, "is_literal", is_literal, inherit=True)
-        set_trait(cls, "is_terminal_modifier", is_terminal_modifier,
-                  inherit=True)
+        set_trait(cls, "is_terminal_modifier", is_terminal_modifier, inherit=True)
         set_trait(cls, "is_shaping", is_shaping, inherit=True)
-        set_trait(cls, "is_in_reference_frame", is_in_reference_frame,
-                  inherit=True)
+        set_trait(cls, "is_in_reference_frame", is_in_reference_frame, inherit=True)
         set_trait(cls, "is_restriction", is_restriction, inherit=True)
         set_trait(cls, "is_evaluation", is_evaluation, inherit=True)
         set_trait(cls, "is_differential", is_differential, inherit=True)
 
         set_trait(cls, "is_scalar", is_scalar, inherit=True)
         set_trait(cls, "is_index_free", _is_index_free, inherit=True)
 
@@ -329,15 +329,16 @@
         _num_ops = determine_num_ops(cls, num_ops, unop, binop, rbinop)
         set_trait(cls, "num_ops", _num_ops)
 
         # Attach builtin type wrappers to Expr
         """# These are currently handled in the as_ufl implementation in constantvalue.py
         if wraps_type is not None:
             if not isinstance(wraps_type, type):
-                msg = "Expecting a type, not a {0.__name__} for the wraps_type argument in definition of {1.__name__}."
+                msg = "Expecting a type, not a {0.__name__} for the
+                wraps_type argument in definition of {1.__name__}."
                 raise TypeError(msg.format(type(wraps_type), cls))
 
             def _ufl_from_type_(value):
                 return cls(value)
             from_type_name = "_ufl_from_{0}_".format(wraps_type.__name__)
             setattr(Expr, from_type_name, staticmethod(_ufl_from_type_))
         """
@@ -376,17 +377,17 @@
         if use_default_hash:
             cls.__hash__ = compute_expr_hash
 
         # NB! This function conditionally adds some methods to the
         # class!  This approach significantly reduces the amount of
         # small functions to implement across all the types but of
         # course it's a bit more opaque.
-        attach_implementations_of_indexing_interface(cls,
-                                                     inherit_shape_from_operand,
-                                                     inherit_indices_from_operand)
+        attach_implementations_of_indexing_interface(
+            cls, inherit_shape_from_operand, inherit_indices_from_operand
+        )
 
         # Update Expr
         update_global_expr_attributes(cls)
 
         # Apply a range of consistency checks to detect bugs in type
         # implementations that Python doesn't check for us, including
         # some checks that a static language compiler would do for us
```

### Comparing `fenics-ufl-2023.2.0/ufl/corealg/map_dag.py` & `fenics_ufl-2024.1.0.post0/ufl/corealg/map_dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,57 +4,58 @@
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Massimiliano Leoni, 2016
 
 from ufl.core.expr import Expr
-from ufl.corealg.traversal import unique_post_traversal, cutoff_unique_post_traversal
 from ufl.corealg.multifunction import MultiFunction
+from ufl.corealg.traversal import cutoff_unique_post_traversal, unique_post_traversal
 
 
-def map_expr_dag(function, expression,  compress=True, vcache=None, rcache=None):
+def map_expr_dag(function, expression, compress=True, vcache=None, rcache=None):
     """Apply a function to each subexpression node in an expression DAG.
 
-    If the same funtion is called multiple times in a transformation
+    If the same function is called multiple times in a transformation
     (as for example in apply_derivatives), then to reuse caches across
     the call, use the arguments vcache and rcache.
 
     Args:
         function: The function
         expression: An expression
         compress: If True (default), the output object from
             the function is cached in a dict and reused such that the
             resulting expression DAG does not contain duplicate objects
-        vcache: Optional dict for caching results of intermediate transformations
+        vcache: Optional dict for caching results of intermediate
+            transformations
         rcache: Optional dict for caching results for compression
 
     Returns:
         The result of the final function call
     """
-    result, = map_expr_dags(function, [expression], compress=compress,
-                            vcache=vcache,
-                            rcache=rcache)
+    (result,) = map_expr_dags(
+        function, [expression], compress=compress, vcache=vcache, rcache=rcache
+    )
     return result
 
 
 def map_expr_dags(function, expressions, compress=True, vcache=None, rcache=None):
-    """Apply a function to each subexpression node in an expression DAG.
+    """Apply a function to each sub-expression node in an expression DAG.
 
     If *compress* is ``True`` (default) the output object from
     the function is cached in a ``dict`` and reused such that the
     resulting expression DAG does not contain duplicate objects.
 
-    If the same funtion is called multiple times in a transformation
+    If the same function is called multiple times in a transformation
     (as for example in apply_derivatives), then to reuse caches across
     the call, use the arguments vcache and rcache.
 
     Args:
         function: The function
-        expression: An expression
+        expressions: An expression
         compress: If True (default), the output object from
             the function is cached in a dict and reused such that the
             resulting expression DAG does not contain duplicate objects
         vcache: Optional dict for caching results of intermediate transformations
         rcache: Optional dict for caching results for compression
 
     Returns:
@@ -76,17 +77,19 @@
         handlers = [function] * Expr._ufl_num_typecodes_
 
     # Create visited set here to share between traversal calls
     visited = set()
 
     # Pick faster traversal algorithm if we have no cutoffs
     if any(cutoff_types):
+
         def traversal(expression):
             return cutoff_unique_post_traversal(expression, cutoff_types, visited)
     else:
+
         def traversal(expression):
             return unique_post_traversal(expression, visited)
 
     for expression in expressions:
         # Iterate over all subexpression nodes, child before parent
         for v in traversal(expression):
             # Skip transformations on cache hit
```

### Comparing `fenics-ufl-2023.2.0/ufl/corealg/multifunction.py` & `fenics_ufl-2024.1.0.post0/ufl/corealg/multifunction.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     def _memoized_handler(self, o):
         c = getattr(self, "_memoized_handler_cache")
         r = c.get(o)
         if r is None:
             r = handler(self, o)
             c[o] = r
         return r
+
     return _memoized_handler
 
 
 class MultiFunction(object):
     """Base class for collections of non-recursive expression node handlers.
 
     Subclass this (remember to call the ``__init__`` method of this class),
@@ -72,16 +73,15 @@
                             raise attribute_error
                         # Default handler name for UFL types
                         handler_name = UFLType._ufl_handler_name_
 
                     if hasattr(self, handler_name):
                         handler_names[classobject._ufl_typecode_] = handler_name
                         break
-            is_cutoff_type = [get_num_args(getattr(self, name)) == 2
-                              for name in handler_names]
+            is_cutoff_type = [get_num_args(getattr(self, name)) == 2 for name in handler_names]
             cache_data = (handler_names, is_cutoff_type)
             MultiFunction._handlers_cache[algorithm_class] = cache_data
 
         # Build handler list for this particular class (get functions
         # bound to self, these cannot be cached)
         handler_names, is_cutoff_type = cache_data
         self._handlers = [getattr(self, name) for name in handler_names]
```

### Comparing `fenics-ufl-2023.2.0/ufl/corealg/traversal.py` & `fenics_ufl-2024.1.0.post0/ufl/corealg/traversal.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,19 @@
                 break
         else:
             yield expr
             lifo.pop()
 
 
 def cutoff_post_traversal(expr, cutofftypes):
-    """Yield ``o`` for each node ``o`` in *expr*, child before parent, but skipping subtrees of the cutofftypes."""
+    """Cut-off post-tranversal.
+
+    Yield ``o`` for each node ``o`` in *expr*, child before parent, but
+    skipping subtrees of the cutofftypes.
+    """
     lifo = [(expr, list(reversed(expr.ufl_operands)))]
     while lifo:
         expr, deps = lifo[-1]
         if cutofftypes[expr._ufl_typecode_]:
             yield expr
             lifo.pop()
         else:
```

### Comparing `fenics-ufl-2023.2.0/ufl/differentiation.py` & `fenics_ufl-2024.1.0.post0/ufl/differentiation.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,188 +2,197 @@
 
 # Copyright (C) 2008-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
+from ufl.argument import Argument, Coargument
 from ufl.checks import is_cellwise_constant
 from ufl.coefficient import Coefficient
-from ufl.argument import Argument, Coargument
 from ufl.constantvalue import Zero
+from ufl.core.base_form_operator import BaseFormOperator
 from ufl.core.expr import Expr
 from ufl.core.operator import Operator
-from ufl.core.base_form_operator import BaseFormOperator
 from ufl.core.terminal import Terminal
 from ufl.core.ufl_type import ufl_type
 from ufl.domain import extract_unique_domain, find_geometric_dimension
 from ufl.exprcontainers import ExprList, ExprMapping
 from ufl.form import BaseForm
 from ufl.precedence import parstr
 from ufl.variable import Variable
 
 # --- Basic differentiation objects ---
 
 
-@ufl_type(is_abstract=True,
-          is_differential=True)
+@ufl_type(is_abstract=True, is_differential=True)
 class Derivative(Operator):
     """Base class for all derivative types."""
 
     __slots__ = ()
 
     def __init__(self, operands):
         """Initalise."""
         Operator.__init__(self, operands)
 
 
-@ufl_type(num_ops=4, inherit_shape_from_operand=0,
-          inherit_indices_from_operand=0)
+@ufl_type(num_ops=4, inherit_shape_from_operand=0, inherit_indices_from_operand=0)
 class CoefficientDerivative(Derivative):
-    """Derivative of the integrand of a form w.r.t. the degrees of freedom in a discrete Coefficient."""
+    """Derivative of form integrand w.r.t. the degrees of freedom in a discrete Coefficient."""
 
     __slots__ = ()
 
-    def __new__(cls, integrand, coefficients, arguments,
-                coefficient_derivatives):
+    def __new__(cls, integrand, coefficients, arguments, coefficient_derivatives):
         """Create a new CoefficientDerivative."""
         if not isinstance(coefficients, ExprList):
             raise ValueError("Expecting ExprList instance with Coefficients.")
         if not isinstance(arguments, ExprList):
             raise ValueError("Expecting ExprList instance with Arguments.")
         if not isinstance(coefficient_derivatives, ExprMapping):
             raise ValueError("Expecting ExprMapping for coefficient derivatives.")
         if isinstance(integrand, Zero):
             return integrand
         return Derivative.__new__(cls)
 
-    def __init__(self, integrand, coefficients, arguments,
-                 coefficient_derivatives):
+    def __init__(self, integrand, coefficients, arguments, coefficient_derivatives):
         """Initalise."""
         if not isinstance(coefficient_derivatives, ExprMapping):
             coefficient_derivatives = ExprMapping(coefficient_derivatives)
-        Derivative.__init__(self, (integrand, coefficients, arguments,
-                                   coefficient_derivatives))
+        Derivative.__init__(self, (integrand, coefficients, arguments, coefficient_derivatives))
 
     def __str__(self):
         """Format as a string."""
-        return "d/dfj { %s }, with fh=%s, dfh/dfj = %s, and coefficient derivatives %s"\
-            % (self.ufl_operands[0], self.ufl_operands[1],
-               self.ufl_operands[2], self.ufl_operands[3])
+        return "d/dfj { %s }, with fh=%s, dfh/dfj = %s, and coefficient derivatives %s" % (
+            self.ufl_operands[0],
+            self.ufl_operands[1],
+            self.ufl_operands[2],
+            self.ufl_operands[3],
+        )
 
 
-@ufl_type(num_ops=4, inherit_shape_from_operand=0,
-          inherit_indices_from_operand=0)
+@ufl_type(num_ops=4, inherit_shape_from_operand=0, inherit_indices_from_operand=0)
 class CoordinateDerivative(CoefficientDerivative):
     """Derivative of the integrand of a form w.r.t. the SpatialCoordinates."""
 
     __slots__ = ()
 
     def __str__(self):
         """Format as a string."""
-        return "d/dfj { %s }, with fh=%s, dfh/dfj = %s, and coordinate derivatives %s"\
-            % (self.ufl_operands[0], self.ufl_operands[1],
-               self.ufl_operands[2], self.ufl_operands[3])
+        return "d/dfj { %s }, with fh=%s, dfh/dfj = %s, and coordinate derivatives %s" % (
+            self.ufl_operands[0],
+            self.ufl_operands[1],
+            self.ufl_operands[2],
+            self.ufl_operands[3],
+        )
 
 
-@ufl_type(num_ops=4, inherit_shape_from_operand=0,
-          inherit_indices_from_operand=0)
+@ufl_type(num_ops=4, inherit_shape_from_operand=0, inherit_indices_from_operand=0)
 class BaseFormDerivative(CoefficientDerivative, BaseForm):
     """Derivative of a base form w.r.t the degrees of freedom in a discrete Coefficient."""
 
     _ufl_noslots_ = True
 
-    def __init__(self, base_form, coefficients, arguments,
-                 coefficient_derivatives):
+    def __init__(self, base_form, coefficients, arguments, coefficient_derivatives):
         """Initalise."""
-        CoefficientDerivative.__init__(self, base_form, coefficients, arguments,
-                                       coefficient_derivatives)
+        CoefficientDerivative.__init__(
+            self, base_form, coefficients, arguments, coefficient_derivatives
+        )
         BaseForm.__init__(self)
 
     def _analyze_form_arguments(self):
         """Collect the arguments of the corresponding BaseForm."""
-        from ufl.algorithms.analysis import extract_type, extract_coefficients
+        from ufl.algorithms.analysis import extract_coefficients, extract_type
+
         base_form, _, arguments, _ = self.ufl_operands
 
         def arg_type(x):
             if isinstance(x, BaseForm):
                 return Coargument
             return Argument
+
         # Each derivative arguments can either be a:
         # - `ufl.BaseForm`: if it contains a `ufl.Coargument`
         # - or a `ufl.Expr`: if it contains a `ufl.Argument`
-        # When a `Coargument` is encountered, it is treated as an argument (i.e. as V* -> V* and not V* x V -> R)
-        # and should result in one single argument (in the dual space).
-        base_form_args = base_form.arguments() + tuple(arg for a in arguments.ufl_operands
-                                                       for arg in extract_type(a, arg_type(a)))
+        # When a `Coargument` is encountered, it is treated as an
+        # argument (i.e. as V* -> V* and not V* x V -> R) and should
+        # result in one single argument (in the dual space).
+        base_form_args = base_form.arguments() + tuple(
+            arg for a in arguments.ufl_operands for arg in extract_type(a, arg_type(a))
+        )
         # BaseFormDerivative's arguments don't necessarily contain BaseArgument objects only
         # -> e.g. `derivative(u ** 2, u, u)` with `u` a Coefficient.
-        base_form_coeffs = base_form.coefficients() + tuple(arg for a in arguments.ufl_operands
-                                                            for arg in extract_coefficients(a))
+        base_form_coeffs = base_form.coefficients() + tuple(
+            arg for a in arguments.ufl_operands for arg in extract_coefficients(a)
+        )
         # Reconstruct arguments for correct numbering
-        self._arguments = tuple(type(arg)(arg.ufl_function_space(), arg.number(), arg.part()) for arg in base_form_args)
+        self._arguments = tuple(
+            type(arg)(arg.ufl_function_space(), arg.number(), arg.part()) for arg in base_form_args
+        )
         self._coefficients = base_form_coeffs
 
 
-@ufl_type(num_ops=4, inherit_shape_from_operand=0,
-          inherit_indices_from_operand=0)
+@ufl_type(num_ops=4, inherit_shape_from_operand=0, inherit_indices_from_operand=0)
 class BaseFormCoordinateDerivative(BaseFormDerivative, CoordinateDerivative):
     """Derivative of a base form w.r.t. the SpatialCoordinates."""
 
     _ufl_noslots_ = True
 
-    def __init__(self, base_form, coefficients, arguments,
-                 coefficient_derivatives):
+    def __init__(self, base_form, coefficients, arguments, coefficient_derivatives):
         """Initalise."""
-        BaseFormDerivative.__init__(self, base_form, coefficients, arguments,
-                                    coefficient_derivatives)
+        BaseFormDerivative.__init__(
+            self, base_form, coefficients, arguments, coefficient_derivatives
+        )
 
 
-@ufl_type(num_ops=4, inherit_shape_from_operand=0,
-          inherit_indices_from_operand=0)
+@ufl_type(num_ops=4, inherit_shape_from_operand=0, inherit_indices_from_operand=0)
 class BaseFormOperatorDerivative(BaseFormDerivative, BaseFormOperator):
     """Derivative of a base form operator w.r.t the degrees of freedom in a discrete Coefficient."""
+
     _ufl_noslots_ = True
 
     # BaseFormOperatorDerivative is only needed because of a different
     # differentiation procedure for BaseformOperator objects.
-    def __init__(self, base_form, coefficients, arguments,
-                 coefficient_derivatives):
+    def __init__(self, base_form, coefficients, arguments, coefficient_derivatives):
         """Initalise."""
-        BaseFormDerivative.__init__(self, base_form, coefficients, arguments,
-                                    coefficient_derivatives)
+        BaseFormDerivative.__init__(
+            self, base_form, coefficients, arguments, coefficient_derivatives
+        )
         self._argument_slots = base_form._argument_slots
 
-    # Enforce Operator reconstruction as Operator is a parent class of both: BaseFormDerivative and BaseFormOperator.
-    # Therfore the latter overwrites Operator reconstruction and we would have:
-    #   -> BaseFormOperatorDerivative._ufl_expr_reconstruct_ = BaseFormOperator._ufl_expr_reconstruct_
+    # Enforce Operator reconstruction as Operator is a parent class of
+    # both: BaseFormDerivative and BaseFormOperator.
+    # Therefore the latter overwrites Operator reconstruction and we would have:
+    #   -> BaseFormOperatorDerivative._ufl_expr_reconstruct_ =
+    #   BaseFormOperator._ufl_expr_reconstruct_
     _ufl_expr_reconstruct_ = Operator._ufl_expr_reconstruct_
     # Set __repr__
     __repr__ = Operator.__repr__
 
     def argument_slots(self, outer_form=False):
         """Return a tuple of expressions containing argument and coefficient based expressions."""
         from ufl.algorithms.analysis import extract_arguments
+
         base_form, _, arguments, _ = self.ufl_operands
-        argument_slots = (base_form.argument_slots(outer_form)
-                          + tuple(arg for a in arguments for arg in extract_arguments(a)))
+        argument_slots = base_form.argument_slots(outer_form) + tuple(
+            arg for a in arguments for arg in extract_arguments(a)
+        )
         return argument_slots
 
 
-@ufl_type(num_ops=4, inherit_shape_from_operand=0,
-          inherit_indices_from_operand=0)
+@ufl_type(num_ops=4, inherit_shape_from_operand=0, inherit_indices_from_operand=0)
 class BaseFormOperatorCoordinateDerivative(BaseFormOperatorDerivative, CoordinateDerivative):
     """Derivative of a base form operator w.r.t. the SpatialCoordinates."""
+
     _ufl_noslots_ = True
 
-    def __init__(self, base_form, coefficients, arguments,
-                 coefficient_derivatives):
+    def __init__(self, base_form, coefficients, arguments, coefficient_derivatives):
         """Initalise."""
-        BaseFormOperatorDerivative.__init__(self, base_form, coefficients, arguments,
-                                            coefficient_derivatives)
+        BaseFormOperatorDerivative.__init__(
+            self, base_form, coefficients, arguments, coefficient_derivatives
+        )
 
 
 @ufl_type(num_ops=2)
 class VariableDerivative(Derivative):
     """Variable Derivative."""
 
     __slots__ = (
@@ -201,16 +210,15 @@
             raise ValueError("Expecting a Variable in VariableDerivative.")
         if v.ufl_free_indices:
             raise ValueError("Differentiation variable cannot have free indices.")
 
         # Simplification
         # Return zero if expression is trivially independent of variable
         if f._ufl_is_terminal_ and f != v:
-            return Zero(f.ufl_shape + v.ufl_shape, f.ufl_free_indices,
-                        f.ufl_index_dimensions)
+            return Zero(f.ufl_shape + v.ufl_shape, f.ufl_free_indices, f.ufl_index_dimensions)
 
         # Construction
         return Derivative.__new__(cls)
 
     def __init__(self, f, v):
         """Initalise."""
         Derivative.__init__(self, (f, v))
@@ -218,20 +226,20 @@
         self.ufl_index_dimensions = f.ufl_index_dimensions
         self.ufl_shape = f.ufl_shape + v.ufl_shape
 
     def __str__(self):
         """Format as a string."""
         if isinstance(self.ufl_operands[0], Terminal):
             return "d%s/d[%s]" % (self.ufl_operands[0], self.ufl_operands[1])
-        return "d/d[%s] %s" % (self.ufl_operands[1],
-                               parstr(self.ufl_operands[0], self))
+        return "d/d[%s] %s" % (self.ufl_operands[1], parstr(self.ufl_operands[0], self))
 
 
 # --- Compound differentiation objects ---
 
+
 @ufl_type(is_abstract=True)
 class CompoundDerivative(Derivative):
     """Base class for all compound derivative types."""
 
     __slots__ = ()
 
     def __init__(self, operands):
@@ -246,92 +254,89 @@
     __slots__ = ("_dim",)
 
     def __new__(cls, f):
         """Create a new Grad."""
         # Return zero if expression is trivially constant
         if is_cellwise_constant(f):
             dim = find_geometric_dimension(f)
-            return Zero(f.ufl_shape + (dim,), f.ufl_free_indices,
-                        f.ufl_index_dimensions)
+            return Zero(f.ufl_shape + (dim,), f.ufl_free_indices, f.ufl_index_dimensions)
         return CompoundDerivative.__new__(cls)
 
     def __init__(self, f):
         """Initalise."""
         CompoundDerivative.__init__(self, (f,))
         self._dim = find_geometric_dimension(f)
 
     def _ufl_expr_reconstruct_(self, op):
         """Return a new object of the same type with new operands."""
         if is_cellwise_constant(op):
             if op.ufl_shape != self.ufl_operands[0].ufl_shape:
                 raise ValueError("Operand shape mismatch in Grad reconstruct.")
             if self.ufl_operands[0].ufl_free_indices != op.ufl_free_indices:
                 raise ValueError("Free index mismatch in Grad reconstruct.")
-            return Zero(self.ufl_shape, self.ufl_free_indices,
-                        self.ufl_index_dimensions)
+            return Zero(self.ufl_shape, self.ufl_free_indices, self.ufl_index_dimensions)
         return self._ufl_class_(op)
 
     def evaluate(self, x, mapping, component, index_values, derivatives=()):
         """Get child from mapping and return the component asked for."""
         component, i = component[:-1], component[-1]
         derivatives = derivatives + (i,)
-        result = self.ufl_operands[0].evaluate(x, mapping, component,
-                                               index_values,
-                                               derivatives=derivatives)
+        result = self.ufl_operands[0].evaluate(
+            x, mapping, component, index_values, derivatives=derivatives
+        )
         return result
 
     @property
     def ufl_shape(self):
         """Get the UFL shape."""
         return self.ufl_operands[0].ufl_shape + (self._dim,)
 
     def __str__(self):
         """Format as a string."""
         return "grad(%s)" % self.ufl_operands[0]
 
 
-@ufl_type(num_ops=1, inherit_indices_from_operand=0, is_terminal_modifier=True,
-          is_in_reference_frame=True)
+@ufl_type(
+    num_ops=1, inherit_indices_from_operand=0, is_terminal_modifier=True, is_in_reference_frame=True
+)
 class ReferenceGrad(CompoundDerivative):
     """Reference grad."""
 
-    __slots__ = ("_dim", )
+    __slots__ = ("_dim",)
 
     def __new__(cls, f):
         """Create a new ReferenceGrad."""
         # Return zero if expression is trivially constant
         if is_cellwise_constant(f):
             dim = extract_unique_domain(f).topological_dimension()
-            return Zero(f.ufl_shape + (dim,), f.ufl_free_indices,
-                        f.ufl_index_dimensions)
+            return Zero(f.ufl_shape + (dim,), f.ufl_free_indices, f.ufl_index_dimensions)
         return CompoundDerivative.__new__(cls)
 
     def __init__(self, f):
         """Initalise."""
         CompoundDerivative.__init__(self, (f,))
         self._dim = extract_unique_domain(f).topological_dimension()
 
     def _ufl_expr_reconstruct_(self, op):
         """Return a new object of the same type with new operands."""
         if is_cellwise_constant(op):
             if op.ufl_shape != self.ufl_operands[0].ufl_shape:
                 raise ValueError("Operand shape mismatch in ReferenceGrad reconstruct.")
             if self.ufl_operands[0].ufl_free_indices != op.ufl_free_indices:
                 raise ValueError("Free index mismatch in ReferenceGrad reconstruct.")
-            return Zero(self.ufl_shape, self.ufl_free_indices,
-                        self.ufl_index_dimensions)
+            return Zero(self.ufl_shape, self.ufl_free_indices, self.ufl_index_dimensions)
         return self._ufl_class_(op)
 
     def evaluate(self, x, mapping, component, index_values, derivatives=()):
         """Get child from mapping and return the component asked for."""
         component, i = component[:-1], component[-1]
         derivatives = derivatives + (i,)
-        result = self.ufl_operands[0].evaluate(x, mapping, component,
-                                               index_values,
-                                               derivatives=derivatives)
+        result = self.ufl_operands[0].evaluate(
+            x, mapping, component, index_values, derivatives=derivatives
+        )
         return result
 
     @property
     def ufl_shape(self):
         """Get the UFL shape."""
         return self.ufl_operands[0].ufl_shape + (self._dim,)
 
@@ -367,16 +372,17 @@
         return self.ufl_operands[0].ufl_shape[:-1]
 
     def __str__(self):
         """Format as a string."""
         return "div(%s)" % self.ufl_operands[0]
 
 
-@ufl_type(num_ops=1, inherit_indices_from_operand=0, is_terminal_modifier=True,
-          is_in_reference_frame=True)
+@ufl_type(
+    num_ops=1, inherit_indices_from_operand=0, is_terminal_modifier=True, is_in_reference_frame=True
+)
 class ReferenceDiv(CompoundDerivative):
     """Reference divergence."""
 
     __slots__ = ()
 
     def __new__(cls, f):
         """Create a new ReferenceDiv."""
@@ -410,32 +416,30 @@
     __slots__ = ("_dim",)
 
     def __new__(cls, f):
         """Create a new NablaGrad."""
         # Return zero if expression is trivially constant
         if is_cellwise_constant(f):
             dim = find_geometric_dimension(f)
-            return Zero((dim,) + f.ufl_shape, f.ufl_free_indices,
-                        f.ufl_index_dimensions)
+            return Zero((dim,) + f.ufl_shape, f.ufl_free_indices, f.ufl_index_dimensions)
         return CompoundDerivative.__new__(cls)
 
     def __init__(self, f):
         """Initalise."""
         CompoundDerivative.__init__(self, (f,))
         self._dim = find_geometric_dimension(f)
 
     def _ufl_expr_reconstruct_(self, op):
         """Return a new object of the same type with new operands."""
         if is_cellwise_constant(op):
             if op.ufl_shape != self.ufl_operands[0].ufl_shape:
                 raise ValueError("Operand shape mismatch in NablaGrad reconstruct.")
             if self.ufl_operands[0].ufl_free_indices != op.ufl_free_indices:
                 raise ValueError("Free index mismatch in NablaGrad reconstruct.")
-            return Zero(self.ufl_shape, self.ufl_free_indices,
-                        self.ufl_index_dimensions)
+            return Zero(self.ufl_shape, self.ufl_free_indices, self.ufl_index_dimensions)
         return self._ufl_class_(op)
 
     @property
     def ufl_shape(self):
         """Get the UFL shape."""
         return (self._dim,) + self.ufl_operands[0].ufl_shape
 
@@ -505,16 +509,17 @@
         self.ufl_shape = _curl_shapes[f.ufl_shape]
 
     def __str__(self):
         """Format as a string."""
         return "curl(%s)" % self.ufl_operands[0]
 
 
-@ufl_type(num_ops=1, inherit_indices_from_operand=0,
-          is_terminal_modifier=True, is_in_reference_frame=True)
+@ufl_type(
+    num_ops=1, inherit_indices_from_operand=0, is_terminal_modifier=True, is_in_reference_frame=True
+)
 class ReferenceCurl(CompoundDerivative):
     """Reference curl."""
 
     __slots__ = ("ufl_shape",)
 
     def __new__(cls, f):
         """Create a new ReferenceCurl."""
```

### Comparing `fenics-ufl-2023.2.0/ufl/duals.py` & `fenics_ufl-2024.1.0.post0/ufl/duals.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 def is_primal(object):
     """Determine if the object belongs to a primal space.
 
     This is not simply the negation of is_dual,
     because a mixed function space containing both primal
     and dual components is neither primal nor dual.
     """
-    return hasattr(object, '_primal') and object._primal
+    return hasattr(object, "_primal") and object._primal
 
 
 def is_dual(object):
     """Determine if the object belongs to a dual space.
 
     This is not simply the negation of is_primal,
     because a mixed function space containing both primal
     and dual components is neither primal nor dual.
     """
-    return hasattr(object, '_dual') and object._dual
+    return hasattr(object, "_dual") and object._dual
```

### Comparing `fenics-ufl-2023.2.0/ufl/equation.py` & `fenics_ufl-2024.1.0.post0/ufl/equation.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         # Try to delegate to equals function
         if hasattr(self.lhs, "equals"):
             return self.lhs.equals(self.rhs)
         elif hasattr(self.rhs, "equals"):
             return self.rhs.equals(self.lhs)
         else:
             raise ValueError("Either lhs or rhs of Equation must implement self.equals(other).")
+
     __nonzero__ = __bool__
 
     def __eq__(self, other):
         """Compare two equations by comparing lhs and rhs."""
         return isinstance(other, Equation) and self.lhs == other.lhs and self.rhs == other.rhs
 
     def __hash__(self):
```

### Comparing `fenics-ufl-2023.2.0/ufl/exprcontainers.py` & `fenics_ufl-2024.1.0.post0/ufl/exprcontainers.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """This module defines special types for representing mapping of expressions to expressions."""
 # Copyright (C) 2014 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
+from ufl.argument import Coargument
+from ufl.coefficient import Cofunction
 from ufl.core.expr import Expr
 from ufl.core.operator import Operator
 from ufl.core.ufl_type import ufl_type
-from ufl.coefficient import Cofunction
-from ufl.argument import Coargument
-
 
 # --- Non-tensor types ---
 
+
 @ufl_type(num_ops="varying")
 class ExprList(Operator):
     """List of Expr objects. For internal use, never to be created by end users."""
 
     __slots__ = ()
 
     def __init__(self, *operands):
```

### Comparing `fenics-ufl-2023.2.0/ufl/exprequals.py` & `fenics_ufl-2024.1.0.post0/ufl/exprequals.py`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/ufl/exproperators.py` & `fenics_ufl-2024.1.0.post0/ufl/exproperators.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,33 +10,31 @@
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Massimiliano Leoni, 2016.
 
 import numbers
 
-from ufl.utils.stacks import StackDict
-from ufl.core.expr import Expr
+from ufl.algebra import Abs, Division, Power, Product, Sum
+from ufl.conditional import GE, GT, LE, LT
 from ufl.constantvalue import Zero, as_ufl
-from ufl.algebra import Sum, Product, Division, Power, Abs
-from ufl.tensoralgebra import Transposed, Inner
-from ufl.core.multiindex import MultiIndex, Index, indices
-from ufl.indexed import Indexed
-from ufl.indexsum import IndexSum
-from ufl.tensors import as_tensor, ComponentTensor
-from ufl.restriction import PositiveRestricted, NegativeRestricted
+from ufl.core.expr import Expr
+from ufl.core.multiindex import Index, MultiIndex, indices
 from ufl.differentiation import Grad
-from ufl.index_combination_utils import create_slice_indices, merge_overlapping_indices
-
 from ufl.exprequals import expr_equals
+from ufl.index_combination_utils import create_slice_indices, merge_overlapping_indices
+from ufl.indexed import Indexed
+from ufl.indexsum import IndexSum
+from ufl.restriction import NegativeRestricted, PositiveRestricted
+from ufl.tensoralgebra import Inner, Transposed
+from ufl.tensors import ComponentTensor, as_tensor
+from ufl.utils.stacks import StackDict
 
 # --- Boolean operators ---
 
-from ufl.conditional import LE, GE, LT, GT
-
 
 def _le(left, right):
     """A boolean expresion (left <= right) for use with conditional."""
     return LE(left, right)
 
 
 def _ge(left, right):
@@ -83,25 +81,30 @@
 # Expr.__and__ = _and
 # Expr.__or__ = _or
 
 
 def _as_tensor(self, indices):
     """A^indices := as_tensor(A, indices)."""
     if not isinstance(indices, tuple):
-        raise ValueError("Expecting a tuple of Index objects to A^indices := as_tensor(A, indices).")
+        raise ValueError(
+            "Expecting a tuple of Index objects to A^indices := as_tensor(A, indices)."
+        )
     if not all(isinstance(i, Index) for i in indices):
-        raise ValueError("Expecting a tuple of Index objects to A^indices := as_tensor(A, indices).")
+        raise ValueError(
+            "Expecting a tuple of Index objects to A^indices := as_tensor(A, indices)."
+        )
     return as_tensor(self, indices)
 
 
 Expr.__xor__ = _as_tensor
 
 
 # --- Helper functions for product handling ---
 
+
 def _mult(a, b):
     """Multiply."""
     # Discover repeated indices, which results in index sums
     afi = a.ufl_free_indices
     bfi = b.ufl_free_indices
     afid = a.ufl_index_dimensions
     bfid = b.ufl_index_dimensions
@@ -305,14 +308,15 @@
 
 
 Expr.__abs__ = _abs
 
 
 # --- Extend Expr with restiction operators a("+"), a("-") ---
 
+
 def _restrict(self, side):
     """Restrict."""
     if side == "+":
         return PositiveRestricted(self)
     if side == "-":
         return NegativeRestricted(self)
     raise ValueError(f"Invalid side '{side}' in restriction operator.")
@@ -322,14 +326,15 @@
     """Evaluate.
 
     Evaluate expression at this particular coordinate, with provided
     values for other terminals in mapping.
     """
     # Evaluate derivatives first
     from ufl.algorithms import expand_derivatives
+
     f = expand_derivatives(self)
 
     # Evaluate recursively
     if mapping is None:
         mapping = {}
     index_values = StackDict()
     return f.evaluate(coord, mapping, component, index_values)
@@ -346,42 +351,49 @@
 
 
 Expr.__call__ = _call
 
 
 # --- Extend Expr with the transpose operation A.T ---
 
+
 def _transpose(self):
     """Transpose a rank-2 tensor expression.
 
-    For more general transpose operations of higher order tensor expressions, use indexing and Tensor.
+    For more general transpose operations of higher order tensor
+    expressions, use indexing and Tensor.
     """
     return Transposed(self)
 
 
 Expr.T = property(_transpose)
 
 
 # --- Extend Expr with indexing operator a[i] ---
 
+
 def _getitem(self, component):
     """Get an item."""
     # Treat component consistently as tuple below
     if not isinstance(component, tuple):
         component = (component,)
 
     shape = self.ufl_shape
 
     # Analyse slices (:) and Ellipsis (...)
-    all_indices, slice_indices, repeated_indices = create_slice_indices(component, shape, self.ufl_free_indices)
+    all_indices, slice_indices, repeated_indices = create_slice_indices(
+        component, shape, self.ufl_free_indices
+    )
 
     # Check that we have the right number of indices for a tensor with
     # this shape
     if len(shape) != len(all_indices):
-        raise ValueError(f"Invalid number of indices {len(all_indices)} for expression of rank {len(shape)}.")
+        raise ValueError(
+            f"Invalid number of indices {len(all_indices)} for expression of rank {len(shape)}."
+        )
 
     # Special case for simplifying foo[...] => foo, foo[:] => foo or
     # similar
     if len(slice_indices) == len(all_indices):
         return self
 
     # Special case for simplifying as_tensor(ai,(i,))[i] => ai
@@ -420,14 +432,15 @@
 
 
 Expr.__getitem__ = _getitem
 
 
 # --- Extend Expr with spatial differentiation operator a.dx(i) ---
 
+
 def _dx(self, *ii):
     """Return the partial derivative with respect to spatial variable number *ii*."""
     d = self
     # Unwrap ii to allow .dx(i,j) and .dx((i,j))
     if len(ii) == 1 and isinstance(ii[0], tuple):
         ii = ii[0]
     # Apply all derivatives
```

### Comparing `fenics-ufl-2023.2.0/ufl/finiteelement/brokenelement.py` & `fenics_ufl-2024.1.0.post0/ufl/referencevalue.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,36 @@
-"""Element."""
-# -*- coding: utf-8 -*-
-# Copyright (C) 2014 Andrew T. T. McRae
+"""Representation of the reference value of a function."""
+# Copyright (C) 2008-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
-#
-# Modified by Massimiliano Leoni, 2016
-
-from ufl.finiteelement.finiteelementbase import FiniteElementBase
-from ufl.sobolevspace import L2
 
-
-class BrokenElement(FiniteElementBase):
-    """The discontinuous version of an existing Finite Element space."""
-    def __init__(self, element):
-        """Init."""
-        self._element = element
-
-        family = "BrokenElement"
-        cell = element.cell()
-        degree = element.degree()
-        quad_scheme = element.quadrature_scheme()
-        value_shape = element.value_shape()
-        reference_value_shape = element.reference_value_shape()
-        FiniteElementBase.__init__(self, family, cell, degree,
-                                   quad_scheme, value_shape, reference_value_shape)
-
-    def __repr__(self):
-        """Doc."""
-        return f"BrokenElement({repr(self._element)})"
-
-    def mapping(self):
-        """Doc."""
-        return self._element.mapping()
-
-    def sobolev_space(self):
-        """Return the underlying Sobolev space."""
-        return L2
-
-    def reconstruct(self, **kwargs):
-        """Doc."""
-        return BrokenElement(self._element.reconstruct(**kwargs))
+from ufl.core.operator import Operator
+from ufl.core.terminal import FormArgument
+from ufl.core.ufl_type import ufl_type
+
+
+@ufl_type(num_ops=1, is_index_free=True, is_terminal_modifier=True, is_in_reference_frame=True)
+class ReferenceValue(Operator):
+    """Representation of the reference cell value of a form argument."""
+
+    __slots__ = ()
+
+    def __init__(self, f):
+        """Initialise."""
+        if not isinstance(f, FormArgument):
+            raise ValueError("Can only take reference value of form arguments.")
+        Operator.__init__(self, (f,))
+
+    @property
+    def ufl_shape(self):
+        """Get the UFL shape."""
+        return self.ufl_operands[0].ufl_element().reference_value_shape
+
+    def evaluate(self, x, mapping, component, index_values, derivatives=()):
+        """Get child from mapping and return the component asked for."""
+        raise NotImplementedError()
 
     def __str__(self):
-        """Doc."""
-        return f"BrokenElement({repr(self._element)})"
-
-    def shortstr(self):
-        """Format as string for pretty printing."""
-        return f"BrokenElement({repr(self._element)})"
+        """Format as a string."""
+        return f"reference_value({self.ufl_operands[0]})"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fenics-ufl-2023.2.0/ufl/form.py` & `fenics_ufl-2024.1.0.post0/ufl/form.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,23 +30,28 @@
 # Export list for ufl.classes
 __all_classes__ = ["Form", "BaseForm", "ZeroBaseForm"]
 
 # --- The Form class, representing a complete variational form or functional ---
 
 
 def _sorted_integrals(integrals):
-    """Sort integrals by domain id, integral type, subdomain id for a more stable signature computation."""
+    """Sort integrals for a stable signature computation.
+
+    Sort integrals by domain id, integral type, subdomain id for a more
+    stable signature computation.
+    """
     # Group integrals in multilevel dict by keys
     # [domain][integral_type][subdomain_id]
-    integrals_dict = defaultdict(
-        lambda: defaultdict(lambda: defaultdict(list)))
+    integrals_dict = defaultdict(lambda: defaultdict(lambda: defaultdict(list)))
     for integral in integrals:
         d = integral.ufl_domain()
         if d is None:
-            raise ValueError("Each integral in a form must have a uniquely defined integration domain.")
+            raise ValueError(
+                "Each integral in a form must have a uniquely defined integration domain."
+            )
         it = integral.integral_type()
         si = integral.subdomain_id()
         integrals_dict[d][it][si] += [integral]
 
     all_integrals = []
 
     def keyfunc(item):
@@ -78,15 +83,15 @@
 class BaseForm(object, metaclass=UFLType):
     """Description of an object containing arguments."""
 
     # Slots is kept empty to enable multiple inheritance with other
     # classes
     __slots__ = ()
     _ufl_is_abstract_ = True
-    _ufl_required_methods_ = ('_analyze_form_arguments', '_analyze_domains', "ufl_domains")
+    _ufl_required_methods_ = ("_analyze_form_arguments", "_analyze_domains", "ufl_domains")
 
     def __init__(self):
         """Initialise."""
         # Internal variables for caching form argument/coefficient data
         self._arguments = None
         self._coefficients = None
 
@@ -133,15 +138,15 @@
         return self.__add__(other)
 
     def __add__(self, other):
         """Add."""
         if isinstance(other, (int, float)) and other == 0:
             # Allow adding 0 or 0.0 as a no-op, needed for sum([a,b])
             return self
-        elif isinstance(other, Zero) and not (other.ufl_shape or other.ufl_free_indices):
+        elif isinstance(other, Zero):
             # Allow adding ufl Zero as a no-op, needed for sum([a,b])
             return self
 
         elif isinstance(other, ZeroBaseForm):
             # Simplify addition with ZeroBaseForm
             return self
 
@@ -187,66 +192,27 @@
             return FormSum((self, scalar))
         return NotImplemented
 
     def __mul__(self, coefficient):
         """Take the action of this form on the given coefficient."""
         if isinstance(coefficient, Expr):
             from ufl.formoperators import action
+
             return action(self, coefficient)
         return NotImplemented
 
     def __ne__(self, other):
         """Immediately evaluate the != operator (as opposed to the == operator)."""
         return not self.equals(other)
 
-    def __call__(self, *args, **kwargs):
-        """Evaluate form by replacing arguments and coefficients.
-
-        Replaces form.arguments() with given positional arguments in
-        same number and ordering. Number of positional arguments must
-        be 0 or equal to the number of Arguments in the form.
-
-        The optional keyword argument coefficients can be set to a dict
-        to replace Coefficients with expressions of matching shapes.
-
-        Example:
-          V = FiniteElement("CG", triangle, 1)
-          v = TestFunction(V)
-          u = TrialFunction(V)
-          f = Coefficient(V)
-          g = Coefficient(V)
-          a = g*inner(grad(u), grad(v))*dx
-          M = a(f, f, coefficients={ g: 1 })
-
-        Is equivalent to M == grad(f)**2*dx.
-        """
-        repdict = {}
+    def __call__(self, x):
+        """Take the action of this form on ``x``."""
+        from ufl.formoperators import action
 
-        if args:
-            arguments = self.arguments()
-            if len(arguments) != len(args):
-                raise ValueError(f"Need {len(arguments)} arguments to form(), got {len(args)}.")
-            repdict.update(zip(arguments, args))
-
-        coefficients = kwargs.pop("coefficients")
-        if kwargs:
-            raise ValueError(f"Unknown kwargs {list(kwargs)}.")
-
-        if coefficients is not None:
-            coeffs = self.coefficients()
-            for f in coefficients:
-                if f in coeffs:
-                    repdict[f] = coefficients[f]
-                else:
-                    warnings("Coefficient %s is not in form." % ufl_err_str(f))
-        if repdict:
-            from ufl.formoperators import replace
-            return replace(self, repdict)
-        else:
-            return self
+        return action(self, x)
 
     def _ufl_compute_hash_(self):
         """Compute the hash."""
         # Ensure compatibility with MultiFunction
         # `hash(self)` will call the `__hash__` method of the subclass.
         return hash(self)
 
@@ -258,15 +224,16 @@
 
 
 @ufl_type()
 class Form(BaseForm):
     """Description of a weak form consisting of a sum of integrals over subdomains."""
 
     __slots__ = (
-        # --- List of Integral objects (a Form is a sum of these Integrals, everything else is derived)
+        # --- List of Integral objects (a Form is a sum of these
+        # Integrals, everything else is derived)
         "_integrals",
         # --- Internal variables for caching various data
         "_integration_domains",
         "_domain_numbering",
         "_subdomain_data",
         "_arguments",
         "_base_form_operators",
@@ -308,14 +275,15 @@
         self._constant_numbering = None
         self._terminal_numbering = None
 
         # Internal variables for caching base form operator data
         self._base_form_operators = None
 
         from ufl.algorithms.analysis import extract_constants
+
         self._constants = extract_constants(self)
 
         # Internal variables for caching of hash and signature after
         # first request
         self._hash = None
         self._signature = None
 
@@ -326,29 +294,31 @@
 
     def integrals(self):
         """Return a sequence of all integrals in form."""
         return self._integrals
 
     def integrals_by_type(self, integral_type):
         """Return a sequence of all integrals with a particular domain type."""
-        return tuple(integral for integral in self.integrals()
-                     if integral.integral_type() == integral_type)
+        return tuple(
+            integral for integral in self.integrals() if integral.integral_type() == integral_type
+        )
 
     def integrals_by_domain(self, domain):
         """Return a sequence of all integrals with a particular integration domain."""
         return tuple(integral for integral in self.integrals() if integral.ufl_domain() == domain)
 
     def empty(self):
         """Returns whether the form has no integrals."""
         return self.integrals() == ()
 
     def ufl_domains(self):
         """Return the geometric integration domains occuring in the form.
 
-        NB! This does not include domains of coefficients defined on other meshes.
+        NB! This does not include domains of coefficients defined on
+        other meshes.
 
         The return type is a tuple even if only a single domain exists.
         """
         if self._integration_domains is None:
             self._analyze_domains()
         return self._integration_domains
 
@@ -361,34 +331,36 @@
 
     def ufl_domain(self):
         """Return the single geometric integration domain occuring in the form.
 
         Fails if multiple domains are found.
 
         NB! This does not include domains of coefficients defined on
-        other meshes, look at form data for that additional
-        information.
+        other meshes, look at form data for that additional information.
         """
         # Collect all domains
         domains = self.ufl_domains()
         # Check that all are equal TODO: don't return more than one if
         # all are equal?
         if not all(domain == domains[0] for domain in domains):
-            raise ValueError("Calling Form.ufl_domain() is only valid if all integrals share domain.")
+            raise ValueError(
+                "Calling Form.ufl_domain() is only valid if all integrals share domain."
+            )
 
         # Return the one and only domain
         return domains[0]
 
     def geometric_dimension(self):
         """Return the geometric dimension shared by all domains and functions in this form."""
-        gdims = tuple(
-            set(domain.geometric_dimension() for domain in self.ufl_domains()))
+        gdims = tuple(set(domain.geometric_dimension() for domain in self.ufl_domains()))
         if len(gdims) != 1:
-            raise ValueError("Expecting all domains and functions in a form "
-                             f"to share geometric dimension, got {tuple(sorted(gdims))}")
+            raise ValueError(
+                "Expecting all domains and functions in a form "
+                f"to share geometric dimension, got {tuple(sorted(gdims))}"
+            )
         return gdims[0]
 
     def domain_numbering(self):
         """Return a contiguous numbering of domains in a mapping ``{domain:number}``."""
         if self._domain_numbering is None:
             self._analyze_domains()
         return self._domain_numbering
@@ -514,17 +486,15 @@
             # Create form sum if form is of other type
             return FormSum((self, 1), (other, 1))
 
         elif isinstance(other, (int, float)) and other == 0:
             # Allow adding 0 or 0.0 as a no-op, needed for sum([a,b])
             return self
 
-        elif isinstance(
-                other,
-                Zero) and not (other.ufl_shape or other.ufl_free_indices):
+        elif isinstance(other, Zero) and not (other.ufl_shape or other.ufl_free_indices):
             # Allow adding ufl Zero as a no-op, needed for sum([a,b])
             return self
 
         else:
             # Let python protocols do their job if we don't handle it
             return NotImplemented
 
@@ -551,14 +521,15 @@
             return Form([scalar * itg for itg in self.integrals()])
         return NotImplemented
 
     def __mul__(self, coefficient):
         """UFL form operator: Take the action of this form on the given coefficient."""
         if isinstance(coefficient, Expr):
             from ufl.formoperators import action
+
             return action(self, coefficient)
         return NotImplemented
 
     def __call__(self, *args, **kwargs):
         """UFL form operator: Evaluate form by replacing arguments and coefficients.
 
         Replaces form.arguments() with given positional arguments in
@@ -596,35 +567,38 @@
             for f in coefficients:
                 if f in coeffs:
                     repdict[f] = coefficients[f]
                 else:
                     warnings.warn("Coefficient %s is not in form." % ufl_err_str(f))
         if repdict:
             from ufl.formoperators import replace
+
             return replace(self, repdict)
         else:
             return self
 
     __matmul__ = __mul__
 
     # --- String conversion functions, for UI purposes only ---
 
     def __str__(self):
         """Compute shorter string representation of form. This can be huge for complicated forms."""
         # Warning used for making sure we don't use this in the general pipeline:
-        # warning("Calling str on form is potentially expensive and should be avoided except during debugging.")
-        # Not caching this because it can be huge
+        # warning("Calling str on form is potentially expensive and
+        # should be avoided except during debugging.") Not caching this
+        # because it can be huge
         s = "\n  +  ".join(str(itg) for itg in self.integrals())
         return s or "<empty Form>"
 
     def __repr__(self):
         """Compute repr string of form. This can be huge for complicated forms."""
         # Warning used for making sure we don't use this in the general pipeline:
-        # warning("Calling repr on form is potentially expensive and should be avoided except during debugging.")
-        # Not caching this because it can be huge
+        # warning("Calling repr on form is potentially expensive and
+        # should be avoided except during debugging.") Not caching this
+        # because it can be huge
         itgs = ", ".join(repr(itg) for itg in self.integrals())
         r = "Form([" + itgs + "])"
         return r
 
     # --- Analysis functions, precomputation and caching of various quantities
 
     def _analyze_domains(self):
@@ -663,25 +637,25 @@
             else:
                 subdomain_data[domain][it].append(sd)
         self._subdomain_data = subdomain_data
 
     def _analyze_form_arguments(self):
         """Analyze which Argument and Coefficient objects can be found in the form."""
         from ufl.algorithms.analysis import extract_arguments_and_coefficients
+
         arguments, coefficients = extract_arguments_and_coefficients(self)
 
         # Define canonical numbering of arguments and coefficients
-        self._arguments = tuple(
-            sorted(set(arguments), key=lambda x: x.number()))
-        self._coefficients = tuple(
-            sorted(set(coefficients), key=lambda x: x.count()))
+        self._arguments = tuple(sorted(set(arguments), key=lambda x: x.number()))
+        self._coefficients = tuple(sorted(set(coefficients), key=lambda x: x.count()))
 
     def _analyze_base_form_operators(self):
         """Analyze which BaseFormOperator objects can be found in the form."""
         from ufl.algorithms.analysis import extract_base_form_operators
+
         base_form_ops = extract_base_form_operators(self)
         self._base_form_operators = tuple(sorted(base_form_ops, key=lambda x: x.count()))
 
     def _compute_renumbering(self):
         """Compute renumbering."""
         # Include integration domains and coefficients in renumbering
         dn = self.domain_numbering()
@@ -716,14 +690,15 @@
                 k += 1
 
         return renumbering
 
     def _compute_signature(self):
         """Compute signature."""
         from ufl.algorithms.signature import compute_form_signature
+
         self._signature = compute_form_signature(self, self._compute_renumbering())
 
 
 def as_form(form):
     """Convert to form if not a form, otherwise return form."""
     if not isinstance(form, BaseForm) and form != 0:
         raise ValueError(f"Unable to convert object to a UFL form: {ufl_err_str(form)}")
@@ -735,32 +710,36 @@
     """Form sum.
 
     Description of a weighted sum of variational forms and form-like objects
     components is the list of Forms to be summed
     arg_weights is a list of tuples of component index and weight
     """
 
-    __slots__ = ("_arguments",
-                 "_coefficients",
-                 "_weights",
-                 "_components",
-                 "ufl_operands",
-                 "_domains",
-                 "_domain_numbering",
-                 "_hash")
-    _ufl_required_methods_ = ('_analyze_form_arguments')
+    __slots__ = (
+        "_arguments",
+        "_coefficients",
+        "_weights",
+        "_components",
+        "ufl_operands",
+        "_domains",
+        "_domain_numbering",
+        "_hash",
+    )
+    _ufl_required_methods_ = "_analyze_form_arguments"
 
     def __new__(cls, *args, **kwargs):
         """Create a new FormSum."""
         # All the components are `ZeroBaseForm`
         if all(component == 0 for component, _ in args):
-            # Assume that the arguments of all the components have consistent with each other  and select
-            # the first one to define the arguments of `ZeroBaseForm`.
-            # This might not always be true but `ZeroBaseForm`'s arguments are not checked anywhere
-            # because we can't reliably always infer them.
+            # Assume that the arguments of all the components have
+            # consistent with each other  and select the first one to
+            # define the arguments of `ZeroBaseForm`.
+            # This might not always be true but `ZeroBaseForm`'s
+            # arguments are not checked anywhere because we can't
+            # reliably always infer them.
             ((arg, _), *_) = args
             arguments = arg.arguments()
             return ZeroBaseForm(arguments)
 
         return super(FormSum, cls).__new__(cls)
 
     def __init__(self, *components):
@@ -768,15 +747,15 @@
         BaseForm.__init__(self)
 
         # Remove `ZeroBaseForm` components
         filtered_components = [(component, w) for component, w in components if component != 0]
 
         weights = []
         full_components = []
-        for (component, w) in filtered_components:
+        for component, w in filtered_components:
             if isinstance(component, FormSum):
                 full_components.extend(component.components())
                 weights.extend([w * wc for wc in component.weights()])
             else:
                 full_components.append(component)
                 weights.append(w)
 
@@ -799,15 +778,15 @@
         return self._weights
 
     def _sum_variational_components(self):
         """Sum variational components."""
         var_forms = None
         other_components = []
         new_weights = []
-        for (i, component) in enumerate(self._components):
+        for i, component in enumerate(self._components):
             if isinstance(component, Form):
                 if var_forms:
                     var_forms = var_forms + (self._weights[i] * component)
                 else:
                     var_forms = self._weights[i] * component
             else:
                 other_components.append(component)
@@ -821,20 +800,22 @@
     def _analyze_form_arguments(self):
         """Return all ``Argument`` objects found in form."""
         arguments = []
         coefficients = []
         for component in self._components:
             arguments.extend(component.arguments())
             coefficients.extend(component.coefficients())
-        self._arguments = tuple(set(arguments))
-        self._coefficients = tuple(set(coefficients))
+        # Define canonical numbering of arguments and coefficients
+        self._arguments = tuple(sorted(set(arguments), key=lambda x: x.number()))
+        self._coefficients = tuple(sorted(set(coefficients), key=lambda x: x.count()))
 
     def _analyze_domains(self):
         """Analyze which domains can be found in FormSum."""
         from ufl.domain import join_domains
+
         # Collect unique domains
         self._domains = join_domains([component.ufl_domain() for component in self._components])
 
     def __hash__(self):
         """Hash."""
         if self._hash is None:
             self._hash = hash(tuple(hash(component) for component in self.components()))
@@ -842,49 +823,54 @@
 
     def equals(self, other):
         """Evaluate ``bool(lhs_form == rhs_form)``."""
         if type(other) is not FormSum:
             return False
         if self is other:
             return True
-        return (len(self.components()) == len(other.components()) and  # noqa: W504
-                all(a == b for a, b in zip(self.components(), other.components())))
+        return len(self.components()) == len(other.components()) and all(
+            a == b for a, b in zip(self.components(), other.components())
+        )
 
     def __str__(self):
         """Compute shorter string representation of form. This can be huge for complicated forms."""
         # Warning used for making sure we don't use this in the general pipeline:
-        # warning("Calling str on form is potentially expensive and should be avoided except during debugging.")
+        # warning("Calling str on form is potentially expensive and
+        # should be avoided except during debugging.")
         # Not caching this because it can be huge
         s = "\n  +  ".join(str(component) for component in self.components())
         return s or "<empty FormSum>"
 
     def __repr__(self):
         """Compute repr string of form. This can be huge for complicated forms."""
         # Warning used for making sure we don't use this in the general pipeline:
-        # warning("Calling repr on form is potentially expensive and should be avoided except during debugging.")
+        # warning("Calling repr on form is potentially expensive and
+        # should be avoided except during debugging.")
         # Not caching this because it can be huge
         itgs = ", ".join(repr(component) for component in self.components())
         r = "FormSum([" + itgs + "])"
         return r
 
 
 @ufl_type()
 class ZeroBaseForm(BaseForm):
     """Description of a zero base form.
 
     ZeroBaseForm is idempotent with respect to assembly and is mostly
     used for sake of simplifying base-form expressions.
     """
 
-    __slots__ = ("_arguments",
-                 "_coefficients",
-                 "ufl_operands",
-                 "_hash",
-                 # Pyadjoint compatibility
-                 "form")
+    __slots__ = (
+        "_arguments",
+        "_coefficients",
+        "ufl_operands",
+        "_hash",
+        # Pyadjoint compatibility
+        "form",
+    )
 
     def __init__(self, arguments):
         """Initialise."""
         BaseForm.__init__(self)
         self._arguments = arguments
         self.ufl_operands = arguments
         self._hash = None
@@ -900,15 +886,15 @@
         return not self == other
 
     def __eq__(self, other):
         """Check equality."""
         if type(other) is ZeroBaseForm:
             if self is other:
                 return True
-            return (self._arguments == other._arguments)
+            return self._arguments == other._arguments
         elif isinstance(other, (int, float)):
             return other == 0
         else:
             return False
 
     def __str__(self):
         """Format as a string."""
```

### Comparing `fenics-ufl-2023.2.0/ufl/formatting/ufl2unicode.py` & `fenics_ufl-2024.1.0.post0/ufl/formatting/ufl2unicode.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """UFL to unicode."""
 
 import numbers
 
 import ufl
-from ufl.corealg.multifunction import MultiFunction
+from ufl.algorithms import compute_form_data
+from ufl.core.multiindex import FixedIndex, Index
 from ufl.corealg.map_dag import map_expr_dag
-from ufl.core.multiindex import Index, FixedIndex
+from ufl.corealg.multifunction import MultiFunction
 from ufl.form import Form
-from ufl.algorithms import compute_form_data
 
 try:
     import colorama
+
     has_colorama = True
 except ImportError:
     has_colorama = False
 
 
 class PrecedenceRules(MultiFunction):
     """An enum-like class for C operator precedence levels."""
@@ -22,77 +23,85 @@
     def __init__(self):
         """Initialise."""
         MultiFunction.__init__(self)
 
     def highest(self, o):
         """Return the highest precendence."""
         return 0
+
     terminal = highest
     list_tensor = highest
     component_tensor = highest
 
     def restricted(self, o):
         """Return precedence of a restriced."""
         return 5
+
     cell_avg = restricted
     facet_avg = restricted
 
     def call(self, o):
         """Return precedence of a call."""
         return 10
+
     indexed = call
     min_value = call
     max_value = call
     math_function = call
     bessel_function = call
 
     def power(self, o):
         """Return precedence of a power."""
         return 12
 
     def mathop(self, o):
         """Return precedence of a mathop."""
         return 15
+
     derivative = mathop
     trace = mathop
     deviatoric = mathop
     cofactor = mathop
     skew = mathop
     sym = mathop
 
     def not_condition(self, o):
         """Return precedence of a not_condition."""
         return 20
 
     def product(self, o):
         """Return precedence of a product."""
         return 30
+
     division = product
     # mod = product
     dot = product
     inner = product
     outer = product
     cross = product
 
     def add(self, o):
         """Return precedence of an add."""
         return 40
+
     # sub = add
     index_sum = add
 
     def lt(self, o):
         """Return precedence of a lt."""
         return 50
+
     le = lt
     gt = lt
     ge = lt
 
     def eq(self, o):
         """Return precedence of an eq."""
         return 60
+
     ne = eq
 
     def and_condition(self, o):
         """Return precedence of an and_condition."""
         return 70
 
     def or_condition(self, o):
@@ -102,14 +111,15 @@
     def conditional(self, o):
         """Return precedence of a conditional."""
         return 72
 
     def lowest(self, o):
         """Return precedence of a lowest."""
         return 80
+
     operator = lowest
 
 
 _precrules = PrecedenceRules()
 
 
 def precedence(expr):
@@ -117,89 +127,89 @@
     return _precrules(expr)
 
 
 class UC:
     """An enum-like class for unicode characters."""
 
     # Letters in this alphabet have contiguous code point numbers
-    bold_math_a = u"𝐚"
-    bold_math_A = u"𝐀"
+    bold_math_a = "𝐚"
+    bold_math_A = "𝐀"
 
-    thin_space = u"\u2009"
+    thin_space = "\u2009"
 
-    superscript_plus = u"⁺"
-    superscript_minus = u"⁻"
-    superscript_equals = u"⁼"
-    superscript_left_paren = u"⁽"
-    superscript_right_paren = u"⁾"
+    superscript_plus = "⁺"
+    superscript_minus = "⁻"
+    superscript_equals = "⁼"
+    superscript_left_paren = "⁽"
+    superscript_right_paren = "⁾"
     superscript_digits = ["⁰", "¹", "²", "³", "⁴", "⁵", "⁶", "⁷", "⁸", "⁹"]
 
-    subscript_plus = u"₊"
-    subscript_minus = u"₋"
-    subscript_equals = u"₌"
-    subscript_left_paren = u"₍"
-    subscript_right_paren = u"₎"
+    subscript_plus = "₊"
+    subscript_minus = "₋"
+    subscript_equals = "₌"
+    subscript_left_paren = "₍"
+    subscript_right_paren = "₎"
     subscript_digits = ["₀", "₁", "₂", "₃", "₄", "₅", "₆", "₇", "₈", "₉"]
 
-    sqrt = u"√"
-    transpose = u"ᵀ"
+    sqrt = "√"
+    transpose = "ᵀ"
 
-    integral = u"∫"
-    integral_double = u"∬"
-    integral_triple = u"∭"
-    integral_contour = u"∮"
-    integral_surface = u"∯"
-    integral_volume = u"∰"
+    integral = "∫"
+    integral_double = "∬"
+    integral_triple = "∭"
+    integral_contour = "∮"
+    integral_surface = "∯"
+    integral_volume = "∰"
 
-    sum = u"∑"
+    sum = "∑"
     division_slash = "∕"
-    partial = u"∂"
-    epsilon = u"ε"
-    omega = u"ω"
-    Omega = u"Ω"
-    gamma = u"γ"
-    Gamma = u"Γ"
-    nabla = u"∇"
-    for_all = u"∀"
-
-    dot = u"⋅"
-    cross_product = u"⨯"
-    circled_times = u"⊗"
-    nary_product = u"∏"
-
-    ne = u"≠"
-    lt = u"<"
-    le = u"≤"
-    gt = u">"
-    ge = u"≥"
-
-    logical_and = u"∧"
-    logical_or = u"∨"
-    logical_not = u"¬"
-
-    element_of = u"∈"
-    not_element_of = u"∉"
-
-    left_white_square_bracket = u"⟦"
-    right_white_squared_bracket = u"⟧"
-    left_angled_bracket = u"⟨"
-    right_angled_bracket = u"⟩"
-    left_double_angled_bracket = u"⟪"
-    right_double_angled_bracket = u"⟫"
+    partial = "∂"
+    epsilon = "ε"
+    omega = "ω"
+    Omega = "Ω"
+    gamma = "γ"
+    Gamma = "Γ"
+    nabla = "∇"
+    for_all = "∀"
+
+    dot = "⋅"
+    cross_product = "⨯"
+    circled_times = "⊗"
+    nary_product = "∏"
+
+    ne = "≠"
+    lt = "<"
+    le = "≤"
+    gt = ">"
+    ge = "≥"
+
+    logical_and = "∧"
+    logical_or = "∨"
+    logical_not = "¬"
+
+    element_of = "∈"
+    not_element_of = "∉"
+
+    left_white_square_bracket = "⟦"
+    right_white_squared_bracket = "⟧"
+    left_angled_bracket = "⟨"
+    right_angled_bracket = "⟩"
+    left_double_angled_bracket = "⟪"
+    right_double_angled_bracket = "⟫"
 
-    combining_right_arrow_above = "\u20D7"
+    combining_right_arrow_above = "\u20d7"
     combining_overline = "\u0305"
 
 
 def bolden_letter(c):
     """Bolden a letter."""
     if ord("A") <= ord(c) <= ord("Z"):
-        c = chr(ord(c) - ord(u"A") + ord(UC.bold_math_A))
+        c = chr(ord(c) - ord("A") + ord(UC.bold_math_A))
     elif ord("a") <= ord(c) <= ord("z"):
-        c = chr(ord(c) - ord(u"a") + ord(UC.bold_math_a))
+        c = chr(ord(c) - ord("a") + ord(UC.bold_math_a))
     return c
 
 
 def superscript_digit(digit):
     """Make a digit superscript."""
     return UC.superscript_digits[ord(digit) - ord("0")]
 
@@ -207,20 +217,20 @@
 def subscript_digit(digit):
     """Make a digit subscript."""
     return UC.subscript_digits[ord(digit) - ord("0")]
 
 
 def bolden_string(s):
     """Bolden a string."""
-    return u"".join(bolden_letter(c) for c in s)
+    return "".join(bolden_letter(c) for c in s)
 
 
 def overline_string(f):
     """Overline a string."""
-    return u"".join(f"{c}{UC.combining_overline}" for c in f)
+    return "".join(f"{c}{UC.combining_overline}" for c in f)
 
 
 def subscript_number(number):
     """Make a number subscript."""
     assert isinstance(number, int)
     prefix = UC.subscript_minus if number < 0 else ""
     number = str(number)
@@ -241,20 +251,15 @@
 
 
 def measure_font(dx):
     """Use the font for measures."""
     return bolden_string(dx)
 
 
-integral_by_dim = {
-    3: UC.integral_triple,
-    2: UC.integral_double,
-    1: UC.integral,
-    0: UC.integral
-}
+integral_by_dim = {3: UC.integral_triple, 2: UC.integral_double, 1: UC.integral, 0: UC.integral}
 
 integral_type_to_codim = {
     "cell": 0,
     "exterior_facet": 1,
     "interior_facet": 1,
     "vertex": "tdim",
     "point": "tdim",
@@ -296,22 +301,23 @@
     itgdim = tdim - codim
 
     # ipost = integral_postfixes[integral_type]
     istr = integral_by_dim[itgdim]
 
     # TODO: Render domain description
 
-    if isinstance(subdomain_id, numbers.Integral):
-        istr += subscript_number(int(subdomain_id))
-    elif subdomain_id == "everywhere":
-        pass
-    elif subdomain_id == "otherwise":
-        istr += "[rest of domain]"
-    elif isinstance(subdomain_id, tuple):
-        istr += ",".join([subscript_number(int(i)) for i in subdomain_id])
+    subdomain_strs = []
+    for subdomain in subdomain_id:
+        if isinstance(subdomain, numbers.Integral):
+            subdomain_strs.append(subscript_number(int(subdomain)))
+        elif subdomain == "everywhere":
+            pass
+        elif subdomain == "otherwise":
+            subdomain_strs.append("[rest of domain]")
+    istr += ",".join(subdomain_strs)
 
     dxstr = ufl.measure.integral_type_to_measure_name[integral_type]
     dxstr = measure_font(dxstr)
 
     return istr, dxstr
 
 
@@ -361,16 +367,15 @@
     argument_names = None
     coefficient_names = None
 
     # Define form as sum of integrals
     lines = []
     integrals = form.integrals()
     for itg in integrals:
-        integrand_string = expression2unicode(
-            itg.integrand(), argument_names, coefficient_names)
+        integrand_string = expression2unicode(itg.integrand(), argument_names, coefficient_names)
 
         istr, dxstr = get_integral_symbol(itg.integral_type(), itg.ufl_domain(), itg.subdomain_id())
 
         line = f"{istr} {integrand_string} {dxstr}"
         lines.append(line)
 
     return "\n  + ".join(lines)
@@ -778,15 +783,15 @@
     def conditional(self, o, c, t, f):
         """Format a conditional."""
         c = par(c)
         t = par(t)
         f = par(t)
         If = opfont("if")
         Else = opfont("else")
-        return " ".join((t, If, c, Else, f))
+        return f"{t} {If} {c} {Else} {f}"
 
     def min_value(self, o, a, b):
         """Format an min_value."""
         op = opfont("min")
         return f"{op}({a}, {b})"
 
     def max_value(self, o, a, b):
```

### Comparing `fenics-ufl-2023.2.0/ufl/formoperators.py` & `fenics_ufl-2024.1.0.post0/ufl/formoperators.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,45 +5,52 @@
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Anders Logg, 2009
 # Modified by Massimiliano Leoni, 2016
 # Modified by Cecile Daversin-Catty, 2018
 
-from ufl.form import Form, FormSum, BaseForm, ZeroBaseForm, as_form
-from ufl.core.expr import Expr, ufl_err_str
-from ufl.core.base_form_operator import BaseFormOperator
-from ufl.split_functions import split
-from ufl.exprcontainers import ExprList, ExprMapping
-from ufl.variable import Variable
-from ufl.finiteelement import MixedElement
+from ufl.action import Action
+from ufl.adjoint import Adjoint
+from ufl.algorithms import (
+    compute_energy_norm,
+    compute_form_action,
+    compute_form_adjoint,
+    compute_form_functional,
+    compute_form_lhs,
+    compute_form_rhs,
+    expand_derivatives,
+    extract_arguments,
+    formsplitter,
+    replace,  # noqa: F401
+)
 from ufl.argument import Argument
 from ufl.coefficient import Coefficient, Cofunction
-from ufl.adjoint import Adjoint
-from ufl.action import Action
-from ufl.differentiation import (CoefficientDerivative, CoordinateDerivative,
-                                 BaseFormDerivative, BaseFormCoordinateDerivative,
-                                 BaseFormOperatorDerivative, BaseFormOperatorCoordinateDerivative)
-from ufl.constantvalue import is_true_ufl_scalar, as_ufl
-from ufl.indexed import Indexed
+from ufl.constantvalue import as_ufl, is_true_ufl_scalar
+from ufl.core.base_form_operator import BaseFormOperator
+from ufl.core.expr import Expr, ufl_err_str
 from ufl.core.multiindex import FixedIndex, MultiIndex
-from ufl.tensors import as_tensor, ListTensor
-from ufl.sorting import sorted_expr
+from ufl.differentiation import (
+    BaseFormCoordinateDerivative,
+    BaseFormDerivative,
+    BaseFormOperatorCoordinateDerivative,
+    BaseFormOperatorDerivative,
+    CoefficientDerivative,
+    CoordinateDerivative,
+)
+from ufl.exprcontainers import ExprList, ExprMapping
+from ufl.finiteelement import MixedElement
+from ufl.form import BaseForm, Form, FormSum, ZeroBaseForm, as_form
 from ufl.functionspace import FunctionSpace
 from ufl.geometry import SpatialCoordinate
-
-# An exception to the rule that ufl.* does not depend on ufl.algorithms.* ...
-from ufl.algorithms import compute_form_adjoint, compute_form_action
-from ufl.algorithms import compute_energy_norm
-from ufl.algorithms import compute_form_lhs, compute_form_rhs, compute_form_functional
-from ufl.algorithms import expand_derivatives, extract_arguments
-from ufl.algorithms import formsplitter
-
-# Part of the external interface
-from ufl.algorithms import replace  # noqa
+from ufl.indexed import Indexed
+from ufl.sorting import sorted_expr
+from ufl.split_functions import split
+from ufl.tensors import ListTensor, as_tensor
+from ufl.variable import Variable
 
 
 def extract_blocks(form, i=None, j=None):
     """Extract blocks.
 
     Given a linear or bilinear form on a mixed space,
     extract the block corresponding to the indices ix, iy.
@@ -111,16 +118,17 @@
     For formbase objects,coefficient can be any object of the correct type,
     and this function returns an Action object.
 
     When `action` is being called multiple times on the same form, expanding derivatives
     become expensive -> `derivatives_expanded` enables to use caching mechanisms to avoid that.
     """
     form = as_form(form)
-    is_coefficient_valid = (not isinstance(coefficient, BaseForm) or
-                            (isinstance(coefficient, BaseFormOperator) and len(coefficient.arguments()) == 1))
+    is_coefficient_valid = not isinstance(coefficient, BaseForm) or (
+        isinstance(coefficient, BaseFormOperator) and len(coefficient.arguments()) == 1
+    )
     # Can't expand derivatives on objects that are not Form or Expr (e.g. Matrix)
     if isinstance(form, (Form, BaseFormOperator)) and is_coefficient_valid:
         if not derivatives_expanded:
             # For external operators differentiation may turn a Form into a FormSum
             form = expand_derivatives(form)
         if isinstance(form, Form):
             return compute_form_action(form, coefficient)
@@ -195,16 +203,20 @@
     if isinstance(coefficient, (list, tuple, ListTensor)):
         coefficients = tuple(coefficient)
     else:
         coefficients = (coefficient,)
 
     if argument is None:
         # Try to create argument if not provided
-        if not all(isinstance(c, (Coefficient, Cofunction, BaseFormOperator)) for c in coefficients):
-            raise ValueError("Can only create arguments automatically for non-indexed coefficients.")
+        if not all(
+            isinstance(c, (Coefficient, Cofunction, BaseFormOperator)) for c in coefficients
+        ):
+            raise ValueError(
+                "Can only create arguments automatically for non-indexed coefficients."
+            )
 
         # Get existing arguments from form and position the new one
         # with the next argument number
         if isinstance(form, Form):
             form_arguments = form.arguments()
         else:
             # To handle derivative(expression), which is at least used
@@ -219,22 +231,22 @@
         parts = set(arg.part() for arg in form_arguments)
         if len(parts - {None}) != 0:
             raise ValueError("Not expecting parts here, provide your own arguments.")
         part = None
 
         # Create argument and split it if in a mixed space
         function_spaces = [c.ufl_function_space() for c in coefficients]
-        domains = [fs.ufl_domain() for fs in function_spaces]
-        elements = [fs.ufl_element() for fs in function_spaces]
         if len(function_spaces) == 1:
             arguments = (Argument(function_spaces[0], number, part),)
         else:
             # Create in mixed space over assumed (for now) same domain
+            domains = [fs.ufl_domain() for fs in function_spaces]
+            elements = [fs.ufl_element() for fs in function_spaces]
             assert all(fs.ufl_domain() == domains[0] for fs in function_spaces)
-            elm = MixedElement(*elements)
+            elm = MixedElement(elements)
             fs = FunctionSpace(domains[0], elm)
             arguments = split(Argument(fs, number, part))
     else:
         # Wrap single argument in tuple for uniform treatment below
         if isinstance(argument, (list, tuple)):
             arguments = tuple(argument)
         else:
@@ -245,15 +257,15 @@
                 if argument.ufl_shape == (n,):
                     arguments = tuple(argument[i] for i in range(n))
                 else:
                     arguments = split(argument)
 
     # Build mapping from coefficient to argument
     m = {}
-    for (c, a) in zip(coefficients, arguments):
+    for c, a in zip(coefficients, arguments):
         if c.ufl_shape != a.ufl_shape:
             raise ValueError("Coefficient and argument shapes do not match!")
         if isinstance(c, (Coefficient, Cofunction, BaseFormOperator, SpatialCoordinate)):
             m[c] = a
         else:
             if not isinstance(c, Indexed):
                 raise ValueError(f"Invalid coefficient type for {ufl_err_str(c)}")
@@ -301,83 +313,97 @@
     subspace of the coefficient space.
 
     If provided, *coefficient_derivatives* should be a mapping from
     ``Coefficient`` instances to their derivatives w.r.t. *coefficient*.
     """
     if isinstance(form, FormSum):
         # Distribute derivative over FormSum components
-        return FormSum(*[(derivative(component, coefficient, argument, coefficient_derivatives), 1)
-                         for component in form.components()])
+        return FormSum(
+            *[
+                (derivative(component, coefficient, argument, coefficient_derivatives), 1)
+                for component in form.components()
+            ]
+        )
     elif isinstance(form, Adjoint):
         # Is `derivative(Adjoint(A), ...)` with A a 2-form even legal ?
         # -> If yes, what's the right thing to do here ?
-        raise NotImplementedError('Adjoint derivative is not supported.')
+        raise NotImplementedError("Adjoint derivative is not supported.")
     elif isinstance(form, Action):
         # Push derivative through Action slots
         left, right = form.ufl_operands
         # Eagerly simplify spatial derivatives when Action results in a scalar.
         if not len(form.arguments()) and isinstance(coefficient, SpatialCoordinate):
             return ZeroBaseForm(())
 
         if len(left.arguments()) == 1:
             dleft = derivative(left, coefficient, argument, coefficient_derivatives)
             dright = derivative(right, coefficient, argument, coefficient_derivatives)
             # Leibniz formula
-            return (action(adjoint(dleft, derivatives_expanded=True), right, derivatives_expanded=True)
-                    + action(left, dright, derivatives_expanded=True))
+            return action(
+                adjoint(dleft, derivatives_expanded=True), right, derivatives_expanded=True
+            ) + action(left, dright, derivatives_expanded=True)
         else:
-            raise NotImplementedError('Action derivative not supported when the left argument is not a 1-form.')
+            raise NotImplementedError(
+                "Action derivative not supported when the left argument is not a 1-form."
+            )
 
-    coefficients, arguments = _handle_derivative_arguments(form, coefficient,
-                                                           argument)
+    coefficients, arguments = _handle_derivative_arguments(form, coefficient, argument)
     if coefficient_derivatives is None:
         coefficient_derivatives = ExprMapping()
     else:
         cd = []
         for k in sorted_expr(coefficient_derivatives.keys()):
             cd += [as_ufl(k), as_ufl(coefficient_derivatives[k])]
         coefficient_derivatives = ExprMapping(*cd)
 
     # Got a form? Apply derivatives to the integrands in turn.
     if isinstance(form, Form):
         integrals = []
         for itg in form.integrals():
             if isinstance(coefficient, SpatialCoordinate):
-                fd = CoordinateDerivative(itg.integrand(), coefficients,
-                                          arguments, coefficient_derivatives)
-            elif isinstance(coefficient, BaseForm) and not isinstance(coefficient, BaseFormOperator):
+                fd = CoordinateDerivative(
+                    itg.integrand(), coefficients, arguments, coefficient_derivatives
+                )
+            elif isinstance(coefficient, BaseForm) and not isinstance(
+                coefficient, BaseFormOperator
+            ):
                 # Make the `ZeroBaseForm` arguments
                 arguments = form.arguments() + coefficient.arguments()
                 return ZeroBaseForm(arguments)
             else:
-                fd = CoefficientDerivative(itg.integrand(), coefficients,
-                                           arguments, coefficient_derivatives)
+                fd = CoefficientDerivative(
+                    itg.integrand(), coefficients, arguments, coefficient_derivatives
+                )
             integrals.append(itg.reconstruct(fd))
         return Form(integrals)
 
     elif isinstance(form, BaseFormOperator):
         if not isinstance(coefficient, SpatialCoordinate):
-            return BaseFormOperatorDerivative(form, coefficients, arguments, coefficient_derivatives)
+            return BaseFormOperatorDerivative(
+                form, coefficients, arguments, coefficient_derivatives
+            )
         else:
-            return BaseFormOperatorCoordinateDerivative(form, coefficients, arguments, coefficient_derivatives)
+            return BaseFormOperatorCoordinateDerivative(
+                form, coefficients, arguments, coefficient_derivatives
+            )
 
     elif isinstance(form, BaseForm):
         if not isinstance(coefficient, SpatialCoordinate):
             return BaseFormDerivative(form, coefficients, arguments, coefficient_derivatives)
         else:
-            return BaseFormCoordinateDerivative(form, coefficients, arguments, coefficient_derivatives)
+            return BaseFormCoordinateDerivative(
+                form, coefficients, arguments, coefficient_derivatives
+            )
 
     elif isinstance(form, Expr):
         # What we got was in fact an integrand
         if not isinstance(coefficient, SpatialCoordinate):
-            return CoefficientDerivative(form, coefficients,
-                                         arguments, coefficient_derivatives)
+            return CoefficientDerivative(form, coefficients, arguments, coefficient_derivatives)
         else:
-            return CoordinateDerivative(form, coefficients,
-                                        arguments, coefficient_derivatives)
+            return CoordinateDerivative(form, coefficients, arguments, coefficient_derivatives)
 
     raise ValueError(f"Invalid argument type {type(form)}.")
 
 
 def sensitivity_rhs(a, u, L, v):
     r"""Compute the right hand side for a sensitivity calculation system.
 
@@ -401,16 +427,16 @@
 
     and solve this system for :math:`\\frac{dx}{dv}`, using the same bilinear
     form *a* and matrix *A* from the original system.
     Assume the forms are written
     ::
 
         v = variable(v_expression)
-        L = IL(v)*dx
-        a = Ia(v)*dx
+        L = IL(v) * dx
+        a = Ia(v) * dx
 
     where ``IL`` and ``Ia`` are integrand expressions.
     Define a ``Coefficient u`` representing the solution
     to the equations. Then we can compute :math:`\\frac{db}{dv}`
     and :math:`\\frac{dA}{dv}` from the forms
     ::
 
@@ -429,13 +455,21 @@
         dL = diff(L, v) - action(diff(a, v), u)
 
     or, using this function,
     ::
 
         dL = sensitivity_rhs(a, u, L, v)
     """
-    if not (isinstance(a, Form) and isinstance(u, Coefficient) and isinstance(L, Form) and isinstance(v, Variable)):
-        raise ValueError("Expecting (a, u, L, v), (bilinear form, function, linear form and scalar variable).")
+    if not (
+        isinstance(a, Form)
+        and isinstance(u, Coefficient)
+        and isinstance(L, Form)
+        and isinstance(v, Variable)
+    ):
+        raise ValueError(
+            "Expecting (a, u, L, v), (bilinear form, function, linear form and scalar variable)."
+        )
     if not is_true_ufl_scalar(v):
         raise ValueError("Expecting scalar variable.")
     from ufl.operators import diff
+
     return diff(L, v) - action(diff(a, v), u)
```

### Comparing `fenics-ufl-2023.2.0/ufl/functionspace.py` & `fenics_ufl-2024.1.0.post0/ufl/functionspace.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,17 +5,20 @@
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Massimiliano Leoni, 2016
 # Modified by Cecile Daversin-Catty, 2018
 
-from ufl.core.ufl_type import attach_operators_from_hash_data
+import typing
+
+from ufl.core.ufl_type import UFLObject
 from ufl.domain import join_domains
 from ufl.duals import is_dual, is_primal
+from ufl.utils.sequences import product
 
 # Export list for ufl.classes
 __all_classes__ = [
     "AbstractFunctionSpace",
     "FunctionSpace",
     "DualSpace",
     "MixedFunctionSpace",
@@ -25,42 +28,46 @@
 
 class AbstractFunctionSpace(object):
     """Abstract function space."""
 
     def ufl_sub_spaces(self):
         """Return ufl sub spaces."""
         raise NotImplementedError(
-            "Missing implementation of IFunctionSpace.ufl_sub_spaces in %s."
-            % self.__class__.__name__
+            f"Missing implementation of ufl_sub_spaces in {self.__class__.__name__}."
         )
 
 
-@attach_operators_from_hash_data
-class BaseFunctionSpace(AbstractFunctionSpace):
+class BaseFunctionSpace(AbstractFunctionSpace, UFLObject):
     """Base function space."""
 
-    def __init__(self, domain, element):
+    def __init__(self, domain, element, label=""):
         """Initialise."""
         if domain is None:
             # DOLFIN hack
-            # TODO: Is anything expected from element.cell() in this case?
+            # TODO: Is anything expected from element.cell in this case?
             pass
         else:
             try:
                 domain_cell = domain.ufl_cell()
             except AttributeError:
-                raise ValueError("Expected non-abstract domain for initalization of function space.")
+                raise ValueError(
+                    "Expected non-abstract domain for initalization of function space."
+                )
             else:
-                if element.cell() != domain_cell:
+                if element.cell != domain_cell:
                     raise ValueError("Non-matching cell of finite element and domain.")
-
         AbstractFunctionSpace.__init__(self)
+        self._label = label
         self._ufl_domain = domain
         self._ufl_element = element
 
+    def label(self):
+        """Return label of boundary domains to differentiate restricted and unrestricted."""
+        return self._label
+
     def ufl_sub_spaces(self):
         """Return ufl sub spaces."""
         return ()
 
     def ufl_domain(self):
         """Return ufl domain."""
         return self._ufl_domain
@@ -86,144 +93,154 @@
             ddata = None
         else:
             ddata = domain._ufl_hash_data_()
         if element is None:
             edata = None
         else:
             edata = element._ufl_hash_data_()
-        return (name, ddata, edata)
+        return (name, ddata, edata, self.label())
 
     def _ufl_signature_data_(self, renumbering, name=None):
         """UFL signature data."""
         name = name or "BaseFunctionSpace"
         domain = self.ufl_domain()
         element = self.ufl_element()
         if domain is None:
             ddata = None
         else:
             ddata = domain._ufl_signature_data_(renumbering)
         if element is None:
             edata = None
         else:
             edata = element._ufl_signature_data_()
-        return (name, ddata, edata)
+        return (name, ddata, edata, self.label())
 
     def __repr__(self):
         """Representation."""
-        r = "BaseFunctionSpace(%s, %s)" % (repr(self._ufl_domain),
-                                           repr(self._ufl_element))
-        return r
+        return f"BaseFunctionSpace({self._ufl_domain!r}, {self._ufl_element!r})"
+
+    @property
+    def value_shape(self) -> typing.Tuple[int, ...]:
+        """Return the shape of the value space on a physical domain."""
+        return self._ufl_element.pullback.physical_value_shape(self._ufl_element, self._ufl_domain)
 
+    @property
+    def value_size(self) -> int:
+        """Return the integer product of the value shape on a physical domain."""
+        return product(self.value_shape)
 
-@attach_operators_from_hash_data
-class FunctionSpace(BaseFunctionSpace):
+
+class FunctionSpace(BaseFunctionSpace, UFLObject):
     """Representation of a Function space."""
 
     _primal = True
     _dual = False
 
     def dual(self):
         """Get the dual of the space."""
-        return DualSpace(self._ufl_domain, self._ufl_element)
+        return DualSpace(self._ufl_domain, self._ufl_element, label=self.label())
 
     def _ufl_hash_data_(self):
         """UFL hash data."""
         return BaseFunctionSpace._ufl_hash_data_(self, "FunctionSpace")
 
     def _ufl_signature_data_(self, renumbering):
         """UFL signature data."""
         return BaseFunctionSpace._ufl_signature_data_(self, renumbering, "FunctionSpace")
 
     def __repr__(self):
         """Representation."""
-        r = "FunctionSpace(%s, %s)" % (repr(self._ufl_domain),
-                                       repr(self._ufl_element))
-        return r
+        return f"FunctionSpace({self._ufl_domain!r}, {self._ufl_element!r})"
+
+    def __str__(self):
+        """String."""
+        return f"FunctionSpace({self._ufl_domain}, {self._ufl_element})"
 
 
-@attach_operators_from_hash_data
-class DualSpace(BaseFunctionSpace):
+class DualSpace(BaseFunctionSpace, UFLObject):
     """Representation of a Dual space."""
 
     _primal = False
     _dual = True
 
-    def __init__(self, domain, element):
+    def __init__(self, domain, element, label=""):
         """Initialise."""
-        BaseFunctionSpace.__init__(self, domain, element)
+        BaseFunctionSpace.__init__(self, domain, element, label)
 
     def dual(self):
         """Get the dual of the space."""
-        return FunctionSpace(self._ufl_domain, self._ufl_element)
+        return FunctionSpace(self._ufl_domain, self._ufl_element, label=self.label())
 
     def _ufl_hash_data_(self):
         """UFL hash data."""
         return BaseFunctionSpace._ufl_hash_data_(self, "DualSpace")
 
     def _ufl_signature_data_(self, renumbering):
         """UFL signature data."""
         return BaseFunctionSpace._ufl_signature_data_(self, renumbering, "DualSpace")
 
     def __repr__(self):
         """Representation."""
-        r = "DualSpace(%s, %s)" % (repr(self._ufl_domain),
-                                   repr(self._ufl_element))
-        return r
+        return f"DualSpace({self._ufl_domain!r}, {self._ufl_element!r})"
+
+    def __str__(self):
+        """String."""
+        return f"DualSpace({self._ufl_domain}, {self._ufl_element})"
 
 
-@attach_operators_from_hash_data
-class TensorProductFunctionSpace(AbstractFunctionSpace):
+class TensorProductFunctionSpace(AbstractFunctionSpace, UFLObject):
     """Tensor product function space."""
 
     def __init__(self, *function_spaces):
         """Initialise."""
         AbstractFunctionSpace.__init__(self)
         self._ufl_function_spaces = function_spaces
 
     def ufl_sub_spaces(self):
         """Return ufl sub spaces."""
         return self._ufl_function_spaces
 
     def _ufl_hash_data_(self):
         """UFL hash data."""
-        return ("TensorProductFunctionSpace",) \
-            + tuple(V._ufl_hash_data_() for V in self.ufl_sub_spaces())
+        return ("TensorProductFunctionSpace",) + tuple(
+            V._ufl_hash_data_() for V in self.ufl_sub_spaces()
+        )
 
     def _ufl_signature_data_(self, renumbering):
         """UFL signature data."""
-        return ("TensorProductFunctionSpace",) \
-            + tuple(V._ufl_signature_data_(renumbering)
-                    for V in self.ufl_sub_spaces())
+        return ("TensorProductFunctionSpace",) + tuple(
+            V._ufl_signature_data_(renumbering) for V in self.ufl_sub_spaces()
+        )
 
     def __repr__(self):
         """Representation."""
-        r = "TensorProductFunctionSpace(*%s)" % repr(self._ufl_function_spaces)
-        return r
+        return f"TensorProductFunctionSpace(*{self._ufl_function_spaces!r})"
 
+    def __str__(self):
+        """String."""
+        return self.__repr__()
 
-@attach_operators_from_hash_data
-class MixedFunctionSpace(AbstractFunctionSpace):
+
+class MixedFunctionSpace(AbstractFunctionSpace, UFLObject):
     """Mixed function space."""
 
     def __init__(self, *args):
         """Initialise."""
         AbstractFunctionSpace.__init__(self)
         self._ufl_function_spaces = args
         self._ufl_elements = list()
         for fs in args:
             if isinstance(fs, BaseFunctionSpace):
                 self._ufl_elements.append(fs.ufl_element())
             else:
                 raise ValueError("Expecting BaseFunctionSpace objects")
 
         # A mixed FS is only primal/dual if all the subspaces are primal/dual"
-        self._primal = all([is_primal(subspace)
-                            for subspace in self._ufl_function_spaces])
-        self._dual = all([is_dual(subspace)
-                          for subspace in self._ufl_function_spaces])
+        self._primal = all([is_primal(subspace) for subspace in self._ufl_function_spaces])
+        self._dual = all([is_dual(subspace) for subspace in self._ufl_function_spaces])
 
     def ufl_sub_spaces(self):
         """Return ufl sub spaces."""
         return self._ufl_function_spaces
 
     def ufl_sub_space(self, i):
         """Return i-th ufl sub space."""
@@ -237,35 +254,36 @@
 
         If additional arguments are passed, these must be integers. In this
         case, the MixedFunctionSpace which is returned will have dual
         components in the positions corresponding to the arguments passed, and
         the original components in the other positions.
         """
         if args:
-            spaces = [space.dual() if i in args else space
-                      for i, space in enumerate(self._ufl_function_spaces)]
+            spaces = [
+                space.dual() if i in args else space
+                for i, space in enumerate(self._ufl_function_spaces)
+            ]
             return MixedFunctionSpace(*spaces)
         else:
-            return MixedFunctionSpace(
-                *[space.dual()for space in self._ufl_function_spaces]
-            )
+            return MixedFunctionSpace(*[space.dual() for space in self._ufl_function_spaces])
 
     def ufl_elements(self):
         """Return ufl elements."""
         return self._ufl_elements
 
     def ufl_element(self):
         """Return ufl element."""
         if len(self._ufl_elements) == 1:
             return self._ufl_elements[0]
         else:
             raise ValueError(
                 "Found multiple elements. Cannot return only one. "
                 "Consider building a FunctionSpace from a MixedElement "
-                "in case of homogeneous dimension.")
+                "in case of homogeneous dimension."
+            )
 
     def ufl_domains(self):
         """Return ufl domains."""
         domainlist = []
         for s in self._ufl_function_spaces:
             domainlist.extend(s.ufl_domains())
         return join_domains(domainlist)
@@ -282,19 +300,22 @@
 
     def num_sub_spaces(self):
         """Return number of subspaces."""
         return len(self._ufl_function_spaces)
 
     def _ufl_hash_data_(self):
         """UFL hash data."""
-        return ("MixedFunctionSpace",) \
-            + tuple(V._ufl_hash_data_() for V in self.ufl_sub_spaces())
+        return ("MixedFunctionSpace",) + tuple(V._ufl_hash_data_() for V in self.ufl_sub_spaces())
 
     def _ufl_signature_data_(self, renumbering):
         """UFL signature data."""
-        return ("MixedFunctionSpace",) \
-            + tuple(V._ufl_signature_data_(renumbering)
-                    for V in self.ufl_sub_spaces())
+        return ("MixedFunctionSpace",) + tuple(
+            V._ufl_signature_data_(renumbering) for V in self.ufl_sub_spaces()
+        )
 
     def __repr__(self):
         """Representation."""
-        return f"MixedFunctionSpace(*{self._ufl_function_spaces})"
+        return f"MixedFunctionSpace(*{self._ufl_function_spaces!r})"
+
+    def __str__(self):
+        """String."""
+        return self.__repr__()
```

### Comparing `fenics-ufl-2023.2.0/ufl/geometry.py` & `fenics_ufl-2024.1.0.post0/ufl/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
 from ufl.core.terminal import Terminal
 from ufl.core.ufl_type import ufl_type
 from ufl.domain import as_domain, extract_unique_domain
+from ufl.sobolevspace import H1
 
 """
 Possible coordinate bootstrapping:
 
 Xf = Xf[q]
     FacetCoordinate = quadrature point on facet (ds,dS)
 
@@ -69,14 +70,15 @@
 Xf = CFK * (X - X0f)
     FacetCoordinate = CellFacetJacobianInverse * (CellCoordinate - CellFacetOrigin)
 """
 
 
 # --- Expression node types
 
+
 @ufl_type(is_abstract=True)
 class GeometricQuantity(Terminal):
     """Geometric quantity."""
 
     __slots__ = ("_domain",)
 
     def __init__(self, domain):
@@ -132,14 +134,15 @@
     """Geometric facet quantity."""
 
     __slots__ = ()
 
 
 # --- Coordinate represented in different coordinate systems
 
+
 @ufl_type()
 class SpatialCoordinate(GeometricCellQuantity):
     """The coordinate in a domain.
 
     In the context of expression integration,
     represents the domain coordinate of each quadrature point.
 
@@ -239,14 +242,15 @@
         # (with a vertex facet).
         t = self._domain.topological_dimension()
         return t <= 1
 
 
 # --- Origin of coordinate systems in larger coordinate systems
 
+
 @ufl_type()
 class CellOrigin(GeometricCellQuantity):
     """The spatial coordinate corresponding to origin of a reference cell."""
 
     __slots__ = ()
     name = "x0"
 
@@ -287,14 +291,15 @@
         """Get the UFL shape."""
         t = self._domain.topological_dimension()
         return (t,)
 
 
 # --- Jacobians of mappings between coordinate systems
 
+
 @ufl_type()
 class Jacobian(GeometricCellQuantity):
     r"""The Jacobian of the mapping from reference cell to spatial coordinates.
 
     .. math:: J_{ij} = \\frac{dx_i}{dX_j}
     """
 
@@ -451,17 +456,18 @@
     def __init__(self, domain):
         """Initialise."""
         GeometricCellQuantity.__init__(self, domain)
 
     @property
     def ufl_shape(self):
         """Get the UFL shape."""
-        cell = extract_unique_domain(self).ufl_cell()
+        domain = extract_unique_domain(self)
+        cell = domain.ufl_cell()
         nv = cell.num_vertices()
-        g = cell.geometric_dimension()
+        g = domain.geometric_dimension()
         return (nv, g)
 
     def is_cellwise_constant(self):
         """Return whether this expression is spatially constant over each cell."""
         # This is always constant for a given cell type
         return True
 
@@ -479,17 +485,18 @@
         t = self._domain.topological_dimension()
         if t < 2:
             raise ValueError("CellEdgeVectors is only defined for topological dimensions >= 2.")
 
     @property
     def ufl_shape(self):
         """Get the UFL shape."""
-        cell = extract_unique_domain(self).ufl_cell()
+        domain = extract_unique_domain(self)
+        cell = domain.ufl_cell()
         ne = cell.num_edges()
-        g = cell.geometric_dimension()
+        g = domain.geometric_dimension()
         return (ne, g)
 
     def is_cellwise_constant(self):
         """Return whether this expression is spatially constant over each cell."""
         # This is always constant for a given cell type
         return True
 
@@ -507,38 +514,41 @@
         t = self._domain.topological_dimension()
         if t < 3:
             raise ValueError("FacetEdgeVectors is only defined for topological dimensions >= 3.")
 
     @property
     def ufl_shape(self):
         """Get the UFL shape."""
-        cell = extract_unique_domain(self).ufl_cell()
+        domain = extract_unique_domain(self)
+        cell = domain.ufl_cell()
         facet_types = cell.facet_types()
 
         # Raise exception for cells with more than one facet type e.g. prisms
         if len(facet_types) > 1:
             raise Exception(f"Cell type {cell} not supported.")
 
         nfe = facet_types[0].num_edges()
-        g = cell.geometric_dimension()
+        g = domain.geometric_dimension()
         return (nfe, g)
 
     def is_cellwise_constant(self):
         """Return whether this expression is spatially constant over each cell."""
         # This is always constant for a given cell type
         return True
 
 
 # --- Determinants (signed or pseudo) of geometry mapping Jacobians
 
+
 @ufl_type()
 class JacobianDeterminant(GeometricCellQuantity):
     """The determinant of the Jacobian.
 
-    Represents the signed determinant of a square Jacobian or the pseudo-determinant of a non-square Jacobian.
+    Represents the signed determinant of a square Jacobian or the
+    pseudo-determinant of a non-square Jacobian.
     """
 
     __slots__ = ()
     name = "detJ"
 
     def is_cellwise_constant(self):
         """Return whether this expression is spatially constant over each cell."""
@@ -572,19 +582,21 @@
         # Only true for a piecewise linear coordinate field in simplex
         # cells
         return self._domain.is_piecewise_linear_simplex_domain()
 
 
 # --- Inverses (signed or pseudo) of geometry mapping Jacobians
 
+
 @ufl_type()
 class JacobianInverse(GeometricCellQuantity):
     """The inverse of the Jacobian.
 
-    Represents the inverse of a square Jacobian or the pseudo-inverse of a non-square Jacobian.
+    Represents the inverse of a square Jacobian or the pseudo-inverse of
+    a non-square Jacobian.
     """
 
     __slots__ = ()
     name = "K"
 
     @property
     def ufl_shape(self):
@@ -608,15 +620,17 @@
     name = "FK"
 
     def __init__(self, domain):
         """Initialise."""
         GeometricFacetQuantity.__init__(self, domain)
         t = self._domain.topological_dimension()
         if t < 2:
-            raise ValueError("FacetJacobianInverse is only defined for topological dimensions >= 2.")
+            raise ValueError(
+                "FacetJacobianInverse is only defined for topological dimensions >= 2."
+            )
 
     @property
     def ufl_shape(self):
         """Get the UFL shape."""
         g = self._domain.geometric_dimension()
         t = self._domain.topological_dimension()
         return (t - 1, g)
@@ -636,15 +650,17 @@
     name = "CFK"
 
     def __init__(self, domain):
         """Initialise."""
         GeometricFacetQuantity.__init__(self, domain)
         t = self._domain.topological_dimension()
         if t < 2:
-            raise ValueError("CellFacetJacobianInverse is only defined for topological dimensions >= 2.")
+            raise ValueError(
+                "CellFacetJacobianInverse is only defined for topological dimensions >= 2."
+            )
 
     @property
     def ufl_shape(self):
         """Get the UFL shape."""
         t = self._domain.topological_dimension()
         return (t - 1, t)
 
@@ -652,14 +668,15 @@
         """Return whether this expression is spatially constant over each cell."""
         # Only true for a piecewise linear coordinate field in simplex cells
         return self._domain.is_piecewise_linear_simplex_domain()
 
 
 # --- Types representing normal or tangent vectors
 
+
 @ufl_type()
 class FacetNormal(GeometricFacetQuantity):
     """The outwards pointing normal vector of the current facet."""
 
     __slots__ = ()
     name = "n"
 
@@ -671,15 +688,16 @@
 
     def is_cellwise_constant(self):
         """Return whether this expression is spatially constant over each cell."""
         # For product cells, this is only true for some but not all
         # facets. Seems like too much work to fix right now.  Only
         # true for a piecewise linear coordinate field with simplex
         # _facets_.
-        is_piecewise_linear = self._domain.ufl_coordinate_element().degree() == 1
+        ce = self._domain.ufl_coordinate_element()
+        is_piecewise_linear = ce.embedded_superdegree <= 1 and ce in H1
         return is_piecewise_linear and self._domain.ufl_cell().has_simplex_facets()
 
 
 @ufl_type()
 class CellNormal(GeometricCellQuantity):
     """The upwards pointing normal vector of the current manifold cell."""
 
@@ -709,15 +727,17 @@
 
     @property
     def ufl_shape(self):
         """Get the UFL shape."""
         t = self._domain.topological_dimension()
         return (t,)
 
-# --- Types representing measures of the cell and entities of the cell, typically used for stabilisation terms
+
+# --- Types representing measures of the cell and entities of the cell,
+# typically used for stabilisation terms
 
 # TODO: Clean up this set of types? Document!
 
 
 @ufl_type()
 class ReferenceCellVolume(GeometricCellQuantity):
     """The volume of the reference cell."""
@@ -796,14 +816,15 @@
 
     __slots__ = ()
     name = "maxfacetedgelength"
 
 
 # --- Types representing other stuff
 
+
 @ufl_type()
 class CellOrientation(GeometricCellQuantity):
     """The orientation (+1/-1) of the current cell.
 
     For non-manifold cells (tdim == gdim), this equals the sign
     of the Jacobian determinant, i.e. +1 if the physical cell is
     oriented the same way as the reference cell and -1 otherwise.
```

### Comparing `fenics-ufl-2023.2.0/ufl/index_combination_utils.py` & `fenics_ufl-2024.1.0.post0/ufl/index_combination_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
 from ufl.core.multiindex import FixedIndex, Index, indices
 
-
 # FIXME: Some of these might be merged into one function, some might
 # be optimized
 
+
 def unique_sorted_indices(indices):
     """Get unique sorted indices.
 
     Given a list of (id, dim) tuples already sorted by id,
     return a unique list with duplicates removed.
     Also checks that the dimensions of duplicates are matching.
     """
@@ -229,8 +229,13 @@
 
     # Consistency checks
     if len(set(free_indices)) != len(free_indices):
         raise ValueError("Not expecting repeated indices left.")
     if len(free_indices) + 2 * len(repeated_indices) != an + bn:
         raise ValueError("Expecting only twice repeated indices.")
 
-    return tuple(free_indices), tuple(index_dimensions), tuple(repeated_indices), tuple(repeated_index_dimensions)
+    return (
+        tuple(free_indices),
+        tuple(index_dimensions),
+        tuple(repeated_indices),
+        tuple(repeated_index_dimensions),
+    )
```

### Comparing `fenics-ufl-2023.2.0/ufl/indexed.py` & `fenics_ufl-2024.1.0.post0/ufl/indexed.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,24 @@
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
 from ufl.constantvalue import Zero
 from ufl.core.expr import Expr, ufl_err_str
-from ufl.core.ufl_type import ufl_type
+from ufl.core.multiindex import FixedIndex, Index, MultiIndex
 from ufl.core.operator import Operator
-from ufl.core.multiindex import Index, FixedIndex, MultiIndex
+from ufl.core.ufl_type import ufl_type
 from ufl.index_combination_utils import unique_sorted_indices
 from ufl.precedence import parstr
 
 
-# --- Indexed expression ---
-
 @ufl_type(is_shaping=True, num_ops=2, is_terminal_modifier=True)
 class Indexed(Operator):
-    """Indexed."""
+    """Indexed expression."""
 
     __slots__ = (
         "ufl_free_indices",
         "ufl_index_dimensions",
     )
 
     def __new__(cls, expression, multiindex):
@@ -61,18 +59,21 @@
 
         shape = expression.ufl_shape
 
         # Error checking
         if len(shape) != len(multiindex):
             raise ValueError(
                 f"Invalid number of indices ({len(multiindex)}) for tensor "
-                f"expression of rank {len(expression.ufl_shape)}:\n    {ufl_err_str(expression)}")
-        if any(int(di) >= int(si) or int(di) < 0
-               for si, di in zip(shape, multiindex)
-               if isinstance(di, FixedIndex)):
+                f"expression of rank {len(expression.ufl_shape)}:\n    {ufl_err_str(expression)}"
+            )
+        if any(
+            int(di) >= int(si) or int(di) < 0
+            for si, di in zip(shape, multiindex)
+            if isinstance(di, FixedIndex)
+        ):
             raise ValueError("Fixed index out of range!")
 
         # Build tuples of free index ids and dimensions
         efi = expression.ufl_free_indices
         efid = expression.ufl_index_dimensions
         fi = list(zip(efi, efid))
         for pos, ind in enumerate(multiindex._indices):
@@ -97,18 +98,19 @@
         if derivatives:
             return A.evaluate(x, mapping, component, index_values, derivatives)
         else:
             return A.evaluate(x, mapping, component, index_values)
 
     def __str__(self):
         """Format as a string."""
-        return "%s[%s]" % (parstr(self.ufl_operands[0], self),
-                           self.ufl_operands[1])
+        return "%s[%s]" % (parstr(self.ufl_operands[0], self), self.ufl_operands[1])
 
     def __getitem__(self, key):
         """Get an item."""
         if key == ():
             # So that one doesn't have to special case indexing of
             # expressions without shape.
             return self
-        raise ValueError(f"Attempting to index with {ufl_err_str(key)}, "
-                         f"but object is already indexed: {ufl_err_str(self)}")
+        raise ValueError(
+            f"Attempting to index with {ufl_err_str(key)}, "
+            f"but object is already indexed: {ufl_err_str(self)}"
+        )
```

### Comparing `fenics-ufl-2023.2.0/ufl/indexsum.py` & `fenics_ufl-2024.1.0.post0/ufl/indexsum.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 
 # Copyright (C) 2008-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
-
-from ufl.core.ufl_type import ufl_type
+from ufl.constantvalue import Zero
 from ufl.core.expr import Expr, ufl_err_str
-from ufl.core.operator import Operator
 from ufl.core.multiindex import MultiIndex
+from ufl.core.operator import Operator
+from ufl.core.ufl_type import ufl_type
 from ufl.precedence import parstr
-from ufl.constantvalue import Zero
-
 
 # --- Sum over an index ---
 
+
 @ufl_type(num_ops=2)
 class IndexSum(Operator):
     """Index sum."""
 
     __slots__ = ("_dimension", "ufl_free_indices", "ufl_index_dimensions")
 
     def __new__(cls, summand, index):
@@ -32,33 +31,33 @@
             raise ValueError(f"Expecting MultiIndex instance, got {ufl_err_str(index)}")
         if len(index) != 1:
             raise ValueError(f"Expecting a single Index but got {len(index)}.")
 
         # Simplification to zero
         if isinstance(summand, Zero):
             sh = summand.ufl_shape
-            j, = index
+            (j,) = index
             fi = summand.ufl_free_indices
             fid = summand.ufl_index_dimensions
             pos = fi.index(j.count())
-            fi = fi[:pos] + fi[pos + 1:]
-            fid = fid[:pos] + fid[pos + 1:]
+            fi = fi[:pos] + fi[pos + 1 :]
+            fid = fid[:pos] + fid[pos + 1 :]
             return Zero(sh, fi, fid)
 
         return Operator.__new__(cls)
 
     def __init__(self, summand, index):
         """Initialise."""
-        j, = index
+        (j,) = index
         fi = summand.ufl_free_indices
         fid = summand.ufl_index_dimensions
         pos = fi.index(j.count())
         self._dimension = fid[pos]
-        self.ufl_free_indices = fi[:pos] + fi[pos + 1:]
-        self.ufl_index_dimensions = fid[:pos] + fid[pos + 1:]
+        self.ufl_free_indices = fi[:pos] + fi[pos + 1 :]
+        self.ufl_index_dimensions = fid[:pos] + fid[pos + 1 :]
         Operator.__init__(self, (summand, index))
 
     def index(self):
         """Get index."""
         return self.ufl_operands[1][0]
 
     def dimension(self):
@@ -68,20 +67,18 @@
     @property
     def ufl_shape(self):
         """Get UFL shape."""
         return self.ufl_operands[0].ufl_shape
 
     def evaluate(self, x, mapping, component, index_values):
         """Evaluate."""
-        i, = self.ufl_operands[1]
+        (i,) = self.ufl_operands[1]
         tmp = 0
         for k in range(self._dimension):
             index_values.push(i, k)
-            tmp += self.ufl_operands[0].evaluate(x, mapping, component,
-                                                 index_values)
+            tmp += self.ufl_operands[0].evaluate(x, mapping, component, index_values)
             index_values.pop()
         return tmp
 
     def __str__(self):
         """Format as a string."""
-        return "sum_{%s} %s " % (str(self.ufl_operands[1]),
-                                 parstr(self.ufl_operands[0], self))
+        return "sum_{%s} %s " % (str(self.ufl_operands[1]), parstr(self.ufl_operands[0], self))
```

### Comparing `fenics-ufl-2023.2.0/ufl/integral.py` & `fenics_ufl-2024.1.0.post0/ufl/integral.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,45 +6,53 @@
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Anders Logg, 2008-2009
 # Modified by Massimiliano Leoni, 2016.
 
 import ufl
-from ufl.core.expr import Expr
 from ufl.checks import is_python_scalar, is_scalar_constant_expression
-from ufl.measure import Measure  # noqa
+from ufl.core.expr import Expr
 from ufl.protocols import id_or_none
 
 # Export list for ufl.classes
 __all_classes__ = ["Integral"]
 
 
 class Integral(object):
     """An integral over a single domain."""
 
-    __slots__ = ("_integrand", "_integral_type", "_ufl_domain", "_subdomain_id", "_metadata", "_subdomain_data")
+    __slots__ = (
+        "_integrand",
+        "_integral_type",
+        "_ufl_domain",
+        "_subdomain_id",
+        "_metadata",
+        "_subdomain_data",
+    )
 
-    def __init__(
-        self, integrand, integral_type, domain, subdomain_id, metadata, subdomain_data
-    ):
+    def __init__(self, integrand, integral_type, domain, subdomain_id, metadata, subdomain_data):
         """Initialise."""
         if not isinstance(integrand, Expr):
             raise ValueError("Expecting integrand to be an Expr instance.")
         self._integrand = integrand
         self._integral_type = integral_type
         self._ufl_domain = domain
         self._subdomain_id = subdomain_id
         self._metadata = metadata
         self._subdomain_data = subdomain_data
 
     def reconstruct(
-        self, integrand=None,
-        integral_type=None, domain=None, subdomain_id=None,
-        metadata=None, subdomain_data=None
+        self,
+        integrand=None,
+        integral_type=None,
+        domain=None,
+        subdomain_id=None,
+        metadata=None,
+        subdomain_data=None,
     ):
         """Construct a new Integral object with some properties replaced with new values.
 
         Example:
             <a = Integral instance>
             b = a.reconstruct(expand_compounds(a.integrand()))
             c = a.reconstruct(metadata={'quadrature_degree':2})
@@ -96,41 +104,51 @@
         if not is_python_scalar(scalar):
             raise ValueError("Cannot multiply an integral with non-constant values.")
         return self.reconstruct(scalar * self._integrand)
 
     def __rmul__(self, scalar):
         """Multiply."""
         if not is_scalar_constant_expression(scalar):
-            raise ValueError("An integral can only be multiplied by a "
-                             "globally constant scalar expression.")
+            raise ValueError(
+                "An integral can only be multiplied by a globally constant scalar expression."
+            )
         return self.reconstruct(scalar * self._integrand)
 
     def __str__(self):
         """Format as a string."""
         fmt = "{ %s } * %s(%s[%s], %s)"
         mname = ufl.measure.integral_type_to_measure_name[self._integral_type]
         s = fmt % (self._integrand, mname, self._ufl_domain, self._subdomain_id, self._metadata)
         return s
 
     def __repr__(self):
         """Representation."""
-        return (f"Integral({self._integrand!r}, {self._integral_type!r}, {self._ufl_domain!r}, "
-                f"{self._subdomain_id!r}, {self._metadata!r}, {self._subdomain_data!r})")
+        return (
+            f"Integral({self._integrand!r}, {self._integral_type!r}, {self._ufl_domain!r}, "
+            f"{self._subdomain_id!r}, {self._metadata!r}, {self._subdomain_data!r})"
+        )
 
     def __eq__(self, other):
         """Check equality."""
-        return (isinstance(other, Integral) and self._integral_type == other._integral_type and  # noqa: W504
-                self._ufl_domain == other._ufl_domain and self._subdomain_id == other._subdomain_id and  # noqa: W504
-                self._integrand == other._integrand and self._metadata == other._metadata and  # noqa: W504
-                id_or_none(self._subdomain_data) == id_or_none(other._subdomain_data))
+        return (
+            isinstance(other, Integral)
+            and self._integral_type == other._integral_type
+            and self._ufl_domain == other._ufl_domain
+            and self._subdomain_id == other._subdomain_id
+            and self._integrand == other._integrand
+            and self._metadata == other._metadata
+            and id_or_none(self._subdomain_data) == id_or_none(other._subdomain_data)
+        )
 
     def __hash__(self):
         """Hash."""
         # Assuming few collisions by ignoring hash(self._metadata) (a
         # dict is not hashable but we assume it is immutable in
         # practice)
-        hashdata = (hash(self._integrand),
-                    self._integral_type,
-                    hash(self._ufl_domain),
-                    self._subdomain_id,
-                    id_or_none(self._subdomain_data))
+        hashdata = (
+            hash(self._integrand),
+            self._integral_type,
+            hash(self._ufl_domain),
+            self._subdomain_id,
+            id_or_none(self._subdomain_data),
+        )
         return hash(hashdata)
```

### Comparing `fenics-ufl-2023.2.0/ufl/mathfunctions.py` & `fenics_ufl-2024.1.0.post0/ufl/mathfunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,23 +4,31 @@
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Anders Logg, 2008
 # Modified by Kristian B. Oelgaard, 2011
 
-import math
 import cmath
+import math
 import numbers
 import warnings
 
+from ufl.constantvalue import (
+    ComplexValue,
+    ConstantValue,
+    FloatValue,
+    IntValue,
+    RealValue,
+    Zero,
+    as_ufl,
+    is_true_ufl_scalar,
+)
 from ufl.core.operator import Operator
 from ufl.core.ufl_type import ufl_type
-from ufl.constantvalue import (is_true_ufl_scalar, Zero, RealValue, FloatValue, IntValue, ComplexValue,
-                               ConstantValue, as_ufl)
 
 """
 TODO: Include additional functions available in <cmath> (need derivatives as well):
 
 Exponential and logarithmic functions:
 log10    Compute common logarithm (function)
 
@@ -38,14 +46,15 @@
 - BesselJ: cyl_bessel_j(nu, x)
 - BesselY: cyl_neumann(nu, x)
 """
 
 
 # --- Function representations ---
 
+
 @ufl_type(is_abstract=True, is_scalar=True, num_ops=1)
 class MathFunction(Operator):
     """Base class for all unary scalar math functions."""
 
     # Freeze member variables for objects in this class
     __slots__ = ("_name",)
 
@@ -61,15 +70,17 @@
         a = self.ufl_operands[0].evaluate(x, mapping, component, index_values)
         try:
             if isinstance(a, numbers.Real):
                 res = getattr(math, self._name)(a)
             else:
                 res = getattr(cmath, self._name)(a)
         except ValueError:
-            warnings.warn('Value error in evaluation of function %s with argument %s.' % (self._name, a))
+            warnings.warn(
+                "Value error in evaluation of function %s with argument %s." % (self._name, a)
+            )
             raise
         return res
 
     def __str__(self):
         """Format as a string."""
         return "%s(%s)" % (self._name, self.ufl_operands[0])
 
@@ -340,17 +351,19 @@
     def evaluate(self, x, mapping, component, index_values):
         """Evaluate."""
         a = self.ufl_operands[0].evaluate(x, mapping, component, index_values)
         b = self.ufl_operands[1].evaluate(x, mapping, component, index_values)
         try:
             res = math.atan2(a, b)
         except TypeError:
-            raise ValueError('Atan2 does not support complex numbers.')
+            raise ValueError("Atan2 does not support complex numbers.")
         except ValueError:
-            warnings.warn('Value error in evaluation of function atan2 with arguments %s, %s.' % (a, b))
+            warnings.warn(
+                "Value error in evaluation of function atan2 with arguments %s, %s." % (a, b)
+            )
             raise
         return res
 
     def __str__(self):
         """Format as a string."""
         return "atan2(%s,%s)" % (self.ufl_operands[0], self.ufl_operands[1])
 
@@ -379,15 +392,15 @@
         return math.erf(a)
 
 
 @ufl_type(is_abstract=True, is_scalar=True, num_ops=2)
 class BesselFunction(Operator):
     """Base class for all bessel functions."""
 
-    __slots__ = ("_name")
+    __slots__ = "_name"
 
     def __init__(self, name, nu, argument):
         """Initialise."""
         if not is_true_ufl_scalar(nu):
             raise ValueError("Expecting scalar nu.")
         if not is_true_ufl_scalar(argument):
             raise ValueError("Expecting scalar argument.")
@@ -406,30 +419,30 @@
 
     def evaluate(self, x, mapping, component, index_values):
         """Evaluate."""
         a = self.ufl_operands[1].evaluate(x, mapping, component, index_values)
         try:
             import scipy.special
         except ImportError:
-            raise ValueError("You must have scipy installed to evaluate bessel functions in python.")
+            raise ValueError(
+                "You must have scipy installed to evaluate bessel functions in python."
+            )
         name = self._name[-1]
         if isinstance(self.ufl_operands[0], IntValue):
             nu = int(self.ufl_operands[0])
-            functype = 'n' if name != 'i' else 'v'
+            functype = "n" if name != "i" else "v"
         else:
-            nu = self.ufl_operands[0].evaluate(x, mapping, component,
-                                               index_values)
-            functype = 'v'
+            nu = self.ufl_operands[0].evaluate(x, mapping, component, index_values)
+            functype = "v"
         func = getattr(scipy.special, name + functype)
         return func(nu, a)
 
     def __str__(self):
         """Format as a string."""
-        return "%s(%s, %s)" % (self._name, self.ufl_operands[0],
-                               self.ufl_operands[1])
+        return "%s(%s, %s)" % (self._name, self.ufl_operands[0], self.ufl_operands[1])
 
 
 @ufl_type()
 class BesselJ(BesselFunction):
     """Bessel J function."""
 
     __slots__ = ()
```

### Comparing `fenics-ufl-2023.2.0/ufl/matrix.py` & `fenics_ufl-2024.1.0.post0/ufl/matrix.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,43 +3,43 @@
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Nacime Bouziani, 2021-2022.
 
-from ufl.form import BaseForm
-from ufl.core.ufl_type import ufl_type
 from ufl.argument import Argument
+from ufl.core.ufl_type import ufl_type
+from ufl.form import BaseForm
 from ufl.functionspace import AbstractFunctionSpace
 from ufl.utils.counted import Counted
 
-
 # --- The Matrix class represents a matrix, an assembled two form ---
 
+
 @ufl_type()
 class Matrix(BaseForm, Counted):
     """An assemble linear operator between two function spaces."""
 
     __slots__ = (
         "_count",
         "_counted_class",
         "_ufl_function_spaces",
         "ufl_operands",
         "_repr",
         "_hash",
         "_ufl_shape",
         "_arguments",
         "_coefficients",
-        "_domains")
+        "_domains",
+    )
 
     def __getnewargs__(self):
         """Get new args."""
-        return (self._ufl_function_spaces[0], self._ufl_function_spaces[1],
-                self._count)
+        return (self._ufl_function_spaces[0], self._ufl_function_spaces[1], self._count)
 
     def __init__(self, row_space, column_space, count=None):
         """Initialise."""
         BaseForm.__init__(self)
         Counted.__init__(self, count, Matrix)
 
         if not isinstance(row_space, AbstractFunctionSpace):
@@ -49,29 +49,35 @@
             raise ValueError("Expecting a FunctionSpace as the column space.")
 
         self._ufl_function_spaces = (row_space, column_space)
 
         self.ufl_operands = ()
         self._domains = None
         self._hash = None
-        self._repr = f"Matrix({self._ufl_function_spaces[0]!r}, {self._ufl_function_spaces[1]!r}, {self._count!r})"
+        self._repr = (
+            f"Matrix({self._ufl_function_spaces[0]!r} "
+            f"{self._ufl_function_spaces[1]!r}, {self._count!r})"
+        )
 
     def ufl_function_spaces(self):
         """Get the tuple of function spaces of this coefficient."""
         return self._ufl_function_spaces
 
     def _analyze_form_arguments(self):
         """Define arguments of a matrix when considered as a form."""
-        self._arguments = (Argument(self._ufl_function_spaces[0], 0),
-                           Argument(self._ufl_function_spaces[1], 1))
+        self._arguments = (
+            Argument(self._ufl_function_spaces[0], 0),
+            Argument(self._ufl_function_spaces[1], 1),
+        )
         self._coefficients = ()
 
     def _analyze_domains(self):
         """Analyze which domains can be found in a Matrix."""
         from ufl.domain import join_domains
+
         # Collect unique domains
         self._domains = join_domains([fs.ufl_domain() for fs in self._ufl_function_spaces])
 
     def __str__(self):
         """Format as a string."""
         count = str(self._count)
         if len(count) == 1:
@@ -91,8 +97,10 @@
 
     def equals(self, other):
         """Check equality."""
         if type(other) is not Matrix:
             return False
         if self is other:
             return True
-        return self._count == other._count and self._ufl_function_spaces == other._ufl_function_spaces
+        return (
+            self._count == other._count and self._ufl_function_spaces == other._ufl_function_spaces
+        )
```

### Comparing `fenics-ufl-2023.2.0/ufl/measure.py` & `fenics_ufl-2024.1.0.post0/ufl/measure.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,49 +6,49 @@
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Anders Logg 2008-2016
 # Modified by Massimiliano Leoni, 2016.
 
 import numbers
-
 from itertools import chain
 
-from ufl.core.expr import Expr
 from ufl.checks import is_true_ufl_scalar
 from ufl.constantvalue import as_ufl
-from ufl.domain import as_domain, AbstractDomain, extract_domains
+from ufl.core.expr import Expr
+from ufl.domain import AbstractDomain, as_domain, extract_domains
 from ufl.protocols import id_or_none
 
-
 # Export list for ufl.classes
 __all_classes__ = ["Measure", "MeasureSum", "MeasureProduct"]
 
 
 # TODO: Design a class IntegralType(name, shortname, codim, num_cells, ...)?
 # TODO: Improve descriptions below:
 
 # Enumeration of valid domain types
 _integral_types = [
     # === Integration over full topological dimension:
     ("cell", "dx"),  # Over cells of a mesh
-
     # === Integration over topological dimension - 1:
     ("exterior_facet", "ds"),  # Over one-sided exterior facets of a mesh
     ("interior_facet", "dS"),  # Over two-sided facets between pairs of adjacent cells of a mesh
-
     # === Integration over topological dimension 0
     ("vertex", "dP"),  # Over vertices of a mesh
-
     # === Integration over custom domains
     ("custom", "dc"),  # Over custom user-defined domains (run-time quadrature points)
     ("cutcell", "dC"),  # Over a cell with some part cut away (run-time quadrature points)
-    ("interface", "dI"),  # Over a facet fragment overlapping with two or more cells (run-time quadrature points)
-    ("overlap", "dO"),  # Over a cell fragment overlapping with two or more cells (run-time quadrature points)
-
+    (
+        "interface",
+        "dI",
+    ),  # Over a facet fragment overlapping with two or more cells (run-time quadrature points)
+    (
+        "overlap",
+        "dO",
+    ),  # Over a cell fragment overlapping with two or more cells (run-time quadrature points)
     # === Firedrake specifics:
     ("exterior_facet_bottom", "ds_b"),  # Over bottom facets on extruded mesh
     ("exterior_facet_top", "ds_t"),  # Over top facets on extruded mesh
     ("exterior_facet_vert", "ds_v"),  # Over side facets of an extruded mesh
     ("interior_facet_horiz", "dS_h"),  # Over horizontal facets of an extruded mesh
     ("interior_facet_vert", "dS_v"),  # Over vertical facets of an extruded mesh
 ]
@@ -71,16 +71,15 @@
     integral_type_to_measure_name[integral_type] = measure_name
     measure_name_to_integral_type[measure_name] = integral_type
 
 
 def as_integral_type(integral_type):
     """Map short name to long name and require a valid one."""
     integral_type = integral_type.replace(" ", "_")
-    integral_type = measure_name_to_integral_type.get(integral_type,
-                                                      integral_type)
+    integral_type = measure_name_to_integral_type.get(integral_type, integral_type)
     if integral_type not in integral_type_to_measure_name:
         raise ValueError("Invalid integral_type.")
     return integral_type
 
 
 def integral_types():
     """Return a tuple of all domain type strings."""
@@ -98,20 +97,22 @@
     The Measure object holds information about integration properties
     to be transferred to a Form on multiplication with a scalar
     expression.
     """
 
     __slots__ = ("_integral_type", "_domain", "_subdomain_id", "_metadata", "_subdomain_data")
 
-    def __init__(self,
-                 integral_type,  # "dx" etc
-                 domain=None,
-                 subdomain_id="everywhere",
-                 metadata=None,
-                 subdomain_data=None):
+    def __init__(
+        self,
+        integral_type,  # "dx" etc
+        domain=None,
+        subdomain_id="everywhere",
+        metadata=None,
+        subdomain_data=None,
+    ):
         """Initialise.
 
         Args:
             integral_type: one of "cell", etc, or short form "dx", etc
             domain: an AbstractDomain object (most often a Mesh)
             subdomain_id: either string "everywhere", a single subdomain id int, or tuple of ints
             metadata: dict, with additional compiler-specific parameters
@@ -119,17 +120,19 @@
                 for optimization or debugging of generated code
             subdomain_data: object representing data to interpret subdomain_id with
         """
         # Map short name to long name and require a valid one
         self._integral_type = as_integral_type(integral_type)
 
         # Check that we either have a proper AbstractDomain or none
-        self._domain = None if domain is None else as_domain(domain)
-        if not (self._domain is None or isinstance(self._domain, AbstractDomain)):
-            raise ValueError("Invalid domain.")
+        if domain is not None:
+            domain = as_domain(domain)
+            if not isinstance(domain, AbstractDomain):
+                raise ValueError("Invalid domain.")
+        self._domain = domain
 
         # Store subdomain data
         self._subdomain_data = subdomain_data
         # FIXME: Cannot require this (yet) because we currently have
         # no way to implement ufl_id for dolfin SubDomain
         # if not (self._subdomain_data is None or hasattr(self._subdomain_data, "ufl_id")):
         #     raise ValueError("Invalid domain data, missing ufl_id() implementation.")
@@ -173,20 +176,17 @@
 
         This data is not interpreted by UFL.
         It is passed to the form compiler which can ignore it or use
         it to compile each integral of a form in a different way.
         """
         return self._metadata
 
-    def reconstruct(self,
-                    integral_type=None,
-                    subdomain_id=None,
-                    domain=None,
-                    metadata=None,
-                    subdomain_data=None):
+    def reconstruct(
+        self, integral_type=None, subdomain_id=None, domain=None, metadata=None, subdomain_data=None
+    ):
         """Construct a new Measure object with some properties replaced with new values.
 
         Example:
             <dm = Measure instance>
             b = dm.reconstruct(subdomain_id=2)
             c = dm.reconstruct(metadata={ "quadrature_degree": 3 })
 
@@ -198,65 +198,80 @@
             subdomain_id = self.subdomain_id()
         if domain is None:
             domain = self.ufl_domain()
         if metadata is None:
             metadata = self.metadata()
         if subdomain_data is None:
             subdomain_data = self.subdomain_data()
-        return Measure(self.integral_type(),
-                       domain=domain, subdomain_id=subdomain_id,
-                       metadata=metadata, subdomain_data=subdomain_data)
+        return Measure(
+            self.integral_type(),
+            domain=domain,
+            subdomain_id=subdomain_id,
+            metadata=metadata,
+            subdomain_data=subdomain_data,
+        )
 
     def subdomain_data(self):
         """Return the integral subdomain_data.
 
         This data is not interpreted by
         UFL.  Its intension is to give a context in which the domain
         id is interpreted.
         """
         return self._subdomain_data
 
     # Note: Must keep the order of the first two arguments here
     # (subdomain_id, metadata) for backwards compatibility, because
     # some tutorials write e.g. dx(0, {...}) to set metadata.
-    def __call__(self, subdomain_id=None, metadata=None, domain=None,
-                 subdomain_data=None, degree=None, scheme=None):
+    def __call__(
+        self,
+        subdomain_id=None,
+        metadata=None,
+        domain=None,
+        subdomain_data=None,
+        degree=None,
+        scheme=None,
+    ):
         """Reconfigure measure with new domain specification or metadata."""
         # Let syntax dx() mean integral over everywhere
-        all_args = (subdomain_id, metadata, domain, subdomain_data,
-                    degree, scheme)
+        all_args = (subdomain_id, metadata, domain, subdomain_data, degree, scheme)
         if all(arg is None for arg in all_args):
             return self.reconstruct(subdomain_id="everywhere")
 
         # Let syntax dx(domain) or dx(domain, metadata) mean integral
         # over entire domain.  To do this we need to hijack the first
         # argument:
         if subdomain_id is not None and (
-            isinstance(subdomain_id, AbstractDomain) or hasattr(subdomain_id, 'ufl_domain')
+            isinstance(subdomain_id, AbstractDomain) or hasattr(subdomain_id, "ufl_domain")
         ):
             if domain is not None:
-                raise ValueError("Ambiguous: setting domain both as keyword argument and first argument.")
-            subdomain_id, domain = "everywhere", as_domain(subdomain_id)
+                raise ValueError(
+                    "Ambiguous: setting domain both as keyword argument and first argument."
+                )
+            subdomain_id, domain = "everywhere", subdomain_id
 
         # If degree or scheme is set, inject into metadata. This is a
         # quick fix to enable the dx(..., degree=3) notation.
         # TODO: Make degree and scheme properties of integrals instead of adding to metadata.
         if (degree, scheme) != (None, None):
             metadata = {} if metadata is None else metadata.copy()
             if degree is not None:
                 metadata["quadrature_degree"] = degree
             if scheme is not None:
                 metadata["quadrature_rule"] = scheme
 
         # If we get any keywords, use them to reconstruct Measure.
         # Note that if only one argument is given, it is the
         # subdomain_id, e.g. dx(3) == dx(subdomain_id=3)
-        return self.reconstruct(subdomain_id=subdomain_id, domain=domain,
-                                metadata=metadata,
-                                subdomain_data=subdomain_data)
+        return self.reconstruct(
+            subdomain_id=subdomain_id,
+            domain=domain,
+            metadata=metadata,
+            subdomain_data=subdomain_data,
+        )
 
     def __str__(self):
         """Format as a string."""
         name = integral_type_to_measure_name[self._integral_type]
         args = []
 
         if self._subdomain_id is not None:
@@ -264,15 +279,15 @@
         if self._domain is not None:
             args.append("domain=%s" % (self._domain,))
         if self._metadata:  # Stored as {} if None
             args.append("metadata=%s" % (self._metadata,))
         if self._subdomain_data is not None:
             args.append("subdomain_data=%s" % (self._subdomain_data,))
 
-        return "%s(%s)" % (name, ', '.join(args))
+        return "%s(%s)" % (name, ", ".join(args))
 
     def __repr__(self):
         """Return a repr string for this Measure."""
         args = []
         args.append(repr(self._integral_type))
 
         if self._subdomain_id is not None:
@@ -280,36 +295,42 @@
         if self._domain is not None:
             args.append("domain=%s" % repr(self._domain))
         if self._metadata:  # Stored as {} if None
             args.append("metadata=%s" % repr(self._metadata))
         if self._subdomain_data is not None:
             args.append("subdomain_data=%s" % repr(self._subdomain_data))
 
-        r = "%s(%s)" % (type(self).__name__, ', '.join(args))
+        r = "%s(%s)" % (type(self).__name__, ", ".join(args))
         return r
 
     def __hash__(self):
         """Return a hash value for this Measure."""
         metadata_hashdata = tuple(sorted((k, id(v)) for k, v in list(self._metadata.items())))
-        hashdata = (self._integral_type,
-                    self._subdomain_id,
-                    hash(self._domain),
-                    metadata_hashdata,
-                    id_or_none(self._subdomain_data))
+        hashdata = (
+            self._integral_type,
+            self._subdomain_id,
+            hash(self._domain),
+            metadata_hashdata,
+            id_or_none(self._subdomain_data),
+        )
         return hash(hashdata)
 
     def __eq__(self, other):
         """Checks if two Measures are equal."""
         sorted_metadata = sorted((k, id(v)) for k, v in list(self._metadata.items()))
         sorted_other_metadata = sorted((k, id(v)) for k, v in list(other._metadata.items()))
 
-        return (isinstance(other, Measure) and self._integral_type == other._integral_type and  # noqa: W504
-                self._subdomain_id == other._subdomain_id and self._domain == other._domain and  # noqa: W504
-                id_or_none(self._subdomain_data) == id_or_none(other._subdomain_data) and  # noqa: W504
-                sorted_metadata == sorted_other_metadata)
+        return (
+            isinstance(other, Measure)
+            and self._integral_type == other._integral_type
+            and self._subdomain_id == other._subdomain_id
+            and self._domain == other._domain
+            and id_or_none(self._subdomain_data) == id_or_none(other._subdomain_data)
+            and sorted_metadata == sorted_other_metadata
+        )
 
     def __add__(self, other):
         """Add two measures (self+other).
 
         Creates an intermediate object used for the notation
           expr * (dx(1) + dx(2)) := expr * dx(1) + expr * dx(2)
         """
@@ -340,16 +361,16 @@
 
         This is to implement the notation
             form = integrand * self
 
         Integration properties are taken from this Measure object.
         """
         # Avoid circular imports
-        from ufl.integral import Integral
         from ufl.form import Form
+        from ufl.integral import Integral
 
         # Allow python literals: 1*dx and 1.0*dx
         if isinstance(integrand, (int, float)):
             integrand = as_ufl(integrand)
 
         # Let other types implement multiplication with Measure if
         # they want to (to support the dolfin-adjoint TimeMeasure)
@@ -357,47 +378,66 @@
             return NotImplemented
 
         # Allow only scalar integrands
         if not is_true_ufl_scalar(integrand):
             raise ValueError(
                 "Can only integrate scalar expressions. The integrand is a "
                 f"tensor expression with value shape {integrand.ufl_shape} and "
-                f"free indices with labels {integrand.ufl_free_indices}.")
+                f"free indices with labels {integrand.ufl_free_indices}."
+            )
 
         # If we have a tuple of domain ids build the integrals one by
         # one and construct as a Form in one go.
         subdomain_id = self.subdomain_id()
         if isinstance(subdomain_id, tuple):
-            return Form(list(chain(*((integrand * self.reconstruct(subdomain_id=d)).integrals()
-                                     for d in subdomain_id))))
+            return Form(
+                list(
+                    chain(
+                        *(
+                            (integrand * self.reconstruct(subdomain_id=d)).integrals()
+                            for d in subdomain_id
+                        )
+                    )
+                )
+            )
 
         # Check that we have an integer subdomain or a string
         # ("everywhere" or "otherwise", any more?)
-        if not isinstance(subdomain_id, (str, numbers.Integral,)):
+        if not isinstance(
+            subdomain_id,
+            (
+                str,
+                numbers.Integral,
+            ),
+        ):
             raise ValueError("Expecting integer or string domain id.")
 
         # If we don't have an integration domain, try to find one in
         # integrand
         domain = self.ufl_domain()
         if domain is None:
             domains = extract_domains(integrand)
             if len(domains) == 1:
-                domain, = domains
+                (domain,) = domains
             elif len(domains) == 0:
                 raise ValueError("This integral is missing an integration domain.")
             else:
-                raise ValueError("Multiple domains found, making the choice of integration domain ambiguous.")
+                raise ValueError(
+                    "Multiple domains found, making the choice of integration domain ambiguous."
+                )
 
         # Otherwise create and return a one-integral form
-        integral = Integral(integrand=integrand,
-                            integral_type=self.integral_type(),
-                            domain=domain,
-                            subdomain_id=subdomain_id,
-                            metadata=self.metadata(),
-                            subdomain_data=self.subdomain_data())
+        integral = Integral(
+            integrand=integrand,
+            integral_type=self.integral_type(),
+            domain=domain,
+            subdomain_id=subdomain_id,
+            metadata=self.metadata(),
+            subdomain_data=self.subdomain_data(),
+        )
         return Form([integral])
 
 
 class MeasureSum(object):
     """Represents a sum of measures.
 
     This is a notational intermediate object to translate the notation
```

### Comparing `fenics-ufl-2023.2.0/ufl/objects.py` & `fenics_ufl-2024.1.0.post0/ufl/objects.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Anders Logg, 2008
 # Modified by Kristian Oelgaard, 2009
 
-from ufl.core.multiindex import indices
 from ufl.cell import Cell
-from ufl.measure import Measure
-from ufl.measure import integral_type_to_measure_name
+from ufl.core.multiindex import indices
+from ufl.measure import Measure, integral_type_to_measure_name
 
 # Default indices
 i, j, k, l = indices(4)  # noqa: E741
 p, q, r, s = indices(4)
 
 for integral_type, measure_name in integral_type_to_measure_name.items():
     globals()[measure_name] = Measure(integral_type)
@@ -23,20 +22,20 @@
 # TODO: Firedrake hack, remove later
 ds_tb = ds_b + ds_t  # noqa: F821
 
 # Default measure dX including both uncut and cut cells
 dX = dx + dC  # noqa: F821
 
 # Create objects for builtin known cell types
-vertex = Cell("vertex", 0)
-interval = Cell("interval", 1)
-triangle = Cell("triangle", 2)
-tetrahedron = Cell("tetrahedron", 3)
-prism = Cell("prism", 3)
-pyramid = Cell("pyramid", 3)
-quadrilateral = Cell("quadrilateral", 2)
-hexahedron = Cell("hexahedron", 3)
-tesseract = Cell("tesseract", 4)
-pentatope = Cell("pentatope", 4)
+vertex = Cell("vertex")
+interval = Cell("interval")
+triangle = Cell("triangle")
+tetrahedron = Cell("tetrahedron")
+prism = Cell("prism")
+pyramid = Cell("pyramid")
+quadrilateral = Cell("quadrilateral")
+hexahedron = Cell("hexahedron")
+tesseract = Cell("tesseract")
+pentatope = Cell("pentatope")
 
 # Facet is just a dummy declaration for RestrictedElement
 facet = "facet"
```

### Comparing `fenics-ufl-2023.2.0/ufl/operators.py` & `fenics_ufl-2024.1.0.post0/ufl/operators.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,38 +10,75 @@
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Kristian B. Oelgaard, 2011
 # Modified by Massimiliano Leoni, 2016.
 
-import warnings
 import operator
+import warnings
 
-from ufl.form import Form
-from ufl.constantvalue import Zero, RealValue, ComplexValue, as_ufl
-from ufl.differentiation import VariableDerivative, Grad, Div, Curl, NablaGrad, NablaDiv
-from ufl.tensoralgebra import (
-    Transposed, Inner, Outer, Dot, Cross, Perp,
-    Determinant, Inverse, Cofactor, Trace, Deviatoric, Skew, Sym)
-from ufl.coefficient import Coefficient
-from ufl.variable import Variable
-from ufl.tensors import as_tensor, as_matrix, as_vector, ListTensor
-from ufl.conditional import (
-    EQ, NE, AndCondition, OrCondition, NotCondition, Conditional, MaxValue, MinValue)
-from ufl.algebra import Conj, Real, Imag
-from ufl.mathfunctions import (
-    Sqrt, Exp, Ln, Erf, Cos, Sin, Tan, Cosh, Sinh, Tanh, Acos, Asin, Atan, Atan2,
-    BesselJ, BesselY, BesselI, BesselK)
+from ufl import sobolevspace
+from ufl.algebra import Conj, Imag, Real
 from ufl.averaging import CellAvg, FacetAvg
-from ufl.indexed import Indexed
-from ufl.geometry import SpatialCoordinate, FacetNormal
 from ufl.checks import is_cellwise_constant
+from ufl.coefficient import Coefficient
+from ufl.conditional import (
+    EQ,
+    NE,
+    AndCondition,
+    Conditional,
+    MaxValue,
+    MinValue,
+    NotCondition,
+    OrCondition,
+)
+from ufl.constantvalue import ComplexValue, RealValue, Zero, as_ufl
+from ufl.differentiation import Curl, Div, Grad, NablaDiv, NablaGrad, VariableDerivative
 from ufl.domain import extract_domains
-from ufl import sobolevspace
+from ufl.form import Form
+from ufl.geometry import FacetNormal, SpatialCoordinate
+from ufl.indexed import Indexed
+from ufl.mathfunctions import (
+    Acos,
+    Asin,
+    Atan,
+    Atan2,
+    BesselI,
+    BesselJ,
+    BesselK,
+    BesselY,
+    Cos,
+    Cosh,
+    Erf,
+    Exp,
+    Ln,
+    Sin,
+    Sinh,
+    Sqrt,
+    Tan,
+    Tanh,
+)
+from ufl.tensoralgebra import (
+    Cofactor,
+    Cross,
+    Determinant,
+    Deviatoric,
+    Dot,
+    Inner,
+    Inverse,
+    Outer,
+    Perp,
+    Skew,
+    Sym,
+    Trace,
+    Transposed,
+)
+from ufl.tensors import ListTensor, as_matrix, as_tensor, as_vector
+from ufl.variable import Variable
 
 # --- Basic operators ---
 
 
 def rank(f):
     """The rank of f."""
     f = as_ufl(f)
@@ -52,21 +89,23 @@
     """The shape of f."""
     f = as_ufl(f)
     return f.ufl_shape
 
 
 # --- Complex operators ---
 
+
 def conj(f):
     """The complex conjugate of f."""
     f = as_ufl(f)
     return Conj(f)
 
 
-# Alias because both conj and conjugate are in numpy and we wish to be consistent.
+# Alias because both conj and conjugate are in numpy and we wish to be
+# consistent.
 conjugate = conj
 
 
 def real(f):
     """The real part of f."""
     f = as_ufl(f)
     return Real(f)
@@ -76,14 +115,15 @@
     """The imaginary part of f."""
     f = as_ufl(f)
     return Imag(f)
 
 
 # --- Elementwise tensor operators ---
 
+
 def elem_op_items(op_ind, indices, *args):
     """Elem op items."""
     sh = args[0].ufl_shape
     indices = tuple(indices)
     n = sh[len(indices)]
 
     def extind(ii):
@@ -92,25 +132,30 @@
     if len(sh) == len(indices) + 1:
         return [op_ind(extind(i), *args) for i in range(n)]
     else:
         return [elem_op_items(op_ind, extind(i), *args) for i in range(n)]
 
 
 def elem_op(op, *args):
-    """Take the elementwise application of operator op on scalar values from one or more tensor arguments."""
+    """Apply element-wise operations.
+
+    Take the element-wise application of operator op on scalar values
+    from one or more tensor arguments.
+    """
     args = [as_ufl(arg) for arg in args]
     sh = args[0].ufl_shape
     if not all(sh == x.ufl_shape for x in args):
-        raise ValueError("Cannot take elementwise operation with different shapes.")
+        raise ValueError("Cannot take element-wise operation with different shapes.")
 
     if sh == ():
         return op(*args)
 
     def op_ind(ind, *args):
         return op(*[x[ind] for x in args])
+
     return as_tensor(elem_op_items(op_ind, (), *args))
 
 
 def elem_mult(A, B):
     """Take the elementwise multiplication of tensors A and B with the same shape."""
     return elem_op(operator.mul, A, B)
 
@@ -123,14 +168,15 @@
 def elem_pow(A, B):
     """Take the elementwise power of tensors A and B with the same shape."""
     return elem_op(operator.pow, A, B)
 
 
 # --- Tensor operators ---
 
+
 def transpose(A):
     """Take the transposed of tensor A."""
     A = as_ufl(A)
     if A.ufl_shape == ():
         return A
     return Transposed(A)
 
@@ -222,24 +268,27 @@
 def tr(A):
     """Take the trace of A."""
     A = as_ufl(A)
     return Trace(A)
 
 
 def diag(A):
-    """Take the diagonal part of rank 2 tensor A or make a diagonal rank 2 tensor from a rank 1 tensor.
+    """Diagonal ranl-2 tensor.
+
+    Take the diagonal part of rank 2 tensor A or make a diagonal rank 2
+    tensor from a rank 1 tensor.
 
     Always returns a rank 2 tensor. See also diag_vector.
     """
     # TODO: Make a compound type or two for this operator
 
     # Get and check dimensions
     r = len(A.ufl_shape)
     if r == 1:
-        n, = A.ufl_shape
+        (n,) = A.ufl_shape
     elif r == 2:
         m, n = A.ufl_shape
         if m != n:
             raise ValueError("Can only take diagonal of square tensors.")
     else:
         raise ValueError("Expecting rank 1 or 2 tensor.")
 
@@ -286,14 +335,15 @@
     """Take the symmetric part of A."""
     A = as_ufl(A)
     return Sym(A)
 
 
 # --- Differential operators
 
+
 def Dx(f, *i):
     """Take the partial derivative of f with respect to spatial variable number i.
 
     Equivalent to f.dx(*i).
     """
     f = as_ufl(f)
     return f.dx(*i)
@@ -314,14 +364,15 @@
     """Take the derivative of f with respect to the variable v.
 
     If f is a form, diff is applied to each integrand.
     """
     # Apply to integrands
     if isinstance(f, Form):
         from ufl.algorithms.map_integrands import map_integrands
+
         return map_integrands(lambda e: diff(e, v), f)
 
     # Apply to expression
     f = as_ufl(f)
     if isinstance(v, SpatialCoordinate):
         return grad(f)
     elif isinstance(v, (Variable, Coefficient)):
@@ -399,67 +450,72 @@
 
 
 rot = curl
 
 
 # --- DG operators ---
 
+
 def jump(v, n=None):
     """Take the jump of v across a facet."""
     v = as_ufl(v)
     is_constant = len(extract_domains(v)) > 0
     if is_constant:
         if n is None:
-            return v('+') - v('-')
+            return v("+") - v("-")
         r = len(v.ufl_shape)
         if r == 0:
-            return v('+') * n('+') + v('-') * n('-')
+            return v("+") * n("+") + v("-") * n("-")
         else:
-            return dot(v('+'), n('+')) + dot(v('-'), n('-'))
+            return dot(v("+"), n("+")) + dot(v("-"), n("-"))
     else:
-        warnings.warn("Returning zero from jump of expression without a domain. "
-                      "This may be erroneous if a dolfin.Expression is involved.")
+        warnings.warn(
+            "Returning zero from jump of expression without a domain. "
+            "This may be erroneous if a dolfin.Expression is involved."
+        )
         # FIXME: Is this right? If v has no domain, it doesn't depend
         # on anything spatially variable or any form arguments, and
         # thus the jump is zero. In other words, I'm assuming that "v
         # has no geometric domains" is equivalent with "v is a spatial
         # constant".  Update: This is NOT true for
         # jump(Expression("x[0]")) from dolfin.
         return Zero(v.ufl_shape, v.ufl_free_indices, v.ufl_index_dimensions)
 
 
 def avg(v):
     """Take the average of v across a facet."""
     v = as_ufl(v)
-    return 0.5 * (v('+') + v('-'))
+    return 0.5 * (v("+") + v("-"))
 
 
 def cell_avg(f):
     """Take the average of v over a cell."""
     return CellAvg(f)
 
 
 def facet_avg(f):
     """Take the average of v over a facet."""
     return FacetAvg(f)
 
 
 # --- Other operators ---
 
+
 def variable(e):
     """Define a variable representing the given expression.
 
     See also diff().
     """
     e = as_ufl(e)
     return Variable(e)
 
 
 # --- Conditional expressions ---
 
+
 def conditional(condition, true_value, false_value):
     """A conditional expression.
 
     This takes the value of true_value
     when condition evaluates to true and false_value otherwise.
     """
     return Conditional(condition, true_value, false_value)
@@ -531,14 +587,15 @@
     x = as_ufl(x)
     y = as_ufl(y)
     return MinValue(x, y)
 
 
 # --- Math functions ---
 
+
 def _mathfunction(f, cls):
     """A mat function."""
     f = as_ufl(f)
     r = cls(f)
     if isinstance(r, (RealValue, Zero, int, float)):
         return float(r)
     if isinstance(r, (ComplexValue, complex)):
@@ -607,15 +664,15 @@
 
 
 def atan2(f1, f2):
     """Take the inverse tangent with two the arguments f1 and f2."""
     f1 = as_ufl(f1)
     f2 = as_ufl(f2)
     if isinstance(f1, (ComplexValue, complex)) or isinstance(f2, (ComplexValue, complex)):
-        raise TypeError('atan2 is incompatible with complex numbers.')
+        raise TypeError("atan2 is incompatible with complex numbers.")
     r = Atan2(f1, f2)
     if isinstance(r, (RealValue, Zero, int, float)):
         return float(r)
     if isinstance(r, (ComplexValue, complex)):
         return complex(r)
     return r
 
@@ -651,14 +708,15 @@
     nu = as_ufl(nu)
     f = as_ufl(f)
     return BesselK(nu, f)
 
 
 # --- Special function for exterior_derivative
 
+
 def exterior_derivative(f):
     """Take the exterior derivative of f.
 
     The exterior derivative uses the element Sobolev space to
     determine whether id, grad, curl or div should be used.
 
     Note that this uses the grad and div operators,
@@ -667,31 +725,43 @@
     # Extract the element from the input f
     if isinstance(f, Indexed):
         expression, indices = f.ufl_operands
         if len(indices) > 1:
             raise NotImplementedError
         index = int(indices[0])
         element = expression.ufl_element()
-        element = element.extract_component(index)[1]
+        while index != 0:
+            for e in element.sub_elements:
+                if e.value_size > index:
+                    element = e
+                    break
+                index -= e.value_size
     elif isinstance(f, ListTensor):
         f0 = f.ufl_operands[0]
         f0expr, f0indices = f0.ufl_operands  # FIXME: Assumption on type of f0!!!
         if len(f0indices) > 1:
             raise NotImplementedError
         index = int(f0indices[0])
         element = f0expr.ufl_element()
-        element = element.extract_component(index)[1]
+        while index != 0:
+            for e in element.sub_elements:
+                if e.value_size > index:
+                    element = e
+                    break
+                index -= e.value_size
     else:
         try:
             element = f.ufl_element()
         except Exception:
             raise ValueError(f"Unable to determine element from {f}")
 
-    gdim = element.cell().geometric_dimension()
-    space = element.sobolev_space()
+    domain = f.ufl_domain()
+
+    gdim = domain.geometric_dimension()
+    space = element.sobolev_space
 
     if space == sobolevspace.L2:
         return f
     elif space == sobolevspace.H1:
         if gdim == 1:
             return grad(f)[0]  # Special-case 1D vectors as scalars
         return grad(f)
```

### Comparing `fenics-ufl-2023.2.0/ufl/permutation.py` & `fenics_ufl-2024.1.0.post0/ufl/permutation.py`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/ufl/precedence.py` & `fenics_ufl-2024.1.0.post0/ufl/precedence.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
 import warnings
 
-
 # FIXME: This code is crap...
 
+
 def parstr(child, parent, pre="(", post=")", format=str):
     """Parstr."""
     # Execute when needed instead of on import, which leads to all
     # kinds of circular trouble.  Fixing this could be an optimization
     # of str(expr) though.
-    if not hasattr(parent, '_precedence'):
+    if not hasattr(parent, "_precedence"):
         assign_precedences(build_precedence_list())
 
     # We want child to be evaluated fully first, and if the parent has
     # higher precedence we later wrap in ().
     s = format(child)
 
     # Operators where operands are always parenthesized because
@@ -37,31 +37,47 @@
 
     # Nothing needed
     return s
 
 
 def build_precedence_list():
     """Build precedence list."""
-    from ufl.classes import (Operator, Terminal, Sum, IndexSum, Product, Division, Power,
-                             MathFunction, BesselFunction, Abs, Indexed)
+    from ufl.classes import (
+        Abs,
+        BesselFunction,
+        Division,
+        Indexed,
+        IndexSum,
+        MathFunction,
+        Operator,
+        Power,
+        Product,
+        Sum,
+        Terminal,
+    )
 
     # TODO: Fill in other types...
     # Power <= Transposed
 
     precedence_list = []
     # Default operator behaviour: should always add parentheses
     precedence_list.append((Operator,))
 
     precedence_list.append((Sum,))
 
     # sum_i a + b = (sum_i a) + b != sum_i (a + b), sum_i binds
     # stronger than +, but weaker than product
     precedence_list.append((IndexSum,))
 
-    precedence_list.append((Product, Division,))
+    precedence_list.append(
+        (
+            Product,
+            Division,
+        )
+    )
 
     # NB! Depends on language!
     precedence_list.append((Power, MathFunction, BesselFunction, Abs))
 
     precedence_list.append((Indexed,))
 
     # Default terminal behaviour: should never add parentheses
@@ -70,15 +86,16 @@
 
 
 def build_precedence_mapping(precedence_list):
     """Given a precedence list, build a dict with class->int mappings.
 
     Utility function used by some external code.
     """
-    from ufl.classes import Expr, all_ufl_classes, abstract_classes
+    from ufl.classes import Expr, abstract_classes, all_ufl_classes
+
     pm = {}
     missing = set()
     # Assign integer values for each precedence level
     k = 0
     for p in precedence_list:
         for c in p:
             pm[c] = k
@@ -99,8 +116,11 @@
 
 def assign_precedences(precedence_list):
     """Given a precedence list, assign ints to class._precedence."""
     pm, missing = build_precedence_mapping(precedence_list)
     for c, p in sorted(pm.items(), key=lambda x: x[0].__name__):
         c._precedence = p
     if missing:
-        warnings.warn("Missing precedence levels for classes:\n" + "\n".join(f"  {c}" for c in sorted(missing)))
+        warnings.warn(
+            "Missing precedence levels for classes:\n"
+            + "\n".join(f"  {c}" for c in sorted(missing))
+        )
```

### Comparing `fenics-ufl-2023.2.0/ufl/protocols.py` & `fenics_ufl-2024.1.0.post0/ufl/protocols.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 
     This allows external libraries to implement an alternative
     to id(obj) in the ufl_id() function, such that ufl can identify
     objects as the same without knowing about their types.
     """
     if obj is None:
         return None
-    elif hasattr(obj, 'ufl_id'):
+    elif hasattr(obj, "ufl_id"):
         return obj.ufl_id()
     else:
         return id(obj)
```

### Comparing `fenics-ufl-2023.2.0/ufl/referencevalue.py` & `fenics_ufl-2024.1.0.post0/ufl/algorithms/apply_function_pullbacks.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,61 @@
-"""Representation of the reference value of a function."""
+"""Algorithm for replacing gradients in an expression."""
+
 # Copyright (C) 2008-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
-from ufl.core.ufl_type import ufl_type
-from ufl.core.operator import Operator
-from ufl.core.terminal import FormArgument
-
-
-@ufl_type(num_ops=1,
-          is_index_free=True,
-          is_terminal_modifier=True,
-          is_in_reference_frame=True)
-class ReferenceValue(Operator):
-    """Representation of the reference cell value of a form argument."""
-
-    __slots__ = ()
-
-    def __init__(self, f):
-        """Initialise."""
-        if not isinstance(f, FormArgument):
-            raise ValueError("Can only take reference value of form arguments.")
-        Operator.__init__(self, (f,))
-
-    @property
-    def ufl_shape(self):
-        """Get the UFL shape."""
-        return self.ufl_operands[0].ufl_element().reference_value_shape()
-
-    def evaluate(self, x, mapping, component, index_values, derivatives=()):
-        """Get child from mapping and return the component asked for."""
-        raise NotImplementedError()
-
-    def __str__(self):
-        """Format as a string."""
-        return f"reference_value({self.ufl_operands[0]})"
+from ufl.algorithms.map_integrands import map_integrand_dags
+from ufl.classes import ReferenceValue
+from ufl.corealg.multifunction import MultiFunction, memoized_handler
+
+
+class FunctionPullbackApplier(MultiFunction):
+    """A pull back applier."""
+
+    def __init__(self):
+        """Initalise."""
+        MultiFunction.__init__(self)
+
+    expr = MultiFunction.reuse_if_untouched
+
+    def terminal(self, t):
+        """Apply to a terminal."""
+        return t
+
+    @memoized_handler
+    def form_argument(self, o):
+        """Apply to a form_argument."""
+        # Represent 0-derivatives of form arguments on reference
+        # element
+        r = ReferenceValue(o)
+        space = o.ufl_function_space()
+        element = o.ufl_element()
+
+        if r.ufl_shape != element.reference_value_shape:
+            raise ValueError(
+                "Expecting reference space expression with shape "
+                f"'{element.reference_value_shape}', got '{r.ufl_shape}'"
+            )
+        f = element.pullback.apply(r)
+        if f.ufl_shape != space.value_shape:
+            raise ValueError(
+                f"Expecting pulled back expression with shape '{space.value_shape}', "
+                f"got '{f.ufl_shape}'"
+            )
+
+        assert f.ufl_shape == o.ufl_shape
+        return f
+
+
+def apply_function_pullbacks(expr):
+    """Change representation of coefficients and arguments in an expression.
+
+    Applies Piola mappings where applicable and represents all
+    form arguments in reference value.
+
+    Args:
+        expr: An Expression
+    """
+    return map_integrand_dags(FunctionPullbackApplier(), expr)
```

### Comparing `fenics-ufl-2023.2.0/ufl/restriction.py` & `fenics_ufl-2024.1.0.post0/ufl/restriction.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 # Copyright (C) 2008-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
 from ufl.core.operator import Operator
-from ufl.precedence import parstr
 from ufl.core.ufl_type import ufl_type
-
+from ufl.precedence import parstr
 
 # --- Restriction operators ---
 
-@ufl_type(is_abstract=True,
-          num_ops=1,
-          inherit_shape_from_operand=0,
-          inherit_indices_from_operand=0,
-          is_restriction=True)
+
+@ufl_type(
+    is_abstract=True,
+    num_ops=1,
+    inherit_shape_from_operand=0,
+    inherit_indices_from_operand=0,
+    is_restriction=True,
+)
 class Restricted(Operator):
     """Restriction."""
 
     __slots__ = ()
 
     # TODO: Add __new__ operator here, e.g. restricted(literal) == literal
 
@@ -30,16 +32,15 @@
 
     def side(self):
         """Get the side."""
         return self._side
 
     def evaluate(self, x, mapping, component, index_values):
         """Evaluate."""
-        return self.ufl_operands[0].evaluate(x, mapping, component,
-                                             index_values)
+        return self.ufl_operands[0].evaluate(x, mapping, component, index_values)
 
     def __str__(self):
         """Format as a string."""
         return f"{parstr(self.ufl_operands[0], self)}({self._side})"
 
 
 @ufl_type(is_terminal_modifier=True)
```

### Comparing `fenics-ufl-2023.2.0/ufl/sobolevspace.py` & `fenics_ufl-2024.1.0.post0/ufl/sobolevspace.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,21 +14,24 @@
 # Modified by Martin Alnaes 2014
 # Modified by Lizao Li 2015
 # Modified by Thomas Gibson 2017
 
 from functools import total_ordering
 from math import inf, isinf
 
+__all_classes__ = ["SobolevSpace", "DirectionalSobolevSpace"]
+
 
 @total_ordering
 class SobolevSpace(object):
     """Symbolic representation of a Sobolev space.
 
-    This implements a subset of the methods of a Python set so that finite elements and
-    other Sobolev spaces can be tested for inclusion.
+    This implements a subset of the methods of a Python set so that
+    finite elements and other Sobolev spaces can be tested for
+    inclusion.
     """
 
     def __init__(self, name, parents=None):
         """Instantiate a SobolevSpace object.
 
         Args:
             name: The name of this space,
@@ -46,15 +49,15 @@
             "HInf": inf,
             # Order for the elements below is taken from
             # its parent Sobolev space
             "HDiv": 0,
             "HCurl": 0,
             "HEin": 0,
             "HDivDiv": 0,
-            "DirectionalH": 0
+            "DirectionalH": 0,
         }[self.name]
 
     def __str__(self):
         """Format as a string."""
         return self.name
 
     def __repr__(self):
@@ -76,100 +79,92 @@
     def __getitem__(self, spatial_index):
         """Returns the Sobolev space associated with a particular spatial coordinate."""
         return self
 
     def __contains__(self, other):
         """Implement `fe in s` where `fe` is a FiniteElement and `s` is a SobolevSpace."""
         if isinstance(other, SobolevSpace):
-            raise TypeError("Unable to test for inclusion of a "
-                            "SobolevSpace in another SobolevSpace. "
-                            "Did you mean to use <= instead?")
-        return other.sobolev_space() == self or self in other.sobolev_space().parents
+            raise TypeError(
+                "Unable to test for inclusion of a SobolevSpace in another SobolevSpace. "
+                "Did you mean to use <= instead?"
+            )
+        return other.sobolev_space == self or self in other.sobolev_space.parents
 
     def __lt__(self, other):
         """In common with intrinsic Python sets, < indicates "is a proper subset of"."""
         return other in self.parents
 
-    def __call__(self, element):
-        """Syntax shortcut to create a HDivElement or HCurlElement."""
-        if self.name == "HDiv":
-            from ufl.finiteelement import HDivElement
-            return HDivElement(element)
-        elif self.name == "HCurl":
-            from ufl.finiteelement import HCurlElement
-            return HCurlElement(element)
-        raise NotImplementedError(
-            "SobolevSpace has no call operator (only the specific HDiv and HCurl instances)."
-        )
-
 
 @total_ordering
 class DirectionalSobolevSpace(SobolevSpace):
     """Directional Sobolev space.
 
     Symbolic representation of a Sobolev space with varying smoothness
-    in differerent spatial directions.
+    in different spatial directions.
     """
 
     def __init__(self, orders):
         """Instantiate a DirectionalSobolevSpace object.
 
         Args:
             orders: an iterable of orders of weak derivatives, where
                 the position denotes in what spatial variable the
                 smoothness requirement is enforced.
         """
         assert all(
-            isinstance(x, int) or isinf(x)
-            for x in orders), "Order must be an integer or infinity."
+            isinstance(x, int) or isinf(x) for x in orders
+        ), "Order must be an integer or infinity."
         name = "DirectionalH"
         parents = [L2]
         super(DirectionalSobolevSpace, self).__init__(name, parents)
         self._orders = tuple(orders)
         self._spatial_indices = range(len(self._orders))
 
     def __getitem__(self, spatial_index):
         """Returns the Sobolev space associated with a particular spatial coordinate."""
         if spatial_index not in range(len(self._orders)):
             raise IndexError("Spatial index out of range.")
         spaces = {0: L2, 1: H1, 2: H2, inf: HInf}
         return spaces[self._orders[spatial_index]]
 
     def __contains__(self, other):
-        """Implement `fe in s` where `fe` is a FiniteElement and `s` is a DirectionalSobolevSpace."""
+        """Check if one space is contained in another.
+
+        Implement `fe in s` where `fe` is a FiniteElement and `s` is a
+        DirectionalSobolevSpace.
+        """
         if isinstance(other, SobolevSpace):
-            raise TypeError("Unable to test for inclusion of a "
-                            "SobolevSpace in another SobolevSpace. "
-                            "Did you mean to use <= instead?")
-        return (other.sobolev_space() == self or all(
-            self[i] in other.sobolev_space().parents
-            for i in self._spatial_indices))
+            raise TypeError(
+                "Unable to test for inclusion of a SobolevSpace in another SobolevSpace. "
+                "Did you mean to use <= instead?"
+            )
+        return other.sobolev_space == self or all(
+            self[i] in other.sobolev_space.parents for i in self._spatial_indices
+        )
 
     def __eq__(self, other):
         """Check equality."""
         if isinstance(other, DirectionalSobolevSpace):
             return self._orders == other._orders
         return all(self[i] == other for i in self._spatial_indices)
 
     def __lt__(self, other):
         """In common with intrinsic Python sets, < indicates "is a proper subset of."""
         if isinstance(other, DirectionalSobolevSpace):
             if self._spatial_indices != other._spatial_indices:
                 return False
-            return any(self._orders[i] > other._orders[i]
-                       for i in self._spatial_indices)
+            return any(self._orders[i] > other._orders[i] for i in self._spatial_indices)
 
         if other in [HDiv, HCurl]:
             return all(self._orders[i] >= 1 for i in self._spatial_indices)
         elif other.name in ["HDivDiv", "HEin"]:
             # Don't know how these spaces compare
             return NotImplementedError(f"Don't know how to compare with {other.name}")
         else:
-            return any(
-                self._orders[i] > other._order for i in self._spatial_indices)
+            return any(self._orders[i] > other._order for i in self._spatial_indices)
 
     def __str__(self):
         """Format as a string."""
         return f"{self.name}({', '.join(map(str, self._orders))})"
 
 
 L2 = SobolevSpace("L2")
```

### Comparing `fenics-ufl-2023.2.0/ufl/sorting.py` & `fenics_ufl-2024.1.0.post0/ufl/sorting.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Anders Logg, 2009-2010.
 # Modified by Johan Hake, 2010.
 
 from functools import cmp_to_key
 
-from ufl.core.expr import Expr
 from ufl.argument import Argument
 from ufl.coefficient import Coefficient
 from ufl.core.multiindex import FixedIndex, MultiIndex
 from ufl.variable import Label
 
 
 def _cmp_multi_index(a, b):
@@ -94,15 +93,15 @@
     # The cost of repr on a terminal is fairly small, and bounded
     x = repr(a)
     y = repr(b)
     return -1 if x < y else (0 if x == y else 1)
 
 
 # Hack up a MultiFunction-like type dispatch for terminal comparisons
-_terminal_cmps = [_cmp_terminal_by_repr] * Expr._ufl_num_typecodes_
+_terminal_cmps = {}
 _terminal_cmps[MultiIndex._ufl_typecode_] = _cmp_multi_index
 _terminal_cmps[Argument._ufl_typecode_] = _cmp_argument
 _terminal_cmps[Coefficient._ufl_typecode_] = _cmp_coefficient
 _terminal_cmps[Label._ufl_typecode_] = _cmp_label
 
 
 def cmp_expr(a, b):
@@ -116,15 +115,19 @@
         x, y = a._ufl_typecode_, b._ufl_typecode_
         if x != y:
             return -1 if x < y else 1
 
         # Now we know that the type is the same, check further based
         # on type specific properties.
         if a._ufl_is_terminal_:
-            c = _terminal_cmps[x](a, b)
+            if x in _terminal_cmps:
+                c = _terminal_cmps[x](a, b)
+            else:
+                c = _cmp_terminal_by_repr(a, b)
+
             if c:
                 return c
         else:
             # If the hash is the same, assume equal for the purpose of
             # sorting.  This introduces a minor chance of
             # nondeterministic behaviour, just as with MultiIndex.
             # Although collected statistics for complicated forms
@@ -134,15 +137,15 @@
             #    return 0
 
             # Delve into subtrees
             aops = a.ufl_operands
             bops = b.ufl_operands
 
             # Sort by children in natural order
-            for (r, s) in zip(aops, bops):
+            for r, s in zip(aops, bops):
                 # Skip subtree if objects are the same
                 if r is s:
                     continue
                 # Append subtree for further inspection
                 left.append((r, s))
 
             # All children compare as equal, a and b must be
```

### Comparing `fenics-ufl-2023.2.0/ufl/split_functions.py` & `fenics_ufl-2024.1.0.post0/ufl/split_functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Anders Logg, 2008
 
-from ufl.utils.sequences import product
-from ufl.finiteelement import TensorElement
-from ufl.tensors import as_vector, as_matrix, ListTensor
+from ufl.functionspace import FunctionSpace
 from ufl.indexed import Indexed
 from ufl.permutation import compute_indices
+from ufl.tensors import ListTensor, as_matrix, as_vector
 from ufl.utils.indexflattening import flatten_multiindex, shape_to_strides
+from ufl.utils.sequences import product
 
 
 def split(v):
     """Split a coefficient or argument.
 
-    If v is a Coefficient or Argument in a mixed space, returns
-    a tuple with the function components corresponding to the subelements.
+    If v is a Coefficient or Argument in a mixed space, returns a tuple
+    with the function components corresponding to the subelements.
     """
+    domain = v.ufl_domain()
+
     # Default range is all of v
     begin = 0
     end = None
 
     if isinstance(v, Indexed):
         # Special case: split previous output of split again
         # Consistent with simple element, just return function in a tuple
@@ -35,77 +37,81 @@
         ops = v.ufl_operands
         if all(isinstance(comp, Indexed) for comp in ops):
             args = [comp.ufl_operands[0] for comp in ops]
             if all(args[0] == args[i] for i in range(1, len(args))):
                 # Get innermost terminal here and its element
                 v = args[0]
                 # Get relevant range of v components
-                begin, = ops[0].ufl_operands[1]
-                end, = ops[-1].ufl_operands[1]
+                (begin,) = ops[0].ufl_operands[1]
+                (end,) = ops[-1].ufl_operands[1]
                 begin = int(begin)
                 end = int(end) + 1
             else:
                 raise ValueError(f"Don't know how to split {v}.")
         else:
             raise ValueError(f"Don't know how to split {v}.")
 
     # Special case: simple element, just return function in a tuple
     element = v.ufl_element()
-    if element.num_sub_elements() == 0:
+    if element.num_sub_elements == 0:
         assert end is None
         return (v,)
 
-    if isinstance(element, TensorElement):
-        if element.symmetry():
-            raise ValueError("Split not implemented for symmetric tensor elements.")
-
     if len(v.ufl_shape) != 1:
-        raise ValueError("Don't know how to split tensor valued mixed functions without flattened index space.")
+        raise ValueError(
+            "Don't know how to split tensor valued mixed functions without flattened index space."
+        )
 
     # Compute value size and set default range end
-    value_size = product(element.value_shape())
+    value_size = v.ufl_function_space().value_size
     if end is None:
         end = value_size
     else:
         # Recursively dive into mixedelement in to subelement
         # corresponding to beginning of range
         j = begin
         while True:
-            sub_i, j = element.extract_subelement_component(j)
-            element = element.sub_elements()[sub_i]
+            for e in element.sub_elements:
+                if j < FunctionSpace(domain, e).value_size:
+                    element = e
+                    break
+                j -= FunctionSpace(domain, e).value_size
             # Then break when we find the subelement that covers the whole range
-            if product(element.value_shape()) == (end - begin):
+            if FunctionSpace(domain, element).value_size == (end - begin):
                 break
 
     # Build expressions representing the subfunction of v for each subelement
     offset = begin
     sub_functions = []
-    for i, e in enumerate(element.sub_elements()):
+    for i, e in enumerate(element.sub_elements):
         # Get shape, size, indices, and v components
         # corresponding to subelement value
-        shape = e.value_shape()
+        shape = FunctionSpace(domain, e).value_shape
         strides = shape_to_strides(shape)
         rank = len(shape)
         sub_size = product(shape)
-        subindices = [flatten_multiindex(c, strides)
-                      for c in compute_indices(shape)]
+        subindices = [flatten_multiindex(c, strides) for c in compute_indices(shape)]
         components = [v[k + offset] for k in subindices]
 
         # Shape components into same shape as subelement
         if rank == 0:
-            subv, = components
+            (subv,) = components
         elif rank <= 1:
             subv = as_vector(components)
         elif rank == 2:
-            subv = as_matrix([components[i * shape[1]: (i + 1) * shape[1]]
-                              for i in range(shape[0])])
+            subv = as_matrix(
+                [components[i * shape[1] : (i + 1) * shape[1]] for i in range(shape[0])]
+            )
         else:
-            raise ValueError(f"Don't know how to split functions with sub functions of rank {rank}.")
+            raise ValueError(
+                f"Don't know how to split functions with sub functions of rank {rank}."
+            )
 
         offset += sub_size
         sub_functions.append(subv)
 
     if end != offset:
         raise ValueError(
-            "Function splitting failed to extract components for whole intended range. Something is wrong.")
+            "Function splitting failed to extract components for whole intended range."
+        )
 
     return tuple(sub_functions)
```

### Comparing `fenics-ufl-2023.2.0/ufl/tensoralgebra.py` & `fenics_ufl-2024.1.0.post0/ufl/tensoralgebra.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Compound tensor algebra operations."""
 # Copyright (C) 2008-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
+from ufl.algebra import Conj, Operator
+from ufl.constantvalue import Zero
 from ufl.core.expr import ufl_err_str
 from ufl.core.ufl_type import ufl_type
-from ufl.constantvalue import Zero
-from ufl.algebra import Operator, Conj
+from ufl.index_combination_utils import merge_nonoverlapping_indices
 from ufl.precedence import parstr
 from ufl.sorting import sorted_expr
-from ufl.index_combination_utils import merge_nonoverlapping_indices
 
 # Algebraic operations on tensors:
 # FloatValues:
 #   dot(a,b)      = a*b
 #   inner(a,b)    = a*b
 #   outer(a,b)    = a*b
 # Vectors:
@@ -37,24 +37,26 @@
 # Argument requirements:
 #   dot(x,y):   last index of x has same dimension as first index of y
 #   inner(x,y): shape of x equals the shape of y
 
 
 # --- Classes representing compound tensor algebra operations ---
 
+
 @ufl_type(is_abstract=True)
 class CompoundTensorOperator(Operator):
     """Compount tensor operator."""
 
     __slots__ = ()
 
     def __init__(self, operands):
         """Initialise."""
         Operator.__init__(self, operands)
 
+
 # TODO: Use this and make Sum handle scalars only?
 #       This would simplify some algorithms. The only
 #       problem is we can't use + in many algorithms because
 #       this type should be expanded by expand_compounds.
 # class TensorSum(CompoundTensorOperator):
 #     "Sum of nonscalar expressions."
 #     pass
@@ -140,16 +142,18 @@
     @property
     def ufl_shape(self):
         """Get the UFL shape."""
         return self.ufl_operands[0].ufl_shape + self.ufl_operands[1].ufl_shape
 
     def __str__(self):
         """Format as a string."""
-        return "%s (X) %s" % (parstr(self.ufl_operands[0], self),
-                              parstr(self.ufl_operands[1], self))
+        return "%s (X) %s" % (
+            parstr(self.ufl_operands[0], self),
+            parstr(self.ufl_operands[1], self),
+        )
 
 
 @ufl_type(num_ops=2)
 class Inner(CompoundTensorOperator):
     """Inner."""
 
     __slots__ = ("ufl_free_indices", "ufl_index_dimensions")
@@ -183,36 +187,36 @@
         self.ufl_free_indices = fi
         self.ufl_index_dimensions = fid
 
     ufl_shape = ()
 
     def __str__(self):
         """Format as a string."""
-        return "%s : %s" % (parstr(self.ufl_operands[0], self),
-                            parstr(self.ufl_operands[1], self))
+        return "%s : %s" % (parstr(self.ufl_operands[0], self), parstr(self.ufl_operands[1], self))
 
 
 @ufl_type(num_ops=2)
 class Dot(CompoundTensorOperator):
     """Dot."""
 
     __slots__ = ("ufl_free_indices", "ufl_index_dimensions")
 
     def __new__(cls, a, b):
         """Create new Dot."""
         ash = a.ufl_shape
         bsh = b.ufl_shape
         ar, br = len(ash), len(bsh)
-        scalar = (ar == 0 and br == 0)
+        scalar = ar == 0 and br == 0
 
         # Checks
         if not ((ar >= 1 and br >= 1) or scalar):
             raise ValueError(
                 "Dot product requires non-scalar arguments, "
-                f"got arguments with ranks {ar} and {br}.")
+                f"got arguments with ranks {ar} and {br}."
+            )
         if not (scalar or ash[-1] == bsh[0]):
             raise ValueError("Dimension mismatch in dot product.")
 
         # Simplification
         if isinstance(a, Zero) or isinstance(b, Zero):
             shape = ash[:-1] + bsh[1:]
             fi, fid = merge_nonoverlapping_indices(a, b)
@@ -232,16 +236,15 @@
     @property
     def ufl_shape(self):
         """Get the UFL shape."""
         return self.ufl_operands[0].ufl_shape[:-1] + self.ufl_operands[1].ufl_shape[1:]
 
     def __str__(self):
         """Format as a string."""
-        return "%s . %s" % (parstr(self.ufl_operands[0], self),
-                            parstr(self.ufl_operands[1], self))
+        return "%s . %s" % (parstr(self.ufl_operands[0], self), parstr(self.ufl_operands[1], self))
 
 
 @ufl_type(is_index_free=True, num_ops=1)
 class Perp(CompoundTensorOperator):
     """Perp."""
 
     __slots__ = ()
@@ -284,15 +287,16 @@
         ash = a.ufl_shape
         bsh = b.ufl_shape
 
         # Checks
         if not (len(ash) == 1 and ash == bsh):
             raise ValueError(
                 f"Cross product requires arguments of rank 1, got {ufl_err_str(a)} "
-                f"and {ufl_err_str(b)}.")
+                f"and {ufl_err_str(b)}."
+            )
 
         # Simplification
         if isinstance(a, Zero) or isinstance(b, Zero):
             fi, fid = merge_nonoverlapping_indices(a, b)
             return Zero(ash, fi, fid)
 
         return CompoundTensorOperator.__new__(cls)
@@ -304,16 +308,15 @@
         self.ufl_free_indices = fi
         self.ufl_index_dimensions = fid
 
     ufl_shape = (3,)
 
     def __str__(self):
         """Format as a string."""
-        return "%s x %s" % (parstr(self.ufl_operands[0], self),
-                            parstr(self.ufl_operands[1], self))
+        return "%s x %s" % (parstr(self.ufl_operands[0], self), parstr(self.ufl_operands[1], self))
 
 
 @ufl_type(num_ops=1, inherit_indices_from_operand=0)
 class Trace(CompoundTensorOperator):
     """Trace."""
 
     __slots__ = ()
@@ -464,15 +467,17 @@
         """Create new Deviatoric."""
         sh = A.ufl_shape
 
         # Checks
         if len(sh) != 2:
             raise ValueError("Deviatoric part of tensor with rank != 2 is undefined.")
         if sh[0] != sh[1]:
-            raise ValueError(f"Cannot take deviatoric part of rectangular matrix with dimensions {sh}.")
+            raise ValueError(
+                f"Cannot take deviatoric part of rectangular matrix with dimensions {sh}."
+            )
         if A.ufl_free_indices:
             raise ValueError("Not expecting free indices in Deviatoric.")
 
         # Simplification
         if isinstance(A, Zero):
             return Zero(A.ufl_shape, A.ufl_free_indices, A.ufl_index_dimensions)
 
@@ -532,15 +537,17 @@
         sh = A.ufl_shape
         Afi = A.ufl_free_indices
 
         # Checks
         if len(sh) != 2:
             raise ValueError("Symmetric part of tensor with rank != 2 is undefined.")
         if sh[0] != sh[1]:
-            raise ValueError(f"Cannot take symmetric part of rectangular matrix with dimensions {sh}.")
+            raise ValueError(
+                f"Cannot take symmetric part of rectangular matrix with dimensions {sh}."
+            )
         if Afi:
             raise ValueError("Not expecting free indices in Sym.")
 
         # Simplification
         if isinstance(A, Zero):
             return Zero(A.ufl_shape, Afi, A.ufl_index_dimensions)
```

### Comparing `fenics-ufl-2023.2.0/ufl/tensors.py` & `fenics_ufl-2024.1.0.post0/ufl/tensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Massimiliano Leoni, 2016.
 
-from ufl.core.ufl_type import ufl_type
+from ufl.constantvalue import Zero, as_ufl
 from ufl.core.expr import Expr
+from ufl.core.multiindex import FixedIndex, Index, MultiIndex, indices
 from ufl.core.operator import Operator
-from ufl.constantvalue import as_ufl, Zero
-from ufl.core.multiindex import Index, FixedIndex, MultiIndex, indices
-from ufl.indexed import Indexed
+from ufl.core.ufl_type import ufl_type
 from ufl.index_combination_utils import remove_indices
-
+from ufl.indexed import Indexed
 
 # --- Classes representing tensors of UFL expressions ---
 
+
 @ufl_type(is_shaping=True, num_ops="varying", inherit_indices_from_operand=0)
 class ListTensor(Operator):
     """Wraps a list of expressions into a tensor valued expression of one higher rank."""
 
     __slots__ = ()
 
     def __new__(cls, *expressions):
@@ -35,19 +35,25 @@
         e0 = expressions[0]
         sh = e0.ufl_shape
         fi = e0.ufl_free_indices
         fid = e0.ufl_index_dimensions
 
         # Obviously, each subexpression must have the same shape
         if any(sh != e.ufl_shape for e in expressions[1:]):
-            raise ValueError("Cannot create a tensor by joining subexpressions with different shapes.")
+            raise ValueError(
+                "Cannot create a tensor by joining subexpressions with different shapes."
+            )
         if any(fi != e.ufl_free_indices for e in expressions[1:]):
-            raise ValueError("Cannot create a tensor where the components have different free indices.")
+            raise ValueError(
+                "Cannot create a tensor where the components have different free indices."
+            )
         if any(fid != e.ufl_index_dimensions for e in expressions[1:]):
-            raise ValueError("Cannot create a tensor where the components have different free index dimensions.")
+            raise ValueError(
+                "Cannot create a tensor where the components have different free index dimensions."
+            )
 
         # Simplify to Zero if possible
         if all(isinstance(e, Zero) for e in expressions):
             shape = (len(expressions),) + sh
             return Zero(shape, fi, fid)
 
         return Operator.__new__(cls)
@@ -55,27 +61,30 @@
     def __init__(self, *expressions):
         """Initialise."""
         Operator.__init__(self, expressions)
 
         # Checks
         indexset = set(self.ufl_operands[0].ufl_free_indices)
         if not all(not (indexset ^ set(e.ufl_free_indices)) for e in self.ufl_operands):
-            raise ValueError("Can't combine subtensor expressions with different sets of free indices.")
+            raise ValueError(
+                "Can't combine subtensor expressions with different sets of free indices."
+            )
 
     @property
     def ufl_shape(self):
         """Get the UFL shape."""
         return (len(self.ufl_operands),) + self.ufl_operands[0].ufl_shape
 
     def evaluate(self, x, mapping, component, index_values, derivatives=()):
         """Evaluate."""
         if len(component) != len(self.ufl_shape):
             raise ValueError(
                 "Can only evaluate scalars, expecting a component "
-                "tuple of length {len(self.ufl_shape)}, not {component}.")
+                "tuple of length {len(self.ufl_shape)}, not {component}."
+            )
         a = self.ufl_operands[component[0]]
         component = component[1:]
         if derivatives:
             return a.evaluate(x, mapping, component, index_values, derivatives)
         else:
             return a.evaluate(x, mapping, component, index_values)
 
@@ -92,44 +101,48 @@
             sub = self.ufl_operands[int(k)]
             return sub if len(key) == 1 else sub[key[1:]]
 
         return Expr.__getitem__(self, origkey)
 
     def __str__(self):
         """Format as a string."""
+
         def substring(expressions, indent):
             ind = " " * indent
             if any(isinstance(e, ListTensor) for e in expressions):
                 substrings = []
                 for e in expressions:
                     if isinstance(e, ListTensor):
                         substrings.append(substring(e.ufl_operands, indent + 2))
                     else:
                         substrings.append(str(e))
                 s = (",\n" + ind).join(substrings)
                 return "%s[\n%s%s\n%s]" % (ind, ind, s, ind)
             else:
                 s = ", ".join(str(e) for e in expressions)
                 return "%s[%s]" % (ind, s)
+
         return substring(self.ufl_operands, 0)
 
 
 @ufl_type(is_shaping=True, num_ops="varying")
 class ComponentTensor(Operator):
     """Maps the free indices of a scalar valued expression to tensor axes."""
 
     __slots__ = ("ufl_shape", "ufl_free_indices", "ufl_index_dimensions")
 
     def __new__(cls, expression, indices):
         """Create a new ComponentTensor."""
         # Simplify
         if isinstance(expression, Zero):
-            fi, fid, sh = remove_indices(expression.ufl_free_indices,
-                                         expression.ufl_index_dimensions,
-                                         [ind.count() for ind in indices])
+            fi, fid, sh = remove_indices(
+                expression.ufl_free_indices,
+                expression.ufl_index_dimensions,
+                [ind.count() for ind in indices],
+            )
             return Zero(sh, fi, fid)
 
         # Construct
         return Operator.__new__(cls)
 
     def __init__(self, expression, indices):
         """Initialise."""
@@ -140,17 +153,19 @@
         if not isinstance(indices, MultiIndex):
             raise ValueError("Expecting a MultiIndex.")
         if not all(isinstance(i, Index) for i in indices):
             raise ValueError(f"Expecting sequence of Index objects, not {indices._ufl_err_str_()}.")
 
         Operator.__init__(self, (expression, indices))
 
-        fi, fid, sh = remove_indices(expression.ufl_free_indices,
-                                     expression.ufl_index_dimensions,
-                                     [ind.count() for ind in indices])
+        fi, fid, sh = remove_indices(
+            expression.ufl_free_indices,
+            expression.ufl_index_dimensions,
+            [ind.count() for ind in indices],
+        )
         self.ufl_free_indices = fi
         self.ufl_index_dimensions = fid
         self.ufl_shape = sh
 
     def _ufl_expr_reconstruct_(self, expressions, indices):
         """Reconstruct."""
         # Special case for simplification as_tensor(A[ii], ii) -> A
@@ -186,17 +201,19 @@
     def __str__(self):
         """Format as a string."""
         return "{ A | A_{%s} = %s }" % (self.ufl_operands[1], self.ufl_operands[0])
 
 
 # --- User-level functions to wrap expressions in the correct way ---
 
+
 def numpy2nestedlists(arr):
     """Convert Numpy array to a nested list."""
     from numpy import ndarray
+
     if not isinstance(arr, ndarray):
         return arr
     return [numpy2nestedlists(arr[k]) for k in range(arr.shape[0])]
 
 
 def _as_list_tensor(expressions):
     """Convert to a list tensor."""
@@ -206,16 +223,17 @@
     else:
         return as_ufl(expressions)
 
 
 def from_numpy_to_lists(expressions):
     """Convert Numpy array to lists."""
     try:
-        import numpy
-        if isinstance(expressions, numpy.ndarray):
+        import numpy as np
+
+        if isinstance(expressions, np.ndarray):
             if expressions.shape == ():
                 # Unwrap scalar ndarray
                 return expressions.item()
             else:
                 expressions = numpy2nestedlists(expressions)
     except Exception:
         pass
@@ -385,14 +403,15 @@
     return tuple(unit_matrix(i, j, d) for i in range(d) for j in range(d))
 
 
 def unit_indexed_tensor(shape, component):
     """Unit indexed tensor."""
     from ufl.constantvalue import Identity
     from ufl.operators import outer  # a bit of circular dependency issue here
+
     r = len(shape)
     if r == 0:
         return 0, ()
     jj = indices(r)
     es = []
     for i in range(r):
         s = shape[i]
```

### Comparing `fenics-ufl-2023.2.0/ufl/utils/counted.py` & `fenics_ufl-2024.1.0.post0/ufl/utils/counted.py`

 * *Files identical despite different names*

### Comparing `fenics-ufl-2023.2.0/ufl/utils/formatting.py` & `fenics_ufl-2024.1.0.post0/ufl/utils/formatting.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     lastlower = False
     for i in name:
         thislower = i.islower() or i.isdigit()
         if not thislower:
             # Don't insert _ between multiple upper case letters
             if lastlower:
                 letters.append("_")
-            i = i.lower()  # noqa: E741
+            i = i.lower()
         lastlower = thislower
         letters.append(i)
     return "".join(letters)
 
 
 def lstr(a):
     """Pretty-print list or tuple, invoking str() on items instead of repr() like str() does."""
@@ -41,15 +41,15 @@
 
     # Key-length cannot be larger than colsize
     if keylen > colsize:
         return str(t)
 
     # Pretty-print table
     s = ""
-    for (key, value) in t:
+    for key, value in t:
         key = str(key)
         if isinstance(value, str):
             value = "'%s'" % value
         else:
             value = str(value)
         s += key + ":" + " " * (keylen - len(key) + 1)
         space = ""
@@ -81,15 +81,18 @@
 
 def _tree_format_expression(expression, indentation, parentheses):
     """Tree format expression."""
     ind = _indent_string(indentation)
     if expression._ufl_is_terminal_:
         s = "%s%s" % (ind, repr(expression))
     else:
-        sops = [_tree_format_expression(o, indentation + 1, parentheses) for o in expression.ufl_operands]
+        sops = [
+            _tree_format_expression(o, indentation + 1, parentheses)
+            for o in expression.ufl_operands
+        ]
         s = "%s%s\n" % (ind, expression._ufl_class_.__name__)
         if parentheses and len(sops) > 1:
             s += "%s(\n" % (ind,)
         s += "\n".join(sops)
         if parentheses and len(sops) > 1:
             s += "\n%s)" % (ind,)
     return s
```

### Comparing `fenics-ufl-2023.2.0/ufl/utils/indexflattening.py` & `fenics_ufl-2024.1.0.post0/ufl/utils/indexflattening.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""This module contains a collection of utilities for mapping between multiindices and a flattened index space."""
+"""Collection of utilities for mapping between multiindices and a flattened index space."""
 
 # Copyright (C) 2008-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
```

### Comparing `fenics-ufl-2023.2.0/ufl/utils/sequences.py` & `fenics_ufl-2024.1.0.post0/ufl/utils/sequences.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 # Copyright (C) 2008-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
 from functools import reduce
-import numpy
+
+import numpy as np
 
 
 def product(sequence):
     """Return the product of all elements in a sequence."""
     p = 1
     for f in sequence:
         p *= f
     return p
 
 
 def max_degree(degrees):
     """Maximum degree for mixture of scalar and tuple degrees."""
-    # numpy.maximum broadcasts scalar degrees to tuple degrees if
-    # necessary.  reduce applies numpy.maximum pairwise.
-    degree = reduce(numpy.maximum, map(numpy.asarray, degrees))
+    # np.maximum broadcasts scalar degrees to tuple degrees if
+    # necessary.  reduce applies np.maximum pairwise.
+    degree = reduce(np.maximum, map(np.asarray, degrees))
     if degree.ndim:
         degree = tuple(map(int, degree))  # tuple degree
     else:
-        degree = int(degree)              # scalar degree
+        degree = int(degree)  # scalar degree
     return degree
```

### Comparing `fenics-ufl-2023.2.0/ufl/utils/sorting.py` & `fenics_ufl-2024.1.0.post0/ufl/utils/sorting.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     """
     L = []
     S = nodes[:]
     for node in nodes:
         for es in edges.values():
             if node in es and node in S:
                 S.remove(node)
-                continue
+                break
 
     while S:
         node = S.pop(0)
         L.append(node)
         node_edges = edges[node]
         while node_edges:
             m = node_edges.pop(0)
@@ -44,18 +44,20 @@
 def sorted_by_count(seq):
     """Sort a sequence by the item.count()."""
     return sorted(seq, key=lambda x: x.count())
 
 
 def sorted_by_key(mapping):
     """Sort dict items by key, allowing different key types."""
+
     # Python3 doesn't allow comparing builtins of different type,
     # therefore the typename trick here
     def _key(x):
         return (type(x[0]).__name__, x[0])
+
     return sorted(mapping.items(), key=_key)
 
 
 def canonicalize_metadata(metadata):
     """Assuming metadata to be a dict with string keys and builtin python types as values.
 
     Transform dict to a tuple of (key, value) item tuples ordered by key,
@@ -76,17 +78,21 @@
 
     newvalues = []
     for value in values:
         if isinstance(value, (dict, list, tuple)):
             value = canonicalize_metadata(value)
         elif isinstance(value, (int, float, str)) or value is None:
             value = str(value)
+        elif hasattr(value, "ufl_signature"):
+            value = value.ufl_signature
         else:
-            warnings.warn(f"Applying str() to a metadata value of type {type(value).__name__}, "
-                          "don't know if this is safe.")
+            warnings.warn(
+                f"Applying str() to a metadata value of type {type(value).__name__}, "
+                "don't know if this is safe."
+            )
             value = str(value)
         newvalues.append(value)
 
     if isinstance(metadata, dict):
         return tuple(zip(keys, newvalues))
     else:
         return tuple(newvalues)
```

### Comparing `fenics-ufl-2023.2.0/ufl/utils/stacks.py` & `fenics_ufl-2024.1.0.post0/ufl/utils/stacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,19 @@
 
     def peek(self):
         """Peek."""
         return self[-1]
 
 
 class StackDict(dict):
-    """A dict that can be changed incrementally with 'd.push(k,v)' and have changes rolled back with 'k,v = d.pop()'."""
+    """A dictionary type.
+
+    A dict that can be changed incrementally with 'd.push(k,v)' and have
+    changes rolled back with 'k,v = d.pop()'.
+    """
 
     def __init__(self, *args, **kwargs):
         """Initialise."""
         dict.__init__(self, *args, **kwargs)
         self._l = []
 
     def push(self, k, v):
```

### Comparing `fenics-ufl-2023.2.0/ufl/variable.py` & `fenics_ufl-2024.1.0.post0/ufl/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 """
 # Copyright (C) 2008-2016 Martin Sandve Alnæs
 #
 # This file is part of UFL (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
-from ufl.utils.counted import Counted
+from ufl.constantvalue import as_ufl
 from ufl.core.expr import Expr
-from ufl.core.ufl_type import ufl_type
-from ufl.core.terminal import Terminal
 from ufl.core.operator import Operator
-from ufl.constantvalue import as_ufl
+from ufl.core.terminal import Terminal
+from ufl.core.ufl_type import ufl_type
+from ufl.utils.counted import Counted
 
 
 @ufl_type()
 class Label(Terminal, Counted):
     """Label."""
 
     __slots__ = ("_count", "_counted_class")
@@ -114,14 +114,16 @@
 
     def label(self):
         """Get label."""
         return self.ufl_operands[1]
 
     def __eq__(self, other):
         """Check equality."""
-        return (isinstance(other, Variable) and self.ufl_operands[1] == other.ufl_operands[1] and  # noqa: W504
-                self.ufl_operands[0] == other.ufl_operands[0])
+        return (
+            isinstance(other, Variable)
+            and self.ufl_operands[1] == other.ufl_operands[1]
+            and self.ufl_operands[0] == other.ufl_operands[0]
+        )
 
     def __str__(self):
         """Format as a string."""
-        return "var%d(%s)" % (self.ufl_operands[1].count(),
-                              self.ufl_operands[0])
+        return "var%d(%s)" % (self.ufl_operands[1].count(), self.ufl_operands[0])
```


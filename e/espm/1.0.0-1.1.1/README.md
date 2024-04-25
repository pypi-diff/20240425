# Comparing `tmp/espm-1.0.0.tar.gz` & `tmp/espm-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espm-1.0.0.tar", last modified: Fri Apr 21 13:25:03 2023, max compression
+gzip compressed data, was "espm-1.1.1.tar", last modified: Thu Apr 25 14:31:01 2024, max compression
```

## Comparing `espm-1.0.0.tar` & `espm-1.1.1.tar`

### file list

```diff
@@ -1,117 +1,107 @@
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 13:25:03.712099 espm-1.0.0/
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 13:25:03.692611 espm-1.0.0/.github/
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 13:25:03.695285 espm-1.0.0/.github/workflows/
--rw-r--r--   0 nati       (501) staff       (20)      870 2023-04-21 08:29:28.000000 espm-1.0.0/.github/workflows/doc.yml
--rw-r--r--   0 nati       (501) staff       (20)     1117 2023-04-21 08:28:14.000000 espm-1.0.0/.github/workflows/python.yml
--rw-r--r--   0 nati       (501) staff       (20)      178 2023-02-21 16:38:53.000000 espm-1.0.0/.readthedocs.yml
--rw-r--r--   0 nati       (501) staff       (20)      862 2023-04-21 12:47:30.000000 espm-1.0.0/CHANGELOG.rst
--rw-r--r--   0 nati       (501) staff       (20)     4300 2023-04-21 13:12:38.000000 espm-1.0.0/CONTRIBUTING.rst
--rw-r--r--   0 nati       (501) staff       (20)     1083 2022-12-06 13:16:22.000000 espm-1.0.0/Licence.txt
--rw-r--r--   0 nati       (501) staff       (20)      429 2023-04-21 13:24:50.000000 espm-1.0.0/MANIFEST.in
--rw-r--r--   0 nati       (501) staff       (20)     3348 2023-04-21 13:25:03.711441 espm-1.0.0/PKG-INFO
--rw-r--r--   0 nati       (501) staff       (20)     2311 2023-04-21 12:10:18.000000 espm-1.0.0/README.rst
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 13:25:03.695903 espm-1.0.0/doc/
--rw-r--r--   0 nati       (501) staff       (20)       30 2020-12-17 09:02:04.000000 espm-1.0.0/doc/changelog.rst
--rw-r--r--   0 nati       (501) staff       (20)     1994 2023-04-21 12:43:34.000000 espm-1.0.0/doc/conf.py
--rw-r--r--   0 nati       (501) staff       (20)       33 2019-04-30 16:36:26.000000 espm-1.0.0/doc/contributing.rst
--rw-r--r--   0 nati       (501) staff       (20)      213 2023-02-23 09:10:02.000000 espm-1.0.0/doc/index.rst
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 13:25:03.696023 espm-1.0.0/doc/introduction/
--rw-r--r--   0 nati       (501) staff       (20)     6066 2023-04-21 12:44:57.000000 espm-1.0.0/doc/introduction/index.rst
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 13:25:03.696955 espm-1.0.0/doc/reference/
--rw-r--r--   0 nati       (501) staff       (20)      220 2023-04-20 12:35:31.000000 espm-1.0.0/doc/reference/datasets.rst
--rw-r--r--   0 nati       (501) staff       (20)      202 2023-02-21 16:38:50.000000 espm-1.0.0/doc/reference/estimators.rst
--rw-r--r--   0 nati       (501) staff       (20)      156 2023-04-20 12:35:31.000000 espm-1.0.0/doc/reference/index.rst
--rw-r--r--   0 nati       (501) staff       (20)       58 2023-02-21 16:38:50.000000 espm-1.0.0/doc/reference/measures.rst
--rw-r--r--   0 nati       (501) staff       (20)      257 2023-04-20 12:35:31.000000 espm-1.0.0/doc/reference/models.rst
--rw-r--r--   0 nati       (501) staff       (20)       70 2023-04-20 12:35:31.000000 espm-1.0.0/doc/reference/table_utils.rst
--rw-r--r--   0 nati       (501) staff       (20)       45 2023-02-21 16:38:50.000000 espm-1.0.0/doc/reference/utils.rst
--rw-r--r--   0 nati       (501) staff       (20)      140 2023-04-20 12:35:31.000000 espm-1.0.0/doc/reference/weights.rst
--rw-r--r--   0 nati       (501) staff       (20)       95 2019-04-30 16:36:26.000000 espm-1.0.0/doc/references.rst
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 13:25:03.697071 espm-1.0.0/doc/styles/
--rw-r--r--   0 nati       (501) staff       (20)      332 2023-02-20 15:43:46.000000 espm-1.0.0/doc/styles/sg_gallery.css
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 13:25:03.697945 espm-1.0.0/espm/
--rw-r--r--   0 nati       (501) staff       (20)       21 2023-04-21 12:46:08.000000 espm-1.0.0/espm/__init__.py
--rw-r--r--   0 nati       (501) staff       (20)     1385 2023-04-20 12:35:31.000000 espm-1.0.0/espm/conf.py
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 13:25:03.699188 espm-1.0.0/espm/datasets/
--rw-r--r--   0 nati       (501) staff       (20)     1026 2023-04-20 12:35:31.000000 espm-1.0.0/espm/datasets/__init__.py
--rw-r--r--   0 nati       (501) staff       (20)     9637 2023-04-20 13:46:14.000000 espm-1.0.0/espm/datasets/base.py
--rw-r--r--   0 nati       (501) staff       (20)     5756 2023-04-21 12:10:18.000000 espm-1.0.0/espm/datasets/built_in_EDXS_datasets.py
--rw-r--r--   0 nati       (501) staff       (20)    19888 2023-04-20 14:51:57.000000 espm-1.0.0/espm/datasets/eds_spim.py
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 13:25:03.699452 espm-1.0.0/espm/datasets/toy-problem/
--rw-r--r--   0 nati       (501) staff       (20)     4316 2023-02-21 16:38:50.000000 espm-1.0.0/espm/datasets/toy-problem/phase1.png
--rw-r--r--   0 nati       (501) staff       (20)     6798 2023-02-21 16:38:50.000000 espm-1.0.0/espm/datasets/toy-problem/phase2.png
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 13:25:03.700146 espm-1.0.0/espm/estimators/
--rw-r--r--   0 nati       (501) staff       (20)      529 2023-02-23 09:58:20.000000 espm-1.0.0/espm/estimators/__init__.py
--rw-r--r--   0 nati       (501) staff       (20)    19415 2023-02-23 13:48:32.000000 espm-1.0.0/espm/estimators/base.py
--rw-r--r--   0 nati       (501) staff       (20)     6026 2023-02-23 09:58:20.000000 espm-1.0.0/espm/estimators/dicotomy.py
--rw-r--r--   0 nati       (501) staff       (20)    10252 2023-04-21 12:10:18.000000 espm-1.0.0/espm/estimators/smooth_nmf.py
--rw-r--r--   0 nati       (501) staff       (20)     5700 2023-02-23 09:58:20.000000 espm-1.0.0/espm/estimators/surrogates.py
--rw-r--r--   0 nati       (501) staff       (20)    11222 2023-02-23 09:58:20.000000 espm-1.0.0/espm/estimators/updates.py
--rwxr-xr-x   0 nati       (501) staff       (20)      143 2023-04-18 07:43:05.000000 espm-1.0.0/espm/hyperspy_extension.yaml
--rw-r--r--   0 nati       (501) staff       (20)    20639 2023-04-20 13:24:00.000000 espm-1.0.0/espm/measures.py
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 13:25:03.700905 espm-1.0.0/espm/models/
--rw-r--r--   0 nati       (501) staff       (20)    13015 2023-04-20 12:35:31.000000 espm-1.0.0/espm/models/EDXS_function.py
--rw-r--r--   0 nati       (501) staff       (20)      500 2023-04-20 12:35:31.000000 espm-1.0.0/espm/models/__init__.py
--rw-r--r--   0 nati       (501) staff       (20)    10090 2023-04-20 12:35:31.000000 espm-1.0.0/espm/models/absorption_edxs.py
--rw-r--r--   0 nati       (501) staff       (20)     5682 2023-04-20 13:36:07.000000 espm-1.0.0/espm/models/base.py
--rw-r--r--   0 nati       (501) staff       (20)    17112 2023-04-20 12:53:51.000000 espm-1.0.0/espm/models/edxs.py
--rw-r--r--   0 nati       (501) staff       (20)     6598 2023-04-20 13:17:58.000000 espm-1.0.0/espm/models/generate_EDXS_phases.py
--rw-r--r--   0 nati       (501) staff       (20)     3130 2023-02-23 09:58:20.000000 espm-1.0.0/espm/spectrum_fitting.py
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 13:25:03.703852 espm-1.0.0/espm/tables/
--rw-r--r--   0 nati       (501) staff       (20)   299008 2023-02-21 16:38:50.000000 espm-1.0.0/espm/tables/100keV_xrays.json
--rw-r--r--   0 nati       (501) staff       (20)   288577 2023-02-21 16:38:50.000000 espm-1.0.0/espm/tables/200keV_xrays.json
--rw-r--r--   0 nati       (501) staff       (20)   282569 2023-02-21 16:38:50.000000 espm-1.0.0/espm/tables/300keV_xrays.json
--rw-r--r--   0 nati       (501) staff       (20)     6242 2023-02-21 16:38:50.000000 espm-1.0.0/espm/tables/SDD_efficiency.txt
--rw-r--r--   0 nati       (501) staff       (20)        0 2023-02-21 16:38:50.000000 espm-1.0.0/espm/tables/__init__.py
--rw-r--r--   0 nati       (501) staff       (20)   166571 2023-02-21 16:38:50.000000 espm-1.0.0/espm/tables/default_xrays.json
--rw-r--r--   0 nati       (501) staff       (20)    11811 2023-02-21 16:38:50.000000 espm-1.0.0/espm/tables/periodic_table_number.json
--rw-r--r--   0 nati       (501) staff       (20)    11616 2023-02-21 16:38:50.000000 espm-1.0.0/espm/tables/periodic_table_symbols.json
--rw-r--r--   0 nati       (501) staff       (20)      779 2023-02-21 16:38:50.000000 espm-1.0.0/espm/tables/siegbahn_to_iupac.json
--rw-r--r--   0 nati       (501) staff       (20)     7514 2023-04-20 12:53:51.000000 espm-1.0.0/espm/tables_utils.py
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 13:25:03.704913 espm-1.0.0/espm/tests/
--rw-r--r--   0 nati       (501) staff       (20)        0 2023-02-21 16:38:50.000000 espm-1.0.0/espm/tests/__init__.py
--rw-r--r--   0 nati       (501) staff       (20)     4910 2023-04-18 07:43:05.000000 espm-1.0.0/espm/tests/test_EDXS.py
--rw-r--r--   0 nati       (501) staff       (20)    11339 2023-04-18 07:43:05.000000 espm-1.0.0/espm/tests/test_datasets.py
--rw-r--r--   0 nati       (501) staff       (20)     1073 2023-02-23 09:58:20.000000 espm-1.0.0/espm/tests/test_docstring.py
--rw-r--r--   0 nati       (501) staff       (20)     9592 2023-04-20 14:57:35.000000 espm-1.0.0/espm/tests/test_estimators.py
--rw-r--r--   0 nati       (501) staff       (20)     1263 2023-02-23 09:58:20.000000 espm-1.0.0/espm/tests/test_laplacian.py
--rw-r--r--   0 nati       (501) staff       (20)     7634 2023-02-23 09:58:20.000000 espm-1.0.0/espm/tests/test_measures.py
--rw-r--r--   0 nati       (501) staff       (20)    29130 2023-02-23 09:58:20.000000 espm-1.0.0/espm/tests/test_updates.py
--rw-r--r--   0 nati       (501) staff       (20)     3652 2023-02-23 09:58:20.000000 espm-1.0.0/espm/tests/test_utils.py
--rw-r--r--   0 nati       (501) staff       (20)    11669 2023-04-20 12:53:51.000000 espm-1.0.0/espm/utils.py
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 13:25:03.705304 espm-1.0.0/espm/weights/
--rw-r--r--   0 nati       (501) staff       (20)      258 2023-04-20 12:53:51.000000 espm-1.0.0/espm/weights/__init__.py
--rw-r--r--   0 nati       (501) staff       (20)    16957 2023-04-20 13:14:42.000000 espm-1.0.0/espm/weights/abundance.py
--rw-r--r--   0 nati       (501) staff       (20)    11055 2023-04-20 12:53:51.000000 espm-1.0.0/espm/weights/generate_weights.py
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 13:25:03.698741 espm-1.0.0/espm.egg-info/
--rw-r--r--   0 nati       (501) staff       (20)     3348 2023-04-21 13:25:03.000000 espm-1.0.0/espm.egg-info/PKG-INFO
--rw-r--r--   0 nati       (501) staff       (20)     2515 2023-04-21 13:25:03.000000 espm-1.0.0/espm.egg-info/SOURCES.txt
--rw-r--r--   0 nati       (501) staff       (20)        1 2023-04-21 13:25:03.000000 espm-1.0.0/espm.egg-info/dependency_links.txt
--rw-r--r--   0 nati       (501) staff       (20)       34 2023-04-21 13:25:03.000000 espm-1.0.0/espm.egg-info/entry_points.txt
--rw-r--r--   0 nati       (501) staff       (20)        1 2023-04-21 13:25:03.000000 espm-1.0.0/espm.egg-info/not-zip-safe
--rw-r--r--   0 nati       (501) staff       (20)      207 2023-04-21 13:25:03.000000 espm-1.0.0/espm.egg-info/requires.txt
--rw-r--r--   0 nati       (501) staff       (20)        5 2023-04-21 13:25:03.000000 espm-1.0.0/espm.egg-info/top_level.txt
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 13:25:03.705426 espm-1.0.0/generated_datasets/
--rw-r--r--   0 nati       (501) staff       (20)  4826704 2023-04-21 08:22:51.000000 espm-1.0.0/generated_datasets/71GPa_experimental_data.hspy
--rwxr-xr-x   0 nati       (501) staff       (20)      143 2023-04-18 07:43:05.000000 espm-1.0.0/hyperspy_extension.yaml
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 13:25:03.711060 espm-1.0.0/notebooks/
--rw-r--r--   0 nati       (501) staff       (20)     4963 2023-02-23 09:58:20.000000 espm-1.0.0/notebooks/VCA.py
--rw-r--r--   0 nati       (501) staff       (20)     5382 2023-04-21 13:25:01.000000 espm-1.0.0/notebooks/api.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    17775 2023-04-21 13:25:01.000000 espm-1.0.0/notebooks/background_fit.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    13661 2023-04-21 13:25:02.000000 espm-1.0.0/notebooks/convergence-speed.ipynb
--rw-r--r--   0 nati       (501) staff       (20)     8875 2023-04-21 13:25:02.000000 espm-1.0.0/notebooks/generate_data.ipynb
--rw-r--r--   0 nati       (501) staff       (20)     3204 2023-04-21 13:25:02.000000 espm-1.0.0/notebooks/make-plots.ipynb
-drwxr-xr-x   0 nati       (501) staff       (20)        0 2023-04-21 13:25:03.711210 espm-1.0.0/notebooks/old/
--rw-r--r--   0 nati       (501) staff       (20)     6289 2022-02-25 16:24:57.000000 espm-1.0.0/notebooks/old/algo-with-negative-variable.ipynb
--rw-r--r--   0 nati       (501) staff       (20)     6820 2023-04-21 13:25:02.000000 espm-1.0.0/notebooks/other_algorithms.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    17002 2023-04-21 13:25:02.000000 espm-1.0.0/notebooks/preprocess_dataset.ipynb
--rw-r--r--   0 nati       (501) staff       (20)     4531 2023-04-21 13:25:02.000000 espm-1.0.0/notebooks/select_spectrum.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    14791 2023-04-21 13:25:02.000000 espm-1.0.0/notebooks/simple-test-regularisation.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    31459 2023-04-21 13:25:03.000000 espm-1.0.0/notebooks/spectrum_fit.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    13889 2023-02-23 09:58:20.000000 espm-1.0.0/notebooks/sunsal.py
--rw-r--r--   0 nati       (501) staff       (20)     7554 2023-04-21 13:25:03.000000 espm-1.0.0/notebooks/surrogate-vs-bregmann.ipynb
--rw-r--r--   0 nati       (501) staff       (20)    18737 2023-04-21 13:25:03.000000 espm-1.0.0/notebooks/toy-ML.ipynb
--rw-r--r--   0 nati       (501) staff       (20)      178 2022-12-06 17:40:13.000000 espm-1.0.0/readthedoc.yml
--rw-r--r--   0 nati       (501) staff       (20)       38 2023-04-21 13:25:03.712159 espm-1.0.0/setup.cfg
--rw-r--r--   0 nati       (501) staff       (20)     1800 2023-04-21 12:45:54.000000 espm-1.0.0/setup.py
--rw-r--r--   0 nati       (501) staff       (20)      218 2023-04-21 12:51:02.000000 espm-1.0.0/todo.md
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2024-04-25 14:31:01.811857 espm-1.1.1/
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2024-04-25 14:31:01.799857 espm-1.1.1/.github/
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2024-04-25 14:31:01.803857 espm-1.1.1/.github/workflows/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      870 2023-06-21 09:55:53.000000 espm-1.1.1/.github/workflows/doc.yml
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1118 2024-04-19 12:27:20.000000 espm-1.1.1/.github/workflows/python.yml
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      213 2023-09-25 08:19:47.000000 espm-1.1.1/.readthedocs.yaml
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     3074 2024-04-25 14:01:25.000000 espm-1.1.1/CHANGELOG.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     4300 2023-06-21 09:55:53.000000 espm-1.1.1/CONTRIBUTING.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1083 2023-06-21 09:55:53.000000 espm-1.1.1/Licence.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      429 2023-06-21 09:55:53.000000 espm-1.1.1/MANIFEST.in
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     4748 2024-04-25 14:31:01.811857 espm-1.1.1/PKG-INFO
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     2898 2024-04-25 14:03:09.000000 espm-1.1.1/README.rst
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2024-04-25 14:31:01.803857 espm-1.1.1/doc/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)       30 2023-06-21 09:55:53.000000 espm-1.1.1/doc/changelog.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1994 2023-06-21 09:55:53.000000 espm-1.1.1/doc/conf.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)       33 2023-06-21 09:55:53.000000 espm-1.1.1/doc/contributing.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      213 2023-06-21 09:55:53.000000 espm-1.1.1/doc/index.rst
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2024-04-25 14:31:01.803857 espm-1.1.1/doc/introduction/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     6997 2024-04-23 15:37:57.000000 espm-1.1.1/doc/introduction/index.rst
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2024-04-25 14:31:01.803857 espm-1.1.1/doc/reference/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      220 2023-06-21 09:55:53.000000 espm-1.1.1/doc/reference/datasets.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      202 2023-06-21 09:55:53.000000 espm-1.1.1/doc/reference/estimators.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      156 2023-06-21 09:55:53.000000 espm-1.1.1/doc/reference/index.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)       58 2023-06-21 09:55:53.000000 espm-1.1.1/doc/reference/measures.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      257 2023-06-21 09:55:53.000000 espm-1.1.1/doc/reference/models.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)       70 2023-06-21 09:55:53.000000 espm-1.1.1/doc/reference/table_utils.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)       45 2023-06-21 09:55:53.000000 espm-1.1.1/doc/reference/utils.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      140 2023-06-21 09:55:53.000000 espm-1.1.1/doc/reference/weights.rst
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)       95 2023-06-21 09:55:53.000000 espm-1.1.1/doc/references.rst
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2024-04-25 14:31:01.803857 espm-1.1.1/doc/styles/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      332 2023-06-21 09:55:53.000000 espm-1.1.1/doc/styles/sg_gallery.css
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2024-04-25 14:31:01.803857 espm-1.1.1/espm/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)       21 2024-04-25 14:03:18.000000 espm-1.1.1/espm/__init__.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1429 2024-04-08 12:10:34.000000 espm-1.1.1/espm/conf.py
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2024-04-25 14:31:01.803857 espm-1.1.1/espm/datasets/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1026 2023-06-21 09:55:53.000000 espm-1.1.1/espm/datasets/__init__.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     9638 2023-06-21 09:55:53.000000 espm-1.1.1/espm/datasets/base.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     5761 2024-04-19 15:39:12.000000 espm-1.1.1/espm/datasets/built_in_EDXS_datasets.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    39492 2024-04-23 13:46:06.000000 espm-1.1.1/espm/datasets/eds_spim.py
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2024-04-25 14:31:01.803857 espm-1.1.1/espm/datasets/toy-problem/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     4316 2023-06-21 09:55:53.000000 espm-1.1.1/espm/datasets/toy-problem/phase1.png
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     6798 2023-06-21 09:55:53.000000 espm-1.1.1/espm/datasets/toy-problem/phase2.png
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2024-04-25 14:31:01.803857 espm-1.1.1/espm/estimators/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      529 2023-06-21 09:55:53.000000 espm-1.1.1/espm/estimators/__init__.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    21262 2024-04-19 15:23:54.000000 espm-1.1.1/espm/estimators/base.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     6026 2023-09-26 15:23:36.000000 espm-1.1.1/espm/estimators/dicotomy.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    16020 2024-04-19 08:23:43.000000 espm-1.1.1/espm/estimators/smooth_nmf.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     5710 2024-03-22 12:33:27.000000 espm-1.1.1/espm/estimators/surrogates.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    14192 2024-04-19 15:27:55.000000 espm-1.1.1/espm/estimators/updates.py
+-rwxrwxr-x   0 adrien    (1000) adrien    (1000)      143 2023-06-21 09:55:53.000000 espm-1.1.1/espm/hyperspy_extension.yaml
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    20639 2023-06-21 09:55:53.000000 espm-1.1.1/espm/measures.py
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2024-04-25 14:31:01.803857 espm-1.1.1/espm/models/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    12278 2024-04-04 16:26:51.000000 espm-1.1.1/espm/models/EDXS_function.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      500 2023-06-21 09:55:53.000000 espm-1.1.1/espm/models/__init__.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    10090 2024-04-04 16:26:59.000000 espm-1.1.1/espm/models/absorption_edxs.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     7383 2024-04-17 17:40:45.000000 espm-1.1.1/espm/models/base.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    18361 2024-04-19 15:55:36.000000 espm-1.1.1/espm/models/edxs.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     6598 2023-06-21 09:55:53.000000 espm-1.1.1/espm/models/generate_EDXS_phases.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     3144 2024-04-04 13:21:41.000000 espm-1.1.1/espm/spectrum_fitting.py
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2024-04-25 14:31:01.803857 espm-1.1.1/espm/tables/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)   299008 2023-06-21 09:55:53.000000 espm-1.1.1/espm/tables/100keV_xrays.json
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)   288577 2023-06-21 09:55:53.000000 espm-1.1.1/espm/tables/200keV_xrays.json
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)   282569 2023-06-21 09:55:53.000000 espm-1.1.1/espm/tables/300keV_xrays.json
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     6242 2023-06-21 09:55:53.000000 espm-1.1.1/espm/tables/SDD_efficiency.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)        0 2023-06-21 09:55:53.000000 espm-1.1.1/espm/tables/__init__.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)   166571 2023-06-21 09:55:53.000000 espm-1.1.1/espm/tables/default_xrays.json
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    11811 2023-06-21 09:55:53.000000 espm-1.1.1/espm/tables/periodic_table_number.json
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    11616 2023-06-21 09:55:53.000000 espm-1.1.1/espm/tables/periodic_table_symbols.json
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      779 2023-06-21 09:55:53.000000 espm-1.1.1/espm/tables/siegbahn_to_iupac.json
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     7514 2023-06-21 09:55:53.000000 espm-1.1.1/espm/tables_utils.py
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2024-04-25 14:31:01.807857 espm-1.1.1/espm/tests/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)        0 2023-06-21 09:55:53.000000 espm-1.1.1/espm/tests/__init__.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     7305 2024-04-23 13:56:31.000000 espm-1.1.1/espm/tests/test_EDXS.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    16558 2024-04-23 15:03:39.000000 espm-1.1.1/espm/tests/test_datasets.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1073 2023-06-21 09:55:53.000000 espm-1.1.1/espm/tests/test_docstring.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    10706 2024-04-23 14:10:04.000000 espm-1.1.1/espm/tests/test_estimators.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1263 2023-06-21 09:55:53.000000 espm-1.1.1/espm/tests/test_laplacian.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     7634 2023-06-21 09:55:53.000000 espm-1.1.1/espm/tests/test_measures.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    29156 2024-03-22 12:33:27.000000 espm-1.1.1/espm/tests/test_updates.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     3649 2024-04-18 16:12:18.000000 espm-1.1.1/espm/tests/test_utils.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    12757 2024-04-22 16:51:07.000000 espm-1.1.1/espm/utils.py
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2024-04-25 14:31:01.807857 espm-1.1.1/espm/weights/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      258 2023-06-21 09:55:53.000000 espm-1.1.1/espm/weights/__init__.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    16919 2024-04-17 15:36:33.000000 espm-1.1.1/espm/weights/abundance.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    11059 2023-10-04 12:57:31.000000 espm-1.1.1/espm/weights/generate_weights.py
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2024-04-25 14:31:01.803857 espm-1.1.1/espm.egg-info/
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     4748 2024-04-25 14:31:01.000000 espm-1.1.1/espm.egg-info/PKG-INFO
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     2235 2024-04-25 14:31:01.000000 espm-1.1.1/espm.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)        1 2024-04-25 14:31:01.000000 espm-1.1.1/espm.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)       34 2024-04-25 14:31:01.000000 espm-1.1.1/espm.egg-info/entry_points.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)        1 2024-04-25 14:31:01.000000 espm-1.1.1/espm.egg-info/not-zip-safe
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      233 2024-04-25 14:31:01.000000 espm-1.1.1/espm.egg-info/requires.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)        5 2024-04-25 14:31:01.000000 espm-1.1.1/espm.egg-info/top_level.txt
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2024-04-25 14:31:01.807857 espm-1.1.1/generated_datasets/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)  4826704 2023-06-21 09:55:53.000000 espm-1.1.1/generated_datasets/71GPa_experimental_data.hspy
+-rwxrwxr-x   0 adrien    (1000) adrien    (1000)      143 2023-06-21 09:55:53.000000 espm-1.1.1/hyperspy_extension.yaml
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2024-04-25 14:31:01.807857 espm-1.1.1/notebooks/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     5531 2024-04-25 14:31:00.000000 espm-1.1.1/notebooks/api.ipynb
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    13854 2024-04-25 14:31:01.000000 espm-1.1.1/notebooks/background_fit.ipynb
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    10998 2024-04-25 14:31:01.000000 espm-1.1.1/notebooks/convergence-speed.ipynb
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    10900 2024-04-19 09:29:49.000000 espm-1.1.1/notebooks/convergence.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     8875 2024-04-25 14:31:01.000000 espm-1.1.1/notebooks/generate_data.ipynb
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    42579 2024-04-25 14:31:01.000000 espm-1.1.1/notebooks/papers_figures.ipynb
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    18941 2024-04-25 14:31:01.000000 espm-1.1.1/notebooks/toy-ML.ipynb
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)       38 2024-04-25 14:31:01.811857 espm-1.1.1/setup.cfg
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1979 2024-04-25 14:01:36.000000 espm-1.1.1/setup.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      326 2024-04-19 14:13:13.000000 espm-1.1.1/todo.md
```

### Comparing `espm-1.0.0/.github/workflows/doc.yml` & `espm-1.1.1/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/.github/workflows/python.yml` & `espm-1.1.1/.github/workflows/python.yml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 on: [push]
 jobs:
   build:
     runs-on: ubuntu-latest
     timeout-minutes: 60
     strategy:
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10']
+        python-version: ['3.8', '3.9', '3.10', '3.11']
         # python-version: ['3.10']
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v1
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `espm-1.0.0/CONTRIBUTING.rst` & `espm-1.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/Licence.txt` & `espm-1.1.1/Licence.txt`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/README.rst` & `espm-1.1.1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 espm: The Electron Spectro-Microscopy Python Library
 =====================================================
 
 .. image:: https://readthedocs.org/projects/espm/badge/?version=latest
     :target: https://espm.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
+The espm package is designed for simulation and physics-guided NMF decomposition of hyperspectral data.
+Even though the package is mainly centered around electron spectro-microscopy applications, custom models can be implemented for other type of data.
+Currently espm supports the simulation and analysis of simultaneous scanning transmission electron microscopy and energy dispersive X-ray spectroscopy (STEM / EDXS). 
+In future implementation, we will try to extend the package to support electron energy loss spectroscopy (EELS).
 
-The espm package is designed for the simulation and analysis of scanning transmission electron microscopy (STEM) hyperspectral data analysis. 
-Currently it only supports energy dispersive X-ray spectroscopy (EDXS) data but we will try to extend it to electron energy loss spectroscopy (EELS) data in the future.
 The main components of the package are:
 - The simulation of STEM-EDXS datasets using :mod:`espm.datasets` which combines :mod:`espm.weights` for the simulation of spatial distributions and :mod:`èspm.models` for the simulation of spectra.
 - The hyperspectral unmixing of STEM-EDXS spectrum images using :mod:`espm.estimators`. This module contains algorithms to perform non-negative matrix factorization with diverse regularisation (e.g. Laplacian or L1) and contraints (e.g. simplex).
 - The :mod:`espm.models` module can also be used to perform a physics-guided decomposition of STEM-EDXS datasets.
 
 Installation
 ------------
@@ -21,30 +23,39 @@
     $ pip install espm
 
 If you want to develop, please use the option::
 
     $ git clone https://github.com/adriente/espm.git
     $ cd espm
     $ pip install cython
-    $ pip install -e ".[dev]" 
+    $ pip install -e ."[dev]" 
+
+If you get issues regarding pandoc when using `make doc`, you can install it using::
+
+    $ sudo apt-get install pandoc
+
+or
+    
+    $ conda install pandoc
 
 Getting started
 ---------------
 Try the api.ipynb notebook in the `notebooks` folder.
 
 
 Documentation
 -------------
 
 The documentation is available at https://espm.readthedocs.io/en/latest/
 
 You can get started with the following notebooks:
 
-* https://espm.readthedocs.io/en/latest/introduction/notebooks/api.html
-* https://espm.readthedocs.io/en/latest/introduction/notebooks/toy-problem.html
+* Simulate STEM-EDXS data : https://espm.readthedocs.io/en/latest/introduction/notebooks/generate_data.ipynb
+* Physics-guided decomposition (ESpM-NMF) STEM-EDXS data : https://espm.readthedocs.io/en/latest/introduction/notebooks/api.html
+* Tests of the ESpM-NMF with a toy dataset : https://espm.readthedocs.io/en/latest/introduction/notebooks/toy-problem.html
 
 CITING
 ------
 
 If you use this library, please cite the following paper::
 
     @article{teurtrie2023espm,
```

### Comparing `espm-1.0.0/doc/conf.py` & `espm-1.1.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/doc/introduction/index.rst` & `espm-1.1.1/doc/introduction/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -80,32 +80,35 @@
     >>> spim.plot_decomposition_loadings(3)
     >>> spim.plot_decomposition_factors(3)
 
 Thanks to the physics-guided approach a direct quantification is possible.
 
 >>> spim.print_concentration_report()
 Concentrations report
-     p0     p1     p2
-V  : 0.0178 0.0061 0.0569 
-Rb : 0.5262 0.0609 0.3005 
-W  : 0.0379 0.0055 0.0326 
-N  : 0.0090 0.0913 0.0110 
-Yb : 0.0000 0.0901 0.0000 
-Pt : 0.0003 0.0179 0.0011 
-Al : 0.0000 0.1100 0.0000 
-Ti : 0.0000 0.0957 0.0000 
-La : 0.0000 0.2163 0.0000
++----------+-----------+-------------+-----------+------------+-----------+-------------+
+| Elements | p0 (at.%) |  p0 std (%) | p1 (at.%) | p1 std (%) | p2 (at.%) |  p2 std (%) |
++----------+-----------+-------------+-----------+------------+-----------+-------------+
+| V        |     4.277 |       0.815 |     0.345 |      5.236 |     0.000 |    5426.331 |
+| Rb       |    89.219 |       0.150 |     0.000 |   1217.568 |     0.000 |   10598.096 |
+| W        |     6.505 |       0.430 |     0.000 | 329274.377 |     0.000 |      93.434 |
+| N        |     0.000 | 3363320.886 |    52.263 |      0.848 |     0.000 |     423.423 |
+| Yb       |     0.000 | 1047375.510 |    38.941 |      0.306 |     0.000 | 1344821.409 |
+| Pt       |     0.000 | 1056115.710 |     8.450 |      0.663 |     0.000 |     172.134 |
+| Al       |     0.000 | 2353678.504 |     0.000 |    307.917 |    23.854 |       0.781 |
+| Ti       |     0.000 | 1773459.648 |     0.000 |    447.319 |    23.390 |       0.594 |
+| La       |     0.000 | 1510548.956 |     0.000 |  15734.933 |    52.756 |       0.337 |
++----------+-----------+-------------+-----------+------------+-----------+-------------+
 
 It uses algorithms that will be presented in a coming contribution.
 
 These algorithms are an important part of this package. They are specialized to solve regularized Poisson NMF problems. Mathematically, they can be expressed as:
 
 .. math::
     
-    \dot{W}, \dot{H} = \arg\min_{W\geq\epsilon, H\geq\epsilon, \sum_i H_{ij}  = 1} D_{GKL}(X || GWH) + \lambda tr ( H^\top \Delta H) + \mu \sum_{i,j} (\log H_{ij} +  \epsilon_{reg})$$
+    \dot{W}, \dot{H} = \arg\min_{W\geq\epsilon, H\geq\epsilon, \sum_i H_{ij}  = 1} D_{GKL}(X || GWH) + \lambda tr ( H^\top \Delta H) + \mu \sum_{i,j} (\log H_{ij} +  \epsilon_{reg})
 
 Here :math:`D_{GKL}` is the fidelity term, i.e. the Generalized KL divergence 
 
 .. math::
     
     D_{GKL}(X \| Y) = \sum_{i,j} X_{ij} \log \frac{X_{ij}}{Y_{ij}} - X_{ij} + Y_{ij}
 
@@ -124,19 +127,19 @@
 
 .. math:: 
     
     \mu \sum_{i,j} (\log H_{ij} +  \epsilon_{reg})
 
 where :math:`\epsilon_{reg}` is the slope of log regularization at 0. This term acts similarly to an L1 penalty but affects less larger values. 
 
-Finally, we assume :math:`W,H\geq \epsilon` and that the lines of :math:`H` sum to 1: 
+Finally, we assume :math:`W,H\geq \epsilon` and that the first :math:`M'` lines of :math:`W` sum to 1: 
 
 .. math:: 
     
-    \sum_i H_{ij}  = 1.
+    \sum_{i \leq M'} W_{ij}  = 1.
 
 The size of:
 
 - :math:`X` is `(n, p)`
 - :math:`W` is `(m, k)`
 - :math:`H` is `(k, p)`
 - :math:`G` is `(n, m)`
```

### Comparing `espm-1.0.0/espm/conf.py` & `espm-1.1.1/espm/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from pathlib import Path
-import hyperspy.misc.eds.ffast_mac as macs
+import exspy.misc.eds.ffast_mac as macs
+# from exspy.misc.eds import ffast_mac as macs
+HSPY_MAC = macs.ffast_mac # Tabulated absorption coefficient in Hyperspy
 
 # Path of the base
 BASE_PATH = Path(__file__).parent
 
 # Path of the db
 DB_PATH = BASE_PATH / Path("tables/")
 
@@ -17,15 +19,14 @@
 
 # Path of the generated datasets
 DATASETS_PATH = BASE_PATH.parent / Path("generated_datasets")
 # Ensure that the folder DATASETS_PATH exists
 DATASETS_PATH.mkdir(exist_ok=True, parents=True)
 
 
-HSPY_MAC = macs.ffast_mac # Tabulated absorption coefficient in Hyperspy
 
 DEFAULT_MISC_PARAMS = {
     "data_folder" : "default_synth_data",
     "shape_2d" : (80,80),
     "N" : 100,
     "densities" : [2.33,19.3],
     "model" : "EDXS",
```

### Comparing `espm-1.0.0/espm/datasets/__init__.py` & `espm-1.1.1/espm/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/espm/datasets/base.py` & `espm-1.1.1/espm/datasets/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
     sample["H"] = weights
     sample["H_flat"] = weights.reshape(-1, weights.shape[-1])
     sample["X"] = X
     sample["Xdot"] = Xdot
     sample["G"] = G
     return sample
 
-def generate_dataset(base_path = DATASETS_PATH, sample_number = 10, base_seed = 0, elements = [],*args, **kwargs): 
+def generate_dataset(*args, base_path = DATASETS_PATH, sample_number = 10, base_seed = 0, elements = [], **kwargs): 
     r"""
     Generate a set of spectrum images files and save them in the generated dataset folder. Each spectrum image is saved in a separate file and was generated using a different seed.
 
     Parameters
     ----------
     base_path : str, optional
         The path to the folder where the samples will be saved. The default is DATASETS_PATH.
```

### Comparing `espm-1.0.0/espm/datasets/built_in_EDXS_datasets.py` & `espm-1.1.1/espm/datasets/built_in_EDXS_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,20 @@
       '70': 0.39973013314240835,
       '78': 0.08298592142537742},
     {'13': 0.43306626599937914,
       '22': 0.3985896640183708,
       '57': 0.8994030840372912}
     ],
     'brstlg_pars' : [
-    {'b0': 7.408513360414626e-05,
-    'b1': 6.606903143185911e-03},
-    {'b0': 7.317975736931391e-05,
-      'b1': 5.2126092148294355e-03},
-    {'b0': 2.2664567599307173e-05,
-      'b1': 3.1627208027847766e-03}
+    {'b0': 11.408513360414626e-06,
+    'b1': 56.606903143185911e-04},
+    {'b0': 17.317975736931391e-06,
+      'b1': 15.2126092148294355e-04},
+    {'b0': 2.2664567599307173e-06,
+      'b1': 13.1627208027847766e-04}
     ],
     'scales' : [1,1,1],
     'model_params': {'e_offset': 0.2,
     'e_size': 1980,
     'e_scale': 0.01,
     'width_slope': 0.01,
     'width_intercept': 0.065,
```

### Comparing `espm-1.0.0/espm/datasets/eds_spim.py` & `espm-1.1.1/espm/models/edxs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,416 +1,383 @@
 r"""
-The module :mod:`espm.eds_spim` implements the :class:`EDS_espm` class, which is a subclass of the :class:`hyperspy.signals.Signal1D` class.
-The main purpose of this class is to provide an easy and clean interface between the hyperspy framework and the espm package: 
-- The metadata are organised to correspond as much as possible to the typical metadata that can be found in hyperspy EDS_TEM object.
-- The machine learning algorithms of espm can be easily applied to the :class:`EDS_espm` object using the standard hyperspy decomposition method. See the notebooks for examples.
-- The :class:`EDS_espm` provides a convinient way to:
-    - get the results of :class:`espm.estimators.NMFEstimator`
-    - access ground truth in case of simulated data
-    - set fixed W and H for the :class:`espm.estimators.NMFEstimator` decomposition
-"""
-
-from  hyperspy.signals import Signal1D
-from espm.models import EDXS
-from espm import models
-from espm.models.edxs import G_EDXS
-from hyperspy.misc.eds.utils import take_off_angle
-from espm.utils import number_to_symbol_list
-import numpy as np
-from espm.estimators import NMFEstimator
+EDXS model
+----------
 
+The :mod:`espm.models.edxs` module implements the creation of the G matrix that contains a modelisation of the characteristic and continuous X-rays.
 
-class EDS_espm(Signal1D) : 
+**This module is a key component of the EDXS data simulation and the EDXS data analysis.**
 
-    def __init__ (self,*args,**kwargs) : 
-        super().__init__(*args,**kwargs)
-        self.shape_2d_ = None
-        self._phases = None
-        self._maps = None
-        self._X = None
-        self._Xdot = None
-        self._maps_2d = None
-        self.G = None
-        self.model_ = None
+"""
 
-    @property
-    def shape_2d (self) : 
-        r"""
-        Shape of the data in the spatial dimension.
+import numpy as np
+import re
+from espm.models import PhysicalModel
+from espm.models.EDXS_function import G_bremsstrahlung, continuum_xrays, gaussian, read_lines_db, read_compact_db, elts_dict_from_dict_list
+from espm.conf import DEFAULT_EDXS_PARAMS
+from espm.utils import arg_helper, symbol_to_number_dict, symbol_to_number_list
+from espm.models.absorption_edxs import absorption_correction, det_efficiency, det_efficiency_from_curve, absorption_mass_thickness
+# Class to model the EDXS spectra. This is a temporary version since there are some design issues.
+
+
+class EDXS(PhysicalModel):
+    def __init__(
+        self, 
+        *args, 
+        width_slope=0.01,
+        width_intercept=0.065,
+        custom_init = False,
+        **kwargs
+    ):
+        r"""
+        :database_path: file path to a database of x-ray data (energy and intensity ratios of the peaks)
+        :abs_db_path: file path to a database of attenuation coefficients (Useful for artificial data only for the moment)
+        :brstlg_pars: dictionary of parameters for the continuum X-rays. Only a part of the parameters can be used without issues.
+        :e_offset: energy offset of the energy axis (float)
+        :e_size: number of energy channels (int)
+        :e_scale: ev/channel calibration of the energy axis (float)
+        :width_slope: The FWHM of the detector increases with energy which is modeled with an affine function. This is the slope of this affine function (float).
+        :width_intercept: The FWHM of the detector increases with energy which is modeled with an affine function. This is the intercept of this affine function (float).
         """
-        if self.shape_2d_ is None : 
-            self.shape_2d_ = self.axes_manager[1].size, self.axes_manager[0].size
-        return self.shape_2d_
-
-    @property
-    def X (self) :
+        super().__init__(*args,**kwargs)
+        self.width_slope = width_slope
+        self.width_intercept = width_intercept
+        
+        self.lines = self.db_mdata["lines"]
+        self.norm = 1.0
+        self.model_elts = []
+        self.custom_init = custom_init
+
+    def __add_elts_G(self, reference_elt = {}, *, elements=[]):
+        for elt in elements:
+            if self.lines : 
+                energies, cs = read_lines_db(elt,self.db_dict)
+            else : 
+                energies, cs = read_compact_db(elt,self.db_dict)
+            if elt in reference_elt : 
+                peaks_low = np.zeros((self.x.shape[0], 1))
+                peaks_high = np.zeros((self.x.shape[0], 1))
+                for i, energy in enumerate(energies):
+                    if (energy > np.min(self.x)) and (energy < np.max(self.x)):
+                            
+                        if type(self.params_dict["Det"]) == str : 
+                            D = det_efficiency_from_curve(energy,self.params_dict["Det"])
+                        else : 
+                            D = det_efficiency(energy,self.params_dict["Det"])
+
+                        A = absorption_correction(energy,**self.params_dict["Abs"],elements_dict = {elt : 1.0})
+                        
+                        width = self.width_slope * energy + self.width_intercept
+                        if energy < reference_elt[elt] : 
+                            peaks_low += (
+                                cs[i]
+                                * gaussian(self.x, energy, width / 2.3548)[
+                                    np.newaxis
+                                ].T
+                            )*D*A
+                        else : 
+                            peaks_high += (
+                                cs[i]
+                                * gaussian(self.x, energy, width / 2.3548)[
+                                    np.newaxis
+                                ].T
+                            )*D*A
+                peaks = np.hstack((peaks_low,peaks_high))
+            else : 
+                peaks = np.zeros((self.x.shape[0], 1))
+                for i, energy in enumerate(energies):
+                    
+                    # The actual detected width is calculated at each energy
+                    if (energy > np.min(self.x)) and (energy < np.max(self.x)):
+                        
+                        if type(self.params_dict["Det"]) == str : 
+                            D = det_efficiency_from_curve(energy,self.params_dict["Det"])
+                        else : 
+                            D = det_efficiency(energy,self.params_dict["Det"])
+
+                        A = absorption_correction(energy,**self.params_dict["Abs"],elements_dict = {elt : 1.0})
+                        
+                        width = self.width_slope * energy + self.width_intercept
+                        
+
+                        peaks += (
+                            cs[i]
+                            * gaussian(self.x, energy, width / 2.3548)[
+                                np.newaxis
+                            ].T
+                        )*D*A
+        
+            
+            if np.max(peaks) > 0.0:
+                self.G = np.concatenate((self.G, peaks), axis=1)
+                if elt in reference_elt : 
+                    self.model_elts.append(str(elt)+'_lo')
+                    self.model_elts.append(str(elt)+'_hi')
+                else : 
+                    self.model_elts.append(str(elt))
+            else : 
+                print("No peak is present in the energy range for element : {}".format(elt))           
+
+    @symbol_to_number_list
+    @symbol_to_number_dict
+    def generate_g_matr(self, g_type="bremsstrahlung",*,elements=[],elements_dict = {},**kwargs):
         r"""
-        The data in the form of a 2D array of shape (n_samples, n_features).
-        """
-        if self._X is None :  
-            shape = self.axes_manager[1].size, self.axes_manager[0].size, self.axes_manager[2].size
-            self._X = self.data.reshape((shape[0]*shape[1], shape[2])).T
-        return self._X
+        Generate the G matrix. With a complete model the matrix is (e_size,n+2). The first n columns correspond to the sum of X-ray characteristic peaks associated to each shell of the elements. The last 2 columns correspond to a bremsstrahlung model. 
+        
+        The first n columns of G (noted :math:`\kappa`), corresponding to the characteristic X-rays, can be calculated using the following formula:
+        
+        .. math::
 
-    @property
-    def Xdot (self) : 
-        r"""
-        The ground truth in the form of a 3D array of shape (shape_2d[0],shape_2d[1],n_features), if available.
-        """
-        if self._Xdot is None : 
-            try : 
-                self._Xdot = self.phases @ self.maps
-            except AttributeError : 
-                print("This dataset contains no ground truth. Nothing was done.")
-        return self._Xdot
+            \kappa_{k,Z} = \sum_{ij} x_{ij}(Z) \frac{1}{\Delta(\varepsilon_k) \sqrt{2\pi} } e{^{-\frac{1}{2} {\left( \frac{\varepsilon_k - \varepsilon^{ij}(Z)}{\Delta(\varepsilon_k)} \right)}^2}}
+        
+        where :math:`\varepsilon_k` is the energy of the kth energy channel, :math:`\varepsilon^{ij}(Z)` is the energy of the ijth line of the Zth element, :math:`\Delta(\varepsilon_k)` is the FWHM of the detector at the energy :math:`\varepsilon_k` and :math:`x_{ij}(Z)` is the intensity ratio of the ijth line of the Zth element. The last term of the equation is a gaussian function centered at :math:`\varepsilon^{ij}(Z)` and with a FWHM of :math:`\Delta(\varepsilon_k)`.
 
+        The last two columns of G (noted :math:`\beta`), corresponding to the bremsstrahlung model, can be calculated using the following formula:
 
-    @property
-    def maps (self) :
-        r"""
-        Ground truth of the spatial distribution of the phases in the form of a 3D array of shape (shape_2d[0],shape_2d[1],n_phases), if available.
-        """ 
-        if self._maps is None : 
-            self._maps = self.build_ground_truth()[1]
-        return self._maps
+        .. math::
 
-    @property
-    def phases (self) : 
-        r"""
-        Ground truth of the spectra of the phases in the form of a 2D array of shape (n_phases,n_features), if available.
-        """
-        if self._phases is None : 
-            self._phases = self.build_ground_truth()[0]
-        return self._phases
+            \beta_{k,n+1} = \frac{\varepsilon_0 - \varepsilon_k}{\varepsilon_0 \varepsilon_k} \times \frac{1 - (\varepsilon_0 - \varepsilon_k)}{\varepsilon_0}
 
-    @property
-    def maps_2d (self) : 
-        r"""
-        Ground truth of the spatial distribution of the phases in the form of a 2D array of shape (shape_2d[0]*shape_2d[1],n_phases), if available.
-        """
-        if self._maps_2d is None : 
-            self._maps_2d = self.build_ground_truth(reshape = False)[1]
-        return self._maps_2d
-    
-    @property
-    def model (self) :
-        r"""
-        The :class:`espm.models.EDXS` model corresponding to the metadata of the :class:`EDS_espm` object.
-        """ 
-        if self.model_ is None : 
-            mod_pars = get_metadata(self)
-            self.model_ = EDXS(**mod_pars)
-        return self.model_
+            \beta_{k,n+2} = \frac{(\varepsilon_0 - \varepsilon_k)^2}{\varepsilon^2_0 \varepsilon_k}
 
-    def build_ground_truth(self,reshape = True) : 
-        r"""
-        Get the ground truth stored in the metadata of the :class:`EDS_espm` object, if available. The reshape arguments can be used to get the ground truth in a form easier to use for machine learning algorithms.
-
-        Parameters
-        ----------
-        reshape : bool, optional
-            If False, the ground truth is returned in the form of a 3D array of shape (shape_2d[0],shape_2d[1],n_phases) and a 2D array of shape (n_phases,n_features).
+        Note that there is no parameter for the bremsstrahlung since it is supposed to be learned with the W matrix (see espm.estimators).
         
-        Returns
-        -------
-        phases : numpy.ndarray
-            The ground truth of the spectra of the phases.
-        weights : numpy.ndarray
-            The ground truth of the spatial distribution of the phases.
-        """
-        if "phases" in self.metadata.Truth.Data : 
-            phases = self.metadata.Truth.Data.phases
-            weights = self.metadata.Truth.Data.weights
-            if reshape : 
-                phases = phases.T
-                weights = weights.reshape((weights.shape[0]*weights.shape[1], weights.shape[2])).T
-        else : 
-            raise AttributeError("There is no ground truth contained in this dataset")
-        return phases, weights
-
-    def build_G(self, problem_type = "bremsstrahlung", reference_elt = {}) :
-        r"""
-        Build the G matrix of the :class:`espm.models.EDXS` model corresponding to the metadata of the :class:`EDS_espm` object and stores it as an attribute.
-
         Parameters
         ----------
-        problem_type : str, optional
-            Determines the type of the G matrix to build. It can be "bremsstrahlung", "no_brstlg" or "identity". The parameters correspond to:
-                - "bremsstrahlung" : the G matrix is a callable with both characteristic X-rays and a bremsstrahlung model.
-                - "no_brstlg" : the G matrix is a matrix with only characteristic X-rays.
-                - "identity" : the G matrix is None which is equivalent to an identity matrix for espm functions.
-        reference_elt : dict, optional
-            Dictionary containing atomic numbers and a corresponding cut-off energies. It is used to separate the characteristic X-rays of the given elements into two energies ranges and assign them each a column in the G matrix instead of having one column per element.
-            For example reference_elt = {"26",3.0} will separate the characteristic X-rays of the element Fe into two energies ranges and assign them each a column in the G matrix. This is useful to circumvent issues with the absorption.
+        g_type : 
+            :string: Options of the edxs model to include in the G matrix. The three possibilities are "identity", "no_brstlg" and "bremsstrahlung". G is going to be the identity matrix, only characteristic X-ray peaks or characteristic X-rays plus bremsstrahlung model, respectively.
+        elements_dict : 
+            :dict: The keys are chemical elements (atomic number) and the values are cut-off energies. This argument is used to split some of the columns of G into 2 columns. The first column corresponds to characteristic X-rays before the cut-off and second one corresponds to characteristic X-rays before the cut-off. This feature is implemented to enable more accurate absorption correction.
+        elements : 
+            :list: List of modeled chemical elements. The list can be populated either with atomic numbers or chemical symbols, e.g. "Fe" or 26.
 
         Returns
         -------
-        G : None or numpy.ndarray or callable
-            The G matrix of the :class:`espm.models.EDXS` model corresponding to the metadata of the :class:`EDS_espm` object.
-        """
-        self.problem_type = problem_type
-        self.reference_elt = reference_elt
-        g_pars = {"g_type" : problem_type, "elements" : self.metadata.Sample.elements, "reference_elt" : reference_elt}
-        
-        if problem_type == "bremsstrahlung" : 
-            self.G = self.update_G
-            # to init the model.model_elts and model.norm
-            self.G()
-        else : 
-            self.G = build_G(self.model,g_pars)
-
-        # Storing the model parameters in the metadata so that the decomposition does not erase them
-        # Indeed the decomposition re-creates a new object of the same class when it is called
-        self.metadata.EDS_model= {}
-        self.metadata.EDS_model.problem_type = problem_type
-        self.metadata.EDS_model.reference_elt = reference_elt
-        self.metadata.EDS_model.elements = self.model.model_elts
-        self.metadata.EDS_model.norm = self.model.norm
-
-    def update_G(self, part_W=None, G=None):
-        r"""
-        Update the absortion part of the bremsstrahlung of the G matrix.
-        """
-        g_params = {"g_type" : self.problem_type, "elements" : self.metadata.Sample.elements, "reference_elt" : self.reference_elt}
-        G = G_EDXS(self.model, g_params, part_W=part_W, G=G)
-        return G
-
-    def set_analysis_parameters (self,beam_energy = 200, azimuth_angle = 0.0, elevation_angle = 22.0, tilt_stage = 0.0, elements = [], thickness = 200e-7, density = 3.5, detector_type = "SDD_efficiency.txt", width_slope = 0.01, width_intercept = 0.065, xray_db = "default_xrays.json") :
-        r"""
-        Helper function to set the metadata of the :class:`EDS_espm` object. Be careful, it will overwrite the metadata of the object.
+        g matrix :
+            :np.array 2D: matrix of the edx model. 
 
-        Parameters
-        ----------
-        beam_energy : float, optional
-            The energy of the electron beam in keV.
-        azimuth_angle : float, optional
-            The azimuth angle of the EDS detector in degrees.
-        elevation_angle : float, optional
-            The elevation angle of the EDS detector in degrees.
-        tilt_stage : float, optional
-            The tilt angle of the sample stage in degrees (usually it correspond to alpha on FEI instruments).
-        elements : list, optional
-            List of the elements to be used in the analysis.
-        thickness : float, optional
-            The thickness of the sample in centimeters.
-        density : float, optional
-            The density of the sample in g/cm^3.
-        detector_type : str, optional
-            The type of the detector. It is either  the name of a text file containing the efficiency of 
-        width_slope : float, optional
-            The slope of the linear fit of the detector width as a function of the energy.
-        width_intercept : float, optional
-            The intercept of the linear fit of the detector width as a function of the energy.
-        xray_db : str, optional
-            The name of the X-ray emission cross-section database to be used. The default tables are avalaible in the espm/tables folder. Additional tables can be generated by emtables.
+        Notes
+        -----
+        See our paper about the espm package :cite:p:`teurtrie2023espm` for more information about the equations of this model.
         """
-        self.set_microscope_parameters(beam_energy = beam_energy, azimuth_angle = azimuth_angle, elevation_angle = elevation_angle,tilt_stage = tilt_stage)
-        self.add_elements(elements = elements)
-        self.metadata.Sample.thickness = thickness
-        self.metadata.Sample.density = density
-        try : 
-            del self.metadata.Acquisition_instrument.TEM.Detector.EDS.type
-        except AttributeError : 
-            pass
-        self.metadata.Acquisition_instrument.TEM.Detector.EDS.type = detector_type
-        self.metadata.Acquisition_instrument.TEM.Detector.EDS.width_slope = width_slope
-        self.metadata.Acquisition_instrument.TEM.Detector.EDS.width_intercept = width_intercept
-        self.metadata.xray_db = xray_db
-
-        self.metadata.Acquisition_instrument.TEM.Detector.EDS.take_off_angle = take_off_angle(tilt_stage,azimuth_angle,elevation_angle)
+        
+        # Reset the internally stored elements list
+        self.model_elts = []
+        
+        if g_type == "bremsstrahlung" : 
+            self.bkgd_in_G = True
+        else : 
+            self.bkgd_in_G = False
 
-    def set_additional_parameters(self,thickness = 200e-7, density = 3.5,  detector_type = "SDD_efficiency.txt", width_slope = 0.01, width_intercept = 0.065, xray_db = "default_xrays.json") : 
-        r"""
-        Helper function to set the metadata that are specific to the :mod:`espm` package so that it does not overwrite experimental metadata.
-        See the documentation of the :func:`set_analysis_parameters` function for the meaning of the parameters.
-        """
-        self.metadata.Sample.thickness = thickness
-        self.metadata.Sample.density = density
-        try : 
-            del self.metadata.Acquisition_instrument.TEM.Detector.EDS.type
-        except AttributeError : 
-            pass
-        self.metadata.Acquisition_instrument.TEM.Detector.EDS.type = detector_type
-        self.metadata.Acquisition_instrument.TEM.Detector.EDS.width_slope = width_slope
-        self.metadata.Acquisition_instrument.TEM.Detector.EDS.width_intercept = width_intercept
-        self.metadata.xray_db = xray_db
-
-        tilt_stage = self.metadata.Acquisition_instrument.TEM.Stage.tilt_alpha
-        azimuth_angle = self.metadata.Acquisition_instrument.TEM.Detector.EDS.azimuth_angle
-        elevation_angle = self.metadata.Acquisition_instrument.TEM.Detector.EDS.elevation_angle
-        self.metadata.Acquisition_instrument.TEM.Detector.EDS.take_off_angle = take_off_angle(tilt_stage,azimuth_angle,elevation_angle)
+        # None is a default value for the G matrix and thus G will be considered to be the identity matrix in most of espm functions.
+        if len(elements) == 0:
+            self.G = None
+
+        elif g_type == "identity" : 
+            self.G = None
+        # model based on elements_list
+        elif (g_type == "bremsstrahlung") or (g_type == "no_brstlg"):
+            
+            # The number of shells depend on the element, it is then not straightforward to pre-determine the size of g_matr
+            self.G = np.zeros((self.x.shape[0], 0))
+            # For each element we unpack all shells and then unpack all lines of each shell.
+            self.__add_elts_G(reference_elt = elements_dict, elements = elements)
+            
+            # Appends a pure continuum spectrum is needed
+            if self.bkgd_in_G:
+                approx_elts = {key : 1.0/len(elements) for key in elements}
+                brstlg_spectrum = G_bremsstrahlung(self.x,self.E0,self.params_dict,elements_dict=approx_elts)
+                if np.max(brstlg_spectrum) > 0.0 : 
+                    self.G = np.concatenate((self.G, brstlg_spectrum), axis=1)
+                else : 
+                    print("Bremsstrahlung parameters were not provided, bkgd not added in G")
+                    self.bkgd_in_G = False
+
+            norms = np.sqrt(np.sum(self.G**2, axis=0, keepdims=True))
+            if g_type == "bremsstrahlung" : 
+                norms[0][:-2] = np.mean(norms[0][:-2])
+            else : 
+                norms[0] = np.mean(norms[0])
+            self.norm = norms
+            self.G /= self.norm
+        else : 
+            print("g_type has to be one of those : \"bremsstrahlung\", \"no_brstlg\" or \"identity\". G will be None, corresponding to \"identity\". ")
 
-    @number_to_symbol_list
-    def add_elements(self, *, elements = []) :
+    def generate_phases(self, phases_parameters) : 
         r"""
-        Add elements to the existing list of elements in the metadata.
+        Generate a series of spectra from list of phase parameters. 
 
         Parameters
         ----------
-        elements : list, optional
-            List of the elements to be added to the existing list of elements in the metadata. They have to be chemical symbols (e.g. ['Si','Fe', 'O']).
-        """
-        try : 
-            self.metadata.Sample.elements = elements
-        except AttributeError :
-            self.metadata.Sample = {}
-            self.metadata.Sample.elements = elements
+        phases_parameters : 
+            :list: List of dicts containing the phase parameters.
+        
+        Returns
+        -------
+        phase_array : 
+            :np.array 2D: Array which lines correspond to the modelled phases in the input list.
 
-    def set_microscope_parameters(self, beam_energy = 200, azimuth_angle = 0.0, elevation_angle = 22.0,tilt_stage = 0.0) : 
-        r"""
-        Helper function to set the microscope parameters of the :class:`EDS_espm` object. Be careful, it will overwrite the microscope parameters of the object.
-        See the documentation of the :func:`set_analysis_parameters` function for the meaning of the parameters.
+        Notes
+        -----
+        The absorption correction is done using the average composition of the phases. The same correction is used for each phase.
         """
-        self.metadata.Acquisition_instrument = {}
-        self.metadata.Acquisition_instrument.TEM = {}
-        self.metadata.Acquisition_instrument.TEM.Stage = {}
-        self.metadata.Acquisition_instrument.TEM.Detector = {}
-        self.metadata.Acquisition_instrument.TEM.Detector.EDS = {}
-        self.metadata.Acquisition_instrument.TEM.beam_energy = beam_energy
-        self.metadata.Acquisition_instrument.TEM.Stage.tilt_alpha = tilt_stage
-        self.metadata.Acquisition_instrument.TEM.Detector.EDS.azimuth_angle = azimuth_angle
-        self.metadata.Acquisition_instrument.TEM.Detector.EDS.elevation_angle = elevation_angle
-        self.metadata.Acquisition_instrument.TEM.Detector.EDS.energy_resolution_MnKa = 130.0
+        self.phases = []
+        unique_elts = dict(elts_dict_from_dict_list([x["elements_dict"] for x in phases_parameters]))
+        for p in phases_parameters:
+            # p.update({"elements_dict" : unique_elts})
+            self.phases.append(self.generate_spectrum(**p,abs_elts_dict = unique_elts))
+        self.phases = np.array(self.phases)
+        self.phases /= self.phases.sum(axis = 1)[:,np.newaxis]
 
-    def set_fixed_W (self,phases_dict) : 
+    @symbol_to_number_dict
+    def generate_spectrum(self, b0=0, b1 = 0, scale = 1.0,abs_elts_dict = {},*,elements_dict = {}):
         r"""
-        Helper function to create a fixed_W matrix. The output matrix will have -1 entries except for the elements (and bremsstrahlung parameters) that are present in the phases_dict dictionary.
-        In the output (fixed_W) matrix, the -1 entries will be ignored during the decomposition using :class:`espm.estimator.NMFEstimator` are normally learned while the non-negative entries will be fixed to the values given in the phases_dict dictionary.
-        Usually, the easiest is to fix some elements to 0.0 in some phases if you want to improve unmixing results. For example, if you have a phase with only Si and O, you can fix the Fe element to 0.0 in this phase.
+        Generate a spectrum from bremsstrahlung parameters and a chemical composition. The modelling is done using the same formula as for the generate_g_matr function.
 
         Parameters
         ----------
-        phases_dict : dict
-            Determines which elements of fixed_W are going to be non-negative. The dictionnary has typically the following structure : phases_dict = {"phase1_name" : {"Fe" : 0.0, "O" : 1.25e23}, "phase2_name" : {"Si" : 0.0, "b0" : 0.05}}.
+        b0 : 
+            :float: First bremsstrahlung parameter. 
+        b1 : 
+            :float: Second bremsstrahlung parameter.
+        scale : 
+            :float: Scale factor to apply to the bremsstrahlung. Feature to be removed, scaling should be done with b0 and b1.
+        abs_elts_dict : 
+            :dict: Dictionnary of elements and associated concentrations. This dictionnary is used to calculate the contribution of the absorption in the spectrum.
+        elements_dict : 
+            :dict: Dictionnary of elements and associated concentrations describing the chemical composition of the modeled sample.
         Returns
         -------
-        W : numpy.ndarray
-        """
-        elements = self.metadata.Sample.elements
-        if self.problem_type == "no_brstlg" : 
-            W = -1* np.ones((len(elements), len(phases_dict.keys())))
-        elif self.problem_type == "bremsstrahlung" : 
-            W = -1* np.ones((len(elements)+2, len(phases_dict.keys())))
-        else : 
-            raise ValueError("problem type should be either no_brstlg or bremsstrahlung")
-        for p, phase in enumerate(phases_dict) : 
-            for e, elt in enumerate(elements) : 
-                for key in phases_dict[phase] : 
-                    if key == elt : 
-                        W[e,p] = phases_dict[phase][key]
-            for key in phases_dict[phase] : 
-                if key == "b0" : 
-                    W[-2,p] = phases_dict[phase][key]
-                if key == "b1" : 
-                    W[-1,p] = phases_dict[phase][key]
-        return W
-    
-    def print_concentration_report (self,abs = False) : 
-        r"""
-        Print a report of the chemical concentrations from a fitted W.
+        spectrum : 
+            :np.array 1D: Output edx spectrum corresponding to the input chemical composition.
 
-        Parameters
-        ----------
-        abs : bool
-            If True, print the absolute concentrations, if False, print the relative concentrations.
+        Examples
+        --------
 
-        Returns
-        -------
-        None
+        .. plot::
+            :context: close-figs
+
+            >>> import matplotlib.pyplot as plt
+            >>> from espm.models.edxs import EDXS
+            >>> from espm.conf import DEFAULT_EDXS_PARAMS
+            >>> b0, b1 = 5.5367e-5, 0.00192181
+            >>> elts_dict = {"Si" : 1.0,"Ca" : 1.0,"O" : 3.0,"C" : 0.3}
+            >>> model = EDXS(**DEFAULT_EDXS_PARAMS)
+            >>> spectrum = model.generate_spectrum(b0,b1, elements_dict = elts_dict)
+            >>> plt.plot(spectrum)
 
         Notes
         -----
-        - This function is only available if the learning results contain a decomposition algorithm that has been fitted.
-        - The "absolute" concentrations correspond to some physical number. To retrieve the number of atoms per unit volume, you need to multiply by the correct pre-factors such as beam current, detector solid angle, etc...
+        Check EDXS_function for details about the bremsstrahlung model.
         """
-        if not(isinstance(self.learning_results.decomposition_algorithm,NMFEstimator)) :
-            raise ValueError("No espm learning results available, please run a decomposition with an espm algorithm first")
+        temp = np.zeros_like(self.x)
+        for elt in elements_dict.keys():
+            if self.lines : 
+                energies, cs = read_lines_db(elt,self.db_dict)
+            else : 
+                energies, cs = read_compact_db(elt,self.db_dict)
+            for i, energy in enumerate(energies):
+                if (energy > np.min(self.x)) and (energy < np.max(self.x)):
+                    if type(self.params_dict["Det"]) == str : 
+                        D = det_efficiency_from_curve(energy,self.params_dict["Det"])
+                    else : 
+                        D = det_efficiency(energy,self.params_dict["Det"])
+                    A = absorption_correction(energy,**self.params_dict["Abs"],elements_dict = {elt : 1.0})
+                
+                    width = self.width_slope * energy + self.width_intercept
+                    temp += (
+                        elements_dict[elt]
+                        * cs[i]
+                        * gaussian(self.x, energy, width / 2.3548)
+                    )*A*D
+        temp /= temp.sum()
+        if abs_elts_dict == {} : 
+            temp += continuum_xrays(self.x,self.params_dict,b0,b1,self.E0,elements_dict=elements_dict) * scale
+        else : 
+            temp += continuum_xrays(self.x,self.params_dict,b0,b1,self.E0,elements_dict=abs_elts_dict) * scale
         
-        W = self.learning_results.decomposition_algorithm.W_
+        return temp
+    
+    def get_elements(self) :
+        for elt in self.model_elts:
+            if re.match(r'[0-9]*(_lo)',elt) : 
+                pass
+            elif re.match(r'[0-9]*(_hi)',elt) :
+                m = re.match(r'([0-9]*)(_hi)',elt) 
+                yield m.group(1)
+            else : 
+                yield elt
         
-        norm = self.metadata.EDS_model.norm
-        elts = self.metadata.EDS_model.elements
+    def carac_X_span(self) : 
+        all_indices = []
+        for elt in self.get_elements():
+            if self.lines : 
+                energies, cs = read_lines_db(elt,self.db_dict)
+            else : 
+                energies, cs = read_compact_db(elt,self.db_dict)
+            for energy in energies:
+                width = self.width_slope * energy + self.width_intercept
+                span = [energy - 2*width, energy + 2*width]
+                indices = np.where((self.x > span[0]) & (self.x < span[1]))[0]
+                all_indices.append(indices)
+        return np.unique(np.concatenate(all_indices))
+    
+    def NMF_initialize_W(self, D) :
+        if self.G is None :
+            raise ValueError('The G matrix is identity, the W matrix cannot be initialized. Please use a np.array for G in the ESpM-NMF instead of the model object')
+        if self.bkgd_in_G and self.custom_init:
+            idx = self.carac_X_span()
+            mask = np.ones(self.G.shape[0], bool)
+            mask[idx] = 0
+            Wbrem = (np.linalg.lstsq(self.G[mask,-2:],D[mask,:],rcond = None)[0]).clip(min = 0)
+            Wcarac = (np.linalg.lstsq(self.G[idx,:-2],D[idx,:] ,rcond = None)[0]).clip(min = 0)
+            # filter = np.where(np.mean(self.G[:,:-2],axis=1)<(np.max(np.mean(self.G[:,:-2],axis=1))*0.001))[0]
+            W = np.vstack((Wcarac,Wbrem))
+        else :
+            W = (np.linalg.lstsq(self.G,D,rcond = None)[0]).clip(min = 0)
 
-        @number_to_symbol_list
-        def convert_elts(elements = []) :
-            return elements
-        
-        elements = convert_elts(elements = elts)
+        return W
         
-        norm_W = W / W.sum(axis = 0)
-        abs_W =   W / norm[0][:,np.newaxis] 
+    def NMF_simplex(self):
+        """
+        Produce the indices of the rows of W on which to perform the simplex constraint.
+        """
+        # We don't check here whether G was correctyl initialized since it is tested in the init.
+        ind_list = []
+        # We skip the low energy lines
+        for i, elt in enumerate(self.model_elts):
+            if re.match(r'[0-9]*(_lo)',elt) : 
+                pass
+            else : 
+                ind_list.append(i)
+        # We skip the bremsstrahlung
+        return ind_list
+    
+    def NMF_update(self, W=None):
+        """
+        Update the G matrix with the new absorption correction.
+        """
+        # We don't need to check whether G was correctyl initialized it should work anyway.
         
-        if abs : 
-            print("Abs. quantif. report")
-            title_string = " "*5
-
-            for i in range(norm_W.shape[1]) : 
-                title_string += "{:}".format("p" + str(i)) + " "*8
-            print(title_string)
-            
-            for i,j in enumerate(elements) : 
-                main_string = ""
-                main_string += "{:2}".format(j) + " : "
-                for k in range(norm_W.shape[1]) :
-                    main_string += "{:.3e} ".format(abs_W[i,k])
-                print(main_string)
-
-        else : 
-            print("Concentrations report")
-            title_string = ""
-
-            for i in range(norm_W.shape[1]) : 
-                title_string += "{:>7}".format("p" + str(i))
-            print(title_string)
-            
-            for i,j in enumerate(elements) : 
-                main_string = ""
-                main_string += "{:2}".format(j) + " : "
-                for k in range(norm_W.shape[1]) :
-                    main_string += "{:05.4f} ".format(norm_W[i,k])
-                print(main_string)
+        if W is None:
+            return self.G
+        if not(self.bkgd_in_G) :
+            return self.G
+        else :
+            new_brstlg = self.update_bremsstrahlung(W)
+            new_G = self.G.copy()
+            new_G[:,-2:] = new_brstlg/self.norm[0][-2:]
+            self.G = new_G
+            return self.G
 
+    def update_bremsstrahlung(self, W) : 
+        """
+        Update the bremsstrahlung part of the G matrix. This function is used for the NMF decomposition so that the absorption correction is updated in between each step.
+        """
+        if not(self.bkgd_in_G) :
+            raise AttributeError("The bremsstrahlung is not comprised in the model.")
         
-
-
-######################
-# Axiliary functions #
-######################
-
-def get_metadata(spim) : 
-    r"""
-    Get the metadata of the :class:`EDS_espm` object and format it as a model parameters dictionary.
-    """
-    mod_pars = {}
-    try :
-        mod_pars["E0"] = spim.metadata.Acquisition_instrument.TEM.beam_energy
-        mod_pars["e_offset"] = spim.axes_manager[-1].offset
-        assert mod_pars["e_offset"] > 0.01, "The energy scale can't include 0, it will produce errors elsewhere. Please crop your data."
-        mod_pars["e_scale"] = spim.axes_manager[-1].scale
-        mod_pars["e_size"] = spim.axes_manager[-1].size
-        mod_pars["db_name"] = spim.metadata.xray_db
-        mod_pars["width_slope"] = spim.metadata.Acquisition_instrument.TEM.Detector.EDS.width_slope
-        mod_pars["width_intercept"] = spim.metadata.Acquisition_instrument.TEM.Detector.EDS.width_intercept
-    
-        pars_dict = {}
-        pars_dict["Abs"] = {
-            "thickness" : spim.metadata.Sample.thickness,
-            "toa" : spim.metadata.Acquisition_instrument.TEM.Detector.EDS.take_off_angle,
-            "density" : spim.metadata.Sample.density
-        }
-        try : 
-            pars_dict["Det"] = spim.metadata.Acquisition_instrument.TEM.Detector.EDS.type.as_dictionary()
-        except AttributeError : 
-            pars_dict["Det"] = spim.metadata.Acquisition_instrument.TEM.Detector.EDS.type
-
-        mod_pars["params_dict"] = pars_dict
-
-    except AttributeError : 
-        print("You need to define the relevant parameters for the analysis. Use the set_analysis_parameters function.")
-
-    return mod_pars
-
-def build_G(model, g_params) :
-    model.generate_g_matr(**g_params)
-    return model.G
-
-
+        indices = self.NMF_simplex()
+        mean_compo = np.mean(W[indices,:],axis=1)
+        normed_compo = mean_compo/np.sum(mean_compo)
+        elements_dict = {key : normed_compo[i] for i,key in enumerate(self.get_elements())}
+        bremsstrahlung = G_bremsstrahlung(self.x,self.E0,self.params_dict,elements_dict=elements_dict)
+        return bremsstrahlung
```

### Comparing `espm-1.0.0/espm/datasets/toy-problem/phase1.png` & `espm-1.1.1/espm/datasets/toy-problem/phase1.png`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/espm/datasets/toy-problem/phase2.png` & `espm-1.1.1/espm/datasets/toy-problem/phase2.png`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/espm/estimators/__init__.py` & `espm-1.1.1/espm/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/espm/estimators/base.py` & `espm-1.1.1/espm/estimators/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from espm.measures import KLdiv_loss, Frobenius_loss, find_min_angle, find_min_MSE
 from espm.conf import log_shift
 from espm.utils import rescaled_DH
 import time
 from abc import ABC, abstractmethod
 from espm.utils import create_laplacian_matrix 
 from scipy.sparse import lil_matrix
+from espm.models.base import PhysicalModel
 
 
 def normalization_factor (X, nc) : 
     m = np.mean(X)
     return nc/(m*X.shape[0])
 
 class NMFEstimator(ABC, TransformerMixin, BaseEstimator):
@@ -98,33 +99,38 @@
     eval_print : int, default=10
         Number of iterations between each evaluation of the loss function.
     true_D : np.array or None, default=None
         Ground truth for the matrix :math:`GW`. Used for evaluation purposes.
     true_H : np.array or None, default=None
         Ground truth for the matrix :math:`H`. Used for evaluation purposes.
     fixed_H : np.array or None, default=None
-        If not None, it fixes the non-zero values of the matrix :math:`H`.
+        If not None, it fixes the non-zero values of the matrix :math:`H`. 
+        Note that convergence is not guaranteed with fixed_H enabled.
     fixed_W : np.array or None, default=None
         If not None, it fixes the non-zero values of the matrix :math:`W`.
+        Note that convergence is not guaranteed with fixed_W enabled.
+    no_stop_criterion : bool, default=False
+        If True, the algorithm will not stop when the stopping criterion is reached and will continue until max_iter is reached.
     hspy_comp : bool, default=False
         If True, the algorithm will use the format compatible with hyperspy.
         Use this option if you run the algorithm with the method decompositio in hyperspy.
         For example:
         .. code-block::python
             >>> est = SmoothNMF( n_components = 3, hspy_comp = True)
             >>> out = spim.decomposition(algorithm = est, return_info=True)
-        
+
     """
     loss_names_ = ["KL_div_loss"]
     const_KL_ = None
     
     def __init__(self, n_components=2, init=None, tol=1e-4, max_iter=200,
                  random_state=None, verbose=1, debug=False,
                  l2=False,  G=None, shape_2d = None, normalize = False, log_shift=log_shift, 
-                 eval_print=10, true_D = None, true_H = None, fixed_H = None, fixed_W = None, hspy_comp = False
+                 eval_print=10, true_D = None, true_H = None, fixed_H = None, fixed_W = None, hspy_comp = False, 
+                 no_stop_criterion = False, simplex_H=False, simplex_W = True
                  ):
         self.n_components = n_components
         self.init = init
         self.tol = tol
         self.max_iter = max_iter
         self.random_state = random_state
         self.verbose = verbose
@@ -136,14 +142,17 @@
         self.eval_print = eval_print
         self.true_D = true_D
         self.true_H = true_H
         self.fixed_H = fixed_H
         self.fixed_W = fixed_W
         self.hspy_comp = hspy_comp
         self.normalize = normalize
+        self.no_stop_criterion = no_stop_criterion
+        self.simplex_H = simplex_H
+        self.simplex_W = simplex_W
 
     def _more_tags(self):
         return {'requires_positive_X': True}
 
     @abstractmethod
     def _iteration(self,  W, H):
         pass
@@ -188,15 +197,17 @@
             loss_ =  KLdiv_loss(X, GW, H, self.log_shift, average=False) + self.const_KL_
         if average:
             loss_ = loss_ / self.GWH_numel_
         self.detailed_loss_ = [loss_]
         return loss_
 
     def fit_transform(self, X, y=None, W=None, H=None):
-        """Learn a NMF model for the data X and returns the transformed data.
+        """
+        Main function of the estimator object.
+        Learn a NMF model for the data X and returns the transformed data.
         This is more efficient than calling fit followed by transform.
 
         The size of:
 
         * :math:`X` is :math:`(n, p)`,
         * :math:`W` is :math:`(m, k)`,
         * :math:`H` is :math:`(k, p)`,
@@ -215,14 +226,17 @@
 
         Returns
         -------
         GW : ndarrays
             Transformed data.
         
         """
+        ############################
+        # Initialize the algorithm #
+        ############################
         if self.hspy_comp : 
             self.X_ = self._validate_data(X.T, dtype=[np.float64, np.float32])
         else : 
             self.X_ = self._validate_data(X, dtype=[np.float64, np.float32])
 
         if self.hspy_comp==False:
             try:
@@ -232,78 +246,91 @@
                 if calframe[1][3]=="decomposition" and "hyperspy" in calframe[1][1]:
                     print("Are you calling the function decomposition from Hyperspy?\n" +
                         "If so, please set the compatibility argument 'hspy_comp' to True.\n\n" + 
                         "If this argument is not set correctly, the function will not work properly!!!")
             except:
                 pass
 
-
+        # The algorithm does not work when full columns or lines of X are zero
         self.X_ = self.remove_zeros_lines(self.X_, self.log_shift)
+
         self.const_KL_ = None
         if self.normalize : 
+            # We normalize the data so that the strength of the regularization is somewhat the same for all datasets
             self.norm_factor_ = normalization_factor(self.X_,self.n_components)
             self.X_ = self.norm_factor_ * self.X_
         
-
-        if callable(self.G): 
-            G = self.G()
-        else : 
+        if isinstance(self.G, PhysicalModel):
+            self.physics_model_ = self.G
+            G = self.physics_model_.NMF_update()
+        else:
+            self.physics_model_ = None
             G = self.G
         
-        self.G_, self.W_, self.H_ = initialize_algorithms(X = self.X_, G = G, W = W, H = H, n_components = self.n_components, init = self.init, random_state = self.random_state, force_simplex = self.force_simplex)
-
+        self.G_, self.W_, self.H_ = initialize_algorithms(X = self.X_,
+                                                          G = G,
+                                                          W = W,
+                                                          H = H,
+                                                          n_components = self.n_components,
+                                                          init = self.init,
+                                                          random_state = self.random_state,
+                                                          simplex_H = self.simplex_H,
+                                                          simplex_W = self.simplex_W,
+                                                          physics_model = self.physics_model_)
+        
         if not(self.shape_2d is None) :
             self.L_ = create_laplacian_matrix(*self.shape_2d)
         else : 
             self.L_ =lil_matrix((self.X_.shape[1],self.X_.shape[1]),dtype=np.float32)
             self.L_.setdiag([1]*self.X_.shape[1])
 
         algo_start = time.time()
-        # If mu_sparse != 0, this is the regularized step of the algorithm
-        # Otherwise this is directly the data fitting step
         eval_before = np.inf
         eval_init = self.loss(self.W_, self.H_)
         self.n_iter_ = 0
 
-        # if self.debug:
         self.losses_ = []
         self.rel_ = []
         self.detailed_losses_ = []
         if not(self.true_D is None) and not(self.true_H is None) : 
             if (self.true_D.shape[1] == self.n_components) and (self.true_H.shape[0] == self.n_components) : 
                 self.angles_ = []
                 self.mse_ = []
                 self.true_losses_ = []
                 true_DH = self.true_D @ self.true_H
             else : 
                 print("The chosen number of components does not match the number of components of the provided truth. The ground truth will be ignored.")
+        
+        #############
+        # Main loop #
+        #############
         try:
             while True:
-                # Take one step in A, P
+                # Take one step in W, H
                 old_W, old_H = self.W_.copy(), self.H_.copy()
                 
                 self.W_, self.H_ = self._iteration(self.W_, self.H_ )
                 eval_after = self.loss(self.W_, self.H_)
                 self.n_iter_ +=1
                 
-                rel_W = np.max((self.W_ - old_W)/(self.W_ + self.tol*np.mean(self.W_) ))
-                rel_H = np.max((self.H_ - old_H)/(self.H_ + self.tol*np.mean(self.H_) ))
+                rel_W = np.max(np.abs((self.W_ - old_W))/(self.W_ + self.tol*np.mean(self.W_) ))
+                rel_H = np.max(np.abs((self.H_ - old_H))/(self.H_ + self.tol*np.mean(self.H_) ))
 
                 # store some information for assessing the convergence
                 # for debugging purposes
                 
                 # We need to store this value as 
                 #    loss = self.loss(self.P_,self.A_, X = true_DA )
                 # might destroy it. Furthermore, saving the data before the if, might cause 
                 # an error if the optimization is stoped with a keyboard interrupt. 
                 detailed_loss_ = self.detailed_loss_
 
                 if not(self.true_D is None) and not(self.true_H is None) :
                     if (self.true_D.shape[1] == self.n_components) and (self.true_H.shape[0] == self.n_components) : 
-                        if self.force_simplex:
+                        if self.simplex_H or self.simplex_W:
                             W, H = self.W_, self.H_ 
                         else:
                             W, H = rescaled_DH(self.W_, self.H_ )
                         GW = self.G_ @ W
                         angles = find_min_angle(self.true_D.T,GW.T, unique=True)
                         mse = find_min_MSE(self.true_H, H,unique=True)
                         loss = self.loss(self.W_,H, X = true_DH )
@@ -315,55 +342,56 @@
                 self.detailed_losses_.append(detailed_loss_)
                 self.rel_.append([rel_W,rel_H])
                               
                 # check convergence criterions
                 if self.n_iter_ >= self.max_iter:
                     print("exits because max_iteration was reached")
                     break
-
-                # If there is no regularization the algorithm stops with this criterion
-                # Otherwise it goes to the data fitting step
-                elif max(rel_H,rel_W) < self.tol:
-                    print(
-                        "exits because of relative change rel_A {} or rel_P {} < tol ".format(
-                            rel_H,rel_W
-                        )
-                    )
-                    break
-                elif abs((eval_before - eval_after)/eval_init) < self.tol:
-                    print(
-                        "exits because of relative change < tol: {}".format(
-                            (eval_before - eval_after)/min(eval_before, eval_after)
+                
+                if not self.no_stop_criterion:
+                    # If there is no regularization the algorithm stops with this criterion
+                    # Otherwise it goes to the data fitting step
+                    if max(rel_H,rel_W) < self.tol:
+                        print(
+                            "exits because of relative change rel_A {} and rel_P {} < tol ".format(
+                                rel_H,rel_W
+                            )
                         )
-                    )
-                    break
+                        break
+                    elif abs((eval_before - eval_after)/eval_init) < self.tol:
+                        print("exits because of relative change < tol: {}".format((eval_before - eval_after)/eval_init))
+                        break
 
-                elif np.isnan(eval_after):
-                    print("exit because of the presence of NaN")
-                    break
+                    elif np.isnan(eval_after):
+                        print("exit because of the presence of NaN")
+                        break
 
-                elif (eval_before - eval_after) < 0:
-                    if hasattr(self, "accelerate"):
-                        if not self.accelerate:
-                            print("exit because of negative decrease {}: {}, {}".format((eval_before - eval_after), eval_before, eval_after))
-                            break
-                    else:
+                    elif (eval_before - eval_after) < 0:
                         print("exit because of negative decrease {}: {}, {}".format((eval_before - eval_after), eval_before, eval_after))
                         break
                 
                 if self.verbose > 0 and np.mod(self.n_iter_, self.eval_print) == 0:
                     print(
                         f"It {self.n_iter_} / {self.max_iter}: loss {eval_after:3e},  {self.n_iter_/(time.time()-algo_start):0.3f} it/s",
                     )
                     pass
-                eval_before = eval_after
+                # Update G might increase the loss so we reevaluate the loss to avoid artificial negative decrease
+                # We do this update every 3 iterations, but it is arbitrary.
+                if self.physics_model_ != None and self.n_iter_%3 == 0: 
+                    self.G_ = self.physics_model_.NMF_update(self.W_)
+                    eval_before = self.loss(self.W_, self.H_)
+                else :
+                    eval_before = eval_after
         except KeyboardInterrupt:
             pass
-        
-        if not(self.force_simplex):
+
+        ###################
+        # End of the loop #
+        ###################
+        if not(self.simplex_H) and not(self.simplex_W):
             self.W_, self.H_ = rescaled_DH(self.W_, self.H_ )
         
         algo_time = time.time() - algo_start
         print(
             f"Stopped after {self.n_iter_} iterations in {algo_time//60} minutes "
             f"and {np.round(algo_time) % 60} seconds."
         )
@@ -436,15 +464,17 @@
             Data matrix of original shape.
         
         """
         check_is_fitted(self)
         return self.G_ @ W @ self.H_
     
     def get_losses(self):
-        
+        """
+        For debug purposes : return the evolution of losses. 
+        """        
         if not(self.true_D is None) and not(self.true_H is None) :
             mse_list = []
             angles_list = []
             for i in range(self.n_components) :
                 angles_list.append("ang_p{}".format(i))
                 mse_list.append("mse_p{}".format(i))
             names = ["full_loss"] + self.loss_names_ + ["rel_W","rel_H"] + angles_list + mse_list + ["true_KL_loss"]
@@ -457,15 +487,15 @@
             tup_list = []
             for i in range(len(self.losses_)) : 
                 tup_list.append((self.losses_[i],) + tuple(self.detailed_losses_[i]) + tuple(self.rel_[i]) \
                     + tuple(self.angles_[i]) + tuple(self.mse_[i]) + (self.true_losses_[i],) )
             
             array = np.array(tup_list,dtype=dt)
         
-        #Bon j'ai copié ca comme un bourrin. Il y a moyen de faire mieux.
+        #TODO : Check this part for optimization
         else : 
             names = ["full_loss"] + self.loss_names_ + ["rel_W","rel_H"]
             dt_list = []
             for elt in names : 
                 dt_list.append((elt,"float64"))
             dt = np.dtype(dt_list)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `espm-1.0.0/espm/estimators/dicotomy.py` & `espm-1.1.1/espm/estimators/dicotomy.py`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/espm/estimators/surrogates.py` & `espm-1.1.1/espm/estimators/surrogates.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,17 +136,17 @@
     Returns
     -------
     float
         Value of the difference between the surrogate and the true value of the Laplacian regularizer at :math:`H^t
 
     """
     b_inf = trace_xtLx(L, H.T) * lambda_L / 2
-    if algo=="log_surrogate":
+    if algo in ["log_surrogate", "bmd"]:
         b_supp = smooth_dgkl_surrogate(Ht, L=L, H=H, sigmaL=sigmaL, lambda_L=lambda_L)
-    elif algo== "l2_surrogate":
+    elif algo=="l2_surrogate":
         b_supp = smooth_l2_surrogate(Ht, L=L, H=H, sigmaL=sigmaL, lambda_L=lambda_L)
     else: 
         raise "Unknown algorithm"
     return b_supp - b_inf
```

### Comparing `espm-1.0.0/espm/estimators/updates.py` & `espm-1.1.1/espm/estimators/updates.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 import numpy as np
 from espm.conf import log_shift, dicotomy_tol, sigmaL
 from sklearn.decomposition._nmf import _initialize_nmf as initialize_nmf 
 from espm.estimators.dicotomy import dichotomy_simplex, dichotomy_simplex_acc, dichotomy_simplex_projected_gradient
 
-def multiplicative_step_w(X, G, W, H, log_shift=log_shift, safe=True, l2=False, fixed_W = None):
+def multiplicative_step_w(X,
+                          G,
+                          W,
+                          H,
+                          simplex_W = False,
+                          log_shift=log_shift,
+                          safe=True,
+                          l2=False,
+                          fixed_W = None,
+                          physics_model=None,
+                          use_bregman=False):
     """
     Multiplicative step in W.
     """
-
     if safe:
         # Allow for very small negative values!
         assert(np.sum(H<-log_shift/2)==0)
         assert(np.sum(W<-log_shift/2)==0)
         assert(np.sum(G<-log_shift/2)==0)
 
         H = np.maximum(H, log_shift)
@@ -24,32 +33,57 @@
 
         GXH = G.T @ (X @ H.T)
 
         new_W = W / GGWHH * GXH
     else:
         GW = G @ W
         GWH = GW @ H
-        # Split to debug timing...
-        # term1 = G.T @ (X / (GWH + eps)) @ H.T
-        op1 = X / GWH
-        
-        mult1 = G.T @ op1
-        term1 = (mult1 @ H.T)
-        term2 = np.sum(G, axis=0,  keepdims=True).T @ np.sum(H, axis=1,  keepdims=True).T
-        new_W = W / term2 * term1
+        if use_bregman:
+            # check if G is the identity matrix
+            if np.allclose(G, np.eye(G.shape[0])):
+                sigmaR = np.sum(X, axis=1, keepdims=True)
+            else:
+                sigmaR = np.sum(X)
+            num = sigmaR * W
+            gradg = - G.T @ (X / GWH) @ H.T + np.sum(G, axis=0,  keepdims=True).T @ np.sum(H, axis=1,  keepdims=True).T
+            denum = gradg * W + sigmaR
+
+        else:
+            # Split to debug timing...
+            # term1 = G.T @ (X / (GWH + eps)) @ H.T
+            op1 = X / GWH
+            if np.any(np.isnan(op1)):
+                GWH = np.maximum(GWH, log_shift)
+                op1 = X / GWH
+            
+            mult1 = G.T @ op1
+            num = W*(mult1 @ H.T)
+            denum = np.sum(G, axis=0,  keepdims=True).T @ np.sum(H, axis=1,  keepdims=True).T
+            if simplex_W:
+                if physics_model != None:
+                    indices = physics_model.NMF_simplex()
+                    nu = dichotomy_simplex(num[indices,:], denum[indices,:], log_shift=log_shift, tol=dicotomy_tol)
+                    denum[indices,:] = denum[indices,:] + nu
+                else : 
+                    nu = dichotomy_simplex(num, denum, log_shift=log_shift, tol=dicotomy_tol)
+                    denum = denum + nu
+
+        new_W = num / denum
     
     new_W = np.maximum(new_W, log_shift)
     
+    # TODO: exclude the fixed values in the update process. It is not straightforward
     if fixed_W is not None: 
         new_W[fixed_W >= 0] = fixed_W[fixed_W >=0]
     return new_W
 
 
 
-def multiplicative_step_h(X, G, W, H, force_simplex=True, mu=0, log_shift=log_shift, epsilon_reg=1, safe=True, dicotomy_tol=dicotomy_tol, lambda_L=0, L=None, l2=False, sigmaL=sigmaL, fixed_H = None):
+
+def multiplicative_step_h(X, G, W, H, simplex_H =False, mu=0, log_shift=log_shift, epsilon_reg=1, safe=True, dicotomy_tol=dicotomy_tol, lambda_L=0, L=None, l2=False, sigmaL=sigmaL, fixed_H = None, use_bregman=False):
     """
     Multiplicative step in A.
     The main terms are calculated first.
     With mu_sparse = 0, the steps in A are calculated once. For mu_sparse != 0, the steps 
     in A are calculated first with particle regularization. Then only the entries allowed 
     by the mask are calculaed, without particle regularization. Note that mu can be passed
     as a vector to regularize the different phase of A differently.
@@ -78,28 +112,38 @@
         else:
             assert (mu==0).all()
         WGGW = GW.T @ GW
         WGX = GW.T @ X
         num = WGX
         denum = WGGW @ H
     else:
-        GWH = GW @ H
-        num = GW.T @ (X / GWH)
-        denum = np.sum(GW, axis=0, keepdims=True).T 
-
-    if not(np.isscalar(mu) and mu==0):
-        if len(np.shape(mu))==1:
-            mu = np.expand_dims(mu, axis=1)
-        denum = denum + mu / (H + epsilon_reg)
-    if not(lambda_L==0):
-        maxH = np.max(H, axis=1, keepdims=True)
-        num = num + lambda_L * sigmaL * maxH
-        denum = denum + lambda_L * sigmaL * maxH + lambda_L * HL 
+        if use_bregman:
+            GWH = GW @ H
+            sigmaR = np.sum(X, axis=0, keepdims=True)
+            num = sigmaR / H
+            gradg = - GW.T @ (X / GWH) +  np.sum(GW, axis=0,  keepdims=True).T
+            denum = gradg + sigmaR / H
+        else:
+            GWH = GW @ H
+            num = GW.T @ (X / GWH)
+            if np.any(np.isnan(num)):
+                GWH = np.maximum(GWH, log_shift)
+                num = GW.T @ (X / GWH)
+            denum = np.sum(GW, axis=0, keepdims=True).T 
+
+        if not(np.isscalar(mu) and mu==0):
+            if len(np.shape(mu))==1:
+                mu = np.expand_dims(mu, axis=1)
+            denum = denum + mu / (H + epsilon_reg)
+        if not(lambda_L==0):
+            maxH = np.max(H, axis=1, keepdims=True)
+            num = num + lambda_L * sigmaL * maxH
+            denum = denum + lambda_L * sigmaL * maxH + lambda_L * HL 
     num = H * num
-    if force_simplex:
+    if simplex_H:
         nu = dichotomy_simplex(num, denum, log_shift=log_shift, tol=dicotomy_tol)
     else:
         nu = 0
     if safe:
         assert np.sum(denum<0)==0
         assert np.sum(num<0)==0
 
@@ -108,15 +152,15 @@
 
     if fixed_H is not None: 
         new_H[fixed_H >= 0] = fixed_H[fixed_H >= 0]
     return new_H
 
 
 
-def initialize_algorithms(X, G, W, H, n_components, init, random_state, force_simplex, logshift=log_shift):
+def initialize_algorithms(X, G, W, H, n_components, init, random_state, simplex_H, simplex_W, logshift=log_shift, physics_model = None):
     # Handle initialization
 
     if G is None : 
         skip_second = True
         # G = sparse.diags(np.ones(X.shape[0]).astype(X.dtype))        
         G = np.diag(np.ones(X.shape[0]).astype(X.dtype))
 
@@ -129,35 +173,50 @@
     else:
         skip_second = False
 
     if W is None:
         if H is None:
             D, H = initialize_nmf(X, n_components=n_components, init=init, random_state=random_state)
             # D, A = u.rescaled_DA(D,A)
-            if force_simplex:
+            if simplex_H:
+                H = np.nan_to_num(H, nan = 1.0/H.shape[0])
                 scale = np.sum(H, axis=0, keepdims=True)
-                H = np.nan_to_num(H/scale, nan = 1.0/H.shape[0] )
-        D = np.abs(np.linalg.lstsq(H.T, X.T,rcond=None)[0].T)
+                H = H/scale
+                
+                # D = np.abs(np.linalg.lstsq(H.T, X.T,rcond=None)[0].T)
+                D = D*np.mean(scale)
+        else:
+            D = np.abs(np.linalg.lstsq(H.T, X.T,rcond=None)[0].T)
         if skip_second:
             W = D
         else:
+            if physics_model != None: 
             # [np.where(G[:,:-2].sum(axis=1)<(np.max(G[:,:-2].sum(axis=1))*0.001))[0],:]
             # Divide in two parts the initial fitting, otherwise the bremsstrahlung (which has a low intensity) tends to be poorly learned
             # First fit the caracteristic Xrays, then subtract that contribution to obtain a rough estimate of the bremsstralung parameters
-            Wcarac = (np.linalg.lstsq(G[:,:-2],D,rcond = None)[0]).clip(min = 0)
-            filter = np.where(np.mean(G[:,:-2],axis=1)<(np.max(np.mean(G[:,:-2],axis=1))*0.001))[0]
-            Wbrem = (np.linalg.lstsq(G[:,-2:][filter,:],D[filter,:],rcond = None)[0]).clip(min = 0)
-            # Wbrem = (np.linalg.lstsq(G[:,-2:],D - G[:,:-2]@Wcarac,rcond = None)[0]).clip(min = 0)
-            W = np.vstack((Wcarac,Wbrem))
+                W = physics_model.NMF_initialize_W(D)
+                # Wbrem = (np.linalg.lstsq(G[:,-2:],D - G[:,:-2]@Wcarac,rcond = None)[0]).clip(min = 0)
+                if simplex_W:
+                    indices = physics_model.NMF_simplex()
+                    W = np.nan_to_num(W, nan = 1.0/W.shape[0])
+                    scale = np.sum(W[indices,:], axis=0, keepdims=True)
+                    W[indices,:] = W[indices,:]/scale
             # P = np.abs(np.linalg.lstsq(G, D,rcond=None)[0])
+            else : 
+                W = np.abs(np.linalg.lstsq(G, D,rcond=None)[0])
+
+                if simplex_W:
+                    W = np.nan_to_num(W, nan = 1.0/W.shape[0])
+                    scale = np.sum(W, axis=0, keepdims=True)
+                    W = W/scale
 
     elif H is None:
         D = G @ W
         H = np.abs(np.linalg.lstsq(D, X, rcond=None)[0])
-        if force_simplex:
+        if simplex_H:
             scale = np.sum(H, axis=0, keepdims=True)
             H = H/scale
 
     W = np.maximum(W, log_shift)
     H = np.maximum(H, log_shift)
 
     return G, W, H
@@ -165,15 +224,15 @@
 def update_q(D, H, log_shift=log_shift):
     """Perform a Q step."""
     Htmp = np.expand_dims(H.T, axis=0)
     Dtmp = np.expand_dims(D, axis=1)
     Ntmp = np.expand_dims(D @ H, axis=2) 
     return Htmp * (Dtmp / (Ntmp+log_shift))
    
-def multiplicative_step_wq(X, G, W, H, log_shift=log_shift, safe=True):
+def multiplicative_step_wq(X, G, W, H, simplex_W = True, log_shift=log_shift, safe=True, physics_model = None):
     """
     Multiplicative step in W using the WQ technique.
 
     This function does exactly the same as `multiplicative_step_w` and is probably slower.
     """
 
     if safe:
@@ -186,17 +245,25 @@
     Q = update_q(GW, H, log_shift=log_shift)
 
     XQ = np.sum(np.expand_dims(X, axis=2) * Q, axis=1)
 
     term1 = G.T @ (XQ / (GW + log_shift)) 
 
     term2 = np.sum(G, axis=0,  keepdims=True).T @ np.sum(H, axis=1,  keepdims=True).T
+    if simplex_W :
+        if physics_model != None:
+            indices = physics_model.NMF_simplex()
+            nu = dichotomy_simplex(term1[indices,:], term2[indices,:], log_shift=log_shift, tol=dicotomy_tol)
+            term2[indices,:] = term2[indices,:] + nu
+        else : 
+            nu = dichotomy_simplex(term1, term2, log_shift=log_shift, tol=dicotomy_tol)
+            term2 = term2 + nu
     return W / term2 * term1
 
-def multiplicative_step_hq(X, G, W, H, force_simplex=True, log_shift=log_shift, safe=True, dicotomy_tol=dicotomy_tol, lambda_L=0, L=None, sigmaL=sigmaL, fixed_H = None):
+def multiplicative_step_hq(X, G, W, H, simplex_H=True, log_shift=log_shift, safe=True, dicotomy_tol=dicotomy_tol, lambda_L=0, L=None, sigmaL=sigmaL, fixed_H = None):
     """
     Multiplicative step in H.
     """
     if not lambda_L==0:
         if L is None:
             raise ValueError("Please provide the laplacian")
 
@@ -211,20 +278,20 @@
 
     minus_c = H * (GW.T @ (X / (GWH+log_shift)))
 
     b = np.sum(GW, axis=0, keepdims=True).T 
     if not lambda_L==0 :
         b = b + lambda_L * H @ L - lambda_L * sigmaL  * H 
         a = lambda_L * sigmaL
-        if force_simplex:
+        if simplex_H:
             nu = dichotomy_simplex_acc(a, b, minus_c, log_shift=log_shift, tol=dicotomy_tol)
             b = b + nu
         new_H = (-b + np.sqrt(b**2 + 4* a *minus_c)) / (2*a)
     else: # We recover the classic case: multiplicative_step_a
-        if force_simplex:
+        if simplex_H:
             nu = dichotomy_simplex(minus_c, b, log_shift=log_shift, tol=dicotomy_tol)
             b = b + nu
         new_H = minus_c / b
 
     # Add the shift...
     new_H = np.maximum(new_H, log_shift)
 
@@ -269,15 +336,15 @@
         grad += mu / (H + epsilon_reg)
 
     if not(lambda_L==0):
         grad += (lambda_L * L @ H.T).T
 
     return grad
 # 
-def proj_grad_step_w(X, G, W, H, gamma, log_shift=log_shift, safe=True, l2=False, fixed_W = None):
+def proj_grad_step_w(X, G, W, H, gamma, simplex_W = True, log_shift=log_shift, safe=True, l2=False, fixed_W = None):
     """Projected gradient step for the variable W."""
 
     if safe:
         H = np.maximum(H, log_shift)
         W = np.maximum(W, log_shift)
 
     grad = gradW(X, G, W, H, log_shift=log_shift, safe=safe, l2=l2)
@@ -285,29 +352,32 @@
     # gradient step
     new_W = W - 1/gamma * grad
     # projection
     new_W = np.maximum(new_W, log_shift)
 
     if fixed_W is not None: 
         new_W[fixed_W >= 0] = fixed_W[fixed_W >=0]
+
+    if simplex_W : 
+        raise NotImplementedError("Simplex constraint not implemented for W using the projected gradient method")
     return new_W
 
-def proj_grad_step_h(X, G, W, H, gamma, force_simplex=True, mu=0, log_shift=log_shift, epsilon_reg=1, safe=True, dicotomy_tol=dicotomy_tol, lambda_L=0, L=None, l2=False, fixed_H = None):
+def proj_grad_step_h(X, G, W, H, gamma, simplex_H=True, mu=0, log_shift=log_shift, epsilon_reg=1, safe=True, dicotomy_tol=dicotomy_tol, lambda_L=0, L=None, l2=False, fixed_H = None):
     """Projected gradient step for the variable H."""
 
     if safe:
         H = np.maximum(H, log_shift)
         W = np.maximum(W, log_shift)
 
     # gradient step
     grad = gradH(X, G, W, H, log_shift=log_shift, safe=safe, mu=mu, epsilon_reg=epsilon_reg, lambda_L=lambda_L, L=L, l2=l2)
     new_H = H - 1/gamma * grad
 
     # Dichotomy
-    if force_simplex:
+    if simplex_H:
         nu = dichotomy_simplex_projected_gradient(new_H, log_shift=log_shift, tol=dicotomy_tol)
     else:
         nu = 0
 
     # projection
     new_H = np.maximum(new_H + nu, log_shift)
```

### Comparing `espm-1.0.0/espm/measures.py` & `espm-1.1.1/espm/measures.py`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/espm/models/EDXS_function.py` & `espm-1.1.1/espm/models/EDXS_function.py`

 * *Files 3% similar despite different names*

```diff
@@ -221,15 +221,14 @@
 
     Notes
     -----
     * When an empty dict is provided. The continuum X-rays are set to 0. This is useful to perform calculations without the bremsstrahlung for example.
     * For an example structure of the params_dict parameter, check the DEFAULT_EDXS_PARAMS espm.conf.
     * For a custom detection efficiency, check the spectrum fit notebook.
     """
-
     if len(params_dict) == 0 : 
         return 0*x
     
     B = lifshin_bremsstrahlung(
             x,
             b0 = b0,
             b1 = b1,
@@ -283,52 +282,53 @@
         E0 = E0
     )
 
     B = np.vstack((B0,B1)).T
     
     return B
 
-@number_to_symbol_list    
-def elts_dict_from_W (part_W,*,elements = []) : 
-    r"""
-    Create a dictionnary of the elemental concentration from a fitted W. It useful to recompute absorption during the our custom NMF calculations.
-
-    Parameters
-    ----------
-    part_W : 
-        :np.array 2D: W matrix output from the NMF calculation. It only makes sense when the NMF decomposition if performed with G.
-    elements : 
-        :list: List of elements as atomic number or symbol.
-
-    Returns
-    -------
-    elements_dictionnary : 
-        :dict: Dictionnary containing the concentration associated to each chemical element of the problem.
-    
-    Examples
-    --------
-    >>> import numpy as np
-    >>> from espm.models.EDXS_function import elts_dict_from_W
-    >>> W = np.ones((4,3))
-    >>> elts = ["Si","Ca","O","C"]
-    >>> elts_dict_from_W(W,elements = elts)
-        {"Si" : 0.25, "Ca" : 0.25, "O" : 0.25, "C" : 0.25}
-
-    Notes
-    -----
-    This function should maybe move to another part of espm.
-    """
-    norm_P = np.mean(part_W / part_W.sum(axis = 0),axis=1)
-    elements_dict = {}
-    with open(SYMBOLS_PERIODIC_TABLE,"r") as f : 
-        SPT = json.load(f)["table"]
-    for i,elt in enumerate(elements) :
-        elements_dict[elt] = norm_P[i] # * SPT[elt]["atomic_mass"]
-    factor =  sum(elements_dict.values())
-    return {key:elements_dict[key]/factor for key in elements_dict}
+# @number_to_symbol_list    
+# def elts_dict_from_W (part_W,*,elements = []) : 
+#     r"""
+#     Create a dictionnary of the elemental concentration from a fitted W. It useful to recompute absorption during the our custom NMF calculations.
+
+#     Parameters
+#     ----------
+#     part_W : 
+#         :np.array 2D: W matrix output from the NMF calculation. It only makes sense when the NMF decomposition if performed with G.
+#     elements : 
+#         :list: List of elements as atomic number or symbol.
+
+#     Returns
+#     -------
+#     elements_dictionnary : 
+#         :dict: Dictionnary containing the concentration associated to each chemical element of the problem.
+    
+#     Examples
+#     --------
+#     >>> import numpy as np
+#     >>> from espm.models.EDXS_function import elts_dict_from_W
+#     >>> W = np.ones((4,3))
+#     >>> elts = ["Si","Ca","O","C"]
+#     >>> elts_dict_from_W(W,elements = elts)
+#         {"Si" : 0.25, "Ca" : 0.25, "O" : 0.25, "C" : 0.25}
+
+#     Notes
+#     -----
+#     This function should maybe move to another part of espm.
+#     """
+#     mask_zeros = np.sum(part_W,axis=0) != 0
+#     norm_P = np.mean(part_W[:,mask_zeros] / part_W[:,mask_zeros].sum(axis = 0),axis=1)
+#     elements_dict = {}
+#     #with open(SYMBOLS_PERIODIC_TABLE,"r") as f : 
+#     #    SPT = json.load(f)["table"]
+#     for i,elt in enumerate(elements) :
+#         elements_dict[elt] = norm_P[i] # * SPT[elt]["atomic_mass"]
+#     factor =  sum(elements_dict.values())
+#     return {key:elements_dict[key]/factor for key in elements_dict}
 
 def elts_dict_from_dict_list (dict_list) : 
     r"""
     Create a single dictionnary of the elemental concentration from a list of dictionnary containing chemical compositions. The new dictionnary corresponds to the average chemical composition of the list.
 
     Parameters
     ----------
@@ -379,39 +379,9 @@
     >>> dicts = [{"Si" : 1.0, "C" : 0.5, "O" : 0.5},{"Ca" : 1.0, "K" : 2.0},{"O" : 1.0, "Si" : 0.5},{"C" : 1.0}] 
     >>> elts_list_from_dict_list(dicts)
         ["Si","Ca","O","C","K"]
     """ 
     unique_elts_dict = sum((Counter(x) for x in dict_list),Counter())
     return list(unique_elts_dict.keys())
 
-def update_bremsstrahlung (G,part_W,model,elements_list) : 
-    r"""
-    Update the continuum X-rays part of the G matrix with the current average chemical composition.
-
-    Parameters
-    ----------
-    G : 
-        :np.array 2D: EDXS modelling matrix.
-    part_W : 
-        :np.array 2D: Learned chemical concentrations.
-    model : 
-        :espm.models.EDXS: EDXS model.
-    elements_list :
-        :list: List of elements as atomic number or symbol.
-    
-    Returns
-    -------
-    new_G : 
-        :np.array 2D: New G matrix with updated continuum X-rays models.
-
-    Notes
-    -----
-    This function should maybe move to another part of espm.
-    """
-    elts = elts_dict_from_W(part_W,elements = elements_list)
-    B = G_bremsstrahlung(model.x,model.E0,model.params_dict,elements_dict=elts)
-    new_G = G.copy()
-    new_G[:,-2:] = B/model.norm[0][-2:]
-    return new_G
-
```

### Comparing `espm-1.0.0/espm/models/absorption_edxs.py` & `espm-1.1.1/espm/models/absorption_edxs.py`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/espm/models/base.py` & `espm-1.1.1/espm/models/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -124,14 +124,15 @@
         -------
         None
 
         """
 
         if self.phases is not None :
             return
+        np.random.seed(seed=self.seed)
         Wdot = np.abs(np.random.laplace(size=[self.C, self.K]))
         self.Wdot = Wdot / np.mean(Wdot)/self.L
 
         self.generate_g_matr()
         self.phases = self.G @ self.Wdot
         
     
@@ -146,15 +147,15 @@
             self.db_dict = {}
             self.db_mdata = {}
         else :
             self.db_dict = self.extract_DB(db_name)
             self.db_mdata = self.extract_DB_mdata(db_name)
         self.bkgd_in_G = False
         self.spectrum = np.zeros_like(self.x)
-        self.G = np.diag(np.ones_like(self.x))
+        self.G = None
         self.phases = None
         self.E0 = E0
 
 
     def extract_DB (self,db_name) :
         r"""
         Read the cross-sections from the database
@@ -208,8 +209,57 @@
 
         Returns
         -------
         energy scale
             :np.array 1D: Linear energy scale based on the given parameters of shape (e_size,)
         """
         return np.linspace(e_offset,e_offset+e_size*e_scale,num=e_size)
+    
+    @abstractmethod
+    def NMF_initialize_W (self, D) :
+        """
+        Function to be called when initializing the NMF optimization. It returns the matrices W.
+        The basic implementation is to return the pseudo-inverse of the matrix G.
+
+        Parameters
+        ----------
+        D : 
+            :np.array 2D: scikit-learn initialization matrix. It should have the shape (n_features, n_components).
+
+        Returns
+        -------
+        W :
+            :np.array 2D: The initialized matrix W of shape (n_G, n_components)
+        """
+        W = np.abs(np.linalg.lstsq(self.G, D,rcond=None)[0])
+        return W
+
+    @abstractmethod
+    def NMF_update (self, W = None) :
+        """
+        Function to be called when during the NMF optimization. It returns the matrix G, updated if necessary. It should be run in between each W iteration.
+        You do not need to implement it, if you do not need to update the matrix G during the optimization.
+
+        Parameters
+        ----------
+        W : 
+            :np.array 2D: The part of the matrix W that is required to update the matrix G.
+
+        Returns
+        -------
+        G :
+            :np.array 2D: The updated matrix G 
+        """
+        return self.G
+
+    @abstractmethod
+    def NMF_simplex (self) :
+        """
+        Function to be called when using the simplex constraint in the ESpM-NMF. Its purpose is to return the indices of the matrix W that will be considered to apply the simplex constraint.
+
+        Returns : 
+        --------
+        indices :
+            :np.array 1D: Indices to be considered to apply the simplex constraint
+        """
+        return np.arange(self.G.shape[1])
```

### Comparing `espm-1.0.0/espm/models/generate_EDXS_phases.py` & `espm-1.1.1/espm/models/generate_EDXS_phases.py`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/espm/spectrum_fitting.py` & `espm-1.1.1/espm/spectrum_fitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,17 @@
         sum_boola+=elt.astype(bool)
     
     
     return part_x, part_y, sum_boola
 
 def residual(pars,x,data = None) : 
     kwargs = params_to_ndict(pars)
-    kwargs["params_dict"] = arg_helper(kwargs["params_dict"],DEFAULT_EDXS_PARAMS)
+    kwargs["params_dict"] = arg_helper(kwargs["params_dict"],DEFAULT_EDXS_PARAMS['params_dict'])
     
-    model = ef.continuum_xrays(x,**kwargs)    
+    model = ef.continuum_xrays(x,**kwargs)   
     
     if data is None : 
         return model
     
     return model - data
 
 def params_to_ndict(params) :
```

### Comparing `espm-1.0.0/espm/tables/100keV_xrays.json` & `espm-1.1.1/espm/tables/100keV_xrays.json`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/espm/tables/200keV_xrays.json` & `espm-1.1.1/espm/tables/200keV_xrays.json`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/espm/tables/300keV_xrays.json` & `espm-1.1.1/espm/tables/300keV_xrays.json`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/espm/tables/SDD_efficiency.txt` & `espm-1.1.1/espm/tables/SDD_efficiency.txt`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/espm/tables/default_xrays.json` & `espm-1.1.1/espm/tables/default_xrays.json`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/espm/tables/periodic_table_number.json` & `espm-1.1.1/espm/tables/periodic_table_number.json`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/espm/tables/periodic_table_symbols.json` & `espm-1.1.1/espm/tables/periodic_table_symbols.json`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/espm/tables/siegbahn_to_iupac.json` & `espm-1.1.1/espm/tables/siegbahn_to_iupac.json`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/espm/tables_utils.py` & `espm-1.1.1/espm/tables_utils.py`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/espm/tests/test_EDXS.py` & `espm-1.1.1/espm/tests/test_EDXS.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from espm.models.absorption_edxs import det_efficiency, absorption_correction
 from espm.models.generate_EDXS_phases import generate_elts_dict
 import numpy as np
 import espm.models.EDXS_function as ef
 from espm.models import EDXS
 from espm.models.EDXS_function import lifshin_bremsstrahlung, lifshin_bremsstrahlung_b0, lifshin_bremsstrahlung_b1
+import hyperspy.api as hs
 
 x = np.linspace(0.2,19,num = 2000)
 det_dict = {
     "detection" : {
         "thickness" : 450e-3,
         "density" : 2.5
     },
@@ -39,14 +40,24 @@
                 "toa" : 35,
                 "density" : 3.12
             },
             "Det" : det_dict
         }
     }
 
+def create_data()  : 
+    a = np.random.rand(50,70,100)
+    s = hs.signals.Signal1D(a)
+    s.axes_manager[-1].offset = 0.2
+    s.axes_manager[-1].scale = 0.1
+    s.set_signal_type("EDS_espm")
+    s.set_analysis_parameters()
+    s.set_elements(elements = ["Si","O","Fe","Ca"])
+    return s
+
 def test_lifshin_bremsstrahlung () : 
     E0 = 200
     x = np.linspace(0.2,E0-0.1, num = 2000 )
     for i in range(10) : 
         b0 = np.random.rand()
         b1 = np.random.rand()
         y0 = lifshin_bremsstrahlung_b0(x,b0,E0)
@@ -66,73 +77,116 @@
 def test_absorption () : 
     elts = generate_elts_dict(42)
     abs_corr = absorption_correction(x,thickness = 1e-4, toa = 35, density = 5, elements_dict=elts)
 
     np.testing.assert_array_less(1e-30,abs_corr)
     np.testing.assert_array_less(abs_corr,1.0)
 
-def test_elts_dict_from_W () : 
-    # elements_mass = [28.085,40.0784,15.999,30.9737619985,12.011]
-    part_W = np.random.rand(5,3)
-    avg_W = part_W.sum(axis=1)/3
-    # weighted_W= [avg_W[i]*elt_mass for i,elt_mass in enumerate(elements_mass)]
-    norm_W = avg_W/np.sum(avg_W)
-    elements_list = ["Si","Ca", "O", "P", "C"]
-
-    result = ef.elts_dict_from_W(part_W, elements = elements_list)
-    for i,key in enumerate(result) : 
-        np.testing.assert_allclose(result[key],norm_W[i],rtol = 1e-1)
-
 def test_elts_dict_from_dict_list () : 
     dict_list = [{"chou" : 1, "carottes" : 2, "navet" : 3}, {"chou" : 2, "oignons" : 3, "navet" : 3}, {"orange" : 6, "citron" : 4, "poireau" : 8}]
     unique_dict = ef.elts_dict_from_dict_list(dict_list)
     sum_elts = 32
     assert unique_dict == {"chou" : 3/sum_elts, "carottes" : 2/sum_elts, "navet" : 6/sum_elts, "orange" : 6/sum_elts, "citron" : 4/sum_elts, "poireau" : 8/sum_elts, "oignons" : 3/sum_elts}
 
 def test_continuum_xrays () : 
     E0 = 200
     b0 = np.random.uniform(0.0,50.0)
     b1 = np.random.uniform(0.0, 50.0)
     cont_x = ef.continuum_xrays(x,model_parameters["params_dict"],b0= b0, b1 = b1, E0 = E0,elements_dict = {"Si" : 1.0, "C" : 0.2, "Bi" : 3.2})
     
     np.testing.assert_array_less(1e-30,cont_x)
 
-def test_update_bremsstrahlung () : 
-    elts_list = ["Si", "Co", "Cu","O"]
-    part_P = np.ones((4,1))/4
-    model = EDXS(**model_parameters)
-    model.generate_g_matr(elements=elts_list)
-    G = model.G
-    new_G = ef.update_bremsstrahlung(G, part_P, model, elts_list)
+def test_get_elements () :
+    s = create_data()
+    s.build_G(elements_dict ={'Fe' : 3.0})
+    nelts = []
+    for i in s.model.get_elements() :
+        nelts.append(i)
+    assert nelts == ['14', '8', '26', '20'] 
+        
+def test_carac_x_span () :
+    # TODO : Find a way to implement the test of this function
+    pass
+
+def test_NMF_initialize_W () : 
+    model = EDXS(**model_parameters)
+    model.generate_g_matr(g_type = "bremsstrahlung", elements = ["Na", "Sr", "Ge", "Nb"], elements_dict={})
+    D = np.random.rand(1900,2)
+    W = model.NMF_initialize_W(D)
+    assert W.shape == (6,2)
+
+    model = EDXS(**model_parameters)
+    model.generate_g_matr(g_type = "no_brstlg", elements = ["Na", "Sr", "Ge", "Nb"], elements_dict={'Nb' : 3.0})
+    D = np.random.rand(1900,4)
+    W = model.NMF_initialize_W(D)
+    assert W.shape == (5,4)
 
-    assert G.shape == new_G.shape
-    np.testing.assert_allclose(G[:,:-2],new_G[:,:-2])
+    model = EDXS(**model_parameters)
+    model.generate_g_matr(g_type = "identity", elements = ["Na", "Sr", "Ge", "Nb"], elements_dict={})
+    with np.testing.assert_raises(ValueError) : 
+        D = np.random.rand(1900,4)
+        W = model.NMF_initialize_W(D)
 
+def test_NMF_simplex () :
+    model = EDXS(**model_parameters)
+    model.generate_g_matr(g_type = "bremsstrahlung", elements = ["Na", "Sr", "Ge", "Nb"], elements_dict={})
+    inds = model.NMF_simplex()
+    assert inds == [0,1,2,3]
+
+    model = EDXS(**model_parameters)
+    model.generate_g_matr(g_type = "no_brstlg", elements = ["Na", "Sr", "Ge", "Nb"], elements_dict={'Nb' : 3.0})
+    inds = model.NMF_simplex()
+    assert inds == [0,1,2,4]
+
+def test_NMF_update () : 
+    model = EDXS(**model_parameters)
+    model.generate_g_matr(g_type = "no_brstlg", elements = ["Na", "Sr", "Ge", "Nb"], elements_dict={})
+    temp_G = model.G.copy()
+    np.testing.assert_array_equal(model.NMF_update(), temp_G)
+    np.testing.assert_array_equal(model.NMF_update(np.random.rand(10,10)), temp_G)
+
+    model = EDXS(**model_parameters)
+    model.generate_g_matr(g_type = "bremsstrahlung", elements = ["Na", "Sr", "Ge", "Nb"], elements_dict={})
+    temp_G = model.G.copy()
+    np.testing.assert_array_equal(model.NMF_update(), temp_G)
+    assert model.NMF_update(np.random.rand(6,10)).shape == model.G.shape
+    with np.testing.assert_raises(AssertionError):
+        np.testing.assert_array_equal(model.NMF_update(np.random.rand(6,10))[:,-2:], temp_G[:,-2:])
+    
 def test_generate_g_matr () : 
     model1 = EDXS(**model_parameters)
     model2 = EDXS(**model_parameters)
     model3 = EDXS(**model_parameters)
+    model4 = EDXS(**model_parameters)
     size = model_parameters["e_size"]
     elts_list = ["Na", "Sr", "Ge", "Nb"]
-    model1.generate_g_matr(g_type = "bremsstrahlung", elements = elts_list)
+    model1.generate_g_matr(g_type = "bremsstrahlung", elements = elts_list, elements_dict={})
     G_brem = model1.G
-    model2.generate_g_matr(g_type = "identity", elements = elts_list)
+    model2.generate_g_matr(g_type = "identity", elements = elts_list, elements_dict={})
     G_id = model2.G
-    model3.generate_g_matr(g_type = "no_brstlg", elements = elts_list)
+    model3.generate_g_matr(g_type = "no_brstlg", elements = elts_list, elements_dict={})
     G_no_brstlg = model3.G
+    model4.generate_g_matr(g_type = "bremsstrahlung", elements = elts_list, elements_dict={'Ge' : 3.0})
+    G_brem_ge = model4.G
 
     assert G_brem.shape == (size, 6)
     assert G_no_brstlg.shape == (size, 4)
+    assert G_brem_ge.shape == (size, 7)
 
     assert G_id is None
     np.testing.assert_allclose(G_brem[:,:-2], G_no_brstlg)
+    np.testing.assert_allclose((G_brem_ge[:,3] + G_brem_ge[:,2])*model4.norm[0,0], G_brem[:,2]*model1.norm[0,0])
 
     # np.testing.assert_array_less(-1e-30, G_id)
     np.testing.assert_array_less(-1e-30, G_brem)
     np.testing.assert_array_less(-1e-30, G_no_brstlg)
+    assert(model1.model_elts == ['11', '38', '32', '41'])
+    assert(model2.model_elts == [])
+    assert(model3.model_elts == ['11', '38', '32', '41'])
+    assert(model4.model_elts == ['11', '38', '32_lo', '32_hi', '41'])
 
 def test_G_bremsstrahlung() : 
     model = EDXS(**model_parameters)
     size = model_parameters["e_size"]
     elts_dict = {"V" : 0.3, "Ti" : 0.1, "Hf" : 0.05, "Pb" : 0.55 }
     B = ef.G_bremsstrahlung(model.x, model.E0, model.params_dict, elements_dict=elts_dict)
```

### Comparing `espm-1.0.0/espm/tests/test_datasets.py` & `espm-1.1.1/espm/tests/test_datasets.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 from espm.models import EDXS
 from espm.models.generate_EDXS_phases import generate_brem_params, generate_random_phases, unique_elts
 import os
 import hyperspy.api as hs
 import shutil
 from espm.conf import DATASETS_PATH
 from pathlib import Path
-from hyperspy.misc.eds.utils import take_off_angle
+from exspy.misc.eds.utils import take_off_angle
 import espm.weights.generate_weights as wts
 from espm.weights.generate_weights import generate_weights
 from espm.models.EDXS_function import elts_list_from_dict_list
 from espm.models.generate_EDXS_phases import generate_modular_phases
+from espm.estimators import SmoothNMF
 
 elts_dicts = [{"Fe" : 0.54860348,
                "Pt" : 0.38286879,
                "Mo" : 0.03166235,
                "O" : 0.03686538},
                {"Ca" : 0.54860348,
                 "Si" : 0.38286879,
@@ -46,28 +47,28 @@
                         "thickness" : 100.0e-7,
                         "toa" : 35,
                         "density" : 5
                     },
                     "Det" : "SDD_efficiency.txt"
                 }}  
 
-misc_params = {"N" : 40,
+misc_params = {"N" : 400,
                 "densities" : [1.3,1.6,1.9],
                 "data_folder" : "test_gen_data",
                 "seed" : 42,
                 "shape_2d" : (100,120),
                 "model" : "EDXS"}
 
 elements = elts_list_from_dict_list(elts_dicts)
 
 def test_generate():
 
     # Generate the phases
     model = EDXS(**model_params)
-    model.generate_g_matr(g_type = "bremsstrahlung", elements=elements)
+    model.generate_g_matr(g_type = "bremsstrahlung", elements=elements, elements_dict = {})
     phases1 = generate_modular_phases(elts_dicts = elts_dicts, brstlg_pars =  brstlg_pars, scales = scales, model_params = model_params)
     G = model.G
     n_phases = len(elts_dicts)
     maps = generate_weights(weight_type='sphere', shape_2d= misc_params["shape_2d"], n_phases=n_phases, seed=misc_params["seed"], radius = 15)
     densities = np.array(misc_params["densities"])
     spim_sample = generate_spim_sample(phases1,maps,model_params=model_params, misc_params=misc_params)
     spim = spim_sample["X"]
@@ -85,15 +86,15 @@
     if os.path.exists("test.hspy"):
         os.remove("test.hspy")
     filename = "test.hspy"
     hspy_spim = sample_to_EDS_espm(spim_sample,elements=elements)
     hspy_spim.save(filename)
     si = hs.load(filename)
     si.build_G(problem_type = "bremsstrahlung")
-    G = si.G()
+    G = si.G
     phases, maps = si.phases, si.maps_2d
     # weights = weights.reshape((100,120,n_phases))
     X = si.data
     W = np.linalg.lstsq(G,X.sum(axis = (0,1)),rcond = None)[0]
     
     assert phases.shape == (1900, 3)
     assert maps.shape == (100,120,3)
@@ -226,14 +227,39 @@
 #     model = EDXS(**DEFAULT_SYNTHETIC_DATA_DICT["model_parameters"])
 #     model.generate_phases(dicts)
 #     np.testing.assert_almost_equal(model.phases,phases)
 
 #     unique_list = unique_elts(dicts)
 #     assert len(unique_list) == len(set(unique_list))
 
+def test_decomposition () :
+    if os.path.exists(str(DATASETS_PATH / Path(misc_params["data_folder"]))):
+        shutil.rmtree(str(DATASETS_PATH / Path(misc_params["data_folder"])))
+
+    phases1 = generate_modular_phases(elts_dicts = elts_dicts, brstlg_pars =  brstlg_pars, scales = scales, model_params = model_params)
+    maps = generate_weights(weight_type='sphere', shape_2d= misc_params["shape_2d"], n_phases=len(elts_dicts), seed=misc_params["seed"], radius = 15)
+    generate_dataset(base_seed=misc_params['seed'],
+                    sample_number=2,
+                    model_params = model_params,
+                    misc_params = misc_params,
+                    phases = phases1,
+                    weights = maps,
+                    elements = elements)
+
+    gen_folder = DATASETS_PATH / Path(misc_params["data_folder"])
+    gen_si = hs.load(gen_folder / Path("sample_0.hspy"))
+    gen_si.change_dtype("float64")
+    gen_si.build_G()
+    est = SmoothNMF(n_components=3, G = gen_si.model, hspy_comp = True)
+    gen_si.decomposition(algorithm = est)
+    np.testing.assert_allclose((est.G_@est.W_@est.H_).sum(axis = 1), gen_si.X.sum(axis = 1), rtol = 0.5)
+    np.testing.assert_allclose(est.W_[:-2,:].sum(axis = 0), np.ones(3), rtol = 0.1)
+
+    shutil.rmtree(str(gen_folder))
+
 def test_spim () : 
 
     if os.path.exists(str(DATASETS_PATH / Path(misc_params["data_folder"]))):
         shutil.rmtree(str(DATASETS_PATH / Path(misc_params["data_folder"])))
     phases1 = generate_modular_phases(elts_dicts = elts_dicts, brstlg_pars =  brstlg_pars, scales = scales, model_params = model_params)
     maps = generate_weights(weight_type='sphere', shape_2d= misc_params["shape_2d"], n_phases=len(elts_dicts), seed=misc_params["seed"], radius = 15)
     generate_dataset(base_seed=misc_params['seed'],
@@ -250,30 +276,37 @@
 
     mod_pars = get_metadata(gen_si)
     # mod_pars["params_dict"]["Abs"]["atomic_fraction"] = False
 
     assert model_params == mod_pars
 
     shape = gen_si.shape_2d
+    gen_si = hs.load(gen_folder / Path("sample_0.hspy"))
     gen_si.build_G(problem_type = "identity")
     assert shape == (100,120)
     assert gen_si.G is None
-    gen_si.build_G(problem_type = "no_brstlg",reference_elt = {})
+    
+    gen_si = hs.load(gen_folder / Path("sample_0.hspy"))
+    gen_si.build_G(problem_type = "no_brstlg",elements_dict = {})
     assert gen_si.G.shape == (1900, 8)
-    gen_si.build_G(problem_type = "bremsstrahlung",reference_elt = {})
-    assert callable(gen_si.G)
-    assert gen_si.G().shape == (1900, 10)
-    Xflat = gen_si.X
     
+    gen_si = hs.load(gen_folder / Path("sample_0.hspy"))
+    gen_si.build_G(problem_type = "bremsstrahlung",elements_dict = {})
+    assert gen_si.G.shape == (1900, 10)
+    
+    Xflat = gen_si.X
+    assert Xflat.shape == (1900, 120*100)
 
-    gen_si.build_G(problem_type = "no_brstlg",reference_elt = {"26" : 3.0})
+    gen_si = hs.load(gen_folder / Path("sample_0.hspy"))
+    gen_si.build_G(problem_type = "bremsstrahlung",elements_dict = {"26" : 3.0})
+    assert gen_si.G.shape == (1900, 11)
+
+    gen_si = hs.load(gen_folder / Path("sample_0.hspy"))
+    gen_si.build_G(problem_type = "no_brstlg",elements_dict = {"26" : 3.0})
     assert gen_si.G.shape == (1900, 9)
-    gen_si.build_G(problem_type = "bremsstrahlung",reference_elt = {"26" : 3.0})
-    assert gen_si.G().shape == (1900, 11)
-    assert Xflat.shape == (1900, 120*100)
 
     detector_dict = {
         "detection" : {
             "thickness" : 45,
             "elements_dict" : {
                 "Si" : 3,
                 "Se" : 4
@@ -297,12 +330,100 @@
     assert gen_si.metadata.Acquisition_instrument.TEM.Stage.tilt_alpha == 4.0
     assert gen_si.metadata.Acquisition_instrument.TEM.beam_energy == 100
     assert gen_si.metadata.Acquisition_instrument.TEM.Detector.EDS.take_off_angle == take_off_angle(4.0,2.0,3.0)
     assert gen_si.metadata.Acquisition_instrument.TEM.Detector.EDS.type.as_dictionary() == detector_dict
     assert gen_si.metadata.Acquisition_instrument.TEM.Detector.EDS.width_slope == 0.3
     assert gen_si.metadata.Acquisition_instrument.TEM.Detector.EDS.width_intercept == 65.0
 
+    gen_si.add_analysis_parameters(beam_energy = 200, azimuth_angle = 3.0, elevation_angle = 4.0, tilt_stage = 5.0, elements = ["Fe"], thickness = 400e-7, density = 3.5, detector_type = 'truc.txt', width_slope = 0.32, width_intercept = 85.0, xray_db = "400keV_xrays.json")
+
+    assert gen_si.metadata.Sample.thickness == 500e-7
+    assert gen_si.metadata.Sample.density == 4
+    assert gen_si.metadata.Sample.elements == ["Si", 'Fe'] or gen_si.metadata.Sample.elements == ["Fe", 'Si']
+    assert gen_si.metadata.xray_db == "100keV_xrays.json"
+    assert gen_si.metadata.Acquisition_instrument.TEM.Stage.tilt_alpha == 4.0
+    assert gen_si.metadata.Acquisition_instrument.TEM.beam_energy == 100
+    assert gen_si.metadata.Acquisition_instrument.TEM.Detector.EDS.take_off_angle == take_off_angle(4.0,2.0,3.0)
+    assert gen_si.metadata.Acquisition_instrument.TEM.Detector.EDS.type == 'truc.txt'
+    assert gen_si.metadata.Acquisition_instrument.TEM.Detector.EDS.width_slope == 0.3
+    assert gen_si.metadata.Acquisition_instrument.TEM.Detector.EDS.width_intercept == 65.0
+
     shutil.rmtree(str(gen_folder))
 
 
+def test_carto_fixed_W() :
+
+    def create_data()  : 
+        a = np.random.rand(50,70,100)
+        s = hs.signals.Signal1D(a)
+        s.axes_manager[-1].offset = 0.2
+        s.axes_manager[-1].scale = 0.1
+        s.set_signal_type("EDS_espm")
+        s.set_analysis_parameters()
+        s.add_elements(elements = ["Si","O","Fe","Ca"])
+        return s
+     
+    s = create_data()
+    s.build_G(problem_type = "bremsstrahlung")
+    fw1 = s.carto_fixed_W(brstlg_comps = 2)
+    tw1_1 = np.diag(-1* np.ones(4))
+    tw1_2 = np.zeros((2,4))
+    tw1_prime = np.vstack((tw1_1,tw1_2))
+    tw1_3 = np.zeros((4,2))
+    tw1_4 = -1*np.ones((2,2))
+    tw1_second = np.vstack((tw1_3,tw1_4))
+    tw1 = np.hstack((tw1_prime,tw1_second))
+
+    assert(fw1.shape == (6,6))
+    np.testing.assert_array_equal(fw1,tw1)
+
+    s = create_data()
+    s.build_G(problem_type = "no_brstlg")
+    fw2 = s.carto_fixed_W()
+    tw2 = np.diag(-1* np.ones(4))
+
+    assert(fw2.shape == (4,4))
+    np.testing.assert_array_equal(fw2,tw2)
+
+    s = create_data()
+    s.build_G(problem_type = "no_brstlg", elements_dict = {"26" : 3.0})
+    fw3 = s.carto_fixed_W()
+    tw3 = np.diag(-1* np.ones(5))
+
+    assert(fw3.shape == (5,5))
+    np.testing.assert_array_equal(fw3,tw3)
+
+def test_set_fixed_W() : 
+    def create_data()  : 
+        a = np.random.rand(50,70,100)
+        s = hs.signals.Signal1D(a)
+        s.axes_manager[-1].offset = 0.2
+        s.axes_manager[-1].scale = 0.1
+        s.set_signal_type("EDS_espm")
+        s.set_analysis_parameters()
+        s.set_elements(elements = ["Si","O","Fe","Ca"])
+        return s
+    
+    s = create_data()
+    s.build_G(problem_type = "bremsstrahlung")
+    fw1 = s.set_fixed_W({'p0' : {"Si" : 0.0, 'O' : 0.5, 'b1' : 10.0},'p1' : {}, 'p2' : {'O' : 0.4, 'Fe' : 0.6, 'b0' : 3.0} })
+    tw1 = (np.array([[0.0, 0.5, -1.0, -1.0, -1.0, 10.0],
+                    [-1.0, -1.0, -1.0, -1.0, -1.0, -1.0],
+                    [-1.0, 0.4, 0.6, -1.0, 3.0, -1.0]])).T
+    assert(fw1.shape == (6,3))
+    np.testing.assert_array_equal(fw1,tw1)
+
+    s = create_data()
+    s.build_G(problem_type = "no_brstlg", elements_dict = {"Fe" : 3.0})
+    fw2 = s.set_fixed_W({'p0' : {"Si" : 0.0, 'O' : 0.5},'p1' : {}, 'p2' : {'O' : 0.4, 'Fe' : 0.6} })
+    tw2 = (np.array([[0.0, 0.5, -1.0, -1.0, -1.0],
+                    [-1.0, -1.0, -1.0, -1.0, -1.0],
+                    [-1.0, 0.4, -1.0, 0.6,-1.0]])).T
+    
+    assert(fw2.shape == (5,3))
+    np.testing.assert_array_equal(fw2,tw2)
+
+def test_estimate_best_binning () : 
+    pass
+    # TODO : Implement this test
```

### Comparing `espm-1.0.0/espm/tests/test_docstring.py` & `espm-1.1.1/espm/tests/test_docstring.py`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/espm/tests/test_estimators.py` & `espm-1.1.1/espm/tests/test_estimators.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,44 +4,42 @@
 from espm.estimators.base import normalization_factor
 import numpy as np
 from espm.models import EDXS
 from espm.weights import generate_weights
 from espm.datasets.base import generate_spim
 from espm.measures import trace_xtLx
 from espm.utils import create_laplacian_matrix
-from espm.models.edxs import G_EDXS
 from espm.models.generate_EDXS_phases import generate_modular_phases
 from espm.datasets.base import generate_spim_sample
-import hyperspy.api as hs
 
 
 phases_dict  = {
     'elts_dicts'  : [
     {"Fe" : 0.54860348,
      "Pt" : 0.38286879,
      "Mo" : 0.03166235},
     {"Ca" : 0.54860348,
      "Si" : 0.38286879,
      "O" : 0.03166235}
     ],
     'brstlg_pars' : [
-    {'b0': 5e-3,
-    'b1': 3e-2},
-    {'b0': 7e-3,
-      'b1': 5e-2}
+    {'b0': 5e-5,
+    'b1': 3e-4},
+    {'b0': 7e-5,
+      'b1': 5e-4}
     ],
     'scales' : [0.05,0.05],
     'model_params': {'e_offset': 0.2,
     'e_size': 2000,
     'e_scale': 0.01,
     'width_slope': 0.01,
     'width_intercept': 0.065,
     'db_name': '200keV_xrays.json',
     'E0': 200,
-    'params_dict': {'Abs': {'thickness': 1e-05,
+    'params_dict': {'Abs': {'thickness': 1e-5,
     'toa': 35,
     'density': 5,
     'atomic_fraction': False},
     'Det': 'SDD_efficiency.txt'}}
     }
 
 misc_dict = {
@@ -50,38 +48,36 @@
   'data_folder': 'built_in_particules',
   'shape_2d': [10, 20],
   'model': 'EDXS',
   'densities': [1.3, 1.6]
 }
 
 def generate_one_sample():
-
-
-    
     # Generate the phases
     model = EDXS(**phases_dict["model_params"])
     phases =  generate_modular_phases(**phases_dict)
-    model.generate_g_matr(g_type="bremsstrahlung", elements=["Fe", "Mo", "Ca", "Si", "O", "Pt"] ,reference_elt={})
+    model.generate_g_matr(g_type="bremsstrahlung", elements=["Fe", "Mo", "Ca", "Si", "O", "Pt"] ,elements_dict={})
     G = model.G
 
     weights = generate_weights.generate_weights("laplacian", misc_dict["shape_2d"], n_phases=len(phases_dict["elts_dicts"]), seed=misc_dict["seed"], size_x = 10, size_y = 10)
 
     sample = generate_spim_sample(phases, weights, phases_dict["model_params"],misc_dict, seed = 42,g_params = {})
 
     X = sample["X"].reshape(-1, sample["X"].shape[-1]).T
     X_cont = sample['Xdot'].reshape(-1, sample['Xdot'].shape[-1]).T
     
     D = sample['GW'].T
     H = sample["H_flat"].T
 
     W = np.abs(np.linalg.lstsq(G, D, rcond=None)[0])
     for i in range(10) : 
-        G = G_EDXS(model, {"g_type" : "bremsstrahlung", "elements" : ["Fe", "Mo", "Ca", "Si", "O", "Pt"]},W[:-2,:],G)
+        G = model.NMF_update(W)
         W = np.abs(np.linalg.lstsq(G, D, rcond=None)[0])
 
+
     w = np.array(misc_dict["densities"])
     N = misc_dict["N"]
 
     return G, W, H, D, w, X, X_cont, N
 
 def gen_fixed_mat () : 
     fixed_W = -1*np.ones((8,2))
@@ -98,72 +94,77 @@
 def test_generate_one_sample():
     G, W, H, D, w, X, Xdot, N = generate_one_sample()
     np.testing.assert_allclose(G @ W , D, atol=1e-3)
     np.testing.assert_allclose( D @ H , Xdot)
     np.testing.assert_allclose(G @ W @ H , Xdot, atol=1e-1)
 
 def test_NMF_scikit () : 
-    estimator = SmoothNMF(n_components= 5,max_iter=200,force_simplex = True,mu = 1.0, epsilon_reg = 1.0,hspy_comp = False)
+    estimator = SmoothNMF(n_components= 5,max_iter=200, simplex_W=False, simplex_H = True,mu = 1.0, epsilon_reg = 1.0,hspy_comp = False)
     check_estimator(estimator)
-    estimator = SmoothNMF( n_components= 5,lambda_L=2,max_iter=200,force_simplex = True,mu = 1.0, epsilon_reg = 1.0,hspy_comp = False)
+    estimator = SmoothNMF( n_components= 5,lambda_L=2,max_iter=200, simplex_W=False, simplex_H = True,mu = 1.0, epsilon_reg = 1.0,hspy_comp = False)
     check_estimator(estimator)
 
 def test_general():
     G, W, H, D, w, X, Xdot, N = generate_one_sample()
 
-    estimator = SmoothNMF(G=G,n_components= 2,max_iter=200,force_simplex = True,mu = 0, epsilon_reg = 1, hspy_comp = False)
+    # Check if we can recover D from H and Xdot 
+    estimator = SmoothNMF(G=G,n_components= 2,max_iter=200, simplex_W=False, simplex_H=True, mu = 0, epsilon_reg = 1, hspy_comp = False)
     D2 = estimator.fit_transform(H=H, X=Xdot)
     np.testing.assert_allclose(D, D2, atol=6e-1)
 
-    estimator = SmoothNMF(n_components= 2,max_iter=200,force_simplex = True,mu = 0, epsilon_reg = 1, hspy_comp = False)
+    # Same without G 
+    estimator = SmoothNMF(n_components= 2,max_iter=200, simplex_W=False, simplex_H=True, mu = 0, epsilon_reg = 1, hspy_comp = False)
     D2 = estimator.fit_transform(H=H, X=Xdot)
-    np.testing.assert_allclose(D, D2, atol=6e-1)
+    np.testing.assert_allclose(D, D2, atol=6e-2)
 
-    estimator = SmoothNMF(G=G,n_components= 2,max_iter=200,force_simplex = False,mu = 0, epsilon_reg = 1, hspy_comp = False)
+    # Check if we can recover D, H from W and Xdot 
+    estimator = SmoothNMF(G=G,n_components= 2,max_iter=200,simplex_W=False, simplex_H = True, mu = 0, epsilon_reg = 1, hspy_comp = False)
     D2 = estimator.fit_transform( W=W, X=Xdot)
-    np.testing.assert_allclose(D, D2, atol=3e-1)
+    H2 = estimator.H_ 
+    np.testing.assert_allclose(D, D2, atol=3e-2)
+    np.testing.assert_allclose(H, H2, atol=3e-2)
 
-    estimator = SmoothNMF(G =G, n_components= 2,max_iter=200,force_simplex = True,mu = 0, epsilon_reg = 1, hspy_comp = False)
+    estimator = SmoothNMF(G =G, n_components= 2,max_iter=200, simplex_W=False, simplex_H=True, mu = 0, epsilon_reg = 1, hspy_comp = False)
     D2 = estimator.fit_transform(W=W, X=Xdot)
     np.testing.assert_allclose(D, D2, atol=3e-1)
 
-    estimator = SmoothNMF(G=G, n_components= 2,max_iter=200,force_simplex = True,mu = 0, epsilon_reg = 1, hspy_comp = False)
+    estimator = SmoothNMF(G=G, n_components= 2,max_iter=200, simplex_W=False, simplex_H = True,mu = 0, epsilon_reg = 1, hspy_comp = False, tol = 1.0e-6)
     estimator.fit_transform(X=Xdot)
     P2, A2 = estimator.W_, estimator.H_ 
     np.testing.assert_allclose(G @ P2 @ A2,  Xdot, atol=1)
 
-    estimator = SmoothNMF(G=G, n_components= 2,max_iter=200,force_simplex = True,mu = 0, epsilon_reg = 1, hspy_comp = False)
+    estimator = SmoothNMF(G=G, n_components= 2,max_iter=200, simplex_W=False, simplex_H = True,mu = 0, epsilon_reg = 1, hspy_comp = False, tol = 1.0e-6)
     estimator.fit_transform(X=X)
     P2, A2 = estimator.W_, estimator.H_ 
-    np.testing.assert_allclose(G @ P2 @ A2,  Xdot, atol=1)
+    np.testing.assert_allclose(G @ P2 @ A2,  Xdot, atol=1.1)
 
-    estimator = SmoothNMF(G=G, shape_2d=[10,20], lambda_L=0, n_components= 2,max_iter=200,force_simplex = True,mu = 0, epsilon_reg = 1, hspy_comp = False)
+    estimator = SmoothNMF(G=G, shape_2d=[10,20], lambda_L=0, n_components= 2,max_iter=200, simplex_W=False, simplex_H = True,mu = 0, epsilon_reg = 1, hspy_comp = False, tol = 1.0e-6)
     estimator.fit_transform(X=X)
     P2, A2 = estimator.W_, estimator.H_ 
-    np.testing.assert_allclose(G @ P2 @ A2,  Xdot, atol=1)
+    np.testing.assert_allclose(G @ P2 @ A2,  Xdot, atol=1.1)
 
-    estimator = SmoothNMF(G=G, lambda_L=100, n_components= 2,max_iter=200,force_simplex = True,mu = 0, epsilon_reg = 1, shape_2d=[10,20], hspy_comp = False)
+    estimator = SmoothNMF(G=G, lambda_L=100, n_components= 2,max_iter=200, simplex_W=False, simplex_H = True,mu = 0, epsilon_reg = 1, shape_2d=[10,20], hspy_comp = False, tol = 1.0e-6)
     estimator.fit_transform(X=X)
     P3, A3 = estimator.W_, estimator.H_ 
-    np.testing.assert_allclose(G @ P3 @ A3,  Xdot, atol=1)
+    np.testing.assert_allclose(G @ P3 @ A3,  Xdot, atol=1.1)
     L = create_laplacian_matrix(10, 20)
 
     assert(trace_xtLx(L, A3.T) < trace_xtLx(L, A2.T))
     # assert(trace_xtLx(L, A.T) < trace_xtLx(L, A2.T) )
     assert(trace_xtLx(L, A3.T) < trace_xtLx(L, H.T)*1.01 )
 
 def test_fixed_mat () :
     G, W, H, D, w, X, Xdot, N = generate_one_sample()
     fW, fH = gen_fixed_mat()
-    estimator = SmoothNMF(G=G, n_components= 2,max_iter=200,force_simplex = True, fixed_W = fW, hspy_comp = False)
+    estimator = SmoothNMF(G=G, n_components= 2,max_iter=200, simplex_W=False, simplex_H=True, fixed_W = fW, hspy_comp = False)
     estimator.fit_transform(X=X)
     P2, A2 = estimator.W_, estimator.H_ 
     np.testing.assert_allclose(P2[fW >= 0],fW[fW>=0])
 
-    estimator = SmoothNMF(G=G, n_components= 2,max_iter=200,force_simplex = True, fixed_H = fH, hspy_comp = False)
+    estimator = SmoothNMF(G=G, n_components= 2,max_iter=200, simplex_W=False, simplex_H=True, fixed_H = fH, hspy_comp = False)
     estimator.fit_transform(X=X)
     P2, A2 = estimator.W_, estimator.H_ 
     np.testing.assert_allclose(A2[fH >= 0],fH[fH>=0])
 
 def test_surrogate_smooth_nmf():
     L = create_laplacian_matrix(4, 3)
     for i in range(10):
@@ -198,26 +199,56 @@
             v4 = smooth_dgkl_surrogate(A1, L, A2)
             v5 = trace_xtLx(L, A2.T) / 2
             assert v4 >= v5
             d = diff_surrogate(A1, A2, L=L, algo="log_surrogate")
             np.testing.assert_almost_equal(v4 - v5 , d)
 
 
-def test_X_normalize () : 
-    X = np.random.rand(10,32)
-    fac = np.random.rand()*50
+
+def test_X_normalize() : 
+    np.random.seed(0)
+    X = np.random.rand(10,32)*100
+    fac = np.random.rand()*50+0.1
+    print(fac)
     X_plus = np.concatenate([X/fac,X/fac],axis = 0)
 
     nc = 5
 
-    estim = SmoothNMF(n_components = nc,lambda_L=1.0, max_iter = 10, init = "nndsvd", normalize=True, shape_2d = [8, 4])
+    estim = SmoothNMF(n_components = nc,lambda_L=1.0, max_iter = 10, init = "nndsvd", normalize=True, shape_2d = [8, 4], random_state = 0, simplex_W=False, simplex_H=True)
     GP = estim.fit_transform(X)
+    H = estim.H_
     GP_plus = estim.fit_transform(X_plus)
+    H_plus = estim.H_
 
-    np.testing.assert_allclose(GP_plus*fac, np.concatenate([GP, GP], axis=0))
+    def close_enough(a,b) :
+        num = np.sum(np.abs(a-b))
+        den = np.sum(np.abs(a))
+        ratio = num/den
+        print(num,den,ratio)
+        return ratio < 1e-4
+
+    # plt.figure(figsize=(10,5))
+    # plt.subplot(121)
+    # plt.imshow(H)
+    # plt.colorbar()
+    # plt.subplot(122)
+    # plt.imshow(H_plus)
+    # plt.colorbar()
+
+    # plt.figure(figsize=(10,5))
+    # plt.subplot(121)
+    # plt.imshow(np.concatenate([GP, GP], axis=0))
+    # plt.colorbar()
+    # plt.subplot(122)
+    # plt.imshow(GP_plus*fac)
+    # plt.colorbar()
+    # np.testing.assert_allclose(GP_plus*fac, np.concatenate([GP, GP], axis=0), atol=1e-10)
+    # np.testing.assert_allclose(H_plus, H, atol=1e-10)
+    assert close_enough(GP_plus*fac, np.concatenate([GP, GP], axis=0))
+    assert close_enough(H_plus, H)
 
 def test_normalization_factor () : 
     X_high = np.random.rand(10,32)
     fac = np.random.rand()*50
     X_low = X_high / fac
 
     nc = 5
@@ -245,15 +276,15 @@
 #     # "max_iter" : 10,
 #     # "init" : "random",
 #     # "random_state" : 1,
 #     # "verbose" : 0
 #     # }
 
 #     # params_snmf = {
-#     #     "force_simplex" : True,
+#     #     "simplex_H" : True,
 #     #     "mu": np.random.rand(k)
 #     # }
 
 #     # params_evalution = {
 #     #     "u" : True,
 #     # }
```

### Comparing `espm-1.0.0/espm/tests/test_laplacian.py` & `espm-1.1.1/espm/tests/test_laplacian.py`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/espm/tests/test_measures.py` & `espm-1.1.1/espm/tests/test_measures.py`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/espm/tests/test_updates.py` & `espm-1.1.1/espm/tests/test_updates.py`

 * *Files 3% similar despite different names*

```diff
@@ -447,36 +447,36 @@
     
     G = np.random.rand(l,c)
     P = np.random.rand(c,k)
     GP = G @ P
 
     X = GP @ A
 
-    Pp = multiplicative_step_w(X, G, P, A, log_shift=0)
+    Pp = multiplicative_step_w(X, G, P, A, log_shift=0, simplex_W = False)
     np.testing.assert_array_almost_equal(Pp, P)
 
-    Pp = multiplicative_step_w(X, G, P, A, log_shift=0, l2=True)
+    Pp = multiplicative_step_w(X, G, P, A, log_shift=0, l2=True, simplex_W = False)
     np.testing.assert_array_almost_equal(Pp, P)
 
     for _ in range(10):
         P = np.random.rand(c,k)
-        Pp = multiplicative_step_w(X, G, P, A)
+        Pp = multiplicative_step_w(X, G, P, A, simplex_W = False)
         Pp2 = make_step_p(X, G, P, A)
         np.testing.assert_array_almost_equal(Pp, Pp2)
         GP = G @ P
         GPp = G @ Pp
         val1 = KLdiv_loss(X, GP, A)
         val2 = KLdiv_loss(X, GPp, A)
         np.testing.assert_array_less(0, Pp)
         assert(val1 > val2)
 
 
     for _ in range(10):
         P = np.random.rand(c,k)
-        Pp = multiplicative_step_w(X, G, P, A, l2=True)
+        Pp = multiplicative_step_w(X, G, P, A, l2=True, simplex_W = False)
         GP = G @ P
         GPp = G @ Pp
         val1 = Frobenius_loss(X, GP, A)
         val2 = Frobenius_loss(X, GPp, A)
         np.testing.assert_array_less(0, Pp)
         assert(val1 > val2)
 
@@ -493,83 +493,83 @@
     G = np.random.rand(l,c)
     P = np.random.rand(c,k)
     GP = G @ P
 
     X = GP @ A
     np.testing.assert_allclose(np.sum(A, axis=0), np.ones([A.shape[1]]), atol=dicotomy_tol)
 
-    Ap = multiplicative_step_h(X, G, P, A, force_simplex=False, mu=0, log_shift=0, epsilon_reg=1, safe=True)
+    Ap = multiplicative_step_h(X, G, P, A, simplex_H=False, mu=0, log_shift=0, epsilon_reg=1, safe=True)
     np.testing.assert_array_almost_equal(A, Ap)
     np.testing.assert_allclose(np.sum(Ap, axis=0), np.ones([Ap.shape[1]]), atol=dicotomy_tol)
 
-    Ap = multiplicative_step_h(X, G, P, A, force_simplex=True, mu=0, log_shift=0, epsilon_reg=1, safe=True)
+    Ap = multiplicative_step_h(X, G, P, A, simplex_H=True, mu=0, log_shift=0, epsilon_reg=1, safe=True)
     np.testing.assert_allclose(A, Ap, atol=dicotomy_tol)        
 
     # Same test for l2
-    Ap = multiplicative_step_h(X, G, P, A, force_simplex=False, mu=0, log_shift=0, epsilon_reg=1, safe=True, l2=True)
+    Ap = multiplicative_step_h(X, G, P, A, simplex_H=False, mu=0, log_shift=0, epsilon_reg=1, safe=True, l2=True)
     np.testing.assert_array_almost_equal(A, Ap)
     np.testing.assert_allclose(np.sum(Ap, axis=0), np.ones([Ap.shape[1]]), atol=dicotomy_tol)
 
-    Ap = multiplicative_step_h(X, G, P, A, force_simplex=True, mu=0, log_shift=0, epsilon_reg=1, safe=True, l2=True)
+    Ap = multiplicative_step_h(X, G, P, A, simplex_H=True, mu=0, log_shift=0, epsilon_reg=1, safe=True, l2=True)
     np.testing.assert_allclose(A, Ap, atol=dicotomy_tol)       
 
     for _ in range(10):
         A = np.random.rand(k,p)
         A = A/np.sum(A, axis=1, keepdims=True)
-        Ap =  multiplicative_step_h(X, G, P, A, force_simplex=False, mu=0, log_shift=0, epsilon_reg=1, safe=True)
+        Ap =  multiplicative_step_h(X, G, P, A, simplex_H=False, mu=0, log_shift=0, epsilon_reg=1, safe=True)
         val1 = KLdiv_loss(X, GP, A)
         val2 = KLdiv_loss(X, GP, Ap)
         np.testing.assert_array_less(0, Ap)
         assert(val1 > val2)
 
-        Ap =  multiplicative_step_h(X, G, P, A, force_simplex=True, mu=0, log_shift=log_shift, epsilon_reg=1, safe=True)
+        Ap =  multiplicative_step_h(X, G, P, A, simplex_H=True, mu=0, log_shift=log_shift, epsilon_reg=1, safe=True)
         Ap2 =  make_step_a(X, G, P, A, mu_sparse=0, eps=log_shift, eps_sparse=1, mask=None)
         np.testing.assert_array_almost_equal(Ap2, Ap)
         np.testing.assert_allclose(np.sum(Ap, axis=0), np.ones([Ap.shape[1]]), atol=dicotomy_tol)
 
         val1 = KLdiv_loss(X, GP, A)
         val2 = KLdiv_loss(X, GP, Ap)
         np.testing.assert_array_less(0, Ap)
         assert(val1 > val2)
 
         epsilon_reg = 1
         mu = np.ones(k)
         mu[0] = 0
-        Ap =  multiplicative_step_h(X, G, P, A, force_simplex=True, mu=mu, log_shift=log_shift, epsilon_reg=epsilon_reg, safe=True)
+        Ap =  multiplicative_step_h(X, G, P, A, simplex_H=True, mu=mu, log_shift=log_shift, epsilon_reg=epsilon_reg, safe=True)
         Ap2 =  make_step_a(X, G, P, A, mu_sparse=1, eps=log_shift, eps_sparse=epsilon_reg, mask=None)
         np.testing.assert_array_almost_equal(Ap2, Ap)
         np.testing.assert_allclose(np.sum(Ap, axis=0), np.ones([Ap.shape[1]]), atol=dicotomy_tol)
 
 
-        Ap =  multiplicative_step_h(X, G, P, A, force_simplex=True, mu=3*mu, log_shift=log_shift, epsilon_reg=epsilon_reg, safe=True)
+        Ap =  multiplicative_step_h(X, G, P, A, simplex_H=True, mu=3*mu, log_shift=log_shift, epsilon_reg=epsilon_reg, safe=True)
         Ap2 =  make_step_a(X, G, P, A, mu_sparse=3, eps=log_shift, eps_sparse=epsilon_reg, mask=None)
         np.testing.assert_array_almost_equal(Ap2, Ap)
         np.testing.assert_allclose(np.sum(Ap, axis=0), np.ones([Ap.shape[1]]), atol=dicotomy_tol)
 
 
         val1 = KLdiv_loss(X, GP, A) + log_reg(A, 3*mu, epsilon_reg)
         val2 = KLdiv_loss(X, GP, Ap) + log_reg(A, 3*mu, epsilon_reg)
         np.testing.assert_array_less(0, Ap)
         assert(val1 > val2)
 
-        # Ap =  multiplicative_step_h(X, G, P, A, force_simplex=True, mu=3, eps=log_shift, epsilon_reg=1, safe=True)
+        # Ap =  multiplicative_step_h(X, G, P, A, simplex_H=True, mu=3, eps=log_shift, epsilon_reg=1, safe=True)
         # Ap2 =  make_step_a(X, G, P, A, mu_sparse=3, eps=log_shift, eps_sparse=1, mask=np.zeros([k])>0)
         # np.testing.assert_array_almost_equal(Ap2, Ap)
         # np.testing.assert_allclose(np.sum(Ap, axis=0), np.ones([Ap.shape[1]]), atol=dicotomy_tol)
 
     for _ in range(10):
         A = np.random.rand(k,p)
         A = A/np.sum(A, axis=1, keepdims=True)
-        Ap =  multiplicative_step_h(X, G, P, A, force_simplex=False, mu=0, log_shift=0, epsilon_reg=1, safe=True, l2=True)
+        Ap =  multiplicative_step_h(X, G, P, A, simplex_H=False, mu=0, log_shift=0, epsilon_reg=1, safe=True, l2=True)
         val1 = Frobenius_loss(X, GP, A)
         val2 = Frobenius_loss(X, GP, Ap)
         np.testing.assert_array_less(0, Ap)
         assert(val1 > val2)
 
-        Ap =  multiplicative_step_h(X, G, P, A, force_simplex=True, mu=0, log_shift=log_shift, epsilon_reg=1, safe=True, l2=True)
+        Ap =  multiplicative_step_h(X, G, P, A, simplex_H=True, mu=0, log_shift=log_shift, epsilon_reg=1, safe=True, l2=True)
         np.testing.assert_allclose(np.sum(Ap, axis=0), np.ones([Ap.shape[1]]), atol=dicotomy_tol)
 
         val1 = Frobenius_loss(X, GP, A)
         val2 = Frobenius_loss(X, GP, Ap)
         np.testing.assert_array_less(0, Ap)
         assert(val1 > val2)
 
@@ -586,31 +586,31 @@
     G = np.random.rand(l,c)
     P = np.random.rand(c,k)
     GP = G @ P
 
     X = GP @ A
     np.testing.assert_allclose(np.sum(A, axis=0), np.ones([A.shape[1]]), atol=dicotomy_tol)
 
-    Ap = multiplicative_step_hq(X, G, P, A, force_simplex=False, log_shift=0,safe=True)
+    Ap = multiplicative_step_hq(X, G, P, A, simplex_H=False, log_shift=0,safe=True)
     np.testing.assert_array_almost_equal(A, Ap)
     np.testing.assert_allclose(np.sum(Ap, axis=0), np.ones([Ap.shape[1]]), atol=dicotomy_tol)
 
-    Ap = multiplicative_step_hq(X, G, P, A, force_simplex=True, log_shift=0, safe=True)
+    Ap = multiplicative_step_hq(X, G, P, A, simplex_H=True, log_shift=0, safe=True)
     np.testing.assert_allclose(A, Ap, atol=dicotomy_tol)        
 
     for _ in range(10):
         A = np.random.rand(k,p)
         A = A/np.sum(A, axis=1, keepdims=True)
-        Ap =  multiplicative_step_hq(X, G, P, A, force_simplex=False,  log_shift=0, safe=True)
+        Ap =  multiplicative_step_hq(X, G, P, A, simplex_H=False,  log_shift=0, safe=True)
         val1 = KLdiv_loss(X, GP, A)
         val2 = KLdiv_loss(X, GP, Ap)
         np.testing.assert_array_less(0, Ap)
         assert(val1 > val2)
 
-        Ap =  multiplicative_step_hq(X, G, P, A, force_simplex=True, log_shift=log_shift, safe=True)
+        Ap =  multiplicative_step_hq(X, G, P, A, simplex_H=True, log_shift=log_shift, safe=True)
         Ap2 =  make_step_a(X, G, P, A, mu_sparse=0, eps=log_shift, eps_sparse=1, mask=None)
         np.testing.assert_array_almost_equal(Ap2, Ap)
         np.testing.assert_allclose(np.sum(Ap, axis=0), np.ones([Ap.shape[1]]), atol=dicotomy_tol)
 
         val1 = KLdiv_loss(X, GP, A)
         val2 = KLdiv_loss(X, GP, Ap)
         np.testing.assert_array_less(0, Ap)
@@ -652,18 +652,18 @@
         for b in range(p):
             for c in range(i):
                 Q[a,b,c] = A[c,b] * D[a,c] / (np.sum(A[:,b] * D[a,:]) + log_shift)
     Q2 = update_q(D, A)
     np.testing.assert_array_almost_equal(Q, Q2)
     assert((np.isnan(Q)==False).all())
 
-def create_toy_problem(l = 25, k = 3, p = 100, c = 10, n_poisson=200, force_simplex=True):
+def create_toy_problem(l = 25, k = 3, p = 100, c = 10, n_poisson=200, simplex_H=True):
 
     A = np.random.rand(k,p)
-    if force_simplex:
+    if simplex_H:
         A = A/np.sum(A, axis=0, keepdims=True)
     
     G = np.random.rand(l,c)
     P = np.random.rand(c,k)
     GP = G @ P
 
     X = GP @ A
@@ -688,15 +688,15 @@
     for _ in range(10):
 
         G, W, H, Xtrue, X = create_toy_problem(p = shape_2d[0]*shape_2d[1], k=k, n_poisson=n_poisson)
 
         true_D = G @ W
         true_H = H
 
-        for force_simplex in [True, False]:
+        for simplex_H in [True, False]:
             for lambda_L in [0, 1, 10]:
                 for mu in [0, 1 ,10]:
 
                     W0 = np.random.rand(*W.shape)
                     H0 = np.random.rand(*H.shape)
                     W0 = np.maximum(W0, log_shift)
                     H0 = np.maximum(H0, log_shift)
@@ -706,26 +706,26 @@
                     gamma_h = estimate_Lipschitz_bound_h(log_shift, X, G, k, mu=mu, lambda_L=lambda_L, epsilon_reg=epsilon_reg)
 
                     loss1 = full_loss(X, G, W0, H0, log_shift, mu, lambda_L, L)
                     
                     grad = gradH(X, G, W0, H0, log_shift=log_shift, l2=False, mu=mu, lambda_L=lambda_L, L=L, epsilon_reg=epsilon_reg)
                     H1 = H0 - 1/gamma_h * grad
                     loss2 = full_loss(X, G, W0, H1, log_shift, mu, lambda_L, L)
-                    H2 =proj_grad_step_h(X, G, W0, H0, gamma_h, log_shift=log_shift, safe=True, l2=False, force_simplex=force_simplex, mu=mu, lambda_L=lambda_L,  L=L, epsilon_reg=epsilon_reg)
+                    H2 =proj_grad_step_h(X, G, W0, H0, gamma_h, log_shift=log_shift, safe=True, l2=False, simplex_H=simplex_H, mu=mu, lambda_L=lambda_L,  L=L, epsilon_reg=epsilon_reg)
                     loss3 = full_loss(X, G, W0, H2, log_shift, mu, lambda_L, L)
                     assert( loss1 >= loss2) 
                     assert(loss1 >= loss3)
                     assert((H2 >= log_shift).all())
 
                     maxit = 10
                     loss_old = loss3
                     grad = gradH(X, G, W0, H2, log_shift=log_shift, l2=False)
                     n_grad_old = np.sum(grad**2)
                     for _ in range(maxit):
-                        H2 = proj_grad_step_h(X, G, W0, H2, gamma_h, log_shift=log_shift, safe=True, l2=False, force_simplex=force_simplex, mu=mu, lambda_L=lambda_L,  L=L, epsilon_reg=epsilon_reg)
+                        H2 = proj_grad_step_h(X, G, W0, H2, gamma_h, log_shift=log_shift, safe=True, l2=False, simplex_H=simplex_H, mu=mu, lambda_L=lambda_L,  L=L, epsilon_reg=epsilon_reg)
                         grad = gradH(X, G, W0, H2, log_shift=log_shift,  mu=mu, lambda_L=lambda_L,  L=L, l2=False)
                         n_grad = np.sum(grad**2)
                         loss = full_loss(X, G, W0, H2, log_shift, mu, lambda_L, L)
                         assert loss<=loss_old+np.abs(loss_old)*0.00001
                         # assert n_grad<=n_grad_old
                         loss_old = loss
                         n_grad_old = n_grad
@@ -748,26 +748,26 @@
 
         gamma_w = estimate_Lipschitz_bound_w(log_shift, X, G, k)
 
         loss1 = KLdiv_loss(X, G@W0, H0, log_shift=log_shift)
         grad = gradW(X, G, W0, H0, log_shift=log_shift, l2=False)
         W1 = W0 - 1/gamma_w * grad
         loss2 = KLdiv_loss(X, G@W1, H0, log_shift=log_shift)
-        W2 =proj_grad_step_w(X, G, W0, H0, gamma_w, log_shift=log_shift, safe=True, l2=False)
+        W2 =proj_grad_step_w(X, G, W0, H0, gamma_w, log_shift=log_shift, safe=True, l2=False, simplex_W = False)
         loss3 = KLdiv_loss(X, G@W2, H0, log_shift=log_shift)
         assert( loss1 >= loss2) 
         assert(loss1 >= loss3)
         assert((W2 >= log_shift).all())
 
         maxit = 10
         loss_old = loss3
         grad = gradW(X, G, W2, H0, log_shift=log_shift, l2=False)
         n_grad_old = np.sum(grad**2)
         for _ in range(maxit):
-            W2 = proj_grad_step_w(X, G, W2, H0, gamma_w, log_shift=log_shift, safe=True, l2=False)
+            W2 = proj_grad_step_w(X, G, W2, H0, gamma_w, log_shift=log_shift, safe=True, l2=False, simplex_W = False)
             grad = gradW(X, G, W2, H0, log_shift=log_shift, l2=False)
 
             n_grad = np.sum(grad**2)
             loss = KLdiv_loss(X, G@W2, H0, log_shift=log_shift)
             assert loss<=loss_old
             assert n_grad<=n_grad_old
             loss_old = loss
```

### Comparing `espm-1.0.0/espm/tests/test_utils.py` & `espm-1.1.1/espm/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from hyperspy.misc.material import _density_of_mixture
+from exspy.misc.material import _density_of_mixture
 import numpy as np
 import espm.utils as u
 
 
 def test_rescale() :
     np.random.seed(0)
     for _ in range(20):
```

### Comparing `espm-1.0.0/espm/utils.py` & `espm-1.1.1/espm/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 r"""Utils for the ESPM package"""
 
 import numpy as np
 from scipy.sparse import lil_matrix, block_diag
 from scipy.optimize import nnls
 from espm.conf import SYMBOLS_PERIODIC_TABLE, NUMBER_PERIODIC_TABLE
 import json
-from hyperspy.misc.material import atomic_to_weight, density_of_mixture
+from exspy.misc.material import atomic_to_weight, density_of_mixture
 from functools import wraps
+import re
 
 _qtg_widgets = []
 _plt_figures = []
 
 def process_losses(losses):
     r""" Process the losses to be plotted
 
@@ -250,15 +251,15 @@
         
         for elt in elements_dict.keys() : 
             list_elts.append(elt)
             list_wt.append(elements_dict[elt])
         
         return density_of_mixture(list_wt,list_elts)
 
-def arg_helper(params, d_params):
+def arg_helper(params, d_params, replace = True):
     r""" Check if all parameter of d_params are in params. If not, they are added to params with the default value.
 
     Parameters
     ----------
     params : dict
         Dictionary of parameters to be checked.
     d_params : dict
@@ -268,20 +269,20 @@
     -------
     params : dict
         Dictionary of parameters with the default parameters added if not present.
     
     """
     for key in d_params.keys():
         params[key] = params.get(key, d_params[key])
-        if isdict(params[key])  and isdict(d_params[key]):
-            params[key] = arg_helper(params[key], d_params[key])
-    check_keys(params, d_params)
+        if isdict(params[key]) and isdict(d_params[key]):
+            params[key] = arg_helper(params[key], d_params[key], replace=replace)
+    check_keys(params, d_params, replace = replace)
     return params
 
-def check_keys(params, d_params, upperkeys = '',toprint = True):
+def check_keys(params, d_params, upperkeys = '',toprint = True, replace = True):
     r""" Check if all parameter of d_params are in params. If not, they are added to params with the default value.
 
     Parameters
     ----------
     params : dict
         Dictionary of parameters to be checked.
     d_params : dict
@@ -314,15 +315,23 @@
             if isdict(params[key]):
 #                 if not(isdict(d_params[key])):
 #                     print('Warning! Optional argument: {}{} is not supposed to be a dictionary'.format(upperkeys,key))
 #                 else:
 #                     check_keys(params[key],d_params[key],upperkeys=upperkeys+'[\'{}\']'.format(key))
                 if isdict(d_params[key]):
                     if toprint :
-                        check_keys(params[key],d_params[key],upperkeys=upperkeys+'[\'{}\']'.format(key))
+                        check_keys(params[key],d_params[key],upperkeys=upperkeys+'[\'{}\']'.format(key), toprint = toprint, replace = replace)
+            else:
+                if replace : 
+                    # If we prefer to keep the values of the default parameters
+                    pass
+                else : 
+                    # If we prefer to let the values of the default parameters unchanged
+                    # useful in EDS_espm to keep the original metadata
+                    params[key] = d_params[key]
     return True
 
 def isdict(p):
     r"""Return True if the variable a dictionary.
     
     :param p: variable to check
     :type p: any
@@ -367,20 +376,36 @@
     symbol_list = []
     with open(NUMBER_PERIODIC_TABLE,"r") as f : 
             NPT = json.load(f)["table"]
     for num in NPT.keys() : 
         symbol_list.append(NPT[num]["symbol"])
     return symbol_list
 
-
 def close_all():
     r"""Close all opened windows."""
     import matplotlib.pyplot as plt
     global _qtg_widgets
     for widget in _qtg_widgets:
         widget.close()
     _qtg_widgets = []
 
     global _plt_figures
     for fig in _plt_figures:
         plt.close(fig)
     _plt_figures = []
+
+def get_explained_intensity_W(G, W, H) : 
+    r""" Compute the explained intensity of each element of W.
+
+    :param np.array 2D G: G matrix of the ESpM-NMF decomposition
+    :param np.array 2D W: W matrix of the ESpM-NMF decomposition
+    :param np.array 2D H: H matrix of the ESpM-NMF decomposition
+
+    :return: np.array 2D
+
+    """
+    # I couldn't find a linear algebra trick
+    int_matrix = np.zeros(W.shape)
+    for i in range(W.shape[0]) : 
+        for j in range(W.shape[1]) : 
+            int_matrix[i,j] = np.sum(G[:,i, np.newaxis]*W[i,j]*H[np.newaxis,j,:])
+    return int_matrix
```

### Comparing `espm-1.0.0/espm/weights/abundance.py` & `espm-1.1.1/espm/weights/abundance.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 import numpy as np
 from espm.models.EDXS_function import gaussian
 import scipy.ndimage as ndimage
 from skimage.filters import threshold_otsu
 import hyperspy.api as hs
 from skimage.filters import median
 from scipy.interpolate import RectBivariateSpline
-# from scipy.interpolate import interp2d
-
 
 class Abundance(object):
     
     def __init__(self, shape_2d, n_phases):
         self.shape_2d = shape_2d
         self.n_phases = n_phases
         self._weights = np.zeros([*shape_2d, n_phases])
@@ -257,15 +255,15 @@
         assert phase_id != 0, "The phase_id cannot be 0, it has to be between 1 and n_phases-1."
         np.random.seed(seed)
         rnd = np.random.rand(size_x,size_y)
         lapl = median(median(rnd))
         # f = interp2d(np.arange(size_x), np.arange(size_y), lapl, kind='cubic')
         f = RectBivariateSpline(np.arange(size_x), np.arange(size_y), lapl.T)
         # For some dumb reason, the interpolation function has to have the coordinates in the opposite order
-        res = f(np.linspace(0,size_y,num = self.shape_2d[1]),np.linspace(0,size_x,num = self.shape_2d[0])).T
+        res = f(np.linspace(0,size_y-1,num = self.shape_2d[1]),np.linspace(0,size_x-1,num = self.shape_2d[0])).T
 
         scaled_res = self.scale_phase(res,conc_min,conc_max)
         self.check_add_weights(scaled_res, phase_id)
 
     def add_random(self,seed, phase_id, conc_min, conc_max) : 
         r"""
         Function to generate random noise.
```

### Comparing `espm-1.0.0/espm/weights/generate_weights.py` & `espm-1.1.1/espm/weights/generate_weights.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         ...     axs[i].set_title(f"Map {i+1}")
         >>> fig.show()
 
     """
     a = Abundance(shape_2d, n_phases)
     np.random.seed(seed)
     for i in range(1,n_phases) :
-        a.add_sphere((np.random.randint(1,shape_2d[0]),np.random.randint(1,shape_2d[1])),radius,1/n_phases,i)
+        a.add_sphere((np.random.randint(1,shape_2d[0]),np.random.randint(1,shape_2d[1])),radius,1/(n_phases-1),i)
     return a.weights
 
 def wedge_weights(shape_2d=[80, 80]):
     r"""
     Generate a weight matrix with a wedge of phase 2 and complementary phase 1.
 
     Parameters
```

### Comparing `espm-1.0.0/espm.egg-info/SOURCES.txt` & `espm-1.1.1/espm.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-.readthedocs.yml
+.readthedocs.yaml
 CHANGELOG.rst
 CONTRIBUTING.rst
 Licence.txt
 MANIFEST.in
 README.rst
 hyperspy_extension.yaml
-readthedoc.yml
 setup.py
 todo.md
 .github/workflows/doc.yml
 .github/workflows/python.yml
 doc/changelog.rst
 doc/conf.py
 doc/contributing.rst
@@ -75,22 +74,14 @@
 espm/tests/test_measures.py
 espm/tests/test_updates.py
 espm/tests/test_utils.py
 espm/weights/__init__.py
 espm/weights/abundance.py
 espm/weights/generate_weights.py
 generated_datasets/71GPa_experimental_data.hspy
-notebooks/VCA.py
 notebooks/api.ipynb
 notebooks/background_fit.ipynb
 notebooks/convergence-speed.ipynb
+notebooks/convergence.py
 notebooks/generate_data.ipynb
-notebooks/make-plots.ipynb
-notebooks/other_algorithms.ipynb
-notebooks/preprocess_dataset.ipynb
-notebooks/select_spectrum.ipynb
-notebooks/simple-test-regularisation.ipynb
-notebooks/spectrum_fit.ipynb
-notebooks/sunsal.py
-notebooks/surrogate-vs-bregmann.ipynb
-notebooks/toy-ML.ipynb
-notebooks/old/algo-with-negative-variable.ipynb
+notebooks/papers_figures.ipynb
+notebooks/toy-ML.ipynb
```

### Comparing `espm-1.0.0/generated_datasets/71GPa_experimental_data.hspy` & `espm-1.1.1/generated_datasets/71GPa_experimental_data.hspy`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/notebooks/api.ipynb` & `espm-1.1.1/notebooks/api.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970870535714286%*

 * *Differences: {"'cells'": "{6: {'source': ['spim.build_G()']}, 7: {'source': {insert: [(6, '- G : The EDX model "*

 * *            'is integrated in the decomposition. The algorithm learns the concentration of each '*

 * *            "chemical element and the bremsstrahlung parameters.\\n')]}}, 8: {'source': ['est = "*

 * *            'SmoothNMF( n_components = 3, tol = 1e-6, max_iter = 200, G = spim.model,hspy_comp = '*

 * *            "True)']}}",*

 * * "'metadata'": "{'language_info': {'version': '3.11.8'}}"}*

```diff
@@ -76,38 +76,39 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "spim.build_G(\"bremsstrahlung\")"
+                "spim.build_G()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Problem solving\n",
                 "\n",
                 "### Picking analysis parameters\n",
                 "\n",
                 "- 3 components for 3 phases\n",
                 "- convergence criterions : tol and max_iter. tol is the minimum change of the loss function between two iterations. max_iter is the max number of iterations.\n",
+                "- G : The EDX model is integrated in the decomposition. The algorithm learns the concentration of each chemical element and the bremsstrahlung parameters.\n",
                 "- hspy_comp is a required parameter if you want to use the hyperspy api"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "est = SmoothNMF( n_components = 3,tol=0.000001, max_iter = 500, G = spim.G,hspy_comp = True)"
+                "est = SmoothNMF( n_components = 3, tol = 1e-6, max_iter = 200, G = spim.model,hspy_comp = True)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -183,15 +184,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.10"
+            "version": "3.11.8"
         },
         "varInspector": {
             "cols": {
                 "lenName": 16,
                 "lenType": 16,
                 "lenVar": 40
             },
```

### Comparing `espm-1.0.0/notebooks/background_fit.ipynb` & `espm-1.1.1/notebooks/toy-ML.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.943807846606344%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(2, 'from espm.estimators import SmoothNMF\\n'), (3, 'from "*

 * *            "espm.measures import find_min_angle, ordered_mse, ordered_mae, ordered_r2\\n'), (4, "*

 * *            "'from espm.models import ToyModel\\n'), (5, 'from espm.weights import "*

 * *            "generate_weights as gw\\n'), (6, 'from espm.datasets.base import "*

 * *            "generate_spim_sample\\n'), (7, 'from espm.utils import process_losses')], delete: "*

 * *            "[13, 12, 11, 10, 9, 8, 7, 6, 4, 2, 1, 0 […]*

```diff
@@ -1,555 +1,610 @@
 {
     "cells": [
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Regularized Poisson NMF on a toy dataset\n",
+                "\n",
+                "This notebook is part of the ESPM package. It is available on [github](https://github.com/adriente/espm/blob/main/notebooks/toy-ML.ipynb) \n",
+                "\n",
+                "In this notebook, we show how to solve a regularized Poisson Non Negative Matrix Factorization (NMF) on a toy dataset. The general goal of this problem is to separate a matrix $X$ into two matrices $D$ and $H$ such that $X \\approx DH$. \n",
+                "We will assume that $D$ is the product of two matrices $G$ and $W$ such that $D = GW$. The matrix $G$ is assumed to be known and therefore $W$ is the matrix we want to find. In the field of electro-microscopy, the matrix $GW$ represent the phases, the matrix $H$ is the matrix of maps (or weights) and $X$ is the data matrix. The maps $H$ are 2D images.\n",
+                "Furthermore, we will assume that $W, H$ are non-negative or more generally greater than a small positive value $\\epsilon$. \n",
+                "\n",
+                "The data measured data $X$ is follow a Poisson distribution, i.e. $X_{ij} \\sim \\text{Poisson}(n_p\\dot{X}_{ij})$. In the context of electro-microscopy, $n_p$ is the number of photons per pixel. $\\dot{X} = G \\dot{W} \\dot{H}$ would correspond a noiseless measurement. \n",
+                "\n",
+                "The size of:\n",
+                "\n",
+                "* $X$ is (n, p),\n",
+                "* $W$ is (m, k),\n",
+                "* $H$ is (k, p),\n",
+                "* $G$ is (n, m).\n",
+                "\n",
+                "In general, m is assumed to be much smaller than n and $G$ is assumed to be known. The parameter `shape_2d` defines the shape of the images for the columns of $H$ and $X$, i.e. `shape_2d[0]*shape_2d[1] = p`.\n",
+                "\n",
+                "Mathematically. the problem can be formulated as:\n",
+                "$$\\dot{W}, \\dot{H} = \\arg\\min_{W\\geq\\epsilon, H\\geq\\epsilon, \\sum_i H_{ij}  = 1} D_{GKL}(X || GWH) + \\lambda tr ( H^\\top \\Delta H) + \\mu \\sum_{i,j} (\\log H_{ij} +  \\epsilon_{reg})$$\n",
+                "\n",
+                "Here $D_{GKL}$ is the fidelity term, i.e. the Generalized KL divergence \n",
+                "\n",
+                "$$D_{GKL}(X \\| Y) = \\sum_{i,j} X_{ij} \\log \\frac{X_{ij}}{Y_{ij}} - X_{ij} + Y_{ij} $$\n",
+                "\n",
+                "The loss is regularized using two terms: a Laplacian regularization on $H$ and a log regularization on $H$. \n",
+                "$\\lambda$ and $\\mu$ are the regularization parameters.\n",
+                "The Laplacian regularization is defined as:\n",
+                "\n",
+                "$$ \\lambda tr ( H^\\top \\Delta H) $$\n",
+                "\n",
+                "where $\\Delta$ is the Laplacian operator (it can be created using the function :mod:`espm.utils.create_laplacian_matrix`). **Note that the columns of the matrices $H$ and $X$ are assumed to be images.** \n",
+                "\n",
+                "The log regularization is defined as:\n",
+                "\n",
+                "$$ \\mu \\sum_{i,j} (\\log H_{ij} +  \\epsilon_{reg}) $$\n",
+                "\n",
+                "where $\\epsilon_{reg}$ is the slope of log regularization at 0. This term acts similarly to an L1 penalty but affects less larger values. \n",
+                "\n",
+                "Finally, we assume $W,H\\geq \\epsilon$ and that the lines of $H$ sum to 1: $$\\sum_i H_{ij}  = 1.$$ This is done by adding the parameter `simplex_H=True` to the class `espm.estimators.SmoothNMF`. This constraint is essential as it prevent the algorithm to find a solution where all the maps tend to 0 because of the other constraints. Note that the same constraint could be applied to $W$ using `simplex_W=True`. These two constraint should not be activated at the same time!\n",
+                "\n",
+                "\n",
+                "In this notebook, we will use the class `espm.estimators.SmoothNMF` to solve the problem.\n"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Imports and function definition\n",
+                "\n",
+                "Let's start by importing the necessary libraries."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Some useful modules for notebooks\n",
+                "%load_ext autoreload\n",
+                "%autoreload 2\n",
+                "%matplotlib inline"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# %matplotlib inline\n",
-                "%matplotlib qt\n",
-                "import hyperspy.api as hs\n",
                 "import numpy as np\n",
-                "import lmfit as lm\n",
                 "import matplotlib.pyplot as plt\n",
-                "import matplotlib\n",
-                "from espm.models import edxs\n",
-                "from espm.models.EDXS_function import print_concentrations_from_W\n",
-                "import espm.spectrum_fitting as sf\n",
-                "from espm.conf import DATASETS_PATH\n",
-                "from pathlib import Path\n",
-                "from espm.datasets import spim\n",
-                "from espm.estimators import SmoothNMF"
+                "from espm.estimators import SmoothNMF\n",
+                "from espm.measures import find_min_angle, ordered_mse, ordered_mae, ordered_r2\n",
+                "from espm.models import ToyModel\n",
+                "from espm.weights import generate_weights as gw\n",
+                "from espm.datasets.base import generate_spim_sample\n",
+                "from espm.utils import process_losses"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Guide to this notebook\n",
-                "\n",
-                "Every time the symbol \u26a0\ufe0f appears, a user input is required in the cell below.\n",
-                "\n",
-                "If a cell made a few windows pop up, please kill the windows once you're done. Otherwise every new plot will be displayed in top of the other (which may slow your computer down). \n",
-                "\n",
-                "Overview of the different steps :\n",
-                "- I. Load the data either a spectrum (go to step III.) or a spectrum image\n",
-                "- II. Select an area of interest in your spectrum image.\n",
-                "- III. Creates an energy scale (x) from your data for the fitting procedure.\n",
-                "- IV. Selects the regions of the spectrum were there are no peaks for background fitting.\n",
-                "- V. Creates the required objects (partial x and y) for the background fitting procedure.\n",
-                "- VI. Fitting the background. If this is not satisfactory go back to IV."
+                "Now we define the parameters that will be used to generate the data.\n"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## I. Load spectrum & energy scale\n",
                 "\n",
-                "The spectrum is expected to be an average spectrum, its energy range is expected to start above 0.0\n",
+                "seed = 42 # for reproducibility\n",
+                "\n",
+                "m = 15 # Number of components\n",
+                "n = 200 # Length of the phases\n",
                 "\n",
-                "\u26a0\ufe0f"
+                "n_poisson = 300 # Average poisson number per pixel (this number will be splitted on the m dimension)\n",
+                "\n",
+                "densities = np.random.uniform(0.1, 2.0, 3) # Random densities\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "input_filename = str(\"phyllo_spectre_moyen.hspy\")\n",
-                "spectrum = hs.load(input_filename)\n",
+                "def get_toy_sample():\n",
+                "    model_params = {\"L\": n, \"C\": m, \"K\": 3, \"seed\": seed}\n",
+                "    misc_params = {\"N\": n_poisson, \"seed\": seed, 'densities' : densities, \"model\": \"ToyModel\"}\n",
+                "\n",
+                "    toy_model = ToyModel(**model_params)\n",
+                "    toy_model.generate_phases()\n",
+                "    phases = toy_model.phases.T\n",
+                "    weights = gw.generate_weights(\"toy_problem\", None)\n",
                 "\n",
-                "offset = spectrum.axes_manager[0].offset\n",
-                "scale = spectrum.axes_manager[0].scale\n",
-                "size = spectrum.axes_manager[0].size\n",
+                "    sample = generate_spim_sample(phases, weights, model_params,misc_params, seed = seed)\n",
+                "    return sample\n",
                 "\n",
-                "x = np.linspace(offset,size*scale+offset,num = size)"
+                "def to_vec(X):\n",
+                "    n = X.shape[2]    \n",
+                "    return X.transpose(2,0,1).reshape(n, -1)\n",
+                "\n",
+                "sample = get_toy_sample()\n",
+                "\n",
+                "GW = sample[\"GW\"].T\n",
+                "G = sample[\"G\"]\n",
+                "H = to_vec(sample[\"H\"])\n",
+                "X = to_vec(sample[\"X\"])\n",
+                "Xdot = to_vec(sample[\"Xdot\"])\n",
+                "shape_2d = sample[\"shape_2d\"]\n",
+                "\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# II. Select areas for bckgd fitting\n",
-                "\n",
-                "\u26a0\ufe0f Input in the ``span_number`` the number of selection areas you wish to use. Once you execute the cell, a window will pop with a few green areas and a red spectrum. The green areas correspond to the regions were the background will be fitted. You can, drag, enlarge and reduce these green areas."
+                "Let us look at the dimension of our problem."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "span_number = 4\n",
-                "\n",
-                "def selection_areas(number,spectrum,scale) :\n",
-                "    spectrum.plot()\n",
-                "    size = spectrum.axes_manager[0].size //(2*number)\n",
-                "    roi_list = []\n",
-                "    for i in range(number) :\n",
-                "        roi_list.append(hs.roi.SpanROI(offset+ size*scale + 2*i*size*scale, 2*size*scale + offset+ 2*i*size*scale))\n",
-                "        roi_list[-1].interactive(spectrum)\n",
-                "    return roi_list\n",
-                "\n",
-                "spans = selection_areas(span_number,spectrum,scale)"
+                "print(f\"\"\"\n",
+                "- X: {X.shape}\n",
+                "- Xdot: {Xdot.shape}\n",
+                "- G: {G.shape}\n",
+                "- GW: {GW.shape}\n",
+                "- H: {H.shape}\n",
+                "- shape_2d: {shape_2d}\n",
+                "\"\"\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Once you are satisfied with the selected areas, save their positions using the cell below"
+                "Here `Xdot` contains the noisless data such that the ground truth `H` and `GW` satisfies:\n",
+                "$$X = GWH$$"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "list_energies = [[roi.left,roi.right] for roi in spans]"
+                "np.testing.assert_allclose(Xdot, GW @ H)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# III. Fitting the continuum\n",
-                "\n",
-                "\u26a0\ufe0f Input the sample parameters below and execute the cell to fit"
+                "Let us plot the ground truth maps $H$ (sometimes also called weights). Here the variable `shape_2d` is used to reshape the columns of $H$ into images."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "thickness = 50e-7\n",
-                "density = 5.11\n",
-                "take_off_angle = 24\n",
-                "elements_dict = {\"Sr\" : 0.25, \"Ti\" : 0.25, \"O\" : 0.5}\n",
-                "detector = \"SDD_efficiency.txt\"\n",
-                "\n",
-                "#################################################################################################\n",
-                "# For a custom detector, uncomment below and replace \"SDD_efficiency.txt\" with the dictionnary. #\n",
-                "#################################################################################################\n",
-                "\n",
-                "# {\"detection\" : {\n",
-                "#     \"thickness\" : 450e-4,\n",
-                "#     \"elements_dict\" : {\n",
-                "#         \"Si\" : 1.0\n",
-                "#     }\n",
-                "# },\"layer\" : {\n",
-                "#     \"thickness\" : 10e-7,\n",
-                "#     \"elements_dict\" : {\n",
-                "#         \"Si\" : 0.33,\n",
-                "#         \"O\" : 0.66,\n",
-                "#         \"Al\" : 1.0\n",
-                "#     }\n",
-                "# }}\n",
                 "\n",
-                "part_x, part_y, sum_boola = sf.make_partial_xy(list_energies,spectrum,x)\n",
-                "\n",
-                "example = {\n",
-                "    \"b0\" : 1.0,\n",
-                "    \"b1\" : 1.0,\n",
-                "    \"params_dict\" : {\n",
-                "    \"Det\" : detector,\n",
-                "    'Abs' : {\n",
-                "        \"thickness\" : thickness,\n",
-                "        \"toa\" : take_off_angle,\n",
-                "        \"density\" : density,\n",
-                "        \"atomic_fraction\" : True},\n",
-                "        \"elements_dict\" : elements_dict\n",
-                "    }\n",
-                "}\n",
-                "\n",
-                "pars = sf.ndict_to_params(example)\n",
-                "\n",
-                "#################################################################################################\n",
-                "# You can uncomment the lines below if you want to add constraints to the absorption parameters #\n",
-                "#################################################################################################\n",
-                "\n",
-                "# pars[\"params_dict__Abs__thickness\"].vary = False\n",
-                "# pars[\"params_dict__Abs__thickness\"].max = 5000e-7\n",
-                "# pars[\"params_dict__Det__layer__thickness\"].vary = False\n",
-                "pars[\"params_dict__Abs__toa\"].vary = False\n",
-                "pars[\"params_dict__Abs__density\"].vary = False\n",
-                "\n",
-                "out = lm.minimize(sf.residual, pars, args=(part_x,), kws={'data': part_y})\n",
-                "print(lm.fit_report(out))"
+                "vmin, vmax = 0,1\n",
+                "cmap = plt.cm.gray_r\n",
+                "plt.figure(figsize=(10, 3))\n",
+                "for i, hdot in enumerate(H):\n",
+                "    plt.subplot(1,3,i+1)\n",
+                "    plt.imshow(H[i].reshape(shape_2d), cmap=cmap, vmin=vmin, vmax=vmax)\n",
+                "    plt.axis(\"off\")\n",
+                "    plt.title(f\"GT - Map {i+1}\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Plotting the results\n",
-                "\n",
-                "The red curves corresponds to the background model, the black one to the data, and the grey area correspond to the selected green areas"
+                "We can also plot the phases corresponding to these maps. The phases corresponds to the matrix $GW$."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "y = spectrum.data\n",
-                "bkgd = sf.residual(out.params,x)\n",
-                "plt.plot(x,y,\"ko-\",markersize=1.5,label=\"exp\",markevery=10)\n",
-                "plt.fill_between(x,0,y,where=sum_boola,label=\"fit windows\",color=\"0.8\")\n",
-                "plt.xlabel(\"Energy (keV)\",fontsize=22)\n",
-                "plt.xticks(fontsize=20)\n",
-                "# plt.ylim(0,1)\n",
-                "plt.yticks(fontsize=20)\n",
-                "plt.ylabel(\"Intensity\",fontsize=22)\n",
-                "plt.plot(x,bkgd,\"r-\",linewidth=1,label=\"fit\")\n",
-                "plt.legend(fontsize=22)"
+                "e = np.linspace(0,1, GW.shape[0])\n",
+                "plt.plot(e, GW)\n",
+                "plt.title(\"GT - Phases\")\n",
+                "plt.xlabel(\"Frequency [normalized]\")\n",
+                "plt.legend([f\"phase {i+1}\" for i in range(3)]);"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# VI. Select the interesting part of the spectrum\n",
-                "\n",
-                "\u26a0\ufe0f A window will pop up with a red spectrum and a green area. With the green areas, you can select the energy range you want to quantify. Usually the low energy region (below 1keV) is not very well fitted by the background model. Hence you probably want to avoid the quantification of low energy characteristic X rays. "
+                "The matrix $G$ is assumed to be known appriori. Here we plot the first 5 lines of $G$."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "s_bkgd = hs.signals.Signal1D(bkgd)\n",
-                "s_bkgd.axes_manager[0].offset = offset\n",
-                "s_bkgd.axes_manager[0].scale = scale\n",
-                "\n",
-                "spectrum.plot()\n",
-                "ax = spectrum._plot.signal_plot.ax\n",
-                "ax.add_line(matplotlib.lines.Line2D(spectrum._plot.axis.axis,bkgd.data))\n",
-                "roi = hs.roi.SpanROI(200*scale,400*scale)\n",
-                "roi.interactive(spectrum)"
+                "l = np.linspace(0, 1,n)\n",
+                "plt.plot(l, G[:,:5]);"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Accepting the choice of quantification energy range"
+                "Note that the function `create_toy_sample` did not return $W$ but only $GW$. \n",
+                "\n",
+                "Using the ground truth $GW$, it can be computed as follows:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "charac_xrays = (spectrum.isig[roi.left:roi.right].data - s_bkgd.isig[roi.left:roi.right].data).clip(min=0)\n",
-                "new_offset = spectrum.isig[roi.left:roi.right].axes_manager[0].offset\n",
-                "new_size = spectrum.isig[roi.left:roi.right].axes_manager[0].size"
+                "W = np.linalg.lstsq(GW, G, rcond=None)[0].T\n",
+                "W.shape"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# VIII. Fitting the characteristic Xrays"
+                "## Solving the problem"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Initialisation of the characteristic Xray model\n",
-                "\u26a0\ufe0f Put the list of elements (by atomic numbers) you want to quantify in ``elt_list``. \n",
-                "\n",
-                "``G_calib`` is a small offset you may want to add so that the peaks are at the right energy. \n",
+                "#### Parameters\n",
                 "\n",
-                "Note that depending on the energy range you chose, not all the elements you put are fitted (e.g. Oxygen will not be taken into account if your energy range starts at 1 keV)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "elt_list = [\"Sr\", \"Ti\"]\n",
-                "G_calib = -0.005\n",
-                "db =  \"default_xrays.json\" # \"300kv_xrays.json\" \n",
-                "\n",
-                "params_dict = {\n",
-                "    \"Abs\" : {\n",
-                "        \"thickness\" : thickness,\n",
-                "        \"density\" : density,\n",
-                "        \"toa\" : take_off_angle\n",
-                "    },\n",
-                "    \"Det\" : detector\n",
-                "}\n",
-                "\n",
-                "true_elt_list = []\n",
-                "for elt in elt_list : \n",
-                "    mod_t = edxs.EDXS(new_offset,new_size,scale,{},db_name = db)\n",
-                "    mod_t.generate_g_matr(elements = [elt],norm=False, g_type = \"no_brstlg\")\n",
-                "    G_t = mod_t.G\n",
-                "    if G_t.shape[1] == 1 : \n",
-                "        true_elt_list.append(elt)\n",
-                "    \n",
-                "mod = edxs.EDXS(new_offset + G_calib,new_size,scale,params_dict,db_name = db)\n",
-                "mod.generate_g_matr(elements = true_elt_list,norm=False, g_type = \"no_brstlg\")\n",
-                "G = mod.G\n",
-                "new_x = np.linspace(new_offset,new_size*scale+new_offset,num = new_size)\n",
-                "print(\"List of elements with Xray lines in the energy range :\")\n",
-                "print(true_elt_list)"
+                "Let us define the different hyperparameters of the problem. Feel free to change them and see how the results change."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Fitting the characteristic Xrays"
+                "Let us first define our regularisation parameters."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "estimator = SmoothNMF(G=G,n_components= 1,max_iter=2000,force_simplex = True,tol = 1e-8,hspy_comp = False)\n",
-                "estimator.fit_transform(charac_xrays[:,np.newaxis], H=np.array([1])[:,np.newaxis])\n",
-                "W = estimator.W_"
+                "lambda_L = 2 # Smoothness of the maps\n",
+                "mu = 0.05 # Sparsity of the maps"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# IX. Plot the results\n",
-                "\n",
-                "\u26a0\ufe0f The popping window will display the bkgd substracted experimental spectrum, the fitted characteristic Xrays model in black and red. Every element composing the model will be displayed with an offset : ``components_offset``. You can change its value below. \n",
-                "\n",
-                "If you want to display the names of the lines of an element that was used for quantification execute the next cells below before kill the window."
+                "We can additionally add a simplex constraint to the problem by setting `simplex_H=True`. This will add the constraint that the line of $H$ sum to 1. This constraint should be activated for the regularizers to work!. Practically, it will prevent the algorithm from simply minimizing $W$ and increasing $H$."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "components_offset = -0.1"
+                "simplex_H = True\n",
+                "simplex_W = False\n"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Finally, we can decide to specify $G$ or not. If the matrix $G$ is not specified, the algorithm will directly estimate $GW$ insead of $W$."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "linestyles = [\":\",\"--\",\"-.\"]\n",
-                "\n",
-                "plt.plot(new_x,charac_xrays,\"ko-\",label=\"exp\",markevery = 10)\n",
-                "plt.plot(new_x,G@W,\"r\",linewidth = 3,label=\"theo\")\n",
-                "plt.xticks(fontsize = 16)\n",
-                "plt.yticks(fontsize = 16)\n",
-                "plt.xlabel(\"energy (keV)\",fontsize = 18)\n",
-                "plt.ylabel(\"Intensity\", fontsize = 18)\n",
-                "\n",
-                "for i in range(G.shape[1]) :\n",
-                "    ls_string = linestyles[i%len(linestyles)] + \"C{}\".format(i%9)\n",
-                "    plt.plot(new_x,G[:,i]*W[i]+components_offset,ls_string,label=str(true_elt_list[i]),linewidth=3)\n",
-                "\n",
-                "\n",
-                "plt.legend(fontsize=18)\n",
-                "plt.tight_layout()"
+                "Gused = G"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# X. Printing the concentrations"
+                "Note that wihtout regularisation, i.e. with the parameters\n",
+                "```python\n",
+                "lambda_L = 0\n",
+                "mu = 0 \n",
+                "Gused = None\n",
+                "simplex_H=False\n",
+                "simplex_W = False\n",
+                "``` \n",
+                "we recover the classical Poisson/KL NMF problem. Our algorithm will apply the MU algorithm from Lee and Seung (2001)."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Full summary of normalized concentrations."
+                "Let us define the parameters for the algorithm. Here the class `espm.estimator.SmoothNMF` heritates from sckit-learn's `NMF` class. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "print_concentrations_from_W(W,elements = true_elt_list)"
+                "\n",
+                "K = len(H) # Number of components / let assume that we know it\n",
+                "params = {}\n",
+                "params[\"tol\"]=1e-6 # Tolerance for the stopping criterion.\n",
+                "params[\"max_iter\"] = 200 # Maximum number of iterations before timing out.\n",
+                "params[\"hspy_comp\"] = False # If should be set to True if hspy data format is used.\n",
+                "params[\"verbose\"] = 1 # Verbosity level.\n",
+                "params[\"eval_print\"] = 10 # Print the evaluation every eval_print iterations.\n",
+                "params[\"epsilon_reg\"] = 1 # Regularization parameter \n",
+                "params[\"linesearch\"] = False # Use linesearch to accelerate convergence\n",
+                "params[\"shape_2d\"] = shape_2d # Shape of the 2D maps\n",
+                "params[\"n_components\"] = K # Number of components\n",
+                "params[\"normalize\"] = True # Normalize the data. It helps to keep the range of the regularization parameters lambda_L and mu in a reasonable range.\n",
+                "\n",
+                "estimator = SmoothNMF(mu=mu, lambda_L=lambda_L, G = Gused, simplex_H=simplex_H, simplex_W=simplex_W, **params)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "\u26a0\ufe0f You can remove some elements of the results, normalizing on the remaining elements."
+                "The function `fit_transform` will solve the problem and return the matrix $GW$."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ignored_elts = [\"Mg\"]\n",
-                "\n",
-                "inds = [true_elt_list.index(elt) for elt in ignored_elts]\n",
-                "remain_elt_list = [v for i,v in enumerate(true_elt_list) if i not in frozenset(inds)] \n",
-                "remain_W = np.delete(W, inds, axis=0)\n",
-                "r = remain_W / remain_W.sum(axis=0)\n",
-                "\n",
-                "print_concentrations_from_W(r,remain_elt_list)"
+                "GW_est = estimator.fit_transform(X)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# VI. Select the interesting part of the spectrum\n",
-                "\n",
-                "\u26a0\ufe0f A window will pop up with a red spectrum and a green area. With the green areas, you can select the energy range you want to quantify. Usually the low energy region (below 1keV) is not very well fitted by the background model. Hence you probably want to avoid the quantification of low energy characteristic X rays. "
+                "We can plot the different losses to see how the algorithm converges."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "s_bkgd = hs.signals.Signal1D(bkgd)\n",
-                "s_bkgd.axes_manager[0].offset = offset\n",
-                "s_bkgd.axes_manager[0].scale = scale\n",
                 "\n",
-                "spectrum.plot()\n",
-                "ax = spectrum._plot.signal_plot.ax\n",
-                "ax.add_line(matplotlib.lines.Line2D(spectrum._plot.axis.axis,bkgd.data))\n",
-                "roi = hs.roi.SpanROI(200*scale,400*scale)\n",
-                "roi.interactive(spectrum)"
+                "losses = estimator.get_losses()\n",
+                "\n",
+                "values, names = process_losses(losses)\n",
+                "\n",
+                "plt.figure(figsize=(10, 6))\n",
+                "for name, value in zip(names[:4], values[:4]):\n",
+                "    plt.plot(value, label=name)\n",
+                "    plt.xlabel(\"iteration\")\n",
+                "plt.yscale(\"log\")\n",
+                "plt.legend()\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "charac_xrays = (spectrum.isig[roi.left:roi.right].data - s_bkgd.isig[roi.left:roi.right].data).clip(min=0)\n",
-                "new_offset = spectrum.isig[roi.left:roi.right].axes_manager[0].offset\n",
-                "new_size = spectrum.isig[roi.left:roi.right].axes_manager[0].size"
+                "losses[0]"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "\u26a0\ufe0f If you want to fix the values of P you obtained in a previous fit put them in ``fixed_elts`` and execute the two following cells. \n",
-                "\n",
-                "For a two steps quantification : Chose a first energy range. Perform a first fit, which initialise P with all the elements. Then go back to the energy range selection, ignore the cell above, chose the fixed elements and perform the fit with fixed elements below. "
+                "We can easily recover $W$ and $H$ from the estimator."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(\"Previous Values for W\")\n",
-                "for i,elt in enumerate(true_elt_list) : \n",
-                "    print(elt, \" : \", W[i])"
+                "H_est = estimator.H_\n",
+                "W_est = estimator.W_"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "fixed_elts = {\"p1\" : {\"Cl\" : 4.26588157e+18}}\n",
+                "Let us compute some metrics to evaluate the quality of the solution. We will use the metrics defined in the module `espm.metrics`.\n",
                 "\n",
-                "dummy_spim = spim.EDS_espm(np.array([1]))\n",
-                "dummy_spim.add_elements(elements = true_elt_list)\n",
-                "dummy_spim.problem_type = \"no_brstlg\"\n",
-                "\n",
-                "fixed_W = dummy_spim.set_fixed_W(fixed_elts)"
+                "We first compute the angles between the phases `GW` and the estimated phases `GW_est`. The angles are computed using the function `compute_angles`. This function also return the indices to match the estimations and the ground truths. Indeed, there is no reason for them to have the same order. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "estimator = NMF(G=G,n_components= 1,max_iter=2000,force_simplex = True,tol = 1e-8,hspy_comp = False,fixed_W = fixed_W)\n",
-                "estimator.fit_transform(charac_xrays[:,np.newaxis], H=np.array([1])[:,np.newaxis])\n",
-                "new_W = estimator.W_"
+                "angles, true_inds = find_min_angle(GW.T, GW_est.T, unique=True, get_ind=True)\n",
+                "print(\"angles : \", angles)"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Now, we can compute the Mean Squared Error (MSE) between the maps `H` and the estimated maps `H_est`. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "print_concentrations_from_W(new_W,elements = true_elt_list)"
+                "mse = ordered_mse(H, H_est, true_inds)\n",
+                "print(\"mse : \", mse)"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Finally, let us plot the results. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "nbsphinx-thumbnail"
+                ]
+            },
             "outputs": [],
             "source": [
-                "ignored_elts = [\"Mg\"]\n",
                 "\n",
-                "inds = [true_elt_list.index(elt) for elt in ignored_elts]\n",
-                "remain_elt_list = [v for i,v in enumerate(true_elt_list) if i not in frozenset(inds)] \n",
-                "remain_W = np.delete(new_W, inds, axis=0)\n",
-                "r = remain_W / remain_W.sum(axis=0)\n",
-                "print_concentrations_from_W(r,elements = true_elt_list)"
+                "def plot_results(Ddot, D, Hdotflat, Hflat):\n",
+                "    fontsize = 30\n",
+                "    scale = 15\n",
+                "    aspect_ratio = 1.4\n",
+                "    marker_list = [\"-o\",\"-s\",\"->\",\"-<\",\"-^\",\"-v\",\"-d\"]\n",
+                "    mark_space = 20\n",
+                "    # cmap = plt.cm.hot_r    \n",
+                "    cmap = plt.cm.gray_r\n",
+                "    vmax = 1\n",
+                "    vmin = 0\n",
+                "    K = len(H)\n",
+                "    L = len(D)\n",
+                "    \n",
+                "    angles, true_inds = find_min_angle(Ddot.T, D.T, unique=True, get_ind=True)\n",
+                "    mse = ordered_mse(Hdotflat, Hflat, true_inds)\n",
+                "    mae = ordered_mae(Hdotflat, Hflat, true_inds)\n",
+                "    r2 = ordered_r2(Hdotflat, Hflat, true_inds)\n",
+                "\n",
+                "\n",
+                "    fig, axes = plt.subplots(K,3,figsize = (scale/K * 3 * aspect_ratio,scale))\n",
+                "    x = np.linspace(0,1, num = L)\n",
+                "    for i in range(K): \n",
+                "        axes[2,i].plot(x,Ddot.T[i,:],'g-',label='ground truth',linewidth=4)\n",
+                "        axes[2,i].plot(x,D[:,true_inds[i]],'r--',label='reconstructed',linewidth=4)\n",
+                "        axes[2,i].set_title(\"{:.2f} deg\".format(angles[i]),fontsize = fontsize-2)\n",
+                "        axes[2,i].set_xlim(0,1)\n",
+                "\n",
+                "        axes[1,i].imshow((Hflat[true_inds[i],:]).reshape(shape_2d),vmin = vmin, vmax = vmax , cmap=cmap)\n",
+                "        axes[1,i].set_title(\"R2: {:.2f}\".format(r2[true_inds[i]]),fontsize = fontsize-2)\n",
+                "        # axes[i,1].set_ylim(0.0,1.0)\n",
+                "        axes[1,i].tick_params(axis = \"both\",labelleft = False, labelbottom = False,left = False, bottom = False)\n",
+                "\n",
+                "        im = axes[0,i].imshow(Hdotflat[i].reshape(shape_2d),vmin = vmin, vmax = vmax, cmap=cmap)\n",
+                "        axes[0,i].set_title(\"Phase {}\".format(i),fontsize = fontsize)\n",
+                "        axes[0,i].tick_params(axis = \"both\",labelleft = False, labelbottom = False,left = False, bottom = False)\n",
+                "        axes[2,0].legend()\n",
+                "\n",
+                "    rows = [\"True maps\",\"Reconstructed maps\",\"Spectra\"]\n",
+                "\n",
+                "    for ax, row in zip(axes[:,0], rows):\n",
+                "        ax.set_ylabel(row, rotation=90, fontsize=fontsize)\n",
+                "\n",
+                "\n",
+                "    fig.subplots_adjust(right=0.84)\n",
+                "    # put colorbar at desire position\n",
+                "    cbar_ax = fig.add_axes([0.85, 0.5, 0.01, 0.3])\n",
+                "    fig.colorbar(im,cax=cbar_ax)\n",
+                "\n",
+                "    # fig.tight_layout()\n",
+                "\n",
+                "    print(\"angles : \", angles)\n",
+                "    print(\"mse : \", mse)\n",
+                "    print(\"mae : \", mae)\n",
+                "    print(\"r2 : \", r2)\n",
+                "\n",
+                "    return fig\n",
+                "\n",
+                "fig = plot_results(GW, GW_est, H, H_est)\n",
+                "plt.show()  \n"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3.10.6 ('espm')",
+            "display_name": "espm",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.6"
+            "version": "3.11.8"
         },
         "vscode": {
             "interpreter": {
-                "hash": "8d2c37261bd18724b44288178b5d93ac658e7a29aba4ea6c1b1b0710c1696ef2"
+                "hash": "8d9f0750808bbb89d6238996d547b1a0ab25cae94b245e8c4572708d26b443fd"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `espm-1.0.0/notebooks/convergence-speed.ipynb` & `espm-1.1.1/notebooks/convergence-speed.ipynb`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.97472223513608%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, '\\n')], delete: [9, 8, 7, 6, 5, 4, 3, 2]}}, 2: "*

 * *            '{\'source\': {insert: [(0, \'naming_hash = {}\\n\'), (1, \'naming_hash["log_surrogate '*

 * *            '- no linesearch"] = "MU update\\\\nno linesearch"\\n\'), (2, '*

 * *            '\'naming_hash["log_surrogate -  linesearch"] = "MU update\\\\nlinesearch"\\n\'), (3, '*

 * *            '\'naming_hash["l2_surrogate - no linesearch"] = "Quadratic update\\\\nno '*

 * *            'linesearch"\\n\'), (4, \'naming_hash["l2_s […]*

```diff
@@ -15,413 +15,304 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
-                "# from snmfem.experiments import load_samples, print_results, load_data, run_experiment\n",
-                "from espm.measures import KL, trace_xtLx\n",
-                "from espm.estimators.updates import multiplicative_step_h, multiplicative_step_w, multiplicative_step_hq\n",
-                "from espm.conf import log_shift, dicotomy_tol, sigmaL\n",
-                "from espm.utils import create_laplacian_matrix\n",
-                "from espm.estimators.smooth_nmf import diff_surrogate\n",
-                "from espm.estimators import SmoothNMF\n",
-                "from copy import deepcopy\n"
+                "\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "def create_toy_problem(l = 25, k = 3, p = 100, c = 10, n_poisson=200, force_simplex=True):\n",
-                "\n",
-                "    A = np.random.rand(k,p)\n",
-                "    if force_simplex:\n",
-                "        A = A/np.sum(A, axis=0, keepdims=True)\n",
-                "    \n",
-                "    G = np.random.rand(l,c)\n",
-                "    P = np.random.rand(c,k)\n",
-                "    GP = G @ P\n",
-                "\n",
-                "    X = GP @ A\n",
+                "naming_hash = {}\n",
+                "naming_hash[\"log_surrogate - no linesearch\"] = \"MU update\\nno linesearch\"\n",
+                "naming_hash[\"log_surrogate -  linesearch\"] = \"MU update\\nlinesearch\"\n",
+                "naming_hash[\"l2_surrogate - no linesearch\"] = \"Quadratic update\\nno linesearch\"\n",
+                "naming_hash[\"l2_surrogate -  linesearch\"] = \"Quadratic update\\nlinesearch\"\n",
+                "naming_hash[\"bmd - no linesearch\"] = \"Block Mirror Descent\\nno linesearch\"\n",
+                "naming_hash[\"bmd -  linesearch\"] = \"Block Mirror Descent\\nlinesearch\"\n",
+                "naming_hash[\"projected_gradient - no linesearch\"] = \"Projected gradient\\nno linesearch\"\n",
+                "naming_hash[\"projected_gradient -  linesearch\"] = \"Projected gradient\\nlinesearch\"\n",
                 "\n",
-                "    Xdot = 1/n_poisson * np.random.poisson(n_poisson * X)\n",
-                "\n",
-                "    return G, P, A, X, Xdot"
+                "# Define colors for each method\n",
+                "colors = {}\n",
+                "colors[\"log_surrogate - no linesearch\"] = \"blue\"\n",
+                "colors[\"log_surrogate -  linesearch\"] = \"darkblue\"\n",
+                "colors[\"l2_surrogate - no linesearch\"] = \"lightgreen\"\n",
+                "colors[\"l2_surrogate -  linesearch\"] = \"darkgreen\"\n",
+                "colors[\"bmd - no linesearch\"] = \"red\"\n",
+                "colors[\"bmd -  linesearch\"] = \"pink\"\n",
+                "colors[\"projected_gradient - no linesearch\"] = \"orange\"\n",
+                "colors[\"projected_gradient -  linesearch\"] = \"violet\""
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "def one_experiment(X, W0, H0, experiment_param, algo_param, global_param):\n",
-                "    est = SmoothNMF(**algo_param, **experiment_param, **global_param)\n",
-                "    W = est.fit_transform(X, W=W0, H=H0)\n",
-                "    H = est.H_\n",
-                "    losses = est.get_losses()\n",
-                "    loss = losses[\"full_loss\"].copy()\n",
-                "    final_loss = loss[-1]\n",
-                "    gamma = losses[\"gamma\"].copy()\n",
-                "    return loss, final_loss, W.copy(), H.copy(), gamma"
+                "## Paper plots"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# global parameters\n",
-                "global_param = dict()\n",
-                "global_param[\"l2\"] = False\n",
-                "global_param[\"verbose\"]= 0\n",
-                "global_param[\"tol\"] = 0\n",
-                "global_param[\"max_iter\"] = 1000\n",
-                "global_param[\"dicotomy_tol\"] = dicotomy_tol\n",
-                "global_param[\"debug\"] = False\n",
-                "global_param[\"log_shift\"] = log_shift\n",
-                "global_param[\"eval_print\"] = 10\n",
-                "global_param[\"hspy_comp\"] = False"
+                "from pathlib import Path\n",
+                "pathfig = Path('./figures/')\n",
+                "pathfig.mkdir(exist_ok=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "force_simplex = True\n",
+                "for laplacian in [False, True]:\n",
+                "    for noise in [False, True]:\n",
+                "        # load data \n",
+                "        filename = f\"losses_{laplacian}_{noise}_{force_simplex}.npz\"\n",
+                "        data = np.load(filename, allow_pickle=True)\n",
+                "        losses = data[\"losses\"]\n",
+                "        l_infty = data[\"l_infty\"]\n",
+                "        params = data[\"params\"]\n",
+                "        captions = [naming_hash[d] for d in data[\"captions\"]]\n",
+                "        cs = [colors[d] for d in data[\"captions\"]]\n",
+                "        true_D = data[\"true_D\"]\n",
+                "        true_H = data[\"true_H\"]\n",
+                "        X = data[\"X\"]\n",
+                "        Xdot = data[\"Xdot\"]\n",
+                "        W = data[\"W\"]\n",
+                "        H = data[\"H\"]\n",
+                "        gammas = data[\"gammas\"]\n",
+                "        shape_2d = params[0][0][\"shape_2d\"]\n",
+                "        k = H.shape[0]\n",
+                "        times = data[\"times\"]\n",
+                "        print(len(losses))\n",
+                "        losses = np.mean(losses-l_infty.reshape(-1, 1, 1), axis=0)\n",
                 "\n",
-                "shape_2d = [10, 15]\n",
-                "k = 5\n",
-                "n_poisson = 200\n",
-                "G, P, A, Xtrue, X = create_toy_problem(p = shape_2d[0]*shape_2d[1], k=k, n_poisson=n_poisson)\n",
-                "\n",
-                "true_D = G @ P\n",
-                "true_H = A\n",
                 "\n",
-                "# X = Xtrue\n",
-                "L = create_laplacian_matrix(*shape_2d)\n",
-                "lambda_L = 20\n",
+                "        plt.figure(figsize=[8, 4])\n",
+                "        for loss, caption, color in zip(losses, captions, cs):\n",
+                "            iterations = np.arange(len(loss))+1\n",
+                "            if len(iterations)>10:\n",
+                "                plt.plot(iterations, loss, \".-\", color=color,  label=caption)\n",
+                "        max_y = np.max(losses)\n",
+                "        min_y = np.min(losses)\n",
+                "        plt.ylim([min_y, max_y])\n",
+                "        plt.xlim([1, losses.shape[1]])\n",
+                "        plt.yscale(\"log\")\n",
+                "        plt.xscale(\"log\")\n",
+                "        plt.xlabel(\"Iterations\")\n",
+                "        plt.legend(loc=\"lower left\")\n",
                 "\n",
-                "W0 = np.random.rand(*true_D.shape)\n",
-                "H0 = np.random.rand(*A.shape)"
+                "        fig = plt.gcf()\n",
+                "        filename = f\"convergence_{'' if laplacian else 'no_'}laplacian_{'' if noise else 'no_'}noise.pdf\"\n",
+                "        fig.savefig(pathfig / Path(filename), bbox_inches='tight')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "\n",
-                "# experiment parameters\n",
-                "experiment_param = dict()\n",
-                "experiment_param[\"force_simplex\"] = False\n",
-                "experiment_param[\"lambda_L\"] = lambda_L \n",
-                "experiment_param[\"mu\"] = 0\n",
-                "experiment_param[\"epsilon_reg\"] = 1\n",
-                "experiment_param[\"normalize\"] = False\n",
-                "experiment_param[\"G\"] = None\n",
-                "experiment_param[\"shape_2d\"] = shape_2d\n",
-                "experiment_param[\"n_components\"] = k\n",
-                "experiment_param[\"true_D\"] = true_D\n",
-                "experiment_param[\"true_H\"] = true_H"
+                "def upper_lower_error(x):\n",
+                "    m = np.mean(x, axis=0, keepdims=True)\n",
+                "    xc = x - m\n",
+                "    upper = []\n",
+                "    n_up = []\n",
+                "    lower = []\n",
+                "    n_low = []\n",
+                "    for i in range(xc.shape[1]):\n",
+                "        n_up.append(np.sum(xc[:,i]>=0))\n",
+                "        upper.append(np.sum((xc[:,i][xc[:,i]>=0])**2))\n",
+                "        n_low.append(np.sum(xc[:,i]<0))\n",
+                "        lower.append(np.sum((xc[:,i][xc[:,i]<0])**2))\n",
+                "    return np.sqrt(np.array(lower)), np.sqrt(np.array(upper))\n",
+                "    # return np.sqrt(np.array(lower))/np.sqrt(n_low), np.sqrt(np.array(upper))/np.sqrt(n_up)\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "losses = []\n",
-                "final_losses = []\n",
-                "Ws = []\n",
-                "Hs = []\n",
-                "params = []\n",
-                "captions = []\n",
-                "gammas = []\n",
-                "for algo in [\"log_surrogate\", \"l2_surrogate\", \"projected_gradient\"]:\n",
-                "    for linesearch in [False, True]:\n",
-                "        # for sL in [sigmaL/4, sigmaL/2, sigmaL]:\n",
-                "        for sL in [sigmaL]:\n",
-                "            # algo parameters\n",
-                "            algo_param = dict()\n",
-                "            algo_param[\"linesearch\"] = linesearch\n",
-                "            algo_param[\"algo\"] = algo\n",
-                "            # algo_param[\"gamma\"] = sL\n",
-                "            if algo == \"projected_gradient\":\n",
-                "                algo_param[\"gamma\"] = [500*sL, 500*sL]\n",
-                "            else:\n",
-                "                algo_param[\"gamma\"] = sL\n",
+                "for l in [25, 100, 500, 1000]:\n",
+                "    shift = 0\n",
+                "    plt.figure(figsize=[6, 3])\n",
+                "    for laplacian in [True, False]:\n",
+                "        for noise in [False, True]:\n",
+                "            filename = f\"losses_{laplacian}_{noise}_{force_simplex}_{l}.npz\"\n",
+                "            data = np.load(filename, allow_pickle=True)\n",
+                "            captions = [naming_hash[d] for d in data[\"captions\"]]\n",
+                "\n",
+                "            times = data[\"times\"]\n",
+                "            times = np.mean(times, axis=0)\n",
+                "            # times_std = np.std(times, axis=0) / np.sqrt(times.shape[0])\n",
+                "            lower_error, upper_error = upper_lower_error(data[\"times\"])\n",
+                "            asymmetric_error = np.array(list(zip(lower_error, upper_error))).T\n",
+                "            X_axis = np.arange(len(captions))\n",
+                "            # plt.boxplot(data[\"times\"],positions=X_axis-0.3+shift, widths=0.2);\n",
+                "            plt.bar(X_axis - 0.3 + shift, times, 0.2, yerr=asymmetric_error, ecolor='black', capsize=3, label = f\"{'Smooth' if laplacian else 'random'} nois{'y' if noise else 'less'} data\")\n",
+                "            # plt.bar(X_axis - 0.3 + shift, times, 0.2, ecolor='black', capsize=3, label = f\"{'Smooth' if laplacian else 'random'} nois{'y' if noise else 'less'} data\")\n",
+                "            shift += 0.2\n",
                 "\n",
-                "            loss, final_loss, W, H, gamma = one_experiment(X, W0, H0, experiment_param, algo_param, global_param)\n",
-                "            losses.append(loss)\n",
-                "            final_losses.append(final_loss)\n",
-                "            params.append([experiment_param, algo_param, global_param])\n",
-                "            Ws.append(W)\n",
-                "            Hs.append(H)\n",
-                "            gammas.append(gamma)\n",
-                "            cl = \"\" if linesearch else \"no\"\n",
-                "            captions.append(f\"{algo} - {cl} linesearch - $\\gamma_0$={sL}\")\n",
-                "            # captions.append(f\"{algo} - {cl} linesearch\")\n",
+                "    plt.xticks(X_axis, captions)\n",
+                "    plt.xticks(rotation=45, ha=\"right\")\n",
+                "    plt.xlabel(\"Algorithm\")\n",
+                "    plt.ylabel(\"Seconds\")\n",
+                "    plt.title(\"n = \"+str(int(l)))\n",
+                "    plt.legend()\n",
                 "\n",
-                "i = np.argmin(final_losses)\n",
-                "global_param_m = deepcopy(global_param)\n",
-                "global_param_m[\"max_iter\"] = global_param_m[\"max_iter\"]*3\n",
-                "_, l_infty, _, _, _ = one_experiment(X, Ws[i], Hs[i], experiment_param, params[i][1], global_param_m)        "
+                "    fig = plt.gcf()\n",
+                "    filename = f\"speed_comparison_{l}.pdf\"\n",
+                "    fig.savefig(pathfig / Path(filename), bbox_inches='tight')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plt.figure(figsize=[10, 6])\n",
-                "# plt.figure(figsize=[15, 10])\n",
+                "filename = f\"losses_{False}_{False}_{True}_100.npz\"\n",
+                "data = np.load(filename, allow_pickle=True)\n",
+                "captions = [naming_hash[d] for d in data[\"captions\"]]\n",
                 "\n",
-                "for loss, caption in zip(losses, captions):\n",
-                "    iterations = np.arange(len(loss))+1\n",
-                "    if len(iterations)>10:\n",
-                "        plt.plot(iterations, loss-l_infty, \".-\", label=caption)\n",
-                "plt.yscale(\"log\")\n",
-                "plt.xscale(\"log\")\n",
-                "plt.xlabel(\"Iterations\")\n",
-                "plt.legend()"
+                "times = data[\"times\"]\n",
+                "\n",
+                "plt.plot(times)\n",
+                "plt.legend(captions)"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "for gamma, caption in zip(gammas, captions):\n",
-                "    iterations = np.arange(len(gamma))+1\n",
-                "\n",
-                "    plt.plot(iterations, gamma, \".\", label=caption)\n",
-                "plt.legend()\n"
+                "### Individual experiment"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "\n",
-                "shape_2d = [10, 15]\n",
-                "k = 5\n",
-                "n_poisson = 200\n",
-                "G, P, A, Xtrue, X = create_toy_problem(p = shape_2d[0]*shape_2d[1], k=k, n_poisson=n_poisson)\n",
-                "\n",
-                "# X = Xtrue\n",
-                "L = create_laplacian_matrix(*shape_2d)\n",
-                "lambda_L = 20\n",
-                "\n",
-                "W1 = np.random.rand(*P.shape)\n",
-                "H1 = np.random.rand(*A.shape)\n",
-                "# H1 = H1/np.sum(H1, axis=0, keepdims=True)\n",
-                "W2 = W1.copy()\n",
-                "H2 = H1.copy()\n",
-                "\n",
-                "W3 = W1.copy()\n",
-                "H3 = H1.copy()\n",
-                "\n",
-                "H4 = H1.copy()\n",
-                "W4 = W1.copy()\n",
-                "\n",
-                "H5 = H1.copy()\n",
-                "W5 = W1.copy()\n",
-                "\n",
-                "W0 = W1.copy()\n",
-                "H0 = H1.copy()\n",
-                "\n",
-                "\n",
-                "\n",
-                "def loss(P, A):\n",
-                "    DA = G @ P @ A\n",
-                "    v1 = KL(X, DA) \n",
-                "    v2 = trace_xtLx(L, A.T)\n",
-                "    return v1 + lambda_L/2 * v2\n",
-                "\n",
-                "maxit = 100\n",
-                "force_simplex = False\n",
-                "loss0 = [loss(W0, H0)]\n",
-                "\n",
-                "loss1 = [loss(W1, H1)]\n",
-                "loss2 = [loss(W2, H2)]\n",
-                "diff_loss2 = []\n",
-                "loss3 = [loss(W3, H3)]\n",
-                "diff_loss3 = []\n",
-                "\n",
-                "loss4 = [loss(W4, H4)]\n",
-                "diff_loss4 = []\n",
-                "loss5 = [loss(W5, H5)]\n",
-                "diff_loss5 = []\n",
-                "\n",
-                "# gammH2 = sigmaL\n",
-                "gammH2 = 1e-3\n",
-                "gammH2 = 0.005\n",
-                "gammH2 = 0.25\n",
-                "\n",
-                "gammH5 = 1e-3\n",
-                "gammH5 = 0.005\n",
-                "gammH5 = 0.4\n",
-                "\n",
-                "gammH3 = sigmaL\n",
-                "# gammH3 = 0.4\n",
-                "gammH3_vec = [gammH3]\n",
-                "d3 = []\n",
-                "\n",
-                "gammH4 = sigmaL\n",
-                "# gammH4 = 0.25\n",
-                "gammH4_vec = [gammH4]\n",
-                "d4 = []\n",
-                "\n",
-                "\n",
-                "\n",
-                "for i in range(maxit):\n",
-                "    H0 = multiplicative_step_h(X, G, W0, H0, force_simplex=force_simplex, lambda_L=lambda_L, L=L)\n",
-                "    W0 = multiplicative_step_w(X, G, W0, H0)\n",
-                "    loss0.append(loss(W0, H0))\n",
-                "    \n",
-                "    H1 = multiplicative_step_hq(X, G, W1, H1, force_simplex=force_simplex, lambda_L=lambda_L, L=L)\n",
-                "    W1 = multiplicative_step_w(X, G, W1, H1)\n",
-                "    loss1.append(loss(W1, H1))\n",
-                "\n",
-                "    \n",
-                "    H2 = multiplicative_step_hq(X, G, W2, H2, force_simplex=force_simplex, lambda_L=lambda_L, L=L, sigmaL=gammH2)\n",
-                "    diff_loss2.append(loss2[-1]-loss(W2, H2))\n",
-                "    W2 = multiplicative_step_w(X, G, W2, H2)\n",
-                "    loss2.append(loss(W2, H2))\n",
-                "\n",
-                "    H3_old = H3.copy()\n",
-                "    H3 = multiplicative_step_hq(X, G, W3, H3, force_simplex=force_simplex, lambda_L=lambda_L, L=L, sigmaL=gammH3)\n",
-                "    d3.append(diff_surrogate(H3_old, H3, L=L, sigmaL=gammH3))\n",
-                "    diff_loss3.append(d3)\n",
-                "    if d3[-1]>0:\n",
-                "        gammH3 = gammH3 / 1.05\n",
-                "    else:\n",
-                "        gammH3 = gammH3 * 1.5\n",
-                "    gammH3_vec.append(gammH3)\n",
-                "    W3 = multiplicative_step_w(X, G, W3, H3)\n",
-                "    loss3.append(loss(W3, H3))\n",
-                "    \n",
-                "    H4_old = H4.copy()\n",
-                "    H4 = multiplicative_step_h(X, G, W4, H4, force_simplex=force_simplex, lambda_L=lambda_L, L=L, sigmaL=gammH4)\n",
-                "    d4.append(diff_surrogate(H4_old, H4, L=L, sigmaL=gammH4, dgkl=True))\n",
-                "    diff_loss4.append(d4)\n",
-                "    if d4[-1]>0:\n",
-                "        gammH4 = gammH4 / 1.05\n",
-                "    else:\n",
-                "        gammH4 = gammH4 * 1.5\n",
-                "    gammH4_vec.append(gammH4)\n",
-                "    W4 = multiplicative_step_w(X, G, W4, H4)\n",
-                "    loss4.append(loss(W4, H4))\n",
-                "    \n",
-                "    H5 = multiplicative_step_hq(X, G, W5, H5, force_simplex=force_simplex, lambda_L=lambda_L, L=L, sigmaL=gammH5)\n",
-                "    diff_loss5.append(loss5[-1]-loss(W5, H5))\n",
-                "    W5 = multiplicative_step_w(X, G, W5, H5)\n",
-                "    loss5.append(loss(W5, H5))\n",
-                "    "
+                "laplacian = False\n",
+                "noise = True\n",
+                "simplex_H = True\n",
+                "\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "for i in range(10*maxit):\n",
-                "    H2 = multiplicative_step_hq(X, G, W2, H2, force_simplex=force_simplex, lambda_L=lambda_L, L=L, sigmaL=gammH5)\n",
-                "    W2 = multiplicative_step_w(X, G, W2, H2)\n",
-                "\n",
-                "l_infty = loss(W2, H2)"
+                "from convergence import run_experiment_set\n",
+                "seed = 50\n",
+                "max_iter = 1000\n",
+                "losses, final_losses, Ws, Hs, params, captions, gammas, l_infty, W, H, true_D, true_H, X, Xdot, times = run_experiment_set(laplacian, noise, simplex_H, seed=seed, max_iter=max_iter)\n",
+                "losses = np.array(losses) - l_infty.reshape(-1, 1)\n",
+                "shape_2d = params[0][0][\"shape_2d\"]\n",
+                "k = H.shape[0]\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "iterations = np.arange(maxit+1)+1\n",
-                "plt.figure(figsize=[15, 10])\n",
-                "plt.plot(iterations, np.array(loss0)-l_infty, \"ko-\", label=\"KL surrogate - theoretical step\")\n",
-                "plt.plot(iterations, np.array(loss5)-l_infty, \"ro-\", label=\"KL surrogate -  manual fixed step\")\n",
-                "plt.plot(iterations, np.array(loss4)-l_infty, \"go-\", label=\"KL surrogate - adaptive step size\")\n",
-                "plt.plot(iterations, np.array(loss1)-l_infty, \"kx-\", label=\"L2 surrogate - theoretical step\")\n",
-                "plt.plot(iterations, np.array(loss2)-l_infty, \"rx-\", label=\"L2 surrogate - manual fixed step\")\n",
-                "plt.plot(iterations, np.array(loss3)-l_infty, \"gx-\", label=\"L2 surrogate - adaptive step size\")\n",
-                "plt.yscale(\"log\")\n",
-                "plt.xscale(\"log\")\n",
-                "plt.legend()\n"
+                "for time, caption in zip(times, captions):\n",
+                "    print(f\"Algorithm: {naming_hash[caption]} took {time} seconds.\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plt.plot(gammH3_vec, \".-\", label=\"L2 surrogate\")\n",
-                "plt.plot(gammH4_vec, \".-\", label=\"DGKL surrogate\")\n",
+                "plt.figure(figsize=[10, 6])\n",
+                "# plt.figure(figsize=[15, 10])\n",
+                "\n",
+                "for loss, caption in zip(losses, captions):\n",
+                "    iterations = np.arange(len(loss))+1\n",
+                "    if len(iterations)>10:\n",
+                "        plt.plot(iterations, loss, \".-\", label=caption)\n",
+                "max_y = np.max(losses)\n",
+                "min_y = np.min(losses)\n",
+                "plt.ylim([min_y, max_y])\n",
+                "plt.xlim([1, losses.shape[1]])\n",
                 "plt.yscale(\"log\")\n",
-                "plt.title(\"Evolution of the step size\")\n",
-                "plt.legend()\n"
+                "plt.xscale(\"log\")\n",
+                "plt.xlabel(\"Iterations\")\n",
+                "plt.legend()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# def f(x, a, b, c):\n",
-                "#     v = x + b\n",
-                "#     return v - np.sqrt( v**2 + 4*a*c) +2*a \n",
-                "# p = 1\n",
-                "# x = np.arange(-2,2, 0.1)\n",
-                "# a = np.random.rand(p)\n",
-                "# a = 0.5\n",
-                "# b = np.random.rand(p)\n",
-                "# c = np.random.rand(p)\n",
-                "# plt.plot(x, f(x,a,b,c))\n",
-                "# plt.plot(x, np.zeros_like(x))"
+                "# for gamma, caption in zip(gammas, captions):\n",
+                "#     iterations = np.arange(len(gamma))+1\n",
+                "\n",
+                "#     plt.plot(iterations, gamma, \".\", label=caption)\n",
+                "# plt.yscale(\"log\")\n",
+                "# plt.legend()\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": []
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
+            "source": [
+                "Hmat = H.reshape(k, shape_2d[0], shape_2d[1])\n",
+                "Hmat_true = true_H.reshape(k, shape_2d[0], shape_2d[1])\n",
+                "scale = 4\n",
+                "cmap = plt.cm.viridis\n",
+                "plt.figure(figsize=(scale*k,2*scale))\n",
+                "for i in range(k):\n",
+                "    plt.subplot(2,k,i+1)\n",
+                "    plt.imshow(Hmat[i], cmap=cmap, vmin=0, vmax=1)\n",
+                "    plt.title(f\"Estimated H {i}\")\n",
+                "    plt.axis('off')\n",
+                "    plt.colorbar()\n",
+                "    plt.subplot(2,k,i+1+k)\n",
+                "    plt.imshow(Hmat_true[i], cmap=cmap, vmin=0, vmax=1)\n",
+                "    plt.title(f\"True H {i}\")\n",
+                "    plt.axis('off')\n",
+                "    plt.colorbar()\n",
+                "\n",
+                "plt.tight_layout()\n"
+            ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "\n",
-                "\n"
+                "plt.plot(true_D)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -440,15 +331,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.6"
+            "version": "3.12.2"
         },
         "vscode": {
             "interpreter": {
                 "hash": "a7ceffc662db6c9d514927743d8d35570797b920e33613212d4f424c0416cf91"
             }
         }
     },
```

### Comparing `espm-1.0.0/notebooks/generate_data.ipynb` & `espm-1.1.1/notebooks/generate_data.ipynb`

 * *Files identical despite different names*

### Comparing `espm-1.0.0/notebooks/simple-test-regularisation.ipynb` & `espm-1.1.1/notebooks/background_fit.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8113652263131732%*

 * *Differences: {"'cells'": "{0: {'source': ['# %matplotlib inline\\n', '%matplotlib qt\\n', 'import hyperspy.api "*

 * *            "as hs\\n', 'import numpy as np\\n', 'import lmfit as lm\\n', 'import "*

 * *            "matplotlib.pyplot as plt\\n', 'import espm.spectrum_fitting as sf\\n', 'from pathlib "*

 * *            "import Path\\n', 'from espm.estimators import SmoothNMF']}, 1: {'cell_type': "*

 * *            "'markdown', 'source': ['# Guide to this notebook\\n', '\\n', 'Every time the symbol "*

 * *            '⚠️ appears, a user input […]*

```diff
@@ -2,475 +2,441 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "%load_ext autoreload\n",
-                "%autoreload 2\n",
-                "%matplotlib inline"
+                "# %matplotlib inline\n",
+                "%matplotlib qt\n",
+                "import hyperspy.api as hs\n",
+                "import numpy as np\n",
+                "import lmfit as lm\n",
+                "import matplotlib.pyplot as plt\n",
+                "import espm.spectrum_fitting as sf\n",
+                "from pathlib import Path\n",
+                "from espm.estimators import SmoothNMF"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "import numpy as np\n",
-                "import matplotlib.pyplot as plt\n",
-                "from espm.datasets.base import generate_spim\n",
-                "from espm.estimators import SmoothNMF\n",
-                "from espm.measures import find_min_angle, find_min_MSE, ordered_mse, ordered_mae, ordered_r2, KLdiv\n"
+                "# Guide to this notebook\n",
+                "\n",
+                "Every time the symbol \u26a0\ufe0f appears, a user input is required in the cell below.\n",
+                "\n",
+                "If a cell made a few windows pop up, please kill the windows once you're done. Otherwise every new plot will be displayed in top of the other (which may slow your computer down). \n",
+                "\n",
+                "Overview of the different steps :\n",
+                "- I. Load the data either a spectrum (go to step III.) or a spectrum image\n",
+                "- II. Select an area of interest in your spectrum image.\n",
+                "- III. Creates an energy scale (x) from your data for the fitting procedure.\n",
+                "- IV. Selects the regions of the spectrum were there are no peaks for background fitting.\n",
+                "- V. Creates the required objects (partial x and y) for the background fitting procedure.\n",
+                "- VI. Fitting the background. If this is not satisfactory go back to IV."
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "C = 15\n",
-                "L = 200\n",
-                "P = 100**2\n",
-                "nx = 50\n",
-                "seed = 1\n",
+                "## I. Load spectrum & energy scale\n",
                 "\n",
-                "n_poisson = 2 # Average poisson number per pixel (this number will be splitted on the L dimension)\n"
+                "This cell will start a gui, that will let you select the dataset you want to analyse. In this notebook, only single spectra are treated, the data are thus automatically summed and cropped.\n",
+                "\n",
+                "\u26a0\ufe0f"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "def syntheticG(L=200, C=15, seed=None):\n",
-                "\n",
-                "    np.random.seed(seed=seed)\n",
-                "    n_el = 45\n",
-                "    n_gauss = np.random.randint(2, 5,[C])\n",
-                "    l = np.arange(0, 1, 1/L)\n",
-                "    mu_gauss = np.random.rand(n_el)\n",
-                "    sigma_gauss = 1/n_el + np.abs(np.random.randn(n_el))/n_el/5\n",
-                "\n",
-                "    G = np.zeros([L,C])\n",
-                "\n",
-                "    def gauss(x, mu, sigma):\n",
-                "        # return np.exp(-(x-mu)**2/(2*sigma**2)) / (sigma * np.sqrt(2*np.pi))\n",
-                "        return np.exp(-(x-mu)**2/(2*sigma**2))\n",
-                "\n",
-                "    for i, c in enumerate(n_gauss):\n",
-                "        inds = np.random.choice(n_el, size=[c] , replace=False)\n",
-                "        for ind in inds:\n",
-                "            w = 0.1+0.9*np.random.rand()\n",
-                "            G[:,i] += w * gauss(l, mu_gauss[ind], sigma_gauss[ind])\n",
-                "    return G\n",
-                "\n",
-                "def build_simple_images(nx = 40):\n",
-                "    \n",
-                "\n",
-                "    im1 = np.zeros(shape=[nx,nx])\n",
-                "    # 1st quarter\n",
-                "    im1[:nx//2,:nx//2] = 1\n",
-                "    # 2st quarter\n",
-                "    im1[nx//6:nx//3,-nx//3:-nx//6] = 0.5\n",
-                "    # 3rd quarter\n",
-                "    im1[-nx//3:,:nx//2] = np.expand_dims(np.arange(0,1, 3/nx), axis=1) * np.ones(shape=[1, nx//2])\n",
-                "    # im1[-nx//3:,:nx//2] = np.expand_dims(np.arange(3/nx,1+3/nx, 3/nx), axis=1) * np.ones(shape=[1, nx//2])\n",
-                "    # 4th quarter\n",
-                "    x,y = np.meshgrid(np.arange(nx), np.arange(nx))\n",
-                "    mask = (x-nx+nx//4)**2 + (y-nx+nx//4)**2<(nx//6)**2\n",
-                "    im1[mask] = 1\n",
-                "\n",
-                "    im0 = 1 - im1\n",
-                "\n",
-                "    Hdot = np.array([im0, im1])\n",
-                "\n",
-                "    return Hdot\n",
-                "\n",
-                "\n",
-                "def create_simple_problem(L, n_poisson,  C, nx=40, seed=None):\n",
-                "    np.random.seed(seed)\n",
-                "    G = syntheticG(L,C, seed=seed)\n",
-                "\n",
-                "    Hdot = build_simple_images(nx)\n",
-                "    K = len(Hdot)\n",
-                "    Hdotflat = Hdot.reshape(K, -1)\n",
-                "    Wdot = np.abs(np.random.laplace(size=[C, K]))\n",
-                "    mask = Wdot>np.mean(Wdot)\n",
-                "    Wdot[np.logical_not(mask)] = 0\n",
-                "    m = np.mean(Wdot[mask])\n",
-                "    Wdot = Wdot / m *K/np.sum(mask)\n",
-                "    Ddot = G @ Wdot\n",
-                "    Ydot = Ddot @ Hdotflat\n",
-                "\n",
-                "    Y = 1/n_poisson * np.random.poisson(n_poisson * Ydot)\n",
-                "    shape_2d = Hdot.shape[1:]\n",
-                "    return G, Wdot, Ddot, Hdot, Hdotflat, Ydot, Y, shape_2d, K\n",
-                "\n",
-                "def plot_results(Ddot, D, Hdotflat, Hflat):\n",
-                "    fontsize = 30\n",
-                "    scale = 15\n",
-                "    aspect_ratio = 1.4\n",
-                "    marker_list = [\"-o\",\"-s\",\"->\",\"-<\",\"-^\",\"-v\",\"-d\"]\n",
-                "    mark_space = 20\n",
-                "    # cmap = plt.cm.hot_r    \n",
-                "    cmap = plt.cm.gray_r\n",
-                "    vmax = 1\n",
-                "    vmin = 0\n",
-                "    K = len(H)\n",
-                "    L = len(D)\n",
-                "    \n",
-                "    angles, true_inds = find_min_angle(Ddot.T, D.T, unique=True, get_ind=True)\n",
-                "    mse = ordered_mse(Hdotflat, Hflat, true_inds)\n",
-                "    mae = ordered_mae(Hdotflat, Hflat, true_inds)\n",
-                "    r2 = ordered_r2(Hdotflat, Hflat, true_inds)\n",
-                "\n",
-                "\n",
-                "    fig, axes = plt.subplots(K, 3,figsize = (scale/K * 3 * aspect_ratio, scale))\n",
-                "    x = np.linspace(0,1, num = L)\n",
-                "    for i in range(K): \n",
-                "        axes[i, 0].plot(x,Ddot.T[i,:],'bo',label='truth',linewidth=4)\n",
-                "        axes[i, 0].plot(x,D[:,true_inds[i]],'r-',label='reconstructed',markersize=3.5)\n",
-                "        axes[i, 0].set_title(\"{:.2f} deg\".format(angles[i]),fontsize = fontsize-2)\n",
-                "        axes[i, 0].set_xlim(0,1)\n",
-                "        axes[i, 0].legend()\n",
-                "\n",
-                "        axes[i, 1].imshow((Hflat[true_inds[i],:]).reshape(shape_2d),vmin = vmin, vmax = vmax , cmap=cmap)\n",
-                "        axes[i, 1].set_title(\"Reconstruction - R2: {:.2f}\".format(r2[true_inds[i]]),fontsize = fontsize-2)\n",
-                "        # axes[i,1].set_ylim(0.0,1.0)\n",
-                "        axes[i, 1].tick_params(axis = \"both\",labelleft = False, labelbottom = False,left = False, bottom = False)\n",
+                "spectrum = hs.load().mean().isig[0.2:]\n",
                 "\n",
-                "        im = axes[i, 2].imshow(Hdotflat[i].reshape(shape_2d),vmin = vmin, vmax = vmax, cmap=cmap)\n",
-                "        axes[i,2].set_title(\"GT - Phase {}\".format(i),fontsize = fontsize)\n",
-                "        axes[i,2].tick_params(axis = \"both\",labelleft = False, labelbottom = False,left = False, bottom = False)\n",
-                "        \n",
+                "# spectrum.set_signal_type('EDS_espm')\n",
                 "\n",
-                "    rows = [f\"Phase {i}\" for i in range(K)]\n",
+                "offset = spectrum.axes_manager[0].offset\n",
+                "scale = spectrum.axes_manager[0].scale\n",
+                "size = spectrum.axes_manager[0].size\n",
                 "\n",
-                "    for ax, row in zip(axes[:,0], rows):\n",
-                "        ax.set_ylabel(row, rotation=90, fontsize=fontsize)\n",
-                "\n",
-                "\n",
-                "    fig.subplots_adjust(right=0.84)\n",
-                "    # put colorbar at desire position\n",
-                "    cbar_ax = fig.add_axes([0.85, 0.5, 0.01, 0.3])\n",
-                "    fig.colorbar(im,cax=cbar_ax)\n",
-                "\n",
-                "    # fig.tight_layout()\n",
-                "\n",
-                "    plt.show()\n",
-                "    print(\"angles : \", angles)\n",
-                "    print(\"mse : \", mse)\n",
-                "    print(\"mae : \", mae)\n",
-                "    print(\"r2 : \", r2)\n",
-                "\n",
-                "    \n",
-                "        "
+                "x = np.linspace(offset,size*scale+offset,num = size)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Create a synthetic problem"
+                "## Setting the relevant metadata\n",
+                "\n",
+                "This cell is important later during the fitting of the characteristic peaks. Check the documentation at : https://espm.readthedocs.io/en/latest/ for details about thos parameters\n",
+                "\n",
+                "\u26a0\ufe0f"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "G = syntheticG(L,C, seed)\n",
-                "l = np.arange(0, 1, 1/L)\n",
-                "plt.plot(l, G[:,:2])\n",
-                "plt.title(\"Spectral response of each elements\")\n"
+                "spectrum.set_analysis_parameters(beam_energy = 200,\n",
+                "                                 azimuth_angle = 0.0,\n",
+                "                                 elevation_angle = 22.0,\n",
+                "                                 tilt_stage = 0.0,\n",
+                "                                 elements = ['Sr', 'Ti', 'O'],\n",
+                "                                 thickness = 200e-7,\n",
+                "                                 density = 3.5,\n",
+                "                                 detector_type = \"SDD_efficiency.txt\",\n",
+                "                                 width_slope = 0.01,\n",
+                "                                 width_intercept = 0.065,\n",
+                "                                 xray_db = \"200keV_xrays.json\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "spectrum.metadata"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# II. Select areas for bckgd fitting\n",
                 "\n",
-                "Hdot = build_simple_images(nx=nx)\n",
-                "vmin, vmax = 0,1\n",
-                "cmap = plt.cm.gray_r\n",
-                "plt.figure(figsize=(10, 3))\n",
-                "for i, hdot in enumerate(Hdot):\n",
-                "    plt.subplot(1,3,i+1)\n",
-                "    plt.imshow(hdot, cmap=cmap, vmin=vmin, vmax=vmax)\n",
-                "    plt.axis(\"off\")\n",
-                "    plt.title(f\"Map {i+1}\")\n"
+                "\u26a0\ufe0f Input in the ``span_number`` the number of selection areas you wish to use. Once you execute the cell, a window will pop with a few green areas and a red spectrum. The green areas correspond to the regions were the background will be fitted. You can, drag, enlarge and reduce these green areas.\n",
+                "\n",
+                "Note : Click on one of the green area before the click and drag operation so that only one of the area is selected and so avoid to drag them all together."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "G, Wdot, Ddot, Hdot, Hdotflat, Ydot, Y, shape_2d, K = create_simple_problem(L=L, n_poisson=n_poisson,  C=C, nx=nx)\n",
-                "plt.plot(Ddot)\n",
+                "span_number = 4\n",
+                "\n",
+                "def selection_areas(number,spectrum,scale) :\n",
+                "    spectrum.plot()\n",
+                "    size = spectrum.axes_manager[0].size //(2*number)\n",
+                "    roi_list = []\n",
+                "    for i in range(number) :\n",
+                "        roi_list.append(hs.roi.SpanROI(offset+ size*scale + 2*i*size*scale, 2*size*scale + offset+ 2*i*size*scale))\n",
+                "        roi_list[-1].interactive(spectrum)\n",
+                "    return roi_list\n",
                 "\n",
-                "Wdot.shape, G.shape, L, C, nx"
+                "spans = selection_areas(span_number,spectrum,scale)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Solve the problem"
+                "Once you are satisfied with the selected areas, save their positions using the cell below"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "list_energies = [[roi.left,roi.right] for roi in spans]"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# III. Fitting the continuum\n",
                 "\n",
-                "mu = 0\n",
-                "lambda_L = 0\n",
-                "force_simplex = True\n",
-                "Gused = None\n",
-                "\n",
-                "params = {}\n",
-                "params[\"tol\"]=1e-6\n",
-                "params[\"max_iter\"] = 500\n",
-                "params[\"hspy_comp\"] = False\n",
-                "params[\"verbose\"] = 0\n",
-                "params[\"epsilon_reg\"] = 1\n",
-                "params[\"linesearch\"] = False\n",
-                "params[\"shape_2d\"] = shape_2d\n",
-                "params[\"n_components\"] = K\n",
-                "\n",
-                "estimator = SmoothNMF(mu=mu, lambda_L=lambda_L, G = Gused, force_simplex=force_simplex, **params)\n",
-                "D = estimator.fit_transform(Y)\n",
-                "Hflat = estimator.H_\n",
-                "H = Hflat.reshape([Hflat.shape[0], *shape_2d])\n",
-                "W = estimator.W_\n",
-                "plt.plot(estimator.losses_)"
+                "\u26a0\ufe0f Input the sample parameters below and execute the cell to fit"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "        \n",
-                "angles, true_inds = find_min_angle(Ddot.T, D.T, unique=True, get_ind=True)\n",
-                "mse = ordered_mse(Hdotflat, Hflat, true_inds)\n",
-                "KL = KLdiv(Y, D, Hflat)\n",
-                "r2 = ordered_r2(Hdotflat, Hflat, true_inds)\n",
+                "thickness = 2e-5\n",
+                "density = 3.5\n",
+                "take_off_angle = 35\n",
+                "elements_dict = {\"Fe\" : 0.0194, \"C\" : 0.8904, \"Pt\" : 0.0051, 'O' : 0.03797, 'Si' : 0.00850 , \"Cu\" : 0.03846}\n",
+                "detector = \"SDD_efficiency.txt\"\n",
+                "\n",
+                "#################################################################################################\n",
+                "# For a custom detector, uncomment below and replace \"SDD_efficiency.txt\" with the dictionnary. #\n",
+                "#################################################################################################\n",
+                "\n",
+                "# {\"detection\" : {\n",
+                "#     \"thickness\" : 450e-4,\n",
+                "#     \"elements_dict\" : {\n",
+                "#         \"Si\" : 1.0\n",
+                "#     }\n",
+                "# },\"layer\" : {\n",
+                "#     \"thickness\" : 10e-7,\n",
+                "#     \"elements_dict\" : {\n",
+                "#         \"Si\" : 0.33,\n",
+                "#         \"O\" : 0.66,\n",
+                "#         \"Al\" : 1.0\n",
+                "#     }\n",
+                "# }}\n",
+                "\n",
+                "part_x, part_y, sum_boola = sf.make_partial_xy(list_energies,spectrum,x)\n",
+                "\n",
+                "example = {\n",
+                "    \"E0\" : 200,\n",
+                "    \"b0\" : 1.0,\n",
+                "    \"b1\" : 1.0,\n",
+                "    \"params_dict\" : {\n",
+                "    \"Det\" : detector,\n",
+                "    'Abs' : {\n",
+                "        \"thickness\" : thickness,\n",
+                "        \"toa\" : take_off_angle,\n",
+                "        \"density\" : density}\n",
+                "    },\n",
+                "    \"elements_dict\" : elements_dict\n",
+                "}\n",
+                "\n",
+                "pars = sf.ndict_to_params(example)\n",
+                "\n",
+                "#################################################################################################\n",
+                "# You can uncomment the lines below if you want to add constraints to the absorption parameters #\n",
+                "#################################################################################################\n",
+                "\n",
+                "pars[\"params_dict__Abs__thickness\"].vary = False\n",
+                "# pars[\"params_dict__Abs__thickness\"].max = 5000e-7\n",
+                "# pars[\"params_dict__Det__layer__thickness\"].vary = False\n",
+                "pars[\"params_dict__Abs__toa\"].vary = False\n",
+                "pars[\"params_dict__Abs__density\"].vary = False\n",
+                "pars[\"E0\"].vary = False\n",
+                "\n",
+                "out = lm.minimize(sf.residual, pars, args=(part_x,), kws={'data': part_y})\n",
+                "print(lm.fit_report(out))"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Plotting the results\n",
                 "\n",
-                "print(\"angles: \", angles)\n",
-                "print(\"mse: \", mse)\n",
-                "print(\"KL divergence: \", KL)\n",
-                "print(\"R2: \", r2)"
+                "The red curves corresponds to the background model, the black one to the data, and the grey area correspond to the selected green areas"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "plot_results(Ddot, D, Hdotflat, Hflat)"
+                "y = spectrum.data\n",
+                "bkgd = sf.residual(out.params,x)\n",
+                "plt.plot(x,y,\"ko-\",markersize=1.5,label=\"exp\",markevery=10)\n",
+                "plt.fill_between(x,0,y,where=sum_boola,label=\"fit windows\",color=\"0.8\")\n",
+                "plt.xlabel(\"Energy (keV)\",fontsize=22)\n",
+                "plt.xticks(fontsize=20)\n",
+                "# plt.ylim(0,1)\n",
+                "plt.yticks(fontsize=20)\n",
+                "plt.ylabel(\"Intensity\",fontsize=22)\n",
+                "plt.plot(x,bkgd,\"r-\",linewidth=1,label=\"fit\")\n",
+                "plt.legend(fontsize=22)"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# VI. Quantify the chemical concentrations\n",
+                "\n",
+                "## Fitting parameters setup\n",
+                "\n",
+                "First remove the fitted background from the complete spectrum and remove the negative values."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# plt.figure(figsize=(10, 4))\n",
-                "# plt.subplot(1,2,1)\n",
-                "# plt.hist(Ydot.flatten()*n_poisson, 100);\n",
-                "# plt.subplot(1,2,1)\n",
-                "# plt.hist(Y.flatten()*n_poisson, 100, alpha=0.5);"
+                "spectrum.data = (spectrum.data - bkgd).clip(min = 0.0)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "In this cell we build the characteristic X-ray model to quantify the spectrum.\n",
+                "\n",
+                "Using the `reference_elt` keyword argument you can decouple characteristic X-ray lines of single elements to get a better fit. It can be necessary when the absorption is incorrectly calculated or when the cross-sections are not well calculated (e.g. for heavy elements).\n",
+                "\n",
+                "The `reference_elt` argument is a dictionary with `{ 'atomic number of the chosen element (int) : energy cutoff (float), .... }`, this way, the intensity of the lines above and below the cutoff are decoupled.\n",
+                "\n",
+                "\u26a0\ufe0f"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "def one_experiment(mu, lambda_L, force_simplex, Gused, params, Y):\n",
-                "    estimator = SmoothNMF(mu=mu, lambda_L=lambda_L, G = Gused, force_simplex=force_simplex, **params)\n",
-                "    D = estimator.fit_transform(Y)\n",
-                "    Hflat = estimator.H_\n",
-                "    H = Hflat.reshape([Hflat.shape[0], *shape_2d])\n",
-                "    W = estimator.W_\n",
-                "    angles, true_inds = find_min_angle(Ddot.T, D.T, unique=True, get_ind=True)\n",
-                "    mse = ordered_mse(Hdotflat, Hflat, true_inds)\n",
-                "    KL = KLdiv(Y, D, Hflat, average=True)\n",
-                "    r2 = ordered_r2(Hdotflat, Hflat, true_inds)\n",
+                "spectrum.build_G(problem_type='no_brstlg',reference_elt={'22' : 3.0})"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "In this cell we set up the parameters of the fitting algorithm.\n",
                 "\n",
-                "    print(\"angles: \", angles)\n",
-                "    print(\"mse: \", mse)\n",
-                "    print(\"KL divergence: \", KL)\n",
-                "    print(\"R2: \", r2)\n",
-                "    return angles, mse, KL, r2"
+                "For most fitting, you don't need to change those parameters."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "\n",
-                "lambda_L = 1\n",
-                "force_simplex = True\n",
-                "Gused = None\n",
-                "\n",
-                "mus = np.array([0, 0.5, 1, 2, 3, 5, 10])\n",
-                "\n",
-                "metrics_mus = []\n",
-                "for i, mu in enumerate(mus):\n",
-                "    print(f\"Experiment -- {i+1}/{len(mus)} --\")\n",
-                "    print(f\"  lambda={lambda_L}, mu={mu}, Gused: {Gused is not None}, simplex: {force_simplex}\")\n",
-                "    metrics_mus.append(one_experiment(mu, lambda_L, force_simplex, Gused, params, Y))\n"
+                "est = SmoothNMF(G=spectrum.model,n_components= 1,max_iter=2000,tol = 1e-8,hspy_comp = False)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Fitting the spectrum"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "est.fit_transform(X = spectrum.data[:,np.newaxis] ,H=np.array([1.0])[:,np.newaxis])"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Printing the concentrations\n",
                 "\n",
-                "r2_mus = np.mean(np.array([e[3] for e in metrics_mus]), axis=1)\n",
-                "angles_mus = np.mean(np.array([e[0] for e in metrics_mus]), axis=1)\n",
-                "\n",
-                "KL_mus = np.array([e[2] for e in metrics_mus])\n",
-                "plt.figure(figsize=(10, 4))\n",
-                "plt.subplot(121)\n",
-                "plt.plot(mus+1, KL_mus, \"-x\")\n",
-                "plt.xscale(\"log\")\n",
-                "plt.subplot(122)\n",
-                "plt.scatter(r2_mus, angles_mus)\n",
-                "plt.plot(r2_mus, angles_mus, linestyle = 'dashed')\n",
-                "for lam, r2, angle in zip(mus, r2_mus, angles_mus):\n",
-                "    plt.annotate(str(lam), xy=(r2+0.0003, angle+0.1), size=10, va='center',ha='left')\n",
-                "plt.xlim([0.885, 0.905])\n",
-                "plt.ylim([4, 6.5])\n",
-                "plt.title(\"Avg. R2 and angle error for different mu\")\n",
-                "plt.xlabel(r'$R^2(H, \\tilde{H})$ [-]')\n",
-                "plt.ylabel(r'$\\theta(W, \\tilde{W})$ [deg]')\n",
-                "plt.grid()\n",
-                "plt.show()"
+                "In relative atomic concentrations"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "force_simplex = True\n",
-                "Gused = None\n",
-                "mu = 0\n",
-                "\n",
-                "\n",
-                "# lambdas = np.array([0, 10, 20, 50, 100, 200, 500, 1000])\n",
-                "lambdas = np.array([0, 0.1, 0.2, 0.5, 1, 2, 5,])\n",
-                "metrics_lambda = []\n",
-                "for i, lambda_L in enumerate(lambdas):\n",
-                "    print(f\"Experiment -- {i+1}/{len(lambdas)} --\")\n",
-                "    print(f\"  lambda={lambda_L}, mu={mu}, Gused={Gused is not None}, simplex={force_simplex}\")\n",
-                "    metrics_lambda.append(one_experiment(mu, lambda_L, force_simplex, Gused, params, Y))\n"
+                "spectrum.print_concentration_report()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Only printing selected elements. For example Cu is almost always present but not relevant to the quantification. It can be nice to remove it by selecting only the relevant elements."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "\n",
-                "r2_lambdas = np.mean(np.array([e[3] for e in metrics_lambda]), axis=1)\n",
-                "angles_lambdas = np.mean(np.array([e[0] for e in metrics_lambda]), axis=1)\n",
-                "\n",
-                "KL_lambdas = np.array([e[2] for e in metrics_lambda])\n",
-                "plt.figure(figsize=(10, 4))\n",
-                "plt.subplot(121)\n",
-                "plt.plot(lambdas+1, KL_lambdas, \"-x\")\n",
-                "plt.xscale(\"log\")\n",
-                "plt.subplot(122)\n",
-                "# plt.scatter(r2_lambdas, angles_lambdas)\n",
-                "\n",
-                "\n",
-                "# plt.annotate(str(1), xy=(angles-0.01, angles_lambdas-0.5), size=20, va='center',ha='left')\n",
-                "plt.scatter(r2_lambdas, angles_lambdas)\n",
-                "plt.plot(r2_lambdas, angles_lambdas, linestyle = 'dashed')\n",
-                "for lam, r2, angle in zip(lambdas, r2_lambdas, angles_lambdas):\n",
-                "    # plt.annotate(str(lam), xy=(r2+0.0003, angle+0.1), size=10, va='center',ha='left')\n",
-                "    plt.annotate(str(lam), xy=(r2+0.000, angle+0.), size=10, va='center',ha='left')\n",
-                "# plt.xlim([0.885, 0.905])\n",
-                "# plt.ylim([4, 6.5])\n",
-                "plt.title(\"Avg. R2 and angle error for different lambda\")\n",
-                "plt.xlabel(r'$R^2(H, \\tilde{H})$ [-]')\n",
-                "plt.ylabel(r'$\\theta(W, \\tilde{W})$ [deg]')\n",
-                "plt.grid()\n",
-                "plt.show()\n",
-                "\n",
-                "\n"
+                "spectrum.print_concentration_report(selected_elts=['Sr'])"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
-            "source": []
+            "source": [
+                "# IX. Plot the results\n",
+                "\n",
+                "\u26a0\ufe0f The popping window will display the bkgd substracted experimental spectrum, the fitted characteristic Xrays model in black and red. Every element composing the model will be displayed with an offset : ``components_offset``. You can change its value below. \n",
+                "\n",
+                "If you want to display the names of the lines of an element that was used for quantification execute the next cells below before kill the window."
+            ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "KL_lambdas"
+                "components_offset = -0.1"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": []
+            "source": [
+                "linestyles = [\":\",\"--\",\"-.\"]\n",
+                "\n",
+                "plt.plot(x,spectrum.data,\"ko-\",label=\"exp\",markevery = 10)\n",
+                "plt.plot(x,spectrum.G@est.W_,\"r\",linewidth = 3,label=\"theo\")\n",
+                "plt.xticks(fontsize = 16)\n",
+                "plt.yticks(fontsize = 16)\n",
+                "plt.xlabel(\"energy (keV)\",fontsize = 18)\n",
+                "plt.ylabel(\"Intensity\", fontsize = 18)\n",
+                "\n",
+                "for i in range(spectrum.G.shape[1]) :\n",
+                "    ls_string = linestyles[i%len(linestyles)] + \"C{}\".format(i%9)\n",
+                "    plt.plot(x,spectrum.G[:,i]*est.W_[i]+components_offset,ls_string,label=str(spectrum.metadata.EDS_model.elements[i]),linewidth=3)\n",
+                "\n",
+                "\n",
+                "plt.legend(fontsize=18)\n",
+                "plt.tight_layout()"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3.9.13 ('SNMF_EDXS-FwWDtlwS')",
+            "display_name": "Python 3.10.6 ('espm')",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.11.8"
         },
         "vscode": {
             "interpreter": {
-                "hash": "1a1b43244e11bc51a1d0b046d5a6cc91cb73bf5187e443fb7c1433042d0ea61d"
+                "hash": "8d2c37261bd18724b44288178b5d93ac658e7a29aba4ea6c1b1b0710c1696ef2"
             }
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `espm-1.0.0/setup.py` & `espm-1.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='espm',
-    version='1.0.0',
+    version='1.1.1',
     description='Electron SPectro-Microscopy Python Library',
     url='https://github.com/adriente/espm',
     author='Adrien Teurtie, Nathanael Perraudin',
-    author_email='nathanael.perraudin@sdsc.ethz.ch',
+    author_email='adrien.teurtrie@univ-lille.fr, nathanael.perraudin@sdsc.ethz.ch',
     license='MIT',
     packages=setuptools.find_packages(),
     zip_safe=False,
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={'hyperspy.extensions': 'espm = espm'},
     include_package_data=True,
@@ -28,18 +28,19 @@
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
         'Intended Audience :: End Users/Desktop',
         'Intended Audience :: Developers', 'Natural Language :: English',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: POSIX :: Linux', 'Programming Language :: C',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.8',
         'Topic :: Scientific/Engineering :: Mathematics',
         'Topic :: Scientific/Engineering'
     ],
     install_requires=[
-        'hyperspy', 'tqdm', 'lmfit', 'scikit-learn'
+        #'hyperspy<2.0.0', 'tqdm', 'lmfit', 'scikit-learn', 'traits @ git+https://github.com/enthought/traits.git'
+        'hyperspy>=2.0.0', 'exspy', 'tqdm', 'lmfit', 'scikit-learn', 'traits<6.0.0'
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.8',
 )
```


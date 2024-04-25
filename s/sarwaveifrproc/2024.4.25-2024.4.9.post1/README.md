# Comparing `tmp/sarwaveifrproc-2024.4.25.tar.gz` & `tmp/sarwaveifrproc-2024.4.9.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarwaveifrproc-2024.4.25.tar", last modified: Thu Apr 25 15:01:20 2024, max compression
+gzip compressed data, was "sarwaveifrproc-2024.4.9.post1.tar", last modified: Tue Apr  9 13:39:19 2024, max compression
```

## Comparing `sarwaveifrproc-2024.4.25.tar` & `sarwaveifrproc-2024.4.9.post1.tar`

### file list

```diff
@@ -1,68 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:01:20.350305 sarwaveifrproc-2024.4.25/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:01:20.334305 sarwaveifrproc-2024.4.25/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:01:20.334305 sarwaveifrproc-2024.4.25/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-25 15:01:20.346305 sarwaveifrproc-2024.4.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:01:20.338305 sarwaveifrproc-2024.4.25/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:01:20.334305 sarwaveifrproc-2024.4.25/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:01:20.338305 sarwaveifrproc-2024.4.25/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/_static/css/sarwaveifrproc.css
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/atbd.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/bibliography.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     5016 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:01:20.342305 sarwaveifrproc-2024.4.25/docs/figures/
--rw-r--r--   0 runner    (1001) docker     (127)    93988 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/figures/ATBD_coarse_idea.png
--rw-r--r--   0 runner    (1001) docker     (127)   117856 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/figures/attrs_intra.png
--rw-r--r--   0 runner    (1001) docker     (127)    69466 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/figures/coordinates.png
--rw-r--r--   0 runner    (1001) docker     (127)    68489 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/figures/coordinates_intra.png
--rw-r--r--   0 runner    (1001) docker     (127)   206274 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/figures/cover.png
--rw-r--r--   0 runner    (1001) docker     (127)   254070 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/figures/level2_variables_grids.png
--rw-r--r--   0 runner    (1001) docker     (127)   362165 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/figures/sar_cross_spectrum.png
--rw-r--r--   0 runner    (1001) docker     (127)   105751 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/figures/variables_inter.png
--rw-r--r--   0 runner    (1001) docker     (127)   101424 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/figures/variables_intra.png
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/product_description.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/refs.bib
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:01:20.342305 sarwaveifrproc-2024.4.25/sarwaveifrproc/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/sarwaveifrproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/sarwaveifrproc/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/sarwaveifrproc/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14564 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/sarwaveifrproc/l2_wave.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/sarwaveifrproc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:01:20.346305 sarwaveifrproc-2024.4.25/sarwaveifrproc/reference_data/
--rw-r--r--   0 runner    (1001) docker     (127)   372928 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/sarwaveifrproc/reference_data/s1a-iw2-slc-dv-20231128t035702-20231128t035727-051412-063451-e01.nc
--rw-r--r--   0 runner    (1001) docker     (127)   143267 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/sarwaveifrproc/reference_data/s1a-iw2-slc-vh-20231128t035702-20231128t035727-051412-063451-002_L1B_xspec_IFR_3.7.6nospectra.nc
--rw-r--r--   0 runner    (1001) docker     (127)   143267 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/sarwaveifrproc/reference_data/s1a-iw2-slc-vv-20231128t035702-20231128t035727-051412-063451-005_L1B_xspec_IFR_3.7.6nospectra.nc
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/sarwaveifrproc/sarwaveifrproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/sarwaveifrproc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:01:20.346305 sarwaveifrproc-2024.4.25/sarwaveifrproc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-25 15:01:20.000000 sarwaveifrproc-2024.4.25/sarwaveifrproc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-25 15:01:20.000000 sarwaveifrproc-2024.4.25/sarwaveifrproc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:01:20.000000 sarwaveifrproc-2024.4.25/sarwaveifrproc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-25 15:01:20.000000 sarwaveifrproc-2024.4.25/sarwaveifrproc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-25 15:01:20.000000 sarwaveifrproc-2024.4.25/sarwaveifrproc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 15:01:20.000000 sarwaveifrproc-2024.4.25/sarwaveifrproc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:01:20.350305 sarwaveifrproc-2024.4.25/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:01:20.346305 sarwaveifrproc-2024.4.25/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/tests/test_output_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/tests/test_predict.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-25 15:01:05.000000 sarwaveifrproc-2024.4.25/tests/test_sarwaveifrproc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:39:19.319471 sarwaveifrproc-2024.4.9.post1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:39:19.311471 sarwaveifrproc-2024.4.9.post1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:39:19.311471 sarwaveifrproc-2024.4.9.post1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-09 13:39:19.319471 sarwaveifrproc-2024.4.9.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:39:19.315471 sarwaveifrproc-2024.4.9.post1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4881 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:39:19.315471 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14564 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/l2_wave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:39:19.319471 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/reference_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   372928 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/reference_data/s1a-iw2-slc-dv-20231128t035702-20231128t035727-051412-063451-e01.nc
+-rw-r--r--   0 runner    (1001) docker     (127)   143267 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/reference_data/s1a-iw2-slc-vh-20231128t035702-20231128t035727-051412-063451-002_L1B_xspec_IFR_3.7.6nospectra.nc
+-rw-r--r--   0 runner    (1001) docker     (127)   143267 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/reference_data/s1a-iw2-slc-vv-20231128t035702-20231128t035727-051412-063451-005_L1B_xspec_IFR_3.7.6nospectra.nc
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/sarwaveifrproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:39:19.319471 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-09 13:39:19.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-09 13:39:19.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:39:19.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-09 13:39:19.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-09 13:39:19.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-09 13:39:19.000000 sarwaveifrproc-2024.4.9.post1/sarwaveifrproc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:39:19.319471 sarwaveifrproc-2024.4.9.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:39:19.319471 sarwaveifrproc-2024.4.9.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/tests/test_predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-09 13:39:09.000000 sarwaveifrproc-2024.4.9.post1/tests/test_sarwaveifrproc.py
```

### Comparing `sarwaveifrproc-2024.4.25/.github/workflows/publish.yml` & `sarwaveifrproc-2024.4.9.post1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.25/.gitignore` & `sarwaveifrproc-2024.4.9.post1/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -123,10 +123,7 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
-
-.idea
-localconfig.yaml
```

### Comparing `sarwaveifrproc-2024.4.25/CONTRIBUTING.rst` & `sarwaveifrproc-2024.4.9.post1/CONTRIBUTING.rst`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Types of Contributions
 ----------------------
 
 Report Bugs
 ~~~~~~~~~~~
 
-Report bugs at https://github.com/umr-lops/sarwaveifrproc/issues.
+Report bugs at https://github.com/agrouaze/sarwaveifrproc/issues.
 
 If you are reporting a bug, please include:
 
 * Your operating system name and version.
 * Any details about your local setup that might be helpful in troubleshooting.
 * Detailed steps to reproduce the bug.
 
@@ -41,15 +41,15 @@
 sarwaveifrproc could always use more documentation, whether as part of the
 official sarwaveifrproc docs, in docstrings, or even on the web in blog posts,
 articles, and such.
 
 Submit Feedback
 ~~~~~~~~~~~~~~~
 
-The best way to send feedback is to file an issue at https://github.com/umr-lops/sarwaveifrproc/issues.
+The best way to send feedback is to file an issue at https://github.com/agrouaze/sarwaveifrproc/issues.
 
 If you are proposing a feature:
 
 * Explain in detail how it would work.
 * Keep the scope as narrow as possible, to make it easier to implement.
 * Remember that this is a volunteer-driven project, and that contributions
   are welcome :)
@@ -99,15 +99,15 @@
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
 3. The pull request should work for Python 3.5, 3.6, 3.7 and 3.8, and for PyPy. Check
-   https://travis-ci.com/umr-lops/sarwaveifrproc/pull_requests
+   https://travis-ci.com/agrouaze/sarwaveifrproc/pull_requests
    and make sure that the tests pass for all supported Python versions.
 
 Tips
 ----
 
 To run a subset of tests::
```

### Comparing `sarwaveifrproc-2024.4.25/LICENSE` & `sarwaveifrproc-2024.4.9.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.25/Makefile` & `sarwaveifrproc-2024.4.9.post1/Makefile`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.25/PKG-INFO` & `sarwaveifrproc-2024.4.9.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarwaveifrproc
-Version: 2024.4.25
+Version: 2024.4.9.post1
 Summary: Python library to generate Level-2 WAVE Product starting from Ifremer Level-1B or Level-1C SAR files
 Author: Robin Marquart, Antoine Grouazel
 License: MIT
 Keywords: SAR,wave,reseach,sea-state
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `sarwaveifrproc-2024.4.25/docs/Makefile` & `sarwaveifrproc-2024.4.9.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.25/docs/conf.py` & `sarwaveifrproc-2024.4.9.post1/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,17 +27,15 @@
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode',
-'sphinxcontrib.bibtex'
-]
+extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
@@ -62,15 +60,15 @@
 release = sarwaveifrproc.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = 'en'
+language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The name of the Pygments (syntax highlighting) style to use.
@@ -93,15 +91,15 @@
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
-# html_style = 'css/sarwaveifrproc.css'
+
 
 # -- Options for HTMLHelp output ---------------------------------------
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = 'sarwaveifrprocdoc'
 
 
@@ -155,11 +153,10 @@
     (master_doc, 'sarwaveifrproc',
      'sarwaveifrproc Documentation',
      author,
      'sarwaveifrproc',
      'One line description of project.',
      'Miscellaneous'),
 ]
-bibtex_bibfiles = ["./refs.bib"]
-bibtex_reference_style = 'author_year'
+
```

### Comparing `sarwaveifrproc-2024.4.25/docs/installation.rst` & `sarwaveifrproc-2024.4.9.post1/docs/installation.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 .. highlight:: shell
 
-############
+============
 Installation
-############
+============
 
 
 Stable release
 --------------
 
-To install **sarwaveifrproc**, run this command in your terminal:
+To install sarwaveifrproc, run this command in your terminal:
 
 .. code-block:: console
 
     $ pip install sarwaveifrproc
 
-.. code-block:: console
-
-    $ micromamba install -c conda-forge sarwaveifrproc
-
 This is the preferred method to install sarwaveifrproc, as it will always install the most recent stable release.
 
 If you don't have `pip`_ installed, this `Python installation guide`_ can guide
 you through the process.
 
 .. _pip: https://pip.pypa.io
 .. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
@@ -32,29 +28,24 @@
 
 The sources for sarwaveifrproc can be downloaded from the `Github repo`_.
 
 You can either clone the public repository:
 
 .. code-block:: console
 
-    $ git clone git://github.com/umr-lops/sarwaveifrproc
+    $ git clone git://github.com/agrouaze/sarwaveifrproc
 
 Or download the `tarball`_:
 
 .. code-block:: console
 
-    $ curl -OJL https://github.com/umr-lops/sarwaveifrproc/tarball/master
+    $ curl -OJL https://github.com/agrouaze/sarwaveifrproc/tarball/master
 
 Once you have a copy of the source, you can install it with:
 
 .. code-block:: console
 
     $ python setup.py install
 
 
-.. _Github repo: https://github.com/umr-lops/sarwaveifrproc
-.. _tarball: https://github.com/umr-lops/sarwaveifrproc/tarball/master
-
-
-.. raw:: latex
-
-    \newpage
+.. _Github repo: https://github.com/agrouaze/sarwaveifrproc
+.. _tarball: https://github.com/agrouaze/sarwaveifrproc/tarball/master
```

### Comparing `sarwaveifrproc-2024.4.25/docs/make.bat` & `sarwaveifrproc-2024.4.9.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.25/pyproject.toml` & `sarwaveifrproc-2024.4.9.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.25/sarwaveifrproc/l2_wave.py` & `sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/l2_wave.py`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.25/sarwaveifrproc/reference_data/s1a-iw2-slc-dv-20231128t035702-20231128t035727-051412-063451-e01.nc` & `sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/reference_data/s1a-iw2-slc-dv-20231128t035702-20231128t035727-051412-063451-e01.nc`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.25/sarwaveifrproc/reference_data/s1a-iw2-slc-vh-20231128t035702-20231128t035727-051412-063451-002_L1B_xspec_IFR_3.7.6nospectra.nc` & `sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/reference_data/s1a-iw2-slc-vh-20231128t035702-20231128t035727-051412-063451-002_L1B_xspec_IFR_3.7.6nospectra.nc`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.25/sarwaveifrproc/reference_data/s1a-iw2-slc-vv-20231128t035702-20231128t035727-051412-063451-005_L1B_xspec_IFR_3.7.6nospectra.nc` & `sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/reference_data/s1a-iw2-slc-vv-20231128t035702-20231128t035727-051412-063451-005_L1B_xspec_IFR_3.7.6nospectra.nc`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.25/sarwaveifrproc/utils.py` & `sarwaveifrproc-2024.4.9.post1/sarwaveifrproc/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import tensorflow as tf
 import datatree as dtt
 import numpy as np
 import glob
 import logging
 import yaml 
 import pickle
-import re
 import os
 from datetime import datetime
 from sarwaveifrproc.l2_wave import generate_l2_wave_product
 
 def get_safe_date(safe):
     """
     Extracts and returns the date and time from a given SAFE directory name.
@@ -46,23 +45,15 @@
     
     if all((pattern in safe) for pattern in ['XSP_', '1SDV', '.SAFE']):
         
         date = get_safe_date(safe)
 
         final_safe = final_safe.replace('XSP_', 'WAV_')
         final_safe = final_safe.replace('1SDV', '2SDV')
-        regexA = re.compile("A[0-9]{2}.SAFE")
-        regexB = re.compile("B[0-9]{2}.SAFE")
-        if  re.search(regexA, final_safe.split('_')[-1]) or re.search(regexB, final_safe.split('_')[-1]):
-            print('match regexp')
-            final_safe = final_safe.replace(final_safe.split('_')[-1], f'{tail.upper()}.SAFE')
-        else:
-            print('no slug existing-> just add the product ID')
-            final_safe = final_safe.replace('.SAFE', f'_{tail.upper()}.SAFE')
-
+        final_safe = final_safe.replace('.SAFE', f'_{tail.upper()}.SAFE')
         
         output_safe = os.path.join(root_savepath, date.strftime('%Y'), date.strftime('%j'), final_safe)
 
         return output_safe
     
     else:
         raise ValueError(f"The input SAFE does not meet the filename requirements.")
@@ -77,26 +68,16 @@
         tail (str, optional): The tail string to be appended to the filename corresponding to the processing options. Defaults to 'e00'.
         
     Returns:
         str: File path for saving the processed file.
     """
     filename = l1x_path.split(os.sep)[-1]
     filename_exploded = filename.split('-')
-    regex_file_number = re.compile("[0-9]{2}[0-6]")
-    if filename[0:2]=='l1':
-        final_filename = '-'.join([*filename_exploded[:4], 'dv', *filename_exploded[5:-1], f'{tail.lower()}.nc'])
-        if re.search(regex_file_number,final_filename.split('-')[9]):
-            final_filename = final_filename.replace(final_filename.split('-')[9]+'-','') #remove the -004- giving the number of the file
-    else:
-        final_filename = '-'.join([*filename_exploded[:3], 'dv', *filename_exploded[4:-1], f'{tail.lower()}.nc'])
-        if re.search(regex_file_number,final_filename.split('-')[8]):
-            final_filename = final_filename.replace(final_filename.split('-')[8]+'-','') #remove the -004- giving the number of the file
-    final_filename = final_filename.replace('l1b','l2')
-    final_filename = final_filename.replace('l1c','l2')
-    final_filename = final_filename.replace('xsp','wav')
+    final_filename = '-'.join([*filename_exploded[:3], 'dv', *filename_exploded[4:-1], f'{tail.lower()}.nc'])
+    
     savepath = os.path.join(output_safe, final_filename)
     return savepath
 
 def load_config():
     """
 
     Returns:
@@ -116,32 +97,32 @@
 
 
 def load_models(paths, predicted_variables):
     """
     Loads models, scalers, and bins necessary for prediction.
 
     Parameters:
-        paths (dict): Dictionary containing paths to model files, scaler files, and bin files.
-            Keys:
-                - 'model_intraburst': Path to the intraburst model file.
-                - 'model_interburst': Path to the interburst model file.
-                - 'scaler_intraburst': Path to the intraburst scaler file.
-                - 'scaler_interburst': Path to the interburst scaler file.
-                - 'bins_intraburst': Path to the intraburst bins directory.
-                - 'bins_interburst': Path to the interburst bins directory.
-        predicted_variables (list): List of variable names to be predicted.
-    Returns:
-        tuple: Tuple containing the following items:
-            - model_intraburst (tf.keras.Model): Intraburst model loaded from the provided path.
-            - model_interburst (tf.keras.Model): Interburst model loaded from the provided path.
-            - scaler_intraburst (RobustScaler): Intraburst scaler loaded from the provided path.
-            - scaler_interburst (RobustScaler): Interburst scaler loaded from the provided path.
-            - bins_intraburst (dict): Dictionary containing intraburst bins for each predicted variable.
-            - bins_interburst (dict): Dictionary containing interburst bins for each predicted variable.
-
+    paths (dict): Dictionary containing paths to model files, scaler files, and bin files.
+        Keys:
+            - 'model_intraburst': Path to the intraburst model file.
+            - 'model_interburst': Path to the interburst model file.
+            - 'scaler_intraburst': Path to the intraburst scaler file.
+            - 'scaler_interburst': Path to the interburst scaler file.
+            - 'bins_intraburst': Path to the intraburst bins directory.
+            - 'bins_interburst': Path to the interburst bins directory.
+    predicted_variables (list): List of variable names to be predicted.
+
+Returns:
+    tuple: Tuple containing the following items:
+        - model_intraburst (tf.keras.Model): Intraburst model loaded from the provided path.
+        - model_interburst (tf.keras.Model): Interburst model loaded from the provided path.
+        - scaler_intraburst (RobustScaler): Intraburst scaler loaded from the provided path.
+        - scaler_interburst (RobustScaler): Interburst scaler loaded from the provided path.
+        - bins_intraburst (dict): Dictionary containing intraburst bins for each predicted variable.
+        - bins_interburst (dict): Dictionary containing interburst bins for each predicted variable.
     """    
     # Unpack paths
     path_model_intraburst, path_model_interburst, path_scaler_intraburst, path_scaler_interburst, path_bins_intraburst, path_bins_interburst = paths.values()
     
     # Load models and scalers using paths provided
     model_intraburst = tf.keras.models.load_model(path_model_intraburst, compile=False)
     scaler_intraburst_array = np.load(path_scaler_intraburst)
```

### Comparing `sarwaveifrproc-2024.4.25/sarwaveifrproc.egg-info/PKG-INFO` & `sarwaveifrproc-2024.4.9.post1/sarwaveifrproc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarwaveifrproc
-Version: 2024.4.25
+Version: 2024.4.9.post1
 Summary: Python library to generate Level-2 WAVE Product starting from Ifremer Level-1B or Level-1C SAR files
 Author: Robin Marquart, Antoine Grouazel
 License: MIT
 Keywords: SAR,wave,reseach,sea-state
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `sarwaveifrproc-2024.4.25/sarwaveifrproc.egg-info/SOURCES.txt` & `sarwaveifrproc-2024.4.9.post1/sarwaveifrproc.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -5,38 +5,23 @@
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
 pyproject.toml
 .github/workflows/publish.yml
 docs/Makefile
-docs/atbd.rst
 docs/authors.rst
-docs/bibliography.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
-docs/modules.rst
-docs/product_description.rst
 docs/readme.rst
-docs/refs.bib
 docs/usage.rst
-docs/_static/css/sarwaveifrproc.css
-docs/figures/ATBD_coarse_idea.png
-docs/figures/attrs_intra.png
-docs/figures/coordinates.png
-docs/figures/coordinates_intra.png
-docs/figures/cover.png
-docs/figures/level2_variables_grids.png
-docs/figures/sar_cross_spectrum.png
-docs/figures/variables_inter.png
-docs/figures/variables_intra.png
 sarwaveifrproc/__init__.py
 sarwaveifrproc/cli.py
 sarwaveifrproc/config.yaml
 sarwaveifrproc/l2_wave.py
 sarwaveifrproc/main.py
 sarwaveifrproc/sarwaveifrproc.py
 sarwaveifrproc/utils.py
@@ -46,10 +31,9 @@
 sarwaveifrproc.egg-info/entry_points.txt
 sarwaveifrproc.egg-info/requires.txt
 sarwaveifrproc.egg-info/top_level.txt
 sarwaveifrproc/reference_data/s1a-iw2-slc-dv-20231128t035702-20231128t035727-051412-063451-e01.nc
 sarwaveifrproc/reference_data/s1a-iw2-slc-vh-20231128t035702-20231128t035727-051412-063451-002_L1B_xspec_IFR_3.7.6nospectra.nc
 sarwaveifrproc/reference_data/s1a-iw2-slc-vv-20231128t035702-20231128t035727-051412-063451-005_L1B_xspec_IFR_3.7.6nospectra.nc
 tests/__init__.py
-tests/test_output_names.py
 tests/test_predict.py
 tests/test_sarwaveifrproc.py
```

### Comparing `sarwaveifrproc-2024.4.25/tests/test_predict.py` & `sarwaveifrproc-2024.4.9.post1/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `sarwaveifrproc-2024.4.25/tests/test_sarwaveifrproc.py` & `sarwaveifrproc-2024.4.9.post1/tests/test_sarwaveifrproc.py`

 * *Files identical despite different names*


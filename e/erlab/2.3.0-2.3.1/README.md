# Comparing `tmp/erlab-2.3.0.tar.gz` & `tmp/erlab-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlab-2.3.0.tar", last modified: Mon Apr 22 14:23:27 2024, max compression
+gzip compressed data, was "erlab-2.3.1.tar", last modified: Thu Apr 25 07:28:14 2024, max compression
```

## Comparing `erlab-2.3.0.tar` & `erlab-2.3.1.tar`

### file list

```diff
@@ -1,184 +1,185 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.210777 erlab-2.3.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.166777 erlab-2.3.0/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.170776 erlab-2.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)     2216 2024-04-22 14:23:20.000000 erlab-2.3.0/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 root         (0) root         (0)      194 2024-04-22 14:23:20.000000 erlab-2.3.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)     1095 2024-04-22 14:23:20.000000 erlab-2.3.0/.github/ISSUE_TEMPLATE/feature-request.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.174777 erlab-2.3.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-22 14:23:20.000000 erlab-2.3.0/.github/workflows/pr.yml
--rw-r--r--   0 root         (0) root         (0)     1893 2024-04-22 14:23:20.000000 erlab-2.3.0/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2898 2024-04-22 14:23:20.000000 erlab-2.3.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)      893 2024-04-22 14:23:20.000000 erlab-2.3.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      793 2024-04-22 14:23:20.000000 erlab-2.3.0/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)   116984 2024-04-22 14:23:23.000000 erlab-2.3.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    35149 2024-04-22 14:23:20.000000 erlab-2.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    48155 2024-04-22 14:23:27.210777 erlab-2.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1473 2024-04-22 14:23:20.000000 erlab-2.3.0/PythonInterface.ipf
--rw-r--r--   0 root         (0) root         (0)     5147 2024-04-22 14:23:20.000000 erlab-2.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.174777 erlab-2.3.0/docs/
--rw-r--r--   0 root         (0) root         (0)      638 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      682 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/environment.yml
--rw-r--r--   0 root         (0) root         (0)      804 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      419 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.178777 erlab-2.3.0/docs/source/
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/bibliography.rst
--rw-r--r--   0 root         (0) root         (0)    17600 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)    15451 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/contributing.rst
--rw-r--r--   0 root         (0) root         (0)      265 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/erlab.accessors.rst
--rw-r--r--   0 root         (0) root         (0)      101 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/erlab.analysis.rst
--rw-r--r--   0 root         (0) root         (0)      141 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/erlab.characterization.rst
--rw-r--r--   0 root         (0) root         (0)      485 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/erlab.constants.rst
--rw-r--r--   0 root         (0) root         (0)      116 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/erlab.interactive.rst
--rw-r--r--   0 root         (0) root         (0)       81 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/erlab.io.rst
--rw-r--r--   0 root         (0) root         (0)      236 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/erlab.lattice.rst
--rw-r--r--   0 root         (0) root         (0)      224 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/erlab.parallel.rst
--rw-r--r--   0 root         (0) root         (0)      174 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/erlab.plotting.rst
--rw-r--r--   0 root         (0) root         (0)     4221 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/getting-started.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.182777 erlab-2.3.0/docs/source/images/
--rw-r--r--   0 root         (0) root         (0)   328062 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/images/flowchart_multiple.pdf
--rw-r--r--   0 root         (0) root         (0)   328737 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/images/flowchart_single.pdf
--rw-r--r--   0 root         (0) root         (0)   996803 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/images/imagetool_dark.png
--rw-r--r--   0 root         (0) root         (0)   966547 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/images/imagetool_light.png
--rw-r--r--   0 root         (0) root         (0)   709231 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/images/ktool_1_dark.png
--rw-r--r--   0 root         (0) root         (0)   694078 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/images/ktool_1_light.png
--rw-r--r--   0 root         (0) root         (0)   703343 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/images/ktool_2_dark.png
--rw-r--r--   0 root         (0) root         (0)   686688 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/images/ktool_2_light.png
--rw-r--r--   0 root         (0) root         (0)     3119 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.186777 erlab-2.3.0/docs/source/pyplots/
--rw-r--r--   0 root         (0) root         (0)     2578 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/pyplots/norms.py
--rw-r--r--   0 root         (0) root         (0)     1344 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/reference.rst
--rw-r--r--   0 root         (0) root         (0)     3099 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/refs.bib
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.186777 erlab-2.3.0/docs/source/user-guide/
--rw-r--r--   0 root         (0) root         (0)    40199 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/user-guide/curve-fitting.ipynb
--rw-r--r--   0 root         (0) root         (0)     2598 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/user-guide/imagetool.rst
--rw-r--r--   0 root         (0) root         (0)     1291 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/user-guide/index.rst
--rw-r--r--   0 root         (0) root         (0)     9011 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/user-guide/indexing.ipynb
--rw-r--r--   0 root         (0) root         (0)    53431 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/user-guide/io.ipynb
--rw-r--r--   0 root         (0) root         (0)   558328 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/user-guide/kconv.ipynb
--rw-r--r--   0 root         (0) root         (0)    25976 2024-04-22 14:23:20.000000 erlab-2.3.0/docs/source/user-guide/plotting.ipynb
--rw-r--r--   0 root         (0) root         (0)      521 2024-04-22 14:23:20.000000 erlab-2.3.0/environment.yml
--rw-r--r--   0 root         (0) root         (0)     3955 2024-04-22 14:23:20.000000 erlab-2.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      344 2024-04-22 14:23:20.000000 erlab-2.3.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 14:23:27.214777 erlab-2.3.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.166777 erlab-2.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.190777 erlab-2.3.0/src/erlab/
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-22 14:23:23.000000 erlab-2.3.0/src/erlab/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.190777 erlab-2.3.0/src/erlab/accessors/
--rw-r--r--   0 root         (0) root         (0)      778 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/accessors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25462 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/accessors/fit.py
--rw-r--r--   0 root         (0) root         (0)    29354 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/accessors/kspace.py
--rw-r--r--   0 root         (0) root         (0)     6418 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/accessors/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.194777 erlab-2.3.0/src/erlab/analysis/
--rw-r--r--   0 root         (0) root         (0)      723 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5514 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/analysis/correlation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.194777 erlab-2.3.0/src/erlab/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)      168 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/analysis/fit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.194777 erlab-2.3.0/src/erlab/analysis/fit/functions/
--rw-r--r--   0 root         (0) root         (0)      957 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/analysis/fit/functions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10583 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/analysis/fit/functions/dynamic.py
--rw-r--r--   0 root         (0) root         (0)     9670 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/analysis/fit/functions/general.py
--rw-r--r--   0 root         (0) root         (0)     6510 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/analysis/fit/minuit.py
--rw-r--r--   0 root         (0) root         (0)    12675 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/analysis/fit/models.py
--rw-r--r--   0 root         (0) root         (0)     1156 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/analysis/fit/spline.py
--rw-r--r--   0 root         (0) root         (0)    20178 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/analysis/gold.py
--rw-r--r--   0 root         (0) root         (0)    17325 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/analysis/image.py
--rw-r--r--   0 root         (0) root         (0)    10468 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/analysis/interpolate.py
--rw-r--r--   0 root         (0) root         (0)    10491 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/analysis/kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.194777 erlab-2.3.0/src/erlab/analysis/mask/
--rw-r--r--   0 root         (0) root         (0)     5401 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/analysis/mask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8440 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/analysis/mask/polygon.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/analysis/transform.py
--rw-r--r--   0 root         (0) root         (0)     5288 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/analysis/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.194777 erlab-2.3.0/src/erlab/characterization/
--rw-r--r--   0 root         (0) root         (0)      191 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3093 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/characterization/resistance.py
--rw-r--r--   0 root         (0) root         (0)     1897 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/characterization/xrd.py
--rw-r--r--   0 root         (0) root         (0)     2152 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.198777 erlab-2.3.0/src/erlab/interactive/
--rw-r--r--   0 root         (0) root         (0)      525 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/interactive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13953 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/interactive/bzplot.py
--rw-r--r--   0 root         (0) root         (0)    21311 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/interactive/colors.py
--rw-r--r--   0 root         (0) root         (0)    22774 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/interactive/curvefittingtool.py
--rw-r--r--   0 root         (0) root         (0)    11443 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/interactive/derivative.py
--rw-r--r--   0 root         (0) root         (0)    16300 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/interactive/dtool.ui
--rw-r--r--   0 root         (0) root         (0)    19138 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/interactive/fermiedge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.198777 erlab-2.3.0/src/erlab/interactive/imagetool/
--rw-r--r--   0 root         (0) root         (0)    19696 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/interactive/imagetool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.198777 erlab-2.3.0/src/erlab/interactive/imagetool/_deprecated/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/interactive/imagetool/_deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51945 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
--rw-r--r--   0 root         (0) root         (0)   114560 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
--rw-r--r--   0 root         (0) root         (0)    27081 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/interactive/imagetool/controls.py
--rw-r--r--   0 root         (0) root         (0)    54116 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/interactive/imagetool/core.py
--rw-r--r--   0 root         (0) root         (0)    13907 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/interactive/imagetool/fastbinning.py
--rw-r--r--   0 root         (0) root         (0)    25270 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/interactive/imagetool/slicer.py
--rw-r--r--   0 root         (0) root         (0)    15835 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/interactive/kspace.py
--rw-r--r--   0 root         (0) root         (0)    19382 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/interactive/ktool.ui
--rw-r--r--   0 root         (0) root         (0)     3341 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/interactive/masktool.py
--rw-r--r--   0 root         (0) root         (0)    54107 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/interactive/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.202777 erlab-2.3.0/src/erlab/io/
--rw-r--r--   0 root         (0) root         (0)     2175 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40888 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/io/dataloader.py
--rw-r--r--   0 root         (0) root         (0)    12590 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/io/exampledata.py
--rw-r--r--   0 root         (0) root         (0)     6893 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/io/igor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.202777 erlab-2.3.0/src/erlab/io/plugins/
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/io/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3672 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/io/plugins/da30.py
--rw-r--r--   0 root         (0) root         (0)     1160 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/io/plugins/kriss.py
--rw-r--r--   0 root         (0) root         (0)     8022 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/io/plugins/merlin.py
--rw-r--r--   0 root         (0) root         (0)     7838 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/io/plugins/ssrl52.py
--rw-r--r--   0 root         (0) root         (0)     6794 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/io/utilities.py
--rw-r--r--   0 root         (0) root         (0)     2533 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/lattice.py
--rw-r--r--   0 root         (0) root         (0)     1559 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/parallel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.202777 erlab-2.3.0/src/erlab/plotting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.206777 erlab-2.3.0/src/erlab/plotting/IgorCT/
--rw-r--r--   0 root         (0) root         (0)     3379 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/IgorCT/Blue-White.txt
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/IgorCT/BlueHot.ibw
--rw-r--r--   0 root         (0) root         (0)     3526 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
--rw-r--r--   0 root         (0) root         (0)     3530 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
--rw-r--r--   0 root         (0) root         (0)     3531 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/IgorCT/ColdWarm.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/IgorCT/PlanetEarth.ibw
--rw-r--r--   0 root         (0) root         (0)     1920 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/IgorCT/ametrine.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/IgorCT/isolum.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/IgorCT/morgenstemning.ibw
--rw-r--r--   0 root         (0) root         (0)     2026 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28998 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/annotations.py
--rw-r--r--   0 root         (0) root         (0)    18278 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/atoms.py
--rw-r--r--   0 root         (0) root         (0)     4295 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/bz.py
--rw-r--r--   0 root         (0) root         (0)    37450 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/colors.py
--rw-r--r--   0 root         (0) root         (0)     2657 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/erplot.py
--rw-r--r--   0 root         (0) root         (0)    31270 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/general.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/plot3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.206777 erlab-2.3.0/src/erlab/plotting/stylelib/
--rw-r--r--   0 root         (0) root         (0)     6839 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/stylelib/fira.mplstyle
--rw-r--r--   0 root         (0) root         (0)     6826 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/stylelib/firalight.mplstyle
--rw-r--r--   0 root         (0) root         (0)    14358 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/stylelib/khan.mplstyle
--rw-r--r--   0 root         (0) root         (0)     9160 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/stylelib/nature.mplstyle
--rw-r--r--   0 root         (0) root         (0)      630 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/stylelib/poster.mplstyle
--rw-r--r--   0 root         (0) root         (0)     7023 2024-04-22 14:23:20.000000 erlab-2.3.0/src/erlab/plotting/stylelib/times.mplstyle
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.210777 erlab-2.3.0/src/erlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)    48155 2024-04-22 14:23:27.000000 erlab-2.3.0/src/erlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4928 2024-04-22 14:23:27.000000 erlab-2.3.0/src/erlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 14:23:27.000000 erlab-2.3.0/src/erlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      554 2024-04-22 14:23:27.000000 erlab-2.3.0/src/erlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-22 14:23:27.000000 erlab-2.3.0/src/erlab.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.206777 erlab-2.3.0/templates/
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-22 14:23:20.000000 erlab-2.3.0/templates/.macros.j2
--rw-r--r--   0 root         (0) root         (0)      161 2024-04-22 14:23:20.000000 erlab-2.3.0/templates/.release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)      423 2024-04-22 14:23:20.000000 erlab-2.3.0/templates/CHANGELOG.md.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.170776 erlab-2.3.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.206777 erlab-2.3.0/tests/accessors/
--rw-r--r--   0 root         (0) root         (0)     5758 2024-04-22 14:23:20.000000 erlab-2.3.0/tests/accessors/test_fit.py
--rw-r--r--   0 root         (0) root         (0)     4035 2024-04-22 14:23:20.000000 erlab-2.3.0/tests/accessors/test_kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.210777 erlab-2.3.0/tests/analysis/
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-22 14:23:20.000000 erlab-2.3.0/tests/analysis/test_fastbinning.py
--rw-r--r--   0 root         (0) root         (0)     4484 2024-04-22 14:23:20.000000 erlab-2.3.0/tests/analysis/test_fit_functions_dynamic.py
--rw-r--r--   0 root         (0) root         (0)     4652 2024-04-22 14:23:20.000000 erlab-2.3.0/tests/analysis/test_fit_functions_general.py
--rw-r--r--   0 root         (0) root         (0)     6036 2024-04-22 14:23:20.000000 erlab-2.3.0/tests/analysis/test_fit_models.py
--rw-r--r--   0 root         (0) root         (0)     5228 2024-04-22 14:23:20.000000 erlab-2.3.0/tests/analysis/test_image.py
--rw-r--r--   0 root         (0) root         (0)     1472 2024-04-22 14:23:20.000000 erlab-2.3.0/tests/analysis/test_interpolate.py
--rw-r--r--   0 root         (0) root         (0)     1463 2024-04-22 14:23:20.000000 erlab-2.3.0/tests/analysis/test_kspace.py
--rw-r--r--   0 root         (0) root         (0)      718 2024-04-22 14:23:20.000000 erlab-2.3.0/tests/analysis/test_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 14:23:27.210777 erlab-2.3.0/tests/io/
--rw-r--r--   0 root         (0) root         (0)     9339 2024-04-22 14:23:20.000000 erlab-2.3.0/tests/io/test_dataloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.932838 erlab-2.3.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.884838 erlab-2.3.1/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.892838 erlab-2.3.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)     2200 2024-04-25 07:28:07.000000 erlab-2.3.1/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 root         (0) root         (0)      206 2024-04-25 07:28:07.000000 erlab-2.3.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-25 07:28:07.000000 erlab-2.3.1/.github/ISSUE_TEMPLATE/feature-request.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.892838 erlab-2.3.1/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-25 07:28:07.000000 erlab-2.3.1/.github/workflows/pr.yml
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-04-25 07:28:07.000000 erlab-2.3.1/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-25 07:28:07.000000 erlab-2.3.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-25 07:28:07.000000 erlab-2.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      793 2024-04-25 07:28:07.000000 erlab-2.3.1/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)   118618 2024-04-25 07:28:11.000000 erlab-2.3.1/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2024-04-25 07:28:07.000000 erlab-2.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    48058 2024-04-25 07:28:14.932838 erlab-2.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-04-25 07:28:07.000000 erlab-2.3.1/PythonInterface.ipf
+-rw-r--r--   0 root         (0) root         (0)     5147 2024-04-25 07:28:07.000000 erlab-2.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.892838 erlab-2.3.1/docs/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      804 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      495 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.896838 erlab-2.3.1/docs/source/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/bibliography.rst
+-rw-r--r--   0 root         (0) root         (0)    17632 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)    15196 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)      106 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/erlab.accessors.rst
+-rw-r--r--   0 root         (0) root         (0)      101 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/erlab.analysis.rst
+-rw-r--r--   0 root         (0) root         (0)      485 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/erlab.constants.rst
+-rw-r--r--   0 root         (0) root         (0)      116 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/erlab.interactive.rst
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/erlab.io.rst
+-rw-r--r--   0 root         (0) root         (0)      236 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/erlab.lattice.rst
+-rw-r--r--   0 root         (0) root         (0)      224 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/erlab.parallel.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/erlab.plotting.rst
+-rw-r--r--   0 root         (0) root         (0)     4221 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/getting-started.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.904838 erlab-2.3.1/docs/source/images/
+-rw-r--r--   0 root         (0) root         (0)   328062 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/images/flowchart_multiple.pdf
+-rw-r--r--   0 root         (0) root         (0)   328737 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/images/flowchart_single.pdf
+-rw-r--r--   0 root         (0) root         (0)   996803 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/images/imagetool_dark.png
+-rw-r--r--   0 root         (0) root         (0)   966547 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/images/imagetool_light.png
+-rw-r--r--   0 root         (0) root         (0)   709231 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/images/ktool_1_dark.png
+-rw-r--r--   0 root         (0) root         (0)   694078 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/images/ktool_1_light.png
+-rw-r--r--   0 root         (0) root         (0)   703343 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/images/ktool_2_dark.png
+-rw-r--r--   0 root         (0) root         (0)   686688 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/images/ktool_2_light.png
+-rw-r--r--   0 root         (0) root         (0)     3119 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.904838 erlab-2.3.1/docs/source/pyplots/
+-rw-r--r--   0 root         (0) root         (0)     2604 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/pyplots/norms.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/reference.rst
+-rw-r--r--   0 root         (0) root         (0)     3099 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/refs.bib
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.908838 erlab-2.3.1/docs/source/user-guide/
+-rw-r--r--   0 root         (0) root         (0)    41262 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/user-guide/curve-fitting.ipynb
+-rw-r--r--   0 root         (0) root         (0)     2598 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/user-guide/imagetool.rst
+-rw-r--r--   0 root         (0) root         (0)     1291 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/user-guide/index.rst
+-rw-r--r--   0 root         (0) root         (0)     9017 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/user-guide/indexing.ipynb
+-rw-r--r--   0 root         (0) root         (0)    54332 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/user-guide/io.ipynb
+-rw-r--r--   0 root         (0) root         (0)    10710 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/user-guide/kconv.ipynb
+-rw-r--r--   0 root         (0) root         (0)    26977 2024-04-25 07:28:07.000000 erlab-2.3.1/docs/source/user-guide/plotting.ipynb
+-rw-r--r--   0 root         (0) root         (0)      464 2024-04-25 07:28:07.000000 erlab-2.3.1/environment.yml
+-rw-r--r--   0 root         (0) root         (0)     4689 2024-04-25 07:28:07.000000 erlab-2.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      299 2024-04-25 07:28:07.000000 erlab-2.3.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 07:28:14.932838 erlab-2.3.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.888838 erlab-2.3.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.908838 erlab-2.3.1/src/erlab/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-25 07:28:11.000000 erlab-2.3.1/src/erlab/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.908838 erlab-2.3.1/src/erlab/accessors/
+-rw-r--r--   0 root         (0) root         (0)      778 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/accessors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25941 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/accessors/fit.py
+-rw-r--r--   0 root         (0) root         (0)    29991 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/accessors/kspace.py
+-rw-r--r--   0 root         (0) root         (0)     7133 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/accessors/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.912838 erlab-2.3.1/src/erlab/analysis/
+-rw-r--r--   0 root         (0) root         (0)      723 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5611 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/analysis/correlation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.912838 erlab-2.3.1/src/erlab/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)      168 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/analysis/fit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.912838 erlab-2.3.1/src/erlab/analysis/fit/functions/
+-rw-r--r--   0 root         (0) root         (0)      957 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/analysis/fit/functions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10753 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/analysis/fit/functions/dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     9691 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/analysis/fit/functions/general.py
+-rw-r--r--   0 root         (0) root         (0)     6968 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/analysis/fit/minuit.py
+-rw-r--r--   0 root         (0) root         (0)    12659 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/analysis/fit/models.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/analysis/fit/spline.py
+-rw-r--r--   0 root         (0) root         (0)    20224 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/analysis/gold.py
+-rw-r--r--   0 root         (0) root         (0)    18225 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/analysis/image.py
+-rw-r--r--   0 root         (0) root         (0)    10496 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/analysis/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)    10184 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/analysis/kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.912838 erlab-2.3.1/src/erlab/analysis/mask/
+-rw-r--r--   0 root         (0) root         (0)     5401 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/analysis/mask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8481 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/analysis/mask/polygon.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/analysis/transform.py
+-rw-r--r--   0 root         (0) root         (0)     5444 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/analysis/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.912838 erlab-2.3.1/src/erlab/characterization/
+-rw-r--r--   0 root         (0) root         (0)      231 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.916838 erlab-2.3.1/src/erlab/interactive/
+-rw-r--r--   0 root         (0) root         (0)      525 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/interactive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14334 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/interactive/bzplot.py
+-rw-r--r--   0 root         (0) root         (0)    21351 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/interactive/colors.py
+-rw-r--r--   0 root         (0) root         (0)    23024 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/interactive/curvefittingtool.py
+-rw-r--r--   0 root         (0) root         (0)    11793 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/interactive/derivative.py
+-rw-r--r--   0 root         (0) root         (0)    16300 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/interactive/dtool.ui
+-rw-r--r--   0 root         (0) root         (0)    19282 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/interactive/fermiedge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.916838 erlab-2.3.1/src/erlab/interactive/imagetool/
+-rw-r--r--   0 root         (0) root         (0)    19829 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/interactive/imagetool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.916838 erlab-2.3.1/src/erlab/interactive/imagetool/_deprecated/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/interactive/imagetool/_deprecated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52047 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
+-rw-r--r--   0 root         (0) root         (0)   114573 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
+-rw-r--r--   0 root         (0) root         (0)    27450 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/interactive/imagetool/controls.py
+-rw-r--r--   0 root         (0) root         (0)    54842 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/interactive/imagetool/core.py
+-rw-r--r--   0 root         (0) root         (0)    13599 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/interactive/imagetool/fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)    25433 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/interactive/imagetool/slicer.py
+-rw-r--r--   0 root         (0) root         (0)    16051 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/interactive/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    19382 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/interactive/ktool.ui
+-rw-r--r--   0 root         (0) root         (0)     2749 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/interactive/masktool.py
+-rw-r--r--   0 root         (0) root         (0)    54600 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/interactive/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.920838 erlab-2.3.1/src/erlab/io/
+-rw-r--r--   0 root         (0) root         (0)     2195 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.920838 erlab-2.3.1/src/erlab/io/characterization/
+-rw-r--r--   0 root         (0) root         (0)      170 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/io/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3091 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/io/characterization/resistance.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/io/characterization/xrd.py
+-rw-r--r--   0 root         (0) root         (0)    41911 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/io/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)    12251 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/io/exampledata.py
+-rw-r--r--   0 root         (0) root         (0)     6998 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/io/igor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.920838 erlab-2.3.1/src/erlab/io/plugins/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/io/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3615 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/io/plugins/da30.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/io/plugins/kriss.py
+-rw-r--r--   0 root         (0) root         (0)     8166 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/io/plugins/merlin.py
+-rw-r--r--   0 root         (0) root         (0)     7667 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/io/plugins/ssrl52.py
+-rw-r--r--   0 root         (0) root         (0)     6806 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/io/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/lattice.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/parallel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.920838 erlab-2.3.1/src/erlab/plotting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.924838 erlab-2.3.1/src/erlab/plotting/IgorCT/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/IgorCT/Blue-White.txt
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/IgorCT/BlueHot.ibw
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
+-rw-r--r--   0 root         (0) root         (0)     3530 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
+-rw-r--r--   0 root         (0) root         (0)     3531 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/IgorCT/ColdWarm.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/IgorCT/PlanetEarth.ibw
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/IgorCT/ametrine.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/IgorCT/isolum.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/IgorCT/morgenstemning.ibw
+-rw-r--r--   0 root         (0) root         (0)     2113 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29615 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/annotations.py
+-rw-r--r--   0 root         (0) root         (0)    18641 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/atoms.py
+-rw-r--r--   0 root         (0) root         (0)     4381 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/bz.py
+-rw-r--r--   0 root         (0) root         (0)    39514 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/colors.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/erplot.py
+-rw-r--r--   0 root         (0) root         (0)    33231 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/general.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/plot3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.924838 erlab-2.3.1/src/erlab/plotting/stylelib/
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/stylelib/fira.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     6826 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/stylelib/firalight.mplstyle
+-rw-r--r--   0 root         (0) root         (0)    14358 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/stylelib/khan.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     9160 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/stylelib/nature.mplstyle
+-rw-r--r--   0 root         (0) root         (0)      630 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/stylelib/poster.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     7023 2024-04-25 07:28:07.000000 erlab-2.3.1/src/erlab/plotting/stylelib/times.mplstyle
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.928838 erlab-2.3.1/src/erlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    48058 2024-04-25 07:28:14.000000 erlab-2.3.1/src/erlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4937 2024-04-25 07:28:14.000000 erlab-2.3.1/src/erlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 07:28:14.000000 erlab-2.3.1/src/erlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      502 2024-04-25 07:28:14.000000 erlab-2.3.1/src/erlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-25 07:28:14.000000 erlab-2.3.1/src/erlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.924838 erlab-2.3.1/templates/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-25 07:28:07.000000 erlab-2.3.1/templates/.macros.j2
+-rw-r--r--   0 root         (0) root         (0)      161 2024-04-25 07:28:07.000000 erlab-2.3.1/templates/.release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)      423 2024-04-25 07:28:07.000000 erlab-2.3.1/templates/CHANGELOG.md.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.888838 erlab-2.3.1/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.928838 erlab-2.3.1/tests/accessors/
+-rw-r--r--   0 root         (0) root         (0)     5785 2024-04-25 07:28:07.000000 erlab-2.3.1/tests/accessors/test_fit.py
+-rw-r--r--   0 root         (0) root         (0)     4035 2024-04-25 07:28:07.000000 erlab-2.3.1/tests/accessors/test_kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.928838 erlab-2.3.1/tests/analysis/
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-25 07:28:07.000000 erlab-2.3.1/tests/analysis/test_fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)     4497 2024-04-25 07:28:07.000000 erlab-2.3.1/tests/analysis/test_fit_functions_dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2024-04-25 07:28:07.000000 erlab-2.3.1/tests/analysis/test_fit_functions_general.py
+-rw-r--r--   0 root         (0) root         (0)     6036 2024-04-25 07:28:07.000000 erlab-2.3.1/tests/analysis/test_fit_models.py
+-rw-r--r--   0 root         (0) root         (0)     5228 2024-04-25 07:28:07.000000 erlab-2.3.1/tests/analysis/test_image.py
+-rw-r--r--   0 root         (0) root         (0)     1472 2024-04-25 07:28:07.000000 erlab-2.3.1/tests/analysis/test_interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2024-04-25 07:28:07.000000 erlab-2.3.1/tests/analysis/test_kspace.py
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-25 07:28:07.000000 erlab-2.3.1/tests/analysis/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 07:28:14.928838 erlab-2.3.1/tests/io/
+-rw-r--r--   0 root         (0) root         (0)     9383 2024-04-25 07:28:07.000000 erlab-2.3.1/tests/io/test_dataloader.py
```

### Comparing `erlab-2.3.0/.github/ISSUE_TEMPLATE/bug-report.yml` & `erlab-2.3.1/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files 6% similar despite different names*

```diff
@@ -2,36 +2,37 @@
 description: Create a report to help us improve.
 labels: [bug]
 assignees: [kmnhan]
 body:
   - type: textarea
     id: what-happened
     attributes:
-      label: What happened?
+      label: Description
       description: |
         Thanks for reporting a bug! Please describe what you were trying to get done.
         Tell us what happened, what went wrong.
     validations:
       required: true
 
   - type: textarea
     id: what-did-you-expect-to-happen
     attributes:
-      label: What did you expect to happen?
+      label: Expected behavior
       description: |
         A clear and concise description of what you expected to happen.
     validations:
       required: false
 
   - type: textarea
     id: sample-code
     attributes:
       label: Minimal Complete Verifiable Example
       description: |
-        Minimal, self-contained copy-pastable example that demonstrates the issue.         This will be automatically formatted into code, so no need for markdown backticks.
+        Minimal, self-contained copy-pastable example that demonstrates the issue.
+        This will be automatically formatted into code, so no need for markdown backticks.
       render: Python
 
   - type: checkboxes
     id: mvce-checkboxes
     attributes:
       label: MVCE confirmation
       description: |
```

### Comparing `erlab-2.3.0/.github/ISSUE_TEMPLATE/feature-request.yml` & `erlab-2.3.1/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files 10% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 description: Suggest an idea for this project.
 labels: [enhancement]
 assignees: [kmnhan]
 body:
   - type: textarea
     id: description
     attributes:
-      label: Is your feature request related to a problem? Please describe.
+      label: Description
       description: |
-        A clear and concise description of what the problem is. Ex. I'm always frustrated when [...]
+        Is your feature request related to a problem?
+        Please provide a clear and concise description of what the problem is. Ex. I'm always frustrated when [...]
     validations:
       required: true
   - type: textarea
     id: solution
     attributes:
-      label: Describe the solution you'd like
+      label: Possible solution
       description: |
         A clear and concise description of what you want to happen.
   - type: textarea
     id: alternatives
     attributes:
-      label: Describe alternatives you've considered
+      label: Alternatives
       description: |
         A clear and concise description of any alternative solutions or features you've considered.
     validations:
       required: false
   - type: textarea
     id: additional-context
     attributes:
```

### Comparing `erlab-2.3.0/.github/workflows/pr.yml` & `erlab-2.3.1/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/.github/workflows/release.yml` & `erlab-2.3.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/.gitignore` & `erlab-2.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/.pre-commit-config.yaml` & `erlab-2.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/.readthedocs.yaml` & `erlab-2.3.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/CHANGELOG.md` & `erlab-2.3.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,46 @@
 # CHANGELOG
 
 
 
+## v2.3.1 (2024-04-25)
+
+### Chore
+
+* (**deps**) make `iminuit` and `superqt` optional ([`1bbcc24`](https://github.com/kmnhan/erlabpy/commit/1bbcc24268312f8c285df0774e1e5d5c8c775650))
+
+* (**deps**) reduce dependencies ([`6a03518`](https://github.com/kmnhan/erlabpy/commit/6a0351859ace99dbfb4f251ccbb78e581d6f7218))
+
+* (**github**) update issue templates ([`6a2dd50`](https://github.com/kmnhan/erlabpy/commit/6a2dd504ac05c5c47a39499dab991d44daee57f9))
+
+* (**deps**) update lmfit dependencies to include &gt;1.3.0 ([`942a810`](https://github.com/kmnhan/erlabpy/commit/942a810783fb574cc36a446333be09a82b1d22ae))
+
+### Fix
+
+* (**interactive**) keep pointer for imagetool, fix typing issues ([`c98c38e`](https://github.com/kmnhan/erlabpy/commit/c98c38ea11bce50ed9bfd8d374064bb2b1659d0c))
+
+* (**kspace**) allow explicit coordinate kwargs ([`fe47efc`](https://github.com/kmnhan/erlabpy/commit/fe47efcde941767c02b582ce8b29d4b3678fd843))
+
+### Refactor
+
+* move `characterization` to `io` ([`9c30f1b`](https://github.com/kmnhan/erlabpy/commit/9c30f1b7df51460f502dcbf999e3fac34be1cf99))
+
+* make zip strict (ruff B905) ([`78bf5f5`](https://github.com/kmnhan/erlabpy/commit/78bf5f5a2db52c14ccf5bfd3c83659ca53c4a408))
+
+### Style
+
+* add mypy compatible type hints ([`c97724d`](https://github.com/kmnhan/erlabpy/commit/c97724dcd9095a3cdc1842e5afb1f29b3c472c45))
+
+### Unknown
+
+* Merge pull request #26 from kmnhan/dev ([`85a60b3`](https://github.com/kmnhan/erlabpy/commit/85a60b37c29aca93db97004f776e8dcdd3d38666))
+
+* Merge branch &#39;main&#39; into dev ([`184afb0`](https://github.com/kmnhan/erlabpy/commit/184afb023dc704b4ab6ffe8ef5c098c19ca19084))
+
+
 ## v2.3.0 (2024-04-22)
 
 ### Chore
 
 * cleanup directory ([`40e1f8d`](https://github.com/kmnhan/erlabpy/commit/40e1f8dcce66d53f9de6fd5905cef3c690633c98))
 
 * customize issue template chooser ([`0aa7617`](https://github.com/kmnhan/erlabpy/commit/0aa7617e7794449756df0abfc3260c6e545f97a3))
```

### Comparing `erlab-2.3.0/LICENSE` & `erlab-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/PKG-INFO` & `erlab-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.3.0
+Version: 2.3.1
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -692,30 +692,27 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: h5netcdf>=1.2.0
 Requires-Dist: igor2>=0.5.6
-Requires-Dist: iminuit>=2.25.2
 Requires-Dist: joblib>=1.3.2
-Requires-Dist: lmfit<1.3.0,>=1.2.0
+Requires-Dist: lmfit!=1.3.0,>=1.2.0
 Requires-Dist: matplotlib>=3.8.0
-Requires-Dist: numba-progress>=1.0.0
 Requires-Dist: numba>=0.59.0
 Requires-Dist: numbagg>=0.8.1
 Requires-Dist: numpy>=1.26.0
 Requires-Dist: pyperclip>=1.8.2
 Requires-Dist: pyqtgraph>=0.13.1
 Requires-Dist: qtawesome>=1.3.1
 Requires-Dist: qtpy>=2.4.1
 Requires-Dist: scipy>=1.12.0
-Requires-Dist: superqt>=0.6.2
 Requires-Dist: tqdm>=4.66.2
-Requires-Dist: uncertainties>=3.0.1
+Requires-Dist: uncertainties>=3.1.4
 Requires-Dist: varname>=0.13.0
 Requires-Dist: xarray>=2024.02.0
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
```

### Comparing `erlab-2.3.0/PythonInterface.ipf` & `erlab-2.3.1/PythonInterface.ipf`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/README.md` & `erlab-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/docs/Makefile` & `erlab-2.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/docs/make.bat` & `erlab-2.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/docs/source/conf.py` & `erlab-2.3.1/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,16 @@
 exclude_patterns = []
 
 default_role = "obj"
 
 # nitpicky = False
 # nitpick_ignore = [("py:class", "numpy.float64")]
 
+highlight_language = "python3"
+
 # -- Linkcode settings -------------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html
 
 
 # based on numpy doc/source/conf.py
 def linkcode_resolve(domain, info):
     """
```

### Comparing `erlab-2.3.0/docs/source/contributing.rst` & `erlab-2.3.1/docs/source/contributing.rst`

 * *Files 4% similar despite different names*

```diff
@@ -251,19 +251,19 @@
    determine the version number for the next release.
 
 2. To push the changes up to your forked repo on GitHub, do a ``git push``.
 
 Open a pull request
 -------------------
 
-When you're ready or need feedback on your code, open a Pull Request (PR) so that the
-xarray developers can give feedback and eventually include your suggested code into the
-``main`` branch. `Pull requests (PRs) on GitHub
+When you're ready or need feedback on your code, open a Pull Request (PR) so that we can
+give feedback and eventually include your suggested code into the ``main`` branch. `Pull
+requests (PRs) on GitHub
 <https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests>`_
-are the mechanism for contributing to xarray's code and documentation.
+are the mechanism for contributing to the code and documentation.
 
 Enter a title for the set of changes with some explanation of what you've done. Mention
 anything you'd like particular attention for - such as a complicated change or some code
 you are not happy with. If you don't think your request is ready to be merged, just say
 so in your pull request message and use the "Draft PR" feature of GitHub. This is a good
 way of getting some preliminary code review.
 
@@ -283,15 +283,15 @@
 
   * Import all Qt bindings from `qtpy <https://github.com/spyder-ide/qtpy>`_, and only
     import the top level modules: ::
 
       from qtpy import QtWidgets, QtCore, QtGui
 
   * Use fully qualified enum names from Qt6 instead of the short-form enums from Qt5, i.
-    e., ``QtCore.Qt.CheckState.Checked`` instead of ``QtCore.Qt.Checked``.
+    e., `QtCore.Qt.CheckState.Checked` instead of `QtCore.Qt.Checked`.
 
   * Use the signal and slot syntax from PySide6 (``QtCore.Signal`` and ``QtCore.Slot``
     instead of ``QtCore.pyqtSignal`` and ``QtCore.pyqtSlot``)
 
   * When using Qt Designer, place ``.ui`` files in the same directory as the Python file
     that   uses them. The files must be imported using the ``loadUiType`` function from
     ``qtpy.uic``. For example: ::
@@ -302,20 +302,17 @@
           def __init__(self):
               super().__init__()
               self.setupUi(self)
 
 - Please try to add type annotations to your code. This will help with code completion
   and static analysis.
 
-- Although it would be great to enforce static type checking, our code base currently
-  does not pass the tests. It would require a large amount of work to get it to pass, so
-  we are not enforcing it at the moment, and it is unclear whether the extra effort is
-  worth it. See `this article
-  <https://typing.readthedocs.io/en/latest/source/typing_anti_pitch.html>`_ for some
-  reasons to avoid static type checking.
+- We are in the process of adding type annotations to the codebase, and most of it
+  should pass `mypy <https://mypy.readthedocs.io/en/stable/>`_ except for the io and
+  interactive modules.
 
 Documentation
 =============
 
 The documentation is written in **reStructuredText**, which is almost like writing in
 plain English, and built using `Sphinx <http://sphinx-doc.org/>`__. The Sphinx
 Documentation has an excellent `introduction to reST
```

### Comparing `erlab-2.3.0/docs/source/getting-started.rst` & `erlab-2.3.1/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/docs/source/images/flowchart_multiple.pdf` & `erlab-2.3.1/docs/source/images/flowchart_multiple.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/docs/source/images/flowchart_single.pdf` & `erlab-2.3.1/docs/source/images/flowchart_single.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/docs/source/images/imagetool_dark.png` & `erlab-2.3.1/docs/source/images/imagetool_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/docs/source/images/imagetool_light.png` & `erlab-2.3.1/docs/source/images/imagetool_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/docs/source/images/ktool_1_dark.png` & `erlab-2.3.1/docs/source/images/ktool_1_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/docs/source/images/ktool_1_light.png` & `erlab-2.3.1/docs/source/images/ktool_1_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/docs/source/images/ktool_2_dark.png` & `erlab-2.3.1/docs/source/images/ktool_2_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/docs/source/images/ktool_2_light.png` & `erlab-2.3.1/docs/source/images/ktool_2_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/docs/source/index.rst` & `erlab-2.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/docs/source/pyplots/norms.py` & `erlab-2.3.1/docs/source/pyplots/norms.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,19 +55,19 @@
         1,
         num + 1,
         width_ratios=[9 - num] + [1] * num,
         layout="constrained",
         figsize=eplt.figwh(),
     )
 
-    for norm, label, k0, k1 in zip(norms, labels, kw0, kw1):
+    for norm, label, k0, k1 in zip(norms, labels, kw0, kw1, strict=True):
         axs[0].plot(x, norm(**k0, **k1)(x), label=label)
 
     bar_data = modulatedBarData(384, 256)
-    for i, (ax, norm, k1) in enumerate(zip(axs[1:], norms, kw1)):
+    for i, (ax, norm, k1) in enumerate(zip(axs[1:], norms, kw1, strict=True)):
         ax.plot(
             0.5,
             1,
             "o",
             c="k",
             mew=0.5,
             ms=5,
```

### Comparing `erlab-2.3.0/docs/source/reference.rst` & `erlab-2.3.1/docs/source/reference.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 *************
 API Reference
 *************
 
-ERLabPy is organized into multiple subpackages and submodules.
+ERLabPy is organized into multiple subpackages and submodules classified by their functionality. The following table lists the subpackages and submodules of ERLabPy.
 
 Subpackages
 ===========
 
 ========================   ========================
 Subpackage                 Description
 ========================   ========================
-`erlab.analysis`           Data analysis
-`erlab.io`                 Read & write ARPES data
-`erlab.plotting`           Plot
-`erlab.interactive`        Interactive plotting based on Qt and pyqtgraph
-`erlab.characterization`   Analyze sample characterization results such as XRD and transport measurements
+`erlab.analysis`           Routines for analyzing ARPES data.
+`erlab.io`                 Reading and writing data.
+`erlab.plotting`           Functions related to static plotting with matplotlib.
+`erlab.interactive`        Interactive tools and widgets based on Qt and pyqtgraph
+`erlab.accessors`          `xarray accessors <https://docs.xarray.dev/en/stable/internals/extending-xarray.html>`_. You will not need to import this module directly.
 ========================   ========================
 
 .. currentmodule:: erlab
 
 .. toctree::
    :hidden:
 
    erlab.analysis
    erlab.io
    erlab.plotting
    erlab.interactive
-   erlab.characterization
+   erlab.accessors
 
 Submodules
 ==========
 
 ==================  ==================
 Submodule           Description
 ==================  ==================
 `erlab.lattice`     Tools for working with real and reciprocal lattices.
-`erlab.constants`   Physical constants and unit conversion
-`erlab.accessors`   `xarray accessors <https://docs.xarray.dev/en/stable/internals/extending-xarray.html>`_
-`erlab.parallel`    Helpers for parallel processing
+`erlab.constants`   Physical constants and functions for unit conversion.
+`erlab.parallel`    Helpers for parallel processing.
 ==================  ==================
 
 .. toctree::
    :hidden:
 
    erlab.lattice
    erlab.constants
-   erlab.accessors
    erlab.parallel
```

### Comparing `erlab-2.3.0/docs/source/refs.bib` & `erlab-2.3.1/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/docs/source/user-guide/curve-fitting.ipynb` & `erlab-2.3.1/docs/source/user-guide/curve-fitting.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9927904044171274%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(3, 'Curve fitting in ERLabPy largely relies on `lmfit "*

 * *            "<https://lmfit.github.io/lmfit-py/>`_.\\n'), (4, 'Along with some convenient models "*

 * *            "for common fitting tasks, ERLabPy provides a powerful\\n'), (5, 'accessor that "*

 * *            "streamlines curve fitting on multidimensional xarray objects.\\n'), (7, 'ERLabPy also "*

 * *            "provides optional integration of lmfit models with `iminuit\\n'), (8, "*

 * *            "'<https://github.com/scik […]*

```diff
@@ -13,33 +13,30 @@
                     "languageId": "raw"
                 }
             },
             "source": [
                 "Curve fitting\n",
                 "=============\n",
                 "\n",
-                "ERLabPy provides two choices for curve fitting: `lmfit\n",
-                "<https://lmfit.github.io/lmfit-py/>`_ and `iminuit\n",
-                "<https://github.com/scikit-hep/iminuit>`_. \n",
-                "\n",
-                "- `lmfit <https://lmfit.github.io/lmfit-py/>`_ provides a high-level interface to\n",
-                "  optimization and curve fitting problems for Python. It builds on and extends many of\n",
-                "  the optimization methods of :mod:`scipy.optimize`, and provides a common interface for\n",
-                "  all of its supported optimization methods.\n",
-                "\n",
-                "- `iminuit <https://github.com/scikit-hep/iminuit>`_ is a Python interface to the Minuit\n",
-                "  C++ library, highly compatible with Jupyter notebooks and the SciPy ecosystem.\n",
-                "  Although developed for high-energy physics, it is a simple and easy-to-use tool for\n",
-                "  solving optimization problems.\n",
+                "Curve fitting in ERLabPy largely relies on `lmfit <https://lmfit.github.io/lmfit-py/>`_.\n",
+                "Along with some convenient models for common fitting tasks, ERLabPy provides a powerful\n",
+                "accessor that streamlines curve fitting on multidimensional xarray objects.\n",
+                "\n",
+                "ERLabPy also provides optional integration of lmfit models with `iminuit\n",
+                "<https://github.com/scikit-hep/iminuit>`_, which is a Python interface to the `Minuit\n",
+                "C++ library <https://root.cern.ch/doc/master/Minuit2Page.html>`_ developed at CERN.\n",
+                "\n",
+                "In this tutorial, we will start with the basics of curve fitting using lmfit, introduce\n",
+                "some models that are available in ERLabPy, and demonstrate curve fitting with the\n",
+                ":meth:`modelfit <erlab.accessors.fit.ModelFitDataArrayAccessor.__call__>` accessor to\n",
+                "fit multidimensional xarray objects. Finally, we will show how to use `iminuit\n",
+                "<https://github.com/scikit-hep/iminuit>`_ with lmfit models.\n",
                 "\n",
-                "In this tutorial, we will show how to use both libraries to fit a simple function to a\n",
-                "set of data points.\n",
-                "\n",
-                "Basic fitting with lmfit\n",
-                "------------------------"
+                "Basic fitting with ``lmfit``\n",
+                "----------------------------"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -316,19 +313,24 @@
                 }
             },
             "source": [
                 "For more information, see the `lmfit documentation\n",
                 "<https://lmfit.github.io/lmfit-py/fitting.html>`_.\n",
                 "\n",
                 "Fitting with pre-defined models\n",
-                "~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n",
+                "-------------------------------\n",
                 "\n",
                 "Creating composite models with different prefixes every time can be cumbersome, so\n",
-                "ERLabPy provides some pre-defined models in :mod:`erlab.analysis.fit.models`. One\n",
-                "example is :class:`MultiPeakModel <erlab.analysis.fit.models.MultiPeakModel>`, which is\n",
+                "ERLabPy provides some pre-defined models in :mod:`erlab.analysis.fit.models`.\n",
+                "\n",
+                "\n",
+                "Fitting multiple peaks\n",
+                "~~~~~~~~~~~~~~~~~~~~~~\n",
+                "\n",
+                "One example is :class:`MultiPeakModel <erlab.analysis.fit.models.MultiPeakModel>`, which is\n",
                 "a composite model of multiple Gaussian or Lorentzian peaks on a linear background. By\n",
                 "supplying keyword arguments, you can specify the number of peaks, their shapes, whether\n",
                 "to multiply with a Fermi-Dirac distribution, and whether to convolve the result with\n",
                 "experimental resolution."
             ]
         },
         {
@@ -384,15 +386,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "data = generate_data(bandshift=-0.2, count=5e+8).T\n",
+                "data = generate_data(bandshift=-0.2, count=5e8, seed=1).T\n",
                 "cut = data.qsel(ky=0.3)\n",
                 "cut.qplot(colorbar=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -464,16 +466,16 @@
                 },
                 "tags": [],
                 "vscode": {
                     "languageId": "raw"
                 }
             },
             "source": [
-                "Fitting xarray objects\n",
-                "----------------------\n",
+                "Fitting ``xarray`` objects\n",
+                "--------------------------\n",
                 "\n",
                 "ERLabPy provides accessors for xarray objects that allows you to fit data with lmfit\n",
                 "models: :meth:`xarray.DataArray.modelfit\n",
                 "<erlab.accessors.fit.ModelFitDataArrayAccessor.__call__>` or\n",
                 ":meth:`xarray.Dataset.modelfit <erlab.accessors.fit.ModelFitDatasetAccessor.__call__>`,\n",
                 "depending on whether you want to fit a single DataArray or multiple DataArrays in a\n",
                 "Dataset. The syntax is similar to :meth:`xarray.DataArray.curvefit` and\n",
@@ -734,19 +736,33 @@
                 "    coords=\"alpha\",\n",
                 "    model=GaussianModel() + LinearModel(),\n",
                 "    params={\n",
                 "        \"center\": xr.DataArray([-2, 0, 2], coords=[darr.beta]),\n",
                 "        \"slope\": -0.1,\n",
                 "    },\n",
                 ")\n",
-                "\n",
+                "result_ds"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Let's overlay the fitted peak positions on the data."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "result_ds.modelfit_data.qplot()\n",
-                "\n",
-                "center_fitted = result_ds.modelfit_coefficients.sel(param=\"center\")\n",
-                "plt.plot(center_fitted, center_fitted.beta, \".\")"
+                "result_center = result_ds.sel(param=\"center\")\n",
+                "plt.plot(result_center.modelfit_coefficients, result_center.beta, '.-')"
             ]
         },
         {
             "cell_type": "raw",
             "metadata": {
                 "editable": true,
                 "raw_mimetype": "text/restructuredtext",
@@ -830,23 +846,23 @@
                 "      gold_selected.parallel_fit(\n",
                 "          dim=\"alpha\",\n",
                 "          model=FermiEdgeModel(),\n",
                 "          params={\"temp\": {\"value\": 100.0, \"vary\": False}},\n",
                 "          guess=True,\n",
                 "      )\n",
                 "\n",
-                ".. note ::\n",
-                "\n",
-                "    - Note that the initial run will take a long time due to the overhead of creating\n",
-                "      parallel workers. Subsequent calls will run faster, since joblib's default backend\n",
-                "      will try to reuse the workers.\n",
-                "    \n",
-                "    - The accessor has some intrinsic overhead due to post-processing. If you need the\n",
-                "      best performance, handle the parallelization yourself with joblib and\n",
-                "      :meth:`lmfit.Model.fit <lmfit.model.Model.fit>`.\n",
+                "  .. note ::\n",
+                "  \n",
+                "      - Note that the initial run will take a long time due to the overhead of creating\n",
+                "        parallel workers. Subsequent calls will run faster, since joblib's default backend\n",
+                "        will try to reuse the workers.\n",
+                "      \n",
+                "      - The accessor has some intrinsic overhead due to post-processing. If you need the\n",
+                "        best performance, handle the parallelization yourself with joblib and\n",
+                "        :meth:`lmfit.Model.fit <lmfit.model.Model.fit>`.\n",
                 "\n",
                 "Saving and loading fits\n",
                 "~~~~~~~~~~~~~~~~~~~~~~~\n",
                 "\n",
                 "Since the resulting dataset contains no Python objects, it can be saved and loaded\n",
                 "reliably as a netCDF file using :meth:`xarray.Dataset.to_netcdf` and\n",
                 ":func:`xarray.open_dataset`, respectively. If you wish to obtain the\n",
@@ -944,16 +960,24 @@
                     "languageId": "raw"
                 }
             },
             "source": [
                 "Also check out the interactive Fermi edge fitting tool,\n",
                 ":func:`erlab.interactive.goldtool`.\n",
                 "\n",
-                "Using iminuit\n",
-                "-------------\n",
+                "Using ``iminuit``\n",
+                "-----------------\n",
+                "\n",
+                ".. note::\n",
+                "\n",
+                "    This part requires `iminuit <https://github.com/scikit-hep/iminuit>`_.\n",
+                "\n",
+                "`iminuit <https://github.com/scikit-hep/iminuit>`_ is a powerful Python interface to the\n",
+                "`Minuit C++ library <https://root.cern.ch/doc/master/Minuit2Page.html>`_ developed at\n",
+                "CERN. To learn more, see the `iminuit documentation <http://scikit-hep.org/iminuit/>`_.\n",
                 "\n",
                 "ERLabPy provides a thin wrapper around :class:`iminuit.Minuit` that allows you to use\n",
                 "lmfit models with iminuit. The example below conducts the same fit as the previous one,\n",
                 "but using iminuit."
             ]
         },
         {
@@ -1045,13 +1069,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.8"
+            "version": "3.11.9"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `erlab-2.3.0/docs/source/user-guide/imagetool.rst` & `erlab-2.3.1/docs/source/user-guide/imagetool.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/docs/source/user-guide/index.rst` & `erlab-2.3.1/docs/source/user-guide/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/docs/source/user-guide/indexing.ipynb` & `erlab-2.3.1/docs/source/user-guide/indexing.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996527777777777%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'dat = generate_data(seed=1)')], delete: [2]}}}"}*

```diff
@@ -43,15 +43,15 @@
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from erlab.io.exampledata import generate_data\n",
                 "\n",
-                "dat = generate_data()"
+                "dat = generate_data(seed=1)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "082ec477",
             "metadata": {
```

### Comparing `erlab-2.3.0/docs/source/user-guide/io.ipynb` & `erlab-2.3.1/docs/source/user-guide/io.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976744674550737%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(105, '\\n'), (106, '.. warning::\\n'), (107, '\\n'), (108, "*

 * *            "'   ERLabPy is still in development and the API may change. Some major changes "*

 * *            "regarding\\n'), (109, '   data loading and handling are planned:\\n'), (110, '\\n'), "*

 * *            "(111, '   - The `xarray datatree structure "*

 * *            "<https://github.com/pydata/xarray/issues/8572>`_\\n'), (112, '     will enable much "*

 * *            "more intuitive and powerful data handling. Once  […]*

```diff
@@ -116,14 +116,27 @@
                 "\n",
                 "Alternatively, `igorwriter <https://github.com/t-onoz/igorwriter>`_ can be used to write\n",
                 "numpy arrays to ``.ibw`` and ``.itx`` files directly.\n",
                 "\n",
                 "Loading ARPES data\n",
                 "------------------\n",
                 "\n",
+                ".. warning::\n",
+                "\n",
+                "   ERLabPy is still in development and the API may change. Some major changes regarding\n",
+                "   data loading and handling are planned:\n",
+                "\n",
+                "   - The `xarray datatree structure <https://github.com/pydata/xarray/issues/8572>`_\n",
+                "     will enable much more intuitive and powerful data handling. Once the feature gets\n",
+                "     incorporated into xarray, ERLabPy will be updated to use it.\n",
+                "\n",
+                "   - A universal translation layer between true data header attributes and\n",
+                "     human-readable representations will be implemented. This will allow for more\n",
+                "     consistent and user-friendly data handling.\n",
+                "\n",
                 "ERLabPy's data loading framework consists of various plugins, or *loaders*, each\n",
                 "designed to load data from a different beamline or laboratory. Each loader is a class\n",
                 "that has a ``load`` method which takes a file path or sequence number and returns data.\n",
                 "\n",
                 "Let's see the list of loaders available by default:"
             ]
         },
@@ -521,14 +534,15 @@
                 "        shape=(250, 1, 300),\n",
                 "        angrange={\"alpha\": (-15, 15), \"beta\": (beta, beta)},\n",
                 "        hv=hv,\n",
                 "        configuration=1,\n",
                 "        temp=temp,\n",
                 "        bandshift=bandshift,\n",
                 "        assign_attributes=False,\n",
+                "        seed=1,\n",
                 "    ).T\n",
                 "\n",
                 "    # Rename coordinates. The loader must rename them back to the original names.\n",
                 "    data = data.rename(\n",
                 "        {\n",
                 "            \"alpha\": \"ThetaX\",\n",
                 "            \"beta\": \"Polar\",\n",
@@ -1066,13 +1080,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.8"
+            "version": "3.11.9"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `erlab-2.3.0/docs/source/user-guide/plotting.ipynb` & `erlab-2.3.1/docs/source/user-guide/plotting.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910049392097264%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(2, 'dat = generate_data(bandshift=-0.2, seed=1).T')], "*

 * *            "delete: [2]}}, 33: {'source': {insert: [(0, 'dat0, dat1 = generate_data(\\n'), (1, "*

 * *            "'    shape=(250, 250, 2), Erange=(-0.3, 0.3), temp=0.0, seed=1, count=1e6\\n'), (2, "*

 * *            "').T\\n'), (4, '_, axs = eplt.plot_slices(\\n'), (9, '    label=True,\\n'), (10, "*

 * *            "')\\n'), (11, '# eplt.label_subplot_properties(axs, values=dict(Eb=[-0.3, 0.3]))')], "*

 * *            "delete: [7, […]*

```diff
@@ -81,15 +81,15 @@
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from erlab.io.exampledata import generate_data\n",
                 "\n",
-                "dat = generate_data(bandshift=-0.2).T"
+                "dat = generate_data(bandshift=-0.2, seed=1).T"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -490,22 +490,26 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "dat0, dat1 = generate_data(shape=(250, 250, 2), Erange=(-0.3, 0.3), temp=0.0).T\n",
+                "dat0, dat1 = generate_data(\n",
+                "    shape=(250, 250, 2), Erange=(-0.3, 0.3), temp=0.0, seed=1, count=1e6\n",
+                ").T\n",
                 "\n",
-                "eplt.plot_slices(\n",
+                "_, axs = eplt.plot_slices(\n",
                 "    [dat0, dat1],\n",
                 "    order=\"F\",\n",
                 "    subplot_kw={\"layout\": \"compressed\", \"sharey\": \"row\"},\n",
                 "    axis=\"scaled\",\n",
-                ")"
+                "    label=True,\n",
+                ")\n",
+                "# eplt.label_subplot_properties(axs, values=dict(Eb=[-0.3, 0.3]))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Suppose we want to visualize the sum and the normalized difference between the two. The simplest way is to plot them side by side."
@@ -513,48 +517,68 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "lightness = dat0 + dat1\n",
-                "color = (dat0 - dat1) / lightness\n",
+                "dat_sum = dat0 + dat1\n",
+                "dat_ndiff = (dat0 - dat1) / dat_sum\n",
                 "\n",
                 "eplt.plot_slices(\n",
-                "    [lightness, color],\n",
+                "    [dat_sum, dat_ndiff],\n",
                 "    order=\"F\",\n",
                 "    subplot_kw={\"layout\": \"compressed\", \"sharey\": \"row\"},\n",
                 "    cmap=[\"viridis\", \"bwr\"],\n",
                 "    axis=\"scaled\",\n",
                 ")\n",
                 "eplt.proportional_colorbar()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The difference array is noisy for small values of the sum. We can plot using a 2D colomap to visualize the relevant features better."
+                "The difference array is noisy for small values of the sum. We can plot using a 2D\n",
+                "colomap, where `dat_ndiff` is mapped to the color along the colormap and `dat_sum` is\n",
+                "mapped to the lightness of the colormap."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "eplt.plot_array_2d(dat_sum, dat_ndiff)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The color normalization for each axis can be set independently with `lnorm` and `cnorm`.\n",
+                "The appearance of the colorbar axes can be customized with the returned `Colorbar`\n",
+                "object."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "_, cb = eplt.plot_array_2d(\n",
-                "    lightness,\n",
-                "    color,\n",
+                "    dat_sum,\n",
+                "    dat_ndiff,\n",
                 "    lnorm=eplt.InversePowerNorm(0.5),\n",
                 "    cnorm=eplt.CenteredInversePowerNorm(0.7, vcenter=0.0, halfrange=1.0),\n",
                 ")\n",
-                "cb.ax.set_xticks([])\n",
-                "eplt.fancy_labels()"
+                "cb.ax.set_xticks(cb.ax.get_xlim())\n",
+                "cb.ax.set_xticklabels([\"Min\", \"Max\"])"
             ]
         },
         {
             "cell_type": "raw",
             "metadata": {
                 "editable": true,
                 "raw_mimetype": "text/restructuredtext",
@@ -633,24 +657,24 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.xarray\n",
                 "\n",
-                "cut.hvplot(x=\"kx\", y=\"eV\", cmap=\"Greys\")"
+                "cut.hvplot(x=\"kx\", y=\"eV\", cmap=\"Greys\", aspect=1.5)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "dat.hvplot(x=\"kx\", y=\"ky\", cmap=\"Greys\", widget_location=\"bottom\")"
+                "dat.hvplot(x=\"kx\", y=\"ky\", cmap=\"Greys\", aspect=\"equal\", widget_location=\"bottom\")"
             ]
         },
         {
             "cell_type": "raw",
             "metadata": {
                 "editable": true,
                 "raw_mimetype": "text/restructuredtext",
@@ -685,13 +709,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.8"
+            "version": "3.11.9"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `erlab-2.3.0/src/erlab/accessors/__init__.py` & `erlab-2.3.1/src/erlab/accessors/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/accessors/fit.py` & `erlab-2.3.1/src/erlab/accessors/fit.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,62 +14,70 @@
 
 import joblib
 import lmfit
 import numpy as np
 import tqdm.auto
 import xarray as xr
 
-from erlab.accessors.utils import _THIS_ARRAY, ERLabAccessor
+from erlab.accessors.utils import (
+    _THIS_ARRAY,
+    ERLabDataArrayAccessor,
+    ERLabDatasetAccessor,
+)
 from erlab.parallel import joblib_progress
 
 if TYPE_CHECKING:
     from xarray.core.types import Dims
 
 
 def _nested_dict_vals(d):
     for v in d.values():
         if isinstance(v, Mapping):
             yield from _nested_dict_vals(v)
         else:
             yield v
 
 
-def _broadcast_dict_values(d: Mapping[str, Any]) -> Mapping[str, xr.DataArray]:
+def _broadcast_dict_values(d: dict[str, Any]) -> dict[str, xr.DataArray]:
     to_broadcast = {}
     for k, v in d.items():
         if isinstance(v, xr.DataArray | xr.Dataset):
             to_broadcast[k] = v
         else:
             to_broadcast[k] = xr.DataArray(v)
 
-    for k, v in zip(to_broadcast.keys(), xr.broadcast(*to_broadcast.values())):
+    for k, v in zip(
+        to_broadcast.keys(), xr.broadcast(*to_broadcast.values()), strict=True
+    ):
         d[k] = v
     return d
 
 
-def _concat_along_keys(d: Mapping[str, xr.DataArray], dim_name: str) -> xr.DataArray:
+def _concat_along_keys(d: dict[str, xr.DataArray], dim_name: str) -> xr.DataArray:
     return xr.concat(d.values(), d.keys()).rename(concat_dim=dim_name)
 
 
-def _parse_params(d: Mapping[str, Any], dask: bool) -> xr.DataArray | _ParametersWraper:
+def _parse_params(
+    d: dict[str, Any] | lmfit.Parameters, dask: bool
+) -> xr.DataArray | _ParametersWraper:
     if isinstance(d, lmfit.Parameters):
         # Input to apply_ufunc cannot be a Mapping, so wrap in a class
         return _ParametersWraper(d)
 
     # Iterate over all values
     for v in _nested_dict_vals(d):
         if isinstance(v, xr.DataArray):
             # For dask arrays, auto rechunking with object dtype is unsupported, so must
             # convert to str
             return _parse_multiple_params(copy.deepcopy(d), dask)
 
     return _ParametersWraper(lmfit.create_params(**d))
 
 
-def _parse_multiple_params(d: Mapping[str, Any], as_str: bool) -> xr.DataArray:
+def _parse_multiple_params(d: dict[str, Any], as_str: bool) -> xr.DataArray:
     for k in d.keys():
         if isinstance(d[k], int | float | complex | xr.DataArray):
             d[k] = {"value": d[k]}
 
         d[k] = _concat_along_keys(_broadcast_dict_values(d[k]), "__dict_keys")
 
     da = _concat_along_keys(_broadcast_dict_values(d), "__param_names")
@@ -107,27 +115,28 @@
 
 class _ParametersWraper:
     def __init__(self, params: lmfit.Parameters):
         self.params = params
 
 
 @xr.register_dataset_accessor("modelfit")
-class ModelFitDatasetAccessor(ERLabAccessor):
+class ModelFitDatasetAccessor(ERLabDatasetAccessor):
     """`xarray.Dataset.modelfit` accessor for fitting lmfit models."""
 
     def __call__(
         self,
         coords: str | xr.DataArray | Iterable[str | xr.DataArray],
         model: lmfit.Model,
         reduce_dims: Dims = None,
         skipna: bool = True,
         params: lmfit.Parameters
-        | Mapping[str, float | dict[str, Any]]
+        | dict[str, float | dict[str, Any]]
         | xr.DataArray
         | xr.Dataset
+        | _ParametersWraper
         | None = None,
         guess: bool = False,
         errors: Literal["raise", "ignore"] = "raise",
         parallel: bool | None = None,
         parallel_kw: dict[str, Any] | None = None,
         progress: bool = False,
         output_result: bool = True,
@@ -370,18 +379,23 @@
                     modres.success = False
                     return popt, perr, pcov, stats, data, best, modres
             else:
                 mask = np.full_like(y, True)
 
             x = np.squeeze(x)
 
-            if n_coords == 1:
-                indep_var_kwargs = {model.independent_vars[0]: x}
+            if model.independent_vars is not None:
+                if n_coords == 1:
+                    indep_var_kwargs = {model.independent_vars[0]: x}
+                else:
+                    indep_var_kwargs = dict(
+                        zip(model.independent_vars[:n_coords], x, strict=True)
+                    )
             else:
-                indep_var_kwargs = dict(zip(model.independent_vars[:n_coords], x))
+                raise ValueError("Independent variables not defined in model")
 
             if guess:
                 if isinstance(model, lmfit.model.CompositeModel):
                     guessed_params = model.make_params()
                     for comp in model.components:
                         try:
                             guessed_params.update(comp.guess(y, **indep_var_kwargs))
@@ -530,35 +544,35 @@
             parallel_kw.setdefault("return_as", "generator_unordered")
             parallel_kw.setdefault("pre_dispatch", "n_jobs")
             parallel_kw.setdefault("prefer", "processes")
 
             parallel_obj = joblib.Parallel(**parallel_kw)
 
             if parallel_obj.return_generator:
-                out_dicts = tqdm.auto.tqdm(
+                out_dicts = tqdm.auto.tqdm(  # type: ignore[call-overload]
                     parallel_obj(
                         joblib.delayed(_output_wrapper)(name, da)
                         for name, da in self._obj.data_vars.items()
                     ),
                     **tqdm_kw,
                 )
             else:
                 with joblib_progress(**tqdm_kw) as _:
                     out_dicts = parallel_obj(
                         joblib.delayed(_output_wrapper)(name, da)
                         for name, da in self._obj.data_vars.items()
                     )
             result = type(self._obj)(
-                dict(itertools.chain.from_iterable(d.items() for d in out_dicts))
+                dict(itertools.chain.from_iterable(d.items() for d in out_dicts))  # type: ignore[call-overload]
             )
             del out_dicts
 
         else:
             result = type(self._obj)()
-            for name, da in tqdm.auto.tqdm(self._obj.data_vars.items(), **tqdm_kw):
+            for name, da in tqdm.auto.tqdm(self._obj.data_vars.items(), **tqdm_kw):  # type: ignore[call-overload]
                 _output_wrapper(name, da, result)
 
         result = result.assign_coords(
             {
                 "param": param_names,
                 "fit_stat": stat_names,
                 "cov_i": param_names,
@@ -568,31 +582,30 @@
         )
         result.attrs = self._obj.attrs.copy()
 
         return result
 
 
 @xr.register_dataarray_accessor("modelfit")
-class ModelFitDataArrayAccessor(ERLabAccessor):
+class ModelFitDataArrayAccessor(ERLabDataArrayAccessor):
     """`xarray.DataArray.modelfit` accessor for fitting lmfit models."""
 
     def __call__(self, *args, **kwargs) -> xr.Dataset:
         return self._obj.to_dataset(name=_THIS_ARRAY).modelfit(*args, **kwargs)
 
     __call__.__doc__ = (
-        ModelFitDatasetAccessor.__call__.__doc__.replace(
-            "Dataset.curvefit", "DataArray.curvefit"
-        )
+        str(ModelFitDatasetAccessor.__call__.__doc__)
+        .replace("Dataset.curvefit", "DataArray.curvefit")
         .replace("Dataset.polyfit", "DataArray.polyfit")
         .replace("[var]_", "")
     )
 
 
 @xr.register_dataarray_accessor("parallel_fit")
-class ParallelFitDataArrayAccessor(ERLabAccessor):
+class ParallelFitDataArrayAccessor(ERLabDataArrayAccessor):
     """
     `xarray.DataArray.parallel_fit` accessor for fitting lmfit models in parallel along
     a single dimension.
 
     """
 
     _VAR_KEYS: tuple[str, ...] = (
@@ -643,15 +656,15 @@
 
         if isinstance(kwargs.get("params", None), xr.DataArray):
             kwargs["params"] = kwargs["params"].to_dataset(dim, promote_attrs=True)
 
         fitres = ds.modelfit(set(self._obj.dims) - {dim}, model, **kwargs)
 
         drop_keys = []
-        concat_vars = {}
+        concat_vars: dict[Hashable, list[xr.DataArray]] = {}
         for k in ds.data_vars.keys():
             for var in self._VAR_KEYS:
                 key = f"{k}_{var}"
                 if key in fitres:
                     if var not in concat_vars:
                         concat_vars[var] = []
                     concat_vars[var].append(fitres[key])
```

### Comparing `erlab-2.3.0/src/erlab/accessors/kspace.py` & `erlab-2.3.1/src/erlab/accessors/kspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,37 +2,37 @@
     "MomentumAccessor",
     "OffsetView",
 ]
 
 import functools
 import time
 import warnings
-from collections.abc import Callable, ItemsView, Iterable, Iterator
-from typing import Literal
+from collections.abc import Hashable, ItemsView, Iterable, Iterator, Mapping
+from typing import Literal, cast
 
 import numpy as np
 import xarray as xr
 
-from erlab.accessors.utils import ERLabAccessor
+from erlab.accessors.utils import ERLabDataArrayAccessor
 from erlab.analysis.interpolate import interpn
 from erlab.analysis.kspace import AxesConfiguration, get_kconv_func, kz_func
 from erlab.constants import rel_kconv, rel_kzconv
-from erlab.interactive.kspace import ktool
+from erlab.interactive.kspace import KspaceTool, ktool
 
 
-def only_angles(method: Callable | None = None):
+def only_angles(method=None):
     """
     A decorator that ensures the data is in angle space before executing the decorated
     method.
 
     If the data is not in angle space (i.e., if "kx" or "ky" dimensions are present), a
     `ValueError` is raised.
     """
 
-    def wrapper(method: Callable):
+    def wrapper(method):
         @functools.wraps(method)
         def _impl(self, *args, **kwargs):
             if "kx" in self._obj.dims or "ky" in self._obj.dims:
                 raise ValueError(
                     f"`{method.__name__}` cannot be called for data in momentum space."
                 )
             return method(self, *args, **kwargs)
@@ -40,24 +40,24 @@
         return _impl
 
     if method is not None:
         return wrapper(method)
     return wrapper
 
 
-def only_momentum(method: Callable | None = None):
+def only_momentum(method=None):
     """
     A decorator that ensures the data is in momentum space before executing the
     decorated method.
 
     If the data is not in momentum space (i.e., if "kx" nor "ky" dimensions are
     present), a `ValueError` is raised.
     """
 
-    def wrapper(method: Callable):
+    def wrapper(method):
         @functools.wraps(method)
         def _impl(self, *args, **kwargs):
             if not ("kx" in self._obj.dims or "ky" in self._obj.dims):
                 raise ValueError(
                     f"`{method.__name__}` cannot be called for data in angle space."
                 )
             return method(self, *args, **kwargs)
@@ -107,18 +107,15 @@
 
     def __init__(self, xarray_obj: xr.DataArray):
         self._obj = xarray_obj
         for k in self._obj.kspace.valid_offset_keys:
             if k + "_offset" not in self._obj.attrs:
                 self[k] = 0.0
 
-    def __len__(self) -> int:
-        return len(self._obj.kspace.valid_offset_keys)
-
-    def __iter__(self) -> Iterator[str, float]:
+    def __iter__(self) -> Iterator[tuple[str, float]]:
         for key in self._obj.kspace.valid_offset_keys:
             yield key, self.__getitem__(key)
 
     def __getitem__(self, key: str) -> float:
         if key in self._obj.kspace.valid_offset_keys:
             return float(self._obj.attrs[key + "_offset"])
         else:
@@ -128,15 +125,18 @@
             )
 
     def __setitem__(self, key: str, value: float) -> None:
         if key in self._obj.kspace.valid_offset_keys:
             self._obj.attrs[key + "_offset"] = float(value)
 
     def __eq__(self, other: object) -> bool:
-        return dict(self) == dict(other)
+        if isinstance(other, Mapping):
+            return dict(self) == dict(other)
+        else:
+            return False
 
     def __repr__(self) -> str:
         return dict(self).__repr__()
 
     def _repr_html_(self) -> str:
         out = ""
         out += "<table><tbody>"
@@ -148,21 +148,21 @@
                 "</tr>"
             )
         out += "</tbody></table>"
         return out
 
     def update(
         self,
-        other: dict | Iterable[tuple[str, float]] | None = None,
+        other: dict[str, float] | Iterable[tuple[str, float]] | None = None,
         **kwargs,
     ) -> "OffsetView":
         """Updates the offset view with the provided key-value pairs."""
         if other is not None:
             for k, v in other.items() if isinstance(other, dict) else other:
-                self[k] = v
+                self[str(k)] = v
         for k, v in kwargs.items():
             self[k] = v
         return self
 
     def items(self) -> ItemsView[str, float]:
         """Returns a view of the offset view as a list of (key, value) pairs."""
         return dict(self).items()
@@ -171,15 +171,15 @@
         """Reset all angle offsets to zero."""
         for k in self._obj.kspace.valid_offset_keys:
             self[k] = 0.0
         return self
 
 
 @xr.register_dataarray_accessor("kspace")
-class MomentumAccessor(ERLabAccessor):
+class MomentumAccessor(ERLabDataArrayAccessor):
     """`xarray.DataArray.kspace` accessor for momentum conversion related utilities.
 
     This class provides convenient access to various momentum-related properties of a
     data object. It allows getting and setting properties such as configuration, inner
     potential, work function, angle resolution, slit axis, momentum axes, angle
     parameters, and offsets.
 
@@ -194,15 +194,15 @@
         details.
         """
         if "configuration" not in self._obj.attrs:
             raise ValueError(
                 "Configuration not found in data attributes! "
                 "Data attributes may have been discarded since initial import."
             )
-        return AxesConfiguration(int(self._obj.attrs.get("configuration")))
+        return AxesConfiguration(int(self._obj.attrs.get("configuration", 0)))
 
     @configuration.setter
     def configuration(self, value: AxesConfiguration | int):
         self._obj.attrs["configuration"] = int(value)
 
     @property
     def inner_potential(self) -> float:
@@ -290,30 +290,30 @@
             return 0.1
 
     @angle_resolution.setter
     def angle_resolution(self, value: float):
         self._obj.attrs["angle_resolution"] = float(value)
 
     @property
-    def slit_axis(self) -> str:
+    def slit_axis(self) -> Literal["kx", "ky"]:
         """Returns the momentum axis parallel to the slit.
 
         Returns
         -------
         str
             Returns ``'kx'`` for type 1 configurations, ``'ky'`` otherwise.
         """
         match self.configuration:
             case AxesConfiguration.Type1 | AxesConfiguration.Type1DA:
                 return "kx"
             case _:
                 return "ky"
 
     @property
-    def other_axis(self) -> str:
+    def other_axis(self) -> Literal["kx", "ky"]:
         """Returns the momentum axis perpendicular to the slit.
 
         Returns
         -------
         str
             Returns ``'ky'`` for type 1 configurations, ``'kx'`` otherwise.
         """
@@ -321,15 +321,15 @@
             case AxesConfiguration.Type1 | AxesConfiguration.Type1DA:
                 return "ky"
             case _:
                 return "kx"
 
     @property
     @only_angles
-    def momentum_axes(self) -> tuple[str, ...]:
+    def momentum_axes(self) -> tuple[Literal["kx", "ky", "kz"], ...]:
         """Returns the momentum axes of the data after conversion.
 
         Returns
         -------
         tuple
             For photon energy dependent scans, it returns the slit axis and ``'kz'``.
             For maps, it returns ``'kx'`` and ``'ky'``. Otherwise, it returns only the
@@ -525,25 +525,25 @@
 
         .. math:: \Delta k_z \sim 1/\lambda
 
         """
         kin = self.kinetic_energy.values
         c1, c2 = 641.0, 0.096
         imfp = (c1 / (kin**2) + c2 * np.sqrt(kin)) * 10
-        return np.amin(1 / imfp)
+        return float(np.amin(1 / imfp))
 
-    def _get_transformed_coords(self) -> dict[str, xr.DataArray]:
+    def _get_transformed_coords(self) -> dict[Literal["kx", "ky", "kz"], xr.DataArray]:
         kx, ky = self._forward_func(self.alpha, self.beta)
         if "hv" in kx.dims:
             kz = kz_func(self.kinetic_energy, self.inner_potential, kx, ky)
             return {"kx": kx, "ky": ky, "kz": kz}
         else:
             return {"kx": kx, "ky": ky}
 
-    def estimate_bounds(self) -> dict[str, tuple[float, float]]:
+    def estimate_bounds(self) -> dict[Literal["kx", "ky", "kz"], tuple[float, float]]:
         """
         Estimates the bounds of the data in momentum space based on the available
         parameters.
 
         Returns
         -------
         bounds : dict[str, tuple[float, float]]
@@ -601,15 +601,15 @@
         elif axis == "kz":
             dim = "hv"
             if not self.has_hv:
                 raise ValueError("No photon energy axis found.")
         else:
             raise ValueError(f"`{axis}` is not a valid momentum axis.")
 
-        if from_numpoints:
+        if from_numpoints and (lims is not None):
             return float((lims[1] - lims[0]) / len(self._obj[dim]))
         elif axis == "kz":
             return self.best_kz_resolution
         else:
             return self.best_kp_resolution
 
     def _forward_func(self, alpha, beta):
@@ -633,23 +633,32 @@
         alpha, beta = self._inverse_func(kxval, kyval, kzval)
 
         out_dict = {"alpha": alpha, "beta": beta}
 
         if self.has_eV:
             out_dict["eV"] = self.binding_energy
 
-        if kz is not None:
+        if kzval is not None:
             out_dict["hv"] = (
                 rel_kzconv * (kxval**2 + kyval**2 + kzval**2)
                 - self.inner_potential
                 + self.work_function
                 - self.binding_energy
             )
 
-        return dict(zip(out_dict.keys(), xr.broadcast(*out_dict.values())))
+        return cast(
+            dict[str, xr.DataArray],
+            dict(
+                zip(
+                    cast(list[str], out_dict.keys()),
+                    xr.broadcast(*out_dict.values()),
+                    strict=True,
+                )
+            ),
+        )
 
     @only_angles
     def convert_coords(self) -> xr.DataArray:
         """Convert the coordinates to momentum space.
 
         Assigns new exact momentum coordinates to the data. This is useful when you want
         to work with momentum coordinates but don't want to interpolate the data.
@@ -658,15 +667,15 @@
         -------
         xarray.DataArray
             The DataArray with transformed coordinates.
         """
         return self._obj.assign_coords(self._get_transformed_coords())
 
     @only_angles
-    def _get_coord_for_conversion(self, name: str) -> xr.DataArray:
+    def _get_coord_for_conversion(self, name: Hashable) -> xr.DataArray:
         """
         Get the coordinte array for given dimension name. This just ensures that the
         energy coordinates are given as binding energy.
         """
         if name == "eV":
             return self.binding_energy
         else:
@@ -775,14 +784,20 @@
                 )
             else:
                 # Take the mean for axes that will not appear in converted data
                 if not silent and lims[1] - lims[0] > 0.001:
                     print(f"Data spans {lims[1] - lims[0]:.3f} Å⁻¹ of {k}")
                 momentum_coords[k] = np.array([(lims[0] + lims[1]) / 2])
 
+        for k, v in coords.items():
+            if k in self.momentum_axes:
+                momentum_coords[k] = v
+            else:
+                raise ValueError(f"Dimension `{k}` is not a momentum axis")
+
         if not silent:
             print("Calculating destination coordinates")
 
         target_dict: dict[str, xr.DataArray] = self._inverse_broadcast(
             momentum_coords.get("kx"),
             momentum_coords.get("ky"),
             momentum_coords.get("kz", None),
@@ -799,21 +814,21 @@
 
         # Now, coords_for_transform contains a subset of kx, ky, kz, eV, and hv coords,
         # depending on the dimensions of the input data.
 
         dim_mapping: dict[str, str] = {}
         for d in coords_for_transform.dims:
             if d == self.slit_axis:
-                dim_mapping["alpha"] = d
+                dim_mapping["alpha"] = str(d)
             elif d == self.other_axis:
-                dim_mapping["beta"] = d
+                dim_mapping["beta"] = str(d)
             elif d == "kz":
-                dim_mapping["hv"] = d
+                dim_mapping["hv"] = str(d)
             else:
-                dim_mapping[d] = d
+                dim_mapping[str(d)] = str(d)
 
         # Delete keys not in the input data, e.g. "beta" for cuts
         for k in list(dim_mapping.keys()):
             if k not in self._obj.dims:
                 del dim_mapping[k]
 
         input_dims: tuple[str, ...] = tuple(dim_mapping.keys())
@@ -824,16 +839,18 @@
             t_start = time.perf_counter()
 
         def _wrap_interpn(arr, *args):
             points, xi = args[: arr.ndim], args[arr.ndim :]
             return interpn(points, arr, xi, bounds_error=False).squeeze()
 
         input_core_dims = [input_dims]
-        input_core_dims.extend([[d] for d in input_dims])
-        input_core_dims.extend([target_dict[d].dims for d in input_dims])
+        input_core_dims.extend([(d,) for d in input_dims])
+        input_core_dims.extend(
+            [cast(tuple[str, ...], target_dict[d].dims) for d in input_dims]
+        )
 
         out = xr.apply_ufunc(
             _wrap_interpn,
             self._data_ensure_binding(),
             *tuple(self._get_coord_for_conversion(dim) for dim in input_dims),
             *tuple(target_dict[dim] for dim in input_dims),
             vectorize=True,
@@ -849,15 +866,15 @@
         ).assign_coords({k: v.squeeze() for k, v in coords_for_transform.items()})
 
         if not silent:
             print(f"Interpolated in {time.perf_counter() - t_start:.3f} s")
 
         return out
 
-    def interactive(self, **kwargs) -> ktool:
+    def interactive(self, **kwargs) -> KspaceTool:
         """Open the interactive momentum space conversion tool."""
         if self._obj.ndim < 3:
             raise ValueError("Interactive tool requires three-dimensional data.")
         return ktool(self._obj, **kwargs)
 
     @only_momentum
     def hv_to_kz(self, hv: float) -> xr.DataArray:
```

### Comparing `erlab-2.3.0/src/erlab/accessors/utils.py` & `erlab-2.3.1/src/erlab/accessors/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,18 +17,25 @@
 T = TypeVar("T")
 
 # Used as the key corresponding to a DataArray's variable when converting
 # arbitrary DataArray objects to datasets, from xarray.core.dataarray
 _THIS_ARRAY: str = "<this-array>"
 
 
-class ERLabAccessor:
+class ERLabDataArrayAccessor:
     """Base class for accessors."""
 
-    def __init__(self, xarray_obj: xr.DataArray | xr.Dataset):
+    def __init__(self, xarray_obj: xr.DataArray):
+        self._obj = xarray_obj
+
+
+class ERLabDatasetAccessor:
+    """Base class for accessors."""
+
+    def __init__(self, xarray_obj: xr.Dataset):
         self._obj = xarray_obj
 
 
 def is_dict_like(value: Any) -> TypeGuard[Mapping[Any, Any]]:
     return hasattr(value, "keys") and hasattr(value, "__getitem__")
 
 
@@ -48,15 +55,15 @@
         raise ValueError(
             f"cannot specify both keyword and positional arguments to .{func_name}"
         )
     return pos_kwargs
 
 
 @xr.register_dataarray_accessor("qplot")
-class PlotAccessor(ERLabAccessor):
+class PlotAccessor(ERLabDataArrayAccessor):
     """`xarray.DataArray.qplot` accessor for plotting data."""
 
     def __call__(self, *args, **kwargs):
         """
         Plot the data. If a 2D data array is provided, it is plotted using
         :func:`plot_array <erlab.plotting.general.plot_array>`. Otherwise, it is
         equivalent to calling :meth:`xarray.DataArray.plot`.
@@ -79,34 +86,34 @@
 
             out = self._obj.plot(*args, **kwargs)
             eplt.fancy_labels(ax)
             return out
 
 
 @xr.register_dataarray_accessor("qshow")
-class ImageToolAccessor(ERLabAccessor):
+class ImageToolAccessor(ERLabDataArrayAccessor):
     """`xarray.DataArray.qshow` accessor for interactive visualization."""
 
-    def __call__(self, *args, **kwargs) -> ImageTool:
+    def __call__(self, *args, **kwargs) -> ImageTool | list[ImageTool] | None:
         if len(self._obj.dims) >= 2:
             return itool(self._obj, *args, **kwargs)
         else:
             raise ValueError("Data must have at leasst two dimensions.")
 
 
 @xr.register_dataarray_accessor("qsel")
-class SelectionAccessor(ERLabAccessor):
+class SelectionAccessor(ERLabDataArrayAccessor):
     """
     `xarray.DataArray.qsel` accessor for conveniently selecting and averaging
     data.
     """
 
     def __call__(
         self,
-        indexers: dict[str, float | slice] | None = None,
+        indexers: Mapping[Hashable, float | slice] | None = None,
         *,
         verbose: bool = False,
         **indexers_kwargs,
     ):
         """Select and average data along specified dimensions.
 
         Parameters
@@ -147,51 +154,64 @@
         ValueError
             If a specified dimension is not present in the data.
         """
 
         indexers = either_dict_or_kwargs(indexers, indexers_kwargs, "qsel")
 
         # Bin widths for each dimension, zero if width not specified
-        bin_widths: dict[str, float] = {}
+        bin_widths: dict[Hashable, float] = {}
 
         for dim in indexers:
-            if not dim.endswith("_width"):
-                bin_widths[dim] = indexers.get(f"{dim}_width", 0.0)
+            if not str(dim).endswith("_width"):
+                width = indexers.get(f"{dim}_width", 0.0)
+                if isinstance(width, slice):
+                    raise ValueError(
+                        f"Slice not allowed for width of dimension `{dim}`"
+                    )
+                else:
+                    bin_widths[dim] = float(width)
                 if dim not in self._obj.dims:
                     raise ValueError(f"Dimension `{dim}` not found in data.")
 
-        scalars: dict[str, float] = {}
-        slices: dict[str, slice] = {}
-        avg_dims: list[str] = []
+        scalars: dict[Hashable, float] = {}
+        slices: dict[Hashable, slice] = {}
+        avg_dims: list[Hashable] = []
 
         for dim, width in bin_widths.items():
+            value = indexers[dim]
+
             if width == 0.0:
-                if isinstance(indexers[dim], slice):
-                    slices[dim] = indexers[dim]
+                if isinstance(value, slice):
+                    slices[dim] = value
                 else:
-                    scalars[dim] = float(indexers[dim])
+                    scalars[dim] = float(value)
             else:
-                slices[dim] = slice(
-                    indexers[dim] - width / 2, indexers[dim] + width / 2
-                )
+                if isinstance(value, slice):
+                    raise ValueError(
+                        f"Slice not allowed for value of dimension `{dim}` "
+                        "with width specified"
+                    )
+                slices[dim] = slice(value - width / 2, value + width / 2)
                 avg_dims.append(dim)
 
         if len(scalars) >= 1:
             for k, v in scalars.items():
                 if v < self._obj[k].min() or v > self._obj[k].max():
                     warnings.warn(
                         f"Selected value {v} for `{k}` is outside coordinate bounds",
                         stacklevel=2,
                     )
-            out = self._obj.sel(**scalars, method="nearest")
+            out = self._obj.sel(
+                {str(k): v for k, v in scalars.items()}, method="nearest"
+            )
         else:
             out = self._obj
 
         if len(slices) >= 1:
-            out = out.sel(**slices)
+            out = out.sel(slices)
 
             lost_coords = {k: out[k].mean() for k in avg_dims}
             out = out.mean(dim=avg_dims, keep_attrs=True)
             out = out.assign_coords(lost_coords)
 
         if verbose:
             print(
```

### Comparing `erlab-2.3.0/src/erlab/analysis/__init__.py` & `erlab-2.3.1/src/erlab/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/analysis/correlation.py` & `erlab-2.3.1/src/erlab/analysis/correlation.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     acf = nanacf(out.values, mode=mode, method=method)
     coords = [out[d].values for d in out.dims]
     steps = [c[1] - c[0] for c in coords]
     out = xr.DataArray(
         acf,
         {
             d: autocorrelation_lags(n, mode) * s
-            for s, n, d in zip(steps, arr.shape, out.dims)
+            for s, n, d in zip(steps, arr.shape, out.dims, strict=True)
         },
         attrs=out.attrs,
     )
     if all(i in out.dims for i in ["kx", "ky"]):
         out = out.rename({"kx": "qx", "ky": "qy"})
     return out
 
@@ -110,22 +110,22 @@
             )
 
         stack_sizes = {d: len(arr[d]) for d in stack_dims}
         stack_iter = tuple(range(s) for s in stack_sizes.values())
 
         out_list = joblib.Parallel(n_jobs=-1, pre_dispatch="3 * n_jobs")(
             joblib.delayed(nanacf)(
-                np.squeeze(arr.isel(dict(zip(stack_dims, vals))).values),
+                np.squeeze(arr.isel(dict(zip(stack_dims, vals, strict=True))).values),
                 mode,
                 method,
             )
             for vals in itertools.product(*stack_iter)
         )
         acf_dims = tuple(filter(lambda d: d not in stack_dims, arr.dims))
-        acf_sizes = dict(zip(acf_dims, out_list[0].shape))
+        acf_sizes = dict(zip(acf_dims, out_list[0].shape, strict=True))
         acf_steps = tuple(arr[d].values[1] - arr[d].values[0] for d in acf_dims)
 
         out_sizes = stack_sizes | acf_sizes
 
         if mode == "same":
             out = arr.copy(deep=True)
         else:
@@ -133,20 +133,22 @@
                 np.empty(tuple(out_sizes[d] for d in arr.dims)),
                 dims=arr.dims,
                 attrs=arr.attrs,
             )
             out = out.assign_coords({d: arr[d] for d in stack_dims})
 
         for i, vals in enumerate(itertools.product(*stack_iter)):
-            out.loc[{s: arr[s][v] for s, v in zip(stack_dims, vals)}] = out_list[i]
+            out.loc[{s: arr[s][v] for s, v in zip(stack_dims, vals, strict=True)}] = (
+                out_list[i]
+            )
 
         out = out.assign_coords(
             {
                 d: autocorrelation_lags(len(arr[d]), mode) * s
-                for s, d in zip(acf_steps, acf_dims)
+                for s, d in zip(acf_steps, acf_dims, strict=True)
             }
         )
         if all(i in out.dims for i in ["kx", "ky"]):
             out = out.rename({"kx": "qx", "ky": "qy"})
     return out
```

### Comparing `erlab-2.3.0/src/erlab/analysis/fit/functions/__init__.py` & `erlab-2.3.1/src/erlab/analysis/fit/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/analysis/fit/functions/dynamic.py` & `erlab-2.3.1/src/erlab/analysis/fit/functions/dynamic.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,16 @@
     "FermiEdge2dFunction",
     "MultiPeakFunction",
     "PolynomialFunction",
     "get_args_kwargs",
 ]
 import functools
 import inspect
-from collections.abc import Callable
+from collections.abc import Callable, Sequence
+from typing import Any, TypedDict, no_type_check, ClassVar
 
 import numpy as np
 import numpy.typing as npt
 import xarray as xr
 
 from erlab.analysis.fit.functions.general import (
     TINY,
@@ -26,15 +27,20 @@
     fermi_dirac,
     gaussian_wh,
     lorentzian_wh,
 )
 from erlab.constants import kb_eV
 
 
-def get_args_kwargs(func) -> tuple[list[str], dict[str, object]]:
+class PeakArgs(TypedDict):
+    args: list[str]
+    kwargs: dict[str, Any]
+
+
+def get_args_kwargs(func: Callable) -> tuple[list[str], dict[str, Any]]:
     """Get all argument names and default values from a function signature.
 
     Parameters
     ----------
     func
         The function to inspect.
 
@@ -68,34 +74,40 @@
             args.append(fnam)
         else:
             args_default[fnam] = fpar.default
 
     return args, args_default
 
 
+def get_args_kwargs_dict(func: Callable) -> PeakArgs:
+    args, kwargs = get_args_kwargs(func)
+    return {"args": args, "kwargs": kwargs}
+
+
 class DynamicFunction:
     """Base class for dynamic functions.
 
     Dynamic functions exploits the way `lmfit` handles asteval functions in
     `lmfit.Model._parse_params`.
     """
 
     @property
     def __name__(self) -> str:
-        return self.__class__.__name__
+        return str(self.__class__.__name__)
 
     @property
     def argnames(self) -> list[str]:
         return ["x"]
 
     @property
     def kwargs(self) -> dict[str, int | float]:
         return {}
 
-    def __call__(self, x: npt.NDArray[np.float64], **params) -> npt.NDArray[np.float64]:
+    @no_type_check
+    def __call__(self, **kwargs):
         raise NotImplementedError("Must be overloaded in child classes")
 
 
 class PolynomialFunction(DynamicFunction):
     """A callable class for a arbitrary degree polynomial.
 
     Parameters
@@ -145,15 +157,15 @@
     convolve
         Flag indicating whether the model should be convolved with a gaussian kernel. If
         `True`, adds a `resolution` parameter to the model, corresponding to the FWHM of
         the gaussian kernel.
 
     """
 
-    PEAK_SHAPES: dict[Callable, list[str]] = {
+    PEAK_SHAPES: ClassVar[dict[Callable, list[str]]] = {
         lorentzian_wh: ["lorentzian", "lor", "l"],
         gaussian_wh: ["gaussian", "gauss", "g"],
     }
 
     DEFAULT_PEAK: str = "lorentzian"
 
     def __init__(
@@ -176,41 +188,41 @@
         if len(peak_shapes) == 1:
             peak_shapes = peak_shapes * self.npeaks
         elif len(peak_shapes) != self.npeaks:
             raise ValueError("Number of peaks does not match given peak shapes")
 
         self._peak_shapes = peak_shapes
 
-        self._peak_funcs = [None] * self.npeaks
-        for i, name in enumerate(self._peak_shapes):
+        self._peak_funcs: list[Callable] = []
+        for name in self._peak_shapes:
             for fcn, aliases in self.PEAK_SHAPES.items():
                 if name in aliases:
-                    self._peak_funcs[i] = fcn
+                    self._peak_funcs.append(fcn)
 
-        if None in self._peak_funcs:
+        if len(self._peak_funcs) != self.npeaks:
             raise ValueError("Invalid peak name")
 
     @functools.cached_property
-    def peak_all_args(self) -> dict[Callable, dict[str, list | dict]]:
-        res = {}
+    def peak_all_args(self) -> dict[Callable, PeakArgs]:
+        res: dict[Callable, PeakArgs] = {}
         for func in self.PEAK_SHAPES:
-            res[func] = dict(zip(("args", "kwargs"), get_args_kwargs(func)))
+            res[func] = get_args_kwargs_dict(func)
         return res
 
     @functools.cached_property
     def peak_argnames(self) -> dict[Callable, list[str]]:
         res = {}
         for func in self.PEAK_SHAPES:
             res[func] = self.peak_all_args[func]["args"][1:] + list(
-                self.peak_all_args[func]["kwargs"].keys()
+                dict(self.peak_all_args[func]["kwargs"]).keys()
             )
         return res
 
     @property
-    def peak_funcs(self) -> list[Callable]:
+    def peak_funcs(self) -> Sequence[Callable]:
         return self._peak_funcs
 
     @property
     def argnames(self) -> list[str]:
         args = ["x"]
         for i, func in enumerate(self.peak_funcs):
             args += [f"p{i}_{arg}" for arg in self.peak_all_args[func]["args"][1:]]
@@ -228,15 +240,15 @@
                 ("temp", 30),  # temperature
                 ("offset", 0),
             ]
         if self.convolve:
             kws += [("resolution", 0.02)]
 
         for i, func in enumerate(self.peak_funcs):
-            for arg, val in self.peak_all_args[func]["kwargs"].items():
+            for arg, val in dict(self.peak_all_args[func]["kwargs"]).items():
                 kws.append((f"p{i}_{arg}", val))
         return kws
 
     def sigma_expr(self, index: int, prefix: str) -> str | None:
         if self._peak_funcs[index] == gaussian_wh:
             return f"{prefix}p{index}_width / (2 * sqrt(2 * log(2)))"
         elif self._peak_funcs[index] == lorentzian_wh:
@@ -248,30 +260,28 @@
         if self._peak_funcs[index] == gaussian_wh:
             return f"{prefix}p{index}_height * {prefix}p{index}_sigma / sqrt(2 * pi)"
         elif self._peak_funcs[index] == lorentzian_wh:
             return f"{prefix}p{index}_height * {prefix}p{index}_sigma * pi"
         else:
             return None
 
-    def eval_peak(self, index: int, x: npt.NDArray[np.float64], **params: dict):
+    def eval_peak(self, index: int, x, **params):
         return self.peak_funcs[index](
             x,
             **{
                 k[3:]: v
                 for k, v in params.items()
                 if k.startswith(f"p{index}") and not k.endswith(("sigma", "amplitude"))
             },
         )
 
-    def eval_bkg(self, x: npt.NDArray[np.float64], **params: dict):
+    def eval_bkg(self, x, **params):
         return params["lin_bkg"] * x + params["const_bkg"]
 
-    def pre_call(
-        self, x: npt.NDArray[np.float64], **params: dict
-    ) -> npt.NDArray[np.float64]:
+    def pre_call(self, x, **params):
         x = np.asarray(x).copy()
         y = np.zeros_like(x)
 
         for i, func in enumerate(self.peak_funcs):
             y += func(
                 x, **{arg: params[f"p{i}_{arg}"] for arg in self.peak_argnames[func]}
             )
@@ -280,17 +290,15 @@
 
         if self.fd:
             y *= fermi_dirac(x, center=params["efermi"], temp=params["temp"])
             y += params["offset"]
 
         return y
 
-    def __call__(
-        self, x: npt.NDArray[np.float64], **params: dict
-    ) -> npt.NDArray[np.float64]:
+    def __call__(self, x, **params):
         if isinstance(x, xr.DataArray):
             return x * 0.0 + self.__call__(x.values, **params)
 
         if self.convolve:
             if "resolution" not in params:
                 raise TypeError(
                     "Missing parameter `resolution` required for convolution"
@@ -315,29 +323,34 @@
             ("temp", 30.0),
             ("lin_bkg", 0.0),
             ("const_bkg", 1.0),
             ("offset", 0.0),
             ("resolution", 0.02),
         ]
 
-    def pre_call(self, eV, alpha, **params: dict):
+    def pre_call(self, eV, alpha, **params):
         center = self.poly(
             np.asarray(alpha),
             *[params.pop(f"c{i}") for i in range(self.poly.degree + 1)],
         )
         return (params["const_bkg"] - params["offset"] + params["lin_bkg"] * eV) / (
             1 + np.exp((1.0 * eV - center) / max(TINY, params["temp"] * kb_eV))
         ) + params["offset"]
 
-    def __call__(self, eV, alpha, **params: dict):
+    def __call__(
+        self,
+        eV: npt.NDArray[np.float64] | xr.DataArray,
+        alpha: npt.NDArray[np.float64] | xr.DataArray,
+        **params,
+    ):
         if isinstance(eV, xr.DataArray) and isinstance(alpha, xr.DataArray):
             out = eV * alpha * 0.0
             return out + self.__call__(eV.values, alpha.values, **params).reshape(
                 out.shape
             )
-        if isinstance("eV", xr.DataArray):
+        if isinstance(eV, xr.DataArray):
             eV = eV.values
-        if isinstance("alpha", xr.DataArray):
+        if isinstance(alpha, xr.DataArray):
             alpha = alpha.values
         if "resolution" not in params:
             raise TypeError("Missing parameter `resolution` required for convolution")
         return do_convolve_2d(eV, alpha, self.pre_call, **params).ravel()
```

### Comparing `erlab-2.3.0/src/erlab/analysis/fit/functions/general.py` & `erlab-2.3.1/src/erlab/analysis/fit/functions/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,38 +128,39 @@
         np.asarray(x, dtype=np.float64), float(resolution), pad=int(pad)
     )
     return np.convolve(func(xn, **kwargs), g, mode="valid")
 
 
 def do_convolve_2d(
     x: npt.NDArray[np.float64],
-    y: npt.NDArray[np.float64],
+    y: npt.NDArray[np.float64] | float,
     func: Callable,
     resolution: float,
     pad: int = 5,
     **kwargs,
 ) -> npt.NDArray[np.float64]:
     idx_x = None
+
+    if not np.iterable(y):
+        y = np.asarray([y])
+
     try:
         # check if x is a meshgrid
         shape_x, idx_x, x = _infer_meshgrid_shape(np.ascontiguousarray(x))
         shape_y, _, y = _infer_meshgrid_shape(np.ascontiguousarray(y))
     except ValueError:
         pass
     else:
         if shape_x != shape_y:
             raise ValueError("x and y do not have matching shape")
 
     xn, g = _gen_kernel(
         np.asarray(np.squeeze(x), dtype=np.float64), resolution, pad=pad
     )
 
-    if not np.iterable(y):
-        y = [y]
-
     convolved = np.vstack(
         [
             np.convolve(func(xn, yi, **kwargs), g, mode="valid")
             for yi in np.asarray(y).flat
         ]
     )
```

### Comparing `erlab-2.3.0/src/erlab/analysis/fit/minuit.py` & `erlab-2.3.1/src/erlab/analysis/fit/minuit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from __future__ import annotations
 
+import importlib
 from collections.abc import Iterable, Sequence
 from typing import TYPE_CHECKING
 
+if not importlib.util.find_spec("iminuit"):
+    raise ImportError("`erlab.analysis.fit.minuit` requires `iminuit` to be installed.")
+
 import iminuit.cost
 import iminuit.util
 import matplotlib.pyplot as plt
 import numpy as np
 import numpy.typing as npt
+import xarray
 from iminuit.util import _detect_log_spacing, _smart_sampling
 
 import erlab.plotting.general
 
 if TYPE_CHECKING:
     import lmfit
 
@@ -23,15 +28,15 @@
         self, args: npt.ArrayLike, model_points: int | Sequence[float] = 0
     ) -> tuple[
         tuple[npt.NDArray, npt.NDArray, npt.NDArray], tuple[npt.NDArray, npt.NDArray]
     ]:
         if self._ndim > 1:
             raise ValueError("visualize is not implemented for multi-dimensional data")
 
-        plt.grid(visible="both")
+        plt.grid(visible=True, axis="both")
         x, y, ye = self._masked.T
         plt.errorbar(
             x, y, ye, fmt="o", lw=0.75, ms=3, mfc="w", zorder=2, c="0.4", capsize=0
         )
         if isinstance(model_points, Iterable):
             xm = np.array(model_points)
             ym = self.model(xm, *args)
@@ -39,15 +44,18 @@
             if _detect_log_spacing(x):
                 xm = np.geomspace(x[0], x[-1], model_points)
             else:
                 xm = np.linspace(x[0], x[-1], model_points)
             ym = self.model(xm, *args)
         else:
             xm, ym = _smart_sampling(
-                lambda x: self.model(x, *args), x[0], x[-1], start=len(x)
+                lambda x: self.model(x, *args),
+                x[0],
+                x[-1],
+                start=len(x),
             )
         plt.plot(xm, ym, "r-", lw=1, zorder=3)
         return (x, y, ye), (xm, ym)
 
     visualize.__doc__ = iminuit.cost.LeastSquares.visualize.__doc__
 
 
@@ -96,25 +104,27 @@
 
     """
 
     @classmethod
     def from_lmfit(
         cls,
         model: lmfit.Model,
-        data: npt.ArrayLike,
-        ivars: npt.ArrayLike | Sequence[npt.ArrayLike],
-        yerr: float | npt.ArrayLike | None = None,
+        data: npt.NDArray | xarray.DataArray,
+        ivars: npt.NDArray
+        | xarray.DataArray
+        | Sequence[npt.NDArray | xarray.DataArray],
+        yerr: float | npt.NDArray | None = None,
         return_cost: bool = False,
         **kwargs,
     ) -> Minuit | tuple[LeastSq, Minuit]:
         if len(model.independent_vars) == 1:
-            if len(ivars) != 1:
+            if isinstance(ivars, np.ndarray | xarray.DataArray):
                 ivars = [ivars]
 
-        x = [np.asarray(a) for a in ivars]
+        x: npt.NDArray | list[npt.NDArray] = [np.asarray(a) for a in ivars]
 
         if len(x) != len(model.independent_vars):
             raise ValueError("Number of independent variables does not match model.")
 
         if len(x) == 1:
             x = x[0]
 
@@ -169,20 +179,24 @@
             values[k] = val
             limits[k] = (float(par.min), float(par.max))
 
         # Convert to kwargs
         if len(model.independent_vars) == 1:
 
             def _temp_func(x, *fargs):
-                return model.func(x, **dict(zip(model._param_root_names, fargs)))
+                return model.func(
+                    x, **dict(zip(model._param_root_names, fargs, strict=True))
+                )
 
         else:
 
             def _temp_func(x, *fargs):
-                return model.func(*x, **dict(zip(model._param_root_names, fargs)))
+                return model.func(
+                    *x, **dict(zip(model._param_root_names, fargs, strict=True))
+                )
 
         c = LeastSq(x, data, yerr, _temp_func)
         m = cls(c, name=param_names, **values)
 
         for n in param_names:
             m.fixed[n] = n in fixed_params
             m.limits[n] = limits[n]
```

### Comparing `erlab-2.3.0/src/erlab/analysis/fit/models.py` & `erlab-2.3.1/src/erlab/analysis/fit/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,16 +111,19 @@
     return n0, m0, n1, m1
 
 
 class FermiEdgeModel(lmfit.Model):
     """
     Fermi-dirac function with linear background above and below the fermi level,
     convolved with a gaussian kernel.
+
     """
 
+    __doc__ = __doc__ + lmfit.models.COMMON_INIT_DOC
+
     @staticmethod
     def LinearBroadFermiDirac(
         x,
         center=0.0,
         temp=30.0,
         resolution=0.02,
         back0=0.0,
@@ -161,15 +164,14 @@
         pars[f"{self.prefix}dos0"].set(value=dos0)
         pars[f"{self.prefix}dos1"].set(value=dos1)
         pars[f"{self.prefix}temp"].set(value=temp)
         pars[f"{self.prefix}resolution"].set(value=0.02)
 
         return lmfit.models.update_param_vals(pars, self.prefix, **kwargs)
 
-    __init__.doc = lmfit.models.COMMON_INIT_DOC
     guess.__doc__ = COMMON_GUESS_DOC
 
 
 class StepEdgeModel(lmfit.Model):
     def __init__(self, independent_vars=("x",), prefix="", missing="raise", **kwargs):
         kwargs.update(
             {
@@ -195,15 +197,15 @@
         pars[f"{self.prefix}back1"].set(value=back1)
         pars[f"{self.prefix}dos0"].set(value=dos0)
         pars[f"{self.prefix}dos1"].set(value=dos1)
         pars[f"{self.prefix}sigma"].set(value=0.02)
 
         return lmfit.models.update_param_vals(pars, self.prefix, **kwargs)
 
-    __init__.doc = lmfit.models.COMMON_INIT_DOC
+    __doc__ = lmfit.models.COMMON_INIT_DOC
     guess.__doc__ = COMMON_GUESS_DOC
 
 
 class PolynomialModel(lmfit.Model):
     def __init__(self, degree=9, **kwargs):
         kwargs.setdefault("name", f"Poly{degree}")
         super().__init__(PolynomialFunction(degree), **kwargs)
@@ -216,15 +218,15 @@
                 pars[f"{self.prefix}c{i}"].set(value=0.0)
         else:
             out = np.polyfit(x, data, self.func.degree)
             for i, coef in enumerate(out[::-1]):
                 pars[f"{self.prefix}c{i}"].set(value=coef)
         return lmfit.models.update_param_vals(pars, self.prefix, **kwargs)
 
-    __init__.doc = lmfit.models.COMMON_INIT_DOC
+    __doc__ = lmfit.models.COMMON_INIT_DOC
     guess.__doc__ = COMMON_GUESS_DOC
 
 
 class MultiPeakModel(lmfit.Model):
     """Model for fitting multiple Gaussian or Lorentzian peaks.
 
     Most input parameters are passed to the :class:`MultiPeakFunction
@@ -322,15 +324,15 @@
         \alpha^i}{k_B T}\right)\right]^{-1} + c\right\}\otimes g(\sigma)
 
     for a :math:`n` th degree polynomial edge with coefficients :math:`c_i` with a
     linear density of states described by :math:`a\omega+b` with a constant background
     :math:`c` convolved with a gaussian, where :math:`\omega` is the binding energy and
     :math:`\alpha` is the detector angle.
 
-    """
+    """ + lmfit.models.COMMON_INIT_DOC.replace("['x']", "['eV', 'alpha']")
 
     def __init__(
         self,
         degree: int = 2,
         independent_vars=("eV", "alpha"),
         **kwargs,
     ):
@@ -377,29 +379,28 @@
 
     def fit(self, data, *args, **kwargs):
         if isinstance(data, xr.DataArray):
             data = data.transpose("eV", "alpha").values
         # Ensure flat fit
         return super().fit(data.ravel(), *args, **kwargs)
 
-    __init__.__doc__ = lmfit.models.COMMON_INIT_DOC.replace("['x']", "['eV', 'alpha']")
     guess.__doc__ = COMMON_GUESS_DOC.replace("x : ", "eV, alpha : ")
 
 
 class BCSGapModel(lmfit.Model):
     def __init__(self, **kwargs):
         super().__init__(bcs_gap, **kwargs)
         self.set_param_hint("a", min=0.0)
         self.set_param_hint("tc", min=0.0)
 
     __doc__ = bcs_gap.__doc__
-    __init__.doc = lmfit.models.COMMON_INIT_DOC
+    __init__.__doc__ = lmfit.models.COMMON_INIT_DOC
 
 
 class DynesModel(lmfit.Model):
     def __init__(self, **kwargs):
         super().__init__(dynes, **kwargs)
         self.set_param_hint("gamma", min=0.0)
         self.set_param_hint("delta", min=0.0)
 
     __doc__ = dynes.__doc__
-    __init__.doc = lmfit.models.COMMON_INIT_DOC
+    __init__.__doc__ = lmfit.models.COMMON_INIT_DOC
```

### Comparing `erlab-2.3.0/src/erlab/analysis/fit/spline.py` & `erlab-2.3.1/src/erlab/analysis/fit/spline.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import xarray as xr
 
 try:
     import csaps
 except ImportError as e:
     raise ImportError(
-        "The `csaps` package is required for this module. "
-        "Please install it using `pip install csaps`."
+        "`erlab.analysis.fit.spline` requires `csaps` to be installed."
     ) from e
 
 
 def xcsaps(arr: xr.DataArray, **kwargs) -> tuple[xr.DataArray, csaps.ISmoothingSpline]:
     """`xarray` compatible `csaps.csaps`.
 
     Parameters
```

### Comparing `erlab-2.3.0/src/erlab/analysis/gold.py` & `erlab-2.3.1/src/erlab/analysis/gold.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,18 @@
     "poly",
     "poly_from_edge",
     "resolution",
     "resolution_roi",
     "spline_from_edge",
 ]
 
-from collections.abc import Callable, Sequence
+from collections.abc import Callable
 
 import joblib
+import lmfit
 import lmfit.model
 import matplotlib
 import matplotlib.figure
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 import numpy as np
 import numpy.typing as npt
@@ -138,15 +139,15 @@
         axes[0].set_title("Data")
         axes[1].set_title("Edge Corrected")
 
     return corrected
 
 
 def edge(
-    gold: xr.DataArray | xr.Dataset,
+    gold: xr.DataArray,
     angle_range: tuple[float, float],
     eV_range: tuple[float, float],
     bin_size: tuple[int, int] = (1, 1),
     temp: float | None = None,
     vary_temp: bool = False,
     fast: bool = False,
     method: str = "leastsq",
@@ -154,15 +155,15 @@
     normalize: bool = True,
     fixed_center: float | None = None,
     progress: bool = True,
     parallel_kw: dict | None = None,
     parallel_obj: joblib.Parallel | None = None,
     return_full: bool = False,
     **kwargs,
-) -> tuple[npt.NDArray, npt.NDArray] | xr.Dataset:
+) -> tuple[xr.DataArray, xr.DataArray] | list[lmfit.model.ModelResult]:
     """
     Fit a Fermi edge to the given gold data.
 
     Parameters
     ----------
     gold
         The gold data to fit the edge model to.
@@ -207,17 +208,18 @@
         The fitted center values and their standard errors, returned when `return_full`
         is `False`.
     fitresults
         A dataset containing the full fit results, returned when `return_full` is
         `True`.
 
     """
+
     if fast:
         params = lmfit.create_params()
-        model_cls = StepEdgeModel
+        model_cls: lmfit.Model = StepEdgeModel
     else:
         if temp is None:
             temp = gold.attrs["temp_sample"]
         params = lmfit.create_params(temp={"value": temp, "vary": vary_temp})
         model_cls = FermiEdgeModel
 
     model = model_cls()
@@ -226,20 +228,20 @@
         parallel_kw = {}
 
     if fixed_center is not None:
         params["center"].set(value=fixed_center, vary=False)
 
     if any(b != 1 for b in bin_size):
         gold_binned = gold.coarsen(alpha=bin_size[0], eV=bin_size[1], boundary="trim")
-        gold = gold_binned.mean()
+        gold = gold_binned.mean()  # type: ignore[attr-defined]
 
     gold_sel = gold.sel(alpha=slice(*angle_range), eV=slice(*eV_range))
 
     # Assuming Poisson noise, the weights are the square root of the counts.
-    weights = 1 / np.sqrt(gold_sel.sum("eV").values)
+    weights = 1 / np.sqrt(np.asarray(gold_sel.sum("eV").values))
 
     n_fits = len(gold_sel.alpha)
 
     if parallel_obj is None:
         if n_fits > 20:
             parallel_kw.setdefault("n_jobs", -1)
         else:
@@ -269,15 +271,15 @@
             **kwargs,
         )
         return res
 
     tqdm_kw = {"desc": "Fitting", "total": n_fits, "disable": not progress}
 
     if parallel_obj.return_generator:
-        fitresults = tqdm.auto.tqdm(
+        fitresults = tqdm.auto.tqdm(  # type: ignore[call-overload]
             parallel_obj(
                 joblib.delayed(_fit)(gold_sel.isel(alpha=i), weights[i])
                 for i in range(n_fits)
             ),
             **tqdm_kw,
         )
     else:
@@ -292,35 +294,32 @@
                 joblib.delayed(_fit)(gold_sel.isel(alpha=i), weights[i])
                 for i in range(n_fits)
             )
 
     if return_full:
         return list(fitresults)
 
-    xval = []
+    xval: list[npt.NDArray] = []
     res_vals = []
 
     for i, r in enumerate(fitresults):
         if hasattr(r, "uvars"):
             center_ufloat = r.uvars["center"]
 
             if normalize:
                 center_ufloat = center_ufloat * stdx + avgx
 
             if not np.isnan(center_ufloat.std_dev):
                 xval.append(gold_sel.alpha.values[i])
                 res_vals.append([center_ufloat.nominal_value, center_ufloat.std_dev])
 
-    xval = np.asarray(xval)
+    coords = {"alpha": np.asarray(xval)}
     yval, yerr = np.asarray(res_vals).T
 
-    return (
-        xr.DataArray(yval, coords={"alpha": xval}),
-        xr.DataArray(yerr, coords={"alpha": xval}),
-    )
+    return xr.DataArray(yval, coords=coords), xr.DataArray(yerr, coords=coords)
 
 
 def poly_from_edge(
     center, weights=None, degree=4, method="leastsq", scale_covar=True
 ) -> lmfit.model.ModelResult:
     model = PolynomialModel(degree=degree)
     pars = model.guess(center.values, x=center[center.dims[0]].values)
@@ -332,15 +331,15 @@
         method=method,
         scale_covar=scale_covar,
     )
     return modelresult
 
 
 def spline_from_edge(
-    center, weights: Sequence[float] | None = None, lam: float | None = None
+    center, weights: npt.ArrayLike | None = None, lam: float | None = None
 ) -> scipy.interpolate.BSpline:
     spl = scipy.interpolate.make_smoothing_spline(
         center.alpha.values,
         center.values,
         w=np.asarray(weights),
         lam=lam,
     )
@@ -444,15 +443,15 @@
         ax2.set_ylim(autoscale_to(res.data))
 
     ax1.set_title("")
     ax2.set_title("")
 
 
 def poly(
-    gold: xr.DataArray | xr.Dataset,
+    gold: xr.DataArray,
     angle_range: tuple[float, float],
     eV_range: tuple[float, float],
     bin_size: tuple[int, int] = (1, 1),
     temp: float | None = None,
     vary_temp: bool = False,
     fast: bool = False,
     method: str = "leastsq",
@@ -497,15 +496,15 @@
         corr = correct_with_edge(gold, modelresult, plot=False)
         return modelresult, corr
     else:
         return modelresult
 
 
 def spline(
-    gold: xr.DataArray | xr.Dataset,
+    gold: xr.DataArray,
     angle_range: tuple[float, float],
     eV_range: tuple[float, float],
     bin_size: tuple[int, int] = (1, 1),
     temp: float | None = None,
     vary_temp: bool = False,
     fast: bool = False,
     method: str = "leastsq",
@@ -539,15 +538,15 @@
         corr = correct_with_edge(gold, spl, plot=False)
         return spl, corr
     else:
         return spl
 
 
 def resolution(
-    gold: xr.DataArray | xr.Dataset,
+    gold: xr.DataArray,
     angle_range: tuple[float, float],
     eV_range_edge: tuple[float, float],
     eV_range_fit: tuple[float, float] | None = None,
     bin_size: tuple[int, int] = (1, 1),
     degree: int = 4,
     fast: bool = False,
     method: str = "leastsq",
```

### Comparing `erlab-2.3.0/src/erlab/analysis/image.py` & `erlab-2.3.1/src/erlab/analysis/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 
 Note
 ----
 For scipy-based filter functions, the default value of the `mode` argument is 'nearest',
 unlike the scipy default of 'reflect'.
 """
 
-from collections.abc import Sequence
+from collections.abc import Collection, Mapping, Sequence, Sized, Hashable
 
 import numpy as np
 import numpy.typing as npt
 import scipy
 import scipy.ndimage
 import xarray as xr
 from numba import carray, cfunc, types
 
 
 def gaussian_filter(
     darr: xr.DataArray,
-    sigma: float | dict[str, float] | Sequence[float],
-    order: int | Sequence[int] | dict[str, int] = 0,
-    mode: str | Sequence[str] | dict[str, str] = "nearest",
+    sigma: float | Collection[float] | Mapping[Hashable, float],
+    order: int | Sequence[int] | Mapping[Hashable, int] = 0,
+    mode: str | Sequence[str] | Mapping[Hashable, str] = "nearest",
     cval: float = 0.0,
     truncate: float = 4.0,
     *,
-    radius: None | float | Sequence[float] | dict[str, float] = None,
+    radius: None | float | Collection[float] | Mapping[Hashable, float] = None,
 ) -> xr.DataArray:
     """Coordinate-aware wrapper around `scipy.ndimage.gaussian_filter`.
 
     Parameters
     ----------
     darr
         The input DataArray.
@@ -95,65 +95,75 @@
         [10, 12, 14, 15, 17],
         [20, 22, 24, 25, 27],
         [29, 31, 33, 34, 36],
         [36, 38, 40, 41, 43]])
     Dimensions without coordinates: x, y
 
     """
-    if np.isscalar(sigma):
-        sigma = dict.fromkeys(darr.dims, sigma)
-    elif not isinstance(sigma, dict):
-        sigma = dict(zip(darr.dims, sigma))
+    if isinstance(sigma, Mapping):
+        sigma_dict = dict(sigma)
+    elif np.isscalar(sigma):
+        sigma_dict = dict.fromkeys(darr.dims, sigma)
+    elif isinstance(sigma, Collection):
+        sigma_dict = dict(zip(darr.dims, sigma, strict=True))
+    else:
+        raise TypeError("`sigma` must be a scalar, sequence, or mapping")
 
     # Get the axis indices to apply the filter
-    axes = tuple(darr.get_axis_num(d) for d in sigma.keys())
+    axes = tuple(darr.get_axis_num(d) for d in sigma_dict.keys())
 
     # Convert arguments to tuples acceptable by scipy
-    if isinstance(order, dict):
-        order = tuple(order.get(d, 0) for d in sigma.keys())
-    if isinstance(mode, dict):
-        mode = tuple(mode[d] for d in sigma.keys())
-    if radius is not None:
-        if len(radius) != len(sigma):
-            raise ValueError("`radius` does not match dimensions of `sigma`")
+    if isinstance(order, Mapping):
+        order = tuple(order.get(str(d), 0) for d in sigma_dict.keys())
+    if isinstance(mode, Mapping):
+        mode = tuple(mode[str(d)] for d in sigma_dict.keys())
 
-        if np.isscalar(radius):
-            radius = dict.fromkeys(sigma.keys(), radius)
-        elif not isinstance(radius, dict):
-            radius = dict(zip(sigma.keys(), radius))
+    if radius is not None:
+        if isinstance(radius, Mapping):
+            radius_dict = dict(radius)
+        elif isinstance(radius, Sized):
+            if len(radius) != len(sigma_dict):
+                raise ValueError("`radius` does not match dimensions of `sigma`")
+            radius_dict = dict(zip(sigma_dict.keys(), radius, strict=True))
+        elif np.isscalar(radius):
+            radius_dict = dict.fromkeys(sigma_dict.keys(), radius)
+        else:
+            raise TypeError("`radius` must be a scalar, sequence, or mapping")
 
         # Calculate radius in pixels
-        radius: tuple[int, ...] = tuple(
+        radius_pix: tuple[int, ...] | None = tuple(
             round(r / (darr[d].values[1] - darr[d].values[0]))
-            for d, r in radius.items()
+            for d, r in radius_dict.items()
         )
+    else:
+        radius_pix = None
 
     # Calculate sigma in pixels
-    sigma: tuple[float, ...] = tuple(
-        val / (darr[d].values[1] - darr[d].values[0]) for d, val in sigma.items()
+    sigma_pix: tuple[float, ...] = tuple(
+        val / (darr[d].values[1] - darr[d].values[0]) for d, val in sigma_dict.items()
     )
 
     return darr.copy(
         data=scipy.ndimage.gaussian_filter(
             darr.values,
-            sigma=sigma,
+            sigma=sigma_pix,
             order=order,
             mode=mode,
             cval=cval,
             truncate=truncate,
-            radius=radius,
+            radius=radius_pix,
             axes=axes,
         )
     )
 
 
 def gaussian_laplace(
     darr: xr.DataArray,
-    sigma: float | dict[str, float] | Sequence[float],
-    mode: str | Sequence[str] | dict[str, str] = "nearest",
+    sigma: float | Collection[float] | Mapping[str, float],
+    mode: str | Sequence[str] | Mapping[str, str] = "nearest",
     cval: float = 0.0,
     **kwargs,
 ) -> xr.DataArray:
     """Coordinate-aware wrapper around `scipy.ndimage.gaussian_laplace`.
 
     This function calculates the Laplacian of the given array using Gaussian second
     derivatives.
@@ -191,36 +201,43 @@
     - The input array is assumed to be regularly spaced.
 
     See Also
     --------
     :func:`scipy.ndimage.gaussian_laplace` : The underlying function used to apply the
         filter.
     """
-    if np.isscalar(sigma):
-        sigma = dict.fromkeys(darr.dims, sigma)
-    elif not isinstance(sigma, dict):
-        sigma = dict(zip(darr.dims, sigma))
 
-    if len(sigma) != darr.ndim:
+    if isinstance(sigma, Mapping):
+        sigma_dict = dict(sigma)
+    elif np.isscalar(sigma):
+        sigma_dict = dict.fromkeys(darr.dims, sigma)
+    elif isinstance(sigma, Collection):
+        sigma_dict = dict(zip(darr.dims, sigma, strict=True))
+    else:
+        raise TypeError("`sigma` must be a scalar, sequence, or mapping")
+
+    if len(sigma_dict) != darr.ndim:
+        required_dims = set(darr.dims) - set(sigma_dict.keys())
         raise ValueError(
-            "`sigma` must be provided for every dimension of the DataArray"
+            "`sigma` missing for the following dimension"
+            f"{'' if len(required_dims) == 1 else 's'}: {required_dims}"
         )
 
     # Convert mode to tuple acceptable by scipy
     if isinstance(mode, dict):
-        mode = tuple(mode[d] for d in sigma.keys())
+        mode = tuple(mode[d] for d in sigma_dict.keys())
 
     # Calculate sigma in pixels
-    sigma: tuple[float, ...] = tuple(
-        val / (darr[d].values[1] - darr[d].values[0]) for d, val in sigma.items()
+    sigma_pix: tuple[float, ...] = tuple(
+        val / (darr[d].values[1] - darr[d].values[0]) for d, val in sigma_dict.items()
     )
 
     return darr.copy(
         data=scipy.ndimage.gaussian_laplace(
-            darr.values, sigma=sigma, mode=mode, cval=cval, **kwargs
+            darr.values, sigma=sigma_pix, mode=mode, cval=cval, **kwargs
         )
     )
 
 
 def gradient_magnitude(
     input: npt.NDArray[np.float64],
     dx: np.float64,
```

### Comparing `erlab-2.3.0/src/erlab/analysis/interpolate.py` & `erlab-2.3.1/src/erlab/analysis/interpolate.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,9 +346,9 @@
 def _get_interpolator_nd_fast(method, **kwargs):
     if method == "linearfast":
         return interpn, kwargs
     else:
         return _get_interpolator_nd_original(method, **kwargs)
 
 
-xarray.core.missing._get_interpolator = _get_interpolator_fast
+xarray.core.missing._get_interpolator = _get_interpolator_fast  # type: ignore[assignment]
 xarray.core.missing._get_interpolator_nd = _get_interpolator_nd_fast
```

### Comparing `erlab-2.3.0/src/erlab/analysis/kspace.py` & `erlab-2.3.1/src/erlab/analysis/kspace.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 """
 
 import enum
 from collections.abc import Callable
 
 import numpy as np
 import numpy.typing as npt
+import xarray
 
 import erlab.constants
 import erlab.io
 import erlab.lattice
 
 
 class AxesConfiguration(enum.IntEnum):
@@ -60,15 +61,15 @@
     k_tot = erlab.constants.rel_kconv * np.sqrt(kinetic_energy)
     k_perp_sq = k_tot**2 - kx**2 - ky**2
     k_z_sq = k_perp_sq + inner_potential / erlab.constants.rel_kzconv
     return np.sqrt(np.clip(k_z_sq, a_min=0, a_max=None))
 
 
 def get_kconv_func(
-    kinetic_energy: float | npt.NDArray,
+    kinetic_energy: float | npt.NDArray | xarray.DataArray,
     configuration: AxesConfiguration,
     angle_params: dict[str, float],
 ) -> tuple[Callable, Callable]:
     """
     Returns the appropriate momentum conversion functions based on the given
     configuration and kinetic energy.
 
@@ -118,34 +119,28 @@
     <https://numpy.org/doc/stable/user/basics.broadcasting.html>`_
 
     """
     k_tot = erlab.constants.rel_kconv * np.sqrt(kinetic_energy)
 
     match configuration:
         case AxesConfiguration.Type1:
-            func = _kconv_func_type1
+            func: Callable = _kconv_func_type1
         case AxesConfiguration.Type2:
             func = _kconv_func_type2
         case AxesConfiguration.Type1DA:
             func = _kconv_func_type1_da
         case AxesConfiguration.Type2DA:
             func = _kconv_func_type2_da
         case _:
             ValueError(f"Invalid configuration {configuration}")
 
     return func(k_tot, **angle_params)
 
 
-def _kconv_func_type1(
-    k_tot: float | npt.NDArray,
-    delta: float = 0.0,
-    xi: float = 0.0,
-    xi0: float = 0.0,
-    beta0: float = 0.0,
-):
+def _kconv_func_type1(k_tot, delta=0.0, xi=0.0, xi0=0.0, beta0=0.0):
     cd, sd = np.cos(np.deg2rad(delta)), np.sin(np.deg2rad(delta))  # δ
     cx, sx = np.cos(np.deg2rad(xi - xi0)), np.sin(np.deg2rad(xi - xi0))  # ξ - ξ0
 
     k_tot_sq = k_tot**2
 
     def _forward_func(alpha, beta):
         alpha_r, beta_r = np.deg2rad(alpha), np.deg2rad(beta - beta0)
@@ -175,21 +170,15 @@
         beta = np.arctan((sd * kx - cd * ky) / (sx * (cd * kx + sd * ky) + cx * kperp))
 
         return np.rad2deg(alpha), np.rad2deg(beta) + beta0
 
     return _forward_func, _inverse_func
 
 
-def _kconv_func_type2(
-    k_tot: float | npt.NDArray,
-    delta: float = 0.0,
-    xi: float = 0.0,
-    xi0: float = 0.0,
-    beta0: float = 0.0,
-):
+def _kconv_func_type2(k_tot, delta=0.0, xi=0.0, xi0=0.0, beta0=0.0):
     cd, sd = np.cos(np.deg2rad(delta)), np.sin(np.deg2rad(delta))  # δ
     cx, sx = np.cos(np.deg2rad(xi - xi0)), np.sin(np.deg2rad(xi - xi0))  # ξ - ξ0
 
     k_tot_sq = k_tot**2
 
     def _forward_func(alpha, beta):
         alpha_r, beta_r = np.deg2rad(alpha), np.deg2rad(beta - beta0)
@@ -219,42 +208,28 @@
         beta = np.arctan((cd * kx + sd * ky) / kperp)
 
         return np.rad2deg(alpha), np.rad2deg(beta) + beta0
 
     return _forward_func, _inverse_func
 
 
-def _kconv_func_type1_da(
-    k_tot: float | npt.NDArray,
-    delta: float = 0.0,
-    chi: float = 0.0,
-    chi0: float = 0.0,
-    xi: float = 0.0,
-    xi0: float = 0.0,
-):
+def _kconv_func_type1_da(k_tot, delta=0.0, chi=0.0, chi0=0.0, xi=0.0, xi0=0.0):
     _fwd_2, _inv_2 = _kconv_func_type2_da(k_tot, delta, chi, chi0, xi, xi0)
 
     def _forward_func(alpha, beta):
         return _fwd_2(-beta, alpha)
 
     def _inverse_func(kx, ky, kz=None):
         alpha, beta = _inv_2(kx, ky, kz)
         return beta, -alpha
 
     return _forward_func, _inverse_func
 
 
-def _kconv_func_type2_da(
-    k_tot: float | npt.NDArray,
-    delta: float = 0.0,
-    chi: float = 0.0,
-    chi0: float = 0.0,
-    xi: float = 0.0,
-    xi0: float = 0.0,
-):
+def _kconv_func_type2_da(k_tot, delta=0.0, chi=0.0, chi0=0.0, xi=0.0, xi0=0.0):
     cd, sd = np.cos(np.deg2rad(delta)), np.sin(np.deg2rad(delta))  # δ, azimuth
     cx, sx = np.cos(np.deg2rad(xi - xi0)), np.sin(np.deg2rad(xi - xi0))  # ξ
     cc, sc = np.cos(np.deg2rad(chi - chi0)), np.sin(np.deg2rad(chi - chi0))  # χ
 
     t11, t12, t13 = cx * cd, cx * sd, -sx
     t21, t22, t23 = sc * sx * cd - cc * sd, sc * sx * sd + cc * cd, sc * cx
     t31, t32, t33 = cc * sx * cd + sc * sd, cc * sx * sd - sc * cd, cc * cx
@@ -296,15 +271,15 @@
         if kz is None:
             k_sq = k_tot_sq
             k = k_tot
         else:
             k_sq = kx**2 + ky**2 + kz**2
             k = np.sqrt(k_sq)
 
-        kperp = _kperp_func(k_sq, kx, ky)  # sqrt(k² − k_x² − k_y²)
+        kperp = _kperp_func(k_sq, kx, ky)  # sqrt(k² - k_x² - k_y²)
 
         proj1 = t11 * kx + t12 * ky + t13 * kperp
         proj2 = t21 * kx + t22 * ky + t23 * kperp
         proj3 = t31 * kx + t32 * ky + t33 * kperp
 
         # Type I DA
         # alpha = (
```

### Comparing `erlab-2.3.0/src/erlab/analysis/mask/__init__.py` & `erlab-2.3.1/src/erlab/analysis/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/analysis/mask/polygon.py` & `erlab-2.3.1/src/erlab/analysis/mask/polygon.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,14 +156,16 @@
     match bounded_side(points, point):
         case Side.ON_UNBOUNDED_SIDE:
             return False
         case Side.ON_BOUNDED_SIDE:
             return True
         case Side.ON_BOUNDARY:
             return boundary
+        case _:
+            return False
 
 
 @numba.njit(nogil=True, cache=True)
 def bounded_side(points: npt.NDArray[np.float64], point: tuple[float, float]) -> Side:
     """Computes if a point is inside, outside, or on the boundary of a polygon.
 
     The polygon is defined by the sequence of points [first,last). Being inside is
```

### Comparing `erlab-2.3.0/src/erlab/analysis/transform.py` & `erlab-2.3.1/src/erlab/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/analysis/utilities.py` & `erlab-2.3.1/src/erlab/analysis/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 __all__ = ["shift"]
 
 import itertools
 import warnings
+from typing import cast
 
 import numpy as np
 import scipy.ndimage
 import xarray as xr
 
 
 def shift(
@@ -81,58 +82,61 @@
         if dim not in darr.dims:
             raise ValueError(f"Dimension {dim} in shift array not found in input array")
         if darr[dim].size != shift[dim].size:
             raise ValueError(
                 f"Dimension {dim} in shift array has different size than input array"
             )
 
-    domain_indices: list[int] = [darr.get_axis_num(ax) for ax in shift.dims]
+    domain_indices: tuple[int, ...] = darr.get_axis_num(shift.dims)
 
     # `along` must be evenly spaced and monotonic increasing
     out = darr.sortby(along).copy()
 
     # Normalize shift values
     along_step: float = out[along].values[1] - out[along].values[0]
     shift = (shift.copy() / along_step).fillna(0.0)
 
     if shift_coords:
         # We first apply the integer part of the average shift to the coords
-        rigid_shift = np.round(shift.values.mean())
+        rigid_shift: float = np.round(shift.values.mean())
         shift = shift - rigid_shift
 
         # Apply coordinate shift
         out = out.assign_coords({along: out[along].values + rigid_shift * along_step})
 
         # The bounds of the remaining shift values are used to pad the data
         nshift_min, nshift_max = shift.values.min(), shift.values.max()
-        pads: tuple[int] = min(0, round(nshift_min)), max(0, round(nshift_max))
+        pads: tuple[int, int] = min(0, round(nshift_min)), max(0, round(nshift_max))
 
         # Construct new coordinate array
         new_along = np.linspace(
             out[along].values[0] + pads[0] * along_step,
             out[along].values[-1] + pads[1] * along_step,
             out[along].size + sum(np.abs(pads)),
         )
 
         # Pad the data and assign new coordinates
-        out = out.pad({along: np.abs(pads)}, mode="constant", constant_values=np.nan)
+        out = out.pad(
+            {along: tuple(np.abs(pads))}, mode="constant", constant_values=np.nan
+        )
         out = out.assign_coords({along: new_along})
 
     for idxs in itertools.product(*[range(darr.shape[i]) for i in domain_indices]):
         # Construct slices for indexing
-        slices = [slice(None)] * darr.ndim
-        for domain_index, i in zip(domain_indices, idxs):
-            slices[domain_index] = i
-        slices = tuple(slices)
+        _slices: list[slice | int] = [slice(None)] * darr.ndim
+        for domain_index, i in zip(domain_indices, idxs, strict=True):
+            _slices[domain_index] = i
+
+        slices: tuple[slice | int, ...] = tuple(_slices)
 
         # Initialize arguments to `scipy.ndimage.shift`
         input = out[slices]
-        shifts = [0] * input.ndim
-        shift_val: float = float(shift.isel(dict(zip(shift.dims, idxs))))
-        shifts[input.get_axis_num(along)] = shift_val
+        shifts: list[float] = [0.0] * input.ndim
+        shift_val: float = float(shift.isel(dict(zip(shift.dims, idxs, strict=True))))
+        shifts[cast(int, input.get_axis_num(along))] = shift_val
 
         # Apply shift
         out[slices] = scipy.ndimage.shift(input.values, shifts, **shift_kwargs)
 
     return out
```

### Comparing `erlab-2.3.0/src/erlab/characterization/resistance.py` & `erlab-2.3.1/src/erlab/io/characterization/resistance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Functions related to analyzing temperature-dependent resistance data.
+"""Functions related to loading temperature-dependent resistance data.
 
 Currently only supports loading raw data from ``.dat`` and ``.csv`` files output by
 physics lab III equipment.
 
 """
 
 import os
```

### Comparing `erlab-2.3.0/src/erlab/characterization/xrd.py` & `erlab-2.3.1/src/erlab/io/characterization/xrd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Functions related to analyzing x-ray diffraction spectra.
+"""Functions related to loading x-ray diffraction spectra.
 
 Currently only supports loading raw data from igor ``.itx`` files.
 
 """
 
 __all__ = ["load_xrd_itx"]
 
@@ -53,17 +53,20 @@
 
     >>> xrd_data.yobs.plot()
 
     """
     kwargs.setdefault("encoding", "windows-1252")
     with open(path, **kwargs) as file:
         content = file.read()
-    head, data = re.search(
-        r"IGOR\nWAVES/O\s(.*?)\nBEGIN\n(.+?)\nEND", content, re.DOTALL
-    ).groups()
+
+    search = re.search(r"IGOR\nWAVES/O\s(.*?)\nBEGIN\n(.+?)\nEND", content, re.DOTALL)
+    if search is None:
+        raise ValueError("Failed to parse .itx file.")
+
+    head, data = search.groups()
     head = head.split(", ")
 
     data = np.array(
         ast.literal_eval("[[" + data.replace("\n", "],[").replace(" ", ",") + "]]")
     )
     ds = xr.Dataset({head[i]: ([head[0]], data[:, i]) for i in range(len(head))})
     if "diff" in ds.data_vars:
```

### Comparing `erlab-2.3.0/src/erlab/constants.py` & `erlab-2.3.1/src/erlab/constants.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/interactive/__init__.py` & `erlab-2.3.1/src/erlab/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/interactive/bzplot.py` & `erlab-2.3.1/src/erlab/interactive/bzplot.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,19 +45,28 @@
                     [1.02619483, 1.77742159, 0.0],
                     [0.0, 0.0, 1.04510734],
                 ]
             )
             param_type = "bvec"
 
         if param_type == "lattice":
+            if len(params) != 6:
+                raise TypeError("Lattice parameters must be a 6-tuple.")
+
             bvec = to_reciprocal(abc2avec(*params))
-        elif param_type == "avec":
-            bvec = to_reciprocal(params)
-        elif param_type == "bvec":
-            bvec = params
+        else:
+            if not isinstance(params, np.ndarray):
+                raise TypeError("Lattice vectors must be a numpy array.")
+            if params.shape != (3, 3):
+                raise TypeError("Lattice vectors must be a 3 by 3 numpy array.")
+
+            if param_type == "avec":
+                bvec = to_reciprocal(params)
+            elif param_type == "bvec":
+                bvec = params
 
         self.controls = None
         self.plot = BZPlotWidget(bvec)
         self.setCentralWidget(self.plot)
 
         self.controls = LatticeWidget(bvec)
         self.controls.sigChanged.connect(self.plot.set_bvec)
```

### Comparing `erlab-2.3.0/src/erlab/interactive/colors.py` & `erlab-2.3.1/src/erlab/interactive/colors.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,25 @@
     "pg_colormap_names",
     "pg_colormap_powernorm",
     "pg_colormap_to_QPixmap",
 ]
 
 import weakref
 from collections.abc import Iterable, Sequence
-from typing import Literal
+from typing import TYPE_CHECKING, Literal
 
-import matplotlib.colors as mcolors
+import matplotlib.colors
 import numpy as np
 import numpy.typing as npt
 import pyqtgraph as pg
 from qtpy import QtCore, QtGui, QtWidgets
 
+if TYPE_CHECKING:
+    from matplotlib.typing import ColorType
+
 EXCLUDED_CMAPS: tuple[str, ...] = (
     "prism",
     "tab10",
     "tab20",
     "tab20b",
     "tab20c",
     "flag",
@@ -152,24 +155,24 @@
 
 
 class ColorMapGammaWidget(QtWidgets.QWidget):
     valueChanged = QtCore.Signal(float)  #: :meta private:
 
     def __init__(
         self,
-        parent: QtWidgets.QWidget = None,
+        parent: QtWidgets.QWidget | None = None,
         value: float = 1.0,
         slider_cls: type | None = None,
         spin_cls: type | None = None,
     ):
         super().__init__(parent=parent)
-        self.setLayout(QtWidgets.QHBoxLayout(self))
-        self.layout().setContentsMargins(0, 0, 0, 0)
-
-        self.layout().setSpacing(3)
+        layout = QtWidgets.QHBoxLayout(self)
+        self.setLayout(layout)
+        layout.setContentsMargins(0, 0, 0, 0)
+        layout.setSpacing(3)
 
         if slider_cls is None:
             slider_cls = QtWidgets.QSlider
         if spin_cls is None:
             spin_cls = QtWidgets.QDoubleSpinBox
 
         self.spin = spin_cls(
@@ -198,38 +201,38 @@
 
         self.slider.setRange(
             self.gamma_scale(self.spin.minimum()),
             self.gamma_scale(self.spin.maximum()),
         )
         self.slider.valueChanged.connect(self.slider_changed)
 
-        self.layout().addWidget(self.label)
-        self.layout().addWidget(self.spin)
-        self.layout().addWidget(self.slider)
+        layout.addWidget(self.label)
+        layout.addWidget(self.spin)
+        layout.addWidget(self.slider)
 
     def value(self) -> float:
         return self.spin.value()
 
     def setValue(self, value: float):
         self.spin.setValue(value)
         self.slider.setValue(self.gamma_scale(value))
 
     def spin_changed(self, value: float):
         self.slider.blockSignals(True)
         self.slider.setValue(self.gamma_scale(value))
         self.slider.blockSignals(False)
         self.valueChanged.emit(value)
 
-    def slider_changed(self, value: float):
+    def slider_changed(self, value: float | int):
         self.spin.setValue(self.gamma_scale_inv(value))
 
     def gamma_scale(self, y: float) -> int:
         return round(1e4 * np.log10(y))
 
-    def gamma_scale_inv(self, x: int) -> float:
+    def gamma_scale_inv(self, x: float | int) -> float:
         return np.power(10, x * 1e-4)
 
 
 class BetterImageItem(pg.ImageItem):
     """:class:`pyqtgraph.ImageItem` with improved colormap support.
 
     Parameters
@@ -244,15 +247,15 @@
     sigColorChanged()
     sigLimitChanged(float, float)
 
     """
 
     sigColorChanged = QtCore.Signal()  #: :meta private:
 
-    def __init__(self, image: npt.NDArray = None, **kwargs):
+    def __init__(self, image: npt.NDArray | None = None, **kwargs):
         super().__init__(image, **kwargs)
 
     def set_colormap(
         self,
         cmap: pg.ColorMap | str,
         gamma: float,
         reverse: bool = False,
@@ -275,15 +278,15 @@
         self.sigColorChanged.emit()
 
 
 class BetterColorBarItem(pg.PlotItem):
     def __init__(
         self,
         parent: QtWidgets.QWidget | None = None,
-        image: Sequence[BetterImageItem] | BetterImageItem | None = None,
+        image: Iterable[BetterImageItem] | BetterImageItem | None = None,
         autoLevels: bool = False,
         limits: tuple[float, float] | None = None,
         pen: QtGui.QPen | str = "c",
         hoverPen: QtGui.QPen | str = "m",
         hoverBrush: QtGui.QBrush | str = "#FFFFFF33",
         **kargs,
     ):
@@ -382,32 +385,31 @@
         pass
 
     def setLimits(self, limits: tuple[float, float] | None):
         self._fixedlimits = limits
         if self._primary_image is not None:
             self.limit_changed()
 
-    def addImage(self, image: Sequence[BetterImageItem] | BetterImageItem):
-        # if isinstance(image, BetterImageItem):
-        if not np.iterable(image):
+    def addImage(self, image: Iterable[BetterImageItem] | BetterImageItem):
+        if not isinstance(image, Iterable):
             self._images.add(weakref.ref(image))
         else:
             for img in image:
                 self._images.add(weakref.ref(img))
 
-    def removeImage(self, image: Sequence[BetterImageItem] | BetterImageItem):
+    def removeImage(self, image: Iterable[BetterImageItem] | BetterImageItem):
         if isinstance(image, Iterable):
             for img in image:
                 self._images.remove(weakref.ref(img))
         else:
             self._images.remove(weakref.ref(image))
 
     def setImageItem(
         self,
-        image: Sequence[BetterImageItem] | BetterImageItem,
+        image: Iterable[BetterImageItem] | BetterImageItem,
         insert_in: pg.PlotItem | None = None,
     ):
         self.addImage(image)
         for img_ref in self._images:
             img = img_ref()
             if img is not None:
                 if hasattr(img, "sigLevelsChanged"):
@@ -523,17 +525,15 @@
     #     self._colorbar.setLookupTable(lut)
     #     # self._colorbar.setColorMap(cmap)
 
     def mouseDragEvent(self, ev):
         ev.ignore()
 
 
-def color_to_QColor(
-    c: str | tuple[float, ...], alpha: float | None = None
-) -> QtGui.QColor:
+def color_to_QColor(c: ColorType, alpha: float | None = None) -> QtGui.QColor:
     """Convert a matplotlib color to a :class:`PySide6.QtGui.QColor`.
 
     Parameters
     ----------
     c
         A valid matplotlib color. See the `matplotlib documentation
         <https://matplotlib.org/stable/tutorials/colors/colors.html>`_ for more
@@ -542,15 +542,15 @@
         If supplied, applies transparency to the color.
 
     Returns
     -------
     PySide6.QtGui.QColor
 
     """
-    return QtGui.QColor.fromRgbF(*mcolors.to_rgba(c, alpha=alpha))
+    return QtGui.QColor.fromRgbF(*matplotlib.colors.to_rgba(c, alpha=alpha))
 
 
 def pg_colormap_names(
     source: Literal["local", "all", "matplotlib"] = "all", exclude_local: bool = False
 ) -> list[str]:
     """Get all valid :obj:`pyqtgraph` colormap names.
 
@@ -696,9 +696,9 @@
     # cmap_arr = np.reshape(cmap.getColors()[:, None], (1, -1, 4), order='C')
     # cmap_arr = np.reshape(
     # cmap.getLookupTable(0, 1, w, alpha=True)[:, None], (1, -1, 4),
     # order='C')
     cmap_arr = cmap.getLookupTable(0, 1, w, alpha=True)[:, None]
 
     # print(cmap_arr.shape)
-    img = QtGui.QImage(cmap_arr, w, 1, QtGui.QImage.Format_RGBA8888)
+    img = QtGui.QImage(cmap_arr, w, 1, QtGui.QImage.Format.Format_RGBA8888)
     return QtGui.QPixmap.fromImage(img).scaled(w, h)
```

### Comparing `erlab-2.3.0/src/erlab/interactive/curvefittingtool.py` & `erlab-2.3.1/src/erlab/interactive/curvefittingtool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 import sys
+from typing import cast
 
 import lmfit
 import pyqtgraph as pg
 import xarray as xr
 from qtpy import QtCore, QtWidgets
 
 from erlab.analysis.fit.models import MultiPeakModel
@@ -50,15 +51,15 @@
     "emcee",
     "shgo",
     "dual_annealing",
 ]
 
 
 class SinglePeakWidget(ParameterGroup):
-    VALID_LINESHAPE = ["lorentzian", "gaussian"]
+    VALID_LINESHAPE: tuple[str, ...] = ("lorentzian", "gaussian")
 
     def __init__(self, peak_index):
         self.peak_index = peak_index
         super().__init__(
             **{
                 "Peak Shape": {"qwtype": "combobox", "items": self.VALID_LINESHAPE},
                 "height": {
@@ -92,15 +93,15 @@
         pd = {}
         for w in self.widgets_of_type(FittingParameterWidget):
             pd = pd | w.param_dict
         return pd
 
     @property
     def peak_shape(self) -> str:
-        return self.values["Peak Shape"]
+        return str(self.values["Peak Shape"])
 
 
 class PlotPeakItem(pg.PlotCurveItem):
     def __init__(self, param_widget: SinglePeakWidget, *args, **kargs):
         self.param_widget = param_widget
         super().__init__(*args, **kargs)
         self._pen_color = self.opts["pen"].color()
@@ -196,15 +197,15 @@
 class edctool(QtWidgets.QMainWindow):
     def __init__(self, data, n_bands: int = 1, parameters=None, *args, **kwargs):
         self.data = data
 
         self.qapp = QtCore.QCoreApplication.instance()
         if not self.qapp:
             self.qapp = QtWidgets.QApplication(sys.argv)
-        self.qapp.setStyle("Fusion")
+        cast(QtWidgets.QApplication, self.qapp).setStyle("Fusion")
         super().__init__()
         self.resize(720, 360)
 
         self._dock0 = QtWidgets.QDockWidget("Parameters", self)
         self._options = QtWidgets.QWidget(self)
         self._options_layout = QtWidgets.QVBoxLayout(self._options)
         self._params_init = ParameterGroup(
@@ -295,16 +296,16 @@
 
         self.modelplot = self.plotwidget.plot()
         self.modelplot.setPen(pg.mkPen("y"))
 
         self.fitplot = self.plotwidget.plot()
         self.fitplot.setPen(pg.mkPen("c"))
 
-        self.peakcurves = []
-        self.peaklines = []
+        self.peakcurves: list[PlotPeakItem] = []
+        self.peaklines: list[PlotPeakPosition] = []
 
         self.refresh_n_peaks()
 
         self._params_init.sigParameterChanged.connect(self._refresh_plot_peaks)
 
         self.setCentralWidget(self.plotwidget)
         self.addDockWidget(QtCore.Qt.DockWidgetArea.RightDockWidgetArea, self._dock0)
@@ -423,15 +424,15 @@
                     "const_bkg",
                     "offset",
                     "resolution",
                 )
             }
         )
         for i in range(self.n_bands):
-            self._params_peak.widget(i).set_values(
+            self._params_peak.widget(i).set_values(  # type: ignore[union-attr]
                 **{k[3:]: v for k, v in params.items() if k.startswith(f"p{i}")}
             )
 
     def __post_init__(self, execute=None):
         self.show()
         self.activateWindow()
         # self.raise_()
@@ -451,15 +452,15 @@
 class mdctool(QtWidgets.QMainWindow):
     def __init__(self, data, n_bands: int = 1, parameters=None, *args, **kwargs):
         self.data = data
 
         self.qapp = QtCore.QCoreApplication.instance()
         if not self.qapp:
             self.qapp = QtWidgets.QApplication(sys.argv)
-        self.qapp.setStyle("Fusion")
+        cast(QtWidgets.QApplication, self.qapp).setStyle("Fusion")
         super().__init__()
         self.resize(720, 360)
 
         self._dock0 = QtWidgets.QDockWidget("Parameters", self)
         self._options = QtWidgets.QWidget(self)
         self._options_layout = QtWidgets.QVBoxLayout(self._options)
         self._params_init = ParameterGroup(
@@ -530,16 +531,16 @@
 
         self.modelplot = self.plotwidget.plot()
         self.modelplot.setPen(pg.mkPen("y"))
 
         self.fitplot = self.plotwidget.plot()
         self.fitplot.setPen(pg.mkPen("c"))
 
-        self.peakcurves = []
-        self.peaklines = []
+        self.peakcurves: list[PlotPeakItem] = []
+        self.peaklines: list[PlotPeakPosition] = []
 
         self.refresh_n_peaks()
 
         self._params_init.sigParameterChanged.connect(self._refresh_plot_peaks)
 
         self.setCentralWidget(self.plotwidget)
         self.addDockWidget(QtCore.Qt.DockWidgetArea.RightDockWidgetArea, self._dock0)
@@ -656,15 +657,15 @@
                     "lin_bkg",
                     "const_bkg",
                     "resolution",
                 )
             }
         )
         for i in range(self.n_bands):
-            self._params_peak.widget(i).set_values(
+            self._params_peak.widget(i).set_values(  # type: ignore[union-attr]
                 **{k[3:]: v for k, v in params.items() if k.startswith(f"p{i}")}
             )
 
     def __post_init__(self, execute=None):
         self.show()
         self.activateWindow()
         # self.raise_()
```

### Comparing `erlab-2.3.0/src/erlab/interactive/derivative.py` & `erlab-2.3.1/src/erlab/interactive/derivative.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Interactive tool for visualizing dispersive data."""
 
 __all__ = ["dtool"]
 
 import functools
 import os
 import sys
+from typing import TYPE_CHECKING, cast
 
 import numpy as np
 import pyqtgraph as pg
 import varname
 import xarray as xr
 from qtpy import QtCore, QtWidgets, uic
 
@@ -22,22 +23,25 @@
 from erlab.interactive.utilities import (
     copy_to_clipboard,
     gen_function_code,
     parse_data,
     xImageItem,
 )
 
+if TYPE_CHECKING:
+    from collections.abc import Hashable
+
 
 class DerivativeTool(
-    *uic.loadUiType(os.path.join(os.path.dirname(__file__), "dtool.ui"))
+    *uic.loadUiType(os.path.join(os.path.dirname(__file__), "dtool.ui"))  # type: ignore[misc]
 ):
     def __init__(self, data: xr.DataArray, *, data_name: str | None = None):
         if data_name is None:
             try:
-                data_name = varname.argname("data", func=self.__init__, vars_only=False)
+                data_name = varname.argname("data", func=self.__init__, vars_only=False)  # type: ignore[misc]
             except varname.VarnameRetrievingError:
                 data_name = "data"
 
         self.data_name: str = data_name
 
         # Initialize UI
         super().__init__()
@@ -46,16 +50,16 @@
 
         if data.ndim != 2:
             raise ValueError("Input DataArray must be 2D")
 
         self.data: xr.DataArray = parse_data(data)
         self._result: xr.DataArray = self.data.copy()
 
-        self.xdim: str = self.data.dims[1]
-        self.ydim: str = self.data.dims[0]
+        self.xdim: Hashable = self.data.dims[1]
+        self.ydim: Hashable = self.data.dims[0]
 
         self.xinc: float = abs(float(self.data[self.xdim][1] - self.data[self.xdim][0]))
         self.yinc: float = abs(float(self.data[self.ydim][1] - self.data[self.ydim][0]))
 
         self.sx_spin.setRange(0.1 * self.xinc, 50 * self.xinc)
         self.sy_spin.setRange(0.1 * self.yinc, 50 * self.yinc)
 
@@ -134,19 +138,19 @@
 
     @functools.cached_property
     def processed_data(self) -> xr.DataArray:
         out = self.data
         if self.interp_group.isChecked():
             out = self.data.interp(
                 {
-                    self.xdim: np.linspace(
-                        *self.data[self.xdim][[0, -1]], self.nx_spin.value()
+                    self.xdim: np.linspace(  # type: ignore[call-overload]
+                        *self.data[self.xdim].values[[0, -1]], self.nx_spin.value()
                     ),
-                    self.ydim: np.linspace(
-                        *self.data[self.ydim][[0, -1]], self.ny_spin.value()
+                    self.ydim: np.linspace(  # type: ignore[call-overload]
+                        *self.data[self.ydim].values[[0, -1]], self.ny_spin.value()
                     ),
                 }
             )
         if self.smooth_group.isChecked():
             for _ in range(self.sn_spin.value()):
                 out = gaussian_filter(
                     out,
@@ -217,15 +221,17 @@
         data_name = (
             self.data_name
         )  # "".join([s.strip() for s in self.data_name.split("\n")])
         if self.interp_group.isChecked():
             arg_dict = {
                 dim: f"|np.linspace(*{data_name}['{dim}'][[0, -1]], {n})|"
                 for dim, n in zip(
-                    [self.xdim, self.ydim], [self.nx_spin.value(), self.ny_spin.value()]
+                    [self.xdim, self.ydim],
+                    [self.nx_spin.value(), self.ny_spin.value()],
+                    strict=True,
                 )
             }
             lines.append(
                 gen_function_code(
                     copy=False, **{f"_processed = {data_name}.interp": [arg_dict]}
                 )
             )
@@ -236,14 +242,15 @@
                 "sigma": dict(
                     zip(
                         (self.xdim, self.ydim),
                         [
                             np.round(s.value(), s.decimals())
                             for s in (self.sx_spin, self.sy_spin)
                         ],
+                        strict=True,
                     )
                 )
             }
             lines.append(f"_processed = {data_name}.copy()")
             data_name = "_processed"
             lines.extend(
                 (
@@ -306,15 +313,15 @@
         except varname.VarnameRetrievingError:
             data_name = "data"
 
     qapp = QtWidgets.QApplication.instance()
     if not qapp:
         qapp = QtWidgets.QApplication(sys.argv)
 
-    qapp.setStyle("Fusion")
+    cast(QtWidgets.QApplication, qapp).setStyle("Fusion")
 
     win = DerivativeTool(data, data_name=data_name)
     win.show()
     win.raise_()
     win.activateWindow()
 
     if execute is None:
```

### Comparing `erlab-2.3.0/src/erlab/interactive/dtool.ui` & `erlab-2.3.1/src/erlab/interactive/dtool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/interactive/fermiedge.py` & `erlab-2.3.1/src/erlab/interactive/fermiedge.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import erlab.analysis
 from erlab.interactive.imagetool import ImageTool
 from erlab.interactive.utilities import (
     AnalysisWindow,
     ParameterGroup,
     ROIControls,
     gen_function_code,
+    xImageItem,
 )
 from erlab.parallel import joblib_progress_qt
 
 if TYPE_CHECKING:
     import lmfit
     import scipy.interpolate
 
@@ -152,28 +153,31 @@
                 self._argnames["data_corr"] = varname.argname(
                     "data_corr", func=self.__init__, vars_only=False
                 )
             except varname.VarnameRetrievingError:
                 self._argnames["data_corr"] = "data_corr"
 
         self.data_corr = data_corr
+        self.hists: pg.HistogramLUTItem
+        self.axes: list[pg.PlotItem]
+        self.images: list[xImageItem]
 
         self.axes[1].setVisible(False)
         self.hists[1].setVisible(False)
         self.axes[2].setVisible(False)
         self.hists[2].setVisible(False)
 
         try:
             temp = float(self.data.attrs["temp_sample"])
         except KeyError:
             temp = 30.0
 
         self.params_roi = ROIControls(self.add_roi(0))
         self.params_edge = ParameterGroup(
-            **{
+            {
                 "T (K)": {"qwtype": "dblspin", "value": temp, "range": (0.0, 400.0)},
                 "Fix T": {"qwtype": "chkbox", "checked": True},
                 "Bin x": {"qwtype": "spin", "value": 1, "minimum": 1},
                 "Bin y": {"qwtype": "spin", "value": 1, "minimum": 1},
                 "Fast": {"qwtype": "chkbox", "checked": False},
                 "Method": {"qwtype": "combobox", "items": LMFIT_METHODS},
                 "Scale cov": {"qwtype": "chkbox", "checked": True},
@@ -191,15 +195,15 @@
                 },
             }
         )
 
         self.params_edge.widgets["Fast"].stateChanged.connect(self._toggle_fast)
 
         self.params_poly = ParameterGroup(
-            **{
+            {
                 "Degree": {"qwtype": "spin", "value": 4, "range": (1, 20)},
                 "Method": {"qwtype": "combobox", "items": LMFIT_METHODS},
                 "Scale cov": {"qwtype": "chkbox", "checked": True},
                 "Residuals": {"qwtype": "chkbox", "checked": False},
                 "Corrected": {"qwtype": "chkbox", "checked": False},
                 "Shift coords": {"qwtype": "chkbox", "checked": True},
                 "itool": {
@@ -216,15 +220,15 @@
                     "text": "Copy to clipboard",
                     "clicked": lambda: self.gen_code("poly"),
                 },
             }
         )
 
         self.params_spl = ParameterGroup(
-            **{
+            {
                 "Auto": {"qwtype": "chkbox", "checked": True},
                 "lambda": {
                     "qwtype": "dblspin",
                     "minimum": 0,
                     "maximum": 10000,
                     "singleStep": 0.001,
                     "decimals": 4,
@@ -295,26 +299,26 @@
             self.axes[i].addItem(self.polycurves[i])
         self.params_poly.sigParameterChanged.connect(lambda: self.perform_fit("poly"))
         self.params_spl.sigParameterChanged.connect(lambda: self.perform_fit("spl"))
 
         self.axes[0].disableAutoRange()
 
         # Setup time calculation
-        self.start_time: float | None = None
-        self.step_times: list[float] = []
+        self.start_time: float
+        self.step_times: list[float]
 
         # Setup progress bar
-        self.progress = QtWidgets.QProgressDialog(
+        self.progress: QtWidgets.QProgressDialog = QtWidgets.QProgressDialog(
             labelText="Fitting...",
             minimum=0,
             parent=self,
             minimumDuration=0,
             windowModality=QtCore.Qt.WindowModal,
         )
-        self.pbar = QtWidgets.QProgressBar()
+        self.pbar: QtWidgets.QProgressBar = QtWidgets.QProgressBar()
         self.progress.setBar(self.pbar)
         self.progress.setFixedSize(self.progress.size())
         self.progress.setCancelButtonText("Abort!")
         self.progress.canceled.disconnect(self.progress.cancel)  # don't auto close
         self.progress.canceled.connect(self.abort_fit)
         self.progress.setAutoReset(False)
         self.progress.cancel()
@@ -356,15 +360,15 @@
 
         self.progress.setLabelText(f"{round(timeleft)} seconds left...")
         self.pbar.setFormat(f"{n}/{self.progress.maximum()} finished")
 
     @QtCore.Slot()
     def perform_edge_fit(self):
         self.start_time = time.perf_counter()
-        self.step_times: list[float] = [0.0]
+        self.step_times = [0.0]
 
         self.progress.setVisible(True)
         self.params_roi.draw_button.setChecked(False)
         x0, y0, x1, y1 = (np.round(x, 3) for x in self.params_roi.roi_limits)
         params = self.params_edge.values
         n_total = len(
             self.data.alpha.coarsen(alpha=params["Bin x"], boundary="trim")
```

### Comparing `erlab-2.3.0/src/erlab/interactive/imagetool/__init__.py` & `erlab-2.3.1/src/erlab/interactive/imagetool/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,18 @@
 
 from __future__ import annotations
 
 __all__ = ["ImageTool", "itool"]
 
 import gc
 import sys
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, cast
 
+import numpy as np
+import numpy.typing as npt
 import xarray as xr
 from qtpy import QtCore, QtWidgets
 
 import erlab.io
 from erlab.interactive.imagetool.controls import (
     ItoolBinningControls,
     ItoolColormapControls,
@@ -34,31 +36,24 @@
 )
 from erlab.interactive.imagetool.core import ImageSlicerArea, SlicerLinkProxy
 from erlab.interactive.utilities import DictMenuBar, copy_to_clipboard
 
 if TYPE_CHECKING:
     from collections.abc import Callable, Sequence
 
-    import numpy as np
-    import numpy.typing as npt
-
     from erlab.interactive.imagetool.slicer import ArraySlicer
 
 
 def itool(
-    data: (
-        Sequence[xr.DataArray | npt.ArrayLike[np.floating]]
-        | xr.DataArray
-        | npt.ArrayLike[np.floating]
-    ),
+    data: Sequence[xr.DataArray | npt.NDArray] | xr.DataArray | npt.NDArray,
     link: bool = False,
     link_colors: bool = True,
     execute: bool | None = None,
     **kwargs,
-):
+) -> ImageTool | list[ImageTool] | None:
     """Create and display an ImageTool window.
 
     Parameters
     ----------
     data
         Array-like object or a sequence of such object with 2 to 4 dimensions. See
         notes.
@@ -74,70 +69,74 @@
     **kwargs
         Additional keyword arguments to be passed onto the underlying slicer area. For a
         full list of supported arguments, see the
         `erlab.interactive.imagetool.core.ImageSlicerArea` documentation.
 
     Returns
     -------
-    ImageTool or tuple of ImageTool
+    ImageTool or list of ImageTool
         The created ImageTool window(s).
 
     Notes
     -----
     - If `data` is a sequence of valid data, multiple ImageTool windows will be created
       and displayed.
     - If `link` is True, the ImageTool windows will be synchronized.
 
     Examples
     --------
     >>> itool(data, cmap="gray", gamma=0.5)
     >>> itool(data_list, link=True)
     """
 
-    qapp: QtWidgets.QApplication = QtWidgets.QApplication.instance()
+    qapp = QtWidgets.QApplication.instance()
     if not qapp:
         qapp = QtWidgets.QApplication(sys.argv)
-    qapp.setStyle("Fusion")
 
-    if isinstance(data, list | tuple):
-        win = ()
-        for d in data:
-            win += (ImageTool(d, **kwargs),)
-        for w in win:
-            w.show()
-        win[-1].activateWindow()
-        win[-1].raise_()
-
-        if link:
-            linker = SlicerLinkProxy(  # noqa: F841
-                *[w.slicer_area for w in win], link_colors=link_colors
-            )
-    else:
-        win = ImageTool(data, **kwargs)
-        win.show()
-        win.raise_()
-        win.activateWindow()
+    if isinstance(qapp, QtWidgets.QApplication):
+        qapp.setStyle("Fusion")
+
+    if isinstance(data, np.ndarray | xr.DataArray):
+        data = cast(list[npt.NDArray | xr.DataArray], [data])
+
+    itool_list = [ImageTool(d, **kwargs) for d in data]
+
+    for w in itool_list:
+        w.show()
+
+    if len(itool_list) == 0:
+        raise ValueError("No data provided")
+
+    itool_list[-1].activateWindow()
+    itool_list[-1].raise_()
+
+    if link:
+        linker = SlicerLinkProxy(  # noqa: F841
+            *[w.slicer_area for w in itool_list], link_colors=link_colors
+        )
+
     if execute is None:
         execute = True
         try:
             shell = get_ipython().__class__.__name__  # type: ignore
             if shell in ["ZMQInteractiveShell", "TerminalInteractiveShell"]:
                 execute = False
                 from IPython.lib.guisupport import start_event_loop_qt4
 
                 start_event_loop_qt4(qapp)
         except NameError:
             pass
+
     if execute:
         qapp.exec()
-        del win
+        del itool_list
         gc.collect()
 
         return None
-    return win
+    return itool_list
 
 
 class BaseImageTool(QtWidgets.QMainWindow):
     def __init__(self, data=None, parent=None, **kwargs):
         super().__init__(parent=parent)
         self.slicer_area = ImageSlicerArea(self, data, **kwargs)
         self.setCentralWidget(self.slicer_area)
@@ -227,15 +226,15 @@
     def colorAct(self):
         return tuple(
             self.action_dict[k]
             for k in ("colorInvertAct", "highContrastAct", "zeroCenterAct")
         )
 
     def _generate_menu_kwargs(self) -> dict:
-        menu_kwargs = {
+        menu_kwargs: dict[str, Any] = {
             "fileMenu": {
                 "title": "&File",
                 "actions": {
                     "&Open...": {
                         "shortcut": "Ctrl+O",
                         "triggered": self._open_file,
                     },
@@ -336,14 +335,15 @@
                     ("Shift Current Cursor Up × 10", "Ctrl+Shift+Up"),
                     ("Shift Current Cursor Down × 10", "Ctrl+Shift+Down"),
                     ("Shift Current Cursor Right × 10", "Ctrl+Shift+Right"),
                     ("Shift Current Cursor Left × 10", "Ctrl+Shift+Left"),
                 ),
                 (1, 1, 0, 0) * 2,
                 (1, -1, 1, -1, 10, -10, 10, -10),
+                strict=True,
             )
         ):
             menu_kwargs["viewMenu"]["actions"]["cursorMoveMenu"]["actions"][
                 f"ShiftCursorAct{i}"
             ] = {
                 "text": t,
                 "shortcut": s,
@@ -369,14 +369,15 @@
                     ("Shift Cursors Up × 10", "Ctrl+Alt+Shift+Up"),
                     ("Shift Cursors Down × 10", "Ctrl+Alt+Shift+Down"),
                     ("Shift Cursors Right × 10", "Ctrl+Alt+Shift+Right"),
                     ("Shift Cursors Left × 10", "Ctrl+Alt+Shift+Left"),
                 ),
                 (1, 1, 0, 0) * 2,
                 (1, -1, 1, -1, 10, -10, 10, -10),
+                strict=True,
             )
         ):
             menu_kwargs["viewMenu"]["actions"]["cursorMoveMenu"]["actions"][
                 f"ShiftAllCursorAct{i}"
             ] = {
                 "text": t,
                 "shortcut": s,
@@ -398,15 +399,17 @@
 
     def refreshMenus(self):
         self.action_dict["snapCursorAct"].blockSignals(True)
         self.action_dict["snapCursorAct"].setChecked(self.array_slicer.snap_to_data)
         self.action_dict["snapCursorAct"].blockSignals(False)
 
         cmap_props = self.slicer_area.colormap_properties
-        for ca, k in zip(self.colorAct, ["reversed", "highContrast", "zeroCentered"]):
+        for ca, k in zip(
+            self.colorAct, ["reversed", "highContrast", "zeroCentered"], strict=True
+        ):
             ca.blockSignals(True)
             ca.setChecked(cmap_props[k])
             ca.blockSignals(False)
 
     def _set_colormap_options(self):
         self.slicer_area.set_colormap(
             reversed=self.colorAct[0].isChecked(),
```

### Comparing `erlab-2.3.0/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py` & `erlab-2.3.1/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py`

 * *Files 0% similar despite different names*

```diff
@@ -835,15 +835,17 @@
             for span in self.spans[axis]:
                 if is_vertical(span):
                     span.set_xy(get_xy_x(*domain))
                 else:
                     span.set_xy(get_xy_y(*domain))
                 span.set_visible(self.visible)
             if self.useblit:
-                for i, span in list(zip(self.span_ax_index[axis], self.spans[axis])):
+                for i, span in list(
+                    zip(self.span_ax_index[axis], self.spans[axis], strict=True)
+                ):
                     self.axes[i].draw_artist(span)
 
     def get_index_of_value(self, axis, val):
         # return np.rint((val-self.lims[axis][0])/self.incs[axis]).astype(int)
         return min(
             np.searchsorted(self.coords[axis] + 0.5 * self.incs[axis], val),
             self.shape[axis] - 1,
@@ -964,15 +966,17 @@
                 #     (0, 4, 5, 1, 2, 3, 1, 2, 3),
                 #     self.maps + self.hists + (self.axes[1].yaxis,
                 #                               self.axes[2].xaxis,
                 #                               self.axes[3].yaxis))))
                 # self.pool(delayed(self.axes[i].draw_artist)(art) for i, art in list(zip(
                 #     (0, 1, 4, 0, 2, 5, 3, 5, 4), self.cursors)))
             else:
-                for i, art in list(zip(self.ax_index, self.all + self.scaling_axes)):
+                for i, art in list(
+                    zip(self.ax_index, self.all + self.scaling_axes, strict=True)
+                ):
                     self.axes[i].draw_artist(art)
             if any(self.averaged):
                 self.update_spans()
             self.canvas.blit()
         else:
             if any(self.averaged):
                 self.update_spans()
```

### Comparing `erlab-2.3.0/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py` & `erlab-2.3.1/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py`

 * *Files 0% similar despite different names*

```diff
@@ -1150,15 +1150,15 @@
                 (0, 0, 1, 0),
                 (1, 0, 0, 0),
                 (0, 0, 0, 1),
                 (0, 1, 1, 0),
             )
         else:
             raise NotImplementedError("Only supports 2D, 3D, and 4D arrays.")
-        for i, (p, sel) in enumerate(zip(self.axes, valid_selection)):
+        for i, (p, sel) in enumerate(zip(self.axes, valid_selection, strict=True)):
             p.setDefaultPadding(0)
             for axis in ["left", "bottom", "right", "top"]:
                 p.getAxis(axis).setTickFont(font)
                 p.getAxis(axis).setStyle(
                     autoExpandTextSpace=True, autoReduceTextSpace=True
                 )
             p.showAxes(sel, showValues=sel, size=(horiz_pad, vert_pad))
```

### Comparing `erlab-2.3.0/src/erlab/interactive/imagetool/controls.py` & `erlab-2.3.1/src/erlab/interactive/imagetool/controls.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,52 +9,55 @@
 
 from typing import TYPE_CHECKING
 
 import numpy as np
 import pyqtgraph as pg
 import qtawesome as qta
 from qtpy import QtCore, QtGui, QtWidgets
-
+import types
 from erlab.interactive.colors import ColorMapComboBox, ColorMapGammaWidget
 from erlab.interactive.utilities import BetterSpinBox
 
 if TYPE_CHECKING:
     import xarray as xr
+    from collections.abc import Mapping
 
     from erlab.interactive.imagetool.core import ImageSlicerArea
     from erlab.interactive.imagetool.slicer import ArraySlicer
 
 
 class IconButton(QtWidgets.QPushButton):
-    ICON_ALIASES = {
-        "invert": "mdi6.invert-colors",
-        "invert_off": "mdi6.invert-colors-off",
-        "contrast": "mdi6.contrast-box",
-        "lock": "mdi6.lock",
-        "unlock": "mdi6.lock-open-variant",
-        "bright_auto": "mdi6.brightness-auto",
-        "bright_percent": "mdi6.brightness-percent",
-        "colorbar": "mdi6.gradient-vertical",
-        "transpose_0": "mdi6.arrow-top-left-bottom-right",
-        "transpose_1": "mdi6.arrow-up-down",
-        "transpose_2": "mdi6.arrow-left-right",
-        "transpose_3": "mdi6.axis-z-arrow",
-        "snap": "mdi6.grid",
-        "snap_off": "mdi6.grid-off",
-        "palette": "mdi6.palette-advanced",
-        "styles": "mdi6.palette-swatch",
-        "layout": "mdi6.page-layout-body",
-        "zero_center": "mdi6.format-vertical-align-center",
-        "table_eye": "mdi6.table-eye",
-        "plus": "mdi6.plus",
-        "minus": "mdi6.minus",
-        "reset": "mdi6.backup-restore",
-        # all_cursors="mdi6.checkbox-multiple-outline",
-        "all_cursors": "mdi6.select-multiple",
-    }
+    ICON_ALIASES: Mapping[str, str] = types.MappingProxyType(
+        {
+            "invert": "mdi6.invert-colors",
+            "invert_off": "mdi6.invert-colors-off",
+            "contrast": "mdi6.contrast-box",
+            "lock": "mdi6.lock",
+            "unlock": "mdi6.lock-open-variant",
+            "bright_auto": "mdi6.brightness-auto",
+            "bright_percent": "mdi6.brightness-percent",
+            "colorbar": "mdi6.gradient-vertical",
+            "transpose_0": "mdi6.arrow-top-left-bottom-right",
+            "transpose_1": "mdi6.arrow-up-down",
+            "transpose_2": "mdi6.arrow-left-right",
+            "transpose_3": "mdi6.axis-z-arrow",
+            "snap": "mdi6.grid",
+            "snap_off": "mdi6.grid-off",
+            "palette": "mdi6.palette-advanced",
+            "styles": "mdi6.palette-swatch",
+            "layout": "mdi6.page-layout-body",
+            "zero_center": "mdi6.format-vertical-align-center",
+            "table_eye": "mdi6.table-eye",
+            "plus": "mdi6.plus",
+            "minus": "mdi6.minus",
+            "reset": "mdi6.backup-restore",
+            # all_cursors="mdi6.checkbox-multiple-outline",
+            "all_cursors": "mdi6.select-multiple",
+        }
+    )
 
     def __init__(self, on: str | None = None, off: str | None = None, **kwargs):
         self.icon_key_on = None
         self.icon_key_off = None
 
         if on is not None:
             self.icon_key_on = on
@@ -84,35 +87,39 @@
         if self.icon_key_off is not None:
             if self.isChecked():
                 self.setIcon(self.get_icon(self.icon_key_off))
                 return
         if self.icon_key_on is not None:
             self.setIcon(self.get_icon(self.icon_key_on))
 
-    def changeEvent(self, evt: QtCore.QEvent):  # handles dark mode
-        if evt.type() == QtCore.QEvent.Type.PaletteChange:
+    def changeEvent(self, evt: QtCore.QEvent | None):  # handles dark mode
+        if evt is not None and evt.type() == QtCore.QEvent.Type.PaletteChange:
             qta.reset_cache()
             self.refresh_icons()
         super().changeEvent(evt)
 
 
-def clear_layout(layout: QtWidgets.QLayout):
+def clear_layout(layout: QtWidgets.QLayout | None) -> None:
+    if layout is None:
+        return
     while layout.count():
         child = layout.takeAt(0)
-        if child.widget():
-            child.widget().deleteLater()
+        if child is not None:
+            w = child.widget()
+            if w is not None:
+                w.deleteLater()
 
 
 class ItoolControlsBase(QtWidgets.QWidget):
     def __init__(
         self, slicer_area: ImageSlicerArea | ItoolControlsBase, *args, **kwargs
     ):
         super().__init__(*args, **kwargs)
         self._slicer_area = slicer_area
-        self.sub_controls = []
+        self.sub_controls: list[QtWidgets.QWidget] = []
         self.initialize_layout()
         self.initialize_widgets()
         self.connect_signals()
         self.update()
 
     @property
     def data(self) -> xr.DataArray:
```

### Comparing `erlab-2.3.0/src/erlab/interactive/imagetool/core.py` & `erlab-2.3.1/src/erlab/interactive/imagetool/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import collections
 import functools
 import inspect
 import os
 import time
 import weakref
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Literal, TypedDict, cast
 
 import numpy as np
 import numpy.typing as npt
 import pyqtgraph as pg
 import xarray as xr
 from qtpy import QtCore, QtGui, QtWidgets
 
@@ -28,14 +28,22 @@
 
 if TYPE_CHECKING:
     from collections.abc import Callable, Iterable, Sequence
 
     from pyqtgraph.graphicsItems.ViewBox import ViewBoxMenu
     from pyqtgraph.GraphicsScene import mouseEvents
 
+    class ColorMapProperties(TypedDict):
+        cmap: str | pg.ColorMap
+        gamma: float
+        reversed: bool
+        highContrast: bool
+        zeroCentered: bool
+
+
 suppressnanwarning = np.testing.suppress_warnings()
 suppressnanwarning.filter(RuntimeWarning, r"All-NaN (slice|axis) encountered")
 
 
 def _link_splitters(
     s0: QtWidgets.QSplitter, s1: QtWidgets.QSplitter, reverse: bool = False
 ):
@@ -114,19 +122,21 @@
     Parameters
     ----------
     func
         The method to sync across multiple instances of `ImageSlicerArea`.
     indices
         If `True`, the input argument named `value` given to `func` are interpreted as
         indices, and will be converted to appropriate values for other instances of
-        `ImageSlicerArea`. The behavior of this conversion is determined by `steps`.
+        `ImageSlicerArea`. The behavior of this conversion is determined by `steps`. If
+        `True`, An input argument named `axis` of type integer must be present in the
+        decorated method to determine the axis along which the index is to be changed.
     steps
-        If `False`, considers `value` as an absolute index. If `True`, considers
-        `value` as a relative value such as the number of steps or bins. See the
-        implementation of `SlicerLinkProxy` for more information.
+        If `False`, considers `value` as an absolute index. If `True`, considers `value`
+        as a relative value such as the number of steps or bins. See the implementation
+        of `SlicerLinkProxy` for more information.
     color
         Boolean whether the decorated method is related to visualization, such as
         colormap control.
 
     """
 
     def my_decorator(func: Callable):
@@ -163,15 +173,15 @@
     link_colors
         Whether to sync color related changes.
     *slicers
         The slicers to link.
 
     """
 
-    def __init__(self, *slicers: list[ImageSlicerArea], link_colors: bool = True):
+    def __init__(self, *slicers: ImageSlicerArea, link_colors: bool = True):
         self.link_colors = link_colors
         self._slicers: set[ImageSlicerArea] = set()
         for s in slicers:
             self.add(s)
 
     def add(self, slicer: ImageSlicerArea):
         if slicer.is_linked:
@@ -224,28 +234,26 @@
         source: ImageSlicerArea,
         target: ImageSlicerArea,
         args: dict[str, Any],
         indices: bool,
         steps: bool,
     ):
         if indices:
-            axis: int | None = args.get("axis")
-            index: int | None = args.get("value")
+            index: int | None = args.get("value", None)
 
             if index is not None:
+                axis: int | None = args.get("axis")
+
                 if axis is None:
-                    args["value"] = [
-                        self.convert_index(source, target, a, i, steps)
-                        for (a, i) in zip(axis, index)
-                    ]
-                else:
-                    args["value"] = self.convert_index(
-                        source, target, axis, index, steps
+                    raise ValueError(
+                        "Axis argument not found in decorated method with `indices=True`"
                     )
 
+                args["value"] = self.convert_index(source, target, axis, index, steps)
+
         args["__slicer_skip_sync"] = True  # passed onto the decorator
         return args
 
     @staticmethod
     def convert_index(
         source: ImageSlicerArea,
         target: ImageSlicerArea,
@@ -305,23 +313,23 @@
     sigBinChanged(cursor, axes)
         Inherited from :class:`erlab.interactive.slicer.ArraySlicer`.
     sigShapeChanged()
         Inherited from :class:`erlab.interactive.slicer.ArraySlicer`.
 
     """
 
-    COLORS: list[QtGui.QColor] = [
+    COLORS: tuple[QtGui.QColor, ...] = (
         pg.mkColor(0.8),
         pg.mkColor("y"),
         pg.mkColor("m"),
         pg.mkColor("c"),
         pg.mkColor("g"),
         pg.mkColor("r"),
         pg.mkColor("b"),
-    ]  #: List of :class:`PySide6.QtGui.QColor` containing colors for multiple cursors.
+    )  #: :class:`PySide6.QtGui.QColor`\ s for multiple cursors.
 
     sigDataChanged = QtCore.Signal()  #: :meta private:
     sigCurrentCursorChanged = QtCore.Signal(int)  #: :meta private:
     sigViewOptionChanged = QtCore.Signal()  #: :meta private:
 
     @property
     def sigCursorCountChanged(self) -> QtCore.SignalInstance:
@@ -358,17 +366,19 @@
     ):
         super().__init__(parent)
 
         self._linking_proxy: SlicerLinkProxy | None = None
 
         self.bench = bench
 
-        self.setLayout(QtWidgets.QHBoxLayout())
-        self.layout().setContentsMargins(0, 0, 0, 0)
-        self.layout().setSpacing(0)
+        layout = QtWidgets.QHBoxLayout()
+        self.setLayout(layout)
+
+        layout.setContentsMargins(0, 0, 0, 0)
+        layout.setSpacing(0)
 
         self._splitters = (
             QtWidgets.QSplitter(QtCore.Qt.Orientation.Vertical),
             QtWidgets.QSplitter(QtCore.Qt.Orientation.Horizontal),
             QtWidgets.QSplitter(QtCore.Qt.Orientation.Vertical),
             QtWidgets.QSplitter(QtCore.Qt.Orientation.Vertical),
             QtWidgets.QSplitter(QtCore.Qt.Orientation.Horizontal),
@@ -379,27 +389,27 @@
             s.setHandleWidth(4)
             s.setStyleSheet("QSplitter::handle{background: #222222;}")
             # palette = s.palette()
             # palette.setColor(QtGui.QPalette.ColorRole.Light, QtGui.QColor("yellow"))
             # s.setPalette(palette)
             # print(s.handleWidth())
             # pass
-        self.layout().addWidget(self._splitters[0])
+        layout.addWidget(self._splitters[0])
         for i, j in ((0, 1), (1, 2), (1, 3), (0, 4), (4, 5), (4, 6)):
             self._splitters[i].addWidget(self._splitters[j])
         _sync_splitters(self._splitters[1], self._splitters[4])
 
         self.cursor_colors: list[QtGui.QColor] = [self.COLORS[0]]
 
         self._colorbar = ItoolColorBar(self)
-        self.layout().addWidget(self._colorbar)
+        layout.addWidget(self._colorbar)
         self._colorbar.setVisible(False)
 
         pkw = {"image_cls": image_cls, "plotdata_cls": plotdata_cls}
-        self.manual_limits: dict[str | list[float]] = {}
+        self.manual_limits: dict[str, list[list[float]]] = {}
         self._plots: tuple[ItoolGraphicsLayoutWidget, ...] = (
             ItoolGraphicsLayoutWidget(self, image=True, display_axis=(0, 1), **pkw),
             ItoolGraphicsLayoutWidget(self, display_axis=(0,), **pkw),
             ItoolGraphicsLayoutWidget(self, display_axis=(1,), is_vertical=True, **pkw),
             ItoolGraphicsLayoutWidget(self, display_axis=(2,), **pkw),
             ItoolGraphicsLayoutWidget(self, image=True, display_axis=(0, 2), **pkw),
             ItoolGraphicsLayoutWidget(self, image=True, display_axis=(2, 1), **pkw),
@@ -410,27 +420,27 @@
             self._splitters[2].addWidget(self._plots[i])
         for i in (6, 3, 7):
             self._splitters[3].addWidget(self._plots[i])
         self._splitters[5].addWidget(self._plots[0])
         for i in (5, 2):
             self._splitters[6].addWidget(self._plots[i])
 
-        self.qapp: QtWidgets.QApplication = QtWidgets.QApplication.instance()
+        self.qapp = cast(QtWidgets.QApplication, QtWidgets.QApplication.instance())
         self.qapp.aboutToQuit.connect(self.on_close)
 
         cmap_reversed = False
 
         if isinstance(cmap, str):
             if cmap.endswith("_r"):
                 cmap = cmap[:-2]
                 cmap_reversed = True
             if cmap.startswith("cet_CET"):
                 cmap = cmap[4:]
 
-        self.colormap_properties: dict[str, str | pg.ColorMap | float | bool] = {
+        self.colormap_properties: ColorMapProperties = {
             "cmap": cmap,
             "gamma": gamma,
             "reversed": cmap_reversed,
             "highContrast": False,
             "zeroCentered": zeroCentered,
         }
 
@@ -484,23 +494,26 @@
     def slices(self) -> tuple[ItoolPlotItem, ...]:
         if self.data.ndim == 2:
             return ()
         elif self.data.ndim == 3:
             return tuple(self.get_axes(ax) for ax in (4, 5))
         elif self.data.ndim == 4:
             return tuple(self.get_axes(ax) for ax in (4, 5, 7))
+        else:
+            raise ValueError("Data must have 2 to 4 dimensions")
 
     @property
     def profiles(self) -> tuple[ItoolPlotItem, ...]:
         if self.data.ndim == 2:
-            profile_axes = (1, 2)
+            profile_axes = [1, 2]
         elif self.data.ndim == 3:
-            profile_axes = (1, 2, 3)
+            profile_axes = [1, 2, 3]
         else:
-            profile_axes = (1, 2, 3, 6)
+            profile_axes = [1, 2, 3, 6]
+
         return tuple(self.get_axes(ax) for ax in profile_axes)
 
     @property
     def main_image(self) -> ItoolPlotItem:
         """returns the main PlotItem"""
         return self.get_axes(0)
 
@@ -635,15 +648,15 @@
                     if d in data.dims
                 ]
             self._data = data.assign_coords({d: np.rad2deg(data[d]) for d in conv_dims})
 
         if hasattr(self, "_array_slicer"):
             self._array_slicer.set_array(self._data, reset=True)
         else:
-            self._array_slicer = ArraySlicer(self._data)
+            self._array_slicer: ArraySlicer = ArraySlicer(self._data)
 
         while self.n_cursors != n_cursors_old:
             self.array_slicer.add_cursor(update=False)
 
         self.connect_signals()
 
         self.adjust_layout()
@@ -809,15 +822,15 @@
         )
         for im in self._imageitems:
             im.set_pg_colormap(cmap, update=update)
         self.sigViewOptionChanged.emit()
 
     @QtCore.Slot(bool)
     def lock_levels(self, lock: bool):
-        self.levels_locked: bool = lock
+        self.levels_locked = lock
 
         if self.levels_locked:
             levels = self.array_slicer.limits
             self._colorbar.cb.setLimits(levels)
         for im in self._imageitems:
             if self.levels_locked:
                 im.setLevels(levels, update=False)
@@ -866,15 +879,15 @@
                   r[3] * r[2]
 
         """
 
         font = QtGui.QFont()
         font.setPointSizeF(float(font_size))
 
-        valid_axis: tuple[tuple[bool, bool, bool, bool]] = (
+        valid_axis: tuple[tuple[Literal[0, 1], ...], ...] = (
             (1, 0, 0, 1),
             (1, 1, 0, 0),
             (0, 0, 1, 1),
             (0, 1, 1, 0),
             (1, 0, 0, 0),
             (0, 0, 0, 1),
             (0, 1, 1, 0),
@@ -901,15 +914,15 @@
             ((r0 + r1 - d) / 2, (r0 + r1 - d) / 2, 0),
             (r3 * r2, r3 * (r0 + r1)),
             (r2,),
             ((r3 * (r0 + r1) - d) / r01, (r3 * (r0 + r1) - d) * r01),
         ]
         if self.data.ndim == 4:
             sizes[3] = (0, 0, (r0 + r1 - d))
-        for split, sz in zip(self._splitters, sizes):
+        for split, sz in zip(self._splitters, sizes, strict=True):
             split.setSizes(tuple(round(s * scale) for s in sz))
 
         for i, sel in enumerate(valid_axis):
             self.get_axes_widget(i).setVisible(i not in invalid)
             if i in invalid:
                 continue
             axes = self.get_axes(i)
@@ -936,45 +949,46 @@
         if value is None:
             value = not self.array_slicer.snap_to_data
         elif value == self.array_slicer.snap_to_data:
             return
         self.array_slicer.snap_to_data = value
         self.sigViewOptionChanged.emit()
 
-    def changeEvent(self, evt: QtCore.QEvent):
-        if evt.type() == QtCore.QEvent.Type.PaletteChange:
-            self.qapp.setStyle(self.qapp.style().name())
+    def changeEvent(self, evt: QtCore.QEvent | None):
+        if evt is not None and evt.type() == QtCore.QEvent.Type.PaletteChange:
+            style = self.qapp.style()
+            if style is not None:
+                self.qapp.setStyle(style.name())
         super().changeEvent(evt)
 
 
 class ItoolCursorLine(pg.InfiniteLine):
     def __init__(self, *args, **kargs):
         super().__init__(*args, **kargs)
-        self.qapp: QtWidgets.QApplication = QtWidgets.QApplication.instance()
 
     @property
     def plotItem(self) -> ItoolPlotItem:
         return self.parentItem().parentItem().parentItem()
 
-    def setBounds(self, bounds: Sequence[float], value: float | None = None):
+    def setBounds(self, bounds: Sequence[np.floating], value: float | None = None):
         if bounds[0] > bounds[1]:
             bounds = list(bounds)
             bounds.reverse()
         self.maxRange = bounds
         if value is None:
             value = self.value()
         self.setValue(value)
 
     def value(self) -> float:
         return float(super().value())
 
     def mouseDragEvent(self, ev: mouseEvents.MouseDragEvent):
         if (
             QtCore.Qt.KeyboardModifier.ControlModifier
-            not in self.qapp.keyboardModifiers()
+            not in QtWidgets.QApplication.keyboardModifiers()
         ):
             if self.movable and ev.button() == QtCore.Qt.MouseButton.LeftButton:
                 if ev.isStart():
                     self.moving = True
                     self.cursorOffset = self.pos() - self.mapToParent(
                         ev.buttonDownPos()
                     )
@@ -997,25 +1011,25 @@
         else:
             self.setMouseHover(False)
             self.plotItem.mouseDragEvent(ev)
 
     def mouseClickEvent(self, ev: mouseEvents.MouseClickEvent):
         if (
             QtCore.Qt.KeyboardModifier.ControlModifier
-            not in self.qapp.keyboardModifiers()
+            not in QtWidgets.QApplication.keyboardModifiers()
         ):
             super().mouseClickEvent(ev)
         else:
             self.setMouseHover(False)
             ev.ignore()
 
     def hoverEvent(self, ev):
         if (
             QtCore.Qt.KeyboardModifier.ControlModifier
-            not in self.qapp.keyboardModifiers()
+            not in QtWidgets.QApplication.keyboardModifiers()
         ):
             super().hoverEvent(ev)
         else:
             self.setMouseHover(False)
 
 
 class ItoolCursorSpan(pg.LinearRegionItem):
@@ -1034,15 +1048,15 @@
 
 class ItoolDisplayObject:
     def __init__(self, axes, cursor: int | None = None):
         self.axes = axes
         if cursor is None:
             cursor = 0
         self._cursor_index = int(cursor)
-        self.qapp: QtGui.QGuiApplication = QtGui.QGuiApplication.instance()
+        self.qapp = QtGui.QGuiApplication.instance()
 
     @property
     def display_axis(self):
         return self.axes.display_axis
 
     @property
     def slicer_area(self) -> ImageSlicerArea:
@@ -1113,21 +1127,27 @@
             self.cursor_index, self.display_axis
         )
         self.setImage(
             image=img, rect=rect, autoLevels=not self.slicer_area.levels_locked
         )
 
     def mouseDragEvent(self, ev: mouseEvents.MouseDragEvent):
-        if QtCore.Qt.KeyboardModifier.ControlModifier in self.qapp.keyboardModifiers():
+        if (
+            QtCore.Qt.KeyboardModifier.ControlModifier
+            in QtWidgets.QApplication.keyboardModifiers()
+        ):
             ev.ignore()
         else:
             super().mouseDragEvent(ev)
 
     def mouseClickEvent(self, ev: mouseEvents.MouseClickEvent):
-        if QtCore.Qt.KeyboardModifier.ControlModifier in self.qapp.keyboardModifiers():
+        if (
+            QtCore.Qt.KeyboardModifier.ControlModifier
+            in QtWidgets.QApplication.keyboardModifiers()
+        ):
             ev.ignore()
         else:
             super().mouseClickEvent(ev)
 
 
 class ItoolPlotItem(pg.PlotItem):
     sigDragged = QtCore.Signal(object, object)
@@ -1177,22 +1197,24 @@
         self.proxy = pg.SignalProxy(
             self.sigDragged,
             delay=1 / 60,
             rateLimit=60,
             slot=self.process_drag,
         )
         if self.slicer_area.bench:
-            self._time_start = None
-            self._time_end = None
-            self._single_queue = collections.deque([0], maxlen=9)
-            self._next_queue = collections.deque([0], maxlen=9)
+            self._time_start: float | None = None
+            self._time_end: float | None = None
+            self._single_queue = collections.deque([0.0], maxlen=9)
+            self._next_queue = collections.deque([0.0], maxlen=9)
 
     @property
-    def axis_dims(self) -> list[str]:
-        dim_list = [self.slicer_area.data.dims[ax] for ax in self.display_axis]
+    def axis_dims(self) -> list[str | None]:
+        dim_list: list[str | None] = [
+            str(self.slicer_area.data.dims[ax]) for ax in self.display_axis
+        ]
         if not self.is_image:
             if self.slicer_data_items[-1].is_vertical:
                 dim_list = [None, *dim_list]
             else:
                 dim_list = [*dim_list, None]
         return dim_list
 
@@ -1200,29 +1222,32 @@
     def is_independent(self) -> bool:
         return self.vb.state["linkedViews"] == [None, None]
 
     def refresh_manual_range(self):
         if self.is_independent:
             return
         for dim, auto, rng in zip(
-            self.axis_dims, self.vb.state["autoRange"], self.vb.state["viewRange"]
+            self.axis_dims,
+            self.vb.state["autoRange"],
+            self.vb.state["viewRange"],
+            strict=True,
         ):
             if dim is not None:
                 if auto:
                     self.slicer_area.manual_limits.pop("dim", None)
                 else:
                     self.slicer_area.manual_limits[dim] = rng
 
     def update_manual_range(self):
         if self.is_independent:
             return
         self.set_range_from(self.slicer_area.manual_limits)
 
     def set_range_from(self, limits: dict[str, list[float]], **kwargs):
-        for dim, key in zip(self.axis_dims, ("xRange", "yRange")):
+        for dim, key in zip(self.axis_dims, ("xRange", "yRange"), strict=True):
             if dim is not None:
                 try:
                     kwargs[key] = limits[dim]
                 except KeyError:
                     pass
         if len(kwargs) != 0:
             self.setRange(**kwargs)
@@ -1248,15 +1273,15 @@
         else:
             ev.ignore()
 
     def process_drag(
         self, sig: tuple[mouseEvents.MouseDragEvent, QtCore.Qt.KeyboardModifier]
     ):
         if self.slicer_area.bench:
-            if self._time_end is not None:
+            if self._time_end is not None and self._time_start is not None:
                 self._single_queue.append(1 / (self._time_end - self._time_start))
             self._time_end = self._time_start
             self._time_start = time.perf_counter()
             if self._time_end is not None:
                 self._next_queue.append(1 / (self._time_start - self._time_end))
             print(
                 "\x1b[2K\x1b[1A\x1b[2K"
@@ -1348,15 +1373,15 @@
                     pen=pg.mkPen(clr_span_edge),
                     brush=pg.mkBrush(clr_span),
                 )
             )
 
         self.cursor_lines.append({})
         self.cursor_spans.append({})
-        for c, s, ax in zip(cursors, spans, self.display_axis):
+        for c, s, ax in zip(cursors, spans, self.display_axis, strict=False):
             self.cursor_lines[-1][ax] = c
             self.cursor_spans[-1][ax] = s
             self.addItem(c)
             c.setZValue(10)
             self.addItem(s)
             s.setZValue(9)
             c.sigDragged.connect(
@@ -1396,15 +1421,17 @@
                     axis, value, update=True, uniform=True, cursor=i
                 )
 
     def remove_cursor(self, index: int):
         item = self.slicer_data_items.pop(index)
         self.removeItem(item)
         for line, span in zip(
-            self.cursor_lines.pop(index).values(), self.cursor_spans.pop(index).values()
+            self.cursor_lines.pop(index).values(),
+            self.cursor_spans.pop(index).values(),
+            strict=True,
         ):
             self.removeItem(line)
             self.removeItem(span)
         for i, item in enumerate(self.slicer_data_items):
             item.cursor_index = i
 
     def refresh_cursor(self, cursor: int):
@@ -1445,15 +1472,17 @@
         self.vb.updateAutoRange()
 
     @QtCore.Slot()
     def refresh_labels(self):
         if self.is_image:
             label_kw = {
                 a: self._get_label_unit(i)
-                for a, i in zip(("top", "bottom", "left", "right"), (0, 0, 1, 1))
+                for a, i in zip(
+                    ("top", "bottom", "left", "right"), (0, 0, 1, 1), strict=True
+                )
                 if self.getAxis(a).isVisible()
             }
         else:
             label_kw = {}
 
             if self.slicer_data_items[-1].is_vertical:
                 valid_ax = ("left", "right")
@@ -1536,15 +1565,15 @@
 
     @property
     def array_slicer(self) -> ArraySlicer:
         return self.slicer_area.array_slicer
 
 
 class ItoolColorBarItem(BetterColorBarItem):
-    def __init__(self, slicer_area: ImageSlicerArea | None = None, **kwargs):
+    def __init__(self, slicer_area: ImageSlicerArea, **kwargs):
         self._slicer_area = slicer_area
         kwargs.setdefault(
             "axisItems",
             {a: BetterAxisItem(a) for a in ("left", "right", "top", "bottom")},
         )
         super().__init__(**kwargs)
 
@@ -1568,22 +1597,22 @@
         self._span.blockSignals(False)
         self._span.sigRegionChanged.connect(self.level_change)
         self._span.sigRegionChangeFinished.connect(self.level_change_fin)
         self.color_changed()
 
 
 class ItoolColorBar(pg.PlotWidget):
-    def __init__(self, slicer_area: ImageSlicerArea | None = None, **cbar_kw):
+    def __init__(self, slicer_area: ImageSlicerArea, **cbar_kw):
         super().__init__(
             parent=slicer_area, plotItem=ItoolColorBarItem(slicer_area, **cbar_kw)
         )
         self.scene().sigMouseClicked.connect(self.mouseDragEvent)
 
     @property
-    def cb(self) -> BetterColorBarItem:
+    def cb(self) -> ItoolColorBarItem:
         return self.plotItem
 
     def set_dimensions(
         self,
         width: int = 30,
         horiz_pad: int | None = None,
         vert_pad: int | None = None,
```

### Comparing `erlab-2.3.0/src/erlab/interactive/imagetool/fastbinning.py` & `erlab-2.3.1/src/erlab/interactive/imagetool/fastbinning.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This module provides a fast, parallelized version of nanmean that supports multiple axes
 based on numba. Enables efficient real-time multidimensional binning.
 
 """
 
 __all__ = ["fast_nanmean"]
 
-from collections.abc import Iterable
+from collections.abc import Collection
 
 import numba
 import numba.core.registry
 import numba.typed
 import numbagg
 import numpy as np
 import numpy.typing as npt
@@ -311,16 +311,16 @@
         frozenset({0, 2, 3}): _nanmean_4_023,
         frozenset({1, 2, 3}): _nanmean_4_123,
     },
 }
 
 
 def fast_nanmean(
-    a: npt.NDArray[np.float32 | np.float64], axis: int | Iterable[int] | None = None
-) -> npt.NDArray[np.float32 | np.float64] | float:
+    a: npt.NDArray[np.float32 | np.float64], axis: int | Collection[int] | None = None
+) -> npt.NDArray[np.float32 | np.float64] | np.float64:
     """A fast, parallelized arithmetic mean for floating point arrays that ignores NaNs.
 
     Parameters
     ----------
     a
         A numpy array of floats.
     axis
@@ -341,27 +341,27 @@
     used. This function does not keep the input dimensions, i.e., the output is
     squeezed.
 
     """
     if a.ndim == 1 or axis is None:
         return _nanmean_all(a)
     elif a.ndim > 4:
-        return np.ascontiguousarray(numbagg.nanmean(a, axis))
-    if hasattr(axis, "__iter__"):
+        return np.ascontiguousarray(numbagg.nanmean(a, axis))  # type: ignore[arg-type]
+    if isinstance(axis, Collection):
         if len(axis) == a.ndim:
             return _nanmean_all(a)
         axis = frozenset(x % a.ndim for x in axis)
     else:
         axis = axis % a.ndim
     return nanmean_funcs[a.ndim][axis](a).astype(a.dtype)
 
 
 def _fast_nanmean_skipcheck(
-    a: npt.NDArray[np.float32 | np.float64], axis: int | Iterable[int]
-) -> npt.NDArray[np.float32 | np.float64] | float:
+    a: npt.NDArray[np.float32 | np.float64], axis: int | Collection[int]
+) -> npt.NDArray[np.float32 | np.float64] | np.float64:
     """A version of `fast_nanmean` with near-zero overhead. Meant for internal use.
 
     Strict assumptions on the input parameters allow skipping some checks.
 
     Parameters
     ----------
     a
@@ -373,22 +373,12 @@
 
     Returns
     -------
     numpy.ndarray or float
         The calculated mean. The output array is always C-contiguous.
 
     """
-    if hasattr(axis, "__iter__"):
+    if isinstance(axis, Collection):
         if len(axis) == a.ndim:
             return _nanmean_all(a)
         axis = frozenset(axis)
     return nanmean_funcs[a.ndim][axis](a).astype(a.dtype)
-
-
-if __name__ == "__main__":
-    for nd, funcs in nanmean_funcs.items():
-        x = np.random.RandomState(42).randn(*((30,) * nd))
-        for axis, func in funcs.items():
-            if isinstance(axis, frozenset):
-                axis = tuple(axis)
-            if not np.allclose(np.nanmean(x, axis), fast_nanmean(x, axis)):
-                print(func)
```

### Comparing `erlab-2.3.0/src/erlab/interactive/imagetool/slicer.py` & `erlab-2.3.1/src/erlab/interactive/imagetool/slicer.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import numpy as np
 import numpy.typing as npt
 from qtpy import QtCore
 
 from erlab.interactive.imagetool.fastbinning import _fast_nanmean_skipcheck
 
 if TYPE_CHECKING:
-    from collections.abc import Sequence
+    from collections.abc import Sequence, Hashable
 
     import xarray as xr
 
 VALID_NDIM = (2, 3, 4)
 
 _signature_array_rect = [
     numba.types.UniTuple(numba.float32, 4)(
@@ -50,16 +50,16 @@
     lims: tuple[tuple[np.float32, np.float32], ...],
     incs: tuple[np.float32, ...],
 ) -> tuple[np.float32, np.float32, np.float32, np.float32]:
     x = lims[i][0] - incs[i]
     y = lims[j][0] - incs[j]
     w = lims[i][-1] - x
     h = lims[j][-1] - y
-    x += 0.5 * incs[i]
-    y += 0.5 * incs[j]
+    x += np.float32(0.5 * incs[i])
+    y += np.float32(0.5 * incs[j])
     return x, y, w, h
 
 
 @numba.njit(_signature_index_of_value, cache=True)
 def _index_of_value(
     axis: int,
     val: np.floating,
@@ -97,15 +97,17 @@
 @numba.njit(
     [
         numba.int64(numba.float32[::1], numba.float32),
         numba.int64(numba.float64[::1], numba.float64),
     ],
     cache=True,
 )
-def _index_of_value_nonuniform(arr: npt.NDArray[np.float32], val: np.float32) -> int:
+def _index_of_value_nonuniform(
+    arr: npt.NDArray[np.float32], val: np.float32
+) -> np.int_:
     return np.searchsorted((arr[:-1] + arr[1:]) / 2, val)
 
 
 class ArraySlicer(QtCore.QObject):
     """Internal class used to slice a :class:`xarray.DataArray` rapidly.
 
     Computes binned line and image profiles from multiple cursors. Also handles the data
@@ -142,15 +144,14 @@
     sigIndexChanged = QtCore.Signal(int, object)  #: :meta private:
     sigBinChanged = QtCore.Signal(int, tuple)  #: :meta private:
     sigCursorCountChanged = QtCore.Signal(int)  #: :meta private:
     sigShapeChanged = QtCore.Signal()  #: :meta private:
 
     def __init__(self, xarray_obj: xr.DataArray):
         super().__init__()
-        self._obj: xr.DataArray | None = None
         self.set_array(xarray_obj, validate=True, reset=True)
 
     @property
     def n_cursors(self) -> int:
         """The number of cursors."""
         return len(self._bins)
 
@@ -201,37 +202,37 @@
     @functools.cached_property
     def data_vals_T(self) -> npt.NDArray[np.floating]:
         return _transposed(self._obj.values)
 
     # Benchmarks result in 10~20x slower speeds for bottleneck and numbagg compared to
     # numpy on arm64 mac with Accelerate BLAS. Needs confirmation on intel systems.
     @functools.cached_property
-    def nanmax(self) -> np.floating:
-        return np.nanmax(self._obj.values)
+    def nanmax(self) -> float:
+        return float(np.nanmax(self._obj.values))
 
     @functools.cached_property
-    def nanmin(self) -> np.floating:
-        return np.nanmin(self._obj.values)
+    def nanmin(self) -> float:
+        return float(np.nanmin(self._obj.values))
 
     @functools.cached_property
-    def absnanmax(self) -> np.floating:
+    def absnanmax(self) -> float:
         return max(abs(self.nanmin), abs(self.nanmax))
 
     @functools.cached_property
-    def absnanmin(self) -> np.floating:
+    def absnanmin(self) -> float:
         mn, mx = self.nanmin, self.nanmax
         if mn * mx <= np.float32(0.0):
-            return np.float32(0.0)
+            return 0.0
         elif mn < np.float32(0.0):
             return -mx
         else:
             return mn
 
     @property
-    def limits(self) -> tuple[np.floating, np.floating]:
+    def limits(self) -> tuple[float, float]:
         """Returns the global minima and maxima of the data."""
         return self.nanmin, self.nanmax
 
     @staticmethod
     def validate_array(data: xr.DataArray) -> xr.DataArray:
         """Validates a given :class:`xarray.DataArray`.
 
@@ -261,15 +262,15 @@
             data = data.astype(np.float64)
 
         new_dims: tuple[str, ...] = ("kx", "ky")
         if all(d in data.dims for d in new_dims):
             # if data has kx and ky axis, transpose
             if "eV" in data.dims:
                 new_dims += ("eV",)
-            new_dims += tuple(d for d in data.dims if d not in new_dims)
+            new_dims += tuple(str(d) for d in data.dims if d not in new_dims)
             data = data.transpose(*new_dims)
 
         nonuniform_dims: list[str] = [
             str(d) for d in data.dims if not _is_uniform(data[d].values)
         ]
         for d in nonuniform_dims:
             data = data.assign_coords(
@@ -300,39 +301,40 @@
     def clear_cache(self):
         self.clear_dim_cache()
         self.clear_val_cache()
 
     def set_array(
         self, xarray_obj: xr.DataArray, validate: bool = True, reset: bool = False
     ) -> None:
-        del self._obj
+        if hasattr(self, "_obj"):
+            del self._obj
 
         if validate:
             self._obj: xr.DataArray = self.validate_array(xarray_obj)
         else:
-            self._obj: xr.DataArray = xarray_obj
-        self._nonuniform_axes: list[str] = [
+            self._obj = xarray_obj
+        self._nonuniform_axes: list[int] = [
             i for i, d in enumerate(self._obj.dims) if str(d).endswith("_idx")
         ]
 
         self.clear_dim_cache()
         if validate:
             self.clear_val_cache()
 
         if reset:
             self._bins: list[list[int]] = [[1] * self._obj.ndim]
             self._indices: list[list[int]] = [
                 [s // 2 - (1 if s % 2 == 0 else 0) for s in self._obj.shape]
             ]
             self._values: list[list[np.float32]] = [
-                [c[i] for c, i in zip(self.coords, self._indices[0])]
+                [c[i] for c, i in zip(self.coords, self._indices[0], strict=True)]
             ]
             self.snap_to_data: bool = False
 
-    def values_of_dim(self, dim: str) -> npt.NDArray[np.float32]:
+    def values_of_dim(self, dim: Hashable) -> npt.NDArray[np.float32]:
         """Fast equivalent of :code:`self._obj[dim].values`.
 
         Returns the cached pointer of the underlying coordinate array, achieving a ~80x
         speedup. This should work most of the time since we only assume floating point
         values, but does require further testing. May break for future versions of
         :obj:`pandas` or :obj:`xarray`. See Notes.
 
@@ -349,21 +351,21 @@
         -----
         Looking at the implementation, I think this may return a pandas array in some
         cases, but I'm not sure so I'll just leave it this way. When something breaks,
         replacing with :code:`self._obj._coords[dim]._data.array.array._ndarray` may
         do the trick.
 
         """
-        return self._obj._coords[dim]._data.array._data
+        return self._obj._coords[dim]._data.array._data  # type: ignore[union-attr]
 
     def add_cursor(self, like_cursor: int = -1, update: bool = True) -> None:
         self._bins.append(list(self.get_bins(like_cursor)))
         new_ind = self.get_indices(like_cursor)
         self._indices.append(list(new_ind))
-        self._values.append([c[i] for c, i in zip(self.coords, new_ind)])
+        self._values.append([c[i] for c, i in zip(self.coords, new_ind, strict=True)])
         if update:
             self.sigCursorCountChanged.emit(self.n_cursors)
 
     def remove_cursor(self, index: int, update: bool = True) -> None:
         if self.n_cursors == 1:
             raise ValueError("There must be at least one cursor.")
         self._bins.pop(index)
@@ -576,15 +578,16 @@
             return _index_of_value_nonuniform(self.coords[axis], value)
 
     def isel_args(
         self, cursor: int, disp: Sequence[int], int_if_one: bool = False
     ) -> dict[str, slice | int]:
         axis = sorted(set(range(self._obj.ndim)) - set(disp))
         return {
-            self._obj.dims[ax]: self._bin_slice(cursor, ax, int_if_one) for ax in axis
+            str(self._obj.dims[ax]): self._bin_slice(cursor, ax, int_if_one)
+            for ax in axis
         }
 
     def qsel_args(self, cursor: int, disp: Sequence[int]) -> dict:
         out: dict[str, float] = {}
         binned = self.get_binned(cursor)
 
         for dim, selector in self.isel_args(cursor, disp, int_if_one=True).items():
@@ -634,25 +637,25 @@
         dict_repr: str = ""
         for k, v in self.isel_args(cursor, disp, int_if_one=True).items():
             dict_repr += f"{k}={v!s}, "
         dict_repr = dict_repr.rstrip(", ")
         return f".isel({dict_repr})"
 
     def xslice(self, cursor: int, disp: Sequence[int]) -> xr.DataArray:
-        isel_kw: dict[str, slice] = self.isel_args(cursor, disp, int_if_one=False)
+        isel_kw = self.isel_args(cursor, disp, int_if_one=False)
         binned_coord_average: dict[str, xr.DataArray] = {
-            k: self._obj[k][isel_kw[k]].mean()
-            for k, v in zip(self._obj.dims, self.get_binned(cursor))
+            str(k): self._obj[k][isel_kw[str(k)]].mean()
+            for k, v in zip(self._obj.dims, self.get_binned(cursor), strict=True)
             if v
         }
         return (
-            self._obj.isel(**isel_kw)
+            self._obj.isel(isel_kw)
             .squeeze()
             .mean(binned_coord_average.keys())
-            .assign_coords(**binned_coord_average)
+            .assign_coords(binned_coord_average)
         )
 
     @QtCore.Slot(int, tuple, result=np.ndarray)
     def slice_with_coord(
         self, cursor: int, disp: Sequence[int]
     ) -> tuple[
         tuple[np.float32, np.float32, np.float32, np.float32] | npt.NDArray[np.float32],
@@ -669,14 +672,16 @@
         elif len(axis) == 1:
             return self._bin_along_axis(cursor, axis[0])
         else:
             return self._bin_along_multiaxis(cursor, axis)
 
     def span_bounds(self, cursor: int, axis: int) -> npt.NDArray[np.float32]:
         slc = self._bin_slice(cursor, axis)
+        if isinstance(slc, int):
+            return self.coords_uniform[axis][slc : slc + 1]
         lb = max(0, slc.start)
         ub = min(self._obj.shape[axis] - 1, slc.stop - 1)
         return self.coords_uniform[axis][[lb, ub]]
 
     def _bin_slice(
         self, cursor: int, axis: int, int_if_one: bool = False
     ) -> slice | int:
```

### Comparing `erlab-2.3.0/src/erlab/interactive/kspace.py` & `erlab-2.3.1/src/erlab/interactive/kspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 )
 from erlab.interactive.imagetool import ImageTool
 from erlab.interactive.utilities import copy_to_clipboard, gen_function_code, xImageItem
 from erlab.plotting.bz import get_bz_edge
 
 
 class KspaceToolGUI(
-    *uic.loadUiType(os.path.join(os.path.dirname(__file__), "ktool.ui"))
+    *uic.loadUiType(os.path.join(os.path.dirname(__file__), "ktool.ui"))  # type: ignore[misc]
 ):
     def __init__(self):
         # Start the QApplication if it doesn't exist
         self.qapp = QtCore.QCoreApplication.instance()
         if not self.qapp:
             self.qapp = QtWidgets.QApplication(sys.argv)
         self.qapp.setStyle("Fusion")
@@ -151,15 +151,17 @@
         super().__init__()
 
         self._argnames = {}
 
         if data_name is None:
             try:
                 self._argnames["data"] = varname.argname(
-                    "data", func=self.__init__, vars_only=False
+                    "data",
+                    func=self.__init__,  # type: ignore[misc]
+                    vars_only=False,
                 )
             except varname.VarnameRetrievingError:
                 self._argnames["data"] = "data"
         else:
             self._argnames["data"] = data_name
 
         self.data: xr.DataArray = data.copy(deep=True)
@@ -256,19 +258,19 @@
         if self.data.kspace.has_hv:
             self.data.kspace.inner_potential = self._offset_spins["V0"].value()
 
         wait_dialog = QtWidgets.QDialog(self)
         wait_dialog.setLayout(QtWidgets.QVBoxLayout())
         wait_dialog.layout().addWidget(QtWidgets.QLabel("Converting..."))
         wait_dialog.open()
-        itool = ImageTool(
+        self._itool = ImageTool(
             self.data.kspace.convert(bounds=self.bounds, resolution=self.resolution)
         )
         wait_dialog.close()
-        itool.show()
+        self._itool.show()
 
     def copy_code(self):
         arg_dict = {}
         if self.bounds is not None:
             arg_dict["bounds"] = self.bounds
         if self.resolution is not None:
             arg_dict["resolution"] = self.resolution
@@ -298,15 +300,18 @@
 
         copy_to_clipboard(out_lines)
 
     @property
     def bounds(self) -> dict[str, tuple[float, float]] | None:
         if self.bounds_group.isChecked():
             return {
-                k: tuple(self._bound_spins[f"{k}{j}"].value() for j in range(2))
+                k: (
+                    self._bound_spins[f"{k}0"].value(),
+                    self._bound_spins[f"{k}1"].value(),
+                )
                 for k in self.data.kspace.momentum_axes
             }
         else:
             return None
 
     @property
     def resolution(self) -> dict[str, float] | None:
@@ -421,9 +426,11 @@
             data_name = varname.argname("data", func=ktool, vars_only=False)
         except varname.VarnameRetrievingError:
             data_name = "data"
     return KspaceTool(data, data_name=data_name)
 
 
 if __name__ == "__main__":
-    dat = erlab.io.load_hdf5("/Users/khan/2210_ALS_f0008.h5")
+    from typing import cast
+
+    dat = cast(xr.DataArray, erlab.io.load_hdf5("/Users/khan/2210_ALS_f0008.h5"))
     win = ktool(dat)
```

### Comparing `erlab-2.3.0/src/erlab/interactive/ktool.ui` & `erlab-2.3.1/src/erlab/interactive/ktool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/interactive/masktool.py` & `erlab-2.3.1/src/erlab/interactive/masktool.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import sys
-
 import pyqtgraph as pg
-from pyqtgraph.Qt import QtCore, QtWidgets
+from pyqtgraph.Qt import QtCore
 
 from erlab.interactive.utilities import AnalysisWindow, ParameterGroup
 
 __all__ = ["masktool"]
 
 
 class PolyLineROIControls(ParameterGroup):
@@ -81,27 +79,7 @@
         else:
             self.images[0].setDataArray(new_arr)
         # else:
         # self.images[0].setDataArray(new_arr)
         # self.images[0].setImage(self.data.isel({dim_z:self.cursor.widgets["slider"].value()}).values)
 
         # self.cursor.values["slider"]
-
-
-if __name__ == "__main__":
-    import erlab.io
-
-    qapp = QtWidgets.QApplication.instance()
-    if not qapp:
-        qapp = QtWidgets.QApplication(sys.argv)
-    qapp.setStyle("Fusion")
-
-    ds = erlab.io.load_igor_h5(
-        "/Users/khan/Documents/ERLab/CsV3Sb5/220630_ALS_Kagome_nesting/maps.h5"
-    )
-    map3 = ds["Map3"].rename(phony_dim_0="kx", phony_dim_1="ky", phony_dim_2="eV")
-    # map6 = ds["Map6"].rename(phony_dim_0="kx", phony_dim_3="ky", phony_dim_4="eV")
-    ct = masktool(map3)
-    ct.show()
-    ct.activateWindow()
-    ct.raise_()
-    qapp.exec()
```

### Comparing `erlab-2.3.0/src/erlab/interactive/utilities.py` & `erlab-2.3.1/src/erlab/interactive/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """Various helper functions and extensions to pyqtgraph."""
 
 from __future__ import annotations
 
 import re
 import sys
+import types
 import warnings
-from typing import Any, Literal
+from typing import TYPE_CHECKING, Any, Literal, cast
 
 import numpy as np
 import numpy.typing as npt
 import pyperclip
 import pyqtgraph as pg
 import xarray as xr
 from qtpy import QtCore, QtGui, QtWidgets
-from superqt import QDoubleSlider
 
 from erlab.interactive.colors import BetterImageItem, pg_colormap_powernorm
 
+if TYPE_CHECKING:
+    from collections.abc import Mapping
+
 __all__ = [
     "AnalysisWidgetBase",
     "AnalysisWindow",
     "BetterAxisItem",
     "BetterSpinBox",
     "DictMenuBar",
     "ParameterGroup",
@@ -247,15 +250,17 @@
             QtWidgets.QSizePolicy.Policy.Fixed,
         )
         self.editingFinished.connect(self.editingFinishedEvent)
         self._updateHeight()
         self._updateWidth()
 
         if self.isReadOnly():
-            self.lineEdit().setReadOnly(True)
+            line_edit = self.lineEdit()
+            if line_edit is not None:
+                line_edit.setReadOnly(True)
             self.setButtonSymbols(self.ButtonSymbols.NoButtons)
         self.setValue(self.value())
 
     def setDecimals(self, decimals):
         self._decimals = decimals
 
     def decimals(self):
@@ -512,14 +517,15 @@
                             r"1E\+?(\-?)0?(\d?\d)",
                             f"{1.0 / self.autoSIPrefixScale:.3G}",
                         ).groups()
                     )
                     for k, v in zip(
                         ("0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "-"),
                         ("⁰", "¹", "²", "³", "⁴", "⁵", "⁶", "⁷", "⁸", "⁹", "⁻"),
+                        strict=True,
                     ):
                         units = units.replace(k, v)
                     units = f"10{units}"
                 except AttributeError:
                     units = f"{1.0 / self.autoSIPrefixScale:.3G}"
                 units = f"(×{units})"
 
@@ -561,16 +567,17 @@
         fixed: bool = False,
         label: str | None = None,
         show_label: bool = True,
     ):
         super().__init__()
         if spin_kw is None:
             spin_kw = {}
-        self.layout = QtWidgets.QHBoxLayout(self)
-        self.layout.setContentsMargins(0, 0, 0, 0)
+        layout = QtWidgets.QHBoxLayout(self)
+        self.setLayout(layout)
+        layout.setContentsMargins(0, 0, 0, 0)
 
         self.param_name = name
         self._prefix = ""
         if label is None:
             label = self.param_name
         self.label = QtWidgets.QLabel(label)
         spin_kw.setdefault("keyboardTracking", False)
@@ -587,22 +594,23 @@
         )
         self.spin_lb.setSizePolicy(
             QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Fixed
         )
         self.spin_ub.setSizePolicy(
             QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Fixed
         )
-        self.check = QtWidgets.QCheckBox(toolTip="Fixed")
+        self.check = QtWidgets.QCheckBox()
+        self.check.setToolTip("Fix parameter")
 
         if show_label:
-            self.layout.addWidget(self.label)
-        self.layout.addWidget(self.spin_value)
-        self.layout.addWidget(self.spin_lb)
-        self.layout.addWidget(self.spin_ub)
-        self.layout.addWidget(self.check)
+            layout.addWidget(self.label)
+        layout.addWidget(self.spin_value)
+        layout.addWidget(self.spin_lb)
+        layout.addWidget(self.spin_ub)
+        layout.addWidget(self.check)
 
         for spin in (self.spin_value, self.spin_lb, self.spin_ub):
             spin.valueChanged.connect(lambda: self.sigParamChanged.emit())
         self.spin_lb.valueChanged.connect(self._refresh_bounds)
         self.spin_ub.valueChanged.connect(self._refresh_bounds)
         self.check.stateChanged.connect(self.setFixed)
 
@@ -807,39 +815,52 @@
             "b": dict(qwtype="dblspin", range=(0, 2), singleStep=0.04),
             "c": QtWidgets.QSlider(range=(0, 10000))
         }
     )
 
     """
 
-    VALID_QWTYPE: dict[str, QtWidgets.QWidget] = {
-        "spin": QtWidgets.QSpinBox,
-        "dblspin": QtWidgets.QDoubleSpinBox,
-        "btspin": BetterSpinBox,
-        "slider": QtWidgets.QSlider,
-        "dblslider": QDoubleSlider,
-        "chkbox": QtWidgets.QCheckBox,
-        "pushbtn": QtWidgets.QPushButton,
-        "chkpushbtn": QtWidgets.QPushButton,
-        "combobox": QtWidgets.QComboBox,
-        "fitparam": FittingParameterWidget,
-    }  # : Dictionary of valid widgets that can be added.
+    VALID_QWTYPE: Mapping[str, type[QtWidgets.QWidget]] = types.MappingProxyType(
+        {
+            "spin": QtWidgets.QSpinBox,
+            "dblspin": QtWidgets.QDoubleSpinBox,
+            "btspin": BetterSpinBox,
+            "slider": QtWidgets.QSlider,
+            "chkbox": QtWidgets.QCheckBox,
+            "pushbtn": QtWidgets.QPushButton,
+            "chkpushbtn": QtWidgets.QPushButton,
+            "combobox": QtWidgets.QComboBox,
+            "fitparam": FittingParameterWidget,
+        }
+    )  # : Dictionary of valid widgets that can be added.
 
     sigParameterChanged: QtCore.SignalInstance = QtCore.Signal(dict)  #: :meta private:
 
-    def __init__(self, ncols: int = 1, groupbox_kw: dict | None = None, **kwargs):
+    def __init__(
+        self,
+        widgets: dict[str, dict] | None = None,
+        ncols: int = 1,
+        groupbox_kw: dict | None = None,
+        **widgets_kwargs,
+    ):
         if groupbox_kw is None:
             groupbox_kw = {}
         super().__init__(**groupbox_kw)
-        self.setLayout(QtWidgets.QGridLayout(self))
+        layout = QtWidgets.QGridLayout(self)
+        self.setLayout(layout)
 
         self.labels = []
         self.untracked = []
         self.widgets: dict[str, QtWidgets.QWidget] = {}
 
+        if widgets is not None:
+            kwargs = widgets
+        else:
+            kwargs = widgets_kwargs
+
         j = 0
         for i, (k, v) in enumerate(kwargs.items()):
             if isinstance(v, dict):
                 showlabel = v.pop("showlabel", k)
                 ind_eff = v.pop("colspan", 1)
                 if ind_eff == "ncols":
                     ind_eff = ncols
@@ -855,35 +876,34 @@
                     "Each value must be a QtWidgets.QWidget instance"
                     "or a dictionary of keyword arguments to getParameterWidget."
                 )
 
             self.labels.append(QtWidgets.QLabel(str(showlabel)))
             self.labels[i].setBuddy(self.widgets[k])
             if showlabel:
-                self.layout().addWidget(self.labels[i], j // ncols, 2 * (j % ncols))
-                self.layout().addWidget(
+                layout.addWidget(self.labels[i], j // ncols, 2 * (j % ncols))
+                layout.addWidget(
                     self.widgets[k], j // ncols, 2 * (j % ncols) + 1, 1, 2 * ind_eff - 1
                 )
             else:
-                self.layout().addWidget(
+                layout.addWidget(
                     self.widgets[k], j // ncols, 2 * (j % ncols), 1, 2 * ind_eff
                 )
             j += ind_eff
 
         self.global_connect()
 
     @staticmethod
     def getParameterWidget(
         qwtype: (
             Literal[
                 "spin",
                 "dblspin",
                 "btspin",
                 "slider",
-                "dblslider",
                 "chkbox",
                 "pushbtn",
                 "chkpushbtn",
                 "combobox",
                 "fitparam",
             ]
             | None
@@ -1050,15 +1070,14 @@
     @property
     def values(self) -> dict[str, float | int | bool]:
         return {k: self.widget_value(v) for k, v in self.widgets.items()}
 
     # "spin": QtWidgets.QSpinBox,
     # "dblspin": QtWidgets.QDoubleSpinBox,
     # "slider": QtWidgets.QSlider,
-    # "dblslider": QDoubleSlider,
     # "chkbox": QtWidgets.QCheckBox,
     # "pushbtn": QtWidgets.QPushButton,
     # "chkpushbtn": QtWidgets.QPushButton,
     # "combobox": QtWidgets.QComboBox,
 
 
 class ROIControls(ParameterGroup):
@@ -1130,23 +1149,25 @@
         return x0, y0, x1, y1
 
     def update_pos(self):
         self.widgets["x0"].setMaximum(self.widgets["x1"].value())
         self.widgets["y0"].setMaximum(self.widgets["y1"].value())
         self.widgets["x1"].setMinimum(self.widgets["x0"].value())
         self.widgets["y1"].setMinimum(self.widgets["y0"].value())
-        for pos, spin in zip(self.roi_limits, self.roi_spin):
+        for pos, spin in zip(self.roi_limits, self.roi_spin, strict=True):
             spin.blockSignals(True)
             spin.setValue(pos)
             spin.blockSignals(False)
 
     def modify_roi(self, x0=None, y0=None, x1=None, y1=None, update=True):
         lim_new = (x0, y0, x1, y1)
         lim_old = self.roi_limits
-        x0, y0, x1, y1 = ((f if f is not None else i) for i, f in zip(lim_old, lim_new))
+        x0, y0, x1, y1 = (
+            (f if f is not None else i) for i, f in zip(lim_old, lim_new, strict=True)
+        )
         xm, ym, xM, yM = self.roi.maxBounds.getCoords()
         x0, y0, x1, y1 = max(x0, xm), max(y0, ym), min(x1, xM), min(y1, yM)
         self.roi.setPos((x0, y0), update=False)
         self.roi.setSize((x1 - x0, y1 - y0), update=update)
 
     def draw_mode(self, toggle):
         vb = self.roi.parentItem().getViewBox()
@@ -1220,21 +1241,14 @@
                 vb._resetTarget()
                 vb.scaleBy(x=x, y=y, center=center)
                 vb.sigRangeChangedManually.emit(vb.state["mouseEnabled"])
 
         vb.mouseDragEvent = mouseDragEventCustom  # set to modified mouseDragEvent
 
 
-class PostInitCaller(type(QtWidgets.QMainWindow)):
-    def __call__(cls, *args, **kwargs):
-        obj = type.__call__(cls, *args, **kwargs)
-        obj.__post_init__()
-        return obj
-
-
 class AnalysisWindow(QtWidgets.QMainWindow):
     def __init__(
         self,
         data,
         title=None,
         layout="horizontal",
         data_is_input=True,
@@ -1314,17 +1328,17 @@
             self.qapp.exec()
 
     def addParameterGroup(self, *args, **kwargs):
         group = ParameterGroup(*args, **kwargs)
         self.controls.addWidget(group)
         return group
 
-    def closeEvent(self, event: QtGui.QCloseEvent) -> None:
-        cb = QtWidgets.QApplication.instance().clipboard()
-        if cb.text(cb.Mode.Clipboard) != "":
+    def closeEvent(self, event: QtGui.QCloseEvent | None) -> None:
+        cb = cast(QtWidgets.QApplication, QtWidgets.QApplication.instance()).clipboard()
+        if event is not None and cb is not None and cb.text(cb.Mode.Clipboard) != "":
             pyperclip.copy(cb.text(cb.Mode.Clipboard))
         return super().closeEvent(event)
 
 
 class AnalysisWidgetBase(pg.GraphicsLayoutWidget):
     """AnalysisWidgetBase
 
@@ -1364,18 +1378,20 @@
 
         for i in range(1, num_ax):
             if link in ("x", "both"):
                 self.axes[i].setXLink(self.axes[0])
             if link in ("y", "both"):
                 self.axes[i].setYLink(self.axes[0])
 
-    def initialize_layout(self, nax):
-        self.hists = [pg.HistogramLUTItem() for _ in range(nax)]
-        self.axes = [pg.PlotItem() for _ in range(nax)]
-        self.images = [xImageItem(axisOrder="row-major") for _ in range(nax)]
+    def initialize_layout(self, nax: int):
+        self.hists: pg.HistogramLUTItem = [pg.HistogramLUTItem() for _ in range(nax)]
+        self.axes: list[pg.PlotItem] = [pg.PlotItem() for _ in range(nax)]
+        self.images: list[xImageItem] = [
+            xImageItem(axisOrder="row-major") for _ in range(nax)
+        ]
         cmap = pg_colormap_powernorm("terrain", 1.0, N=6)
         for i in range(nax):
             self.addItem(self.axes[i], *self.get_axis_pos(i))
             self.addItem(self.hists[i], *self.get_hist_pos(i))
             self.axes[i].addItem(self.images[i])
             self.hists[i].setImageItem(self.images[i])
             self.hists[i].gradient.setColorMap(cmap)
@@ -1500,28 +1516,28 @@
 
     def refresh_all(self):
         self.set_input()
         self.refresh_output()
 
 
 class DictMenuBar(QtWidgets.QMenuBar):
-    def __init__(self, parent: QtWidgets.QWidget | None = ..., **kwargs) -> None:
+    def __init__(self, parent: QtWidgets.QWidget | None = None, **kwargs) -> None:
         super().__init__(parent)
 
         self.menu_dict: dict[str, QtWidgets.QMenu] = {}
         self.action_dict: dict[str, QtWidgets.QAction] = {}
 
         self.add_items(**kwargs)
 
     def __getattribute__(self, __name: str) -> Any:
         try:
             return super().__getattribute__(__name)
         except AttributeError:
             try:
-                out = self.menu_dict[__name]
+                out: Any = self.menu_dict[__name]
             except KeyError:
                 out = self.action_dict[__name]
             warnings.warn(
                 f"Menu or Action '{__name}' called as an attribute",
                 PendingDeprecationWarning,
                 stacklevel=2,
             )
@@ -1592,15 +1608,17 @@
             action.changed.connect(changed)
         return action
 
 
 if __name__ == "__main__":
     from scipy.ndimage import gaussian_filter  # , uniform_filter
 
-    qapp = QtWidgets.QApplication.instance()
+    qapp: QtWidgets.QApplication = cast(
+        QtWidgets.QApplication, QtWidgets.QApplication.instance()
+    )
     if not qapp:
         qapp = QtWidgets.QApplication(sys.argv)
     qapp.setStyle("Fusion")
 
     dat = (
         xr.open_dataarray(
             "/Users/khan/Documents/ERLab/CsV3Sb5/2021_Dec_ALS_CV3Sb5/Data/cvs_kxy_small.nc"
```

### Comparing `erlab-2.3.0/src/erlab/io/__init__.py` & `erlab-2.3.1/src/erlab/io/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
    :toctree: generated
 
    plugins
    dataloader
    utilities
    igor
    exampledata
+   characterization
 
 
 For a single session, it is very common to use only one type of loader for a single
 folder with all your data. Hence, the module provides a way to set a default loader for
 a session. This is done using the :func:`set_loader` function. The same can be done for
 the data directory using the :func:`set_data_dir` function.
```

### Comparing `erlab-2.3.0/src/erlab/io/dataloader.py` & `erlab-2.3.1/src/erlab/io/dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,57 +19,66 @@
 
 import contextlib
 import datetime
 import importlib
 import itertools
 import os
 import warnings
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, ClassVar, Self, cast
 
 import joblib
 import numpy as np
 import numpy.typing as npt
 import pandas
 import xarray as xr
 
 if TYPE_CHECKING:
-    from collections.abc import Iterable, Sequence
+    from collections.abc import Iterable, Mapping
+
+    DataFromSingleFile = xr.DataArray | xr.Dataset | list[xr.DataArray]
 
 
 def _is_uniform(arr: npt.NDArray) -> bool:
     dif = np.diff(arr)
     return np.allclose(dif, dif[0], rtol=3e-05, atol=3e-05, equal_nan=True)
 
 
-def _is_monotonic(arr: npt.NDArray) -> bool:
+def _is_monotonic(arr: npt.NDArray) -> np.bool_:
     dif = np.diff(arr)
     return np.all(dif >= 0) or np.all(dif <= 0)
 
 
 class ValidationError(Exception):
     """This exception is raised when the loaded data fails validation checks."""
 
 
 class ValidationWarning(UserWarning):
     """This warning is issued when the loaded data fails validation checks."""
 
 
+class LoaderNotFoundError(Exception):
+    """This exception is raised when a loader is not found in the registry."""
+
+    def __init__(self, key: str):
+        super().__init__(f"Loader for name or alias {key} not found in the registry")
+
+
 class LoaderBase:
     """Base class for all data loaders."""
 
-    name: str = None
+    name: str
     """
     Name of the loader. Using a unique and descriptive name is recommended. For easy
     access, it is recommended to use a name that passes :func:`str.isidentifier`.
     """
 
-    aliases: list[str] | None = None
+    aliases: Iterable[str] | None = None
     """List of alternative names for the loader."""
 
-    name_map: dict[str, str | Iterable[str]] = {}
+    name_map: ClassVar[dict[str, str | Iterable[str]]] = {}
     """
     Dictionary that maps **new** coordinate or attribute names to **original**
     coordinate or attribute names. If there are multiple possible names for a single
     attribute, the value can be passed as an iterable.
     """
 
     coordinate_attrs: tuple[str, ...] = ()
@@ -79,15 +88,15 @@
     Note
     ----
     Although the data loader tries to preserve the original attributes, the attributes
     given here, both before and after renaming, will be removed from attrs for
     consistency.
     """
 
-    additional_attrs: dict[str, str | int | float] = {}
+    additional_attrs: ClassVar[dict[str, str | int | float]] = {}
     """Additional attributes to be added to the data."""
 
     always_single: bool = True
     """
     If `True`, this indicates that all individual scans always lead to a single data
     file. No concatenation of data from multiple files will be performed.
     """
@@ -103,15 +112,15 @@
 
     @property
     def name_map_reversed(self) -> dict[str, str]:
         """A reversed version of the name_map dictionary."""
         return self.reverse_mapping(self.name_map)
 
     @staticmethod
-    def reverse_mapping(mapping: dict[str, str | Iterable[str]]) -> dict[str, str]:
+    def reverse_mapping(mapping: Mapping[str, str | Iterable[str]]) -> dict[str, str]:
         """Reverse the given mapping dictionary to form a one-to-one mapping.
 
         Parameters
         ----------
         mapping
             The mapping dictionary to be reversed.
 
@@ -264,14 +273,15 @@
 
         elif isinstance(val, list):
             return ", ".join(
                 [f"[{k}]×{len(tuple(g))}" for k, g in itertools.groupby(val)]
             )
 
         elif np.issubdtype(type(val), np.floating):
+            val = cast(np.floating, val)
             if val.is_integer():
                 return cls.formatter(np.int64(val))
             else:
                 return np.format_float_positional(val, precision=4, trim="-").replace(
                     "-", "−"
                 )
         elif np.issubdtype(type(val), np.integer):
@@ -307,16 +317,16 @@
         if len(hidden) > 0:
             style = style.hide(hidden, axis="columns")
 
         return style
 
     def load(
         self,
-        identifier: str | os.PathLike | int | None,
-        data_dir: str | os.PathLike | None = None,
+        identifier: str | int,
+        data_dir: str | None = None,
         **kwargs,
     ) -> xr.DataArray | xr.Dataset | list[xr.DataArray]:
         """Load ARPES data.
 
         Parameters
         ----------
         identifier
@@ -396,16 +406,14 @@
             data = self.load_single(identifier)
 
         data = self.post_process_general(data)
 
         if not self.skip_validate:
             self.validate(data)
 
-        data.attrs["data_loader_name"] = str(self.name)
-
         return data
 
     def summarize(
         self,
         data_dir: str | os.PathLike,
         usecache: bool = True,
         *,
@@ -463,27 +471,27 @@
 
         if not display:
             return df
 
         styled = self.get_styler(df)
 
         try:
-            shell = get_ipython().__class__.__name__  # type: ignore
+            shell = get_ipython().__class__.__name__  # type: ignore[name-defined]
             if display and (
                 shell in ["ZMQInteractiveShell", "TerminalInteractiveShell"]
             ):
-                from IPython.display import display
+                from IPython.display import display  # type: ignore[assignment]
 
                 with pandas.option_context(
                     "display.max_rows", len(df), "display.max_columns", len(df.columns)
                 ):
-                    display(styled)
+                    display(styled)  # type: ignore[misc]
 
                 if importlib.util.find_spec("ipywidgets"):
-                    display(self.isummarize(df=df))
+                    display(self.isummarize(df=df))  # type: ignore[misc]
 
                 return None
 
         except NameError:
             pass
 
         return styled
@@ -509,33 +517,33 @@
 
         """
         if not importlib.util.find_spec("ipywidgets"):
             raise ImportError(
                 "ipywidgets and IPython is required for interactive summaries"
             )
         if df is None:
-            kwargs.setdefault("display", False)
-            df = self.summarize(**kwargs)
+            kwargs["display"] = False
+            df = cast(pandas.DataFrame, self.summarize(**kwargs))
 
         import matplotlib.pyplot as plt
-        import erlab.plotting.erplot as eplt
-
         from ipywidgets import (
             HTML,
             Button,
             Dropdown,
             FloatSlider,
             HBox,
             Layout,
             Output,
             Select,
             VBox,
         )
         from ipywidgets.widgets.interaction import show_inline_matplotlib_plots
 
+        import erlab.plotting.erplot as eplt
+
         self._temp_data: xr.DataArray | None = None
 
         def _format_data_info(series) -> str:
             table = ""
             table += (
                 "<div class='widget-inline-hbox widget-select' "
                 "style='height:220px;overflow-y:auto;'>"
@@ -751,15 +759,15 @@
             over multiple files, the coordinates will be iterables corresponding to each
             file in the `files` list. For single file scans, an empty dictionary is
             returned.
 
         """
         raise NotImplementedError("method must be implemented in the subclass")
 
-    def infer_index(self, name: str) -> tuple[int | None, dict | None]:
+    def infer_index(self, name: str) -> tuple[int | None, dict[str, Any]]:
         """Infer the index for the given file name.
 
         This method takes a file name and tries to infer the scan index from it. If the
         index can be inferred, it is returned; otherwise, `None` should be returned.
 
         Parameters
         ----------
@@ -798,36 +806,47 @@
             Summary of the data in the directory.
 
         """
         raise NotImplementedError("This loader does not support folder summaries")
 
     def combine_multiple(
         self,
-        data_list: list[xr.DataArray | xr.Dataset],
-        coord_dict: dict[str, Sequence],
-    ) -> xr.DataArray | xr.Dataset | Sequence[xr.DataArray | xr.Dataset]:
+        data_list: list[xr.DataArray | xr.Dataset | list[xr.DataArray]],
+        coord_dict: dict[str, Iterable],
+    ) -> (
+        xr.DataArray | xr.Dataset | list[xr.DataArray | xr.Dataset | list[xr.DataArray]]
+    ):
         if len(coord_dict) == 0:
             try:
                 # Try to merge the data without conflicts
                 return xr.merge(data_list)
             except:  # noqa: E722
                 # On failure, return a list
                 return data_list
         else:
             for i in range(len(data_list)):
-                data_list[i] = data_list[i].assign_coords(
-                    {k: v[i] for k, v in coord_dict.items()}
+                if isinstance(data_list[i], list):
+                    data_list[i] = self.combine_multiple(data_list[i], coord_dict={})
+
+                if not isinstance(data_list[i], list):
+                    data_list[i] = data_list[i].assign_coords(
+                        {k: v[i] for k, v in coord_dict.items()}
+                    )
+            try:
+                return xr.concat(
+                    data_list,
+                    dim=next(iter(coord_dict.keys())),
+                    coords="different",
                 )
-            return xr.concat(
-                data_list, dim=next(iter(coord_dict.keys())), coords="different"
-            )
+            except:  # noqa: E722
+                return data_list
 
     def post_process_general(
-        self, data: xr.DataArray | xr.Dataset | list[xr.DataArray | xr.Dataset]
-    ) -> xr.DataArray | xr.Dataset | list[xr.DataArray | xr.Dataset]:
+        self, data: xr.DataArray | xr.Dataset | list[xr.DataArray]
+    ) -> xr.DataArray | xr.Dataset | list[xr.DataArray]:
         if isinstance(data, xr.DataArray):
             return self.post_process(data)
 
         elif isinstance(data, list):
             return [self.post_process(d) for d in data]
 
         elif isinstance(data, xr.Dataset):
@@ -864,19 +883,23 @@
                 if a in data.attrs and a not in data.coords
             }
         )
         return data
 
     def post_process(self, data: xr.DataArray) -> xr.DataArray:
         data = self.process_keys(data)
-        data = data.assign_attrs(self.additional_attrs)
+        data = data.assign_attrs(
+            self.additional_attrs | {"data_loader_name": str(self.name)}
+        )
         return data
 
     @classmethod
-    def validate(cls, data: xr.DataArray | xr.Dataset):
+    def validate(
+        cls, data: xr.DataArray | xr.Dataset | list[xr.DataArray | xr.Dataset]
+    ) -> None:
         """Validate the input data to ensure it is in the correct format.
 
         Checks for the presence of all required coordinates and attributes. If the data
         does not pass validation, a `ValidationError` is raised or a warning is issued,
         depending on the value of the `strict_validation` flag. Validation is skipped
         for loaders with attribute `skip_validate` set to `True`.
 
@@ -914,15 +937,15 @@
                     f"Invalid configuration {data.attrs['configuration']}"
                 )
             elif "chi" not in data.coords:
                 cls._raise_or_warn("Missing coordinate chi")
 
     def load_multiple_parallel(
         self, file_paths: list[str], n_jobs: int | None = None
-    ) -> list[xr.DataArray | xr.Dataset]:
+    ) -> list[xr.DataArray | xr.Dataset | list[xr.DataArray]]:
         """Load multiple files in parallel.
 
         Parameters
         ----------
         file_paths
             A list of file paths to load.
         n_jobs
@@ -954,32 +977,32 @@
 class RegistryBase:
     """Base class for the loader registry.
 
     This class implements the singleton pattern, ensuring that only one instance of the
     registry is created and used throughout the application.
     """
 
-    __instance = None
+    __instance: RegistryBase | None = None
 
     def __new__(cls):
         if not isinstance(cls.__instance, cls):
             cls.__instance = super().__new__(cls)
         return cls.__instance
 
     @classmethod
-    def instance(cls) -> LoaderRegistry:
+    def instance(cls) -> Self:
         """Returns the registry instance."""
         return cls()
 
 
 class LoaderRegistry(RegistryBase):
-    loaders: dict[str, LoaderBase | type[LoaderBase]] = {}
+    loaders: ClassVar[dict[str, LoaderBase | type[LoaderBase]]] = {}
     """Registered loaders \n\n:meta hide-value:"""
 
-    alias_mapping: dict[str, str] = {}
+    alias_mapping: ClassVar[dict[str, str]] = {}
     """Mapping of aliases to loader names \n\n:meta hide-value:"""
 
     current_loader: LoaderBase | None = None
     """Current loader \n\n:meta hide-value:"""
 
     default_data_dir: str | os.PathLike | None = None
     """Default directory to search for data files \n\n:meta hide-value:"""
@@ -992,36 +1015,39 @@
         self.alias_mapping[loader_class.name] = loader_class.name
         if loader_class.aliases is not None:
             for alias in loader_class.aliases:
                 self.alias_mapping[alias] = loader_class.name
 
     def get(self, key: str) -> LoaderBase:
         loader_name = self.alias_mapping.get(key)
+        if loader_name is None:
+            raise LoaderNotFoundError(key)
+
         loader = self.loaders.get(loader_name)
 
         if loader is None:
-            raise KeyError(f"Loader for {key} not found")
+            raise LoaderNotFoundError(key)
 
         if not isinstance(loader, LoaderBase):
             # If not an instance, create one
-            self.loaders[loader_name] = loader()
-            loader = self.loaders[loader_name]
+            loader = loader()
+            self.loaders[loader_name] = loader
 
         return loader
 
     def __getitem__(self, key: str) -> LoaderBase:
         return self.get(key)
 
     def __getattr__(self, key: str) -> LoaderBase:
         try:
             return self.get(key)
-        except KeyError as e:
-            raise AttributeError(f"Loader for {key} not found") from e
+        except LoaderNotFoundError as e:
+            raise AttributeError(str(e)) from e
 
-    def set_loader(self, loader: str | LoaderBase):
+    def set_loader(self, loader: str | LoaderBase | None):
         """Set the current data loader.
 
         All subsequent calls to `load` will use the loader set here.
 
         Parameters
         ----------
         loader
@@ -1090,15 +1116,15 @@
         finally:
             if loader is not None:
                 self.set_loader(old_loader)
 
             if data_dir is not None:
                 self.set_data_dir(old_data_dir)
 
-    def set_data_dir(self, data_dir: str | os.PathLike):
+    def set_data_dir(self, data_dir: str | os.PathLike | None):
         """Set the default data directory for the data loader.
 
         All subsequent calls to `load` will use the `data_dir` set here unless
         specified.
 
         Parameters
         ----------
@@ -1107,15 +1133,15 @@
 
         Note
         ----
         This will only affect `load`. If the loader's ``load`` method is called
         directly, it will not use the default data directory.
 
         """
-        if not os.path.isdir(data_dir):
+        if data_dir is not None and not os.path.isdir(data_dir):
             raise FileNotFoundError(f"Directory {data_dir} not found")
         self.default_data_dir = data_dir
 
     def load(
         self,
         identifier: str | os.PathLike | int | None,
         data_dir: str | os.PathLike | None = None,
```

### Comparing `erlab-2.3.0/src/erlab/io/exampledata.py` & `erlab-2.3.1/src/erlab/io/exampledata.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     bandshift: float = 0.0,
     Sreal: float = 0.0,
     Simag: float = 0.03,
     kres: float = 0.01,
     Eres: float = 2.0e-3,
     noise: bool = True,
     seed: int | None = None,
-    count: int = 1e8,
+    count: int = 100000000,
     ccd_sigma: float = 0.6,
 ) -> xr.DataArray:
     """Generate simulated data for a given shape in momentum space.
 
     Parameters
     ----------
     shape
@@ -104,20 +104,20 @@
     xarray.DataArray
         The generated data with coordinates for kx, ky, and eV.
 
     """
     if isinstance(krange, dict):
         kx = np.linspace(*krange["kx"], shape[0])
         ky = np.linspace(*krange["ky"], shape[1])
-    elif not np.iterable(krange):
-        kx = np.linspace(-krange, krange, shape[0])
-        ky = np.linspace(-krange, krange, shape[1])
-    else:
+    elif isinstance(krange, tuple):
         kx = np.linspace(*krange, shape[0])
         ky = np.linspace(*krange, shape[1])
+    else:
+        kx = np.linspace(-krange, krange, shape[0])
+        ky = np.linspace(-krange, krange, shape[1])
 
     eV = np.linspace(*Erange, shape[2])
 
     dE = eV[1] - eV[0]
 
     point_iter = np.array(np.meshgrid(kx, ky)).T.reshape(-1, 2)
 
@@ -165,15 +165,15 @@
     bandshift: float = 0.0,
     Sreal: float = 0.0,
     Simag: float = 0.03,
     angres: float = 0.1,
     Eres: float = 10.0e-3,
     noise: bool = True,
     seed: int | None = None,
-    count: int = 1e8,
+    count: int = 100000000,
     ccd_sigma: float = 0.6,
     assign_attributes: bool = False,
 ) -> xr.DataArray:
     """Generate simulated data for a given shape in angle space.
 
     Parameters
     ----------
@@ -224,20 +224,20 @@
         The generated data with coordinates for alpha, beta, and eV.
 
     """
 
     if isinstance(angrange, dict):
         alpha = np.linspace(*angrange["alpha"], shape[0])
         beta = np.linspace(*angrange["beta"], shape[1])
-    elif not np.iterable(angrange):
-        alpha = np.linspace(-angrange, angrange, shape[0])
-        beta = np.linspace(-angrange, angrange, shape[1])
-    else:
+    elif isinstance(angrange, tuple):
         alpha = np.linspace(*angrange, shape[0])
         beta = np.linspace(*angrange, shape[1])
+    else:
+        alpha = np.linspace(-angrange, angrange, shape[0])
+        beta = np.linspace(-angrange, angrange, shape[1])
 
     if not isinstance(configuration, erlab.analysis.kspace.AxesConfiguration):
         configuration = erlab.analysis.kspace.AxesConfiguration(configuration)
 
     eV = np.linspace(*Erange, shape[2])
 
     Ekin = hv - 4.5 + eV[None, None, :]
@@ -303,15 +303,15 @@
     b: float = 0.1,
     c: float = 0.0,
     temp: float = 100.0,
     Eres: float = 1e-2,
     angres: float = 0.1,
     edge_coeffs: Sequence[float] = (0.04, 1e-5, -3e-4),
     background_coeffs: Sequence[float] = (1.0, 0.0, -2e-3),
-    count: int = 1e6,
+    count: int = 1000000,
     noise: bool = True,
     seed: int | None = None,
     ccd_sigma: float = 0.6,
 ) -> xr.DataArray:
     """
     Generate a curved Fermi edge with a linear density of states.
 
@@ -380,23 +380,7 @@
 
     if noise:
         data[:] = scipy.ndimage.gaussian_filter(
             rng.poisson(data).astype(float), sigma=ccd_sigma
         )
 
     return data.assign_attrs(temp_sample=temp)
-
-
-if __name__ == "__main__":
-    # out = generate_data(
-    #     shape=(201, 202, 203),
-    #     krange=1.4,
-    #     Erange=(-0.45, 0.09),
-    #     temp=30,
-    #     bandshift=-0.2,
-    #     count=1000,
-    #     noise=True,
-    # )
-    out = generate_data_angles()
-    import erlab.plotting.erplot as eplt
-
-    eplt.itool([out, out.kspace.convert()])
```

### Comparing `erlab-2.3.0/src/erlab/io/igor.py` & `erlab-2.3.1/src/erlab/io/igor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 import os
 
 import h5netcdf
 import igor2.binarywave
 import igor2.packed
 import igor2.record
+from typing import Any
 import numpy as np
 import xarray as xr
 
 __all__ = ["load_experiment", "load_igor_hdf5", "load_wave"]
 
 
 def _load_experiment_raw(
     filename: str | os.PathLike,
     folder: str | None = None,
     *,
     prefix: str | None = None,
     ignore: list[str] | None = None,
     recursive: bool = False,
     **kwargs,
-) -> xr.Dataset:
+) -> dict[str, xr.DataArray]:
     if folder is None:
-        folder = []
+        split_path: list[Any] = []
     if ignore is None:
         ignore = []
 
     for bo in [">", "=", "<"]:
         try:
             _, expt = igor2.packed.load(filename, initial_byte_order=bo)
             break
         except ValueError:
             continue
 
-    waves = {}
+    waves: dict[str, xr.DataArray] = {}
     if isinstance(folder, str):
-        folder = folder.split("/")
-    folder = [n.encode() for n in folder]
+        split_path = folder.split("/")
+    split_path = [n.encode() for n in split_path]
 
     expt = expt["root"]
-    for dirname in folder:
+    for dirname in split_path:
         expt = expt[dirname]
 
     def unpack_folders(expt):
         for name, record in expt.items():
             if isinstance(record, igor2.record.WaveRecord):
                 if prefix is not None:
                     if not name.decode().startswith(prefix):
@@ -212,15 +213,15 @@
             return dim
         else:
             return f"{dim} ({unit})"
 
     dims = [get_dim_name(i) for i in range(_MAXDIM)]
     coords = {
         dims[i]: np.linspace(b, b + a * (c - 1), c)
-        for i, (a, b, c) in enumerate(zip(sfA, sfB, shape))
+        for i, (a, b, c) in enumerate(zip(sfA, sfB, shape, strict=True))
         if c != 0
     }
 
     attrs = {}
     for ln in d.get("note", "").decode().splitlines():
         if "=" in ln:
             k, v = ln.split("=", 1)
```

### Comparing `erlab-2.3.0/src/erlab/io/plugins/__init__.py` & `erlab-2.3.1/src/erlab/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/io/plugins/da30.py` & `erlab-2.3.1/src/erlab/io/plugins/da30.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,36 +3,35 @@
 DA30L analyzer using ``SES.exe``. Must be subclassed to implement the actual loading.
 """
 
 import configparser
 import os
 import tempfile
 import zipfile
-
+from typing import ClassVar
 import numpy as np
 import xarray as xr
 
 from erlab.io.dataloader import LoaderBase
 from erlab.io.igor import load_experiment, load_wave
 
 
 class DA30Loader(LoaderBase):
-    name: str = "da30"
-    aliases: list[str] = ["DA30"]
+    name = "da30"
+    aliases = ("DA30",)
 
-    name_map: dict[str, str] = {
+    name_map: ClassVar[dict] = {
         "eV": ["Kinetic Energy [eV]", "Energy [eV]"],
         "alpha": ["Y-Scale [deg]", "Thetax [deg]"],
         "beta": ["Thetay [deg]"],
         "hv": ["BL Energy", "Excitation Energy"],
     }
-    coordinate_attrs: tuple[str, ...] = ()
-    additional_attrs: dict[str, str | int | float] = {}
-    always_single: bool = True
-    skip_validate: bool = True
+    additional_attrs: ClassVar[dict] = {}
+    always_single = True
+    skip_validate = True
 
     def load_single(self, file_path: str | os.PathLike) -> xr.DataArray:
         ext = os.path.splitext(file_path)[-1]
 
         match ext:
             case ".ibw":
                 data = load_wave(file_path)
```

### Comparing `erlab-2.3.0/src/erlab/io/plugins/kriss.py` & `erlab-2.3.1/src/erlab/io/plugins/kriss.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Plugin for data acquired at KRISS."""
 
 import os
 import re
 from collections.abc import Iterable
+from typing import ClassVar
 
 import erlab.io.utilities
 from erlab.io.plugins.da30 import DA30Loader
 
 
 class KRISSLoader(DA30Loader):
-    name: str = "kriss"
+    name = "kriss"
 
-    aliases: list[str] = ["KRISS"]
+    aliases = ("KRISS",)
 
-    coordinate_attrs: tuple[str, ...] = ("beta", "chi", "xi", "hv", "x", "y", "z")
+    coordinate_attrs = ("beta", "chi", "xi", "hv", "x", "y", "z")
 
-    additional_attrs: dict[str, str | int | float] = {"configuration": 4}
+    additional_attrs: ClassVar[dict] = {"configuration": 4}
 
     @property
     def name_map(self):
         return super().name_map | {"chi": "ThetaY", "xi": "ThetaX"}
 
     def identify(
         self, num: int, data_dir: str | os.PathLike
```

### Comparing `erlab-2.3.0/src/erlab/io/plugins/merlin.py` & `erlab-2.3.1/src/erlab/io/plugins/merlin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,86 +1,89 @@
 """Data loader for beamline 4.0.3 at ALS."""
 
 import datetime
 import glob
 import os
 import re
+from typing import Any, ClassVar
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import xarray as xr
 
 import erlab.io.utilities
 from erlab.io.dataloader import LoaderBase
 from erlab.io.igor import load_experiment, load_wave
 
 
 class BL403Loader(LoaderBase):
-    name: str = "merlin"
-    aliases: list[str] = ["ALS_BL4", "als_bl4", "BL403", "bl403"]
+    name = "merlin"
 
-    name_map: dict[str, str | list[str]] = {
+    aliases = ("ALS_BL4", "als_bl4", "BL403", "bl403")
+
+    name_map: ClassVar[dict] = {
         "alpha": "deg",
         "beta": ["Polar", "Polar Compens"],
         "delta": "Azimuth",
         "xi": "Tilt",
         "x": "Sample X",
         "y": "Sample Y (Vert)",
         "z": "Sample Z",
         "hv": "BL Energy",
         "polarization": "EPU POL",
         "temp_sample": "Temperature Sensor B",
         "mesh_current": "Mesh Current",
     }
-    coordinate_attrs: tuple[str, ...] = (
+    coordinate_attrs = (
         "beta",
         "delta",
         "xi",
         "hv",
         "x",
         "y",
         "z",
         "polarization",
         "mesh_current",
     )
-    additional_attrs: dict[str, str | int | float] = {
+    additional_attrs: ClassVar[dict] = {
         "configuration": 1,
         "sample_workfunction": 4.44,
     }
-    always_single: bool = False
+    always_single = False
 
     def load_single(self, file_path: str | os.PathLike) -> xr.DataArray:
         if os.path.splitext(file_path)[1] == ".ibw":
             return self.load_live(file_path)
 
         data = load_experiment(file_path)
         # One file always corresponds to single region, so assume only one data variable
         data: xr.DataArray = data.data_vars[next(iter(data.data_vars.keys()))]
 
         return self.process_keys(data)
 
-    def identify(
-        self, num: int, data_dir: str | os.PathLike
-    ) -> tuple[list[str], dict[str, npt.NDArray[np.float64]]]:
+    def identify(self, num: int, data_dir: str | os.PathLike):
         coord_dict: dict[str, npt.NDArray[np.float64]] = {}
 
         # Look for scans
         files = glob.glob(f"*_{str(num).zfill(3)}_S*.pxt", root_dir=data_dir)
         files.sort()
         # Assume files sorted by scan #
 
         if len(files) == 0:
             # Look for multiregion scan
             files = glob.glob(f"*_{str(num).zfill(3)}_R*.pxt", root_dir=data_dir)
             files.sort()
         elif len(files) > 1:
-            prefix: str = re.match(
+            match_prefix = re.match(
                 r"(.*?)_" + str(num).zfill(3) + r"(?:_S\d{3})?.pxt", files[0]
-            ).group(1)
+            )
+            if match_prefix is None:
+                raise RuntimeError(f"Failed to match prefix in {files[0]}")
+            prefix: str = match_prefix.group(1)
 
             motor_file = os.path.join(
                 data_dir, f"{prefix}_{str(num).zfill(3)}_Motor_Pos.txt"
             )
 
             coord_arr = np.loadtxt(motor_file, skiprows=1)
             with open(motor_file) as f:
@@ -100,24 +103,28 @@
         if len(files) == 0:
             raise FileNotFoundError(f"No files found for scan {num} in {data_dir}")
 
         files = [os.path.join(data_dir, f) for f in files]
 
         return files, coord_dict
 
-    def infer_index(self, name: str) -> tuple[int | None, dict]:
+    def infer_index(self, name: str) -> tuple[int | None, dict[str, Any]]:
         try:
-            scan_num: str = re.match(r".*?(\d{3})(?:_S\d{3})?", name).group(1)
-        except (AttributeError, IndexError):
-            return None, None
+            match_scan = re.match(r".*?(\d{3})(?:_S\d{3})?", name)
+            if match_scan is None:
+                return None, {}
+
+            scan_num: str = match_scan.group(1)
+        except IndexError:
+            return None, {}
 
         if scan_num.isdigit():
             return int(scan_num), {}
         else:
-            return None, None
+            return None, {}
 
     def post_process(self, data: xr.DataArray) -> xr.DataArray:
         data = super().post_process(data)
 
         if "eV" in data.coords:
             data = data.assign_coords(eV=-data.eV.values)
```

### Comparing `erlab-2.3.0/src/erlab/io/plugins/ssrl52.py` & `erlab-2.3.1/src/erlab/io/plugins/ssrl52.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,45 @@
 """Data loader for beamline 5-2 at SSRL."""
 
 import datetime
 import os
 import re
+from typing import ClassVar
 
 import h5netcdf
 import numpy as np
-import numpy.typing as npt
 import pandas as pd
 import xarray as xr
 
 import erlab.io.utilities
 from erlab.io.dataloader import LoaderBase
 
 
 class SSRL52Loader(LoaderBase):
-    name: str = "ssrl"
-    aliases: list[str] = ["ssrl52", "bl5-2"]
+    name = "ssrl"
+    aliases = ("ssrl52", "bl5-2")
 
-    name_map: dict[str, str] = {
+    name_map: ClassVar[dict] = {
         "eV": "Kinetic Energy",
         "alpha": "ThetaX",
         "beta": ["ThetaY", "YDeflection", "DeflectionY"],
         "delta": ["A", "a"],  # azi
         "chi": ["T", "t"],  # polar
         "xi": ["F", "f"],  # tilt
         "x": "X",
         "y": "Y",
         "z": "Z",
         "hv": ["BL_energy", "BL_photon_energy"],
         "temp_sample": ["TB", "sample_stage_temperature"],
         "sample_workfunction": "WorkFunction",
     }
-    coordinate_attrs: tuple[str, ...] = (
-        "beta",
-        "delta",
-        "chi",
-        "xi",
-        "hv",
-        "x",
-        "y",
-        "z",
-    )
-    additional_attrs: dict[str, str | int | float] = {
+
+    coordinate_attrs = ("beta", "delta", "chi", "xi", "hv", "x", "y", "z")
+
+    additional_attrs: ClassVar[dict] = {
         "configuration": 3,
         "sample_workfunction": 4.5,
     }
 
     always_single: bool = True
     skip_validate: bool = True
 
@@ -119,15 +112,15 @@
         return self.process_keys(data)
 
     def identify(
         self,
         num: int,
         data_dir: str | os.PathLike,
         zap: bool = False,
-    ) -> tuple[list[str], dict[str, npt.NDArray[np.float64]]]:
+    ):
         if zap:
             target_files = erlab.io.utilities.get_files(
                 data_dir, extensions=(".h5",), contains="zap"
             )
         else:
             target_files = erlab.io.utilities.get_files(
                 data_dir, extensions=(".h5",), notcontains="zap"
```

### Comparing `erlab-2.3.0/src/erlab/io/utilities.py` & `erlab-2.3.1/src/erlab/io/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,15 +200,15 @@
     elif data.ndim > 4:
         igor_compat = False
 
     if igor_compat:
         # IGORWaveScaling order: chunk row column layer
         scaling = [[1, 0]]
         for i in range(data.ndim):
-            coord: npt.NDArray = data[data.dims[i]].values
+            coord: npt.NDArray = np.asarray(data[data.dims[i]].values)
             delta = coord[1] - coord[0]
             scaling.append([delta, coord[0]])
         if data.ndim == 4:
             scaling[0] = scaling.pop(-1)
         data.attrs["IGORWaveScaling"] = scaling
     data.to_netcdf(
         filename,
```

### Comparing `erlab-2.3.0/src/erlab/lattice.py` & `erlab-2.3.1/src/erlab/lattice.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/parallel.py` & `erlab-2.3.1/src/erlab/parallel.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/plotting/IgorCT/Blue-White.txt` & `erlab-2.3.1/src/erlab/plotting/IgorCT/Blue-White.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/plotting/IgorCT/BlueHot.ibw` & `erlab-2.3.1/src/erlab/plotting/IgorCT/BlueHot.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/plotting/IgorCT/CTBlueWhite.ibw` & `erlab-2.3.1/src/erlab/plotting/IgorCT/CTBlueWhite.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw` & `erlab-2.3.1/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/plotting/IgorCT/CTRedTemperature.ibw` & `erlab-2.3.1/src/erlab/plotting/IgorCT/CTRedTemperature.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/plotting/IgorCT/ColdWarm.ibw` & `erlab-2.3.1/src/erlab/plotting/IgorCT/ColdWarm.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/plotting/IgorCT/PlanetEarth.ibw` & `erlab-2.3.1/src/erlab/plotting/IgorCT/PlanetEarth.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/plotting/IgorCT/ametrine.ibw` & `erlab-2.3.1/src/erlab/plotting/IgorCT/ametrine.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/plotting/IgorCT/isolum.ibw` & `erlab-2.3.1/src/erlab/plotting/IgorCT/isolum.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/plotting/IgorCT/morgenstemning.ibw` & `erlab-2.3.1/src/erlab/plotting/IgorCT/morgenstemning.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/plotting/__init__.py` & `erlab-2.3.1/src/erlab/plotting/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,14 +58,18 @@
     fname
         Path to the Igor CT wave file.
     name
         The name to register the colormap as.
 
     """
     file = pkgutil.get_data(__package__, "IgorCT/" + fname)
+
+    if file is None:
+        raise FileNotFoundError(f"Could not find file {fname}")
+
     if fname.endswith(".txt"):
         values = np.genfromtxt(io.StringIO(file.decode()))
     elif fname.endswith(".ibw"):
         values = erlab.io.load_wave(io.BytesIO(file)).values
 
     cmap = matplotlib.colors.LinearSegmentedColormap.from_list(name, values / 65535)
     matplotlib.colormaps.register(cmap)
```

### Comparing `erlab-2.3.0/src/erlab/plotting/annotations.py` & `erlab-2.3.1/src/erlab/plotting/annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,21 @@
     "set_xlabels",
     "set_ylabels",
     "sizebar",
 ]
 
 import io
 import re
-from typing import TYPE_CHECKING, Literal
+from typing import TYPE_CHECKING, Any, Literal, cast
 
 import matplotlib
+import matplotlib.backends.backend_pdf
+import matplotlib.backends.backend_svg
+import matplotlib.figure
+import matplotlib.mathtext
 import matplotlib.pyplot as plt
 import matplotlib.ticker
 import matplotlib.transforms as mtransforms
 import numpy as np
 import pyperclip
 from mpl_toolkits.axes_grid1.anchored_artists import AnchoredSizeBar
 
@@ -260,14 +264,15 @@
         fontproperties = matplotlib.font_manager.FontProperties(size=fontsize)
     else:
         fontproperties.set_size(fontsize)
     if rcparams is None:
         rcparams = {}
     parser = matplotlib.mathtext.MathTextParser("path")
     width, height, depth, _, _ = parser.parse(s, dpi=72, prop=fontproperties)
+
     fig = matplotlib.figure.Figure(figsize=(width / 72, height / 72))
     fig.patch.set_facecolor("none")
     fig.text(0, depth / height, s, fontproperties=fontproperties)
 
     if svg:
         matplotlib.backends.backend_svg.FigureCanvasSVG(fig)
     else:
@@ -281,19 +286,19 @@
         rcparams[f"mathtext.{k}"] = v
 
     with io.BytesIO() as buffer:
         if svg:
             rcparams.setdefault("svg.fonttype", "path" if outline else "none")
             rcparams.setdefault("svg.image_inline", True)
             with plt.rc_context(rcparams):
-                fig.canvas.print_svg(buffer)
+                fig.canvas.print_svg(buffer)  # type: ignore[attr-defined]
         else:
             rcparams.setdefault("pdf.fonttype", 3 if outline else 42)
             with plt.rc_context(rcparams):
-                fig.canvas.print_pdf(buffer)
+                fig.canvas.print_pdf(buffer)  # type: ignore[attr-defined]
         pyperclip.copy(buffer.getvalue().decode("utf-8"))
 
 
 def fancy_labels(ax=None, deg2rad=False):
     if ax is None:
         ax = plt.gca()
     if np.iterable(ax):
@@ -304,15 +309,15 @@
     ax.set_xlabel(label_for_dim(dim_name=ax.get_xlabel(), deg2rad=deg2rad))
     ax.set_ylabel(label_for_dim(dim_name=ax.get_ylabel(), deg2rad=deg2rad))
     if hasattr(ax, "get_zlabel"):
         ax.set_zlabel(label_for_dim(dim_name=ax.get_zlabel(), deg2rad=deg2rad))
 
 
 def label_subplot_properties(
-    axes: matplotlib.axes.Axes | Sequence[matplotlib.axes.Axes],
+    axes: matplotlib.axes.Axes | Iterable[matplotlib.axes.Axes],
     values: dict,
     decimals: int | None = None,
     si: int = 0,
     name: str | None = None,
     unit: str | None = None,
     order: Literal["C", "F", "A", "K"] = "C",
     **kwargs,
@@ -348,34 +353,34 @@
 
     """
     kwargs.setdefault("fontweight", plt.rcParams["font.weight"])
     kwargs.setdefault("prefix", "")
     kwargs.setdefault("suffix", "")
     kwargs.setdefault("loc", "upper right")
 
-    strlist = []
+    strlist: Any = []
     for k, v in values.items():
         if not isinstance(v, tuple | list | np.ndarray):
             v = [v]
         else:
             v = np.array(v).flatten(order=order)
         strlist.append(
             [
                 property_label(k, val, decimals=decimals, si=si, name=name, unit=unit)
                 for val in v
             ]
         )
-    strlist = list(zip(*strlist))
+    strlist = list(zip(*strlist, strict=True))
     strlist = ["\n".join(strlist[i]) for i in range(len(strlist))]
     label_subplots(axes, strlist, order=order, **kwargs)
 
 
 def label_subplots(
-    axes: matplotlib.axes.Axes | Sequence[matplotlib.axes.Axes],
-    values: Sequence[int | str] | None = None,
+    axes: matplotlib.axes.Axes | Iterable[matplotlib.axes.Axes],
+    values: Iterable[int | str] | None = None,
     startfrom: int = 1,
     order: Literal["C", "F", "A", "K"] = "C",
     loc: Literal[
         "upper left",
         "upper center",
         "upper right",
         "center left",
@@ -463,44 +468,44 @@
     if plt.rcParams["text.usetex"] & (fontweight == "bold"):
         prefix = "\\textbf{" + prefix
         suffix = suffix + "}"
         kwargs.pop("fontweight")
 
     axlist = np.array(axes, dtype=object).flatten(order=order)
     if values is None:
-        values = np.array([i + startfrom for i in range(len(axlist))], dtype=np.int64)
+        value_arr = np.array(
+            [i + startfrom for i in range(len(axlist))], dtype=np.int64
+        )
     else:
-        values = np.array(values).flatten(order=order)
-        if not (axlist.size == values.size):
+        value_arr = np.array(values).flatten(order=order)
+        if not (axlist.size == value_arr.size):
             raise IndexError(
                 "The number of given values must match the number of given axes."
             )
 
     for i in range(len(axlist)):
         bbox_to_anchor = axlist[i].bbox
         if fontsize is None:
             if isinstance(axlist[i], matplotlib.figure.Figure):
-                fs = "large"
+                fontsize = "large"
             else:
-                fs = "medium"
-        else:
-            fs = fontsize
+                fontsize = "medium"
 
         bbox_transform = matplotlib.transforms.ScaledTranslation(
             offset[0] / 72, offset[1] / 72, axlist[i].get_figure().dpi_scale_trans
         )
-        label_str = _alph_label(values[i], prefix, suffix, numeric, capital)
+        label_str = _alph_label(value_arr[i], prefix, suffix, numeric, capital)
         with plt.rc_context({"text.color": axes_textcolor(axlist[i])}):
             at = matplotlib.offsetbox.AnchoredText(
                 label_str,
                 loc=loc,
                 frameon=False,
                 pad=0,
                 borderpad=0.5,
-                prop=dict(fontsize=fs, **kwargs),
+                prop=dict(fontsize=fontsize, **kwargs),
                 bbox_to_anchor=bbox_to_anchor,
                 bbox_transform=bbox_transform,
                 clip_on=False,
             )
         axlist[i].add_artist(at)
 
 
@@ -583,24 +588,26 @@
     if plt.rcParams["text.usetex"] & (fontweight == "bold"):
         prefix = "\\textbf{" + prefix
         suffix = suffix + "}"
         kwargs.pop("fontweight")
 
     axlist = np.array(axes, dtype=object).flatten(order=order)
     if values is None:
-        values = np.array([i + startfrom for i in range(len(axlist))], dtype=np.int64)
+        value_arr = np.array(
+            [i + startfrom for i in range(len(axlist))], dtype=np.int64
+        )
     else:
-        values = np.array(values).flatten(order=order)
-        if not (axlist.size == values.size):
+        value_arr = np.array(values).flatten(order=order)
+        if not (axlist.size == value_arr.size):
             raise IndexError(
                 "The number of given values must match the number of given axes."
             )
 
     for i in range(len(axlist)):
-        label_str = _alph_label(values[i], prefix, suffix, numeric, capital)
+        label_str = _alph_label(value_arr[i], prefix, suffix, numeric, capital)
         trans = matplotlib.transforms.ScaledTranslation(
             offset[0] / 72, offset[1] / 72, axlist[i].get_figure().dpi_scale_trans
         )
 
         if fontsize is None:
             fontsize = "medium"
         axlist[i].figure.text(
@@ -620,15 +627,15 @@
     points: Sequence[float],
     labels: Sequence[str],
     y: float | Sequence[float] = 0.0,
     pad: tuple[float, float] = (0, 1.75),
     literal: bool = False,
     roman: bool = True,
     bar: bool = False,
-    ax: matplotlib.axes.Axes | Iterable[matplotlib.axes.Axes] = None,
+    ax: matplotlib.axes.Axes | Iterable[matplotlib.axes.Axes] | None = None,
     **kwargs,
 ):
     """Mark points above the horizontal axis.
 
     Useful when annotating high symmetry points along a cut.
 
     Parameters
@@ -650,43 +657,52 @@
         If ``True``, prints a bar over the label.
     ax
         `matplotlib.axes.Axes` to annotate.
 
     """
     if ax is None:
         ax = plt.gca()
+
     if np.iterable(ax):
         for a in np.asarray(ax, dtype=object).flatten():
             mark_points(points, labels, y, pad, literal, roman, bar, a, **kwargs)
     else:
+        ax = cast(matplotlib.axes.Axes, ax)  # to appease mypy
+        fig = ax.get_figure()
+
+        if fig is None:
+            raise ValueError("Given axes does not belong to a figure")
+
         for k, v in {"ha": "center", "va": "baseline", "fontsize": "small"}.items():
             kwargs.setdefault(k, v)
+
         if not np.iterable(y):
-            y = [y] * len(points)
+            y = [y] * len(points)  # type: ignore[list-item]
+
         with plt.rc_context({"font.family": "serif"}):
-            for xi, yi, label in zip(points, y, labels):
+            for xi, yi, label in zip(points, y, labels, strict=True):
                 ax.text(
                     xi,
                     yi,
                     label if literal else parse_point_labels(label, roman, bar),
                     transform=ax.transData
                     + mtransforms.ScaledTranslation(
-                        pad[0] / 72, pad[1] / 72, ax.figure.dpi_scale_trans
+                        pad[0] / 72, pad[1] / 72, fig.dpi_scale_trans
                     ),
                     **kwargs,
                 )
 
 
 def mark_points_outside(
     points: Sequence[float],
     labels: Sequence[str],
     axis: Literal["x", "y"] = "x",
     roman: bool = True,
     bar: bool = False,
-    ax: matplotlib.axes.Axes | Iterable[matplotlib.axes.Axes] = None,
+    ax: matplotlib.axes.Axes | Iterable[matplotlib.axes.Axes] | None = None,
 ):
     """Mark points above the horizontal axis.
 
     Useful when annotating high symmetry points along a cut.
 
     Parameters
     ----------
@@ -708,14 +724,16 @@
     """
     if ax is None:
         ax = plt.gca()
     if np.iterable(ax):
         for a in np.asarray(ax, dtype=object).flatten():
             mark_points_outside(points, labels, axis, roman, bar, a)
     else:
+        ax = cast(matplotlib.axes.Axes, ax)  # to appease mypy
+
         if axis == "x":
             label_ax = ax.twiny()
             label_ax.set_xlim(ax.get_xlim())
             label_ax.set_xticks(points)
             label_ax.set_xticklabels(
                 [parse_point_labels(lab, roman, bar) for lab in labels]
             )
@@ -771,15 +789,15 @@
         horizontalalignment="right",
         verticalalignment="top",
         transform=ax.transAxes,
         **kwargs,
     )
 
 
-def property_label(key, value, decimals=None, si=0, name=None, unit=None):
+def property_label(key, value, decimals=None, si=0, name=None, unit=None) -> str:
     if name == "":
         delim = ""
     else:
         delim = " = "
     if name is None:
         name = name_for_dim(key, escaped=False)
         if name is None:
@@ -879,33 +897,33 @@
         else:
             setlabel(label.replace(f"({unit})", f"({get_si_str(si)}{unit})"))
 
 
 def set_titles(axes, labels, order="C", **kwargs):
     axlist = np.array(axes, dtype=object).flatten(order=order)
     labels = np.asarray(labels)
-    for ax, label in zip(axlist.flat, labels.flat):
+    for ax, label in zip(axlist.flat, labels.flat, strict=True):
         ax.set_title(label, **kwargs)
 
 
 def set_xlabels(axes, labels, order="C", **kwargs):
     axlist = np.array(axes, dtype=object).flatten(order=order)
     if isinstance(labels, str):
         labels = [labels] * len(axlist)
     labels = np.asarray(labels)
-    for ax, label in zip(axlist.flat, labels.flat):
+    for ax, label in zip(axlist.flat, labels.flat, strict=True):
         ax.set_xlabel(label, **kwargs)
 
 
 def set_ylabels(axes, labels, order="C", **kwargs):
     axlist = np.array(axes, dtype=object).flatten(order=order)
     if isinstance(labels, str):
         labels = [labels] * len(axlist)
     labels = np.asarray(labels)
-    for ax, label in zip(axlist.flat, labels.flat):
+    for ax, label in zip(axlist.flat, labels.flat, strict=True):
         ax.set_ylabel(label, **kwargs)
 
 
 def sizebar(
     ax: matplotlib.axes.Axes,
     value: float,
     unit: str,
```

### Comparing `erlab-2.3.0/src/erlab/plotting/atoms.py` & `erlab-2.3.1/src/erlab/plotting/atoms.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 Some of the projection code was adapted from kwant.
 
 """
 
 import contextlib
 import functools
 import itertools
-from collections.abc import Callable, Sequence
-from typing import Literal
+from collections.abc import Callable, Iterable, Mapping, Sequence
+from typing import Literal, cast
 
 import matplotlib.collections
-import matplotlib.colors as mcolors
+import matplotlib.colors
 import matplotlib.pyplot as plt
 import mpl_toolkits.mplot3d
 import mpl_toolkits.mplot3d.art3d
 import mpl_toolkits.mplot3d.proj3d
 import numpy as np
 import numpy.typing as npt
+from matplotlib.typing import ColorType
 
 __all__ = ["Atom3DCollection", "Bond3DCollection", "CrystalProperty"]
 
 
 def sunflower_sphere(n: int = 100) -> npt.NDArray[np.float64]:
     """Returns n points on a sphere using the sunflower algorithm."""
     indices = np.arange(0, n, dtype=float) + 0.5
@@ -74,15 +75,17 @@
 def projected_length_pos(ax: mpl_toolkits.mplot3d.Axes3D, length, position):
     if position.ndim > 1:
         if not np.iterable(length):
             length = np.ones(len(position)) * length
         return np.asarray(
             [
                 projected_length_pos(ax, d, p)
-                for d, p in zip(np.asarray(length).flat, np.asarray(position))
+                for d, p in zip(
+                    np.asarray(length).flat, np.asarray(position), strict=True
+                )
             ]
         )
     rc = np.asarray(position).reshape(-1, 1)
     rs = unit_sphere * length + rc
 
     transform = mpl_toolkits.mplot3d.proj3d.proj_transform
     proj = ax.get_proj()
@@ -96,15 +99,15 @@
 def _zalpha(colors, zs):
     """Modified from `mpl_toolkits.mplot3d.art3d` to modifies the brightness of the
     color based on depth, rather than setting the transparency."""
     if len(colors) == 0 or len(zs) == 0:
         return np.zeros((0, 4))
     norm = plt.Normalize(min(zs), max(zs))
     sats = 1 - norm(zs) * 0.7
-    rgba = np.broadcast_to(mcolors.to_rgba_array(colors), (len(zs), 4))
+    rgba = np.broadcast_to(matplotlib.colors.to_rgba_array(colors), (len(zs), 4))
     rgba = rgba.T * sats
     rgba += 1 - sats
     rgba = rgba.T
     rgba[:, 3] = 1
     return rgba
 
 
@@ -127,15 +130,15 @@
         color_array = (
             _zalpha(color_array, self._vzs)
             if self._vzs is not None and self._depthshade
             else color_array
         )
         if len(color_array) > 1:
             color_array = color_array[self._z_markers_idx]
-        return mcolors.to_rgba_array(color_array, self._alpha)
+        return matplotlib.colors.to_rgba_array(color_array, self._alpha)
 
     def set_sizes(self, sizes: np.ndarray, dpi: float = 72.0):
         super().set_sizes(sizes, dpi)
         self.sizes_orig = np.asarray(sizes) if np.iterable(sizes) else sizes
 
     @contextlib.contextmanager
     def _use_zordered_offset(self):
@@ -236,23 +239,23 @@
         #     self._transforms[:, 2, 2] = 1.0
         # self.stale = True
 
 
 class CrystalProperty:
     def __init__(
         self,
-        atom_pos: dict[
-            str, npt.NDArray[np.float64] | Sequence[npt.NDArray[np.float64]]
+        atom_pos: Mapping[
+            str, Iterable[float | np.floating | npt.NDArray[np.floating]]
         ],
         avec: npt.NDArray[np.float64],
-        offset: npt.NDArray[np.float64] | Sequence[float] = (0.0, 0.0, 0.0),
-        radii: Sequence[float] | None = None,
-        colors: Sequence[str | tuple[float, ...]] | None = None,
+        offset: Iterable[float] = (0.0, 0.0, 0.0),
+        radii: Iterable[float] | None = None,
+        colors: Iterable[ColorType] | None = None,
         repeat: tuple[int, int, int] = (1, 1, 1),
-        bounds: dict[Literal["x", "y", "z"], tuple[float, float]] | None = None,
+        bounds: Mapping[Literal["x", "y", "z"], tuple[float, float]] | None = None,
         mask: Callable | None = None,
         r_factor: float = 0.4,
     ):
         """
         A class that stores the information required to plot a three dimensional crystal
         structure. The crystal can be repeated along the lattice vectors, and can be
         masked. Bonds can be added between atoms.
@@ -292,24 +295,26 @@
         """
         self.atom_pos_given = atom_pos
         self.avec = avec
         self.offset = np.asarray(offset)
 
         if radii is None:
             radii = [1.0] * len(self.atoms)
-        self.atom_radii: dict[str, float] = dict(zip(self.atoms, radii))
+        self.atom_radii: dict[str, float] = dict(zip(self.atoms, radii, strict=True))
 
         if colors is None:
             colors = [f"C{i}" for i in range(len(self.atoms))]
+
         self.atom_color: dict[str, str] = {
-            k: mcolors.to_hex(v) for k, v in zip(self.atoms, colors)
+            k: matplotlib.colors.to_hex(v)
+            for k, v in zip(self.atoms, colors, strict=True)
         }
 
         self.repeat: tuple[int, int, int] = repeat
-        self._bounds: dict[Literal["x", "y", "z"], tuple[float, float]] = (
+        self._bounds: Mapping[Literal["x", "y", "z"], tuple[float, float]] = (
             {} if bounds is None else bounds
         )
         self.mask: Callable | None = mask
 
         self.segments: list[
             tuple[npt.NDArray[np.float64], npt.NDArray[np.float64]]
         ] = []
@@ -322,25 +327,30 @@
     def from_fractional(
         cls,
         frac_pos: dict[str, list[tuple[float, float, float]]],
         avec: npt.NDArray[np.float64],
         *args,
         **kwargs,
     ):
-        atom_pos = {}
+        atom_pos: dict[str, list[npt.NDArray[np.float64]]] = {}
         for k, v in frac_pos.items():
-            atom_pos[k] = [x[0] * avec[0] + x[1] * avec[1] + x[2] * avec[2] for x in v]
+            atom_pos[k] = [
+                np.asarray(
+                    x[0] * avec[0] + x[1] * avec[1] + x[2] * avec[2], dtype=np.float64
+                )
+                for x in v
+            ]
         return cls(atom_pos, avec, *args, **kwargs)
 
     @property
     def bounds(self) -> list[tuple[float, float]]:
         bound_list = []
         for dim in ("x", "y", "z"):
             try:
-                bound_list.append(self._bounds[dim])
+                bound_list.append(self._bounds[cast(Literal["x", "y", "z"], dim)])
             except KeyError:
                 bound_list.append((-np.inf, np.inf))
         return bound_list
 
     @property
     def atoms(self) -> list[str]:
         return list(self.atom_pos_given.keys())
@@ -382,25 +392,25 @@
         for k, v in atom_pos.items():
             masked_atom_pos[k] = np.asarray(
                 [p for i, p in enumerate(v) if i in valid[k][0]]
             )
         return masked_atom_pos
 
     @property
-    def _color_array(self) -> tuple[npt.NDArray[np.str_]]:
+    def _color_array(self) -> npt.NDArray[np.str_]:
         return np.asarray(
             [
                 self.atom_color[k]
                 for k, v in self.atom_pos.items()
                 for _ in range(len(v))
             ]
         )
 
     @property
-    def _size_array(self) -> tuple[npt.NDArray[np.float64]]:
+    def _size_array(self) -> npt.NDArray[np.float64]:
         return np.asarray(
             [
                 self.atom_radii[k]
                 for k, v in self.atom_pos.items()
                 for _ in range(len(v))
             ]
         )
@@ -460,14 +470,15 @@
             Keyword arguments passed onto `mpl_toolkits.mplot3d.Axes3D.scatter` used to
             plot the atoms.
 
         """
 
         if ax is None:
             ax = plt.gcf().add_subplot(projection="3d")
+        ax = cast(mpl_toolkits.mplot3d.Axes3D, ax)
 
         if clean_axes:
             ax.set_facecolor("none")
             ax.xaxis.set_pane_color((1, 1, 1, 0))
             ax.yaxis.set_pane_color((1, 1, 1, 0))
             ax.zaxis.set_pane_color((1, 1, 1, 0))
             ax.grid(False)
```

### Comparing `erlab-2.3.0/src/erlab/plotting/bz.py` & `erlab-2.3.1/src/erlab/plotting/bz.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "linewidth": ["lw", 0.5],
 }
 
 
 def get_bz_edge(
     basis: npt.NDArray[np.float64],
     reciprocal: bool = True,
-    extend: tuple[int, int, int] | tuple[int, int] | None = None,
+    extend: tuple[int, ...] | None = None,
 ) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.float64]]:
     """Calculates the edge of the first Brillouin zone (BZ) from lattice vectors.
 
     Parameters
     ----------
     basis
         ``(N, N)`` numpy array where ``N = 2``or ``3`` with each row containing the
@@ -43,76 +43,79 @@
     lines : array-like
         ``(M, 2, N)`` array that specifies the endpoints of the ``M`` lines that make up
         the BZ edge, where ``N = len(basis)``.
     vertices : array-like
         Vertices of the BZ.
 
     """
-    if not (basis.shape == (2, 2) or basis.shape == (3, 3)):
+    if basis.shape == (2, 2):
+        ndim = 2
+    elif basis.shape == (3, 3):
+        ndim = 3
+    else:
         raise ValueError("Shape of `basis` must be (N, N) where N = 2 or 3.")
+
     if not reciprocal:
         basis = 2 * np.pi * np.linalg.inv(basis).T
 
-    ndim = basis.shape[-1]
-
     if extend is None:
         extend = (1,) * ndim
 
     points = (
-        np.tensordot(basis, np.mgrid[[slice(-1, 2) for _ in range(ndim)]], axes=[0, 0])
+        np.tensordot(basis, np.mgrid[[slice(-1, 2) for _ in range(ndim)]], axes=(0, 0))
         .reshape((ndim, 3**ndim))
         .T
     )
 
     # Get index of origin
     zero_ind = np.where((points == 0).all(axis=1))[0][0]
 
     vor = scipy.spatial.Voronoi(points)
 
     lines = []
     vertices = []
 
-    for pointidx, simplex in zip(vor.ridge_points, vor.ridge_vertices):
+    for pointidx, simplex in zip(vor.ridge_points, vor.ridge_vertices, strict=True):
         simplex = np.asarray(simplex)
         if zero_ind in pointidx:
             # If the origin is included in the ridge, add the vertices
             lines.append(vor.vertices[np.r_[simplex, simplex[0]]])
             vertices.append(vor.vertices[simplex])
 
     # Remove duplicates
-    lines_new = []
-    vertices_new = []
+    lines_new: list[npt.NDArray] = []
+    vertices_new: list[npt.NDArray] = []
 
     for line in lines:
         for i in range(line.shape[0] - 1):
             if not any(
                 np.allclose(line[i : i + 2], line_new)
                 or np.allclose(line[i : i + 2], np.flipud(line_new))
                 for line_new in lines_new
             ):
                 lines_new.append(line[i : i + 2])
     for v in np.r_[*vertices]:
         if not any(np.allclose(v, vn) for vn in vertices_new):
             vertices_new.append(v)
 
-    lines = np.asarray(lines_new)
-    vertices = np.asarray(vertices_new)
+    lines_arr = np.asarray(lines_new)
+    vertices_arr = np.asarray(vertices_new)
 
     # Extend the BZ
     additional_lines = []
     additional_verts = []
     for vals in itertools.product(*[range(-n + 1, n) for n in extend]):
         if vals != (0,) * ndim:
             displacement = np.dot(vals, basis)
-            additional_lines.append(lines + displacement)
-            additional_verts.append(vertices + displacement)
-    lines = np.r_[lines, *additional_lines]
-    vertices = np.r_[vertices, *additional_verts]
+            additional_lines.append(lines_arr + displacement)
+            additional_verts.append(vertices_arr + displacement)
+    lines_arr = np.r_[lines_arr, *additional_lines]
+    vertices_arr = np.r_[vertices_arr, *additional_verts]
 
-    return lines, vertices
+    return lines_arr, vertices_arr
 
 
 def plot_hex_bz(
     a=3.54, rotate=0.0, offset=(0.0, 0.0), reciprocal=True, ax=None, **kwargs
 ):
     """
     Plots a 2D hexagonal BZ overlay on the specified axes.
```

### Comparing `erlab-2.3.0/src/erlab/plotting/colors.py` & `erlab-2.3.1/src/erlab/plotting/colors.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,26 +43,28 @@
     "prominent_color",
     "proportional_colorbar",
     "unify_clim",
 ]
 
 from collections.abc import Iterable, Sequence
 from numbers import Number
-from typing import Any, Literal
+from typing import Any, Literal, cast
 
 import matplotlib
 import matplotlib.axes
 import matplotlib.cm
 import matplotlib.collections
+import matplotlib.colorbar
 import matplotlib.colors
 import matplotlib.image
 import matplotlib.pyplot as plt
 import matplotlib.transforms
 import numpy as np
 import numpy.typing as npt
+from matplotlib.typing import ColorType
 
 
 class InversePowerNorm(matplotlib.colors.Normalize):
     r"""
     Linearly map a given value to the 0-1 range and then apply an inverse power-law
     normalization over that range.
 
@@ -465,40 +467,42 @@
     Parameters
     ----------
     ax
         Parent axes.
     image_only
         Only consider images as a valid mappable, by default `False`.
     silent
-        If `False`, raises a `RuntimeError`. If `True`, silently returns `None`.
+        If `False`, raises a `RuntimeError` when no mappable is found. If `True`,
+        silently returns `None`.
 
     Returns
     -------
     matplotlib.cm.ScalarMappable or None
 
     """
     if not image_only:
         try:
-            mappable = ax.collections[-1]
+            mappable: Any = ax.collections[-1]
         except (IndexError, AttributeError):
             mappable = None
 
     if image_only or mappable is None:
         try:
             mappable = ax.get_images()[-1]
         except (IndexError, AttributeError):
             mappable = None
 
-    if not silent and mappable is None:
-        raise RuntimeError(
-            "No mappable was found to use for colorbar "
-            "creation. First define a mappable such as "
-            "an image (with imshow) or a contour set ("
-            "with contourf)."
-        )
+    if mappable is None:
+        if not silent:
+            raise RuntimeError(
+                "No mappable was found to use for colorbar "
+                "creation. First define a mappable such as "
+                "an image (with imshow) or a contour set ("
+                "with contourf)."
+            )
     return mappable
 
 
 def unify_clim(
     axes: np.ndarray,
     target: matplotlib.axes.Axes | None = None,
     image_only: bool = False,
@@ -513,29 +517,37 @@
         The target axis to unify the color limits. If provided, the target color limits
         will be taken from this axes. Otherwise, the color limits will be set to include
         all mappables in the ``axes``.
     image_only
         If `True`, only consider mappables that are images. Default is `False`.
 
     """
+    vmn: float | None
+    vmx: float | None
+
     if target is None:
-        vmn, vmx = [], []
+        vmn_list, vmx_list = [], []
         for ax in axes.flat:
-            mappable = get_mappable(ax, image_only=image_only)
-            vmn.append(mappable.norm.vmin)
-            vmx.append(mappable.norm.vmax)
-        vmn, vmx = min(vmn), max(vmx)
-
+            mappable = get_mappable(ax, image_only=image_only, silent=True)
+            if mappable is not None:
+                if mappable.norm.vmin is not None:
+                    vmn_list.append(mappable.norm.vmin)
+                if mappable.norm.vmax is not None:
+                    vmx_list.append(mappable.norm.vmax)
+        vmn, vmx = min(vmn_list), max(vmx_list)
     else:
-        mappable = get_mappable(target, image_only=image_only)
-        vmn, vmx = mappable.norm.vmin, mappable.norm.vmax
+        mappable = get_mappable(target, image_only=image_only, silent=True)
+        if mappable is not None:
+            vmn, vmx = mappable.norm.vmin, mappable.norm.vmax
 
+    # Apply color limits
     for ax in axes.flat:
-        mappable = get_mappable(ax, image_only=image_only)
-        mappable.norm.vmin, mappable.norm.vmax = vmn, vmx
+        mappable = get_mappable(ax, image_only=image_only, silent=True)
+        if mappable is not None:
+            mappable.norm.vmin, mappable.norm.vmax = vmn, vmx
 
 
 def proportional_colorbar(
     mappable: matplotlib.cm.ScalarMappable | None = None,
     cax: matplotlib.axes.Axes | None = None,
     ax: matplotlib.axes.Axes | Iterable[matplotlib.axes.Axes] | None = None,
     **kwargs,
@@ -593,24 +605,31 @@
     fontsize = kwargs.pop("fontsize", None)
 
     if ax is None:
         if cax is None:
             ax = plt.gca()
             if mappable is None:
                 mappable = get_mappable(ax)
-    elif isinstance(ax, np.ndarray):
+    elif isinstance(ax, Iterable):
+        if not isinstance(ax, np.ndarray):
+            ax = np.array(ax, dtype=object)
         i = 0
         while mappable is None and i < len(ax.flat):
             mappable = get_mappable(ax.flatten()[i], silent=(i != (len(ax.flat) - 1)))
             i += 1
     elif mappable is None:
         mappable = get_mappable(ax)
 
+    if mappable is None:
+        raise RuntimeError("No mappable was found to use for colorbar creation")
+
     if mappable.colorbar is None:
         plt.colorbar(mappable=mappable, cax=cax, ax=ax, **kwargs)
+        mappable.colorbar = cast(matplotlib.colorbar.Colorbar, mappable.colorbar)
+
     ticks = mappable.colorbar.get_ticks()
     if cax is None:
         mappable.colorbar.remove()
     kwargs.setdefault("ticks", ticks)
     kwargs.setdefault("cmap", mappable.cmap)
     kwargs.setdefault("norm", mappable.norm)
     kwargs.setdefault("pad", 0.05)
@@ -714,14 +733,16 @@
         "lower left",
         "lower center",
         "lower right",
     ] = "upper right",
     **kwargs,
 ) -> matplotlib.axes.Axes:
     fig = parent_axes.get_figure()
+    if fig is None:
+        raise RuntimeError("Parent axes is not attached to a figure")
     locator = InsetAxesLocator(parent_axes, width, height, pad, loc)
     ax_ = fig.add_axes(locator(parent_axes, None).bounds, **kwargs)
     ax_.set_axes_locator(locator)
     return ax_
 
 
 class InsetAxesLocator:
@@ -804,15 +825,15 @@
     else:
         cax = _ez_inset(ax, w, h, pad=(-w - pad / 72, 0), **kwargs)
     return cax
 
 
 # TODO: fix colorbar size properly
 def nice_colorbar(
-    ax: matplotlib.axes.Axes | None = None,
+    ax: matplotlib.axes.Axes | Iterable[matplotlib.axes.Axes] | None = None,
     mappable: matplotlib.cm.ScalarMappable | None = None,
     width: float = 5.0,
     aspect: float = 5.0,
     pad: float = 3.0,
     minmax: bool = False,
     orientation: Literal["vertical", "horizontal"] = "vertical",
     floating=False,
@@ -870,27 +891,32 @@
             ax=ax,
             cax=_gen_cax(parent, width, aspect, pad, is_horizontal),
             orientation=orientation,
             **kwargs,
         )
 
     else:
-        if np.iterable(ax):
+        if isinstance(ax, Iterable):
+            if not isinstance(ax, np.ndarray):
+                ax = np.array(ax, dtype=object)
             bbox = matplotlib.transforms.Bbox.union(
                 [
                     x.get_window_extent().transformed(
                         x.figure.dpi_scale_trans.inverted()
                     )
                     for x in ax.flat
                 ]
             )
         else:
-            bbox = ax.get_window_extent().transformed(
-                ax.figure.dpi_scale_trans.inverted()
-            )
+            fig = ax.get_figure()
+
+            if fig is None:
+                raise RuntimeError("Axes is not attached to a figure")
+
+            bbox = ax.get_window_extent().transformed(fig.dpi_scale_trans.inverted())
 
         if orientation == "horizontal":
             kwargs["anchor"] = (1, 1)
             kwargs["location"] = "top"
             kwargs["fraction"] = width / (72 * bbox.height)
             kwargs["pad"] = pad / (72 * bbox.height)
             kwargs["shrink"] = width * aspect / (72 * bbox.width)
@@ -947,18 +973,29 @@
     rgb = rgba[:, :-1]
     a = rgba[:, -1][:, np.newaxis]
     rgb *= a
     rgb += (1 - a) * background
     return rgb.reshape(original_shape[:-1] + (3,))
 
 
+def _get_segment_for_color(
+    cmap: matplotlib.colors.LinearSegmentedColormap,
+    color: Literal["red", "green", "blue", "alpha"],
+) -> Any:
+    if hasattr(cmap, "_segmentdata"):
+        if color in cmap._segmentdata:
+            return cmap._segmentdata[color]
+    return None
+
+
 def _is_segment_iterable(cmap: matplotlib.colors.Colormap) -> bool:
     if not isinstance(cmap, matplotlib.colors.LinearSegmentedColormap):
         return False
-    if any(callable(cmap._segmentdata[c]) for c in ["red", "green", "blue"]):
+
+    if any(callable(_get_segment_for_color(cmap, c)) for c in ["red", "green", "blue"]):  # type: ignore[arg-type]
         return False
     return True
 
 
 def combined_cmap(
     cmap1: matplotlib.colors.Colormap | str,
     cmap2: matplotlib.colors.Colormap | str,
@@ -996,23 +1033,33 @@
     """
     if isinstance(cmap1, str):
         cmap1 = matplotlib.colormaps[cmap1]
     if isinstance(cmap2, str):
         cmap2 = matplotlib.colormaps[cmap2]
 
     if all(_is_segment_iterable(c) for c in (cmap1, cmap2)):
-        segnew = {}
+        cmap1 = cast(
+            matplotlib.colors.LinearSegmentedColormap, cmap1
+        )  # to appease mypy
+        cmap2 = cast(
+            matplotlib.colors.LinearSegmentedColormap, cmap2
+        )  # to appease mypy
+
+        segnew: dict[
+            Literal["red", "green", "blue", "alpha"], Sequence[tuple[float, ...]]
+        ] = {}
+
         for c in ["red", "green", "blue"]:
             seg1_c, seg2_c = (
-                np.asarray(cmap1._segmentdata[c]),
-                np.asarray(cmap2._segmentdata[c]),
+                np.asarray(_get_segment_for_color(cmap1, c)),  # type: ignore[arg-type]
+                np.asarray(_get_segment_for_color(cmap2, c)),  # type: ignore[arg-type]
             )
             seg1_c[:, 0] = seg1_c[:, 0] * 0.5
             seg2_c[:, 0] = seg2_c[:, 0] * 0.5 + 0.5
-            segnew[c] = np.r_[seg1_c, seg2_c]
+            segnew[c] = np.r_[seg1_c, seg2_c]  # type: ignore[index]
         cmap = matplotlib.colors.LinearSegmentedColormap(
             name=name, segmentdata=segnew, N=N
         )
     else:
         cmap = matplotlib.colors.LinearSegmentedColormap.from_list(
             name=name,
             colors=np.r_[
@@ -1025,19 +1072,19 @@
         matplotlib.colormaps.register(cmap.reversed())
     return cmap
 
 
 def gen_2d_colormap(
     ldat,
     cdat,
-    cmap: matplotlib.colors.Colormap | str = None,
+    cmap: matplotlib.colors.Colormap | str | None = None,
     *,
     lnorm: plt.Normalize | None = None,
     cnorm: plt.Normalize | None = None,
-    background: Any = None,
+    background: ColorType | None = None,
     N: int = 256,
 ):
     """Generate a 2D colormap image from lightness and color data.
 
     Parameters
     ----------
     ldat : array-like
@@ -1077,44 +1124,45 @@
     if lnorm is None:
         lnorm = plt.Normalize()
 
     if cnorm is None:
         cnorm = plt.Normalize()
 
     if background is None:
-        background: tuple[float, float, float] = (1, 1, 1, 1)
+        background_arr: tuple[float, float, float, float] = (1.0, 1.0, 1.0, 1.0)
     else:
-        background: tuple[float, float, float] = matplotlib.colors.to_rgba(background)
+        background_arr = matplotlib.colors.to_rgba(background)
 
     ldat_masked = np.ma.masked_invalid(ldat)
     cdat_masked = np.ma.masked_invalid(cdat)
 
     lnorm.autoscale_None(ldat_masked)
     cnorm.autoscale_None(cdat_masked)
 
     l_vals = lnorm(ldat_masked)
     c_vals = cnorm(cdat_masked)
     l_vals = l_vals[:, :, np.newaxis]
 
     img = cmap(c_vals)
     img *= l_vals
-    img += (1 - l_vals) * background
+    img += (1 - l_vals) * background_arr
 
-    l_linear = lnorm(np.linspace(lnorm.vmin, lnorm.vmax, N))[:, np.newaxis, np.newaxis]
-    cmap_img = np.repeat(
-        cmap(cnorm(np.linspace(cnorm.vmin, cnorm.vmax, N)))[np.newaxis, :], N, 0
-    )
+    lmin, lmax = cast(float, lnorm.vmin), cast(float, lnorm.vmax)  # to appease mypy
+    cmin, cmax = cast(float, cnorm.vmin), cast(float, cnorm.vmax)
+
+    l_linear = lnorm(np.linspace(lmin, lmax, N))[:, np.newaxis, np.newaxis]
+    cmap_img = np.repeat(cmap(cnorm(np.linspace(cmin, cmax, N)))[np.newaxis, :], N, 0)
     cmap_img *= l_linear
-    cmap_img += (1 - l_linear) * background
+    cmap_img += (1 - l_linear) * background_arr
 
     return cmap_img, img
 
 
-def color_distance(c1, c2) -> float:
-    """Calculate the color distance between two RGB colors.
+def color_distance(c1: ColorType, c2: ColorType) -> float:
+    """Calculate the color distance between two matplotlib colors.
 
     Parameters
     ----------
     c1, c2
         Color to calculate the distance between in any format that
         :func:`matplotlib.colors.to_rgb` can handle.
 
@@ -1139,15 +1187,15 @@
     dR2 = (R2 - R1) ** 2
     dG2 = (G2 - G1) ** 2
     dB2 = (B2 - B1) ** 2
     r = 0.5 * (R1 + R2) / 256
     return np.sqrt((2 + r) * dR2 + 4 * dG2 + (2 + 255 / 256 - r) * dB2)
 
 
-def close_to_white(c) -> bool:
+def close_to_white(c: ColorType) -> bool:
     """Check if a given color is closer to white than black.
 
     Parameters
     ----------
     c
         Color in any format that :func:`matplotlib.colors.to_rgb` can handle.
 
@@ -1184,15 +1232,17 @@
     Determines if an image is *light* or *dark* by checking whether the prominent color
     is closer to white than black.
 
     """
     return close_to_white(prominent_color(im))
 
 
-def axes_textcolor(ax: matplotlib.axes.Axes, light="k", dark="w"):
+def axes_textcolor(
+    ax: matplotlib.axes.Axes, light: ColorType = "k", dark: ColorType = "w"
+):
     """Determine the text color based on the color of the mappable in an axes.
 
     Parameters
     ----------
     ax
         The axes object for which the text color needs to be determined.
     light
```

### Comparing `erlab-2.3.0/src/erlab/plotting/erplot.py` & `erlab-2.3.1/src/erlab/plotting/erplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/plotting/general.py` & `erlab-2.3.1/src/erlab/plotting/general.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,19 @@
     "plot_array",
     "plot_array_2d",
     "plot_slices",
 ]
 
 import contextlib
 import copy
-from typing import TYPE_CHECKING, Any, Literal
+from collections.abc import Iterable
+from typing import TYPE_CHECKING, Any, Literal, Union, cast
 
 import matplotlib
-import matplotlib.colors as mcolors
+import matplotlib.colors
 import matplotlib.image
 import matplotlib.patches
 import matplotlib.path
 import matplotlib.pyplot as plt
 import numpy as np
 import numpy.typing as npt
 import xarray as xr
@@ -36,15 +37,15 @@
     _ez_inset,
     axes_textcolor,
     gen_2d_colormap,
     nice_colorbar,
 )
 
 if TYPE_CHECKING:
-    from collections.abc import Callable, Iterable, Sequence
+    from collections.abc import Callable, Collection, Sequence
 
 figure_width_ref = {
     "aps": [3.4, 7.0],
     "aip": [3.37, 6.69],
     "nature": [88 / 25.4, 180 / 25.4],
 }
 
@@ -115,28 +116,30 @@
         self,
         ax: matplotlib.axes.Axes,
         horizOn: bool = True,
         vertOn: bool = True,
         textOn: bool = True,
         useblit: bool = True,
         textprops: dict | None = None,
-        **lineprops: dict,
+        **lineprops,
     ):
         super().__init__(ax)
 
         if textprops is None:
             textprops = {}
 
-        self.connect_event("motion_notify_event", self.onmove)
-        self.connect_event("draw_event", self.clear)
+        self.connect_event("motion_notify_event", self.onmove)  # type: ignore[arg-type]
+        self.connect_event("draw_event", self.clear)  # type: ignore[arg-type]
 
         self.visible = True
         self.horizOn = horizOn
         self.vertOn = vertOn
         self.textOn = textOn
+        if self.canvas is None:
+            raise RuntimeError("No canvas found to attach to")
         self.useblit = useblit and self.canvas.supports_blit
 
         if self.useblit:
             lineprops["animated"] = True
             textprops["animated"] = True
 
         lcolor = lineprops.pop("color", lineprops.pop("c", "0.35"))
@@ -287,22 +290,22 @@
 def plot_array(
     arr: xr.DataArray,
     ax: matplotlib.axes.Axes | None = None,
     *,
     colorbar: bool = False,
     colorbar_kw: dict | None = None,
     gamma: float = 1.0,
-    norm: mcolors.Normalize | None = None,
+    norm: matplotlib.colors.Normalize | None = None,
     xlim: float | tuple[float, float] | None = None,
     ylim: float | tuple[float, float] | None = None,
     crop: bool = False,
     rad2deg: bool | Iterable[str] = False,
     func: Callable | None = None,
     func_args: dict | None = None,
-    **improps: dict,
+    **improps,
 ) -> matplotlib.image.AxesImage:
     """Plots a 2D :class:`xarray.DataArray` using :func:`matplotlib.pyplot.imshow`.
 
     Parameters
     ----------
     arr
         A two-dimensional :class:`xarray.DataArray` to be plotted.
@@ -336,20 +339,24 @@
     if colorbar_kw is None:
         colorbar_kw = {}
     if func_args is None:
         func_args = {}
 
     if isinstance(arr, np.ndarray):
         arr = xr.DataArray(arr)
+
     if ax is None:
         ax = plt.gca()
-    if xlim is not None and not np.iterable(xlim):
+
+    if xlim is not None and not isinstance(xlim, Iterable):
         xlim = (-xlim, xlim)
-    if ylim is not None and not np.iterable(ylim):
+
+    if ylim is not None and not isinstance(ylim, Iterable):
         ylim = (-ylim, ylim)
+
     if rad2deg is not False:
         if np.iterable(rad2deg):
             conv_dims = rad2deg
         else:
             conv_dims = [
                 d for d in ["phi", "theta", "beta", "alpha", "chi"] if d in arr.dims
             ]
@@ -364,15 +371,15 @@
         else:
             colorbar_kw.setdefault("extend", "min")
     elif "vmax" in improps:
         norm_kw["vmax"] = improps.pop("vmax")
         colorbar_kw.setdefault("extend", "max")
 
     if norm is None:
-        norm = copy.deepcopy(mcolors.PowerNorm(gamma, **norm_kw))
+        norm = copy.deepcopy(matplotlib.colors.PowerNorm(gamma, **norm_kw))
 
     improps_default = {
         "interpolation": "none",
         "extent": array_extent(arr),
         "aspect": "auto",
         "origin": "lower",
         "rasterized": True,
@@ -381,48 +388,53 @@
         improps.setdefault(k, v)
 
     if crop:
         if xlim is not None:
             arr = arr.copy(deep=True).sel({arr.dims[1]: slice(*xlim)})
         if ylim is not None:
             arr = arr.copy(deep=True).sel({arr.dims[0]: slice(*ylim)})
+
     if func is not None:
         img = ax.imshow(func(arr.values, **func_args), norm=norm, **improps)
     else:
         img = ax.imshow(arr.values, norm=norm, **improps)
-    ax.set_xlabel(arr.dims[1])
-    ax.set_ylabel(arr.dims[0])
+
+    ax.set_xlabel(str(arr.dims[1]))
+    ax.set_ylabel(str(arr.dims[0]))
     fancy_labels(ax)
+
     if xlim is not None:
         ax.set_xlim(*xlim)
     if ylim is not None:
         ax.set_ylim(*ylim)
+
     if colorbar:
         nice_colorbar(ax=ax, **colorbar_kw)
+
     return img
 
 
 def plot_array_2d(
     larr: xr.DataArray,
     carr: xr.DataArray,
     ax: matplotlib.axes.Axes | None = None,
     *,
     normalize_with_larr: bool = False,
     xlim: float | tuple[float, float] | None = None,
     ylim: float | tuple[float, float] | None = None,
-    cmap: mcolors.Colormap | str = None,
-    lnorm: mcolors.Normalize | None = None,
-    cnorm: mcolors.Normalize | None = None,
+    cmap: matplotlib.colors.Colormap | str | None = None,
+    lnorm: matplotlib.colors.Normalize | None = None,
+    cnorm: matplotlib.colors.Normalize | None = None,
     background: Any = None,
     colorbar: bool = True,
     cax: matplotlib.axes.Axes | None = None,
     colorbar_kw: dict | None = None,
     imshow_kw: dict | None = None,
     N: int = 256,
-    **indexers_kwargs: dict,
+    **indexers_kwargs,
 ):
     if lnorm is None:
         lnorm = plt.Normalize()
     else:
         lnorm = copy.deepcopy(lnorm)
     if cnorm is None:
         cnorm = plt.Normalize()
@@ -442,24 +454,27 @@
         imshow_kw.setdefault(k, v)
     if ax is None:
         ax = plt.gca()
 
     larr = larr.qsel(**indexers_kwargs).copy(deep=True)
     carr = carr.qsel(**indexers_kwargs).copy(deep=True)
     sel_kw = {}
+
     if xlim is not None:
-        if not np.iterable(xlim):
+        if not isinstance(xlim, Iterable):
             xlim = (-xlim, xlim)
         sel_kw[larr.dims[1]] = slice(*xlim)
+
     if ylim is not None:
-        if not np.iterable(ylim):
+        if not isinstance(ylim, Iterable):
             ylim = (-ylim, ylim)
         sel_kw[larr.dims[0]] = slice(*ylim)
-    larr = larr.sel(**sel_kw)
-    carr = carr.sel(**sel_kw)
+
+    larr = larr.sel(sel_kw)
+    carr = carr.sel(sel_kw)
 
     if normalize_with_larr:
         carr = carr / larr
 
     if lnorm is None:
         lnorm = plt.Normalize()
 
@@ -474,44 +489,55 @@
         cnorm=cnorm,
         background=background,
         N=N,
     )
 
     if colorbar:
         if cax is None:
+            fig = ax.get_figure()
+            if fig is None:
+                raise ValueError(
+                    "Cannot create colorbar without a figure. Please provide `cax`."
+                )
+
             colorbar_kw.setdefault("aspect", 2)
             colorbar_kw.setdefault("anchor", (0, 1))
             colorbar_kw.setdefault("panchor", (0, 1))
-            cb = ax.get_figure().colorbar(plt.cm.ScalarMappable(), ax=ax, **colorbar_kw)
+
+            cb = fig.colorbar(plt.cm.ScalarMappable(), ax=ax, **colorbar_kw)
             cax = cb.ax
             cax.clear()
 
+        lmin, lmax = cast(float, lnorm.vmin), cast(float, lnorm.vmax)  # to appease mypy
+        cmin, cmax = cast(float, cnorm.vmin), cast(float, cnorm.vmax)
+
         cax.imshow(
             cmap_img.transpose(1, 0, 2),
-            extent=(lnorm.vmin, lnorm.vmax, cnorm.vmin, cnorm.vmax),
+            extent=(lmin, lmax, cmin, cmax),
             origin="lower",
             aspect="auto",
         )
 
     im = ax.imshow(img, extent=array_extent(larr), **imshow_kw)
-    ax.set_xlabel(larr.dims[0])
-    ax.set_ylabel(larr.dims[1])
+    ax.set_xlabel(str(larr.dims[0]))
+    ax.set_ylabel(str(larr.dims[1]))
+    fancy_labels(ax)
 
     if colorbar:
         return im, cb
     else:
         return im, None
 
 
 def gradient_fill(
-    x: Sequence[int | float],
-    y: Sequence[int | float],
+    x: Collection[int | float],
+    y: Collection[int | float],
     y0: float | None = None,
     color: str | tuple[float, float, float] | tuple[float, float, float, float] = "C0",
-    cmap: str | mcolors.Colormap | None = None,
+    cmap: str | matplotlib.colors.Colormap | None = None,
     transpose: bool = False,
     reverse: bool = False,
     ax: matplotlib.axes.Axes | None = None,
     **kwargs,
 ) -> matplotlib.image.AxesImage:
     """Applies a gradient fill to a line plot.
 
@@ -539,41 +565,43 @@
     matplotlib.image.AxesImage
 
     """
     color = kwargs.pop("c", color)
     kwargs.setdefault("norm", InversePowerNorm(0.5))
     kwargs.setdefault("alpha", 0.75)
     if cmap is None:
-        cmap = mcolors.LinearSegmentedColormap.from_list(
-            "", colors=[(1, 1, 1, 0), mcolors.to_rgba(color)], N=1024
+        cmap = matplotlib.colors.LinearSegmentedColormap.from_list(
+            "", colors=[(1, 1, 1, 0), matplotlib.colors.to_rgba(color)], N=1024
         )
     if isinstance(cmap, str):
         cmap = matplotlib.colormaps[cmap]
     if reverse:
         cmap = cmap.reversed()
 
     if ax is None:
         ax = plt.gca()
     x, y = np.asarray(x), np.asarray(y)
     valid_inds = (~np.isnan(x)) * (~np.isnan(y))
     x, y = x[valid_inds], y[valid_inds]
 
     if y0 is None:
         y0 = min(y)
+
+    x = np.asarray(x)
     xn = np.r_[x[0], x, x[-1]]
     yn = np.r_[y0, y, y0]
     patch = matplotlib.patches.PathPatch(
         matplotlib.path.Path(np.array([xn, yn]).T), edgecolor="none", facecolor="none"
     )
     ax.add_patch(patch)
 
     im = matplotlib.image.AxesImage(
         ax, cmap=cmap, interpolation="bicubic", origin="lower", zorder=0, **kwargs
     )
-    im.use_sticky_edges = False
+    im.use_sticky_edges = False  # type: ignore[attr-defined]
     ax.add_artist(im)
     if transpose:
         im.set_data(np.linspace(0, 1, 1024).reshape(1024, 1).T)
     else:
         im.set_data(np.linspace(0, 1, 1024).reshape(1024, 1))
     # with autoscale_off(ax):
     im.set_extent((min(xn), max(xn), min(yn), max(yn)))
@@ -594,27 +622,34 @@
     axis: Literal[
         "on", "off", "equal", "scaled", "tight", "auto", "image", "scaled", "square"
     ] = "auto",
     show_all_labels: bool = False,
     colorbar: Literal["none", "right", "rightspan", "all"] = "none",
     hide_colorbar_ticks: bool = True,
     annotate: bool = True,
-    cmap: str | mcolors.Colormap | Iterable[mcolors.Colormap | str] | None = None,
-    norm: mcolors.Normalize | Iterable[mcolors.Normalize] | None = None,
+    cmap: str
+    | matplotlib.colors.Colormap
+    | Iterable[
+        str | matplotlib.colors.Colormap | Iterable[matplotlib.colors.Colormap | str]
+    ]
+    | None = None,
+    norm: matplotlib.colors.Normalize
+    | Iterable[matplotlib.colors.Normalize | Iterable[matplotlib.colors.Normalize]]
+    | None = None,
     order: Literal["C", "F"] = "C",
     cmap_order: Literal["C", "F"] = "C",
     norm_order: Literal["C", "F"] | None = None,
     gradient: bool = False,
     gradient_kw: dict | None = None,
     subplot_kw: dict | None = None,
     annotate_kw: dict | None = None,
     colorbar_kw: dict | None = None,
-    axes: npt.NDArray[matplotlib.axes.Axes] | None = None,
-    **values: dict,
-) -> tuple[matplotlib.figure.Figure, npt.NDArray[matplotlib.axes.Axes]]:
+    axes: Iterable[matplotlib.axes.Axes] | None = None,
+    **values,
+) -> tuple[matplotlib.figure.Figure, Iterable[matplotlib.axes.Axes]]:
     """Automated comparison plot of slices.
 
     Parameters
     ----------
     maps
         Arrays to plot.
     figsize
@@ -762,26 +797,26 @@
         slice_width = None
 
     else:
         slice_dim = next(k for k in slice_kw if not k.endswith("_width"))
         slice_levels = slice_kw[slice_dim]
         slice_width = kwargs.pop(slice_dim + "_width", None)
 
-    plot_dims = [d for d in dims if d != slice_dim]
+    plot_dims: list[str] = [str(d) for d in dims if d != slice_dim]
 
     if len(plot_dims) not in (1, 2):
         raise ValueError("The data to plot must be 1D or 2D")
 
-    if not np.iterable(slice_levels):
+    if not isinstance(slice_levels, Iterable):
         slice_levels = [slice_levels]
 
-    if xlim is not None and not np.iterable(xlim):
+    if xlim is not None and not isinstance(xlim, Iterable):
         xlim = (-xlim, xlim)
 
-    if ylim is not None and not np.iterable(ylim):
+    if ylim is not None and not isinstance(ylim, Iterable):
         ylim = (-ylim, ylim)
 
     auto_gradient_color = all(k not in gradient_kw for k in ("c", "color"))
 
     if hide_colorbar_ticks:
         colorbar_kw["ticks"] = []
 
@@ -792,27 +827,33 @@
         nrow, ncol = len(slice_levels), len(maps)
 
     elif order == "C":
         nrow, ncol = len(maps), len(slice_levels)
 
     cmap_name = cmap
     cmap_norm = norm
+
     if axes is None:
         fig, axes = plt.subplots(nrow, ncol, figsize=figsize, **subplot_kw)
-
+        axes = cast(npt.NDArray[Any], axes)
     else:
+        if not isinstance(axes, np.ndarray):
+            if not isinstance(axes, Iterable):
+                raise TypeError("axes must be an iterable of matplotlib.axes.Axes")
+            axes = np.array(axes, dtype=object)
+
         fig = axes.flat[0].get_figure()
 
     if nrow == 1:
         axes = axes[:, np.newaxis].reshape(1, -1)
 
     if ncol == 1:
         axes = axes[:, np.newaxis].reshape(-1, 1)
 
-    qsel_kw = {}
+    qsel_kw: dict[str, Any] = {}
 
     if crop:
         if len(plot_dims) == 1:
             if transpose and (ylim is not None):
                 qsel_kw[plot_dims[0]] = slice(*ylim)
 
             elif xlim is not None:
@@ -821,40 +862,49 @@
         elif len(plot_dims) == 2:
             if xlim is not None:
                 qsel_kw[plot_dims[1]] = slice(*xlim)
 
             if ylim is not None:
                 qsel_kw[plot_dims[0]] = slice(*ylim)
 
-    if slice_width is not None:
+    if slice_width is not None and slice_dim is not None:
         qsel_kw[slice_dim + "_width"] = slice_width
 
     for i in range(len(slice_levels)):
         if slice_dim is not None:
             qsel_kw[slice_dim] = slice_levels[i]
 
         for j in range(len(maps)):
             dat_sel = maps[j].copy(deep=True).qsel(**qsel_kw)
 
             if order == "F":
                 ax = axes[i, j]
             elif order == "C":
                 ax = axes[j, i]
 
-            if np.iterable(cmap_name) and not isinstance(cmap_name, str):
+            if isinstance(cmap_name, Iterable) and not isinstance(cmap_name, str):
+                cmap_name = list(cmap_name)
                 if cmap_order == "F":
-                    if isinstance(cmap_name[i], str):
+                    if isinstance(cmap_name[i], str | matplotlib.colors.Colormap):
                         cmap = cmap_name[i]
                     else:
-                        cmap = cmap_name[i][j]
+                        cmap = list(
+                            cast(
+                                Iterable[str | matplotlib.colors.Colormap], cmap_name[i]
+                            )
+                        )[j]
                 elif cmap_order == "C":
-                    if isinstance(cmap_name[j], str):
+                    if isinstance(cmap_name[j], str | matplotlib.colors.Colormap):
                         cmap = cmap_name[j]
                     else:
-                        cmap = cmap_name[j][i]
+                        cmap = list(
+                            cast(
+                                Iterable[str | matplotlib.colors.Colormap], cmap_name[j]
+                            )
+                        )[i]
             else:
                 cmap = cmap_name
 
             if len(plot_dims) == 1:
                 if cmap is not None:
                     kwargs["color"] = cmap
                     if auto_gradient_color:
@@ -880,29 +930,32 @@
 
                     if gradient:
                         gradient_fill(
                             dat_sel[plot_dims[0]], dat_sel.values, ax=ax, **gradient_kw
                         )
 
             elif len(plot_dims) == 2:
-                if np.iterable(cmap_norm):
+                if isinstance(cmap_norm, Iterable):
+                    cmap_norm = list(cmap_norm)
                     if norm_order == "F":
                         try:
-                            norm = cmap_norm[i][j]
+                            norm = list(cast(Iterable[plt.Normalize], cmap_norm[i]))[j]
                         except TypeError:
                             norm = cmap_norm[i]
 
                     elif norm_order == "C":
                         try:
-                            norm = cmap_norm[j][i]
+                            norm = list(cast(Iterable[plt.Normalize], cmap_norm[j]))[i]
                         except TypeError:
                             norm = cmap_norm[j]
                 else:
                     norm = copy.deepcopy(cmap_norm)
-                plot_array(dat_sel, ax=ax, norm=norm, cmap=cmap, **kwargs)
+                plot_array(
+                    dat_sel, ax=ax, norm=cast(plt.Normalize, norm), cmap=cmap, **kwargs
+                )
 
     if same_limits and len(plot_dims) == 2:
         vmn, vmx = [], []
         for ax in axes.flat:
             vmn.append(ax.get_images()[0].norm.vmin)
             vmx.append(ax.get_images()[0].norm.vmax)
         vmn, vmx = min(vmn), max(vmx)
@@ -935,20 +988,23 @@
             values={slice_dim: slice_levels * len(maps)},
             order=order,
             **annotate_kw,
         )
     return fig, axes
 
 
+MultipleLine2D = list[Union[matplotlib.lines.Line2D, "MultipleLine2D"]]
+
+
 def fermiline(
     ax: matplotlib.axes.Axes | None = None,
     value: float = 0.0,
     orientation: Literal["h", "v"] = "h",
     **kwargs,
-) -> matplotlib.lines.Line2D:
+) -> matplotlib.lines.Line2D | MultipleLine2D:
     """Plots a constant energy line to denote the Fermi level.
 
     Parameters
     ----------
     ax
         The `matplotlib.axes.Axes` to annotate.
     value
```

### Comparing `erlab-2.3.0/src/erlab/plotting/plot3d.py` & `erlab-2.3.1/src/erlab/plotting/plot3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 
 def set_3d_properties(self, verts, zs=0, zdir="z"):
     zs = np.broadcast_to(zs, len(verts))
     self._segment3d = np.asarray(
         [
             (*np.dot(_transform_zdir(zdir), (x, y, 0)), 0, 0, z)
-            for ((x, y), z) in zip(verts, zs)
+            for ((x, y), z) in zip(verts, zs, strict=True)
         ]
     )
 
 
 def pathpatch_translate(pathpatch, delta):
     pathpatch._segment3d += np.asarray(delta)
```

### Comparing `erlab-2.3.0/src/erlab/plotting/stylelib/fira.mplstyle` & `erlab-2.3.1/src/erlab/plotting/stylelib/fira.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/plotting/stylelib/firalight.mplstyle` & `erlab-2.3.1/src/erlab/plotting/stylelib/firalight.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/plotting/stylelib/khan.mplstyle` & `erlab-2.3.1/src/erlab/plotting/stylelib/khan.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/plotting/stylelib/nature.mplstyle` & `erlab-2.3.1/src/erlab/plotting/stylelib/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/plotting/stylelib/poster.mplstyle` & `erlab-2.3.1/src/erlab/plotting/stylelib/poster.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab/plotting/stylelib/times.mplstyle` & `erlab-2.3.1/src/erlab/plotting/stylelib/times.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/src/erlab.egg-info/PKG-INFO` & `erlab-2.3.1/src/erlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.3.0
+Version: 2.3.1
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -692,30 +692,27 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: h5netcdf>=1.2.0
 Requires-Dist: igor2>=0.5.6
-Requires-Dist: iminuit>=2.25.2
 Requires-Dist: joblib>=1.3.2
-Requires-Dist: lmfit<1.3.0,>=1.2.0
+Requires-Dist: lmfit!=1.3.0,>=1.2.0
 Requires-Dist: matplotlib>=3.8.0
-Requires-Dist: numba-progress>=1.0.0
 Requires-Dist: numba>=0.59.0
 Requires-Dist: numbagg>=0.8.1
 Requires-Dist: numpy>=1.26.0
 Requires-Dist: pyperclip>=1.8.2
 Requires-Dist: pyqtgraph>=0.13.1
 Requires-Dist: qtawesome>=1.3.1
 Requires-Dist: qtpy>=2.4.1
 Requires-Dist: scipy>=1.12.0
-Requires-Dist: superqt>=0.6.2
 Requires-Dist: tqdm>=4.66.2
-Requires-Dist: uncertainties>=3.0.1
+Requires-Dist: uncertainties>=3.1.4
 Requires-Dist: varname>=0.13.0
 Requires-Dist: xarray>=2024.02.0
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
```

### Comparing `erlab-2.3.0/src/erlab.egg-info/SOURCES.txt` & `erlab-2.3.1/src/erlab.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 docs/make.bat
 docs/requirements.txt
 docs/source/bibliography.rst
 docs/source/conf.py
 docs/source/contributing.rst
 docs/source/erlab.accessors.rst
 docs/source/erlab.analysis.rst
-docs/source/erlab.characterization.rst
 docs/source/erlab.constants.rst
 docs/source/erlab.interactive.rst
 docs/source/erlab.io.rst
 docs/source/erlab.lattice.rst
 docs/source/erlab.parallel.rst
 docs/source/erlab.plotting.rst
 docs/source/getting-started.rst
@@ -76,16 +75,14 @@
 src/erlab/analysis/fit/spline.py
 src/erlab/analysis/fit/functions/__init__.py
 src/erlab/analysis/fit/functions/dynamic.py
 src/erlab/analysis/fit/functions/general.py
 src/erlab/analysis/mask/__init__.py
 src/erlab/analysis/mask/polygon.py
 src/erlab/characterization/__init__.py
-src/erlab/characterization/resistance.py
-src/erlab/characterization/xrd.py
 src/erlab/interactive/__init__.py
 src/erlab/interactive/bzplot.py
 src/erlab/interactive/colors.py
 src/erlab/interactive/curvefittingtool.py
 src/erlab/interactive/derivative.py
 src/erlab/interactive/dtool.ui
 src/erlab/interactive/fermiedge.py
@@ -102,14 +99,17 @@
 src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
 src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
 src/erlab/io/__init__.py
 src/erlab/io/dataloader.py
 src/erlab/io/exampledata.py
 src/erlab/io/igor.py
 src/erlab/io/utilities.py
+src/erlab/io/characterization/__init__.py
+src/erlab/io/characterization/resistance.py
+src/erlab/io/characterization/xrd.py
 src/erlab/io/plugins/__init__.py
 src/erlab/io/plugins/da30.py
 src/erlab/io/plugins/kriss.py
 src/erlab/io/plugins/merlin.py
 src/erlab/io/plugins/ssrl52.py
 src/erlab/plotting/__init__.py
 src/erlab/plotting/annotations.py
```

### Comparing `erlab-2.3.0/templates/.macros.j2` & `erlab-2.3.1/templates/.macros.j2`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/tests/accessors/test_fit.py` & `erlab-2.3.1/tests/accessors/test_fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,17 @@
     p_guess = [0.0, 0.5]
 
     if use_dask:
         da = da.chunk({"x": 1})
 
     # params as DataArray of JSON strings
     params = []
-    for a, p, f in zip(a_guess, p_guess, np.full_like(da.x, 2, dtype=float)):
+    for a, p, f in zip(
+        a_guess, p_guess, np.full_like(da.x, 2, dtype=float), strict=True
+    ):
         params.append(lmfit.create_params(a=a, p=p, f=f).dumps())
     params = xr.DataArray(params, coords=[da.x])
     fit = da.modelfit(
         coords=[da.t],
         model=lmfit.Model(sine),
         params=params,
     )
```

### Comparing `erlab-2.3.0/tests/accessors/test_kspace.py` & `erlab-2.3.1/tests/accessors/test_kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/tests/analysis/test_fastbinning.py` & `erlab-2.3.1/tests/analysis/test_fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/tests/analysis/test_fit_functions_dynamic.py` & `erlab-2.3.1/tests/analysis/test_fit_functions_dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     assert isinstance(result, xr.DataArray)
     assert np.allclose(result, expected_result)
 
     # Test case 3: Evaluate polynomial function with parameters
     x = np.arange(5, dtype=np.float64)
     coeffs = RAND_STATE.randn(3)
     expected_result = np.polyval(np.asarray(list(reversed(coeffs))), x)
-    params = dict(zip([f"c{i}" for i in range(3)], coeffs))
+    params = dict(zip([f"c{i}" for i in range(3)], coeffs, strict=True))
     result = PolynomialFunction(degree=2)(x, **params)
     assert np.allclose(result, expected_result)
 
 
 def test_multi_peak_function_call():
     # Test case 1: Evaluate multi-peak function with numpy array input
     x = np.linspace(-5, 5, 20, dtype=np.float64)
```

### Comparing `erlab-2.3.0/tests/analysis/test_fit_functions_general.py` & `erlab-2.3.1/tests/analysis/test_fit_functions_general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/tests/analysis/test_fit_models.py` & `erlab-2.3.1/tests/analysis/test_fit_models.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/tests/analysis/test_image.py` & `erlab-2.3.1/tests/analysis/test_image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/tests/analysis/test_interpolate.py` & `erlab-2.3.1/tests/analysis/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/tests/analysis/test_kspace.py` & `erlab-2.3.1/tests/analysis/test_kspace.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,26 +14,28 @@
         erlab.analysis.kspace._kconv_func_type2,
     ):
         for delta, xi, xi0, beta0 in zip(
             [0, 90.0, -90.0],
             [0, 30.0, -30.0],
             [0.0, 10.0, -10.0],
             [0.0, 10.0, -10.0],
+            strict=True,
         ):
             funcs.append(kconv_func(k_tot, delta, xi, xi0, beta0))
     for kconv_func in (
         erlab.analysis.kspace._kconv_func_type1_da,
         erlab.analysis.kspace._kconv_func_type2_da,
     ):
         for delta, chi, chi0, xi, xi0 in zip(
             [0, 90.0, -90.0],
             [0, 10.0, -30.0],
             [0.0, 10.0, -10.0],
             [0.0, 10.0, -10.0],
             [0.0, 10.0, -10.0],
+            strict=True,
         ):
             funcs.append(kconv_func(k_tot, delta, chi, chi0, xi, xi0))
     return funcs
 
 
 def test_transform():
     for forward_func, inverse_func in _generate_funclist():
```

### Comparing `erlab-2.3.0/tests/analysis/test_utilities.py` & `erlab-2.3.1/tests/analysis/test_utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.3.0/tests/io/test_dataloader.py` & `erlab-2.3.1/tests/io/test_dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import csv
 import datetime
 import glob
 import os
 import re
 import tempfile
+from typing import ClassVar
 
 import erlab.io
 import numpy as np
 import pandas as pd
-from erlab.io.exampledata import generate_data_angles
 from erlab.io.dataloader import LoaderBase
+from erlab.io.exampledata import generate_data_angles
 
 
 def make_data(beta=5.0, temp=20.0, hv=50.0, bandshift=0.0):
     data = generate_data_angles(
         shape=(250, 1, 300),
         angrange={"alpha": (-15, 15), "beta": (beta, beta)},
         hv=hv,
@@ -84,17 +85,17 @@
 
     # List the generated files
     sorted(os.listdir(tmp_dir.name))
 
     class ExampleLoader(LoaderBase):
         name = "example"
 
-        aliases = ["Ex"]
+        aliases = ("Ex",)
 
-        name_map = {
+        name_map: ClassVar[dict] = {
             "eV": "BindingEnergy",
             "alpha": "ThetaX",
             "beta": [
                 "Polar",
                 "Polar Compens",
             ],  # Can have multiple names assigned to the same name
             "delta": "Azimuth",
@@ -103,29 +104,29 @@
             "y": "Y",
             "z": "Z",
             "hv": "PhotonEnergy",
             "polarization": "UndPol",
             "temp_sample": "TB",
         }
 
-        coordinate_attrs: tuple[str, ...] = (
+        coordinate_attrs = (
             "beta",
             "delta",
             "xi",
             "hv",
             "x",
             "y",
             "z",
             "polarization",
             "photon_flux",
         )
         # Attributes to be used as coordinates. Place all attributes that we don't want to
         # lose when merging multiple file scans here.
 
-        additional_attrs = {
+        additional_attrs: ClassVar[dict] = {
             "configuration": 1,  # Experimental geometry. Required for momentum conversion
             "sample_workfunction": 4.3,
         }  # Any additional metadata you want to add to the data
 
         skip_validate = False
 
         always_single = False
```


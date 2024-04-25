# Comparing `tmp/pyroomacoustics-0.7.3.tar.gz` & `tmp/pyroomacoustics-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroomacoustics-0.7.3.tar", last modified: Mon Dec  5 08:00:15 2022, max compression
+gzip compressed data, was "pyroomacoustics-0.7.4.tar", last modified: Thu Apr 25 16:07:16 2024, max compression
```

## Comparing `pyroomacoustics-0.7.3.tar` & `pyroomacoustics-0.7.4.tar`

### file list

```diff
@@ -1,520 +1,524 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.074282 pyroomacoustics-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2022-12-05 07:56:05.000000 pyroomacoustics-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      809 2022-12-05 07:56:05.000000 pyroomacoustics-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2022-12-05 08:00:15.074282 pyroomacoustics-0.7.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    12344 2022-12-05 07:56:05.000000 pyroomacoustics-0.7.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      338 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.006283 pyroomacoustics-0.7.3/pyroomacoustics/
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18958 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/acoustics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.010283 pyroomacoustics-0.7.3/pyroomacoustics/adaptive/
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/adaptive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/adaptive/adaptive_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/adaptive/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/adaptive/lms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/adaptive/rls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/adaptive/subband_lms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.010283 pyroomacoustics-0.7.3/pyroomacoustics/adaptive/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/adaptive/tests/test_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/adaptive/tests/test_adaptive_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/adaptive/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    47884 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/beamforming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.014283 pyroomacoustics-0.7.3/pyroomacoustics/bss/
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/bss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8743 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/bss/auxiva.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/bss/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9143 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/bss/fastmnmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7899 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/bss/fastmnmf2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6616 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/bss/ilrma.py
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/bss/sparseauxiva.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.014283 pyroomacoustics-0.7.3/pyroomacoustics/bss/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/bss/tests/test_bss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/bss/tests/test_trinicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/bss/trinicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/build_rir.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.014283 pyroomacoustics-0.7.3/pyroomacoustics/data/
--rw-r--r--   0 runner    (1001) docker     (123)    17123 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/data/materials.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.014283 pyroomacoustics-0.7.3/pyroomacoustics/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10431 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/datasets/cmu_arctic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/datasets/google_speech_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.014283 pyroomacoustics-0.7.3/pyroomacoustics/datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/datasets/tests/test_corpus_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/datasets/tests/test_download_uncompress.py
--rw-r--r--   0 runner    (1001) docker     (123)    15585 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/datasets/timit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.014283 pyroomacoustics-0.7.3/pyroomacoustics/denoise/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/denoise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15361 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/denoise/iterative_wiener.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/denoise/spectral_subtraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11791 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/denoise/subspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    10895 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/directivities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.018283 pyroomacoustics-0.7.3/pyroomacoustics/doa/
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/doa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/doa/cssm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/doa/detect_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)    19496 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/doa/doa.py
--rw-r--r--   0 runner    (1001) docker     (123)     9468 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/doa/frida.py
--rw-r--r--   0 runner    (1001) docker     (123)    12493 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/doa/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6409 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/doa/music.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/doa/normmusic.py
--rw-r--r--   0 runner    (1001) docker     (123)    16268 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/doa/plotters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/doa/srp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.018283 pyroomacoustics-0.7.3/pyroomacoustics/doa/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/doa/tests/test_doa.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/doa/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    69516 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/doa/tools_fri_doa_plane.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/doa/tops.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/doa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/doa/waves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.022283 pyroomacoustics-0.7.3/pyroomacoustics/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/experimental/deconvolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/experimental/delay_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/experimental/localization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9728 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/experimental/measure_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/experimental/physics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12723 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/experimental/point_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/experimental/rt60.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/experimental/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.022283 pyroomacoustics-0.7.3/pyroomacoustics/experimental/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/experimental/tests/test_deconvolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/experimental/tests/test_measure_rt60.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.022283 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/common.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:14.994283 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.026283 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/COPYING.BSD
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/COPYING.GPL
--rw-r--r--   0 runner    (1001) docker     (123)    26530 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/COPYING.LGPL
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/COPYING.MINPACK
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/COPYING.MPL2
--rw-r--r--   0 runner    (1001) docker     (123)      779 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/COPYING.README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.030283 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/Cholesky
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/CholmodSupport
--rw-r--r--   0 runner    (1001) docker     (123)    17969 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/Core
--rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/Dense
--rw-r--r--   0 runner    (1001) docker     (123)       35 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/Eigen
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/Eigenvalues
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/Geometry
--rw-r--r--   0 runner    (1001) docker     (123)      874 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/Householder
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/IterativeLinearSolvers
--rw-r--r--   0 runner    (1001) docker     (123)      939 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/Jacobi
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/LU
--rw-r--r--   0 runner    (1001) docker     (123)      991 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/MetisSupport
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/OrderingMethods
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/PaStiXSupport
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/PardisoSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/QR
--rw-r--r--   0 runner    (1001) docker     (123)      945 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/QtAlignedMalloc
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/SPQRSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/SVD
--rw-r--r--   0 runner    (1001) docker     (123)      919 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/Sparse
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/SparseCholesky
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/SparseCore
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/SparseLU
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/SparseQR
--rw-r--r--   0 runner    (1001) docker     (123)      797 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/StdDeque
--rw-r--r--   0 runner    (1001) docker     (123)      726 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/StdList
--rw-r--r--   0 runner    (1001) docker     (123)      803 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/StdVector
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/SuperLUSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/UmfPackSupport
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.002283 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.030283 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Cholesky/
--rw-r--r--   0 runner    (1001) docker     (123)    24440 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Cholesky/LDLT.h
--rw-r--r--   0 runner    (1001) docker     (123)    18395 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Cholesky/LLT.h
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.030283 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/CholmodSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    22307 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.038282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/
--rw-r--r--   0 runner    (1001) docker     (123)    12218 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Array.h
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Assign.h
--rw-r--r--   0 runner    (1001) docker     (123)    38153 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/AssignEvaluator.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    12479 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0 runner    (1001) docker     (123)    13910 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    18064 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Block.h
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/BooleanRedux.h
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0 runner    (1001) docker     (123)     6970 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0 runner    (1001) docker     (123)    62197 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0 runner    (1001) docker     (123)     7593 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    31424 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0 runner    (1001) docker     (123)    27420 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/DenseBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    24212 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    21959 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Diagonal.h
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)      970 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Dot.h
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/EigenBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0 runner    (1001) docker     (123)    21123 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)    22185 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/IO.h
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Inverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Map.h
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/MapBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    40402 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    19170 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    22154 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/NestByValue.h
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/NoAlias.h
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/NumTraits.h
--rw-r--r--   0 runner    (1001) docker     (123)    21646 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    45180 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Product.h
--rw-r--r--   0 runner    (1001) docker     (123)    49497 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Random.h
--rw-r--r--   0 runner    (1001) docker     (123)    17852 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Redux.h
--rw-r--r--   0 runner    (1001) docker     (123)    12800 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Ref.h
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Replicate.h
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Reverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Select.h
--rw-r--r--   0 runner    (1001) docker     (123)    14245 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Solve.h
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/SolverBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/StableNorm.h
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Stride.h
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Swap.h
--rw-r--r--   0 runner    (1001) docker     (123)    14777 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Transpose.h
--rw-r--r--   0 runner    (1001) docker     (123)    14386 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Transpositions.h
--rw-r--r--   0 runner    (1001) docker     (123)    37234 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0 runner    (1001) docker     (123)    29441 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     8074 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Visitor.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:14.998283 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.038282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX/
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    27787 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.038282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX512/
--rw-r--r--   0 runner    (1001) docker     (123)    15733 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    50936 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.042282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AltiVec/
--rw-r--r--   0 runner    (1001) docker     (123)    16443 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    37671 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.042282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    22059 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/Half.h
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    10744 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    35442 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.042282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/Default/
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/Default/Settings.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.042282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/NEON/
--rw-r--r--   0 runner    (1001) docker     (123)    17706 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    28726 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/NEON/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.042282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/SSE/
--rw-r--r--   0 runner    (1001) docker     (123)    19426 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    35825 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.042282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/ZVector/
--rw-r--r--   0 runner    (1001) docker     (123)    15366 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    32283 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.042282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)    18263 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)      607 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)    27944 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/UnaryFunctors.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.046282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/
--rw-r--r--   0 runner    (1001) docker     (123)    81106 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (123)    18478 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    15188 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    26808 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0 runner    (1001) docker     (123)    19632 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    11198 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     9901 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0 runner    (1001) docker     (123)    20403 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    13743 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    14722 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    13979 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularSolverVector.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.046282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/
--rwxr-xr-x   0 runner    (1001) docker     (123)    15722 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0 runner    (1001) docker     (123)    21579 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/Constants.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     3564 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (123)    14150 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/ForwardDeclarations.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     4026 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0 runner    (1001) docker     (123)    36570 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/Macros.h
--rw-r--r--   0 runner    (1001) docker     (123)    40154 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/Memory.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    19365 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/Meta.h
--rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/NonMPL2.h
--rw-r--r--   0 runner    (1001) docker     (123)      809 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (123)    10518 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0 runner    (1001) docker     (123)    34198 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/XprHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.050282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/
--rw-r--r--   0 runner    (1001) docker     (123)    12558 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    17021 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    22944 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/EigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    17176 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    14351 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-r--r--   0 runner    (1001) docker     (123)    23586 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/RealQZ.h
--rw-r--r--   0 runner    (1001) docker     (123)    20288 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/RealSchur.h
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    33674 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    22444 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.050282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/AlignedBox.h
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/AngleAxis.h
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/EulerAngles.h
--rw-r--r--   0 runner    (1001) docker     (123)    20539 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Homogeneous.h
--rw-r--r--   0 runner    (1001) docker     (123)    11961 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Hyperplane.h
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/OrthoMethods.h
--rw-r--r--   0 runner    (1001) docker     (123)     8308 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/ParametrizedLine.h
--rw-r--r--   0 runner    (1001) docker     (123)    32152 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Quaternion.h
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Rotation2D.h
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/RotationBase.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     6324 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Scaling.h
--rw-r--r--   0 runner    (1001) docker     (123)    60514 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Transform.h
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Translation.h
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Umeyama.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.050282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/arch/
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/arch/Geometry_SSE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.050282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Householder/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Householder/BlockHouseholder.h
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Householder/Householder.h
--rw-r--r--   0 runner    (1001) docker     (123)    20603 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Householder/HouseholderSequence.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.054282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-r--r--   0 runner    (1001) docker     (123)     9184 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (123)    15062 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-r--r--   0 runner    (1001) docker     (123)    15234 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-r--r--   0 runner    (1001) docker     (123)    11527 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.054282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Jacobi/
--rw-r--r--   0 runner    (1001) docker     (123)    15957 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Jacobi/Jacobi.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.054282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/Determinant.h
--rw-r--r--   0 runner    (1001) docker     (123)    32803 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/FullPivLU.h
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/InverseImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    21478 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/PartialPivLU.h
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.054282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/arch/
--rw-r--r--   0 runner    (1001) docker     (123)    13669 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/arch/Inverse_SSE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.054282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/MetisSupport/
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/MetisSupport/MetisSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.054282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/OrderingMethods/
--rw-r--r--   0 runner    (1001) docker     (123)    16396 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/OrderingMethods/Amd.h
--rw-r--r--   0 runner    (1001) docker     (123)    62266 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/OrderingMethods/Ordering.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.054282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/PaStiXSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    22248 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.054282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/PardisoSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    20032 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.054282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/
--rw-r--r--   0 runner    (1001) docker     (123)    24881 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/ColPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    20805 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (123)    25478 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/FullPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/HouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.054282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SPQRSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    11405 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.058282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/
--rw-r--r--   0 runner    (1001) docker     (123)    48778 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/BDCSVD.h
--rw-r--r--   0 runner    (1001) docker     (123)    32949 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/JacobiSVD.h
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    12650 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/SVDBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    15957 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/UpperBidiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.058282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCholesky/
--rw-r--r--   0 runner    (1001) docker     (123)    24010 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.062282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/
--rw-r--r--   0 runner    (1001) docker     (123)    10537 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/AmbiVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/CompressedStorage.h
--rw-r--r--   0 runner    (1001) docker     (123)    13178 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseAssign.h
--rw-r--r--   0 runner    (1001) docker     (123)    25592 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseBlock.h
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseColEtree.h
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    25840 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    12487 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseDot.h
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseFuzzy.h
--rw-r--r--   0 runner    (1001) docker     (123)    12589 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseMap.h
--rw-r--r--   0 runner    (1001) docker     (123)    52349 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    17923 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparsePermutation.h
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseRedux.h
--rw-r--r--   0 runner    (1001) docker     (123)    15492 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseRef.h
--rw-r--r--   0 runner    (1001) docker     (123)    25715 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseTranspose.h
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseTriangularView.h
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseUtil.h
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseView.h
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/TriangularSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.062282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/
--rw-r--r--   0 runner    (1001) docker     (123)    27923 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU.h
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLUImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-r--r--   0 runner    (1001) docker     (123)    10022 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.062282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseQR/
--rw-r--r--   0 runner    (1001) docker     (123)    28373 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseQR/SparseQR.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.062282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/StlSupport/
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/StlSupport/StdDeque.h
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/StlSupport/StdList.h
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/StlSupport/StdVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/StlSupport/details.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.062282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SuperLUSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    34341 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.062282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/UmfPackSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    17202 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.066282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/Image.h
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/Kernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/RealSvd2x2.h
--rw-r--r--   0 runner    (1001) docker     (123)    30560 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/blas.h
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/lapack.h
--rwxr-xr-x   0 runner    (1001) docker     (123)  1058368 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/lapacke.h
--rw-r--r--   0 runner    (1001) docker     (123)      474 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/lapacke_mangling.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.066282 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)    13132 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    16929 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    37403 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2022-12-05 07:56:09.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    12168 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/geometry.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/geometry.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12313 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/libroom.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/microphone.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    36541 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/room.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/room.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10388 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/wall.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/wall.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10012 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/multirate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16514 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.066282 pyroomacoustics-0.7.3/pyroomacoustics/phase/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/phase/gl.py
--rw-r--r--   0 runner    (1001) docker     (123)    12717 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)   114165 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/room.py
--rw-r--r--   0 runner    (1001) docker     (123)    13564 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/soundsource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.070282 pyroomacoustics-0.7.3/pyroomacoustics/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_anechoic_room.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_angle_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_autocorr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_bandpass_filterbank.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_build_rir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_create_noisy_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_issue_115.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_issue_162.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_issue_22.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_issue_235.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_issue_236.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_issue_69.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_issue_87.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_rake_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_random_ism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_room_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_room_is_insided.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_room_mix.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_room_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_rt60.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_shoebox_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_soundsource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_source_directivities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_source_directivity_flipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_visibility_shoebox2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_visibility_shoebox3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_visibility_uroom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/test_volume_area.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.070282 pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/test_ccw3p.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/test_geometry_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/test_is_inside_2d_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/test_ray_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/test_room_construct.py
--rw-r--r--   0 runner    (1001) docker     (123)    15834 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/test_room_walls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/test_shoebox_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/test_wall_construct.py
--rw-r--r--   0 runner    (1001) docker     (123)    11472 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/test_wall_intersection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/test_wall_side_reflect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.070282 pyroomacoustics-0.7.3/pyroomacoustics/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/transform/dft.py
--rw-r--r--   0 runner    (1001) docker     (123)    29407 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/transform/stft.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.074282 pyroomacoustics-0.7.3/pyroomacoustics/transform/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/transform/tests/test_dft.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/transform/tests/test_dft_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)    33318 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/transform/tests/test_stft.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/transform/tests/test_stft_oneshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/transform/tests/test_stft_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)    21729 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21427 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/pyroomacoustics/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:00:15.010283 pyroomacoustics-0.7.3/pyroomacoustics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2022-12-05 08:00:14.000000 pyroomacoustics-0.7.3/pyroomacoustics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27919 2022-12-05 08:00:14.000000 pyroomacoustics-0.7.3/pyroomacoustics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 08:00:14.000000 pyroomacoustics-0.7.3/pyroomacoustics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 07:56:39.000000 pyroomacoustics-0.7.3/pyroomacoustics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2022-12-05 08:00:14.000000 pyroomacoustics-0.7.3/pyroomacoustics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-05 08:00:14.000000 pyroomacoustics-0.7.3/pyroomacoustics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-05 08:00:15.074282 pyroomacoustics-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2022-12-05 07:56:06.000000 pyroomacoustics-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.978135 pyroomacoustics-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-04-25 16:07:16.978135 pyroomacoustics-0.7.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12460 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.886136 pyroomacoustics-0.7.4/pyroomacoustics/
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18956 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/acoustics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.890136 pyroomacoustics-0.7.4/pyroomacoustics/adaptive/
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/adaptive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/adaptive/adaptive_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/adaptive/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/adaptive/lms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/adaptive/rls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/adaptive/subband_lms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.890136 pyroomacoustics-0.7.4/pyroomacoustics/adaptive/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/adaptive/tests/test_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/adaptive/tests/test_adaptive_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/adaptive/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47859 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/beamforming.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.894136 pyroomacoustics-0.7.4/pyroomacoustics/bss/
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/bss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/bss/auxiva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/bss/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/bss/fastmnmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/bss/fastmnmf2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/bss/ilrma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/bss/sparseauxiva.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.894136 pyroomacoustics-0.7.4/pyroomacoustics/bss/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/bss/tests/test_bss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/bss/tests/test_trinicon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/bss/trinicon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/build_rir.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.894136 pyroomacoustics-0.7.4/pyroomacoustics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    17123 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/data/materials.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.894136 pyroomacoustics-0.7.4/pyroomacoustics/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/datasets/cmu_arctic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/datasets/google_speech_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.894136 pyroomacoustics-0.7.4/pyroomacoustics/datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/datasets/tests/test_corpus_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/datasets/tests/test_download_uncompress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15582 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/datasets/timit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.894136 pyroomacoustics-0.7.4/pyroomacoustics/denoise/
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/denoise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15284 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/denoise/iterative_wiener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/denoise/spectral_subtraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11765 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/denoise/subspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/directivities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.898136 pyroomacoustics-0.7.4/pyroomacoustics/doa/
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/doa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/doa/cssm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/doa/detect_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19483 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/doa/doa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9460 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/doa/frida.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12479 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/doa/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/doa/music.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/doa/normmusic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16261 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/doa/plotters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/doa/srp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.898136 pyroomacoustics-0.7.4/pyroomacoustics/doa/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/doa/tests/test_doa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/doa/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69514 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/doa/tools_fri_doa_plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/doa/tops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/doa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/doa/waves.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.902136 pyroomacoustics-0.7.4/pyroomacoustics/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/experimental/deconvolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/experimental/delay_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/experimental/localization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/experimental/measure_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/experimental/physics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12719 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/experimental/point_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/experimental/rt60.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/experimental/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.902136 pyroomacoustics-0.7.4/pyroomacoustics/experimental/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/experimental/tests/test_deconvolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/experimental/tests/test_measure_rt60.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.902136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/common.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.878136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.906136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/COPYING.BSD
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/COPYING.GPL
+-rw-r--r--   0 runner    (1001) docker     (127)    26530 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/COPYING.LGPL
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/COPYING.MINPACK
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/COPYING.MPL2
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/COPYING.README
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.910136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/Cholesky
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/CholmodSupport
+-rw-r--r--   0 runner    (1001) docker     (127)    17969 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/Core
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/Dense
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/Eigen
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/Eigenvalues
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/Geometry
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/Householder
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/IterativeLinearSolvers
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/Jacobi
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/LU
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/MetisSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/OrderingMethods
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/PaStiXSupport
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1116 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/PardisoSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/QR
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/QtAlignedMalloc
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/SPQRSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/SVD
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/Sparse
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/SparseCholesky
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/SparseCore
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/SparseLU
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/SparseQR
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/StdDeque
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/StdList
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/StdVector
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/SuperLUSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/UmfPackSupport
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.882136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.910136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Cholesky/
+-rw-r--r--   0 runner    (1001) docker     (127)    24440 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18395 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.910136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/CholmodSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    22307 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.926136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/
+-rw-r--r--   0 runner    (1001) docker     (127)    12218 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Assign.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38153 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/AssignEvaluator.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12479 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13910 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18064 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Block.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/BooleanRedux.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    62197 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31424 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27420 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24212 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21959 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12666 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11507 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Dot.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21123 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22185 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/IO.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Map.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40402 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19170 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22154 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21646 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    45180 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Product.h
+-rw-r--r--   0 runner    (1001) docker     (127)    49497 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Random.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Redux.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12800 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Ref.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Select.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Solve.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Stride.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Swap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14386 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    37234 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29441 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.878136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.926136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 runner    (1001) docker     (127)    18037 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17776 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27787 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.926136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 runner    (1001) docker     (127)    15733 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    50936 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.926136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 runner    (1001) docker     (127)    16443 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10797 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37671 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.930136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22059 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/Half.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10744 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35442 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.930136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/Default/Settings.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.930136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 runner    (1001) docker     (127)    17706 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28726 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/NEON/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.930136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 runner    (1001) docker     (127)    19426 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18888 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35825 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.930136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 runner    (1001) docker     (127)    15366 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32283 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.934136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18263 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27944 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.938136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/
+-rw-r--r--   0 runner    (1001) docker     (127)    81106 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18478 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15188 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26808 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19632 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20403 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13979 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.938136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15722 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21579 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/Constants.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3564 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14150 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/ForwardDeclarations.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4026 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 runner    (1001) docker     (127)    36570 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40154 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/Memory.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19365 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10518 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34198 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.942136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/
+-rw-r--r--   0 runner    (1001) docker     (127)    12558 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17021 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22944 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9715 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23586 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20288 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    33674 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22444 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.946136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20539 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32152 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/RotationBase.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6324 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0 runner    (1001) docker     (127)    60514 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Umeyama.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.946136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/arch/Geometry_SSE.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.946136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Householder/
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20603 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Householder/HouseholderSequence.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.946136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7253 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9184 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15062 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15234 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.946136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Jacobi/
+-rw-r--r--   0 runner    (1001) docker     (127)    15957 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Jacobi/Jacobi.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.950136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/Determinant.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32803 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15064 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21478 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.950136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/arch/Inverse_SSE.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.950136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/MetisSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/MetisSupport/MetisSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.950136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/OrderingMethods/
+-rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 runner    (1001) docker     (127)    62266 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/OrderingMethods/Ordering.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.950136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    22248 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.950136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/PardisoSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    20032 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.950136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/
+-rw-r--r--   0 runner    (1001) docker     (127)    24881 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20805 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25478 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14022 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.950136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SPQRSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.954136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/
+-rw-r--r--   0 runner    (1001) docker     (127)    48778 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32949 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12650 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15957 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/UpperBidiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.954136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCholesky/
+-rw-r--r--   0 runner    (1001) docker     (127)    24010 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.958135 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/
+-rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25592 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25840 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12487 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    52349 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17923 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25715 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14831 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/TriangularSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.962136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/
+-rw-r--r--   0 runner    (1001) docker     (127)    27923 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.962136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseQR/
+-rw-r--r--   0 runner    (1001) docker     (127)    28373 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseQR/SparseQR.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.962136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/StlSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/StlSupport/details.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.966136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    34341 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.966136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.966136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/Image.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/Kernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30560 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/blas.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/lapack.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)  1058368 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/lapacke_mangling.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.970136 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)    13132 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16929 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)    37403 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-25 16:03:09.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12587 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/geometry.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/geometry.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12848 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/libroom.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/microphone.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/rir_builder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/rir_builder.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    36566 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/room.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/room.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/threadpool.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10388 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/wall.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/wall.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/multirate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17408 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.970136 pyroomacoustics-0.7.4/pyroomacoustics/phase/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/phase/gl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/recognition.py
+-rw-r--r--   0 runner    (1001) docker     (127)   117575 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/room.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11373 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/soundsource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.974135 pyroomacoustics-0.7.4/pyroomacoustics/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_air_absorption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_anechoic_room.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_angle_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_autocorr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_bandpass_filterbank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_build_rir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_create_noisy_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_issue_115.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_issue_162.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_issue_22.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_issue_235.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_issue_236.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_issue_69.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_issue_87.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_materials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_rake_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_random_ism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_room_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_room_is_insided.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_room_mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_room_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_rt60.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_shoebox_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_soundsource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_source_directivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_source_directivity_flipping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_visibility_shoebox2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_visibility_shoebox3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_visibility_uroom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/test_volume_area.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.978135 pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/test_ccw3p.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/test_geometry_routines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/test_is_inside_2d_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/test_ray_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/test_room_construct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15823 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/test_room_walls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/test_shoebox_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/test_wall_construct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/test_wall_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/test_wall_side_reflect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.978135 pyroomacoustics-0.7.4/pyroomacoustics/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/transform/dft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28975 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/transform/stft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.978135 pyroomacoustics-0.7.4/pyroomacoustics/transform/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/transform/tests/test_dft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/transform/tests/test_dft_timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31814 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/transform/tests/test_stft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/transform/tests/test_stft_oneshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/transform/tests/test_stft_timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21842 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/pyroomacoustics/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:07:16.978135 pyroomacoustics-0.7.4/pyroomacoustics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-04-25 16:07:16.000000 pyroomacoustics-0.7.4/pyroomacoustics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    28095 2024-04-25 16:07:16.000000 pyroomacoustics-0.7.4/pyroomacoustics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:07:16.000000 pyroomacoustics-0.7.4/pyroomacoustics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:03:52.000000 pyroomacoustics-0.7.4/pyroomacoustics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-25 16:07:16.000000 pyroomacoustics-0.7.4/pyroomacoustics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-25 16:07:16.000000 pyroomacoustics-0.7.4/pyroomacoustics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:07:16.978135 pyroomacoustics-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-04-25 16:03:07.000000 pyroomacoustics-0.7.4/setup.py
```

### Comparing `pyroomacoustics-0.7.3/LICENSE` & `pyroomacoustics-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/MANIFEST.in` & `pyroomacoustics-0.7.4/MANIFEST.in`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Acoustic data for the simulation
 include pyroomacoustics/data/materials.json
 
 # The header files for the compiled extension
+include pyroomacoustics/libroom_src/*.h
 include pyroomacoustics/libroom_src/*.hpp
 include pyroomacoustics/libroom_src/*.cpp
 
 # The compiled extension code rely on Eigen, which is included
 include pyroomacoustics/libroom_src/ext/eigen/COPYING.*
 graft pyroomacoustics/libroom_src/ext/eigen/Eigen
```

### Comparing `pyroomacoustics-0.7.3/PKG-INFO` & `pyroomacoustics-0.7.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: pyroomacoustics
-Version: 0.7.3
+Version: 0.7.4
 Summary: A simple framework for room acoustics and audio processing in Python.
 Home-page: https://github.com/LCAV/pyroomacoustics
 Author: Laboratory for Audiovisual Communications, EPFL
 Author-email: fakufaku@gmail.ch
 License: MIT
 Keywords: room acoustics signal processing doa beamforming adaptive
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: Cython
+Requires-Dist: numpy>=1.13.0
+Requires-Dist: scipy>=0.18.0
+Requires-Dist: pybind11>=2.2
 
 .. image:: https://github.com/LCAV/pyroomacoustics/raw/master/logo/pyroomacoustics_logo_horizontal.png
-   :scale: 80 %
    :alt: Pyroomacoustics logo
    :align: left
 
 ------------------------------------------------------------------------------
 
-.. image:: https://travis-ci.org/LCAV/pyroomacoustics.svg?branch=pypi-release
-    :target: https://travis-ci.org/LCAV/pyroomacoustics
 .. image:: https://readthedocs.org/projects/pyroomacoustics/badge/?version=pypi-release
     :target: http://pyroomacoustics.readthedocs.io/en/pypi-release/
     :alt: Documentation Status
 .. image:: https://mybinder.org/badge_logo.svg
     :target: https://mybinder.org/v2/gh/LCAV/pyroomacoustics/master?filepath=notebooks%2Fpyroomacoustics_demo.ipynb
     :alt: Test on mybinder
 .. image:: https://img.shields.io/discord/829534160812245012?color=%237289DA&label=pyroomacoustics%20Discord&logo=discord&logoColor=white
@@ -240,14 +240,19 @@
 
 A couple of `detailed demos with illustrations <https://github.com/LCAV/pyroomacoustics/tree/master/notebooks>`_ are available.  
 
 A comprehensive set of examples covering most of the functionalities
 of the package can be found in the ``examples`` folder of the `GitHub
 repository <https://github.com/LCAV/pyroomacoustics/tree/master/examples>`_.
 
+A `video introduction to pyroomacoustics <https://www.youtube.com/watch?v=c3DTtc--_F4>`_.
+
+A `video tutorial series on using pyroomacoustics <https://youtube.com/playlist?list=PL6QnpHKwdPYgxLV_Ijr6K_3Gdyfhk0SHg&si=gsSuUm9Yw2_sjYhr>`_
+covering many advanced topics.
+
 Authors
 -------
 
 * Robin Scheibler
 * Ivan Dokmanić
 * Sidney Barthe
 * Eric Bezzam
```

### Comparing `pyroomacoustics-0.7.3/README.rst` & `pyroomacoustics-0.7.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 .. image:: https://github.com/LCAV/pyroomacoustics/raw/master/logo/pyroomacoustics_logo_horizontal.png
-   :scale: 80 %
    :alt: Pyroomacoustics logo
    :align: left
 
 ------------------------------------------------------------------------------
 
-.. image:: https://travis-ci.org/LCAV/pyroomacoustics.svg?branch=pypi-release
-    :target: https://travis-ci.org/LCAV/pyroomacoustics
 .. image:: https://readthedocs.org/projects/pyroomacoustics/badge/?version=pypi-release
     :target: http://pyroomacoustics.readthedocs.io/en/pypi-release/
     :alt: Documentation Status
 .. image:: https://mybinder.org/badge_logo.svg
     :target: https://mybinder.org/v2/gh/LCAV/pyroomacoustics/master?filepath=notebooks%2Fpyroomacoustics_demo.ipynb
     :alt: Test on mybinder
 .. image:: https://img.shields.io/discord/829534160812245012?color=%237289DA&label=pyroomacoustics%20Discord&logo=discord&logoColor=white
@@ -214,14 +211,19 @@
 
 A couple of `detailed demos with illustrations <https://github.com/LCAV/pyroomacoustics/tree/master/notebooks>`_ are available.  
 
 A comprehensive set of examples covering most of the functionalities
 of the package can be found in the ``examples`` folder of the `GitHub
 repository <https://github.com/LCAV/pyroomacoustics/tree/master/examples>`_.
 
+A `video introduction to pyroomacoustics <https://www.youtube.com/watch?v=c3DTtc--_F4>`_.
+
+A `video tutorial series on using pyroomacoustics <https://youtube.com/playlist?list=PL6QnpHKwdPYgxLV_Ijr6K_3Gdyfhk0SHg&si=gsSuUm9Yw2_sjYhr>`_
+covering many advanced topics.
+
 Authors
 -------
 
 * Robin Scheibler
 * Ivan Dokmanić
 * Sidney Barthe
 * Eric Bezzam
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/__init__.py` & `pyroomacoustics-0.7.4/pyroomacoustics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/acoustics.py` & `pyroomacoustics-0.7.4/pyroomacoustics/acoustics.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,14 @@
         if output=='sos'.
     """
 
     filters = []
     nyquist = fs / 2.0
 
     for band in bands:
-
         # remove bands above nyquist frequency
         if band[0] >= nyquist:
             raise ValueError("Bands should be below Nyquist frequency")
 
         # Truncate the highest band to Nyquist frequency
         norm_band = np.minimum(0.99, np.array(band) / nyquist)
 
@@ -157,15 +156,14 @@
     fs: float, optional
         The sampling frequency used (default: 16000 Hz)
     third_octave: bool, optional
         Use third octave bands if True (default: False)
     """
 
     def __init__(self, base_frequency=125.0, fs=16000, n_fft=512):
-
         self.base_freq = base_frequency
         self.fs = fs
         self.n_fft = n_fft
 
         # compute the number of bands
         self.n_bands = math.floor(np.log2(fs / base_frequency))
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/adaptive/__init__.py` & `pyroomacoustics-0.7.4/pyroomacoustics/adaptive/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -99,19 +99,19 @@
 :py:obj:`pyroomacoustics.adaptive.algorithms`
     a dictionary containing all the adaptive filter object subclasses availables indexed by
     keys ``['RLS', 'BlockRLS', 'BlockLMS', 'NLMS', 'SubbandLMS']``
 
 """
 
 from .adaptive_filter import *
+from .data_structures import *
 from .lms import *
 from .rls import *
 from .subband_lms import *
 from .util import *
-from .data_structures import *
 
 # Create this dictionary as a shortcut to different algorithms
 algorithms = {
     "RLS": RLS,
     "BlockRLS": BlockRLS,
     "NLMS": NLMS,
     "BlockLMS": BlockLMS,
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/adaptive/adaptive_filter.py` & `pyroomacoustics-0.7.4/pyroomacoustics/adaptive/adaptive_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import division, print_function
-import scipy.linalg as la
+
 import numpy as np
+import scipy.linalg as la
 
 
 class AdaptiveFilter:
     """
     The dummy base class of an adaptive filter. This class doesn't compute
     anything. It merely stores values in a buffer. It is used as a template
     for all other algorithms.
     """
 
     def __init__(self, length):
-
         # filter length
         self.length = length
 
         self.reset()
 
     def reset(self):
         """
@@ -50,9 +50,8 @@
 
         # update buffers
         self.x[1:] = self.x[0:-1]
         self.x[0] = x_n
         self.d = d_n
 
     def name(self):
-
         return self.__class__.__name__
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/adaptive/data_structures.py` & `pyroomacoustics-0.7.4/pyroomacoustics/adaptive/data_structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     length: int
         buffer length
     dtype: numpy.type
         data type
     """
 
     def __init__(self, length=20, dtype=np.float64):
-
         self.buf = np.zeros(length, dtype=dtype)
         self.len = length
         self.head = self.len
 
     def push(self, val):
         """Add one element at the front of the buffer"""
 
@@ -67,15 +66,14 @@
         # create a view that starts at head
         ptr = self.buf[self.head :]
 
         # returned desired range
         return ptr[r]
 
     def __repr__(self):
-
         if self.head == self.len:
             return "[]"
         else:
             return str(self.buf[self.head :])
 
 
 class Powers:
@@ -99,20 +97,18 @@
         >>> an = Powers(0.5)
         >>> print(an[4])
         0.0625
 
     """
 
     def __init__(self, a, length=20, dtype=np.float64):
-
         self.a = dtype(a)
         self.pwr = self.a ** np.arange(length)
 
     def __getitem__(self, r):
-
         # find maximum power requested
         if isinstance(r, int):
             high = r + 1
         elif isinstance(r, slice):
             high = r.stop
         elif isinstance(r, list):
             high = max(r) + 1
@@ -144,15 +140,14 @@
     p: float, 0 < p < 1
         probability to output a 1
     length: int
         the number of flips to precompute
     """
 
     def __init__(self, p, length=10000):
-
         self.p = p
         self.length = length
         self.buffer = np.random.random(length) < p
         self.dirty_coins = 0
 
     def fresh_flips(self, n):
         """Generates n binary random values now"""
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/adaptive/lms.py` & `pyroomacoustics-0.7.4/pyroomacoustics/adaptive/lms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 Least Mean Squares Family
 =========================
 
 Implementations of adaptive filters from the LMS class. These algorithms have a
 low complexity and reliable behavior with a somewhat slower convergence.
 """
-from __future__ import division, print_function, absolute_import
+
+from __future__ import absolute_import, division, print_function
+
 import numpy as np
 import scipy.linalg as la
 
 from .adaptive_filter import AdaptiveFilter
 
 
 class NLMS(AdaptiveFilter):
@@ -22,15 +24,14 @@
     length: int
         the length of the filter
     mu: float, optional
         the step size (default 0.5)
     """
 
     def __init__(self, length, mu=0.5):
-
         self.mu = mu
         AdaptiveFilter.__init__(self, length)
 
     def update(self, x_n, d_n):
         """
         Updates the adaptive filter with a new sample
 
@@ -61,15 +62,14 @@
     L: int, optional
         block size (default is 1)
     nlms: bool, optional
         whether or not to normalize as in NLMS (default is False)
     """
 
     def __init__(self, length, mu=0.01, L=1, nlms=False):
-
         self.nlms = nlms
 
         # sketching parameters
         self.L = L  # block size
 
         NLMS.__init__(self, length, mu=mu)
         self.reset()
@@ -99,15 +99,14 @@
         self.n += 1
         slot = self.L - ((self.n - 1) % self.L) - 1
         self.x[slot] = x_n
         self.d[slot] = d_n
 
         # Block update
         if self.n % self.L == 0:
-
             # block-update parameters
             X = la.hankel(self.x[: self.L], r=self.x[self.L - 1 :])
 
             e = self.d - np.dot(X, self.w)
 
             if self.nlms:
                 norm = np.linalg.norm(X, axis=1) ** 2
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/adaptive/rls.py` & `pyroomacoustics-0.7.4/pyroomacoustics/adaptive/rls.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 Recursive Least Squares Family
 ==============================
 
 Implementations of adaptive filters from the RLS class. These algorithms
 typically have a higher computational complexity, but a faster convergence.
 """
 
-from __future__ import division, print_function, absolute_import
+from __future__ import absolute_import, division, print_function
+
 import numpy as np
-from .data_structures import Buffer, Powers
+
 from .adaptive_filter import AdaptiveFilter
+from .data_structures import Buffer, Powers
 from .util import hankel_stride_trick
 
+
 # First the classic RLS (for real numbered signals)
 class RLS(AdaptiveFilter):
     """
     Implementation of the exponentially weighted Recursive Least Squares (RLS)
     adaptive filter algorithm.
 
     Parameters
@@ -28,15 +31,14 @@
         the regularization term (default 10)
     dtype: numpy type
         the bit depth of the numpy arrays to use (default np.float32)
 
     """
 
     def __init__(self, length, lmbd=0.999, delta=10, dtype=np.float32):
-
         self.lmbd = lmbd
         self.lmbd_inv = 1 / lmbd
         self.delta = delta
         self.x_buf_size = 10 * length
 
         self.dtype = dtype
 
@@ -125,15 +127,14 @@
     dtype: numpy type
         the bit depth of the numpy arrays to use (default np.float32)
     L: int, optional
         the block size (default to length)
     """
 
     def __init__(self, length, lmbd=0.999, delta=10, dtype=np.float32, L=None):
-
         # block size
         if L is None:
             self.block = length
         else:
             self.block = int(L)
 
         RLS.__init__(self, length, lmbd=lmbd, delta=delta, dtype=dtype)
@@ -174,15 +175,14 @@
 
         # Push new data in buffers
         self.x.push(x_n)
         self.d.push(d_n)
 
         # Block update
         if self.n % self.block == 0:
-
             x_vec = self.x.top(self.block + self.length - 1)
             d_vec = self.d.top(self.block)
 
             # The Hankel data matrix
             X = hankel_stride_trick(x_vec, (self.block, self.length))
 
             # Compute the error term
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/adaptive/subband_lms.py` & `pyroomacoustics-0.7.4/pyroomacoustics/adaptive/subband_lms.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 # You should have received a copy of the MIT License along with this program. If
 # not, see <https://opensource.org/licenses/MIT>.
 
 import numpy as np
 
 
 class SubbandLMS:
-
     """
     Frequency domain implementation of LMS. Adaptive filter for each
     subband.
 
     Parameters
     ----------
     num_taps: int
@@ -40,24 +39,22 @@
     mu: float, optional
         step size for each subband (default 0.5)
     nlms: bool, optional
         whether or not to normalize as in NLMS (default is True)
     """
 
     def __init__(self, num_taps, num_bands, mu=0.5, nlms=True):
-
         self.num_taps = num_taps
         self.num_bands = num_bands
         self.mu = mu
         self.nlms = nlms
 
         self.reset()
 
     def reset(self):
-
         # filter bank
         self.W = np.zeros((self.num_taps, self.num_bands), dtype=np.complex64)
 
         # input signal
         self.X = np.zeros((self.num_taps, self.num_bands), dtype=np.complex64)
 
         # reference signal
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/adaptive/tests/test_adaptive.py` & `pyroomacoustics-0.7.4/pyroomacoustics/adaptive/tests/test_adaptive.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import division, print_function
 
 from unittest import TestCase
+
 import numpy as np
 from scipy.signal import fftconvolve
+
 import pyroomacoustics as pra
 
 # fix RNG for a deterministic result
 np.random.seed(0)
 
 # parameters
 length = 15  # the unknown filter length
@@ -19,14 +21,15 @@
 
 # create a known driving signal
 x = np.random.randn(n_samples)
 
 # convolve with the unknown filter
 d_clean = fftconvolve(x, w)[:n_samples]
 
+
 # a function to the adaptive filter on all the samples
 def run_filter(algorithm, x, d):
     for i in range(x.shape[0]):
         algorithm.update(x[i], d[i])
 
 
 class TestAdaptiveFilter(TestCase):
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/adaptive/tests/test_adaptive_frequency.py` & `pyroomacoustics-0.7.4/pyroomacoustics/adaptive/tests/test_adaptive_frequency.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import division, print_function
 
 from unittest import TestCase
+
 import numpy as np
 from scipy.signal import fftconvolve
+
 import pyroomacoustics as pra
 
 # fix RNG for a deterministic result
 np.random.seed(0)
 
 # parameters
 num_taps = 6  # the unknown filter length
@@ -27,40 +29,35 @@
 hop = fft_length // 2
 stft_in = pra.transform.STFT(fft_length, hop=hop, analysis_window=window)
 
 n = 0
 num_blocks = 0
 X_concat = np.zeros((num_bands, n_samples // hop), dtype=np.complex64)
 while n_samples - n > hop:
-
-    stft_in.analysis(
-        x[
-            n : n + hop,
-        ]
-    )
+    stft_in.analysis(x[n : n + hop,])
     X_concat[:, num_blocks] = stft_in.X
 
     n += hop
     num_blocks += 1
 
 # convolve in frequency domain with unknown filter
 Y_concat = np.zeros((num_bands, num_blocks), dtype=np.complex64)
 for k in range(num_bands):
     Y_concat[k, :] = fftconvolve(X_concat[k, :], W[:, k])[:num_blocks]
 
+
 # run filters on each block
 def run_filters(algorithm, X_concat, Y_concat):
     num_blocks = X_concat.shape[1]
     for n in range(num_blocks):
         algorithm.update(X_concat[:, n], Y_concat[:, n])
 
 
 class TestAdaptiveFilterFrequencyDomain(TestCase):
     def test_subband_nlms(self):
-
         subband_nlms = pra.adaptive.SubbandLMS(
             num_taps=num_taps, num_bands=num_bands, mu=0.5, nlms=True
         )
         run_filters(subband_nlms, X_concat, Y_concat)
         error_per_band = np.linalg.norm(subband_nlms.W.conj() - W, axis=0)
         error = np.max(abs(error_per_band))
         print("Subband NLMS Reconstruction Error", error)
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/adaptive/util.py` & `pyroomacoustics-0.7.4/pyroomacoustics/adaptive/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,17 +47,15 @@
         raise ValueError("A dimensions not compatible with toeplitz(c,r)")
 
     x = np.concatenate((c, np.zeros(zp, dtype=c.dtype), r[-1:0:-1]))
     xf = np.fft.rfft(x, n=fft_len)
 
     Af = np.fft.rfft(A, n=fft_len, axis=0)
 
-    return np.fft.irfft((Af.T * xf).T, n=fft_len, axis=0)[
-        :m,
-    ]
+    return np.fft.irfft((Af.T * xf).T, n=fft_len, axis=0)[:m,]
 
 
 def hankel_multiplication(c, r, A, mkl=True, **kwargs):
     """
     Compute numpy.dot(scipy.linalg.hankel(c,r=r), A) using the FFT.
 
     Parameters
@@ -74,17 +72,15 @@
 
     if mkl and has_mklfft:
         fmul = mkl_toeplitz_multiplication
     else:
         fmul = toeplitz_multiplication
         A = A[: r.shape[0], :]
 
-    return fmul(c[::-1], r, A, **kwargs)[
-        ::-1,
-    ]
+    return fmul(c[::-1], r, A, **kwargs)[::-1,]
 
 
 def mkl_toeplitz_multiplication(c, r, A, A_padded=False, out=None, fft_len=None):
     """
     Compute numpy.dot(scipy.linalg.toeplitz(c,r), A) using the FFT from the mkl_fft package.
 
     Parameters
@@ -130,17 +126,15 @@
     out *= xf[:, None]
 
     if A_padded:
         fft.irfft(out, n=fft_len, axis=0, out=A)
     else:
         A = fft.irfft(out, n=fft_len, axis=0)
 
-    return A[
-        :m,
-    ]
+    return A[:m,]
 
 
 def naive_toeplitz_multiplication(c, r, A):
     """
     Compute numpy.dot(scipy.linalg.toeplitz(c,r), A)
 
     Parameters
@@ -228,15 +222,14 @@
     if matrix:
         return la.circulant(c)
     else:
         return c
 
 
 if __name__ == "__main__":
-
     import time
 
     try:
         import mkl as mkl_service
 
         mkl_service.set_num_threads(7)
     except ImportError:
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/beamforming.py` & `pyroomacoustics-0.7.4/pyroomacoustics/beamforming.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,14 @@
     pos_mic_x = pos_array_norm * np.cos(pos_array_angle)
     pos_mic_y = pos_array_norm * np.sin(pos_array_angle)
 
     return np.array([pos_mic_x, pos_mic_y])
 
 
 def fir_approximation_ls(weights, T, n1, n2):
-
     freqs_plus = np.array(weights.keys())[:, np.newaxis]
     freqs = np.vstack([freqs_plus, -freqs_plus])
     omega = 2 * np.pi * freqs
     omega_discrete = omega * T
 
     n = np.arange(n1, n2)
 
@@ -321,15 +320,14 @@
         azimuth_plot = np.linspace(start=0, stop=360, num=361, endpoint=True)
         if colatitude is not None:
             colatitude_plot = np.linspace(start=0, stop=180, num=180, endpoint=True)
 
     azimuth_list = np.arange(M) * 360 / M + phi0
     directivity_list = []
     for i in range(M):
-
         orientation = DirectionVector(
             azimuth=azimuth_list[i], colatitude=colatitude, degrees=True
         )
         directivity.set_orientation(orientation)
         directivity_list.append(copy.copy(directivity))
 
         if ax is not None:
@@ -346,19 +344,17 @@
 
 # =========================================================================
 # Classes (microphone array and beamformer related)
 # =========================================================================
 
 
 class MicrophoneArray(object):
-
     """Microphone array class."""
 
     def __init__(self, R, fs, directivity=None):
-
         R = np.array(R)
         self.dim = R.shape[0]  # are we in 2D or in 3D
         self.nmic = R.shape[1]  # number of microphones
 
         # Check the shape of the passed array
         if self.dim != 2 and self.dim != 3:
             dim_mismatch = True
@@ -382,15 +378,14 @@
             self.set_directivity(directivity)
 
         self.signals = None
 
         self.center = np.mean(R, axis=1, keepdims=True)
 
     def set_directivity(self, directivities):
-
         """
         This functions sets self.directivity as a list of directivities with `n_mics` entries,
         where `n_mics` is the number of microphones
         Parameters
         -----------
         directivities:
             single directivity for all microphones or a list of directivities for each microphone
@@ -612,23 +607,21 @@
 
         if self.weights is None:
             raise NameError("Weights must be defined.")
 
         self.filters = np.zeros((self.M, self.Lg))
 
         if self.N <= self.Lg:
-
             # go back to time domain and shift DC to center
             tw = np.fft.irfft(np.conj(self.weights), axis=1, n=self.N)
             self.filters[:, : self.N] = np.concatenate(
                 (tw[:, -self.N // 2 :], tw[:, : self.N // 2]), axis=1
             )
 
         elif self.N > self.Lg:
-
             # Least-square projection
             for i in np.arange(self.M):
                 Lgp = np.floor((1 - non_causal) * self.Lg)
                 Lgm = self.Lg - Lgp
                 # the beamforming weights in frequency are the complex
                 # conjugates of the FT of the filter
                 w = np.concatenate((np.conj(self.weights[i]), self.weights[i, -2:0:-1]))
@@ -637,28 +630,26 @@
                 k = np.arange(self.N)[:, np.newaxis]
                 l = np.concatenate((np.arange(self.N - Lgm, self.N), np.arange(Lgp)))
                 F = np.exp(-2j * np.pi * k * l / self.N)
 
                 self.filters[i] = np.real(np.linalg.lstsq(F, w, rcond=None)[0])
 
     def weights_from_filters(self):
-
         if self.filters is None:
             raise NameError("Filters must be defined.")
 
         # this is what we want to use, really.
         # self.weights = np.conj(np.fft.rfft(self.filters, n=self.N, axis=1))
 
         # quick hack to be able to use MKL acceleration package from anaconda
         self.weights = np.zeros((self.M, self.N // 2 + 1), dtype=np.complex128)
         for m in range(self.M):
             self.weights[m] = np.conj(np.fft.rfft(self.filters[m], n=self.N))
 
     def steering_vector_2D(self, frequency, phi, dist, attn=False):
-
         phi = np.array([phi]).reshape(phi.size)
 
         # Assume phi and dist are measured from the array's center
         X = dist * np.array([np.cos(phi), np.sin(phi)]) + self.center
 
         D = distance(self.R, X)
         omega = 2 * np.pi * frequency
@@ -697,29 +688,27 @@
             # The projected microphone distances on the unit vectors
             D = -1 * np.dot(self.R.T, p)
 
             # subtract minimum in each column
             D -= np.min(D)
 
         else:
-
             D = distance(self.R, X)
 
         phase = np.exp(-1j * omega * D / constants.get("c"))
 
         if attn:
             # TO DO 1: This will mean slightly different absolute value for
             # every entry, even within the same steering vector. Perhaps a
             # better paradigm is far-field with phase carrier.
             return 1.0 / (4 * np.pi) / D * phase
         else:
             return phase
 
     def response(self, phi_list, frequency):
-
         i_freq = np.argmin(np.abs(self.frequencies - frequency))
 
         if self.weights is None and self.filters is not None:
             self.weights_from_filters()
         elif self.weights is None and self.filters is None:
             raise NameError(
                 "Beamforming weights or filters need to be computed" " first."
@@ -732,15 +721,14 @@
                 self.frequencies[i_freq], phi_list, constants.get("ffdist")
             ),
         )
 
         return self.frequencies[i_freq], bfresp
 
     def response_from_point(self, x, frequency):
-
         i_freq = np.argmin(np.abs(self.frequencies - frequency))
 
         if self.weights is None and self.filters is not None:
             self.weights_from_filters()
         elif self.weights is None and self.filters is None:
             raise NameError(
                 "Beamforming weights or filters need to be computed" " first."
@@ -753,15 +741,14 @@
                 self.frequencies[i_freq], x, attn=True, ff=False
             ),
         )
 
         return self.frequencies[i_freq], bfresp
 
     def plot_response_from_point(self, x, legend=None):
-
         if self.weights is None and self.filters is not None:
             self.weights_from_filters()
         elif self.weights is None and self.filters is None:
             raise NameError(
                 "Beamforming weights or filters need to be computed" " first."
             )
 
@@ -798,15 +785,14 @@
             plt.plot(self.frequencies, np.unwrap(np.angle(hf)))
         plt.ylabel("Phase")
         plt.xlabel("Frequency [Hz]")
         plt.axis("tight")
         plt.legend(legend)
 
     def plot_beam_response(self):
-
         if self.weights is None and self.filters is not None:
             self.weights_from_filters()
         elif self.weights is None and self.filters is None:
             raise NameError("Beamforming weights or filters need to be computed first.")
 
         phi = np.linspace(-np.pi, np.pi - np.pi / 180, 360)
         freq = self.frequencies
@@ -859,15 +845,14 @@
         for i in np.arange(1, 5):
             yticks[i - 1] = np.argmin(np.abs(freq - 1000.0 * i * f_0))
         # yticks = np.array(plt.getp(plt.gca(), 'yticks'), dtype=np.int)
         plt.setp(plt.gca(), "yticks", yticks)
         plt.setp(plt.gca(), "yticklabels", np.arange(1, 5) * f_0)
 
     def snr(self, source, interferer, f, R_n=None, dB=False):
-
         i_f = np.argmin(np.abs(self.frequencies - f))
 
         if self.weights is None and self.filters is not None:
             self.weights_from_filters()
         elif self.weights is None and self.filters is None:
             raise NameError(
                 "Beamforming weights or filters need to be computed" " first."
@@ -901,15 +886,14 @@
 
         if dB is True:
             SNR = 10 * np.log10(SNR)
 
         return SNR
 
     def udr(self, source, interferer, f, R_n=None, dB=False):
-
         i_f = np.argmin(np.abs(self.frequencies - f))
 
         if self.weights is None and self.filters is not None:
             self.weights_from_filters()
         elif self.weights is None and self.filters is None:
             raise NameError(
                 "Beamforming weights or filters need to be computed" " first."
@@ -935,20 +919,18 @@
         UDR = np.real(mdot(H(w), A_good, H(A_good), w) / mdot(H(w), R_nq, w))
         if dB is True:
             UDR = 10 * np.log10(UDR)
 
         return UDR
 
     def process(self, FD=False):
-
         if self.signals is None or len(self.signals) == 0:
             raise NameError("No signal to beamform.")
 
         if FD is True:
-
             # STFT processing
             if self.weights is None and self.filters is not None:
                 self.weights_from_filters()
             elif self.weights is None and self.filters is None:
                 raise NameError(
                     "Beamforming weights or filters need to be " "computed first."
                 )
@@ -977,15 +959,14 @@
             # remove the zero padding from output signal
             if self.zpb == 0:
                 output = output[self.zpf :]
             else:
                 output = output[self.zpf : -self.zpb]
 
         else:
-
             # TD processing
 
             if self.weights is not None and self.filters is None:
                 self.filters_from_weights()
             elif self.weights is None and self.filters is None:
                 raise NameError(
                     "Beamforming weights or filters need to be " "computed first."
@@ -997,15 +978,14 @@
             output = fftconvolve(self.filters[0], self.signals[0])
             for i in range(1, len(self.signals)):
                 output += fftconvolve(self.filters[i], self.signals[i])
 
         return output
 
     def plot(self, sum_ir=False, FD=True):
-
         if self.weights is None and self.filters is not None:
             self.weights_from_filters()
         elif self.weights is not None and self.filters is None:
             self.filters_from_weights()
         elif self.weights is None and self.filters is None:
             raise NameError(
                 "Beamforming weights or filters need to be " "computed first."
@@ -1057,27 +1037,25 @@
         self.weights = np.exp(
             2j * np.pi * self.frequencies[:, np.newaxis] * proj / constants.get("c")
         ).T
 
     def rake_delay_and_sum_weights(
         self, source, interferer=None, R_n=None, attn=True, ff=False
     ):
-
         self.weights = np.zeros((self.M, self.frequencies.shape[0]), dtype=complex)
 
         K = source.images.shape[1] - 1
 
         for i, f in enumerate(self.frequencies):
             W = self.steering_vector_2D_from_point(f, source.images, attn=attn, ff=ff)
             self.weights[:, i] = 1.0 / self.M / (K + 1) * np.sum(W, axis=1)
 
     def rake_one_forcing_weights(
         self, source, interferer=None, R_n=None, ff=False, attn=True
     ):
-
         if R_n is None:
             R_n = np.zeros((self.M, self.M))
 
         self.weights = np.zeros((self.M, self.frequencies.shape[0]), dtype=complex)
 
         for i, f in enumerate(self.frequencies):
             if interferer is None:
@@ -1112,15 +1090,14 @@
 
         if R_n is None:
             R_n = np.zeros((self.M, self.M))
 
         self.weights = np.zeros((self.M, self.frequencies.shape[0]), dtype=complex)
 
         for i, f in enumerate(self.frequencies):
-
             A_good = self.steering_vector_2D_from_point(
                 f, source.images, attn=attn, ff=ff
             )
 
             if interferer is None:
                 A_bad = np.array([[]])
             else:
@@ -1139,15 +1116,14 @@
             self.weights[:, i] = (K_inv.dot(a_good) / mdot(H(a_good), K_inv, a_good))[
                 :, 0
             ]
 
     def rake_max_udr_weights(
         self, source, interferer=None, R_n=None, ff=False, attn=True
     ):
-
         if source.images.shape[1] == 1:
             self.rake_max_sinr_weights(
                 source.images, interferer.images, R_n=R_n, ff=ff, attn=attn
             )
             return
 
         if R_n is None:
@@ -1464,15 +1440,14 @@
         off = (Lg - Lh) / 2
         L = self.Lg + Lh - 1
 
         H = np.zeros((Lg * self.M, 2 * L))
         As = np.zeros((Lg * self.M, K))
 
         for r in np.arange(self.M):
-
             # build constraint matrix
             hs = u.low_pass_dirac(
                 s_time[r, :, np.newaxis], s_dmp[r, :, np.newaxis], self.fs, Lh
             )[:, ::-1]
             As[r * Lg + off : r * Lg + Lh + off, :] = hs.T
 
             # build interferer RIR matrix
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/bss/__init__.py` & `pyroomacoustics-0.7.4/pyroomacoustics/bss/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,14 @@
 
 .. [6] K. Sekiguchi, Y. Bando, A. A. Nugraha, K. Yoshii, T. Kawahara, *Fast Multichannel
     Nonnegative Matrix Factorization with Directivity-Aware Jointly-Diagonalizable Spatial
     Covariance Matrices for Blind Source Separation*, IEEE/ACM Trans. ASLP, vol. 28, pp. 2610-2625, 2020.
 
 """
 
-from .trinicon import trinicon
 from .auxiva import auxiva
-from .ilrma import ilrma
-from .sparseauxiva import sparseauxiva
+from .common import projection_back, sparir
 from .fastmnmf import fastmnmf
 from .fastmnmf2 import fastmnmf2
-from .common import projection_back, sparir
+from .ilrma import ilrma
+from .sparseauxiva import sparseauxiva
+from .trinicon import trinicon
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/bss/auxiva.py` & `pyroomacoustics-0.7.4/pyroomacoustics/bss/auxiva.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,14 @@
     proj_back=True,
     W0=None,
     model="laplace",
     init_eig=False,
     return_filters=False,
     callback=None,
 ):
-
     """
     This is an implementation of AuxIVA/OverIVA that separates the input
     signal into statistically independent sources. The separation is done
     in the time-frequency domain and the FFT length should be approximately
     equal to the reverberation time.
 
     Two different statistical models (Laplace or time-varying Gauss) can
@@ -155,15 +154,14 @@
 
     def update_J_from_orth_const():
         tmp = np.matmul(W, Cx)
         J[:, :, :] = tensor_H(np.linalg.solve(tmp[:, :, :n_src], tmp[:, :, n_src:]))
 
     # initialize A and W
     if W0 is None:
-
         if init_eig:
             # Initialize the demixing matrices with the principal
             # eigenvectors of the input covariance
             v, w = np.linalg.eig(Cx)
             for f in range(n_freq):
                 ind = np.argsort(v[f])[-n_src:]
                 W[f, :, :] = np.conj(w[f][:, ind])
@@ -194,15 +192,14 @@
     X = X.transpose([1, 2, 0]).copy()
 
     # Compute the demixed output
     def demix(Y, X, W):
         Y[:, :, :] = np.matmul(W, X)
 
     for epoch in range(n_iter):
-
         demix(Y, X, W)
 
         if callback is not None and epoch % 10 == 0:
             Y_tmp = Y.transpose([2, 0, 1])
             if proj_back:
                 z = projection_back(Y_tmp, X_original[:, :, 0])
                 callback(Y_tmp * np.conj(z[None, :, :]))
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/bss/common.py` & `pyroomacoustics-0.7.4/pyroomacoustics/bss/common.py`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/bss/fastmnmf.py` & `pyroomacoustics-0.7.4/pyroomacoustics/bss/fastmnmf.py`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/bss/fastmnmf2.py` & `pyroomacoustics-0.7.4/pyroomacoustics/bss/fastmnmf2.py`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/bss/ilrma.py` & `pyroomacoustics-0.7.4/pyroomacoustics/bss/ilrma.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 """
 ILRMA
 =====
 
 Blind Source Separation using Independent Low-Rank Matrix Analysis (ILRMA).
 """
 import numpy as np
+
 from .common import projection_back
 
 
 def ilrma(
     X,
     n_src=None,
     n_iter=20,
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/bss/sparseauxiva.py` & `pyroomacoustics-0.7.4/pyroomacoustics/bss/sparseauxiva.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # You should have received a copy of the MIT License along with this program. If
 # not, see <https://opensource.org/licenses/MIT>.
 
 import numpy as np
+
 from .common import projection_back, sparir
 
 
 def sparseauxiva(
     X,
     S=None,
     n_src=None,
     n_iter=20,
     proj_back=True,
     W0=None,
     model="laplace",
     return_filters=False,
     callback=None,
 ):
-
     """
     Implementation of sparse AuxIVA algorithm for BSS presented in
 
     J. Janský, Z. Koldovský, and N. Ono, *A computationally cheaper method
     for blind speech separation based on AuxIVA and incomplete demixing transform,*
     Proc. IEEE, IWAENC, pp. 1-5, Sept. 2016.
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/bss/tests/test_bss.py` & `pyroomacoustics-0.7.4/pyroomacoustics/bss/tests/test_bss.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import unittest
+
 import numpy as np
-import pyroomacoustics as pra
 from scipy.io import wavfile
-import unittest
+
+import pyroomacoustics as pra
 
 np.random.seed(0)
 
 # We use several sound samples for each source to have a long enough length
 wav_files = [
     [
         "examples/input_samples/cmu_arctic_us_axb_a0004.wav",
@@ -18,17 +20,17 @@
         "examples/input_samples/cmu_arctic_us_aew_a0003.wav",
     ],
 ]
 
 # List of frame lengths to test
 L = [256, 512, 1024, 2048, 4096]
 
+
 # Frequency Blind Source Separation
 def freq_bss(algo="auxiva", L=256, **kwargs):
-
     # Room dimensions in meters
     room_dim = [8, 9]
 
     # create a room with sources and mics
     room = pra.ShoeBox(room_dim, fs=16000, max_order=0, sigma2_awgn=1e-8)
 
     # get signals
@@ -54,15 +56,14 @@
 
     # compute RIRs
     room.compute_rir()
 
     # Record each source separately
     separate_recordings = []
     for source, signal in zip(room.sources, signals):
-
         source.signal[:] = signal
 
         room.simulate()
         separate_recordings.append(room.mic_array.signals)
 
         source.signal[:] = 0.0
     separate_recordings = np.array(separate_recordings)
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/bss/tests/test_trinicon.py` & `pyroomacoustics-0.7.4/pyroomacoustics/bss/tests/test_trinicon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
-import pyroomacoustics as pra
 from scipy.io import wavfile
 
+import pyroomacoustics as pra
+
 # We use several sound samples for each source to have a long enough length
 wav_files = [
     [
         "examples/input_samples/cmu_arctic_us_axb_a0004.wav",
         "examples/input_samples/cmu_arctic_us_axb_a0005.wav",
         "examples/input_samples/cmu_arctic_us_axb_a0006.wav",
     ],
@@ -55,15 +56,14 @@
 
     # compute RIRs
     room.compute_rir()
 
     # Record each source separately
     separate_recordings = []
     for source, signal in zip(room.sources, signals):
-
         source.signal[:] = signal
 
         room.simulate()
         separate_recordings.append(room.mic_array.signals)
 
         source.signal[:] = 0.0
     separate_recordings = np.array(separate_recordings)
@@ -108,15 +108,14 @@
 
     # compute RIRs
     room.compute_rir()
 
     # Record each source separately
     separate_recordings = []
     for source, signal in zip(room.sources, signals):
-
         source.signal[:] = signal
 
         room.simulate()
         separate_recordings.append(room.mic_array.signals)
 
         source.signal[:] = 0.0
     separate_recordings = np.array(separate_recordings)
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/bss/trinicon.py` & `pyroomacoustics-0.7.4/pyroomacoustics/bss/trinicon.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,14 @@
     S = signals.shape[1]  # total signal length
     M = S / hop  # number of online blocks
 
     y = np.zeros((Q, S))  # the processed output signal
 
     m = 1  # online block index
     while m <= M:  # online loop
-
         # new chunk of input signal
         x = np.zeros((P, K * L + N))
         if m * hop > S:
             # we need some zero padding at the back
             le = S - (m - 1) * hop + N
             x[:le] = signals[:, m * hop - K * L - N :]
         if m * hop >= K * L + N:
@@ -114,15 +113,14 @@
             # we need some zero padding at the beginning
             x[:, -m * hop :] = signals[:, : m * hop]
 
         # use filter from previous iteration to initialize offline part
         w_new = w.copy()
 
         for j in range(j_max):  # offline update loop
-
             y_c = np.zeros((Q, K * L + N - L))  # c stands for chunk
             y_blocks = np.zeros((Q, K, N))
 
             for q in range(Q):
                 # convolve with filters
                 for p in range(P):
                     # We discard the 'oldest' output of the convolution according
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/build_rir.pyx` & `pyroomacoustics-0.7.4/pyroomacoustics/build_rir.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # cython: infer_types=True
 
 import numpy as np
+
 cimport cython
+from libc.math cimport ceil, floor
 
-from libc.math cimport floor, ceil
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 def fast_rir_builder(
         double [:] rir,
         double [:] time,
         double [:] alpha,
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/data/materials.json` & `pyroomacoustics-0.7.4/pyroomacoustics/data/materials.json`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/datasets/__init__.py` & `pyroomacoustics-0.7.4/pyroomacoustics/datasets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,11 +133,11 @@
     # show the spectrogram
     plt.figure()
     matches[0].plot()
     plt.show()
   
 """
 
-from .base import Meta, Sample, AudioSample, Dataset
-from .timit import Word, Sentence, TimitCorpus
+from .base import AudioSample, Dataset, Meta, Sample
 from .cmu_arctic import CMUArcticCorpus, CMUArcticSentence, cmu_arctic_speakers
-from .google_speech_commands import GoogleSpeechCommands, GoogleSample
+from .google_speech_commands import GoogleSample, GoogleSpeechCommands
+from .timit import Sentence, TimitCorpus, Word
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/datasets/base.py` & `pyroomacoustics-0.7.4/pyroomacoustics/datasets/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,14 @@
         for sample in self.samples[:n]:
             print(sample)
 
     def __str__(self):
         r = "The dataset contains {} samples.\n".format(len(self))
         r += "Metadata attributes are:\n"
         for field, values in self.info.items():
-
             r += "  {} ({}) :\n".format(field, len(values))
 
             # for attributes with lots of values, we just print a few
             if len(values) > 6:
                 short_list = _take(6, values.items())
                 for value, number in short_list[:3]:
                     r += "      * {} occurs {} times\n".format(value, number)
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/datasets/cmu_arctic.py` & `pyroomacoustics-0.7.4/pyroomacoustics/datasets/cmu_arctic.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 License: Permissive, attribution required
 
 Price: Free
 
 URL: http://www.festvox.org/cmu_arctic/
 """
+
 import os
 
 import numpy as np
 from scipy.io import wavfile
 
 try:
     import sounddevice as sd
@@ -107,15 +108,14 @@
     lang: str or list of str, optional
         The language, only 'English' is available here
     accent: str of list of str, optional
         The accent of the speaker
     """
 
     def __init__(self, basedir=None, download=False, build=True, **kwargs):
-
         # initialize
         Dataset.__init__(self)
 
         # we give a meaningful alias to the sample list from the base class
         self.sentences = self.samples
 
         # default base directory is the current one
@@ -199,18 +199,16 @@
     def build_corpus(self, **kwargs):
         """
         Build the corpus with some filters (sex, lang, accent, sentence_tag, sentence)
         """
 
         # Check all the sentences
         for tag, info in cmu_arctic_sentences.items():
-
             # And all speakers for each sentence
             for speaker, path in info["paths"].items():
-
                 # This is the metadata for this sample
                 meta = Meta(
                     speaker=speaker,
                     tag=tag,
                     text=info["text"],
                     **cmu_arctic_speakers[speaker]
                 )
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/datasets/google_speech_commands.py` & `pyroomacoustics-0.7.4/pyroomacoustics/datasets/google_speech_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,27 +15,29 @@
 https://aiyprojects.withgoogle.com/open_speech_recording
 
 Tutorial on creating a word classifier:
 
 https://www.tensorflow.org/versions/master/tutorials/audio_recognition
 """
 
-import os, glob
+import glob
+import os
+
 import numpy as np
 from scipy.io import wavfile
 
 try:
     import sounddevice as sd
 
     have_sounddevice = True
 except:
     have_sounddevice = False
 
+from .base import AudioSample, Dataset, Meta
 from .utils import download_uncompress
-from .base import Meta, AudioSample, Dataset
 
 url = "http://download.tensorflow.org/data/speech_commands_v0.01.tar.gz"
 
 
 class GoogleSpeechCommands(Dataset):
     """
     This class will load the Google Speech Commands Dataset in a
@@ -65,15 +67,14 @@
     seed: int, optional
         Which seed to use for the random generator when selecting a subset of samples. By default, ``seed=0``.
     """
 
     def __init__(
         self, basedir=None, download=False, build=True, subset=None, seed=0, **kwargs
     ):
-
         # initialize
         Dataset.__init__(self)
         self.size_by_samples = {}
 
         # default base directory is the current one
         self.basedir = basedir
         if basedir is None:
@@ -104,15 +105,14 @@
         """
 
         self.subdirs = glob.glob(os.path.join(self.basedir, "*", "."))
         self.classes = [s.split(os.sep)[-2] for s in self.subdirs]
 
         # go through all subdirectories / soundtypes
         for idx, word in enumerate(self.classes):
-
             if word == "_background_noise_":
                 speech = False
             else:
                 speech = True
 
             # get all list of all files in the subdirectory
             word_path = self.subdirs[idx]
@@ -125,15 +125,14 @@
                 self.rng.shuffle(rand_idx)
                 files = [files[i] for i in rand_idx[:n_files]]
 
             self.size_by_samples[word] = len(files)
 
             # add each file to the corpus
             for filename in files:
-
                 file_loc = os.path.join(self.basedir, word, os.path.basename(filename))
 
                 # could also add score of original model for each word?
                 if speech:
                     meta = Meta(word=word, speech=speech, file_loc=file_loc)
                 else:
                     noise_type = os.path.basename(filename).split(".")[0]
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/datasets/tests/test_corpus_base.py` & `pyroomacoustics-0.7.4/pyroomacoustics/datasets/tests/test_corpus_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Example of the basic operations with ``pyroomacoustics.datasets.Dataset``
 and ``pyroomacoustics.datasets.Sample`` classes
 """
-from pyroomacoustics.datasets import Sample, Dataset
+
+from pyroomacoustics.datasets import Dataset, Sample
 
 
 def test_dataset():
     # Prepare a few artificial samples
     samples = [
         {
             "data": 0.99,
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/datasets/timit.py` & `pyroomacoustics-0.7.4/pyroomacoustics/datasets/timit.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 URL: https://catalog.ldc.upenn.edu/ldc93s1
 """
 
 import os
 
 import numpy as np
+
 from pyroomacoustics.transform import stft
 
 try:
     import sounddevice as sd
 
     have_sounddevice = True
 except:
@@ -125,15 +126,14 @@
         The sampling frequency
     phonems: list, optional
         A list of phones contained in the word
 
     """
 
     def __init__(self, word, boundaries, data, fs, phonems=None):
-
         self.word = word
         self.phonems = phonems
         self.boundaries = boundaries
         self.samples = data[boundaries[0] : boundaries[1]]
         self.fs = fs
         self.features = None
 
@@ -253,22 +253,20 @@
         f_ph.close()
 
         for line in w_lines:
             t = line.split()
 
             # just a sanity check
             if len(t) == 3:
-
                 # the word boundary
                 w_bnd = np.array([int(t[0]), int(t[1])])
 
                 # recover the phonems making up the word
                 w_ph_list = []
                 while ph_l_index < len(ph_lines):
-
                     ph_line = ph_lines[ph_l_index]
                     u = ph_line.split()
 
                     # phonem boundary
                     ph_bnd = np.array([int(u[0]), int(u[1])])
 
                     # Check phonem boundary does not exceeds word boundary
@@ -315,15 +313,14 @@
         """Play the sound sample"""
         if have_sounddevice:
             sd.play(self.data, samplerate=self.fs)
         else:
             print("Warning: sounddevice package is required to play audiofiles.")
 
     def plot(self, L=512, hop=128, zpb=0, phonems=False, **kwargs):
-
         try:
             import matplotlib.pyplot as plt
             import seaborn as sns
         except ImportError:
             return
 
         sns.set_style("white")
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/datasets/utils.py` & `pyroomacoustics-0.7.4/pyroomacoustics/datasets/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # You should have received a copy of the MIT License along with this program. If
 # not, see <https://opensource.org/licenses/MIT>.
 
+import bz2
 import os
 import tarfile
-import bz2
 
 try:
     from urllib.request import urlopen
 except ImportError:
     from urllib import urlopen
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/denoise/__init__.py` & `pyroomacoustics-0.7.4/pyroomacoustics/denoise/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,10 +20,10 @@
     IEEE Transactions on Speech and Audio Processing, vol. 3, no. 4, pp. 251-266, Jul 1995.
 
 .. [3] J. Lim and A. Oppenheim, *All-Pole Modeling of Degraded Speech,*
     IEEE Transactions on Acoustics, Speech, and Signal Processing 26.3 (1978): 197-210.
 
 """
 
+from .iterative_wiener import *
 from .spectral_subtraction import *
 from .subspace import *
-from .iterative_wiener import *
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/denoise/iterative_wiener.py` & `pyroomacoustics-0.7.4/pyroomacoustics/denoise/iterative_wiener.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,14 @@
         Threshold to distinguish between (signal+noise) and (noise) frames. A
         high value will classify more frames as noise but might remove desired
         signal!
 
     """
 
     def __init__(self, frame_len, lpc_order, iterations, alpha=0.8, thresh=0.01):
-
         if frame_len % 2:
             raise ValueError(
                 "Frame length should be even as this method " "relies on 50% overlap."
             )
 
         if (alpha > 1) or (alpha < 0):
             raise ValueError("`alpha` parameter should be within [0,1].")
@@ -215,25 +214,23 @@
             frame_dft = np.fft.rfft(current_frame)
         frame_dft /= np.sqrt(self.frame_len)
 
         frame_energy = np.std(current_frame) ** 2
 
         # simple VAD
         if frame_energy < self.thresh:  # noise frame
-
             # update noise power spectral density
             # assuming white noise, i.e. flat spectrum
             self.noise_psd = (
                 self.alpha * self.noise_psd + (1 - self.alpha) * frame_energy
             )
 
             # update wiener filter
             self.wiener_filt[:] = compute_wiener_filter(self.speech_psd, self.noise_psd)
         else:  # speech frame
-
             s_i = current_frame
 
             # iteratively update speech power spectral density / wiener filter
             for i in range(self.iterations):
                 a = lpc(s_i, self.lpc_order)
                 g2 = compute_squared_gain(a, self.noise_psd, current_frame)
                 self.speech_psd[:] = compute_speech_psd(a, g2, self.frame_len)
@@ -408,25 +405,19 @@
     stft = STFT(frame_len, hop=hop, analysis_window=window, streaming=True)
     scnr = IterativeWiener(frame_len, lpc_order, iterations, alpha, thresh)
 
     processed_audio = np.zeros(noisy_signal.shape)
     n = 0
     while noisy_signal.shape[0] - n >= hop:
         # SCNR in frequency domain
-        stft.analysis(
-            noisy_signal[
-                n : (n + hop),
-            ]
-        )
+        stft.analysis(noisy_signal[n : (n + hop),])
         X = scnr.compute_filtered_output(
             current_frame=stft.fft_in_buffer, frame_dft=stft.X
         )
 
         # back to time domain
-        processed_audio[
-            n : n + hop,
-        ] = stft.synthesis(X)
+        processed_audio[n : n + hop,] = stft.synthesis(X)
 
         # update step
         n += hop
 
     return processed_audio
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/denoise/spectral_subtraction.py` & `pyroomacoustics-0.7.4/pyroomacoustics/denoise/spectral_subtraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,14 @@
     alpha: float, optional
         Exponent factor to modify transition behavior towards the dB reduction
         specified by ``db_reduc``. Default is 1.
 
     """
 
     def __init__(self, nfft, db_reduc, lookback, beta, alpha=1):
-
         self.beta = beta
         self.alpha = alpha
 
         self.n_bins = nfft // 2 + 1
         self.p_prev = np.zeros((self.n_bins, lookback + 1))
         self.gmin = 10 ** (-db_reduc / 20)
 
@@ -206,23 +205,17 @@
     stft = STFT(nfft, hop=hop, analysis_window=window, streaming=True)
     scnr = SpectralSub(nfft, db_reduc, lookback, beta, alpha)
 
     processed_audio = np.zeros(noisy_signal.shape)
     n = 0
     while noisy_signal.shape[0] - n >= hop:
         # SCNR in frequency domain
-        stft.analysis(
-            noisy_signal[
-                n : (n + hop),
-            ]
-        )
+        stft.analysis(noisy_signal[n : (n + hop),])
         gain_filt = scnr.compute_gain_filter(stft.X)
 
         # back to time domain
-        processed_audio[
-            n : n + hop,
-        ] = stft.synthesis(gain_filt * stft.X)
+        processed_audio[n : n + hop,] = stft.synthesis(gain_filt * stft.X)
 
         # update step
         n += hop
 
     return processed_audio
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/denoise/subspace.py` & `pyroomacoustics-0.7.4/pyroomacoustics/denoise/subspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,14 @@
         frame_len=256,
         mu=10,
         lookback=10,
         skip=2,
         thresh=0.01,
         data_type="float32",
     ):
-
         if frame_len % 2:
             raise ValueError(
                 "Frame length should be even as this method " "performs 50% overlap."
             )
 
         if data_type == "float64":
             data_type = np.float64
@@ -195,15 +194,14 @@
         self.prev_samples[:] = new_samples
         self.current_out[:] = self.prev_output + denoised_out[: self.hop]
         self.prev_output[:] = denoised_out[self.hop :]
 
         return self.current_out
 
     def compute_signal_projection(self):
-
         sigma = np.linalg.lstsq(self.cov_n, self.cov_sn, rcond=None)[0] - np.eye(
             self.frame_len
         )
         eigenvals, eigenvecs = np.linalg.eig(sigma)
 
         n_pos = sum(eigenvals > 0)
         order = np.argsort(eigenvals, axis=-1)[::-1]
@@ -213,15 +211,14 @@
             q1[w, w] = pos_eigenvals[w] / (pos_eigenvals[w] + self.mu)
 
         v_t = np.transpose(-eigenvecs[:, order])
         self.h_opt[:] = np.real(np.linalg.multi_dot([np.linalg.pinv(v_t), q1, v_t]))
         # self.h_opt = np.dot(np.linalg.lstsq(v_t, q1, rcond=None)[0], v_t)
 
     def update_cov_matrices(self, new_samples):
-
         # remove cov of old samples
         self.cov_sn *= self.n_frames
         self.cov_sn -= self._cov_sn[0]
 
         old_cov_n = self.cov_n.copy()
         self.cov_n *= sum(self.n_noise_frames)
         self.cov_n -= self._cov_n[0]
@@ -305,16 +302,13 @@
     """
 
     scnr = Subspace(frame_len, mu, lookback, skip, thresh, data_type)
     processed_audio = np.zeros(noisy_signal.shape)
     n = 0
     hop = frame_len // 2
     while noisy_signal.shape[0] - n >= hop:
-
-        processed_audio[
-            n : n + hop,
-        ] = scnr.apply(noisy_signal[n : n + hop])
+        processed_audio[n : n + hop,] = scnr.apply(noisy_signal[n : n + hop])
 
         # update step
         n += hop
 
     return processed_audio
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/directivities.py` & `pyroomacoustics-0.7.4/pyroomacoustics/directivities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import abc
-import numpy as np
 from enum import Enum
+
+import numpy as np
+
 from pyroomacoustics.doa import spher2cart
-from pyroomacoustics.utilities import requires_matplotlib, all_combinations
+from pyroomacoustics.utilities import all_combinations, requires_matplotlib
 
 
 class DirectivityPattern(Enum):
     """
     Common cardioid patterns and their corresponding coefficient for the expression:
 
     .. math::
@@ -211,15 +213,14 @@
             x_offset = 0
             y_offset = 0
 
         if degrees:
             azimuth = np.radians(azimuth)
 
         if colatitude is not None:
-
             if degrees:
                 colatitude = np.radians(colatitude)
 
             if ax is None:
                 fig = plt.figure()
                 ax = fig.add_subplot(1, 1, 1, projection="3d")
 
@@ -258,15 +259,14 @@
                 ax.set_title("Directivity Plot")
 
             ax.set_xlabel("x")
             ax.set_ylabel("y")
             ax.set_zlabel("z")
 
         else:
-
             if ax is None:
                 fig = plt.figure()
                 ax = plt.subplot(111)
 
             # compute response
             resp = self.get_response(azimuth=azimuth, magnitude=True, degrees=False)
             RESP = resp
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/doa/__init__.py` & `pyroomacoustics-0.7.4/pyroomacoustics/doa/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -104,24 +104,24 @@
 
 .. [7] H. Pan, R. Scheibler, E. Bezzam, I. Dokmanic, and M. Vetterli, *FRIDA:
     FRI-based DOA estimation for arbitrary array layouts*, Proc. ICASSP,
     pp 3186-3190, 2017
 
 """
 
+from .cssm import *
 from .doa import *
-from .srp import *
+from .frida import *
+from .grid import *
 from .music import *
 from .normmusic import *
-from .cssm import *
-from .waves import *
+from .srp import *
 from .tops import *
-from .frida import *
-from .grid import *
 from .utils import *
+from .waves import *
 
 # Create this dictionary as a shortcut to different algorithms
 algorithms = {
     "SRP": SRP,
     "MUSIC": MUSIC,
     "NormMUSIC": NormMUSIC,
     "CSSM": CSSM,
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/doa/cssm.py` & `pyroomacoustics-0.7.4/pyroomacoustics/doa/cssm.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,14 @@
         mode="far",
         r=None,
         azimuth=None,
         colatitude=None,
         num_iter=5,
         **kwargs
     ):
-
         MUSIC.__init__(
             self,
             L=L,
             fs=fs,
             nfft=nfft,
             c=c,
             num_src=num_src,
@@ -91,15 +90,14 @@
         beta = []
         invalid = []
 
         # Find number of spatial spectrum peaks at each frequency band.
         # If there are less peaks than expected sources, leave the band out
         # Otherwise, store the location of the peaks.
         for k in range(self.num_freq):
-
             self.grid.set_values(
                 1 / self._compute_spatial_spectrum(C_hat[k, :, :], self.freq_bins[k])
             )
             idx = self.grid.find_peaks(k=self.num_src)
 
             if len(idx) < self.num_src:  # remove frequency
                 invalid.append(k)
@@ -115,15 +113,14 @@
         f0 = self.freq_bins[f0]
 
         # iterate to find DOA, maximum number of iterations is 20
         i = 0
 
         # while(i < self.iter or (len(self.src_idx) < self.num_src and i < 20)):
         while i < self.iter:
-
             # coherent sum
             R = self._coherent_sum(C_hat, f0, beta)
 
             # subspace decomposition
             Es, En, ws, wn = self._subspace_decomposition(R)
 
             # compute spatial spectrum
@@ -133,15 +130,14 @@
             self.grid.set_values(self._compute_spatial_spectrum(cross, f0))
             idx = self.grid.find_peaks(k=self.num_src)
             beta = np.tile(idx, (self.num_freq, 1))
 
             i += 1
 
     def _coherent_sum(self, C_hat, f0, beta):
-
         R = np.zeros((self.M, self.M))
 
         # coherently sum frequencies
         for j in range(len(self.freq_bins)):
             k = self.freq_bins[j]
 
             Aj = self.mode_vec[k, :, beta[j]].T
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/doa/detect_peaks.py` & `pyroomacoustics-0.7.4/pyroomacoustics/doa/detect_peaks.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 Author: Marcos Duarte, https://github.com/demotu/BMC
 Version: 1.0.4
 License: MIT
 """
 
 from __future__ import division, print_function
+
 import numpy as np
 
 __author__ = "Marcos Duarte, https://github.com/demotu/BMC"
 __version__ = "1.0.4"
 __license__ = "MIT"
 
 
@@ -21,15 +22,14 @@
     threshold=0,
     edge="rising",
     kpsh=False,
     valley=False,
     show=False,
     ax=None,
 ):
-
     """
     Detect peaks in data based on their amplitude and other features.
 
     Parameters
     ----------
     x : 1D array_like
         data.
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/doa/doa.py` & `pyroomacoustics-0.7.4/pyroomacoustics/doa/doa.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,14 @@
 
         if precompute:
             self.mode_vec = np.exp(1j * self.omega[:, None, None] * self.tau)
         else:
             self.mode_vec = None
 
     def __getitem__(self, ref):
-
         # If the look up table was precomputed
         if self.precompute:
             return self.mode_vec[ref]
 
         # we use this to test if an integer is passed
         integer = (
             int,
@@ -188,15 +187,14 @@
         azimuth=None,
         colatitude=None,
         n_grid=None,
         dim=2,
         *args,
         **kwargs
     ):
-
         if dim > L.shape[0]:
             raise ValueError("Microphones locations missing dimensions.")
 
         self.L = L  # locations of mics
         self.fs = fs  # sampling frequency
         self.c = c  # speed of sound
         self.M = L.shape[1]  # number of microphones
@@ -232,60 +230,52 @@
             raise ValueError("The dimension must be 2 or 3.")
         else:
             self.dim = dim
 
         # Some logic to create a grid for search
         self.grid = None
         if azimuth is None and colatitude is None:
-
             # Use a default grid size
             if dim == 2:
-
                 if n_grid is None:
                     n_grid = 360
 
                 self.grid = GridCircle(n_points=n_grid)
 
             elif dim == 3:
-
                 if n_grid is None:
                     n_grid = 180 * 90
 
                 self.grid = GridSphere(n_points=n_grid)
 
         elif azimuth is None and colatitude is not None:
-
             raise ValueError("Azimuth should always be specified.")
 
         else:
-
             if dim == 2:
-
                 if colatitude is not None:
                     warnings.warn("Colatitude is ignored for 2D problems.")
 
                 self.grid = GridCircle(azimuth=azimuth)
 
             elif dim == 3:
-
                 if azimuth.ndim != 1:
                     raise ValueError("Azimuth should be a 1D ndarray.")
 
                 if colatitude is None:
                     warnings.warn(
                         "Colatitude is not specified. Setting all colatitude to pi / 2."
                     )
 
                     colatitude = (np.pi / 2) * np.ones(azimuth.shape[0])
                     grid_points = np.vstack((azimuth, colatitude))
 
                     self.grid = GridSphere(spherical_points=grid_points)
 
                 else:
-
                     # when both azimuth and theta are specified,
                     # we assume we want the cartesian product
                     A, C = np.meshgrid(np.unique(azimuth), np.unique(colatitude))
                     grid_points = np.vstack((A.flatten(), C.flatten()))
 
                     self.grid = GridSphere(spherical_points=grid_points)
 
@@ -362,15 +352,14 @@
         # Run the algorithm
         self._process(X)
 
         # locate sources
         from .frida import FRIDA
 
         if not isinstance(self, FRIDA):
-
             self.src_idx = self.grid.find_peaks(k=self.num_src)
 
             self.num_src = len(self.src_idx)
 
             if self.dim == 2:
                 self.azimuth_recon = self.grid.azimuth[self.src_idx]
             elif self.dim == 3:
@@ -419,21 +408,19 @@
         num_mic = self.M
         phi_plt = self.grid.azimuth
 
         # determine amplitudes
         from .frida import FRIDA
 
         if not isinstance(self, FRIDA):  # use spatial spectrum
-
             dirty_img = self.grid.values
             alpha_recon = self.grid.values[self.src_idx]
             alpha_ref = alpha_recon
 
         else:  # create dirty image
-
             dirty_img = self._gen_dirty_img()
             alpha_recon = np.mean(np.abs(self.alpha_recon), axis=1)
             alpha_recon /= alpha_recon.max()
             if alpha_ref is None:  # non-simulated case
                 alpha_ref = alpha_recon
 
         # plot
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/doa/frida.py` & `pyroomacoustics-0.7.4/pyroomacoustics/doa/frida.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import division, print_function
 
+import numpy as np
 from scipy import linalg as la
 
-# import numpy as np
-
-from .doa import *
+from .doa import DOA
 from .tools_fri_doa_plane import (
-    pt_src_recon_multiband,
-    extract_off_diag,
     cov_mtx_est,
-    polar2cart,
+    extract_off_diag,
     make_G,
     make_GtG_and_inv,
+    polar2cart,
+    pt_src_recon_multiband,
 )
 
 
 class FRIDA(DOA):
     """
     Implements the FRI-based direction of arrival finding algorithm [FRIDA]_.
 
@@ -90,15 +89,14 @@
         signal_type="visibility",
         use_lu=True,
         verbose=False,
         symb=True,
         use_cache=False,
         **kwargs
     ):
-
         DOA.__init__(self, L, fs, nfft, c=c, num_src=num_src, mode="far", **kwargs)
 
         # intialize some attributes
         self.visi_noisy_all = None
         self.alpha_recon = np.array(num_src, dtype=float)
 
         # These might be used to select high SNR frames for cross correlation computation
@@ -151,15 +149,14 @@
         else:
             raise ValueError("Signal type can be 'visibility' or 'raw'.")
 
         # loop over all subbands
         self.num_freq = self.freq_bins.shape[0]
 
         if self.dim == 2:
-
             # build the G matrix if necessary
             if self.G is None:
                 self.G = make_G(
                     self.L[0, :],
                     self.L[1, :],
                     2 * np.pi * self.freq_hz,
                     self.c,
@@ -186,15 +183,14 @@
                 signal_type=self.signal_type,
                 G_lst=self.G,
                 GtG_lst=self.GtG,
                 GtG_inv_lst=self.GtG_inv,
             )
 
         elif self.dim == 3:
-
             raise ValueError("3D reconstruction is not yet available with FRIDA.")
 
     def _raw_average(self, X):
         """Correct the time rotation and average the raw microphone signal"""
         phaser = np.exp(
             -1j
             * 2
@@ -204,15 +200,14 @@
             * self.nfft
             / self.fs
         )
 
         return np.mean(X[:, self.freq_bins, :] * phaser, axis=2)
 
     def _visibilities(self, X):
-
         visi_noisy_all = []
         for band_count in range(self.num_freq):
             # Estimate the covariance matrix and extract off-diagonal entries
             fn = self.freq_bins[band_count]
             energy = np.var(X[:, fn, :], axis=0)
             I = np.where(energy > self.stft_noise_margin * self.stft_noise_floor)
             R = cov_mtx_est(X[:, fn, I[0]])
@@ -241,22 +236,20 @@
         :return:
         """
 
         sound_speed = self.c
         num_mic = self.M
 
         if self.dim == 2:
-
             x_plt, y_plt = polar2cart(1, self.grid.azimuth)
             img = np.zeros(self.grid.n_points, dtype=complex)
 
             pos_mic_x = self.L[0, :]
             pos_mic_y = self.L[1, :]
             for i in range(self.num_freq):
-
                 visi = self.visi_noisy_all[:, i]
                 omega_band = 2 * np.pi * self.freq_hz[i]
 
                 pos_mic_x_normalised = pos_mic_x / (sound_speed / omega_band)
                 pos_mic_y_normalised = pos_mic_y / (sound_speed / omega_band)
 
                 count_visi = 0
@@ -272,15 +265,14 @@
                                 -1j * (p_x_qqp * x_plt + p_y_qqp * y_plt)
                             )
                             count_visi += 1
 
             return img / (num_mic * (num_mic - 1))
 
         elif self.dim == 3:
-
             raise ValueError("3D reconstruction is not yet available with FRIDA.")
 
 
 # -------------MISC--------------#
 
 # def polar2cart(rho, phi):
 #     """
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/doa/grid.py` & `pyroomacoustics-0.7.4/pyroomacoustics/doa/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Routines to perform grid search on the sphere
 """
-from __future__ import division, print_function, absolute_import
 
-import numpy as np
-import scipy.spatial as sp  # import ConvexHull, SphericalVoronoi
+from __future__ import absolute_import, division, print_function
 
 from abc import ABCMeta, abstractmethod
 
+import numpy as np
+import scipy.spatial as sp  # import ConvexHull, SphericalVoronoi
+
 from .detect_peaks import detect_peaks
 from .utils import great_circ_dist
 
 
 class Grid:
     """
     This is an abstract class with attributes and methods for grids
@@ -21,15 +22,14 @@
     n_points: int
         the number of points on the grid
     """
 
     __metaclass__ = ABCMeta
 
     def __init__(self, n_points):
-
         self.n_points = n_points
         self.values = None
         self.cartesian = np.zeros((3, n_points))
         self.spherical = np.zeros((2, n_points))
         self.x = self.cartesian[0, :]
         self.y = self.cartesian[1, :]
         self.z = self.cartesian[2, :]
@@ -43,15 +43,14 @@
         return NotImplemented
 
     @abstractmethod
     def find_peaks(self, k=1):
         return NotImplemented
 
     def set_values(self, vals):
-
         vals = np.array(vals)
 
         if vals.ndim == 0:
             self.values = np.ones(self.n_points) * vals
 
         else:
             if vals.shape != (self.n_points,):
@@ -72,15 +71,14 @@
         The number of uniformly spaced points in the grid.
     azimuth: ndarray, optional
         An array of azimuth (in radians) to use for grid locations. Overrides n_points.
     """
 
     def __init__(self, n_points=360, azimuth=None):
         if azimuth is not None:
-
             if azimuth.ndim != 1:
                 raise ValueError("Azimuth must be a 1D ndarray.")
 
             azimuth = np.sort(azimuth)
 
             n_points = azimuth.shape[0]
 
@@ -96,22 +94,20 @@
         self.colatitude[:] = np.pi / 2  # Fix colatitude to ecuador
 
         # cartesian coordinates
         self.x[:] = np.cos(azimuth)
         self.y[:] = np.sin(azimuth)
 
     def apply(self, func, spherical=False):
-
         if spherical:
             self.values = func(self.azimuth)
         else:
             self.values = func(self.x, self.y)
 
     def find_peaks(self, k=1):
-
         # make circular
         val_ext = np.append(self.values, self.values[:10])
 
         # run peak finding
         indexes = detect_peaks(val_ext, show=False) % self.n_points
         candidates = np.unique(indexes)  # get rid of duplicates, if any
 
@@ -119,15 +115,14 @@
         peaks = self.values[candidates]
         max_idx = np.argsort(peaks)[-k:]
 
         # return the indices of peaks found
         return candidates[max_idx]
 
     def plot(self, mark_peaks=0):
-
         try:
             import matplotlib.pyplot as plt
         except ImportError:
             import warnings
 
             warnings.warn("Matplotlib is required for plotting")
             return
@@ -137,15 +132,14 @@
 
         pts = np.append(self.azimuth, self.azimuth[0])
         vals = np.append(self.values, self.values[0])
 
         ax.plot(pts, vals, "-")
 
         if mark_peaks > 0:
-
             idx = self.find_peaks(k=mark_peaks)
 
             ax.plot(pts[idx], vals[idx], "ro")
 
 
 class GridSphere(Grid):
     """
@@ -164,15 +158,14 @@
     ----------
     http://lgdv.cs.fau.de/uploads/publications/spherical_fibonacci_mapping.pdf
     http://stackoverflow.com/questions/9600801/evenly-distributing-n-points-on-a-sphere
     """
 
     def __init__(self, n_points=1000, spherical_points=None):
         if spherical_points is not None:
-
             if spherical_points.ndim != 2 or spherical_points.shape[0] != 2:
                 raise ValueError("spherical_points must be a 2D array with two rows.")
 
             n_points = spherical_points.shape[1]
 
         # Parent constructor
         Grid.__init__(self, n_points)
@@ -250,19 +243,17 @@
 
         min_dist = np.inf
         max_dist = 0
 
         dist = []
 
         for u in range(self.n_points):
-
             phi1, theta1 = self.spherical[:, u]
 
             for v in self.neighbors[u]:
-
                 phi2, theta2 = self.spherical[:, v]
 
                 d = great_circ_dist(1, theta1, phi1, theta2, phi2)
 
                 dist.append(d)
 
                 if d < min_dist:
@@ -283,15 +274,14 @@
         """
 
         candidates = []
 
         # We start by looking at points whose neighbors all have lower values
         # than themselves
         for v in range(self.n_points):
-
             is_local_max = True
 
             for u in self.neighbors[v]:
                 if self.values[u] > self.values[v]:
                     is_local_max = False
                     break
 
@@ -336,15 +326,14 @@
         azimuth_ref=None,
         colatitude_recon=None,
         azimuth_recon=None,
         plotly=True,
         projection=True,
         points_only=False,
     ):
-
         if points_only:
             dirty_img = None
             dirty_grid_x = None
             dirty_grid_y = None
         else:
             dirty_grid_x, dirty_grid_y, dirty_img = self.regrid()
 
@@ -376,53 +365,50 @@
     def plot_old(self, plot_points=False, mark_peaks=0):
         """Plot the points on the sphere with their values"""
 
         from scipy import rand
 
         try:
             import matplotlib.colors as colors
+            import matplotlib.pyplot as plt
 
             # from mpl_toolkits.mplot3d import Axes3D
             import mpl_toolkits.mplot3d as a3
-            import matplotlib.pyplot as plt
         except ImportError:
             import warnings
 
             warnings.warn("Matplotlib is required for plotting")
             return
 
         fig = plt.figure()
         ax = fig.add_subplot(111, projection="3d")
 
         if plot_points:
             ax.scatter(self.x, self.y, self.z, c="b", marker="o")
 
         if mark_peaks > 0:
-
             id = self.find_peaks(k=mark_peaks)
             s = 1.05
             ax.scatter(
                 s * self.x[id], s * self.y[id], s * self.z[id], c="k", marker="o"
             )
 
         voronoi = sp.SphericalVoronoi(self.cartesian.T)
         voronoi.sort_vertices_of_regions()
 
         if self.values is not None:
-
             col_max = self.values.max()
             col_min = self.values.min()
 
             if col_min != col_max:
                 col_map = (self.values - col_min) / (col_max - col_min)
             else:
                 col_map = self.values / col_max
 
         else:
-
             col_map = np.zeros(self.n_points)
 
         cmap = plt.get_cmap("coolwarm")
 
         # plot the walls
         for v_ind, col in zip(voronoi.regions, col_map):
             triangle = a3.art3d.Poly3DCollection(
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/doa/music.py` & `pyroomacoustics-0.7.4/pyroomacoustics/doa/music.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
         mode="far",
         r=None,
         azimuth=None,
         colatitude=None,
         frequency_normalization=False,
         **kwargs
     ):
-
         DOA.__init__(
             self,
             L=L,
             fs=fs,
             nfft=nfft,
             c=c,
             num_src=num_src,
@@ -119,15 +118,14 @@
             import warnings
 
             warnings.warn("Only for 2D.")
             return
 
         # plot
         for k in range(self.num_freq):
-
             freq = float(self.freq_bins[k]) / self.nfft * self.fs
             azimuth = self.grid.azimuth * 180 / np.pi
 
             plt.plot(azimuth, self.Pssl[k, 0 : len(azimuth)])
 
             plt.ylabel("Magnitude")
             plt.xlabel("Azimuth [degrees]")
@@ -142,15 +140,14 @@
         # timeframe, frequ, no idea
         denom = np.matmul(
             np.conjugate(mod_vec[..., None, :]), np.matmul(cross, mod_vec[..., None])
         )
         return 1.0 / abs(denom[..., 0, 0])
 
     def _compute_spatial_spectrum(self, cross, k):
-
         P = np.zeros(self.grid.n_points)
 
         for n in range(self.grid.n_points):
             Dc = np.array(self.mode_vec[k, :, n], ndmin=2).T
             Dc_H = np.conjugate(np.array(self.mode_vec[k, :, n], ndmin=2))
             denom = np.linalg.multi_dot([Dc_H, cross, Dc])
             P[n] = 1 / abs(denom)
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/doa/normmusic.py` & `pyroomacoustics-0.7.4/pyroomacoustics/doa/normmusic.py`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/doa/plotters.py` & `pyroomacoustics-0.7.4/pyroomacoustics/doa/plotters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 A collection of functions to plot maps and points on circles and spheres.
 """
+
 import numpy as np
 
 
 def polar_plt_dirac(
     self,
     azimuth_ref=None,
     alpha_ref=None,
@@ -46,21 +47,19 @@
     num_mic = self.M
     phi_plt = self.grid.azimuth
 
     # determine amplitudes
     from fri import FRI
 
     if not isinstance(self, FRI):  # use spatial spectrum
-
         dirty_img = self.grid.values
         alpha_recon = self.grid.values[self.src_idx]
         alpha_ref = alpha_recon
 
     else:  # create dirty image
-
         dirty_img = self._gen_dirty_img()
         alpha_recon = np.mean(np.abs(self.alpha_recon), axis=1)
         alpha_recon /= alpha_recon.max()
         if alpha_ref is None:  # non-simulated case
             alpha_ref = alpha_recon
 
     # plot
@@ -238,17 +237,17 @@
     surface_base:
         radius corresponding to lowest height on the map
     sufrace_height:
         radius difference between the lowest and highest point on the map
     """
 
     try:
-        from plotly.offline import plot
-        import plotly.graph_objs as go
         import plotly
+        import plotly.graph_objs as go
+        from plotly.offline import plot
     except ImportError:
         import warnings
 
         warnings.warn("The plotly package is required to use this function")
         return
 
     plotly.offline.init_notebook_mode()
@@ -256,15 +255,14 @@
     traces = []
 
     if (
         dirty_img is not None
         and azimuth_grid is not None
         and colatitude_grid is not None
     ):
-
         surfacecolor = np.abs(dirty_img)  # for plotting purposes
 
         base = surface_base
 
         surf_diff = surfacecolor.max() - surfacecolor.min()
         if surf_diff > 0:
             height = surface_height / surf_diff
@@ -292,15 +290,14 @@
         trace1["contours"]["x"]["highlightwidth"] = 1
         trace1["contours"]["y"]["highlightwidth"] = 1
         trace1["contours"]["z"]["highlightwidth"] = 1
 
         traces.append(trace1)
 
     if colatitude_ref is not None and azimuth_ref is not None:
-
         x_ref = np.sin(colatitude_ref) * np.cos(azimuth_ref)
         y_ref = np.sin(colatitude_ref) * np.sin(azimuth_ref)
         z_ref = np.cos(colatitude_ref)
 
         if not hasattr(colatitude_ref, "__iter__"):
             colatitude_ref = [colatitude_ref]
             azimuth_ref = [azimuth_ref]
@@ -331,15 +328,14 @@
                 line=dict(color="rgb(204, 204, 204)", width=2),
                 color="rgb(0, 0.447, 0.741)",
             ),
         )
         traces.append(trace2)
 
     if colatitude is not None and azimuth is not None:
-
         x_recon = np.sin(colatitude) * np.cos(azimuth)
         y_recon = np.sin(colatitude) * np.sin(azimuth)
         z_recon = np.cos(colatitude)
 
         if not hasattr(colatitude, "__iter__"):
             colatitude_ref = [colatitude]
             azimuth = [azimuth]
@@ -437,15 +433,14 @@
     ax = fig.add_subplot(111, projection="mollweide")
 
     if (
         dirty_img is not None
         and colatitude_grid is not None
         and azimuth_grid is not None
     ):
-
         azimuth_plt_internal = azimuth_grid.copy()
         azimuth_plt_internal[azimuth_grid > np.pi] -= np.pi * 2
         p_hd = ax.pcolormesh(
             azimuth_plt_internal,
             np.pi / 2.0 - colatitude_grid,
             np.real(dirty_img),
             cmap="Spectral_r",
@@ -465,15 +460,14 @@
             spacing="proportional",
         )
         # p_hdc.formatter.set_powerlimits((0, 0))
         p_hdc.ax.tick_params(labelsize=8.5)
         p_hdc.update_ticks()
 
     if colatitude_ref is not None and azimuth_ref is not None:
-
         if hasattr(colatitude_ref, "__iter__"):
             K = colatitude_ref.size
             x_ref = azimuth_ref.copy()
             y_ref = (
                 np.pi * 0.5 - colatitude_ref.copy()
             )  # convert CO-LATITUDE to LATITUDE
 
@@ -497,15 +491,14 @@
             marker="^",
             linewidths=0,
             cmap="Spectral_r",
             label="Original",
         )
 
     if colatitude is not None and azimuth is not None:
-
         if hasattr(colatitude, "__iter__"):
             K_est = colatitude.size
             x = azimuth.copy()
             y = np.pi * 0.5 - colatitude.copy()  # convert CO-LATITUDE to LATITUDE
 
             ind = x > np.pi
             x[ind] -= 2 * np.pi  # scale conversion to -pi to pi
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/doa/srp.py` & `pyroomacoustics-0.7.4/pyroomacoustics/doa/srp.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         num_src=1,
         mode="far",
         r=None,
         azimuth=None,
         colatitude=None,
         **kwargs
     ):
-
         DOA.__init__(
             self,
             L=L,
             fs=fs,
             nfft=nfft,
             c=c,
             num_src=num_src,
@@ -105,15 +104,14 @@
         # and we end up with the product:
         # <number of frames> x <number of microphones> x <number of freqs>
         # the number of frames appears because the covariance matrix
         # is not normalized
         DC_offset = pX.shape[-1] * self.L.shape[1] * len(self.freq_bins)
 
         for n in range(self.grid.n_points):
-
             # In the loop, this is just a fancy way of computing
             # the quadratic form:
             # mode_vec^H @ CC @ mode_vec
 
             # get the mode vector axis: (frequency, microphones)
             mode_vec = self.mode_vec[self.freq_bins, :, n]
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/doa/tests/test_doa.py` & `pyroomacoustics-0.7.4/pyroomacoustics/doa/tests/test_doa.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # @version: 1.0  date: 2017/06/20 by Robin Scheibler
 # @author: robin.scheibler@epfl.ch, ivan.dokmanic@epfl.ch, sidney.barthe@epfl.ch
 # @copyright: EPFL-IC-LCAV 2017
 
 import unittest
 
 import numpy as np
-import pyroomacoustics as pra
 from scipy.signal import fftconvolve
 
+import pyroomacoustics as pra
+
 # fix the RNG seed for repeatability
 np.random.seed(0)
 
 # Location of original source
 azimuth = 61.0 / 180.0 * np.pi  # 60 degrees
 tol = 0.3 / 180.0 * np.pi  # 0.3 degrees tolerance for the test
 
@@ -92,15 +93,14 @@
         doa = pra.doa.algorithms["FRIDA"](R, fs, nfft, c=c)
         doa.locate_sources(X, freq_bins=freq_bins)
         print("distance:", pra.doa.circ_dist(azimuth, doa.azimuth_recon))
         self.assertTrue(pra.doa.circ_dist(azimuth, doa.azimuth_recon) < tol)
 
 
 if __name__ == "__main__":
-
     """
     algo_names = sorted(pra.doa.algorithms.keys())
 
     for algo_name in algo_names:
         doa = pra.doa.algorithms[algo_name](R, fs, nfft, c=c, max_four=4)
         doa.locate_sources(X, freq_bins=freq_bins)
         print(
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/doa/tests/test_utils.py` & `pyroomacoustics-0.7.4/pyroomacoustics/doa/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+
 import pyroomacoustics as pra
 
 
 def test_cart_spher_convertion(repetitions=10, vectorized=True):
     """Tests that the convertion is invertible"""
 
     np.random.seed(124584)
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/doa/tools_fri_doa_plane.py` & `pyroomacoustics-0.7.4/pyroomacoustics/doa/tools_fri_doa_plane.py`

 * *Files 0% similar despite different names*

```diff
@@ -1623,15 +1623,14 @@
         )
     )
 
     mtx_brecon = np.zeros((sz_Rc1 + sz_Rc0, sz_Rc1 + sz_Rc0))
     mtx_brecon[:sz_Rc1, :sz_Rc1] = GtG
 
     for inner in range(max_iter):
-
         # update the mtx_loop matrix
         mtx_loop[row_s1:row_e1, col_s1:col_e1] = -R_loop
         mtx_loop[row_s2:row_e2, col_s2:col_e2] = -R_loop.T
 
         # matrix should be symmetric
         # mtx_loop = (mtx_loop + mtx_loop.T) / 2.
         mtx_loop += mtx_loop.T
@@ -1705,15 +1704,14 @@
         signal=signal_type,
     )
 
     return np.array(G_lst)
 
 
 def make_GtG_and_inv(G_lst):
-
     GtG_lst = []
     GtG_inv_lst = []
     for loop in range(len(G_lst)):
         G_loop = G_lst[loop]
 
         GtG = np.dot(G_loop.T, G_loop)
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/doa/tops.py` & `pyroomacoustics-0.7.4/pyroomacoustics/doa/tops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Author: Eric Bezzam
 # Date: July 15, 2016
 
 import numpy as np
-from .music import MUSIC
+from scipy import linalg
 from scipy.linalg import svdvals
 
-from scipy import linalg
+from .music import MUSIC
 
 
 class TOPS(MUSIC):
     """
     Class to apply Test of Orthogonality of Projected Subspaces [TOPS]_ for
     Direction of Arrival (DoA) estimation.
 
@@ -57,15 +57,14 @@
         num_src=1,
         mode="far",
         r=None,
         azimuth=None,
         colatitude=None,
         **kwargs
     ):
-
         MUSIC.__init__(
             self,
             L=L,
             fs=fs,
             nfft=nfft,
             c=c,
             num_src=num_src,
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/doa/utils.py` & `pyroomacoustics-0.7.4/pyroomacoustics/doa/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This module contains useful functions to compute distances and errors on on
 circles and spheres.
 """
+
 from __future__ import division
 
 import numpy as np
 
 
 def circ_dist(azimuth1, azimuth2, r=1.0):
     """
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/doa/waves.py` & `pyroomacoustics-0.7.4/pyroomacoustics/doa/waves.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
         mode="far",
         r=None,
         azimuth=None,
         colatitude=None,
         num_iter=5,
         **kwargs
     ):
-
         MUSIC.__init__(
             self,
             L=L,
             fs=fs,
             nfft=nfft,
             c=c,
             num_src=num_src,
@@ -88,15 +87,14 @@
         C_hat = self._compute_correlation_matrices(X)
 
         # compute initial estimates
         beta = []
         invalid = []
 
         for k in range(self.num_freq):
-
             self.grid.set_values(
                 1 / self._compute_spatial_spectrum(C_hat[k, :, :], self.freq_bins[k])
             )
             idx = self.grid.find_peaks(k=self.num_src)
 
             if len(idx) < self.num_src:  # remove frequency
                 invalid.append(k)
@@ -114,15 +112,14 @@
         i = 0
         self.Z = np.empty(
             (self.M, len(self.freq_bins) * self.num_src), dtype="complex64"
         )
 
         # while(i < self.iter or (len(self.src_idx) < self.num_src and i < 20)):
         while i < self.iter:
-
             # construct waves matrix
             self._construct_waves_matrix(C_hat, f0, beta)
 
             # subspace decomposition with svd
             u, s, v = np.linalg.svd(self.Z)
             Un = u[:, self.num_src :]
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/experimental/__init__.py` & `pyroomacoustics-0.7.4/pyroomacoustics/experimental/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "delay_calibration",
     "deconvolution",
     "localization",
     "signals",
     "rt60",
 ]
 
+from .deconvolution import deconvolve, wiener_deconvolve
+from .delay_calibration import DelayCalibration
+from .localization import edm_line_search, tdoa, tdoa_loc
 from .measure_ir import measure_ir
 from .physics import calculate_speed_of_sound
 from .point_cloud import PointCloud
-from .delay_calibration import DelayCalibration
-from .deconvolution import deconvolve, wiener_deconvolve
-from .localization import tdoa, tdoa_loc, edm_line_search
-from .signals import window, exponential_sweep, linear_sweep
 from .rt60 import measure_rt60
+from .signals import exponential_sweep, linear_sweep, window
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/experimental/deconvolution.py` & `pyroomacoustics-0.7.4/pyroomacoustics/experimental/deconvolution.py`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/experimental/delay_calibration.py` & `pyroomacoustics-0.7.4/pyroomacoustics/experimental/delay_calibration.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,14 @@
         # subtract distance
         delays -= int(distance / self.c * self.fs)
 
         return delays
 
 
 if __name__ == "__main__":
-
     try:
         import sounddevice as sd
 
         sd.default.device = (2, 2)
         sd.default.channels = (1, 2)
         dc = DelayCalibration(
             48000, mls_bits=16, pad_time=0.5, repeat=1, temperature=25.6, humidity=30.0
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/experimental/localization.py` & `pyroomacoustics-0.7.4/pyroomacoustics/experimental/localization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import division, print_function
 
 import numpy as np
 from scipy import linalg as la
+
 from .point_cloud import PointCloud
 
 try:
     import mklfft as fft
 except ImportError:
     import numpy.fft as fft
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/experimental/measure_ir.py` & `pyroomacoustics-0.7.4/pyroomacoustics/experimental/measure_ir.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 try:
     import sounddevice as sd
 
     sounddevice_available = True
 except:
     sounddevice_available = False
 
-from .signals import exponential_sweep, linear_sweep
 from .deconvolution import wiener_deconvolve
+from .signals import exponential_sweep, linear_sweep
 
 _sweep_types = {
     "exponential": exponential_sweep,
     "linear": linear_sweep,
 }
 
 
@@ -173,15 +173,14 @@
     if deconvolution:
         return recorded_signal, h
     else:
         return recorded_signal
 
 
 if __name__ == "__main__":
-
     """
     This is just an interface to measure impulse responses easily
     """
 
     import argparse
 
     parser = argparse.ArgumentParser(
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/experimental/point_cloud.py` & `pyroomacoustics-0.7.4/pyroomacoustics/experimental/point_cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,14 @@
                 self.labels = labels
             else:
                 raise ValueError("There needs to be one label per marker point")
         else:
             self.labels = [str(i) for i in range(self.m)]
 
     def __getitem__(self, ref):
-
         if isinstance(ref, (str, unicode)):
             if self.labels is None:
                 raise ValueError("Labels not set for this marker set")
             index = self.labels.index(ref)
         elif isinstance(ref, int) or isinstance(ref, slice):
             index = ref
         elif isinstance(ref, list):
@@ -333,26 +332,24 @@
 
         azimuth = np.arctan2(v[1], v[0])
         elevation = np.arctan2(v[2], la.norm(v[:2]))
 
         return np.array([azimuth, elevation])
 
     def plot(self, axes=None, show_labels=True, **kwargs):
-
         try:
-            from mpl_toolkits.mplot3d import Axes3D
             import matplotlib.pyplot as plt
+            from mpl_toolkits.mplot3d import Axes3D
         except ImportError:
             import warnings
 
             warnings.warn("Matplotlib is required for plotting")
             return
 
         if self.dim == 2:
-
             # Create a figure if needed
             if axes is None:
                 axes = plt.subplot(111)
 
             axes.plot(self.X[0, :], self.X[1, :], **kwargs)
             axes.axis(aspect="equal")
             plt.show()
@@ -382,15 +379,14 @@
                         None,
                     )
 
         return axes
 
 
 if __name__ == "__main__":
-
     import matplotlib.pyplot as plt
 
     # number of markers
     m = 4
     dim = 2
 
     D = np.zeros((m, m))
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/experimental/rt60.py` & `pyroomacoustics-0.7.4/pyroomacoustics/experimental/rt60.py`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/experimental/signals.py` & `pyroomacoustics-0.7.4/pyroomacoustics/experimental/signals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 A few test signals like sweeps and stuff.
 """
+
 from __future__ import division, print_function
+
 import numpy as np
 
 
 def window(signal, n_win):
     """window the signal at beginning and end with window of size n_win/2"""
 
     win = np.hanning(2 * n_win)
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/experimental/tests/test_deconvolution.py` & `pyroomacoustics-0.7.4/pyroomacoustics/experimental/tests/test_deconvolution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from unittest import TestCase
+
 import numpy as np
 from scipy.signal import fftconvolve
 
 import pyroomacoustics as pra
 
 # fix seed for repeatability
 np.random.seed(0)
@@ -29,15 +30,14 @@
     y += sigma_noise * noise
 
     return y, sigma_noise
 
 
 class TestDeconvolution(TestCase):
     def test_deconvolve_hann_noiseless(self):
-
         h = h_hann
         h_len = h_hann.shape[0]
         SNR = 1000.0
         tol = 1e-7
 
         y, sigma_noise = generate_signals(SNR, x, h, noise)
 
@@ -45,15 +45,14 @@
         rmse = np.sqrt(np.linalg.norm(h_hat - h) ** 2 / h_len)
 
         print("rmse=", rmse, "(tol=", tol, ")")
 
         self.assertTrue(rmse < tol)
 
     def test_wiener_deconvolve_hann_noiseless(self):
-
         h = h_hann
         h_len = h_hann.shape[0]
         SNR = 1000.0
         tol = 1e-7
 
         y, sigma_noise = generate_signals(SNR, x, h, noise)
 
@@ -64,15 +63,14 @@
 
         print("rmse=", rmse, "(tol=", tol, ")")
 
         self.assertTrue(rmse < tol)
 
 
 if __name__ == "__main__":
-
     import matplotlib.pyplot as plt
 
     h = h_hann
     y, sigma_noise = generate_signals(SNR, x, h, noise)
 
     h_hat1 = pra.experimental.deconvolve(y, x, length=h_len)
     res1 = np.linalg.norm(y - fftconvolve(x, h_hat1)) ** 2 / y.shape[0]
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/experimental/tests/test_measure_rt60.py` & `pyroomacoustics-0.7.4/pyroomacoustics/experimental/tests/test_measure_rt60.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """
 Test code for RT60 measurement routine
 """
 import numpy as np
+
 import pyroomacoustics as pra
 
 eps = 1e-15
 
 e_abs = 1.0 - (1.0 - 0.35) ** 2
 room = pra.ShoeBox([10, 7, 6], fs=16000, materials=pra.Material(e_abs), max_order=17)
 room.add_source([3, 2.5, 1.7])
@@ -63,10 +64,9 @@
     matplotlib.use("Agg")
 
     pra.experimental.measure_rt60(ir, plot=True)
     pra.experimental.measure_rt60(ir, plot=True, rt60_tgt=0.3)
 
 
 if __name__ == "__main__":
-
     test_rt60()
     test_rt60_plot()
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/common.hpp` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/common.hpp`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/COPYING.BSD` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/COPYING.BSD`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/COPYING.GPL` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/COPYING.GPL`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/COPYING.LGPL` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/COPYING.LGPL`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/COPYING.MINPACK` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/COPYING.MINPACK`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/COPYING.MPL2` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/COPYING.MPL2`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/COPYING.README` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/COPYING.README`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/CMakeLists.txt` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/Cholesky` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/CholmodSupport` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/Core` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/Core`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/Eigenvalues` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/Geometry` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/Householder` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/IterativeLinearSolvers` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/Jacobi` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/LU` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/LU`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/MetisSupport` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/OrderingMethods` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/PaStiXSupport` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/PardisoSupport` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/QR` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/QR`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/QtAlignedMalloc` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/SPQRSupport` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/SVD` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/Sparse` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/SparseCholesky` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/SparseCore` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/SparseLU` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/SparseQR` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/StdDeque` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/StdList` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/StdVector` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/SuperLUSupport` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/UmfPackSupport` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Cholesky/LDLT.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Cholesky/LLT.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/CholmodSupport/CholmodSupport.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Array.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ArrayBase.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ArrayWrapper.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Assign.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/AssignEvaluator.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Assign_MKL.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/BandMatrix.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Block.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/BooleanRedux.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CommaInitializer.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ConditionEstimator.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CoreEvaluators.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CoreIterators.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CwiseBinaryOp.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CwiseNullaryOp.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CwiseTernaryOp.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CwiseUnaryOp.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CwiseUnaryView.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/DenseBase.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/DenseCoeffsBase.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/DenseStorage.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Diagonal.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/DiagonalMatrix.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/DiagonalProduct.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Dot.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/EigenBase.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ForceAlignedAccess.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Fuzzy.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/GeneralProduct.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/GenericPacketMath.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/GlobalFunctions.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/IO.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Inverse.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Map.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/MapBase.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/MathFunctions.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/MathFunctionsImpl.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Matrix.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/MatrixBase.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/NestByValue.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/NoAlias.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/NumTraits.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/PermutationMatrix.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/PlainObjectBase.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Product.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ProductEvaluators.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Random.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Redux.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Ref.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Replicate.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ReturnByValue.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Reverse.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Select.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/SelfAdjointView.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Solve.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/SolveTriangular.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/SolverBase.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/StableNorm.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Stride.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Swap.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Transpose.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Transpositions.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/TriangularMatrix.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/VectorBlock.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/VectorwiseOp.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Visitor.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX/Complex.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX/PacketMath.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AltiVec/Complex.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/Complex.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/Half.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/Half.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/MathFunctions.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/PacketMath.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/PacketMathHalf.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/PacketMathHalf.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/TypeCasting.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/CUDA/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/Default/ConjHelper.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/Default/Settings.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/NEON/Complex.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/NEON/PacketMath.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/SSE/Complex.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/SSE/PacketMath.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/ZVector/Complex.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/AssignmentFunctors.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/BinaryFunctors.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/NullaryFunctors.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/StlFunctors.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/TernaryFunctors.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/UnaryFunctors.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixVector.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/Parallelizer.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointProduct.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularMatrixVector.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularSolverVector.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/BlasUtil.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/Constants.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/DisableStupidWarnings.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/ForwardDeclarations.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/MKL_support.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/Macros.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/Memory.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/Meta.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/StaticAssert.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/XprHelper.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/ComplexSchur.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/EigenSolver.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/RealQZ.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/RealSchur.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/AlignedBox.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/AngleAxis.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/EulerAngles.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Homogeneous.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Hyperplane.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/OrthoMethods.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/ParametrizedLine.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Quaternion.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Rotation2D.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/RotationBase.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Scaling.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Transform.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Translation.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Umeyama.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/arch/Geometry_SSE.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Geometry/arch/Geometry_SSE.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Householder/BlockHouseholder.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Householder/Householder.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Householder/HouseholderSequence.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Jacobi/Jacobi.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/Determinant.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/FullPivLU.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/InverseImpl.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/PartialPivLU.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/arch/Inverse_SSE.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/LU/arch/Inverse_SSE.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/MetisSupport/MetisSupport.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/OrderingMethods/Amd.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/OrderingMethods/Ordering.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/PardisoSupport/PardisoSupport.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/ColPivHouseholderQR.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/FullPivHouseholderQR.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/HouseholderQR.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/BDCSVD.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/JacobiSVD.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/SVDBase.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/UpperBidiagonalization.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/AmbiVector.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/CompressedStorage.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseAssign.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseBlock.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseColEtree.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseCompressedBase.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseDenseProduct.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseDot.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseFuzzy.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseMap.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseMatrix.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseMatrixBase.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparsePermutation.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseProduct.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseRedux.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseRef.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseSolverBase.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseTranspose.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseTriangularView.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseUtil.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseVector.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseView.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/TriangularSolver.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLUImpl.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_Memory.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_Structs.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_Utils.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseQR/SparseQR.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/StlSupport/StdDeque.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/StlSupport/StdList.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/StlSupport/StdVector.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/StlSupport/details.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/Image.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/Kernel.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/RealSvd2x2.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/blas.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/lapack.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/lapacke.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/BlockMethods.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/geometry.cpp` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/geometry.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -229,99 +229,102 @@
 
 Eigen::Vector3f cross(Eigen::Vector3f v1, Eigen::Vector3f v2)
 {
   /* Convenience function to take cross product of two vectors */
   return v1.cross(v2);
 }
 
+bool on_segment(const Eigen::Vector2f &c1, const Eigen::Vector2f &c2, const Eigen::Vector2f &p) {
+  // Given three collinear points c1, c2, p, the function checks if 
+  // point p lies on line segment c1 <-> c2
+
+  float x_down, x_up, y_down, y_up;
+  x_down = fminf(c1.coeff(0), c2.coeff(0));
+  x_up = fmaxf(c1.coeff(0), c2.coeff(0));
+  y_down = fminf(c1.coeff(1), c2.coeff(1));
+  y_up = fmaxf(c1.coeff(1), c2.coeff(1));
+  return (x_down <= p.coeff(0) && p.coeff(0) <= x_up && y_down <= p.coeff(1) && p.coeff(1) <= y_up);
+}
 
-int is_inside_2d_polygon(const Eigen::Vector2f &p,
+inline int is_left(const Eigen::Vector2f &P0, const Eigen::Vector2f &P1, const Eigen::Vector2f &P2)
+{
+  // isLeft(): tests if a point is Left|On|Right of an infinite line.
+  // on the line is defined as within epsilon
+  // Input: three points P0, P1, and P2
+  // Return: >0 for P2 left of the line through P0 and P1
+  // =0 for P2 on the line
+  // <0 for P2 right of the line
+  // See: Algorithm 1 "Area of Triangles and Polygons"
+  float test_value = (
+      (P1.coeff(0) - P0.coeff(0)) * (P2.coeff(1) - P0.coeff(1))
+      - (P2.coeff(0) - P0.coeff(0)) * (P1.coeff(1) - P0.coeff(1))
+  );
+
+  if (fabsf(test_value) < libroom_eps)
+    return 0;
+  else if (test_value > 0)
+    return 1;
+  else
+    return -1;
+}
+
+int is_inside_2d_polygon(const Eigen::Vector2f &p_test,
     const Eigen::Matrix<float,2,Eigen::Dynamic> &corners)
 {
   /*
-    Checks if a given point is inside a given polygon in 2D.
+    Checks if a given point is inside a given polygon in 2D using the winding
+    number method.
 
     This function checks if a point (defined by its coordinates) is inside
     a polygon (defined by an array of coordinates of its corners) by counting
-    the number of intersections between the borders and a segment linking
-    the given point with a computed point outside the polygon.
-    A boolean is also returned to indicate if a point is on a border of the
-    polygon (the point is still considered inside), which can be useful for
-    limit cases computations.
+    the number of left intersections between the edges and a half-line starting from
+    the test point.
+
+    This is Dave Sunday's winding number algorithm described here:
+    http://profs.ic.uff.br/~anselmo/cursos/CGI/slidesNovos/Inclusion%20of%20a%20Point%20in%20a%20Polygon.pdf
+    It was modified to explicitely check for points on the edges of the polygon.
 
     p: (array size 2) coordinates of the point
     corners: (array size 2xN, N>2) coordinates of the corners of the polygon
     n_corners: the number of corners
 
     returns: 
     -1 : if the point is outside
     0 : the point is inside
     1 : the point is on the boundary
     */
-
-  bool is_inside = false;  // initialize point not in the polygon
-  int c1c2p, c1c2p0, pp0c1, pp0c2;
   int n_corners = corners.cols();
-
-  // find a point outside the polygon
-  int i_min;
-  corners.row(0).minCoeff(&i_min);
-  Eigen::Vector2f p_out;
-  p_out.resize(2);
-  p_out.coeffRef(0) = corners.coeff(0,i_min) - 1;
-  p_out.coeffRef(1) = p.coeff(1);
-
-  // Now count intersections
+  int wn = 0; // the winding number counter
+              // loop through all edges of the polygon
   for (int i = 0, j = n_corners-1 ; i < n_corners ; j=i++)
   {
-
-    // Check first if the point is on the segment
-    // We count the border as inside the polygon
-    c1c2p = ccw3p(corners.col(i), corners.col(j), p);
-    if (c1c2p == 0)
+    if (ccw3p(corners.col(j), corners.col(i), p_test) == 0 && on_segment(corners.col(j), corners.col(i), p_test))
     {
-      // Here we know that p is co-linear with the two corners
-      float x_down, x_up, y_down, y_up;
-      x_down = fminf(corners.coeff(0,i), corners.coeff(0,j));
-      x_up = fmaxf(corners.coeff(0,i), corners.coeff(0,j));
-      y_down = fminf(corners.coeff(1,i), corners.coeff(1,j));
-      y_up = fmaxf(corners.coeff(1,i), corners.coeff(1,j));
-      if (x_down <= p.coeff(0) && p.coeff(0) <= x_up && y_down <= p.coeff(1) && p.coeff(1) <= y_up)
-        return 1;
+      // point is on the edge, we consider it inside
+      return 1;
     }
-
-    // Now check intersection with standard method
-    c1c2p0 = ccw3p(corners.col(i), corners.col(j), p_out);
-    if (c1c2p == c1c2p0)  // no intersection
-      continue;
-
-    pp0c1 = ccw3p(p, p_out, corners.col(i));
-    pp0c2 = ccw3p(p, p_out, corners.col(j));
-    if (pp0c1 == pp0c2)  // no intersection
-      continue;
-
-    // at this point we are sure there is an intersection
-
-    // the second condition takes care of horizontal edges and intersection on vertex
-    float c_max = fmaxf(corners.coeff(1,i), corners.coeff(1,j));
-    if (p.coeff(1) + libroom_eps < c_max)
-    {
-      is_inside = !is_inside;
+    if (corners.coeff(1,j) <= p_test.coeff(1)) { // start y <= P.y
+      if (corners.coeff(1,i) > p_test.coeff(1)) { // an upward crossing
+        if (is_left(corners.col(j), corners.col(i), p_test) > 0) // P left of edge
+          ++wn; // have a valid up intersect
+      }
+    } else { // start y > P.y (no test needed)
+      if (corners.coeff(1, i) <= p_test.coeff(1)) { // a downward crossing
+        if (is_left(corners.col(j), corners.col(i), p_test) < 0) // P right of edge
+          --wn; // have a valid down intersect
+      }
     }
-
   }
 
-  // for a odd number of intersections, the point is in the polygon
-  if (is_inside)
-    return 0;  // point strictly inside
+  if (wn == 0)
+    return -1;
   else
-    return -1; // point is outside
+    return 0;
 }
 
-
 float area_2d_polygon(const Eigen::Matrix<float, 2, Eigen::Dynamic> &corners)
 {
   /*
     Computes the signed area of a 2D surface represented by its corners.
     
     :arg corners: (Eigen::Matrix 2xN, N>2) list of coordinates of the corners forming the surface
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/geometry.hpp` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/geometry.hpp`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/libroom.cpp` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/libroom.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,304 +1,288 @@
-/* 
+/*
  * Python bindings for libroom
  * Copyright (C) 2019  Robin Scheibler, Cyril Cadoux
  *
  * Permission is hereby granted, free of charge, to any person obtaining a copy
  * of this software and associated documentation files (the "Software"), to deal
  * in the Software without restriction, including without limitation the rights
  * to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  * copies of the Software, and to permit persons to whom the Software is
  * furnished to do so, subject to the following conditions:
  *
- * The above copyright notice and this permission notice shall be included in all
- * copies or substantial portions of the Software.
+ * The above copyright notice and this permission notice shall be included in
+ * all copies or substantial portions of the Software.
  *
  * THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
  * IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
  * FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
  * AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  * LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  * OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
  * SOFTWARE.
  *
- * You should have received a copy of the MIT License along with this program. If
- * not, see <https://opensource.org/licenses/MIT>.
+ * You should have received a copy of the MIT License along with this program.
+ * If not, see <https://opensource.org/licenses/MIT>.
  */
 
-#include <string>
-#include <vector>
-#include <pybind11/pybind11.h>
 #include <pybind11/eigen.h>
+#include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
+
 #include <Eigen/Dense>
+#include <string>
+#include <vector>
 
 #include "common.hpp"
 #include "geometry.hpp"
 #include "microphone.hpp"
-#include "wall.hpp"
+#include "rir_builder.hpp"
 #include "room.hpp"
+#include "wall.hpp"
 
 namespace py = pybind11;
 
 float libroom_eps = 1e-5;  // epsilon is set to 0.1 millimeter (100 um)
 
-
 PYBIND11_MODULE(libroom, m) {
-  m.doc() = "Libroom room simulation extension plugin"; // optional module docstring
+  m.doc() =
+      "Libroom room simulation extension plugin";  // optional module docstring
 
   // The 3D Room class
   py::class_<Room<3>>(m, "Room")
-    .def(py::init<
-        const std::vector<Wall<3>> &,
-        const std::vector<int> &,
-        const std::vector<Microphone<3>> &,
-        float, int, float, float, float, float, bool
-        >())
-    .def(py::init<
-        const Vectorf<3> &,
-        const Eigen::Array<float,Eigen::Dynamic,6> &,
-        const Eigen::Array<float,Eigen::Dynamic,6> &,
-        const std::vector<Microphone<3>> &,
-        float, int, float, float, float, float, bool
-        >())
-    .def("set_params", &Room<3>::set_params)
-    .def("add_mic", &Room<3>::add_mic)
-    .def("reset_mics", &Room<3>::reset_mics)
-    .def("image_source_model", &Room<3>::image_source_model)
-    .def("get_wall", &Room<3>::get_wall)
-    .def("get_max_distance", &Room<3>::get_max_distance)
-    .def("next_wall_hit", &Room<3>::next_wall_hit)
-    .def("scat_ray", &Room<3>::scat_ray)
-    .def("simul_ray", &Room<3>::simul_ray)
-    .def("ray_tracing",
-        (void (Room<3>::*)(
-                             const Eigen::Matrix<float,2,Eigen::Dynamic> &angles,
-                             const Vectorf<3> source_pos
-                             )
-        )
-        &Room<3>::ray_tracing)
-    .def("ray_tracing",
-        (void (Room<3>::*)(
-                             size_t nb_phis,
-                             size_t nb_thetas,
-                             const Vectorf<3> source_pos
-                             )
-        )
-        &Room<3>::ray_tracing)
-    .def("ray_tracing",
-        (void (Room<3>::*)(
-                             size_t nb_rays,
-                             const Vectorf<3> source_pos
-                             )
-        )
-        &Room<3>::ray_tracing)
-    .def("contains", &Room<3>::contains)
-    .def_property("is_hybrid_sim", &Room<3>::get_is_hybrid_sim, &Room<3>::set_is_hybrid_sim)
-    .def_property_readonly_static("dim", [](py::object /* self */) { return 3; })
-    .def_readonly("walls", &Room<3>::walls)
-    .def_readonly("sources", &Room<3>::sources)
-    .def_readonly("orders", &Room<3>::orders)
-    .def_readonly("orders_xyz", &Room<3>::orders_xyz)
-    .def_readonly("attenuations", &Room<3>::attenuations)
-    .def_readonly("gen_walls", &Room<3>::gen_walls)
-    .def_readonly("visible_mics", &Room<3>::visible_mics)
-    .def_readonly("walls", &Room<3>::walls)
-    .def_readonly("obstructing_walls", &Room<3>::obstructing_walls)
-    .def_readonly("microphones", &Room<3>::microphones)
-    .def_readonly("max_dist", &Room<3>::max_dist)
-    ;
+      .def(py::init<const std::vector<Wall<3>> &, const std::vector<int> &,
+                    const std::vector<Microphone<3>> &, float, int, float,
+                    float, float, float, bool>())
+      .def(py::init<const Vectorf<3> &,
+                    const Eigen::Array<float, Eigen::Dynamic, 6> &,
+                    const Eigen::Array<float, Eigen::Dynamic, 6> &,
+                    const std::vector<Microphone<3>> &, float, int, float,
+                    float, float, float, bool>())
+      .def("set_params", &Room<3>::set_params)
+      .def("add_mic", &Room<3>::add_mic)
+      .def("reset_mics", &Room<3>::reset_mics)
+      .def("image_source_model", &Room<3>::image_source_model)
+      .def("get_wall", &Room<3>::get_wall)
+      .def("get_max_distance", &Room<3>::get_max_distance)
+      .def("next_wall_hit", &Room<3>::next_wall_hit)
+      .def("scat_ray", &Room<3>::scat_ray)
+      .def("simul_ray", &Room<3>::simul_ray)
+      .def("ray_tracing",
+           (void(Room<3>::*)(
+               const Eigen::Matrix<float, 2, Eigen::Dynamic> &angles,
+               const Vectorf<3> source_pos)) &
+               Room<3>::ray_tracing)
+      .def("ray_tracing", (void(Room<3>::*)(size_t nb_phis, size_t nb_thetas,
+                                            const Vectorf<3> source_pos)) &
+                              Room<3>::ray_tracing)
+      .def("ray_tracing",
+           (void(Room<3>::*)(size_t nb_rays, const Vectorf<3> source_pos)) &
+               Room<3>::ray_tracing)
+      .def("contains", &Room<3>::contains)
+      .def_property("is_hybrid_sim", &Room<3>::get_is_hybrid_sim,
+                    &Room<3>::set_is_hybrid_sim)
+      .def_property_readonly_static("dim",
+                                    [](py::object /* self */) { return 3; })
+      .def_readonly("walls", &Room<3>::walls)
+      .def_readonly("sources", &Room<3>::sources)
+      .def_readonly("orders", &Room<3>::orders)
+      .def_readonly("orders_xyz", &Room<3>::orders_xyz)
+      .def_readonly("attenuations", &Room<3>::attenuations)
+      .def_readonly("gen_walls", &Room<3>::gen_walls)
+      .def_readonly("visible_mics", &Room<3>::visible_mics)
+      .def_readonly("walls", &Room<3>::walls)
+      .def_readonly("obstructing_walls", &Room<3>::obstructing_walls)
+      .def_readonly("microphones", &Room<3>::microphones)
+      .def_readonly("max_dist", &Room<3>::max_dist);
 
   // The 2D Room class
   py::class_<Room<2>>(m, "Room2D")
-    //.def(py::init<py::list, py::list, const Eigen::MatrixXf &>())
-    .def(py::init<
-        const std::vector<Wall<2>> &,
-        const std::vector<int> &,
-        const std::vector<Microphone<2>> &,
-        float, int, float, float, float, float, bool
-        >())
-    .def(py::init<
-        const Vectorf<2> &,
-        const Eigen::Array<float,Eigen::Dynamic,4> &,
-        const Eigen::Array<float,Eigen::Dynamic,4> &,
-        const std::vector<Microphone<2>> &,
-        float, int, float, float, float, float, bool
-        >())
-    .def("set_params", &Room<2>::set_params)
-    .def("add_mic", &Room<2>::add_mic)
-    .def("reset_mics", &Room<2>::reset_mics)
-    .def("image_source_model", &Room<2>::image_source_model)
-    .def("get_wall", &Room<2>::get_wall)
-    .def("get_max_distance", &Room<2>::get_max_distance)
-    .def("next_wall_hit", &Room<2>::next_wall_hit)
-    .def("scat_ray", &Room<2>::scat_ray)
-    .def("simul_ray", &Room<2>::simul_ray)
-    .def("ray_tracing",
-        (void (Room<2>::*)(
-                             const Eigen::Matrix<float,1,Eigen::Dynamic> &angles,
-                             const Vectorf<2> source_pos
-                            )
-        )
-        &Room<2>::ray_tracing)
-    .def("ray_tracing",
-        (void (Room<2>::*)(
-                             size_t nb_phis,
-                             size_t nb_thetas,
-                             const Vectorf<2> source_pos
-                            )
-        )
-        &Room<2>::ray_tracing)
-    .def("ray_tracing",
-        (void (Room<2>::*)(
-                             size_t n_rays,
-                             const Vectorf<2> source_pos
-                            )
-        )
-        &Room<2>::ray_tracing)
-    .def("contains", &Room<2>::contains)
-    .def_property_readonly_static("dim", [](py::object /* self */) { return 2; })
-    .def_property("is_hybrid_sim", &Room<2>::get_is_hybrid_sim, &Room<2>::set_is_hybrid_sim)
-    .def_readonly("walls", &Room<2>::walls)
-    .def_readonly("sources", &Room<2>::sources)
-    .def_readonly("orders", &Room<2>::orders)
-    .def_readonly("orders_xyz", &Room<2>::orders_xyz)
-    .def_readonly("attenuations", &Room<2>::attenuations)
-    .def_readonly("gen_walls", &Room<2>::gen_walls)
-    .def_readonly("visible_mics", &Room<2>::visible_mics)
-    .def_readonly("walls", &Room<2>::walls)
-    .def_readonly("obstructing_walls", &Room<2>::obstructing_walls)
-    .def_readonly("microphones", &Room<2>::microphones)
-    .def_readonly("max_dist", &Room<2>::max_dist)
-    ;
+      //.def(py::init<py::list, py::list, const Eigen::MatrixXf &>())
+      .def(py::init<const std::vector<Wall<2>> &, const std::vector<int> &,
+                    const std::vector<Microphone<2>> &, float, int, float,
+                    float, float, float, bool>())
+      .def(py::init<const Vectorf<2> &,
+                    const Eigen::Array<float, Eigen::Dynamic, 4> &,
+                    const Eigen::Array<float, Eigen::Dynamic, 4> &,
+                    const std::vector<Microphone<2>> &, float, int, float,
+                    float, float, float, bool>())
+      .def("set_params", &Room<2>::set_params)
+      .def("add_mic", &Room<2>::add_mic)
+      .def("reset_mics", &Room<2>::reset_mics)
+      .def("image_source_model", &Room<2>::image_source_model)
+      .def("get_wall", &Room<2>::get_wall)
+      .def("get_max_distance", &Room<2>::get_max_distance)
+      .def("next_wall_hit", &Room<2>::next_wall_hit)
+      .def("scat_ray", &Room<2>::scat_ray)
+      .def("simul_ray", &Room<2>::simul_ray)
+      .def("ray_tracing",
+           (void(Room<2>::*)(
+               const Eigen::Matrix<float, 1, Eigen::Dynamic> &angles,
+               const Vectorf<2> source_pos)) &
+               Room<2>::ray_tracing)
+      .def("ray_tracing", (void(Room<2>::*)(size_t nb_phis, size_t nb_thetas,
+                                            const Vectorf<2> source_pos)) &
+                              Room<2>::ray_tracing)
+      .def("ray_tracing",
+           (void(Room<2>::*)(size_t n_rays, const Vectorf<2> source_pos)) &
+               Room<2>::ray_tracing)
+      .def("contains", &Room<2>::contains)
+      .def_property_readonly_static("dim",
+                                    [](py::object /* self */) { return 2; })
+      .def_property("is_hybrid_sim", &Room<2>::get_is_hybrid_sim,
+                    &Room<2>::set_is_hybrid_sim)
+      .def_readonly("walls", &Room<2>::walls)
+      .def_readonly("sources", &Room<2>::sources)
+      .def_readonly("orders", &Room<2>::orders)
+      .def_readonly("orders_xyz", &Room<2>::orders_xyz)
+      .def_readonly("attenuations", &Room<2>::attenuations)
+      .def_readonly("gen_walls", &Room<2>::gen_walls)
+      .def_readonly("visible_mics", &Room<2>::visible_mics)
+      .def_readonly("walls", &Room<2>::walls)
+      .def_readonly("obstructing_walls", &Room<2>::obstructing_walls)
+      .def_readonly("microphones", &Room<2>::microphones)
+      .def_readonly("max_dist", &Room<2>::max_dist);
 
   // The Wall class
   py::class_<Wall<3>> wall_cls(m, "Wall");
 
   wall_cls
-    .def(py::init<const Eigen::Matrix<float,3,Eigen::Dynamic> &, const Eigen::ArrayXf &, const Eigen::ArrayXf &, const std::string &>(),
-        py::arg("corners"), py::arg("absorption") = Eigen::ArrayXf::Zero(1),
-        py::arg("scattering") = Eigen::ArrayXf::Zero(1), py::arg("name") = "")
-    .def("area", &Wall<3>::area)
-    .def("intersection", &Wall<3>::intersection)
-    .def("intersects", &Wall<3>::intersects)
-    .def("side", &Wall<3>::side)
-    .def("reflect", &Wall<3>::reflect)
-    .def("normal_reflect", (Vectorf<3>(Wall<3>::*)(const Vectorf<3>&, const Vectorf<3>&, float) const)&Wall<3>::normal_reflect)
-    .def("normal_reflect", (Vectorf<3>(Wall<3>::*)(const Vectorf<3>&) const)&Wall<3>::normal_reflect)
-    .def("same_as", &Wall<3>::same_as)
-    .def_property_readonly_static("dim", [](py::object /* self */) { return 3; })
-    .def_readwrite("absorption", &Wall<3>::absorption)
-    .def_readwrite("scatter", &Wall<3>::scatter)
-    .def_readwrite("name", &Wall<3>::name)
-    .def_readonly("corners", &Wall<3>::corners)
-    .def_readonly("origin", &Wall<3>::origin)
-    .def_readonly("normal", &Wall<3>::normal)
-    .def_readonly("basis", &Wall<3>::basis)
-    .def_readonly("flat_corners", &Wall<3>::flat_corners)
-    ;
+      .def(py::init<const Eigen::Matrix<float, 3, Eigen::Dynamic> &,
+                    const Eigen::ArrayXf &, const Eigen::ArrayXf &,
+                    const std::string &>(),
+           py::arg("corners"), py::arg("absorption") = Eigen::ArrayXf::Zero(1),
+           py::arg("scattering") = Eigen::ArrayXf::Zero(1),
+           py::arg("name") = "")
+      .def("area", &Wall<3>::area)
+      .def("intersection", &Wall<3>::intersection)
+      .def("intersects", &Wall<3>::intersects)
+      .def("side", &Wall<3>::side)
+      .def("reflect", &Wall<3>::reflect)
+      .def("normal_reflect",
+           (Vectorf<3>(Wall<3>::*)(const Vectorf<3> &, const Vectorf<3> &,
+                                   float) const) &
+               Wall<3>::normal_reflect)
+      .def("normal_reflect",
+           (Vectorf<3>(Wall<3>::*)(const Vectorf<3> &) const) &
+               Wall<3>::normal_reflect)
+      .def("same_as", &Wall<3>::same_as)
+      .def_property_readonly_static("dim",
+                                    [](py::object /* self */) { return 3; })
+      .def_readwrite("absorption", &Wall<3>::absorption)
+      .def_readwrite("scatter", &Wall<3>::scatter)
+      .def_readwrite("name", &Wall<3>::name)
+      .def_readonly("corners", &Wall<3>::corners)
+      .def_readonly("origin", &Wall<3>::origin)
+      .def_readonly("normal", &Wall<3>::normal)
+      .def_readonly("basis", &Wall<3>::basis)
+      .def_readonly("flat_corners", &Wall<3>::flat_corners);
 
   py::enum_<Wall<3>::Isect>(wall_cls, "Isect")
-    .value("NONE", Wall<3>::Isect::NONE)
-    .value("VALID", Wall<3>::Isect::VALID)
-    .value("ENDPT", Wall<3>::Isect::ENDPT)
-    .value("BNDRY", Wall<3>::Isect::BNDRY)
-    .export_values();
+      .value("NONE", Wall<3>::Isect::NONE)
+      .value("VALID", Wall<3>::Isect::VALID)
+      .value("ENDPT", Wall<3>::Isect::ENDPT)
+      .value("BNDRY", Wall<3>::Isect::BNDRY)
+      .export_values();
 
   // The Wall class
   py::class_<Wall<2>> wall2d_cls(m, "Wall2D");
 
   wall2d_cls
-    .def(py::init<const Eigen::Matrix<float,2,Eigen::Dynamic> &, const Eigen::ArrayXf &, const Eigen::ArrayXf &, std::string &>(),
-        py::arg("corners"), py::arg("absorption") = Eigen::ArrayXf::Zero(1),
-        py::arg("scattering") = Eigen::ArrayXf::Zero(1), py::arg("name") = "")
-    .def("area", &Wall<2>::area)
-    .def("intersection", &Wall<2>::intersection)
-    .def("intersects", &Wall<2>::intersects)
-    .def("side", &Wall<2>::side)
-    .def("reflect", &Wall<2>::reflect)
-    .def("normal_reflect", (Vectorf<2>(Wall<2>::*)(const Vectorf<2>&, const Vectorf<2>&, float) const)&Wall<2>::normal_reflect)
-    .def("normal_reflect", (Vectorf<2>(Wall<2>::*)(const Vectorf<2>&) const)&Wall<2>::normal_reflect)
-    .def("same_as", &Wall<2>::same_as)
-    .def_property_readonly_static("dim", [](py::object /* self */) { return 2; })
-    .def_readwrite("absorption", &Wall<2>::absorption)
-    .def_readwrite("scatter", &Wall<2>::scatter)
-    .def_readwrite("name", &Wall<2>::name)
-    .def_readonly("corners", &Wall<2>::corners)
-    .def_readonly("origin", &Wall<2>::origin)
-    .def_readonly("normal", &Wall<2>::normal)
-    .def_readonly("basis", &Wall<2>::basis)
-    .def_readonly("flat_corners", &Wall<2>::flat_corners)
-    ;
+      .def(py::init<const Eigen::Matrix<float, 2, Eigen::Dynamic> &,
+                    const Eigen::ArrayXf &, const Eigen::ArrayXf &,
+                    std::string &>(),
+           py::arg("corners"), py::arg("absorption") = Eigen::ArrayXf::Zero(1),
+           py::arg("scattering") = Eigen::ArrayXf::Zero(1),
+           py::arg("name") = "")
+      .def("area", &Wall<2>::area)
+      .def("intersection", &Wall<2>::intersection)
+      .def("intersects", &Wall<2>::intersects)
+      .def("side", &Wall<2>::side)
+      .def("reflect", &Wall<2>::reflect)
+      .def("normal_reflect",
+           (Vectorf<2>(Wall<2>::*)(const Vectorf<2> &, const Vectorf<2> &,
+                                   float) const) &
+               Wall<2>::normal_reflect)
+      .def("normal_reflect",
+           (Vectorf<2>(Wall<2>::*)(const Vectorf<2> &) const) &
+               Wall<2>::normal_reflect)
+      .def("same_as", &Wall<2>::same_as)
+      .def_property_readonly_static("dim",
+                                    [](py::object /* self */) { return 2; })
+      .def_readwrite("absorption", &Wall<2>::absorption)
+      .def_readwrite("scatter", &Wall<2>::scatter)
+      .def_readwrite("name", &Wall<2>::name)
+      .def_readonly("corners", &Wall<2>::corners)
+      .def_readonly("origin", &Wall<2>::origin)
+      .def_readonly("normal", &Wall<2>::normal)
+      .def_readonly("basis", &Wall<2>::basis)
+      .def_readonly("flat_corners", &Wall<2>::flat_corners);
 
   // The different wall intersection cases
   m.attr("WALL_ISECT_NONE") = WALL_ISECT_NONE;
   m.attr("WALL_ISECT_VALID") = WALL_ISECT_VALID;
   m.attr("WALL_ISECT_VALID_ENDPT") = WALL_ISECT_VALID_ENDPT;
   m.attr("WALL_ISECT_VALID_BNDRY") = WALL_ISECT_VALID_BNDRY;
 
   // The microphone class
   py::class_<Microphone<3>>(m, "Microphone")
-    .def(py::init<const Vectorf<3> &, int, float, float>())
-    .def_readonly("loc", &Microphone<3>::loc)
-    .def_readonly("hits", &Microphone<3>::hits)
-    .def_readonly("histograms", &Microphone<3>::histograms)
-    ;
+      .def(py::init<const Vectorf<3> &, int, float, float>())
+      .def_readonly("loc", &Microphone<3>::loc)
+      .def_readonly("hits", &Microphone<3>::hits)
+      .def_readonly("histograms", &Microphone<3>::histograms);
 
   py::class_<Microphone<2>>(m, "Microphone2D")
-    .def(py::init<const Vectorf<2> &, int, float, float>())
-    .def_readonly("loc", &Microphone<2>::loc)
-    .def_readonly("hits", &Microphone<2>::hits)
-    .def_readonly("histograms", &Microphone<2>::histograms)
-    ;
+      .def(py::init<const Vectorf<2> &, int, float, float>())
+      .def_readonly("loc", &Microphone<2>::loc)
+      .def_readonly("hits", &Microphone<2>::hits)
+      .def_readonly("histograms", &Microphone<2>::histograms);
 
   // The 2D histogram class
   py::class_<Histogram2D>(m, "Histogram2D")
-    .def(py::init<int, int>())
-    .def("log", &Histogram2D::log)
-    .def("bin", &Histogram2D::bin)
-    .def("get_hist", &Histogram2D::get_hist)
-    .def("reset", &Histogram2D::reset)
-    ;
+      .def(py::init<int, int>())
+      .def("log", &Histogram2D::log)
+      .def("bin", &Histogram2D::bin)
+      .def("get_hist", &Histogram2D::get_hist)
+      .def("reset", &Histogram2D::reset);
 
   // Structure to hold detector hit information
   py::class_<Hit>(m, "Hit")
-    .def(py::init<int>())
-    .def(py::init<const float, const Eigen::ArrayXf &>())
-    .def_readonly("transmitted", &Hit::transmitted)
-    .def_readonly("distance", &Hit::distance)
-    ;
+      .def(py::init<int>())
+      .def(py::init<const float, const Eigen::ArrayXf &>())
+      .def_readonly("transmitted", &Hit::transmitted)
+      .def_readonly("distance", &Hit::distance);
 
   // getter and setter for geometric epsilon
   m.def("set_eps", [](const float &eps) { libroom_eps = eps; });
   m.def("get_eps", []() { return libroom_eps; });
 
   // Routines for the geometry packages
   m.def("ccw3p", &ccw3p, "Determines the orientation of three points");
 
-  m.def("check_intersection_2d_segments",
-      &check_intersection_2d_segments,
-      "A function that checks if two line segments intersect");
-
-  m.def("intersection_2d_segments",
-      &intersection_2d_segments,
-      "A function that finds the intersection of two line segments");
-
-  m.def("intersection_3d_segment_plane",
-      &intersection_3d_segment_plane,
-      "A function that finds the intersection between a line segment and a plane");
+  m.def("check_intersection_2d_segments", &check_intersection_2d_segments,
+        "A function that checks if two line segments intersect");
+
+  m.def("intersection_2d_segments", &intersection_2d_segments,
+        "A function that finds the intersection of two line segments");
+
+  m.def("intersection_3d_segment_plane", &intersection_3d_segment_plane,
+        "A function that finds the intersection between a line segment and a "
+        "plane");
 
   m.def("cross", &cross, "Cross product of two 3D vectors");
 
   m.def("is_inside_2d_polygon", &is_inside_2d_polygon,
-      "Checks if a 2D point lies in or out of a planar polygon");
+        "Checks if a 2D point lies in or out of a planar polygon");
 
   m.def("area_2d_polygon", &area_2d_polygon,
-      "Compute the signed area of a planar polygon");
+        "Compute the signed area of a planar polygon");
 
   m.def("cos_angle_between", &cos_angle_between,
-      "Computes the angle between two 2D or 3D vectors");
+        "Computes the angle between two 2D or 3D vectors");
 
   m.def("dist_line_point", &dist_line_point,
-      "Computes the distance between a point and an infinite line");
+        "Computes the distance between a point and an infinite line");
 
+  m.def("rir_builder", &rir_builder, "RIR builder");
+  m.def("delay_sum", &delay_sum, "Delay and sum");
+  m.def("fractional_delay", &fractional_delay, "Fractional delays");
 }
-
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/microphone.hpp` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/microphone.hpp`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/room.cpp` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/room.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -658,15 +658,15 @@
     // There are no obstructing walls in shoebox rooms
     if (scattered_ray)
       return std::make_tuple(result, -1, 0.);
 
     // The direction vector
     Vectorf<D> dir = end - start;
 
-    for (int shoebox_orders_idx = 0 ; shoebox_orders_idx < D ; shoebox_orders_idx++)
+    for (size_t shoebox_orders_idx = 0 ; shoebox_orders_idx < D ; shoebox_orders_idx++)
     {
       auto d = shoebox_orders[shoebox_orders_idx];
 
       float abs_dir0 = std::abs(dir[d[0]]);
       if (abs_dir0 < libroom_eps)
         continue;
 
@@ -725,15 +725,15 @@
     size_t n_walls = scattered_ray ? obstructing_walls.size() : walls.size();
 
     for (size_t i(0) ; i < n_walls ; ++i)
     {
       Wall<D> & w = scattered_ray ? walls[obstructing_walls[i]] : walls[i];
 
       // To store the result of this iteration
-      Vectorf<D> temp_hit;
+      Vectorf<D> temp_hit = Vectorf<D>::Zero();
 
       // As a side effect, temp_hit gets a value (VectorXf) here
       int ret = w.intersection(start, end, temp_hit);
 
       if (ret > -1)
       {
         float temp_dist = (temp_hit - start).norm();
@@ -944,14 +944,15 @@
           //   because the ray will continue its way          
           float travel_dist_at_mic = travel_dist + distance;
 
           double r_sq = double(travel_dist_at_mic) * travel_dist_at_mic;
           auto p_hit = (1 - sqrt(1 - mic_radius_sq / std::max(mic_radius_sq, r_sq)));
           energy = transmitted / (r_sq * p_hit);
           // energy = transmitted / (travel_dist_at_mic - sqrtf(fmaxf(0.f, travel_dist_at_mic * travel_dist_at_mic - mic_radius_sq)));
+
           microphones[k].log_histogram(travel_dist_at_mic, energy, start);
         }
       }
     }
 
     // Update the characteristics
     travel_dist += hit_distance;
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/room.hpp` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/room.hpp`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/wall.cpp` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/wall.cpp`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/libroom_src/wall.hpp` & `pyroomacoustics-0.7.4/pyroomacoustics/libroom_src/wall.hpp`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/metrics.py` & `pyroomacoustics-0.7.4/pyroomacoustics/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import os
 import platform
 
 import numpy as np
+
+try:
+    from scipy.signal import hann
+except ImportError:
+    from scipy.signal.windows import hann
+
 from scipy.stats import binom as _binom
 from scipy.stats import norm as _norm
-from scipy.signal import hann
 
 from .transform import stft
 
 
 def median(x, alpha=None, axis=-1, keepdims=False):
     """
     Computes 95% confidence interval for the median.
@@ -34,34 +39,23 @@
 
     # sort the array
     xsw = np.sort(xsw, axis=0)
     n = xsw.shape[0]
 
     if n % 2 == 1:
         # if n is odd, take central element
-        m = xsw[
-            n // 2,
-        ]
+        m = xsw[n // 2,]
     else:
         # if n is even, average the two central elements
-        m = 0.5 * (
-            xsw[
-                n // 2 - 1,
-            ]
-            + xsw[
-                n // 2,
-            ]
-        )
+        m = 0.5 * (xsw[n // 2 - 1,] + xsw[n // 2,])
 
     if alpha is None:
         if keepdims:
             m = np.moveaxis(
-                m[
-                    np.newaxis,
-                ],
+                m[np.newaxis,],
                 0,
                 axis,
             )
         return m
 
     else:
         # bound for using the large n approximation
@@ -81,49 +75,35 @@
             if j < 0:
                 raise ValueError(
                     "Warning: Sample size is too small. No confidence interval found."
                 )
             else:
                 ci = np.array(
                     [
-                        xsw[
-                            j,
-                        ]
-                        - m,
-                        xsw[
-                            k,
-                        ]
-                        - m,
+                        xsw[j,] - m,
+                        xsw[k,] - m,
                     ]
                 )
 
         else:
             # we use the Normal approximation for large sets
             norm = _norm()
             eta = norm.ppf(1 - alpha / 2)
             j = int(np.floor(0.5 * n - 0.5 * eta * np.sqrt(n))) - 1
             k = int(np.ceil(0.5 * n + 0.5 * eta * np.sqrt(n)))
             ci = np.array(
                 [
-                    xsw[
-                        j,
-                    ]
-                    - m,
-                    xsw[
-                        k,
-                    ]
-                    - m,
+                    xsw[j,] - m,
+                    xsw[k,] - m,
                 ]
             )
 
         if keepdims:
             m = np.moveaxis(
-                m[
-                    np.newaxis,
-                ],
+                m[np.newaxis,],
                 0,
                 axis,
             )
             if axis < 0:
                 ci = np.moveaxis(
                     ci[
                         :,
@@ -160,15 +140,14 @@
     :returns: (float) The mean of the squared differences of x1 and x2.
     """
     return (np.abs(x1 - x2) ** 2).sum() / len(x1)
 
 
 # Itakura-Saito distance function
 def itakura_saito(x1, x2, sigma2_n, stft_L=128, stft_hop=128):
-
     P1 = np.abs(stft.analysis(x1, stft_L, stft_hop)) ** 2
     P2 = np.abs(stft(x2, stft_L, stft_hop)) ** 2
 
     VAD1 = P1.mean(axis=1) > 2 * stft_L**2 * sigma2_n
     VAD2 = P2.mean(axis=1) > 2 * stft_L**2 * sigma2_n
     VAD = np.logical_or(VAD1, VAD2)
 
@@ -179,15 +158,14 @@
 
     IS = (R - np.log(R) - 1.0).mean(axis=1)
 
     return np.median(IS)
 
 
 def snr(ref, deg):
-
     return np.sum(ref**2) / np.sum((ref - deg) ** 2)
 
 
 # Perceptual Evaluation of Speech Quality for multiple files using multiple threads
 def pesq(ref_file, deg_files, Fs=8000, swap=False, wb=False, bin="./bin/pesq"):
     """
     pesq_vals = pesq(ref_file, deg_files, sample_rate=None, bin='./bin/pesq'):
@@ -240,15 +218,14 @@
     pipes = [
         subprocess.Popen(args + [deg], stdout=subprocess.PIPE) for deg in deg_files
     ]
     states = np.ones(len(pipes), dtype=np.bool)
 
     # Recover output as the processes finish
     while states.any():
-
         for i, p in enumerate(pipes):
             if states[i] == True and p.poll() is not None:
                 states[i] = False
                 out = p.stdout.readlines()
                 last_line = out[-1][:-2]
 
                 if wb is True:
@@ -330,15 +307,14 @@
     # slope values
     nCoeffs = 500
     coeffs = np.linspace(5000, 150000, nCoeffs)
     ss = np.zeros(nCoeffs)
 
     # loop through different slope values
     for k in range(nCoeffs):
-
         # get masks
         a = coeffs[k]
 
         maskTime = np.logical_and(t_mesh > t_min, t_mesh < t_max)
 
         maskFreq = np.logical_and(
             f_mesh > t_mesh * a - fb / 2, f_mesh < t_mesh * a + fb / 2
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/multirate.py` & `pyroomacoustics-0.7.4/pyroomacoustics/multirate.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     # constraints
     N_C = int(C * N)
     w = np.linspace(0, w_max * np.pi, N_C)[:, np.newaxis]
 
     n = np.arange(N)
 
     try:
-        from cvxopt import solvers, matrix
+        from cvxopt import matrix, solvers
     except:
         raise ValueError(
             "To use the frac_delay function, the cvxopt module is necessary."
         )
 
     f = np.concatenate((np.zeros(N), np.ones(1)))
 
@@ -66,15 +66,14 @@
     plt.plot(h)
     """
 
     return h
 
 
 def low_pass(numtaps, B, epsilon=0.1):
-
     bands = [0, (1 - epsilon) * B, B, 0.5]
     desired = [1, 0]
 
     from scipy.signal import remez
 
     h = remez(numtaps, bands, desired, grid_density=32)
 
@@ -92,15 +91,14 @@
     plt.plot(h)
     """
 
     return h
 
 
 def resample(x, p, q):
-
     import fractions
 
     gcd = fractions.gcd(p, q)
     p /= gcd
     q /= gcd
 
     m = np.maximum(p, q)
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/parameters.py` & `pyroomacoustics-0.7.4/pyroomacoustics/parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,53 +35,82 @@
 
 import numpy as np
 
 # tolerance for computations
 eps = 1e-10
 
 
+def get_num_threads():
+    """
+    Returns the number of threads available for pyroomacoustics
+
+    The number of threads can be set by
+    1. Setting the ``PRA_NUM_THREADS`` environment variable
+    2. Calling ``pra.constants.set("num_threads") = new_num_threads
+    3. Seting ``OMP_NUM_THREADS`` or ``MKL_NUM_THREADS``
+    """
+
+    num_cores = os.cpu_count()
+
+    # the specific environment variable takes prescedence
+    if "PRA_NUM_THREADS" in os.environ:
+        return int(os.environ["PRA_NUM_THREADS"])
+
+    # we also respect OMP and MKL variables
+    env_var = [
+        "OMP_NUM_THREADS",
+        "MKL_NUM_THREADS",
+    ]
+
+    all_limits = [int(getattr(os.environ, var, num_cores)) for var in env_var]
+
+    return min(all_limits)
+
+
 # We implement the constants as a dictionary so that they can
 # be modified at runtime.
 # The class Constants gives an interface to update the value of
 # constants or add new ones.
 _constants = {}
 _constants_default = {
     "c": 343.0,  # speed of sound at 20 C in dry air
     "ffdist": 10.0,  # distance to the far field
     "fc_hp": 300.0,  # cut-off frequency of standard high-pass filter
     "frac_delay_length": 81,  # Length of the fractional delay filters used for RIR gen
     "room_isinside_max_iter": 20,  # Max iterations for checking if point is inside room
+    "sinc_lut_granularity": 20,  # num. points in integer interval in the sinc interp. LUT
+    "num_threads": get_num_threads(),  # num. of threads to use
 }
 
 
 class Constants:
     """
     A class to provide easy access package wide to user settable constants.
     """
 
     def set(self, name, val):
         # add constant to dictionnary
         _constants[name] = val
 
     def get(self, name):
-
         try:
             v = _constants[name]
         except KeyError:
             try:
                 v = _constants_default[name]
             except KeyError:
                 raise NameError(name + ": no such constant")
 
         return v
 
 
 # the instanciation of the class
 constants = Constants()
 
+
 # Compute the speed of sound as a function
 # of temperature, humidity, and pressure
 def calculate_speed_of_sound(t, h, p):
     """
     Compute the speed of sound as a function of
     temperature, humidity and pressure
 
@@ -147,15 +176,14 @@
     temperature: float, optional
         The room temperature
     humidity: float in range (0, 100), optional
         The room relative humidity in %. Default is 0.
     """
 
     def __init__(self, temperature=None, humidity=None):
-
         self.p = 100.0  # pressure in kilo-Pascal (kPa), not used
         if humidity is None:
             self.H = 0.0
         else:
             self.H = humidity
 
         if self.H < 0.0 or self.H > 100:
@@ -285,15 +313,14 @@
             (i.e. flat).
         * str: The scattering values will be obtained from the database.
         * dict: A dictionary containing keys ``description``, ``coeffs``, and
             ``center_freqs``.
     """
 
     def __init__(self, energy_absorption, scattering=None):
-
         # Handle the energy absorption input based on its type
         if isinstance(energy_absorption, (float, np.float32, np.float64)):
             # This material is flat over frequencies
             energy_absorption = {"coeffs": [energy_absorption]}
 
         elif isinstance(energy_absorption, str):
             # Get the coefficients from the database
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/phase/__init__.py` & `pyroomacoustics-0.7.4/pyroomacoustics/phase/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/phase/gl.py` & `pyroomacoustics-0.7.4/pyroomacoustics/phase/gl.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,33 +164,28 @@
     # Initialize the signal
     Y = X * ini
     y = engine.synthesis(Y)
 
     # the successive application of analysis/synthesis introduces
     # a shift of ``fft_size - hop`` that we must correct
     the_shift = fft_size - hop
-    y[:-the_shift,] = y[
-        the_shift:,
-    ]
+    y[:-the_shift,] = y[the_shift:,]
 
     for epoch in range(n_iter):
-
         # possibly monitor the reconstruction
         if callback is not None:
             callback(epoch, Y, y)
 
         # back to STFT domain
         Y[:, :] = engine.analysis(y)
 
         # enforce magnitudes
         Y *= X / np.abs(Y)
 
         # back to time domain
-        y[:-the_shift,] = engine.synthesis(Y)[
-            the_shift:,
-        ]
+        y[:-the_shift,] = engine.synthesis(Y)[the_shift:,]
 
     # last callback
     if callback is not None:
         callback(epoch, Y, y)
 
     return y
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/recognition.py` & `pyroomacoustics-0.7.4/pyroomacoustics/recognition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import division, print_function
 
-import numpy as np
 import os
-from scipy.stats import multivariate_normal
-import sys
 import struct
+import sys
+
+import numpy as np
+from scipy.stats import multivariate_normal
 
 try:
     import sounddevice as sd
 
     have_sounddevice = True
 except:
     have_sounddevice = False
@@ -20,15 +21,14 @@
     def __init__(self, nstates, odim=1, examples=None):
         """Initialize the Gaussian emission object"""
 
         # The emissions parameters
         self.K = nstates
 
         if examples is None:
-
             # Initialize to random components
             self.O = odim
             self.mu = np.random.normal(size=(self.K, self.O))
             self.Sigma = np.ones((self.K, self.O)) * 10
 
         else:
             # Initialize all components to the same mean and variance of the data
@@ -37,15 +37,14 @@
             X = np.concatenate(examples, axis=0)
 
             self.mu = np.array([np.mean(X, axis=0)] * self.K)
             centered = X - self.mu[0]
             self.Sigma = np.array([np.mean(centered**2, axis=0)] * self.K)
 
     def update_parameters(self, examples, gamma):
-
         g = np.concatenate(gamma, axis=0)
         X = np.concatenate(examples, axis=0)
         Z = g.sum(axis=0)
 
         for k in range(self.K):
             self.mu[k] = np.sum(X.T * g[:, k], axis=1) / Z[k]
             centered = (X - self.mu[k]) ** 2
@@ -99,15 +98,14 @@
             X = np.concatenate(examples, axis=0)
 
             self.mu = np.array([np.mean(X, axis=0)] * self.K)
             centered = X - self.mu[0]
             self.Sigma = np.array([np.diag(np.mean(centered**2, axis=0))] * self.K)
 
     def update_parameters(self, examples, gamma):
-
         g = np.concatenate(gamma, axis=0)
         X = np.concatenate(examples, axis=0)
         Z = g.sum(axis=0)
 
         for k in range(self.K):
             self.mu[k] = np.sum(X.T * g[:, k], axis=1) / Z[k]
             centered = X - self.mu[k]
@@ -226,29 +224,27 @@
             row[:] /= row.sum()
         self.pi[:] /= self.pi.sum()
 
         # Run the EM algorithm
         loglikelihood_old = -np.inf  # log-likelihood
         n_iter = 0
         while True:
-
             # Initialize new parameters value for accumulation
             loglikelihood = 0.0
 
             # We need to run the forward/backward algorithm for each example and
             # and combine the result to form the new estimates
             gamma = []
             xhi = []
             p_x_given_z = self.emission.prob_x_given_state(examples)
 
             # Expectation-step
             # -----------------
 
             for X, pxz in zip(examples, p_x_given_z):
-
                 # check dimension of emission
                 if X.shape[1] != self.emission.O:
                     raise ValueError(
                         "Error: Emission vectors of all examples should have the same size"
                     )
 
                 # First compute alpha and beta using forward/backward algo
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/room.py` & `pyroomacoustics-0.7.4/pyroomacoustics/room.py`

 * *Files 2% similar despite different names*

```diff
@@ -478,14 +478,44 @@
     For shoebox rooms, the walls are labelled as follows:
 
     - ``west``/``east`` for the walls in the y-z plane with a small/large x coordinates, respectively
     - ``south``/``north`` for the walls in the x-z plane with a small/large y coordinates, respectively
     - ``floor``/``ceiling`` for the walls int x-y plane with small/large z coordinates, respectively
 
 
+Air Absorption
+--------------
+
+The absorption of sound energy by air is frequency dependent.
+The absorption is described the frequency dependent coefficient :math:`\\alpha(f)` and the energy decreases with distance as :math:`e^{-\\alpha(f) d}`.
+This can be turned simply by providing the keyword argument ``air_absorption=True`` to the room constructor or calling ``set_absorption()`` on an existing room.
+The coefficients are also temperature and humidity dependent and the default values are as follows.
+
+========= ========    ====== ====== ====== ===== ===== ===== ===== =====
+Temp. (C) Hum. (%)    125 Hz 250 Hz 500 Hz 1 kHz 2 kHz 4 kHz 8 kHz 
+========= ========    ====== ====== ====== ===== ===== ===== ===== =====
+10        30-50       0.1    0.2    0.5    1.1   2.7   9.4   29.0  x1e-3
+10        50-70       0.1    0.2    0.5    0.8   1.8   5.9   21.1  x1e-3
+10        70-90       0.1    0.2    0.5    0.7   1.4   4.4   15.8  x1e-3
+20        30-50       0.1    0.3    0.6    1.0   1.9   5.8   20.3  x1e-3
+20        50-70       0.1    0.3    0.6    1.0   1.7   4.1   13.5  x1e-3
+20        70-90       0.1    0.3    0.6    1.1   1.7   3.5   10.6  x1e-3
+========= ========    ====== ====== ====== ===== ===== ===== ===== =====
+
+It is possible to set custom coefficients by providing a lists of coefficients and corresponding frequencies.
+If the frequencies are not provided, the default values of 125 Hz to 8 kHz octave bands are assumed.
+Note, that the number of octave bands will depend on the sampling frequency used.
+For 16 kHz, there will be 7 octave bands.
+If less than 7 coefficients are provided, or if the center frequencies do not correspond, a simple interpolation is used to fill the missing values.
+Missing values at end of the array are simply replicated from the last value.
+
+.. code-block:: python
+
+    room.set_air_absorption([0.1, 0.2, 0.4, 1.3, 2.8, 9.4, 23.0])
+
 Controlling the signal-to-noise ratio
 -------------------------------------
 
 It is in general necessary to scale the signals from different sources to
 obtain a specific signal-to-noise or signal-to-interference ratio (SNR and SIR,
 respectively). This can be done by passing some options to the :py:func:`simulate()`
 function. Because the relative amplitude of signals will change at different microphones
@@ -651,29 +681,38 @@
 
 """
 
 
 from __future__ import division, print_function
 
 import math
+import os
+import sys
 import warnings
 
 import numpy as np
 import scipy.spatial as spatial
 from scipy.interpolate import interp1d
 
 from . import beamforming as bf
 from . import libroom
 from .acoustics import OctaveBandsFactory, rt60_eyring, rt60_sabine
 from .beamforming import MicrophoneArray
 from .directivities import CardioidFamily, source_angle_shoebox
 from .doa import GridCircle, GridSphere
 from .experimental import measure_rt60
 from .libroom import Wall, Wall2D
-from .parameters import Material, Physics, constants, eps, make_materials
+from .parameters import (
+    Material,
+    Physics,
+    constants,
+    eps,
+    get_num_threads,
+    make_materials,
+)
 from .soundsource import SoundSource
 from .utilities import angle_function, fractional_delay
 
 
 def wall_factory(corners, absorption, scattering, name=""):
     """Call the correct method according to wall dimension"""
     if corners.shape[0] == 3:
@@ -681,24 +720,22 @@
     elif corners.shape[0] == 2:
         return Wall2D(corners, absorption, scattering, name)
     else:
         raise ValueError("Rooms can only be 2D or 3D")
 
 
 def sequence_generation(volume, duration, c, fs, max_rate=10000):
-
     # repeated constant
     fpcv = 4 * np.pi * c**3 / volume
 
     # initial time
     t0 = ((2 * np.log(2)) / fpcv) ** (1.0 / 3.0)
     times = [t0]
 
     while times[-1] < t0 + duration:
-
         # uniform random variable
         z = np.random.rand()
         # rate of the point process at this time
         mu = np.minimum(fpcv * (t0 + times[-1]) ** 2, max_rate)
         # time interval to next point
         dt = np.log(1 / z) / mu
 
@@ -846,15 +883,14 @@
         temperature=None,
         humidity=None,
         air_absorption=False,
         ray_tracing=False,
         use_rand_ism=False,
         max_rand_disp=0.08,
     ):
-
         self.walls = walls
 
         # Get the room dimension from that of the walls
         self.dim = walls[0].dim
 
         # Create a mapping with friendly names for walls
         self._wall_mapping()
@@ -897,15 +933,14 @@
         temperature,
         humidity,
         air_absorption,
         ray_tracing,
         use_rand_ism,
         max_rand_disp,
     ):
-
         self.fs = fs
 
         if t0 != 0.0:
             raise NotImplementedError(
                 "Global simulation delay not " "implemented (aka t0)"
             )
         self.t0 = t0
@@ -948,15 +983,14 @@
         # in the beginning, nothing has been
         self.visibility = None
 
         # initialize the attribute for the impulse responses
         self.rir = None
 
     def _init_room_engine(self, *args):
-
         args = list(args)
 
         if len(args) == 0:
             # This is a polygonal room
             # find the non convex walls
             obstructing_walls = find_non_convex_walls(self.walls)
             args += [self.walls, obstructing_walls]
@@ -979,15 +1013,14 @@
         # Create the real room object
         if self.dim == 2:
             self.room_engine = libroom.Room2D(*args)
         else:
             self.room_engine = libroom.Room(*args)
 
     def _update_room_engine_params(self):
-
         # Now, if it exists, set the parameters of room engine
         if self.room_engine is not None:
             self.room_engine.set_params(
                 self.c,  # speed of sound
                 self.max_order,
                 self.rt_args["energy_thres"],
                 self.rt_args["time_thres"],
@@ -1121,42 +1154,58 @@
         self._update_room_engine_params()
 
     def unset_ray_tracing(self):
         """Deactivates the ray tracer"""
         self.simulator_state["rt_needed"] = False
         self._update_room_engine_params()
 
-    def set_air_absorption(self, coefficients=None):
+    def set_air_absorption(
+        self, coefficients=None, center_freqs=None, interp_kind="linear"
+    ):
         """
         Activates or deactivates air absorption in the simulation.
 
         Parameters
         ----------
-        coefficients: list of float
-            List of air absorption coefficients, one per octave band
+        coefficients: list of float, optional
+            Optional list of air absorption coefficients, one per octave band.
+            If not provided, values corresponding to the temperature and humidity
+            of the room are used.
+        center_freqs: list, optional
+            The optional list of center frequencies for the octave bands.
+            If not provided, the values of the default ocatave bands are used.
+        interp_kind: str
+            Specifies the kind of interpolation as a string (‘linear’,
+            ‘nearest’, ‘zero’, ‘slinear’, ‘quadratic’, ‘cubic’, ‘previous’,
+            ‘next’, where ‘zero’, ‘slinear’, ‘quadratic’ and ‘cubic’ refer to a
+            spline interpolation of zeroth, first, second or third order;
+            ‘previous’ and ‘next’ simply return the previous or next value of
+            the point) or as an integer specifying the order of the spline
+            interpolator to use. Default is ‘linear’.
         """
 
         self.simulator_state["air_abs_needed"] = True
         if coefficients is None:
             self.air_absorption = self.octave_bands(**self.physics.get_air_absorption())
         else:
             # ignore temperature and humidity if coefficients are provided
-            self.air_absorption = self.physics().get_air_absorption()
+            self.air_absorption = self.octave_bands(
+                coeffs=coefficients, center_freqs=center_freqs, interp_kind=interp_kind
+            )
 
     def unset_air_absorption(self):
         """Deactivates air absorption in the simulation"""
         self.simulator_state["air_abs_needed"] = False
 
     def set_sound_speed(self, c):
         """Sets the speed of sound unconditionnaly"""
         self.c = c
         self._update_room_engine_params()
 
     def _wall_mapping(self):
-
         # mapping between wall names and indices
         self.wallsId = {}
         for i in range(len(self.walls)):
             if self.walls[i].name is not None:
                 self.wallsId[self.walls[i].name] = i
 
     @classmethod
@@ -1238,15 +1287,14 @@
             )
 
         ############################
         # BEGIN COMPATIBILITY CODE #
         ############################
 
         if materials is not None:
-
             if absorption_compatibility_request:
                 import warnings
 
                 warnings.warn(
                     "Because materials were specified, deprecated absorption parameter is ignored.",
                     DeprecationWarning,
                 )
@@ -1390,15 +1438,14 @@
         else:
             absorption_compatibility_request = False
         ##########################
         # END COMPATIBILITY CODE #
         ##########################
 
         if materials is not None:
-
             if absorption_compatibility_request:
                 import warnings
 
                 warnings.warn(
                     "Because materials were specified, "
                     "deprecated absorption parameter is ignored.",
                     DeprecationWarning,
@@ -1409,15 +1456,14 @@
 
             for mat in materials.values():
                 assert isinstance(
                     mat, Material
                 ), "Material not specified using correct class"
 
         elif absorption_compatibility_request:
-
             import warnings
 
             warnings.warn(
                 "absorption parameter is deprecated for Room.extrude",
                 DeprecationWarning,
             )
 
@@ -1510,15 +1556,14 @@
                 cmap=matplotlib.cm.jet,
                 facecolor=np.array([1, 1, 1]),
                 edgecolor=np.array([0, 0, 0]),
             )
             ax.add_collection(p)
 
             if self.mic_array is not None:
-
                 for i in range(self.mic_array.nmic):
                     ax.scatter(
                         self.mic_array.R[0][i],
                         self.mic_array.R[1][i],
                         marker="x",
                         linewidth=0.5,
                         s=mic_marker_size,
@@ -1541,15 +1586,14 @@
                     freq is not None
                     and isinstance(self.mic_array, bf.Beamformer)
                     and (
                         self.mic_array.weights is not None
                         or self.mic_array.filters is not None
                     )
                 ):
-
                     freq = np.array(freq)
                     if freq.ndim == 0:
                         freq = np.array([freq])
 
                     # define a new set of colors for the beam patterns
                     newmap = plt.get_cmap("autumn")
                     desat = 0.7
@@ -1643,15 +1687,14 @@
                 bbox = self.get_bbox()
                 ax.set_xlim(bbox[0, :])
                 ax.set_ylim(bbox[1, :])
 
             return fig, ax
 
         if self.dim == 3:
-
             import matplotlib.colors as colors
             import matplotlib.pyplot as plt
             import mpl_toolkits.mplot3d as a3
 
             if ax is None:
                 fig = plt.figure(figsize=figsize)
                 ax = a3.Axes3D(fig, auto_add_to_figure=False)
@@ -1725,15 +1768,14 @@
                 bbox = self.get_bbox()
                 ax.set_xlim3d(bbox[0, :])
                 ax.set_ylim3d(bbox[1, :])
                 ax.set_zlim3d(bbox[2, :])
 
             # draw the microphones
             if self.mic_array is not None:
-
                 for i in range(self.mic_array.nmic):
                     ax.scatter(
                         self.mic_array.R[0][i],
                         self.mic_array.R[1][i],
                         self.mic_array.R[2][i],
                         marker="x",
                         linewidth=0.5,
@@ -1925,15 +1967,14 @@
         Returns
         -------
         :py:obj:`~pyroomacoustics.room.Room`
             The room is returned for further tweaking.
         """
 
         if isinstance(obj, SoundSource):
-
             if obj.dim != self.dim:
                 raise ValueError(
                     (
                         "The Room and SoundSource objects must be of the same "
                         "dimensionality. The Room is {}D but the SoundSource "
                         "is {}D"
                     ).format(self.dim, obj.dim)
@@ -1941,15 +1982,14 @@
 
             if not self.is_inside(np.array(obj.position)):
                 raise ValueError("The source must be added inside the room.")
 
             self.sources.append(obj)
 
         elif isinstance(obj, MicrophoneArray):
-
             if obj.dim != self.dim:
                 raise ValueError(
                     (
                         "The Room and MicrophoneArray objects must be of the same "
                         "dimensionality. The Room is {}D but the MicrophoneArray "
                         "is {}D"
                     ).format(self.dim, obj.dim)
@@ -2099,60 +2139,57 @@
             The SoundSource object to add to the room
         """
         if directivity is not None:
             sndsrc.set_directivity(directivity)
         return self.add(sndsrc)
 
     def image_source_model(self):
-
         if not self.simulator_state["ism_needed"]:
             return
 
         self.visibility = []
 
         for source in self.sources:
-
             n_sources = self.room_engine.image_source_model(source.position)
 
             if n_sources > 0:
-
                 # Copy to python managed memory
                 source.images = self.room_engine.sources.copy()
                 source.orders = self.room_engine.orders.copy()
                 source.orders_xyz = self.room_engine.orders_xyz.copy()
                 source.walls = self.room_engine.gen_walls.copy()
                 source.damping = self.room_engine.attenuations.copy()
                 source.generators = -np.ones(source.walls.shape)
 
                 # if randomized image method is selected, add a small random
                 # displacement to the image sources
                 if self.simulator_state["random_ism_needed"]:
-
                     n_images = np.shape(source.images)[1]
 
                     # maximum allowed displacement is 8cm
                     max_disp = self.max_rand_disp
 
                     # add a random displacement to each cartesian coordinate
-                    disp = np.random.uniform(-max_disp, max_disp, size=(3, n_images))
+                    disp = np.random.uniform(
+                        -max_disp, max_disp, size=(self.dim, n_images)
+                    )
                     source.images += disp
 
                 self.visibility.append(self.room_engine.visible_mics.copy())
 
                 # We need to check that microphones are indeed in the room
                 for m in range(self.mic_array.R.shape[1]):
                     # if not, it's not visible from anywhere!
                     if not self.is_inside(self.mic_array.R[:, m]):
                         self.visibility[-1][m, :] = 0
 
         # Update the state
         self.simulator_state["ism_done"] = True
 
     def ray_tracing(self):
-
         if not self.simulator_state["rt_needed"]:
             return
 
         # this will be a list of lists with
         # shape (n_mics, n_src, n_directions, n_bands, n_time_bins)
         self.rt_histograms = [[] for r in range(self.mic_array.M)]
 
@@ -2184,29 +2221,27 @@
         self.rir = []
 
         volume_room = self.get_volume()
 
         for m, mic in enumerate(self.mic_array.R.T):
             self.rir.append([])
             for s, src in enumerate(self.sources):
-
                 """
                 Compute the room impulse response between the source
                 and the microphone whose position is given as an
                 argument.
                 """
                 # fractional delay length
                 fdl = constants.get("frac_delay_length")
                 fdl2 = fdl // 2
 
                 # default, just in case both ism and rt are disabled (should never happen)
                 N = fdl
 
                 if self.simulator_state["ism_needed"]:
-
                     # compute azimuth and colatitude angles for receiver
                     if self.mic_array.directivity is not None:
                         angle_function_array = angle_function(src.images, mic)
                         azimuth = angle_function_array[0]
                         colatitude = angle_function_array[1]
 
                     # compute azimuth and colatitude angles for source
@@ -2223,15 +2258,14 @@
                     t_max = time.max()
                     N = int(math.ceil(t_max * self.fs))
 
                 else:
                     t_max = 0.0
 
                 if self.simulator_state["rt_needed"]:
-
                     # get the maximum length from the histograms
                     nz_bins_loc = np.nonzero(self.rt_histograms[m][s][0].sum(axis=0))[0]
                     if len(nz_bins_loc) == 0:
                         n_bins = 0
                     else:
                         n_bins = nz_bins_loc[-1] + 1
 
@@ -2255,24 +2289,21 @@
 
                 # Do band-wise RIR construction
                 is_multi_band = self.is_multi_band
                 bws = self.octave_bands.get_bw() if is_multi_band else [self.fs / 2]
                 rir_bands = []
 
                 for b, bw in enumerate(bws):
-
-                    ir_loc = np.zeros_like(ir)
+                    ir_loc = np.zeros_like(ir, dtype=np.float32)
 
                     # IS method
                     if self.simulator_state["ism_needed"]:
-
                         alpha = src.damping[b, :] / dist
 
                         if self.mic_array.directivity is not None:
-
                             alpha *= self.mic_array.directivity[m].get_response(
                                 azimuth=azimuth,
                                 colatitude=colatitude,
                                 frequency=bw,
                                 degrees=False,
                             )
 
@@ -2281,32 +2312,40 @@
                                 azimuth=azimuth_s,
                                 colatitude=colatitude_s,
                                 frequency=bw,
                                 degrees=False,
                             )
 
                         # Use the Cython extension for the fractional delays
-                        from .build_rir import fast_rir_builder
+                        # from .build_rir import fast_rir_builder
 
                         vis = self.visibility[s][m, :].astype(np.int32)
                         # we add the delay due to the factional delay filter to
                         # the arrival times to avoid problems when propagation
                         # is shorter than the delay to to the filter
                         # hence: time + fdl2
                         time_adjust = time + fdl2 / self.fs
-                        fast_rir_builder(ir_loc, time_adjust, alpha, vis, self.fs, fdl)
+                        libroom.rir_builder(
+                            ir_loc,
+                            time_adjust.astype(np.float32),
+                            alpha.astype(np.float32),
+                            vis,
+                            self.fs,
+                            fdl,
+                            constants.get("sinc_lut_granularity"),
+                            constants.get("num_threads"),
+                        )
 
                         if is_multi_band:
                             ir_loc = self.octave_bands.analysis(ir_loc, band=b)
 
                         ir += ir_loc
 
                     # Ray Tracing
                     if self.simulator_state["rt_needed"]:
-
                         if is_multi_band:
                             seq_bp = self.octave_bands.analysis(seq, band=b)
                         else:
                             seq_bp = seq.copy()
 
                         # interpolate the histogram and multiply the sequence
                         seq_bp_rot = seq_bp.reshape((-1, hbss))
@@ -2326,15 +2365,14 @@
                         ir_loc[fdl2 : fdl2 + N] += seq_bp
 
                     # keep for further processing
                     rir_bands.append(ir_loc)
 
                 # Do Air absorption
                 if self.simulator_state["air_abs_needed"]:
-
                     # In case this was not multi-band, do the band pass filtering
                     if len(rir_bands) == 1:
                         rir_bands = self.octave_bands.analysis(rir_bands[0]).T
 
                     # Now apply air absorption
                     for band, air_abs in zip(rir_bands, self.air_absorption):
                         air_decay = np.exp(-0.5 * air_abs * distance_rir)
@@ -2559,15 +2597,14 @@
         bbox = self.get_bbox()
         bbox_center = np.mean(bbox, axis=1)
         bbox_max_dist = np.linalg.norm(bbox[:, 1] - bbox[:, 0]) / 2
 
         # re-run until we get a non-ambiguous result
         it = 0
         while it < constants.get("room_isinside_max_iter"):
-
             # Get random point outside the bounding box
             random_vec = np.random.randn(self.dim)
             random_vec /= np.linalg.norm(random_vec)
             p0 = bbox_center + 2 * bbox_max_dist * random_vec
 
             ambiguous = False  # be optimistic
             is_on_border = False  # we have to know if the point is on the boundary
@@ -2615,15 +2652,14 @@
             """
                 Error could not determine if point is in or out in maximum number of iterations.
                 This is most likely a bug, please report it.
                 """
         )
 
     def wall_area(self, wall):
-
         """Computes the area of a 3D planar wall.
 
         Parameters
         ----------
         wall: Wall instance
             the wall object that is defined in 3D space
 
@@ -2697,15 +2733,14 @@
             bandwidths = [1.0]
 
         V = self.volume
         S = np.sum([w.area() for w in self.walls])
         c = self.c
 
         for i, bw in enumerate(bandwidths):
-
             # average absorption coefficients
             a = 0.0
             for w in self.walls:
                 if len(w.absorption) == 1:
                     a += w.area() * w.absorption[0]
                 else:
                     a += w.area() * w.absorption[i]
@@ -2827,15 +2862,14 @@
         temperature=None,
         humidity=None,
         air_absorption=False,
         ray_tracing=False,
         use_rand_ism=False,
         max_rand_disp=0.08,
     ):
-
         p = np.array(p, dtype=np.float32)
 
         if len(p.shape) > 1 and (len(p) != 2 or len(p) != 3):
             raise ValueError("`p` must be a vector of length 2 or 3.")
 
         self.dim = p.shape[0]
 
@@ -2880,15 +2914,14 @@
             absorption = dict(zip(self.wall_names, [absorption] * n_walls))
 
         ##########################
         # END COMPATIBILITY CODE #
         ##########################
 
         if materials is not None:
-
             if absorption_compatibility_request:
                 warnings.warn(
                     "Because `materials` were specified, deprecated "
                     "`absorption` parameter is ignored.",
                     DeprecationWarning,
                 )
 
@@ -2904,15 +2937,14 @@
 
             for w_name in self.wall_names:
                 assert isinstance(
                     materials[w_name], Material
                 ), "Material not specified using correct class"
 
         elif absorption_compatibility_request:
-
             warnings.warn(
                 "Using absorption parameter is deprecated. Use `materials` with "
                 "`Material` object instead.",
                 DeprecationWarning,
             )
 
             # order the wall absorptions
@@ -2934,15 +2966,14 @@
                     materials[w_name] = Material(energy_absorption=correct_abs)
                 else:
                     raise KeyError(
                         "Absorption needs to have keys 'east', 'west', "
                         "'north', 'south', 'ceiling' (3d), 'floor' (3d)."
                     )
         else:
-
             # In this case, no material is provided, use totally reflective
             # walls, no scattering
             materials = dict(
                 zip(self.wall_names, [Material(energy_absorption=0.0)] * n_walls)
             )
 
         # If some of the materials used are multi-band, we need to resample
@@ -3093,15 +3124,14 @@
             temperature=temperature,
             humidity=humidity,
             air_absorption=air_absorption,
             ray_tracing=ray_tracing,
         )
 
     def __str__(self):
-
         return "AnechoicRoom instance in {}D.".format(self.dim)
 
     def is_inside(self, p):
         """Overloaded function to eliminate testing if objects are inside "room"."""
         # always return True because we want the walls to have no effect.
         return True
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/soundsource.py` & `pyroomacoustics-0.7.4/pyroomacoustics/soundsource.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # @version: 1.0  date: 05/06/2015 by Sidney Barthe
 # @author: robin.scheibler@epfl.ch, ivan.dokmanic@epfl.ch, sidney.barthe@epfl.ch
 # @copyright: EPFL-IC-LCAV 2015
 from __future__ import division, print_function
 
 import numpy as np
-from .parameters import constants
+
 from .directivities import Directivity
+from .parameters import constants
 
 
 class SoundSource(object):
     """
     A class to represent sound sources.
 
     This object represents a sound source in a room by a list containing the original source position
@@ -27,15 +28,14 @@
         generators=None,  # parent source
         walls=None,  # generating wall
         orders=None,
         signal=None,
         delay=0,
         directivity=None,
     ):
-
         position = np.array(position)
         self.dim = position.shape[0]
 
         # Check the shape of the passed array
         if self.dim != 2 and self.dim != 3:
             dim_mismatch = True
         else:
@@ -115,15 +115,14 @@
         ----------
         signal: ndarray
             a N-length ndarray, representing a sequence of samples generated by the source.
         """
         self.signal = signal
 
     def distance(self, ref_point):
-
         return np.sqrt(np.sum((self.images - ref_point[:, np.newaxis]) ** 2, axis=0))
 
     def set_ordering(self, ordering, ref_point=None):
         """
         Set the order in which we retrieve images sources.
         Can be: 'nearest', 'strongest', 'order'
         Optional argument: ref_point
@@ -131,30 +130,27 @@
 
         self.ordering = ordering
 
         if ref_point is not None and ref_point.ndim > 1:
             ref_point = ref_point[:, 0]
 
         if ordering == "nearest":
-
             if ref_point is None:
                 raise NameError("For nearest ordering, a reference point is needed.")
 
             self.I = self.distance(ref_point).argsort()
 
         elif ordering == "strongest":
-
             if ref_point is None:
                 raise NameError("For strongest ordering, a reference point is needed.")
 
             strength = np.linalg.norm(self.damping, 0) / (self.distance(ref_point))
             self.I = strength.argsort()
 
         elif ordering == "order":
-
             self.ordering = "order"
 
         else:
             raise NameError("Ordering can be nearest, strongest, order.")
 
     def __getitem__(self, index):
         """Overload the bracket operator to access a subset image sources"""
@@ -233,79 +229,14 @@
 
     def get_damping(self, max_order=None):
         if max_order is None:
             max_order = len(np.max(self.orders))
 
         return self.damping[:, self.orders <= max_order]
 
-    def get_rir(self, mic, visibility, Fs, t0=0.0, t_max=None):
-        """
-        Compute the room impulse response between the source
-        and the microphone whose position is given as an
-        argument.
-
-        Parameters
-        ----------
-        mic: ndarray
-            microphone position
-        visibility: int32
-            1 if mic visibile from source, 0 else. Exact type is important for C extension
-        Fs: int
-            sampling frequency
-        t0: float
-            time offset, defaults to 0
-        t_max: None
-            max time, defaults to 1.05 times the propagation time from mic to source
-        """
-
-        # fractional delay length
-        fdl = constants.get("frac_delay_length")
-        fdl2 = (fdl - 1) // 2
-
-        # compute the distance
-        dist = self.distance(mic)
-        time = dist / constants.get("c") + t0
-        if self.damping.shape[0] == 1:
-            alpha = self.damping[0, :] / (4.0 * np.pi * dist)
-        else:
-            raise NotImplementedError("Not implemented for multiple frequency bands")
-
-        # the number of samples needed
-        if t_max is None:
-            # we give a little bit of time to the sinc to decay anyway
-            N = np.ceil((1.05 * time.max() - t0) * Fs)
-        else:
-            N = np.ceil((t_max - t0) * Fs)
-
-        N += fdl
-
-        t = np.arange(N) / float(Fs)
-        ir = np.zeros(t.shape)
-
-        try:
-            # Try to use the Cython extension
-            from .build_rir import fast_rir_builder
-
-            fast_rir_builder(ir, time, alpha, visibility.astype(np.int32), Fs, fdl)
-
-        except ImportError:
-            print("Cython-extension build_rir unavailable. Falling back to pure python")
-            # fallback to pure Python implemenation
-            from .utilities import fractional_delay
-
-            for i in range(time.shape[0]):
-                if visibility[i] == 1:
-                    time_ip = int(np.round(Fs * time[i]))
-                    time_fp = (Fs * time[i]) - time_ip
-                    ir[time_ip - fdl2 : time_ip + fdl2 + 1] += alpha[
-                        i
-                    ] * fractional_delay(time_fp)
-
-        return ir
-
     def wall_sequence(self, i):
         """
         Print the wall sequence for the image source indexed by i
         """
         p = self.generators[i]
         if np.isnan(p):
             return []
@@ -349,15 +280,15 @@
 
     where H_{ij} is channel matrix between microphone i and source j.
     H is of type (M*Lg)x((Lg+Lh-1)*S) where Lh is the channel length (determined by epsilon),
     and M, S are the number of microphones, sources, respectively.
     """
 
     from .beamforming import distance
-    from .utilities import low_pass_dirac, convmtx
+    from .utilities import convmtx, low_pass_dirac
 
     for s in sources:
         if s.damping.shape[0] > 1:
             raise NotImplementedError("Multiple frequency bands not supported yet")
 
     # set the boundaries of RIR filter for given epsilon
     d_min = np.inf
@@ -385,15 +316,14 @@
 
     # build the channel matrix
     L = Lg + Lh - 1
     H = np.zeros((Lg * mics.shape[1], len(sources) * L))
 
     for s in range(len(sources)):
         for r in np.arange(mics.shape[1]):
-
             dist = sources[s].distance(mics[:, r])
             time = dist / constants.get("c") - t_min + offset
             if unit_damping == True:
                 dmp = 1.0 / (4 * np.pi * dist)
             else:
                 dmp = sources[s].damping[0, :] / (4 * np.pi * dist)
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/sync.py` & `pyroomacoustics-0.7.4/pyroomacoustics/sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 def time_align(ref, deg, L=4096):
     """
     return a copy of deg time-aligned and of same-length as ref.
     L is the block length used for correlations.
     """
 
     # estimate delay of signal
-    from numpy import zeros, minimum
+    from numpy import minimum, zeros
 
     delay = delay_estimation(ref, deg, L)
 
     # time-align with reference segment for error metric computation
     sig = zeros(ref.shape[0])
     if delay >= 0:
         length = minimum(deg.shape[0], ref.shape[0] - delay)
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_anechoic_room.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_anechoic_room.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import numpy as np
+
 import pyroomacoustics as pra
 
 
 def test_anechoic_room(debug=False):
-
     # sound signal
     fs = 40000
     freq = 440
     times = np.linspace(0, 1, 100)
     signal = np.sin(2 * np.pi * freq * times)
 
     for dim in [2, 3]:
-
         # create Anechoic room using the correct class
         room_infinite = pra.AnechoicRoom(fs=fs, dim=dim)
 
         # create same room using Shoebox
         room_shoebox = pra.ShoeBox([10] * dim, fs=fs, max_order=0)
 
         # Add a source somewhere in the room
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_autocorr.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_autocorr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+import time
+from unittest import TestCase
+
 import numpy as np
+
 from pyroomacoustics import autocorr
-from unittest import TestCase
-import time
 
 N = 256
 n_iter = 100
 x = np.random.randn(N)
 tol = 1e-12
 
 
 def consistent_results(p, biased=True):
-
     r_time = autocorr(x, p, method="time", biased=biased)
     r_fft = autocorr(x, p, method="fft", biased=biased)
     r_np = autocorr(x, p, method="numpy", biased=biased)
     r_pra = autocorr(x, p, method="pra", biased=biased)
 
     err_fft = np.linalg.norm(r_time - r_fft)
     err_np = np.linalg.norm(r_time - r_np)
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_bandpass_filterbank.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_bandpass_filterbank.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 This tests the construction of a bank of octave filters
 """
-import pyroomacoustics as pra
 
 import numpy as np
 from scipy.signal import sosfreqz
 
+import pyroomacoustics as pra
+
 tol = 1.0  # decibel
 
 
 def test_bandpass_filterbank():
     f0 = 125.0 / 2.0
     fs = 16000
 
@@ -35,15 +36,14 @@
 
     assert err <= tol, "Bandpass filterbank test fails (err {} > tol {})".format(
         err, tol
     )
 
 
 if __name__ == "__main__":
-
     import matplotlib.pyplot as plt
 
     f0 = 125.0 / 2.0
     fs = 16000
 
     bands, fc = pra.octave_bands(f0)
     filters = pra.bandpass_filterbank(bands, fs=fs, order=16)
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_create_noisy_signal.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_create_noisy_signal.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import division, print_function
+
+import os
 from unittest import TestCase
+
 import numpy as np
-import os
-from pyroomacoustics import create_noisy_signal, rms, normalize
 from scipy.io import wavfile
 
+from pyroomacoustics import create_noisy_signal, normalize, rms
+
 tol = 1e-5
 
 signal_fp = os.path.join(
     os.path.dirname(__file__),
     "..",
     "..",
     "examples",
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_issue_115.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_issue_115.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+
 import pyroomacoustics as pra
 
 
 def test_issue_115_ism_breaking():
     """
     When a source was too close to the microphone, the time-of-flight
     might be smaller than the delay due to the fractionnal delay filter
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_issue_162.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_issue_162.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+
 import pyroomacoustics as pra
 
 
 def compute_rir(order):
     fromPos = np.zeros((3))
     toPos = np.ones((3, 1))
     roomSize = np.array([3, 3, 3])
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_issue_22.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_issue_22.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 
 The test creates a random but fixed room and calls
 Room.image_source_model() 25000 times.
 
 If the C module is not installed (pure python
 fallback version), then nothing is done.
 """
+
 import numpy as np
+
 import pyroomacoustics
 
 
 def test_issue_22():
-
     np.random.seed(0)
 
     n_mics = 1
     n_src = 1
     n_times = 25000
     dim = 3
     mic_pos = np.random.rand(dim, n_mics)
@@ -44,17 +45,15 @@
     src_pos = np.random.rand(dim, n_src) * room_dim[:, None]
     for src in src_pos.T:
         shoebox.add_source(src)
 
     shoebox.add_microphone_array(pyroomacoustics.MicrophoneArray(mic_pos, fs))
 
     for i in range(n_times):
-
         shoebox.image_source_model()
 
         if i != 0 and i % 1000 == 0:
             print(i)
 
 
 if __name__ == "__main__":
-
     test_issue_22()
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_issue_236.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_issue_236.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import warnings
 
 import numpy
 import numpy as np
+
 import pyroomacoustics as pra
 
 warnings.filterwarnings(action="ignore", category=UserWarning)
 
 
 def random_room_ism(max_order=10, eps=1e-6, verbose=False):
     """
@@ -50,15 +51,14 @@
     if verbose:
         print("error", np.linalg.norm(trans_shoebox - trans_general))
 
     assert error < eps
 
 
 def test_ism_shoebox_vs_general(verbose=False):
-
     np.random.seed(0)
     n_repeat = 100
     max_order = 10
     eps = 5e-6
 
     for i in range(n_repeat):
         random_room_ism(max_order=max_order, eps=eps, verbose=verbose)
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_issue_69.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_issue_69.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import unittest
 
 import numpy as np
+
 import pyroomacoustics as pra
 
 room_dim = [15, 14, 16]
 absorption = 0.2
 e_abs = 1.0 - (1.0 - absorption) ** 2
 source_position = [2.0, 3.1, 2.0]
 mic_position = [2.0, 1.5, 2.0]
 fs = 16000
 max_order = 5
 
+
 # scenario A
 def get_room_constructor_args():
     """
     When provided with sources and microphones, the constructor
     should try to compute the RIR immediately
     """
     source = pra.SoundSource(position=source_position)
@@ -45,24 +47,22 @@
     shoebox.image_source_model()
     shoebox.compute_rir()
     return shoebox
 
 
 class RoomConstructorSources(unittest.TestCase):
     def test_room_constructor(self):
-
         room_1 = get_room_constructor_args()
         self.assertTrue(isinstance(room_1.sources[0], pra.SoundSource))
 
     def test_room_add_method(self):
         room_2 = get_room_add_method()
         self.assertTrue(isinstance(room_2.sources[0], pra.SoundSource))
 
     def test_rir_equal(self):
         room_1 = get_room_constructor_args()
         room_2 = get_room_add_method()
         self.assertTrue(np.allclose(room_1.rir[0][0], room_2.rir[0][0]))
 
 
 if __name__ == "__main__":
-
     unittest.main()
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_issue_87.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_issue_87.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import unittest
 
 import numpy as np
+
 import pyroomacoustics as pra
 
 
 def make_filters(n_mics):
     # Location of original source
     azimuth = 61.0 / 180.0 * np.pi  # 60 degrees
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_materials.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_materials.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Just run the Material command with a bunch of inputs to make sure
 it works as expected
 """
-import pyroomacoustics as pra
 
+import pyroomacoustics as pra
 
 scat_test = {
     "coeffs": [0.1, 0.1, 0.1, 0.2, 0.2, 0.2, 0.3],
     "center_freqs": [125, 250, 500, 1000, 2000, 4000, 8000],
 }
 abs_test = {
     "coeffs": [0.3, 0.4, 0.25, 0.11, 0.05, 0.03, 0.3],
@@ -108,15 +108,14 @@
 def test_empty():
     mat_list = pra.make_materials()
 
     assert mat_list == []
 
 
 if __name__ == "__main__":
-
     test_material_e_float()
     test_material_es_float()
     test_material_es_dict
     test_material_e_db()
     test_material_es_db()
     test_material_e_dict()
     test_material_es_dict()
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_metrics.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 from scipy.stats import norm as _norm
+
 import pyroomacoustics as pra
 
 
 def test_median():
-
     # simple tests
     x = np.arange(1, 11)
     m = pra.median(x)
     assert m == 5.5
 
     x = np.arange(1, 12)
     m = pra.median(x)
@@ -38,23 +38,21 @@
     from scipy.stats import uniform
 
     dist = uniform()
     true_median = dist.median()
 
     for n in N:
         for a in alpha:
-
             failures = np.zeros(R, dtype=bool)
 
             for r in range(R):
                 x = dist.rvs(size=n)
                 m, ci = pra.median(x, alpha=a)
 
                 if true_median < m + ci[0] or m + ci[1] < true_median:
                     failures[r] = 1
 
             assert sum(failures) / R <= 1.2 * a  # allow some slack for realizations
 
 
 if __name__ == "__main__":
-
     test_median()
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_rake_filters.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_rake_filters.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+
 import pyroomacoustics as pra
 
 room = pra.ShoeBox([4, 6], fs=16000, max_order=1)
 
 # add sources in the room
 room.add_source([2, 1.5])  # nice source
 room.add_source([2, 4.5])  # interferer
@@ -40,15 +41,14 @@
     bf.rake_perceptual_filters(
         room.sources[0][:4], interferer=room.sources[1][:4], R_n=Rn
     )
     pass
 
 
 if __name__ == "__main__":
-
     import matplotlib.pyplot as plt
 
     bf.rake_perceptual_filters(
         room.sources[0][:4], interferer=room.sources[1][:4], R_n=Rn, epsilon=0.1
     )
     bf.plot()
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_random_ism.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_random_ism.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Created on Tue Feb  8 17:50:45 2022
 
 @author: od0014
 
 Script to test removal of sweeping echoes with randomized image method
 """
+
 import pyroomacoustics as pra
 from pyroomacoustics import metrics as met
 
-
 # create an example with sweeping echo - from Enzo's paper
 room_size = [4, 4, 4]
 source_loc = [1, 2, 2]
 mic_loc = [0.5, 1, 0.75]
 fs = 44100
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_room_add.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_room_add.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import numpy as np
+
 import pyroomacoustics as pra
 
 sig = np.arange(10)
 room_size = [10, 9, 8]
 source_loc0 = [1.5, 1.7, 2.1]
 source_loc1 = [3.5, 7.7, 2.1]
 mic0 = [7, 8, 3.9]
 mic1 = [7.87, 3.6, 6.1]
 
 
 def test_add_source_mic():
-
     room = pra.ShoeBox(room_size).add_source(source_loc0).add_microphone(mic0)
 
     assert len(room.sources) == 1
     assert np.allclose(room.sources[0].position, source_loc0)
     assert len(room.mic_array) == 1
     assert room.mic_array.R.shape == (3, 1)
     assert np.allclose(room.mic_array.R[:, 0], mic0)
@@ -26,15 +26,14 @@
     assert len(room.mic_array) == 2
     assert np.allclose(room.mic_array.R[:, 0], mic0)
     assert np.allclose(room.mic_array.R[:, 1], mic1)
     assert room.mic_array.R.shape == (3, 2)
 
 
 def test_add_source_mic_obj():
-
     room = pra.ShoeBox(room_size)
 
     source0 = pra.SoundSource(source_loc0, signal=sig)
     source1 = pra.SoundSource(source_loc1, signal=sig)
 
     mic_array0 = pra.MicrophoneArray(np.c_[mic0], fs=room.fs)
     mic_array1 = pra.MicrophoneArray(np.c_[mic1], fs=room.fs)
@@ -54,15 +53,14 @@
     assert len(room.mic_array) == 2
     assert np.allclose(room.mic_array.R[:, 0], mic0)
     assert np.allclose(room.mic_array.R[:, 1], mic1)
     assert room.mic_array.R.shape == (3, 2)
 
 
 def test_add_source_mic_obj_2():
-
     room = pra.ShoeBox(room_size)
 
     source0 = pra.SoundSource(source_loc0, signal=sig)
     source1 = pra.SoundSource(source_loc1, signal=sig)
     mic_array = pra.MicrophoneArray(np.c_[mic0, mic1], fs=room.fs)
 
     room.add(source0).add(source1).add(mic_array)
@@ -73,15 +71,14 @@
     assert len(room.mic_array) == 2
     assert np.allclose(room.mic_array.R[:, 0], mic0)
     assert np.allclose(room.mic_array.R[:, 1], mic1)
     assert room.mic_array.R.shape == (3, 2)
 
 
 def test_add_source_mic_ndarray():
-
     source0 = pra.SoundSource(source_loc0, signal=sig)
     source1 = pra.SoundSource(source_loc1, signal=sig)
     mic_array = np.c_[mic0, mic1]
 
     room = (
         pra.ShoeBox(room_size).add(source0).add(source1).add_microphone_array(mic_array)
     )
@@ -92,15 +89,14 @@
     assert len(room.mic_array) == 2
     assert np.allclose(room.mic_array.R[:, 0], mic0)
     assert np.allclose(room.mic_array.R[:, 1], mic1)
     assert room.mic_array.R.shape == (3, 2)
 
 
 def test_add_source_mic_ndarray_2():
-
     source0 = pra.SoundSource(source_loc0, signal=sig)
     source1 = pra.SoundSource(source_loc1, signal=sig)
     mic_array = np.c_[mic0, mic1]
 
     room = pra.ShoeBox(room_size).add(source0).add(source1).add_microphone(mic_array)
 
     assert len(room.sources) == 2
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_room_is_insided.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_room_is_insided.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+
 import pyroomacoustics as pra
 
 
 def test_room_is_inside():
     # fix the seed for repeatable testing
     np.random.seed(0)
 
@@ -62,9 +63,8 @@
         assert not room.is_inside([1, 4, 3], include_borders=False)
 
         assert not room.is_inside([2, 2, 7])
         assert not room.is_inside([2, 2, -7])
 
 
 if __name__ == "__main__":
-
     test_room_is_inside()
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_room_mix.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_room_mix.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Tests the mixing function of ``Room.simulate``
 """
+
 import unittest
 
 import numpy as np
+
 import pyroomacoustics as pra
 
 e_abs = 1.0 - (1.0 - 0.25) ** 2
 room = pra.ShoeBox([9, 5, 4], fs=16000, materials=pra.Material(e_abs), max_order=15)
 
 # three microphones
 room.add_microphone_array(
@@ -32,15 +34,14 @@
     "n_src": 2,
     "n_tgt": 1,
     "ref_mic": 1,
 }
 
 
 def callback_mix(premix, snr=0, sir=0, ref_mic=0, n_src=None, n_tgt=None):
-
     # first normalize all separate recording to have unit power at microphone one
     p_mic_ref = np.std(premix[:, ref_mic, :], axis=1)
     premix /= p_mic_ref[:, None, None]
 
     # now compute the power of interference signal needed to achieve desired SIR
     sigma_i = np.sqrt(10 ** (-sir / 10) / (n_src - n_tgt))
     premix[n_tgt:n_src, :, :] *= sigma_i
@@ -54,15 +55,14 @@
     )
 
     return mix
 
 
 class TestRoomMix(unittest.TestCase):
     def test_mix(self):
-
         # Run the simulation
         premix = room.simulate(
             callback_mix=callback_mix,
             callback_mix_kwargs=mix_kwargs,
             return_premix=True,
         )
         mics_signals = room.mic_array.signals
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_rt60.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_rt60.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import numpy as np
 
 import pyroomacoustics as pra
 
-eps = 1e-10
+eps = 1e-6
 room_dim = [10, 7.5, 3.5]  # meters
 fs = 16000
 
 V = np.prod(room_dim)
 S = 2 * (
     room_dim[0] * room_dim[1] + room_dim[1] * room_dim[2] + room_dim[2] * room_dim[0]
 )
 
 
 def test_rt60_theory_single_band():
-
     # The desired reverberation time and dimensions of the room
     rt60_tgt = 0.3  # seconds
 
     # We invert Sabine's formula to obtain the parameters for the ISM simulator
     e_absorption, max_order = pra.inverse_sabine(rt60_tgt, room_dim)
 
     # Create the room
@@ -29,29 +28,27 @@
     assert (rt60_sabine - room.rt60_theory(formula="sabine")) < eps
 
     rt60_eyring = pra.rt60_eyring(S, V, e_absorption, 0.0, room.c)
     assert (rt60_eyring - room.rt60_theory(formula="eyring")) < eps
 
 
 def test_rt60_theory_multi_band():
-
     # Create the room
     room = pra.ShoeBox(
         room_dim,
         fs=fs,
         materials=pra.Material("curtains_cotton_0.5"),
     )
 
     # run the different rt60 functions
     room.rt60_theory(formula="sabine")
     room.rt60_theory(formula="eyring")
 
 
 def test_rt60_measure():
-
     # Create the room
     room = pra.ShoeBox(
         room_dim,
         fs=fs,
         materials=pra.Material("curtains_cotton_0.5"),
         max_order=10,
     )
@@ -64,11 +61,10 @@
 
     room.compute_rir()
 
     room.measure_rt60()
 
 
 if __name__ == "__main__":
-
     test_rt60_theory_single_band()
     test_rt60_theory_multi_band()
     test_rt60_measure()
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_shoebox_constants.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_shoebox_constants.py`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_source_directivities.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_source_directivities.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import pyroomacoustics as pra
+from unittest import TestCase
+
 import numpy as np
+
+import pyroomacoustics as pra
 from pyroomacoustics.directivities import (
-    DirectivityPattern,
-    DirectionVector,
     CardioidFamily,
+    DirectionVector,
+    DirectivityPattern,
 )
-from unittest import TestCase
-
 
 # create room
 room = pra.ShoeBox(
     p=[7, 5, 5],
     materials=pra.Material(0.07),
     fs=16000,
     max_order=1,
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_source_directivity_flipping.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_source_directivity_flipping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import pyroomacoustics as pra
-import numpy as np
 from unittest import TestCase
 
+import numpy as np
+
+import pyroomacoustics as pra
 import pyroomacoustics.directivities
 
 
 class TestSourceDirectivityFlipping(TestCase):
     def test_x(self):
         # create room
         mic_loc = [5, 12, 5]
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_sync.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_sync.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,57 @@
 import numpy as np
 from scipy.signal import fftconvolve
+
 import pyroomacoustics as pra
 
 
 def test_correlate():
-
     N = [100, 200, 50, 37]
     M = [47, 82, 151, 893]
 
     for n, m in zip(N, M):
-
         x = np.random.randn(n)
         y = np.random.randn(m)
 
         assert np.allclose(pra.correlate(x, y), np.correlate(x, y, mode="full"))
 
 
 def test_tdoa_delay_int():
-
     N = [100, 200, 50, 1000]
     M = [47, 37, 12, 128]
     delays = [27, 4, 10, 347]
 
     for n, m, tau in zip(N, M, delays):
-
         pulse = np.random.randn(m)
         x1 = np.zeros(n)
         x1[:m] = pulse
         x2 = np.zeros(n)
         x2[tau : tau + m] = pulse
 
         d1 = pra.tdoa(x1, x2)
         d2 = pra.tdoa(x2, x1)
 
         assert int(d1) == -tau
         assert int(d2) == tau
 
 
 def test_tdoa_delay_frac_phat():
-
     N = [14, 200, 70, 40, 28]
     M = [3, 78, 12, 10, 12]
 
     # important to start at zero and only use positive
     # delays due to fractional_delay_filter_bank function
     # subtracting minimum delay
     delays = [0.0, 0.3, 3.5, 10.1, 5.7]
 
     zero_delay_filter = pra.fractional_delay(0.0)
     frac_filters = pra.fractional_delay_filter_bank(delays)
 
     # test without explicit sampling frequency
     for n, m, tau, fil in zip(N, M, delays, frac_filters):
-
         pulse = np.random.randn(m)
         signal = np.zeros(n)
         signal[:m] = pulse
         x1 = fftconvolve(zero_delay_filter, signal)
         x2 = fftconvolve(signal, fil)
 
         d1 = pra.tdoa(x1, x2, interp=20, phat=True)
@@ -70,11 +65,10 @@
         d4 = pra.tdoa(x2, x1, interp=20, phat=True, fs=fs)
 
         assert np.allclose(d3, -tau / fs)
         assert np.allclose(d4, tau / fs)
 
 
 if __name__ == "__main__":
-
     test_correlate()
     test_tdoa_delay_int()
     test_tdoa_delay_frac_phat()
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_visibility_shoebox2d.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_visibility_shoebox2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # @version: 1.0  date: 05/06/2015 by Sidney Barthe
 # @author: robin.scheibler@epfl.ch, ivan.dokmanic@epfl.ch, sidney.barthe@epfl.ch
 # @copyright: EPFL-IC-LCAV 2015
 
 import unittest
 
 import numpy as np
+
 import pyroomacoustics as pra
 
 fs = 8000
 t0 = 0.0
 absorption = 0.90
 e_abs = 1.0 - (1.0 - absorption) ** 2
 max_order_sim = 2
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_visibility_shoebox3d.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_visibility_shoebox3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # @version: 1.0  date: 05/06/2015 by Sidney Barthe
 # @author: robin.scheibler@epfl.ch, ivan.dokmanic@epfl.ch, sidney.barthe@epfl.ch
 # @copyright: EPFL-IC-LCAV 2015
 
 import unittest
 
 import numpy as np
+
 import pyroomacoustics as pra
 
 fs = 8000
 t0 = 0.0
 absorption = 0.90
 e_abs = 1.0 - (1.0 - absorption) ** 2
 max_order_sim = 2
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_visibility_uroom.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_visibility_uroom.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # @version: 1.0  date: 05/06/2015 by Sidney Barthe
 # @author: robin.scheibler@epfl.ch, ivan.dokmanic@epfl.ch, sidney.barthe@epfl.ch
 # @copyright: EPFL-IC-LCAV 2015
 
 from unittest import TestCase
 
 import numpy as np
+
 import pyroomacoustics as pra
 
 fs = 8000
 t0 = 0.0
 absorption = 0.90
 e_abs = 1.0 - (1.0 - absorption) ** 2
 max_order_sim = 2
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/test_volume_area.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/test_volume_area.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
+
 import pyroomacoustics as pra
 
 
 def test_room_volume():
-
     eps = 0.00001
 
     # Create the 2D L-shaped room from the floor polygon
     pol = 4 * np.array([[0, 0], [0, 1], [2, 1], [2, 0.5], [1, 0.5], [1, 0]]).T
     r_absor = 0.1
     e_abs = 1.0 - (1.0 - r_absor) ** 2
     room = pra.Room.from_corners(
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/test_ccw3p.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/test_ccw3p.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # You should have received a copy of the MIT License along with this program. If
 # not, see <https://opensource.org/licenses/MIT>.
 
 import numpy as np
+
 import pyroomacoustics as pra
 
 cases = {
     "anti-clockwise": {
         "points": np.array([[1, -1], [2, -1], [1, 0]]),
         "expected": 1,  # anti-clockwise
         "label": "Test: CCW3P anti-clockwise",
@@ -41,15 +42,14 @@
         "expected": 0,  # co-linear
         "label": "Test: CCW3P co-linear",
     },
 }
 
 
 def ccw3p(case):
-
     p1, p2, p3 = case["points"]
 
     r = pra.libroom.ccw3p(p1, p2, p3)
 
     assert r == case["expected"], case["label"] + " returned: {}, expected {}".format(
         r, case["expected"]
     )
@@ -64,14 +64,12 @@
 
 
 def test_ccw3p_colinear():
     ccw3p(cases["co-linear"])
 
 
 if __name__ == "__main__":
-
     for lbl, case in cases.items():
-
         try:
             ccw3p(case)
         except:
             print("{} failed".format(lbl))
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/test_geometry_routines.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/test_geometry_routines.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # SOFTWARE.
 #
 # You should have received a copy of the MIT License along with this program. If
 # not, see <https://opensource.org/licenses/MIT>.
 from __future__ import division
 
 import unittest
+
 import numpy as np
 
 import pyroomacoustics as pra
 
 
 class TestGeometryRoutines(unittest.TestCase):
     def test_area_square(self):
@@ -222,45 +223,41 @@
 
     def test_cosangleBetween3D_special(self):
         eps = 0.001
         result = pra.libroom.cos_angle_between([36.0, 1.0, -4.0], [12.0, -1.0, 2.0])
         self.assertTrue(np.allclose(result, 0.956345613, atol=eps))
 
     def test_dist_line_point2D(self):
-
         start = [3, 3]
         end = [6, 9]
         point = [11, 4]
 
         eps = 0.001
         res = pra.libroom.dist_line_point(start, end, point)
         self.assertTrue(abs(res - np.sqrt(6 * 6 + 3 * 3)) < eps)
 
     def test_dist_line_point2D_vert(self):
-
         start = [-4, 12]
         end = [-4, 27]
         point = [7, 10]
 
         eps = 0.001
         res = pra.libroom.dist_line_point(start, end, point)
         self.assertTrue(abs(res - 11) < eps)
 
     def test_dist_line_point3D(self):
-
         start = [0, 0, 0]
         end = [1, 2, 3]
         point = [4, 5, 6]
 
         eps = 0.001
         res = pra.libroom.dist_line_point(start, end, point)
         self.assertTrue(abs(res - 1.963961012) < eps)
 
     def test_dist_line_point3D_online(self):
-
         start = [0, 0, 0]
         end = [0, 0, 3]
         point = [0, 0, 6]
 
         eps = 0.001
         res = pra.libroom.dist_line_point(start, end, point)
         self.assertTrue(abs(res) < eps)
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/test_is_inside_2d_polygon.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/test_is_inside_2d_polygon.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,31 +20,22 @@
 # SOFTWARE.
 #
 # You should have received a copy of the MIT License along with this program. If
 # not, see <https://opensource.org/licenses/MIT>.
 from __future__ import division
 
 import numpy as np
+
 import pyroomacoustics as pra
 
 polygons = [
     np.array(
         [  # this one is clockwise
-            [
-                0,
-                4,
-                4,
-                0,
-            ],
-            [
-                0,
-                0,
-                4,
-                4,
-            ],
+            [0, 4, 4, 0],
+            [0, 0, 4, 4],
         ]
     ),
     np.array(
         [  # this one is clockwise!
             [0, 0, 1, 1, 3, 3],
             [0, 1, 1, 2, 2, 0],
         ]
@@ -134,15 +125,14 @@
 
 
 def test_top_outside():
     run_inside_pol("top_outside")
 
 
 if __name__ == "__main__":
-
     test_inside()
     test_on_border()
     test_on_corner()
     test_outside()
     test_top_outside()
     test_horiz_wall_align()
     test_ray_through_vertex()
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/test_ray_energy.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/test_ray_energy.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 # SOFTWARE.
 #
 # You should have received a copy of the MIT License along with this program. If
 # not, see <https://opensource.org/licenses/MIT>.
 from __future__ import division
 
 import unittest
+
 import numpy as np
+
 import pyroomacoustics as pra
 
 
 class SimpleHistogram(list):
     """A Histogram class based on list"""
 
     def __init__(self, bin_size):
@@ -48,15 +50,14 @@
             self.append(val)
         else:
             self[pos] += val
 
 
 class TestRayEnergy(unittest.TestCase):
     def test_square_room(self):
-
         """
         This is a cubic room of 2x2x2 meters. The source is placed at [0.5,0.5, 1]
         and the receiver at [1.5, 1.5, 1]. A ray is launched towards [1, 0, 1] so that
         the first receiver hit is after travel distance of 2*sqrt(2) and each subsequent
         hit travels a further 4*sqrt(2) until the threshold energy is reached.
         """
 
@@ -78,18 +79,18 @@
             p_hit = 1.0 - np.sqrt(1.0 - detector_radius**2 / r_sq)
             histogram_gt.add(distance, transmitted / (r_sq * p_hit))
             transmitted *= (1.0 - energy_absorption) ** 4  # 4 wall hits
             distance += round_trip
 
         print("Creating the python room (polyhedral)")
         walls_corners = [
-            np.array([[0, 2, 2, 0], [0, 0, 0, 0], [0, 0, 2, 2]]),  # left
-            np.array([[0, 0, 2, 2], [2, 2, 2, 2], [0, 2, 2, 0]]),  # right
-            np.array([[0, 0, 0, 0], [0, 2, 2, 0], [0, 0, 2, 2]]),  # front`
-            np.array([[2, 2, 2, 2], [0, 0, 2, 2], [0, 2, 2, 0]]),  # back
+            np.array([[0, 2, 2, 0], [0, 0, 0, 0], [0, 0, 2, 2]]),  # front
+            np.array([[0, 0, 2, 2], [2, 2, 2, 2], [0, 2, 2, 0]]),  # back
+            np.array([[0, 0, 0, 0], [0, 2, 2, 0], [0, 0, 2, 2]]),  # left`
+            np.array([[2, 2, 2, 2], [0, 0, 2, 2], [0, 2, 2, 0]]),  # right
             np.array(
                 [
                     [0, 2, 2, 0],
                     [0, 0, 2, 2],
                     [0, 0, 0, 0],
                 ]
             ),  # floor
@@ -152,13 +153,13 @@
         )
 
         h_poly = room_poly.room_engine.microphones[0].histograms[0].get_hist()
         h_cube = room_cube.room_engine.microphones[0].histograms[0].get_hist()
         histogram_rt_poly = np.array(h_poly[0])[: len(histogram_gt)]
         histogram_rt_cube = np.array(h_cube[0])[: len(histogram_gt)]
 
-        self.assertTrue(np.allclose(histogram_rt_poly, histogram_gt))
-        self.assertTrue(np.allclose(histogram_rt_cube, histogram_gt))
+        self.assertTrue(np.allclose(histogram_rt_poly, histogram_gt, atol=1e-5))
+        self.assertTrue(np.allclose(histogram_rt_cube, histogram_gt, atol=1e-5))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/test_room_construct.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/test_room_construct.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # SOFTWARE.
 #
 # You should have received a copy of the MIT License along with this program. If
 # not, see <https://opensource.org/licenses/MIT>.
 from __future__ import division
 
 import numpy as np
+
 import pyroomacoustics as pra
 
 wall_corners = [
     np.array([[0, 3, 3, 0], [0, 0, 0, 0], [0, 0, 2, 2]]),  # left
     np.array([[0, 0, 6, 6], [8, 8, 8, 8], [0, 4, 4, 0]]),  # right
     np.array([[0, 0, 6, 3], [0, 8, 8, 0], [0, 0, 0, 0]]),  # floor
     np.array([[0, 3, 6, 0], [0, 0, 8, 8], [2, 2, 4, 4]]),  # ceiling
@@ -66,9 +67,8 @@
 
 
 def test_room_construct():
     room_construct()
 
 
 if __name__ == "__main__":
-
     room = test_room_construct()
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/test_room_walls.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/test_room_walls.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 # You should have received a copy of the MIT License along with this program. If
 # not, see <https://opensource.org/licenses/MIT>.
 from __future__ import division
 
 import unittest
 
 import numpy as np
+
 import pyroomacoustics as pra
 
 c0 = np.array(
     [
         [0, 3, 3, 0],
         [0, 0, 0, 0],
         [0, 0, 2, 2],
@@ -237,15 +238,14 @@
 )  # side4
 
 wall_corners_2D_shoebox = [f0, f1, f2, f3]
 absorptions_shoebox = [0.1, 0.1, 0.1, 0.1]
 
 
 def room_factory(walls, obstructing_walls, microphones):
-
     args = [
         walls,
         obstructing_walls,
         [],
         pra.constants.get("c"),  # speed of sound
         3,
         1e-7,  # energy_thres
@@ -264,15 +264,14 @@
         room.add_mic(microphones[:, None, m])
 
     return room
 
 
 class TestRoomWalls(unittest.TestCase):
     def test_max_dist_3D(self):
-
         walls = [
             pra.wall_factory(c, [a], [s])
             for c, a, s in zip(wall_corners_3D, absorptions_3D, scatterings_2D)
         ]
         obstructing_walls = []
         microphones = np.array(
             [
@@ -292,15 +291,14 @@
 
         eps = 0.001
         result = room.get_max_distance()
         correct = np.sqrt(116) + 1
         self.assertTrue(abs(result - correct) < eps)
 
     def test_max_dist_2D(self):
-
         walls = [
             pra.wall_factory(c, [a], [s])
             for c, a, s in zip(wall_corners_2D, absorptions_2D, scatterings_2D)
         ]
         obstructing_walls = []
         microphones = np.array(
             [
@@ -343,26 +341,24 @@
         )
         w2 = pra.wall_factory(
             wall_corners_3D[1], absorptions_3D[:1], scatterings_3D[:1]
         )
         self.assertTrue(not w1.same_as(w2))
 
     def test_same_wall_false3D_more_corners(self):
-
         # Modification of wall_corners_3D[0]: adding a corner => 5 corners wall
         c1 = np.array([[0, 3, 3, 1.5, 0], [0, 0, 0, 0, 0], [0, 0, 2, 1.5, 2]])
 
         w1 = pra.wall_factory(
             wall_corners_3D[0], absorptions_3D[:1], scatterings_3D[:1]
         )
         w2 = pra.wall_factory(c1, absorptions_3D[:1], scatterings_3D[:1])
         self.assertTrue(not w1.same_as(w2))
 
     def test_next_wall_hit(self):
-
         walls = [
             pra.wall_factory(c, [a], [s])
             for c, a, s in zip(wall_corners_3D, absorptions_3D, scatterings_3D)
         ]
         obstructing_walls = []
         microphones = np.array(
             [
@@ -396,15 +392,14 @@
         correct_result = np.allclose(ttuple[0], result, atol=eps)
         correct_next_wall = ttuple[1] == 4
         correct_distance = np.allclose(ttuple[2], np.linalg.norm(result - start))
 
         self.assertTrue(correct_next_wall and correct_result and correct_distance)
 
     def test_next_wall_nohit(self):
-
         walls = [
             pra.wall_factory(c, [a], [s])
             for c, a, s in zip(wall_corners_3D, absorptions_3D, scatterings_3D)
         ]
         obstructing_walls = []
         microphones = np.array(
             [
@@ -431,15 +426,14 @@
         end = [-2, -3, -1]
 
         ttuple = room.next_wall_hit(start, end, False)
 
         self.assertTrue(ttuple[1] == -1)
 
     def test_next_wall_hit2D(self):
-
         walls = [
             pra.wall_factory(c, [a], [s])
             for c, a, s in zip(wall_corners_2D, absorptions_2D, scatterings_2D)
         ]
         obstructing_walls = []
         microphones = np.array(
             [
@@ -507,15 +501,14 @@
             [pra.libroom.Hit(1)]
         ]  # arbitrary initialisation to have the correct shape
         self.assertTrue(
             not room.scat_ray(energy, prev_wall, prev_last_hit, last_hit, total_dist)
         )
 
     def test_scat_ray_ok(self):
-
         walls = [
             pra.wall_factory(c, [a], [s])
             for c, a, s in zip(
                 wall_corners_2D_non_convex, absorptions_2D, scatterings_2D
             )
         ]
         obstructing_walls = [1, 2]
@@ -585,58 +578,54 @@
 
         eps = 0.0001
         result = room.compute_scat_energy(energy, scatter_coef, prev_wall, prev_last_hit, last_hit, mic_pos, total_dist)
         self.assertTrue(np.allclose(result, np.sqrt(0.1*2*(1-np.sqrt(3.1*3.1-0.1*0.1)/3.1))/(5), atol=eps))
     """
 
     def test_contains_2D(self):
-
         walls = [
             pra.wall_factory(c, [a], [s])
             for c, a, s in zip(
                 wall_corners_2D_non_convex, absorptions_2D, scatterings_2D
             )
         ]
         obstructing_walls = []
         microphones = np.array([[0.5], [0.2]])
 
         room = room_factory(walls, obstructing_walls, microphones)
 
         self.assertTrue(room.contains(microphones[:, 0]))
 
     def test_notcontains_2D(self):
-
         walls = [
             pra.wall_factory(c, [a], [s])
             for c, a, s in zip(
                 wall_corners_2D_non_convex, absorptions_2D, scatterings_2D
             )
         ]
         obstructing_walls = []
         microphones = np.array([[1.0], [1.7]])
 
         room = room_factory(walls, obstructing_walls, microphones)
 
         self.assertTrue(not room.contains(microphones[:, 0]))
 
     def test_contains_3D(self):
-
         walls = [
             pra.wall_factory(c, [a], [s])
             for c, a, s in zip(wall_corners_3D, absorptions_3D, scatterings_3D)
         ]
         obstructing_walls = []
         microphones = np.array([[1.0], [1.0], [1.0]])
 
         room = room_factory(walls, obstructing_walls, microphones)
 
         self.assertTrue(room.contains(microphones[:, 0]))
 
     def test_notcontains_3D(self):
-
         walls = [
             pra.wall_factory(c, [a], [s])
             for c, a, s in zip(wall_corners_3D, absorptions_3D, scatterings_3D)
         ]
         obstructing_walls = []
         microphones = np.array([[5.0], [7.0], [40]])
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/test_shoebox_simple.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/test_shoebox_simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 
 This test just checks that the ray tracing runs properly without segfault
 for the Shoebox rooms.
 
 It was created to address Issue #293 on github.
 https://github.com/LCAV/pyroomacoustics/issues/293<Paste>
 """
+
 import numpy as np
-import pyroomacoustics as pra
 import pytest
 
+import pyroomacoustics as pra
+
 
 def test_issu293_segfault_2d():
     np.random.seed(0)
     for i in range(30):
         room_dim = [30.0, 30.0]
         source = [2.0, 3.0]
         mic_array = [[8.0], [8.0]]
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/test_wall_construct.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/test_wall_construct.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # SOFTWARE.
 #
 # You should have received a copy of the MIT License along with this program. If
 # not, see <https://opensource.org/licenses/MIT>.
 from __future__ import division
 
 import numpy as np
+
 import pyroomacoustics as pra
 
 eps = 1e-6
 
 # The vertices of the wall are assumed to turn counter-clockwise around the
 # normal of the wall
 
@@ -111,14 +112,13 @@
     wall2 = pra.wall_factory(w_info["corners"][:, ::-1], [0.2], [0.1])
 
     err = np.linalg.norm(wall1.normal + wall2.normal)
     assert err < eps, "The error is {}".format(err)
 
 
 if __name__ == "__main__":
-
     test_wall_3d_construct_0()
     test_wall_3d_normal_0()
     test_wall_3d_area_0()
     test_wall_3d_construct_1()
     test_wall_3d_normal_1()
     test_wall_3d_area_1()
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/test_wall_intersection.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/test_wall_intersection.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # SOFTWARE.
 #
 # You should have received a copy of the MIT License along with this program. If
 # not, see <https://opensource.org/licenses/MIT>.
 from __future__ import division
 
 import numpy as np
+
 import pyroomacoustics as pra
 
 eps = 1e-6
 
 cases = {
     "3d_valid": {
         "corners": np.array(
@@ -300,15 +301,14 @@
         "absorption": [0.2],
         "scattering": [0.1],
     },
 }
 
 
 def run_intersect(lbl):
-
     case = cases[lbl]
     wall = pra.wall_factory(case["corners"], case["absorption"], case["scattering"])
     p1, p2 = case["seg"]
 
     isect_exp = case["intersect"]
     r_exp = case["type"]
     isect = np.zeros(wall.dim, dtype=np.float32)
@@ -400,15 +400,14 @@
 
 
 def test_2d_none_2():
     run_intersect("2d_none_2")
 
 
 if __name__ == "__main__":
-
     test_3d_valid()
     test_3d_endpt_1()
     test_3d_endpt_2()
     test_3d_bndry()
     test_3d_vertex()
     test_3d_endpt_bndry_1()
     test_3d_endpt_bndry_2()
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/tests/tests_libroom/test_wall_side_reflect.py` & `pyroomacoustics-0.7.4/pyroomacoustics/tests/tests_libroom/test_wall_side_reflect.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 # SOFTWARE.
 #
 # You should have received a copy of the MIT License along with this program. If
 # not, see <https://opensource.org/licenses/MIT>.
 from __future__ import division
 
 import unittest
+
 import numpy as np
+
 import pyroomacoustics as pra
 
 eps = 1e-6
 
 corners = {
     "3d": np.array(
         [
@@ -94,15 +96,14 @@
     r = wall.side(p)
 
     print("{}: returned={} expected={}".format(label, r, r_exp))
     return r == r_exp
 
 
 def run_reflect(label):
-
     p = points[label]["p"]
     p_refl = np.array(points[label]["reflect"])
     r_exp = points[label]["expect"]
     d = points[label]["d"]
 
     wall = pra.wall_factory(corners[d], [0.1], [0.1])
 
@@ -161,15 +162,14 @@
         self.assertTrue(ret)
 
     def test_reflect_2d_on(self):
         ret = run_reflect("2d_on")
         self.assertTrue(ret)
 
     def test_reflected_end2D(self):
-
         eps = 0.001
         start = [1, 3]
 
         hit = [5, 3]
         # normal = [-1, -1]
         corners = np.array(
             [
@@ -180,15 +180,14 @@
         wall = pra.wall_factory(corners, [0.1], [0.1])
         length = 4
 
         res = wall.normal_reflect(start, hit, length)
         self.assertTrue(np.allclose(res, [5.0, -1.0], atol=eps))
 
     def test_reflected_end3D(self):
-
         eps = 0.001
         start = [1, 1, 1]
         hit = [-1, 1, 3]
         # normal = [1, 0, 0]
         corners = np.array(
             [
                 [
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/transform/__init__.py` & `pyroomacoustics-0.7.4/pyroomacoustics/transform/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,11 +11,10 @@
     | :py:obj:`pyroomacoustics.transform.dft`
 STFT
     | A class for continuous STFT processing and frequency domain filtering
     | :py:obj:`pyroomacoustics.transform.stft`
 
 """
 
-
 from . import stft
 from .dft import DFT
 from .stft import STFT
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/transform/dft.py` & `pyroomacoustics-0.7.4/pyroomacoustics/transform/dft.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 More on ``pyfftw`` can be read here: 
 https://pyfftw.readthedocs.io/en/latest/index.html
 
 More on ``mkl_fft`` can be read here: 
 https://github.com/IntelPython/mkl_fft
 """
 
-import numpy as np
-from numpy.fft import rfft, irfft
 import warnings
 
+import numpy as np
+from numpy.fft import irfft, rfft
+
 try:
     import pyfftw
 
     pyfftw_available = True
 except ImportError:
     pyfftw_available = False
 
@@ -90,15 +91,14 @@
         analysis_window=None,
         synthesis_window=None,
         transform="numpy",
         axis=0,
         precision="double",
         bits=None,
     ):
-
         self.nfft = nfft
         self.D = D
         self.axis = axis
 
         if bits is not None and precision is not None:
             warnings.warn(
                 'Deprecated keyword "bits" ignored in favor of new keyword "precision"',
@@ -153,15 +153,15 @@
             else:
                 self.synthesis_window = synthesis_window.astype(time_dtype)
         else:
             self.synthesis_window = None
 
         if transform == "fftw":
             if pyfftw_available:
-                from pyfftw import empty_aligned, FFTW
+                from pyfftw import FFTW, empty_aligned
 
                 self.transform = transform
                 # allocate input (real) and output for pyfftw
                 if self.D == 1:
                     self.a = empty_aligned(self.nfft, dtype=time_dtype)
                     self.b = empty_aligned(self.nfft // 2 + 1, dtype=freq_dtype)
                     self._forward = FFTW(self.a, self.b)
@@ -223,28 +223,20 @@
 
         # apply window if needed
         if self.analysis_window is not None:
             np.multiply(self.analysis_window, x, x)
 
         # apply DFT
         if self.transform == "fftw":
-            self.a[
-                :,
-            ] = x
-            self.X[
-                :,
-            ] = self._forward()
+            self.a[:,] = x
+            self.X[:,] = self._forward()
         elif self.transform == "mkl":
-            self.X[
-                :,
-            ] = mkl_fft.rfft_numpy(x, self.nfft, axis=self.axis)
+            self.X[:,] = mkl_fft.rfft_numpy(x, self.nfft, axis=self.axis)
         else:
-            self.X[
-                :,
-            ] = rfft(x, self.nfft, axis=self.axis)
+            self.X[:,] = rfft(x, self.nfft, axis=self.axis)
 
         return self.X
 
     def synthesis(self, X=None):
         """
         Perform time synthesis of frequency domain to real signal using the
         inverse DFT.
@@ -265,31 +257,23 @@
         if X is not None:
             if X.shape != self.X.shape:
                 raise ValueError(
                     "Invalid input dimensions! Got (%d, %d), expecting (%d, %d)."
                     % (X.shape[0], X.shape[1], self.X.shape[0], self.X.shape[1])
                 )
 
-            self.X[
-                :,
-            ] = X
+            self.X[:,] = X
 
         # inverse DFT
         if self.transform == "fftw":
             self.b[:] = self.X
-            self.x[
-                :,
-            ] = self._backward()
+            self.x[:,] = self._backward()
         elif self.transform == "mkl":
-            self.x[
-                :,
-            ] = mkl_fft.irfft_numpy(self.X, self.nfft, axis=self.axis)
+            self.x[:,] = mkl_fft.irfft_numpy(self.X, self.nfft, axis=self.axis)
         else:
-            self.x[
-                :,
-            ] = irfft(self.X, self.nfft, axis=self.axis)
+            self.x[:,] = irfft(self.X, self.nfft, axis=self.axis)
 
         # apply window if needed
         if self.synthesis_window is not None:
             np.multiply(self.synthesis_window, self.x, self.x)
 
         return self.x
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/transform/stft.py` & `pyroomacoustics-0.7.4/pyroomacoustics/transform/stft.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 # not, see <https://opensource.org/licenses/MIT>.
 
 """Class for real-time STFT analysis and processing."""
 from __future__ import division
 
 import numpy as np
 from numpy.lib.stride_tricks import as_strided as _as_strided
+
 from .dft import DFT
 
 
 class STFT(object):
     """
     A class for STFT processing.
 
@@ -80,15 +81,14 @@
         synthesis_window=None,
         channels=1,
         transform="numpy",
         streaming=True,
         precision="double",
         **kwargs
     ):
-
         # initialize parameters
         self.num_samples = N  # number of samples per frame
         self.num_channels = channels  # number of channels
         self.mono = True if self.num_channels == 1 else False
         if hop is not None:  # hop size --> number of input samples
             self.hop = hop
         else:
@@ -179,17 +179,15 @@
             self.y_p = np.zeros(
                 (self.n_state_out, self.num_channels), dtype=self.time_dtype
             )
             # output samples
             self.out = np.zeros((self.hop, self.num_channels), dtype=self.time_dtype)
 
         # useful views on the input buffer
-        self.fft_in_state = self.fft_in_buffer[
-            self.zf : self.zf + self.n_state,
-        ]
+        self.fft_in_state = self.fft_in_buffer[self.zf : self.zf + self.n_state,]
         self.fresh_samples = self.fft_in_buffer[
             self.zf + self.n_state : self.zf + self.n_state + self.hop,
         ]
         self.old_samples = self.fft_in_buffer[
             self.zf + self.hop : self.zf + self.hop + self.n_state,
         ]
 
@@ -346,15 +344,14 @@
             if len(x_shape) > 1:  # received multi-channel
                 raise ValueError(
                     "Received %d channels; expecting 1D mono " "signal." % x_shape[1]
                 )
 
         # ----check number of frames
         if self.streaming:  # need integer multiple of hops
-
             if self.fixed_input:
                 if x_shape[0] != self.num_frames * self.hop:
                     raise ValueError(
                         "Input must be of length %d; received %d "
                         "samples." % (self.num_frames * self.hop, x_shape[0])
                     )
             else:
@@ -368,15 +365,14 @@
                             (x, np.zeros((extra_samples, self.num_channels)))
                         )
 
         # non-streaming
         # need at least num_samples for last frame
         # e.g.[hop|hop|...|hop|num_samples]
         else:
-
             if self.fixed_input:
                 if x_shape[0] != (self.hop * (self.num_frames - 1) + self.num_samples):
                     raise ValueError(
                         "Input must be of length %d; received %d "
                         "samples."
                         % (
                             (self.hop * (self.num_frames - 1) + self.num_samples),
@@ -392,15 +388,14 @@
                         x = np.concatenate((x, np.zeros(extra_samples)))
                     else:
                         x = np.concatenate(
                             (x, np.zeros((extra_samples, self.num_channels)))
                         )
                     self.num_frames = 1
                 else:
-
                     # calculate num_frames and append zeros if necessary
                     self.num_frames = int(
                         np.ceil((x_shape[0] - self.num_samples) / self.hop) + 1
                     )
                     extra_samples = (
                         (self.num_frames - 1) * self.hop + self.num_samples
                     ) - x_shape[0]
@@ -444,58 +439,44 @@
         Parameters
         -----------
         x_n : numpy array
             [self.hop] new samples
         """
 
         # correct input size check in: dft.analysis()
-        self.fresh_samples[:,] = x_n[
-            :,
-        ]  # introduce new samples
-        self.x_p[
-            :,
-        ] = self.old_samples  # save next state
+        self.fresh_samples[:,] = x_n[:,]  # introduce new samples
+        self.x_p[:,] = self.old_samples  # save next state
 
         # apply DFT to current frame
         self.X[:] = self.dft.analysis(self.fft_in_buffer)
 
         # shift backwards in the buffer the state
-        self.fft_in_state[:,] = self.x_p[
-            :,
-        ]
+        self.fft_in_state[:,] = self.x_p[:,]
 
     def _analysis_streaming(self, x):
         """
         STFT analysis for streaming case in which we expect
         [num_frames*hop] samples
         """
 
         if self.num_frames == 1:
             self._analysis_single(x)
         else:
             n = 0
             for k in range(self.num_frames):
                 # introduce new samples
-                self.fresh_samples[:,] = x[
-                    n : n + self.hop,
-                ]
+                self.fresh_samples[:,] = x[n : n + self.hop,]
                 # save next state
-                self.x_p[
-                    :,
-                ] = self.old_samples
+                self.x_p[:,] = self.old_samples
 
                 # apply DFT to current frame
-                self.X[
-                    k,
-                ] = self.dft.analysis(self.fft_in_buffer)
+                self.X[k,] = self.dft.analysis(self.fft_in_buffer)
 
                 # shift backwards in the buffer the state
-                self.fft_in_state[:,] = self.x_p[
-                    :,
-                ]
+                self.fft_in_state[:,] = self.x_p[:,]
 
                 n += self.hop
 
     def _analysis_non_streaming(self, x):
         """
         STFT analysis for non-streaming case in which we expect
         [(num_frames-1)*hop+num_samples] samples
@@ -503,30 +484,28 @@
 
         ## ----- STRIDED WAY
         new_strides = (x.strides[0], self.hop * x.strides[0])
         new_shape = (self.num_samples, self.num_frames)
 
         if not self.mono:
             for c in range(self.num_channels):
-
                 y = _as_strided(x[:, c], shape=new_shape, strides=new_strides)
                 y = np.concatenate(
                     (
                         np.zeros((self.zf, self.num_frames)),
                         y,
                         np.zeros((self.zb, self.num_frames)),
                     )
                 )
 
                 if self.num_frames == 1:
                     self.X[:, c] = self.dft_frames.analysis(y[:, 0]).T
                 else:
                     self.X[:, :, c] = self.dft_frames.analysis(y).T
         else:
-
             y = _as_strided(x, shape=new_shape, strides=new_strides)
             y = np.concatenate(
                 (
                     np.zeros((self.zf, self.num_frames)),
                     y,
                     np.zeros((self.zb, self.num_frames)),
                 )
@@ -583,15 +562,14 @@
         else:
             self.X = X
             self.num_frames = num_frames
 
         return self.X
 
     def process(self, X=None):
-
         """
         Parameters
         -----------
         X  : numpy array
             X can take on multiple shapes:
             1) (N,) if it is single channel and only one frame
             2) (N,D) if it is multi-channel and only one frame
@@ -617,19 +595,17 @@
             self._process_single()
         elif self.num_frames > 1:
             self._process_multiple()
 
         return self.X
 
     def _process_single(self):
-
         np.multiply(self.X, self.H, self.X)
 
     def _process_multiple(self):
-
         if not self.fixed_input:
             if self.mono:
                 self.H_multi = np.tile(self.H, (self.num_frames, 1))
             else:
                 self.H_multi = np.tile(self.H, (self.num_frames, 1, 1))
 
         np.multiply(self.X, self.H_multi, self.X)
@@ -690,30 +666,27 @@
         x_r : numpy array
             Recovered signal.
 
         """
 
         # synthesis + overlap and add
         if not self.mono:
-
             x_r = np.zeros(
                 (self.num_frames * self.hop, self.num_channels), dtype=self.time_dtype
             )
 
             n = 0
             for f in range(self.num_frames):
-
                 # apply IDFT to current frame and reconstruct output
-                x_r[
-                    n : n + self.hop,
-                ] = self._overlap_and_add(self.dft.synthesis(self.X[f, :, :]))
+                x_r[n : n + self.hop,] = self._overlap_and_add(
+                    self.dft.synthesis(self.X[f, :, :])
+                )
                 n += self.hop
 
         else:
-
             x_r = np.zeros(self.num_frames * self.hop, dtype=self.time_dtype)
 
             # treat number of frames as the multiple channels for DFT
             if not self.fixed_input:
                 self.dft_frames = DFT(
                     nfft=self.nfft,
                     D=self.num_frames,
@@ -724,46 +697,33 @@
 
             # back to time domain
             mx = self.dft_frames.synthesis(self.X.T)
 
             # overlap and add
             n = 0
             for f in range(self.num_frames):
-                x_r[
-                    n : n + self.hop,
-                ] = self._overlap_and_add(mx[:, f])
+                x_r[n : n + self.hop,] = self._overlap_and_add(mx[:, f])
                 n += self.hop
 
         return x_r
 
     def _overlap_and_add(self, x=None):
-
         if x is None:
             x = self.dft.x
 
-        self.out[:,] = x[
-            0 : self.hop,
-        ]  # fresh output samples
+        self.out[:,] = x[0 : self.hop,]  # fresh output samples
 
         # add state from previous frames when overlap is used
         if self.n_state_out > 0:
             m = np.minimum(self.hop, self.n_state_out)
-            self.out[:m,] += self.y_p[
-                :m,
-            ]
+            self.out[:m,] += self.y_p[:m,]
             # update state variables
-            self.y_p[: -self.hop,] = self.y_p[
-                self.hop :,
-            ]  # shift out left
-            self.y_p[
-                -self.hop :,
-            ] = 0.0
-            self.y_p[:,] += x[
-                -self.n_state_out :,
-            ]
+            self.y_p[: -self.hop,] = self.y_p[self.hop :,]  # shift out left
+            self.y_p[-self.hop :,] = 0.0
+            self.y_p[:,] += x[-self.n_state_out :,]
 
         return self.out
 
 
 " ---------------------------------------------------------------------------- "
 " --------------- One-shot functions to avoid creating object. --------------- "
 " ---------------------------------------------------------------------------- "
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/transform/tests/test_dft.py` & `pyroomacoustics-0.7.4/pyroomacoustics/transform/tests/test_dft.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from __future__ import division, print_function
+
 from unittest import TestCase
+
 import numpy as np
+
 import pyroomacoustics as pra
 
 tol = -80  # dB
 nfft = 128
 D = 7
 x = np.random.randn(nfft, D).astype("float32")
 X_numpy = np.fft.rfft(x, axis=0).astype("complex64")
@@ -18,15 +21,14 @@
 
     pyfftw_available = True
 except ImportError:
     pyfftw_available = False
 
 
 def no_window(nfft, D, transform, axis=0):
-
     if D == 1:
         x_local = x[:, 0]
         X_local = X_numpy[:, 0]
     else:
         if axis == 0:
             x_local = x
             X_local = X_numpy
@@ -45,15 +47,14 @@
     x_r = dft.synthesis()
     err_bwd = pra.dB(np.linalg.norm(x_local - x_r) + eps)
 
     return err_fwd, err_bwd
 
 
 def window(nfft, D, analysis_window, synthesis_window, axis=0):
-
     if D == 1:
         x_local = x[:, 0]
         X_local = X_numpy[:, 0]
     else:
         if axis == 0:
             x_local = x
             X_local = X_numpy
@@ -123,15 +124,14 @@
         res = window(nfft, D, analysis_window, synthesis_window)
         self.assertTrue(res)
         res = window(nfft, D, analysis_window, synthesis_window, axis=1)
         self.assertTrue(res)
 
 
 if __name__ == "__main__":
-
     print()
     print("1D")
     res = no_window(nfft, D=1, transform="numpy")
     print("numpy :", res)
     if pyfftw_available:
         res = no_window(nfft, D=1, transform="fftw")
         print("fftw :", res)
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/transform/tests/test_dft_timing.py` & `pyroomacoustics-0.7.4/pyroomacoustics/transform/tests/test_dft_timing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from __future__ import division, print_function
+
+import time
+
 import numpy as np
+
 import pyroomacoustics as pra
-import time
 
 try:
     import pyfftw
 
     pyfftw_available = True
 except ImportError:
     pyfftw_available = False
@@ -21,15 +24,14 @@
 n_trials = 1000
 nfft = 128
 D = 7
 x = np.random.randn(nfft, D).astype("float32")
 
 
 def timing(transform, n_trials):
-
     dft = pra.transform.DFT(nfft, D, transform=transform)
     start_time = time.time()
     for k in range(n_trials):
         dft.analysis(x)
     analysis_time = (time.time() - start_time) / n_trials * 1e6
     start_time = time.time()
     for k in range(n_trials):
@@ -62,15 +64,14 @@
 synthesis_time = (time.time() - start_time) / n_trials * 1e6
 print(
     "avg numpy w/o class : %f [1e-6 sec], (analysis, synthesis)=(%f, %f) [1e-6 sec]"
     % (analysis_time + synthesis_time, analysis_time, synthesis_time)
 )
 
 if pyfftw_available:
-
     # prepare
     a = pyfftw.empty_aligned([nfft, D], dtype="float32")
     b = pyfftw.empty_aligned([nfft // 2 + 1, D], dtype="complex64")
     c = pyfftw.empty_aligned([nfft, D], dtype="float32")
     forward = pyfftw.FFTW(a, b, axes=(0,))
     backward = pyfftw.FFTW(b, c, axes=(0,), direction="FFTW_BACKWARD")
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/transform/tests/test_stft.py` & `pyroomacoustics-0.7.4/pyroomacoustics/transform/tests/test_stft.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import division, print_function
 
 from unittest import TestCase
 
 import numpy as np
+from scipy.signal import fftconvolve
+
 import pyroomacoustics as pra
 from pyroomacoustics.transform import STFT
-from scipy.signal import fftconvolve
 
 """
 We create a signal, a simple filter and compute their convolution.
 
 Then we test STFT block procesing with and without overlap,
 and with and without filtering. Simulating a case of real-time
 block processing.
@@ -32,15 +33,14 @@
 # convolved signal
 y = np.zeros((x.shape[0] + h_len - 1, x.shape[1]))
 for i in range(x.shape[1]):
     y[:, i] = fftconvolve(x[:, i], h[:, i])
 
 
 def incorrect_input_size(D, num_frames):
-
     if D == 1:
         x_local = x[:, 0]
     else:
         x_local = x[:, :D]
 
     # parameters
     block_size = 512
@@ -75,17 +75,15 @@
         x_local = x[:, :D]
 
     # parameters
     block_size = 512  # make sure the FFT size is a power of 2
     hop = block_size  # no overlap
     if not streaming:
         num_samples = (num_frames - 1) * hop + block_size
-        x_local = x_local[
-            :num_samples,
-        ]
+        x_local = x_local[:num_samples,]
 
     # Create the STFT object
     if fixed_memory:
         stft = STFT(
             block_size,
             hop=hop,
             channels=D,
@@ -98,45 +96,28 @@
             block_size, hop=hop, channels=D, transform=transform, streaming=streaming
         )
 
     # collect the processed blocks
     processed_x = np.zeros(x_local.shape)
 
     if streaming:
-
         n = 0
         hop_frames = hop * num_frames
         # process the signals while full blocks are available
         while x_local.shape[0] - n > hop_frames:
-            stft.analysis(
-                x_local[
-                    n : n + hop_frames,
-                ]
-            )
-            processed_x[
-                n : n + hop_frames,
-            ] = stft.synthesis()
+            stft.analysis(x_local[n : n + hop_frames,])
+            processed_x[n : n + hop_frames,] = stft.synthesis()
             n += hop_frames
 
     else:
-
         stft.analysis(x_local)
         processed_x = stft.synthesis()
         n = processed_x.shape[0]
 
-    error = np.max(
-        np.abs(
-            x_local[
-                :n,
-            ]
-            - processed_x[
-                :n,
-            ]
-        )
-    )
+    error = np.max(np.abs(x_local[:n,] - processed_x[:n,]))
 
     return error
 
 
 def with_arbitrary_overlap_synthesis_window(
     D, num_frames=1, fixed_memory=False, streaming=True, overlap=0.5
 ):
@@ -154,17 +135,15 @@
         x_local = x[:, :D]
 
     # parameters
     block_size = 512  # make sure the FFT size is a power of 2
     hop = int((1 - overlap) * block_size)  # quarter overlap
     if not streaming:
         num_samples = (num_frames - 1) * hop + block_size
-        x_local = x_local[
-            :num_samples,
-        ]
+        x_local = x_local[:num_samples,]
 
     analysis_window = pra.hann(block_size)
     synthesis_window = pra.transform.stft.compute_synthesis_window(analysis_window, hop)
 
     # Create the STFT object
     if fixed_memory:
         stft = STFT(
@@ -188,37 +167,25 @@
             streaming=streaming,
         )
 
     # collect the processed blocks
     processed_x = np.zeros(x_local.shape)
 
     if streaming:
-
         n = 0
         hop_frames = hop * num_frames
         # process the signals while full blocks are available
         while x_local.shape[0] - n > hop_frames:
-            stft.analysis(
-                x_local[
-                    n : n + hop_frames,
-                ]
-            )
-            processed_x[
-                n : n + hop_frames,
-            ] = stft.synthesis()
+            stft.analysis(x_local[n : n + hop_frames,])
+            processed_x[n : n + hop_frames,] = stft.synthesis()
             n += hop_frames
 
         error = np.max(
             np.abs(
-                x_local[
-                    : n - block_size + hop,
-                ]
-                - processed_x[
-                    block_size - hop : n,
-                ]
+                x_local[: n - block_size + hop,] - processed_x[block_size - hop : n,]
             )
         )
 
         if 20 * np.log10(error) > -10:
             import matplotlib.pyplot as plt
 
             if x_local.ndim == 1:
@@ -226,30 +193,20 @@
                 plt.plot(processed_x[block_size - hop : n])
             else:
                 plt.plot(x_local[: n - block_size + hop, 0])
                 plt.plot(processed_x[block_size - hop : n, 0])
             plt.show()
 
     else:
-
         stft.analysis(x_local)
         processed_x = stft.synthesis()
         n = processed_x.shape[0]
 
         L = block_size - hop
-        error = np.max(
-            np.abs(
-                x_local[
-                    L:-L,
-                ]
-                - processed_x[
-                    L:,
-                ]
-            )
-        )
+        error = np.max(np.abs(x_local[L:-L,] - processed_x[L:,]))
 
         if 20 * np.log10(error) > -10:
             import matplotlib.pyplot as plt
 
             if x_local.ndim == 1:
                 plt.plot(x_local[L:-L])
                 plt.plot(processed_x[L:])
@@ -280,17 +237,15 @@
         h_local = h[:, :D]
 
     # parameters
     block_size = 512 - h_len + 1  # make sure the FFT size is a power of 2
     hop = block_size  # no overlap
     if not streaming:
         num_samples = (num_frames - 1) * hop + block_size
-        x_local = x_local[
-            :num_samples,
-        ]
+        x_local = x_local[:num_samples,]
 
     # Create the STFT object
     if fixed_memory:
         stft = STFT(
             block_size,
             hop=hop,
             channels=D,
@@ -306,47 +261,30 @@
     # setup the filter
     stft.set_filter(h_local, zb=h_len - 1)
 
     # collect the processed blocks
     processed_x = np.zeros(x_local.shape)
 
     if not streaming:
-
         stft.analysis(x_local)
         stft.process()
         processed_x = stft.synthesis()
         n = processed_x.shape[0]
 
     else:
-
         n = 0
         hop_frames = hop * num_frames
         # process the signals while full blocks are available
         while x_local.shape[0] - n > hop_frames:
-            stft.analysis(
-                x_local[
-                    n : n + hop_frames,
-                ]
-            )
+            stft.analysis(x_local[n : n + hop_frames,])
             stft.process()  # apply the filter
-            processed_x[
-                n : n + hop_frames,
-            ] = stft.synthesis()
+            processed_x[n : n + hop_frames,] = stft.synthesis()
             n += hop_frames
 
-    error = np.max(
-        np.abs(
-            y_local[
-                :n,
-            ]
-            - processed_x[
-                :n,
-            ]
-        )
-    )
+    error = np.max(np.abs(y_local[:n,] - processed_x[:n,]))
 
     return error
 
 
 def with_half_overlap_no_filter(D, num_frames=1, fixed_memory=False, streaming=True):
     """
     D             - number of channels
@@ -363,17 +301,15 @@
 
     # parameters
     block_size = 512  # make sure the FFT size is a power of 2
     hop = block_size // 2  # half overlap
     window = pra.hann(block_size)  # the analysis window
     if not streaming:
         num_samples = (num_frames - 1) * hop + block_size
-        x_local = x_local[
-            :num_samples,
-        ]
+        x_local = x_local[:num_samples,]
 
     # Create the STFT object
     if fixed_memory:
         stft = STFT(
             block_size,
             hop=hop,
             channels=D,
@@ -392,56 +328,35 @@
             streaming=streaming,
         )
 
     # collect the processed blocks
     processed_x = np.zeros(x_local.shape)
 
     if not streaming:
-
         stft.analysis(x_local)
         processed_x = stft.synthesis()
         n = processed_x.shape[0]
 
         error = np.max(
             np.abs(
-                x_local[
-                    block_size - hop : n - hop,
-                ]
-                - processed_x[
-                    block_size - hop : n - hop,
-                ]
+                x_local[block_size - hop : n - hop,]
+                - processed_x[block_size - hop : n - hop,]
             )
         )
 
     else:
-
         n = 0
         hop_frames = hop * num_frames
         # process the signals while full blocks are available
         while x_local.shape[0] - n > hop_frames:
-            stft.analysis(
-                x_local[
-                    n : n + hop_frames,
-                ]
-            )
-            processed_x[
-                n : n + hop_frames,
-            ] = stft.synthesis()
+            stft.analysis(x_local[n : n + hop_frames,])
+            processed_x[n : n + hop_frames,] = stft.synthesis()
             n += hop_frames
 
-        error = np.max(
-            np.abs(
-                x_local[
-                    : n - hop,
-                ]
-                - processed_x[
-                    hop:n,
-                ]
-            )
-        )
+        error = np.max(np.abs(x_local[: n - hop,] - processed_x[hop:n,]))
 
     return error
 
 
 def with_half_overlap_with_filter(D, num_frames=1, fixed_memory=False, streaming=True):
     """
     D             - number of channels
@@ -462,17 +377,15 @@
 
     # parameters
     block_size = 512 - h_len + 1  # make sure the FFT size is a power of 2
     hop = block_size // 2  # half overlap
     window = pra.hann(block_size)  # the analysis window
     if not streaming:
         num_samples = (num_frames - 1) * hop + block_size
-        x_local = x_local[
-            :num_samples,
-        ]
+        x_local = x_local[:num_samples,]
 
     # Create the STFT object
     if fixed_memory:
         stft = STFT(
             block_size,
             hop=hop,
             channels=D,
@@ -494,71 +407,49 @@
     # setup the filter
     stft.set_filter(h_local, zb=h_len - 1)
 
     # collect the processed blocks
     processed_x = np.zeros(x_local.shape)
 
     if not streaming:
-
         stft.analysis(x_local)
         stft.process()
         processed_x = stft.synthesis()
         n = processed_x.shape[0]
 
         error = np.max(
             np.abs(
-                y_local[
-                    block_size : n - block_size,
-                ]
-                - processed_x[
-                    block_size : n - block_size,
-                ]
+                y_local[block_size : n - block_size,]
+                - processed_x[block_size : n - block_size,]
             )
         )
 
     else:
-
         n = 0
         hop_frames = hop * num_frames
         # process the signals while full blocks are available
         while x_local.shape[0] - n > hop_frames:
-            stft.analysis(
-                x_local[
-                    n : n + hop_frames,
-                ]
-            )
+            stft.analysis(x_local[n : n + hop_frames,])
             stft.process()  # apply the filter
-            processed_x[
-                n : n + hop_frames,
-            ] = stft.synthesis()
+            processed_x[n : n + hop_frames,] = stft.synthesis()
             n += hop_frames
 
-        error = np.max(
-            np.abs(
-                y_local[
-                    : n - hop,
-                ]
-                - processed_x[
-                    hop:n,
-                ]
-            )
-        )
+        error = np.max(np.abs(y_local[: n - hop,] - processed_x[hop:n,]))
 
         # if D==1:
         #     import matplotlib.pyplot as plt
         #     plt.figure()
         #     plt.plot(y_local)
         #     plt.plot(processed_x)
         #     plt.show()
 
     return error
 
 
 def call_all_stft_tests(num_frames=1, fixed_memory=False, streaming=True, overlap=True):
-
     error = no_overlap_no_filter(1, num_frames, fixed_memory, streaming)
     print("no overlap, no filter, mono             : %0.0f dB" % (20 * np.log10(error)))
 
     error = no_overlap_no_filter(D, num_frames, fixed_memory, streaming)
     print("no overlap, no filter, multichannel     : %0.0f dB" % (20 * np.log10(error)))
 
     error = no_overlap_with_filter(1, num_frames, fixed_memory, streaming)
@@ -997,15 +888,14 @@
             error = with_arbitrary_overlap_synthesis_window(
                 1, num_frames=50, fixed_memory=True, streaming=False, overlap=overlap
             )
             self.assertTrue(error < tol)
 
 
 if __name__ == "__main__":
-
     print()
     print("TEST INFO")
     print("-------------------------------------------------------------")
     print("Max error in dB for randomly generated signal of %d samples." % len(x))
     print("Multichannel corresponds to %d channels." % D)
     print("-------------------------------------------------------------")
     print()
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/transform/tests/test_stft_oneshot.py` & `pyroomacoustics-0.7.4/pyroomacoustics/transform/tests/test_stft_oneshot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from __future__ import division, print_function
+
 from unittest import TestCase
+
 import numpy as np
+
 import pyroomacoustics as pra
 from pyroomacoustics.transform import stft
 
-
 # test parameters
 tol = -100  # dB
 np.random.seed(0)
 D = 3
 block_size = 512
 
 # test signal (noise)
 x = np.random.randn(block_size * 20, D).astype(np.float32)
 
 
 def no_overlap(D):
-
     if D == 1:
         x_local = x[:, 0]
     else:
         x_local = x[:, :D]
 
     hop = block_size
 
@@ -30,15 +31,14 @@
     # synthesis
     x_r = stft.synthesis(X, L=block_size, hop=hop)
 
     return pra.dB(np.max(np.abs(x_local - x_r)))
 
 
 def half_overlap(D):
-
     if D == 1:
         x_local = x[:, 0]
     else:
         x_local = x[:, :D]
 
     hop = block_size // 2
 
@@ -46,24 +46,15 @@
     analysis_win = pra.hann(block_size)
     X = stft.analysis(x_local, L=block_size, hop=hop, win=analysis_win)
 
     # synthesis
     x_r = stft.synthesis(X, L=block_size, hop=hop)
 
     return pra.dB(
-        np.max(
-            np.abs(
-                x_local[
-                    : -block_size + hop,
-                ]
-                - x_r[
-                    block_size - hop :,
-                ]
-            )
-        )
+        np.max(np.abs(x_local[: -block_size + hop,] - x_r[block_size - hop :,]))
     )
 
 
 def append_one_sample(D):
     hop = block_size // 2
     n_samples = x.shape[0]
     n_frames = n_samples // hop
@@ -78,29 +69,19 @@
     analysis_win = pra.hann(block_size)
     X = stft.analysis(x_local, L=block_size, hop=hop, win=analysis_win)
 
     # synthesis
     x_r = stft.synthesis(X, L=block_size, hop=hop)
 
     return pra.dB(
-        np.max(
-            np.abs(
-                x_local[
-                    : -block_size + hop,
-                ]
-                - x_r[
-                    block_size - hop : -1,
-                ]
-            )
-        )
+        np.max(np.abs(x_local[: -block_size + hop,] - x_r[block_size - hop : -1,]))
     )
 
 
 def hop_one_sample(D):
-
     if D == 1:
         x_local = x[:, 0]
     else:
         x_local = x[:, :D]
 
     hop = 1
 
@@ -109,24 +90,15 @@
     X = stft.analysis(x_local, L=block_size, hop=hop, win=analysis_win)
 
     # synthesis
     synthesis_win = pra.transform.stft.compute_synthesis_window(analysis_win, hop)
     x_r = stft.synthesis(X, L=block_size, hop=hop, win=synthesis_win)
 
     return pra.dB(
-        np.max(
-            np.abs(
-                x_local[
-                    : -block_size + hop,
-                ]
-                - x_r[
-                    block_size - hop :,
-                ]
-            )
-        )
+        np.max(np.abs(x_local[: -block_size + hop,] - x_r[block_size - hop :,]))
     )
 
 
 class TestSTFTOneShot(TestCase):
     def test_no_overlap(self):
         self.assertTrue(no_overlap(1) < tol)
         self.assertTrue(no_overlap(D) < tol)
@@ -141,15 +113,14 @@
 
     def test_hop_one_sample(self):
         self.assertTrue(hop_one_sample(1) < tol)
         self.assertTrue(hop_one_sample(D) < tol)
 
 
 if __name__ == "__main__":
-
     print()
     print("TEST INFO")
     print("-------------------------------------------------------------")
     print("Max error in dB for randomly generated signal of %d samples." % len(x))
     print("Multichannel corresponds to %d channels." % D)
     print("-------------------------------------------------------------")
     print()
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/transform/tests/test_stft_timing.py` & `pyroomacoustics-0.7.4/pyroomacoustics/transform/tests/test_stft_timing.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import division, print_function
 
+import time
+import warnings
+
 import numpy as np
+
 import pyroomacoustics as pra
 from pyroomacoustics.transform import STFT
-import time
-import warnings
 
 # test signal
 np.random.seed(0)
 num_mic = 25
 signals = np.random.randn(100000, num_mic).astype(np.float32)
 fs = 16000
 
@@ -30,97 +32,60 @@
 )
 print()
 print("----- SINGLE FRAME AT A TIME -----")
 print("With STFT object (not fixed) : ", end="")
 stft = STFT(block_size, hop=hop, channels=num_mic, streaming=True, analysis_window=win)
 start = time.time()
 for k in range(num_times):
-
     x_r = np.zeros(signals.shape)
     n = 0
     while signals.shape[0] - n > hop:
-        stft.analysis(
-            signals[
-                n : n + hop,
-            ]
-        )
-        x_r[
-            n : n + hop,
-        ] = stft.synthesis()
+        stft.analysis(signals[n : n + hop,])
+        x_r[n : n + hop,] = stft.synthesis()
         n += hop
 avg_time = (time.time() - start) / num_times
 print("%0.3f sec" % avg_time)
-err_dB = 20 * np.log10(
-    np.max(
-        np.abs(
-            signals[
-                : n - hop,
-            ]
-            - x_r[
-                hop:n,
-            ]
-        )
-    )
-)
+err_dB = 20 * np.log10(np.max(np.abs(signals[: n - hop,] - x_r[hop:n,])))
 print("Error [dB] : %0.3f" % err_dB)
 
 
 print("With STFT object (fixed) : ", end="")
 stft = STFT(
     block_size,
     hop=hop,
     channels=num_mic,
     num_frames=1,
     streaming=True,
     analysis_window=win,
 )
 start = time.time()
 for k in range(num_times):
-
     x_r = np.zeros(signals.shape)
     n = 0
     while signals.shape[0] - n > hop:
-        stft.analysis(
-            signals[
-                n : n + hop,
-            ]
-        )
-        x_r[
-            n : n + hop,
-        ] = stft.synthesis()
+        stft.analysis(signals[n : n + hop,])
+        x_r[n : n + hop,] = stft.synthesis()
         n += hop
 avg_time = (time.time() - start) / num_times
 print("%0.3f sec" % avg_time)
-err_dB = 20 * np.log10(
-    np.max(
-        np.abs(
-            signals[
-                : n - hop,
-            ]
-            - x_r[
-                hop:n,
-            ]
-        )
-    )
-)
+err_dB = 20 * np.log10(np.max(np.abs(signals[: n - hop,] - x_r[hop:n,])))
 print("Error [dB] : %0.3f" % err_dB)
 
 
 """
 Multiple frame at a time (non-streaming)
 """
 print()
 print("----- MULTIPLE FRAMES AT A TIME -----")
 
 warnings.filterwarnings("ignore")  # to avoid warning of appending zeros to be printed
 print("With STFT object (not fixed) : ", end="")
 stft = STFT(block_size, hop=hop, channels=num_mic, analysis_window=win, streaming=False)
 start = time.time()
 for k in range(num_times):
-
     stft.analysis(signals)
     x_r = stft.synthesis()
 
 avg_time = (time.time() - start) / num_times
 print("%0.3f sec" % avg_time)
 err_dB = 20 * np.log10(
     np.max(np.abs(signals[hop : len(x_r) - hop] - x_r[hop : len(x_r) - hop]))
@@ -137,15 +102,14 @@
     channels=num_mic,
     num_frames=num_frames,
     analysis_window=win,
     streaming=False,
 )
 start = time.time()
 for k in range(num_times):
-
     stft.analysis(signals[: (num_frames - 1) * hop + block_size, :])
     x_r = stft.synthesis()
 avg_time = (time.time() - start) / num_times
 print("%0.3f sec" % avg_time)
 err_dB = 20 * np.log10(
     np.max(np.abs(signals[hop : len(x_r) - hop] - x_r[hop : len(x_r) - hop]))
 )
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/utilities.py` & `pyroomacoustics-0.7.4/pyroomacoustics/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 import itertools
 
 import numpy as np
 from scipy import signal
 from scipy.io import wavfile
 
+from .doa import cart2spher
 from .parameters import constants, eps
 from .sync import correlate
 
 
 def requires_matplotlib(func):
     def function_wrapper(*args, **kwargs):
         try:
@@ -306,15 +307,14 @@
     plt.setp(plt.gca(), "yticks", yticks)
     plt.setp(plt.gca(), "yticklabels", yticklabels)
 
     plt.setp(plt.getp(plt.gca(), "ygridlines"), "ls", "--")
 
 
 def spectrum(signal, Fs, N):
-
     from .stft import spectroplot, stft
     from .windows import hann
 
     F = stft(signal, N, N / 2, win=hann(N))
     spectroplot(F.T, N, N / 2, Fs)
 
 
@@ -331,15 +331,14 @@
     Fs,
     fft_size=512,
     norm=False,
     equal=False,
     title1=None,
     title2=None,
 ):
-
     try:
         import matplotlib.pyplot as plt
     except ImportError:
         import warnings
 
         warnings.warn("Matplotlib is required for plotting")
         return
@@ -407,15 +406,14 @@
         vmax=vmax,
         cmap=plt.get_cmap(cmap),
         interpolation=interpolation,
     )
 
 
 def real_spectrum(signal, axis=-1, **kwargs):
-
     try:
         import matplotlib.pyplot as plt
     except ImportError:
         import warnings
 
         warnings.warn("Matplotlib is required for plotting")
         return
@@ -561,14 +559,17 @@
     -------
     numpy array
         A fractional delay filter with specified delay.
     """
 
     N = constants.get("frac_delay_length")
 
+    if isinstance(t0, np.ndarray) and t0.ndim == 1:
+        t0 = t0[:, None]
+
     return np.hanning(N) * np.sinc(np.arange(N) - (N - 1) / 2 - t0)
 
 
 def fractional_delay_filter_bank(delays):
     """
     Creates a fractional delay filter bank of windowed sinc filters
 
@@ -647,28 +648,22 @@
             0,
         ]
         / r[0]
     )
     epsilon = r[0]
 
     for j in np.arange(1, p):
-
         g = np.sum(np.conj(r[1 : j + 1]) * a[::-1])
         gamma = -g / epsilon
         a = np.concatenate((a, np.zeros(1))) + gamma * np.concatenate(
             (np.zeros(1), np.conj(a[::-1]))
         )
         epsilon = epsilon * (1 - np.abs(gamma) ** 2)
         delta = np.dot(np.conj(r[1 : j + 1]), np.flipud(x))
-        q = (
-            b[
-                j,
-            ]
-            - delta
-        ) / epsilon
+        q = (b[j] - delta) / epsilon
         if len(b.shape) == 1:
             x = np.concatenate((x, np.zeros(1))) + q * np.conj(a[::-1])
         else:
             x = np.concatenate((x, np.zeros((1, b.shape[1]))), axis=0) + q * np.conj(
                 a[::-1, np.newaxis]
             )
 
@@ -776,55 +771,48 @@
 """
 GEOMETRY UTILITIES
 """
 
 
 def angle_function(s1, v2):
     """
-    Compute azimuth and colatitude angles in radians for a given set of points `s1` and a singular point `v2`.
+    Compute azimuth and colatitude angles in radians for a given set of points `s1`
+    with respect to a reference point `v2`.
 
     Parameters
     -----------
     s1 : numpy array
         3×N for a set of N 3-D points, 2×N for a set of N 2-D points.
     v2 : numpy array
         3×1 for a 3-D point, 2×1 for a 2-D point.
 
     Returns
     -----------
     numpy array
-        2×N numpy array with azimuth and colatitude angles in radians.
-
+        2×N numpy array with azimuth and colatitude angles in radians in the
+        first and second row, respectively.
+        If the input vectors are 2-D, the colatitude is always fixed to pi/2.
     """
 
     if len(s1.shape) == 1:
         s1 = s1[:, np.newaxis]
     if len(v2.shape) == 1:
         v2 = v2[:, np.newaxis]
 
     assert s1.shape[0] == v2.shape[0]
 
-    x_vals = s1[0]
-    y_vals = s1[1]
-    x2 = v2[0]
-    y2 = v2[1]
-
-    # colatitude calculation for 3-D coordinates
-    if s1.shape[0] == 3 and v2.shape[0] == 3:
-
-        z2 = v2[2]
-        z_vals = s1[2]
-
-        colatitude = np.arctan2(
-            ((x_vals - x2) ** 2 + (y_vals - y2) ** 2) ** 1 / 2, (z_vals - z2)
-        )
-
-    # colatitude calculation for 2-D coordinates
-    elif s1.shape[0] == 2 and v2.shape[0] == 2:
-
-        num_points = s1.shape[1]
-        colatitude = np.ones(num_points) * np.pi / 2
-
-    # azimuth calculation (same for 2-D and 3-D)
-    azimuth = np.arctan2((y_vals - y2), (x_vals - x2))
+    ndim = s1.shape[0]
+    if ndim == 2:
+        s1 = np.concatenate((s1, np.zeros((1, s1.shape[1]))), axis=0)
+        v2 = np.concatenate((v2, np.zeros((1, v2.shape[1]))), axis=0)
+
+    # this is slightly wasteful for 2d points, but is safer as we are relying
+    # on tried and tested code
+    az, co, r = cart2spher(s1 - v2)
+
+    if ndim == 2:
+        # this is only necessary to handle correctly the case s1 - v2 = 0
+        # in this case cart2spher returns zero, but we would like to have
+        # colatitude = pi/2 for consistency
+        co[:] = np.pi / 2
 
-    return np.vstack((azimuth, colatitude))
+    return np.vstack((az, co))
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics/windows.py` & `pyroomacoustics-0.7.4/pyroomacoustics/windows.py`

 * *Files identical despite different names*

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics.egg-info/PKG-INFO` & `pyroomacoustics-0.7.4/pyroomacoustics.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: pyroomacoustics
-Version: 0.7.3
+Version: 0.7.4
 Summary: A simple framework for room acoustics and audio processing in Python.
 Home-page: https://github.com/LCAV/pyroomacoustics
 Author: Laboratory for Audiovisual Communications, EPFL
 Author-email: fakufaku@gmail.ch
 License: MIT
 Keywords: room acoustics signal processing doa beamforming adaptive
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: Cython
+Requires-Dist: numpy>=1.13.0
+Requires-Dist: scipy>=0.18.0
+Requires-Dist: pybind11>=2.2
 
 .. image:: https://github.com/LCAV/pyroomacoustics/raw/master/logo/pyroomacoustics_logo_horizontal.png
-   :scale: 80 %
    :alt: Pyroomacoustics logo
    :align: left
 
 ------------------------------------------------------------------------------
 
-.. image:: https://travis-ci.org/LCAV/pyroomacoustics.svg?branch=pypi-release
-    :target: https://travis-ci.org/LCAV/pyroomacoustics
 .. image:: https://readthedocs.org/projects/pyroomacoustics/badge/?version=pypi-release
     :target: http://pyroomacoustics.readthedocs.io/en/pypi-release/
     :alt: Documentation Status
 .. image:: https://mybinder.org/badge_logo.svg
     :target: https://mybinder.org/v2/gh/LCAV/pyroomacoustics/master?filepath=notebooks%2Fpyroomacoustics_demo.ipynb
     :alt: Test on mybinder
 .. image:: https://img.shields.io/discord/829534160812245012?color=%237289DA&label=pyroomacoustics%20Discord&logo=discord&logoColor=white
@@ -240,14 +240,19 @@
 
 A couple of `detailed demos with illustrations <https://github.com/LCAV/pyroomacoustics/tree/master/notebooks>`_ are available.  
 
 A comprehensive set of examples covering most of the functionalities
 of the package can be found in the ``examples`` folder of the `GitHub
 repository <https://github.com/LCAV/pyroomacoustics/tree/master/examples>`_.
 
+A `video introduction to pyroomacoustics <https://www.youtube.com/watch?v=c3DTtc--_F4>`_.
+
+A `video tutorial series on using pyroomacoustics <https://youtube.com/playlist?list=PL6QnpHKwdPYgxLV_Ijr6K_3Gdyfhk0SHg&si=gsSuUm9Yw2_sjYhr>`_
+covering many advanced topics.
+
 Authors
 -------
 
 * Robin Scheibler
 * Ivan Dokmanić
 * Sidney Barthe
 * Eric Bezzam
```

### Comparing `pyroomacoustics-0.7.3/pyroomacoustics.egg-info/SOURCES.txt` & `pyroomacoustics-0.7.4/pyroomacoustics.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -85,16 +85,19 @@
 pyroomacoustics/experimental/tests/test_deconvolution.py
 pyroomacoustics/experimental/tests/test_measure_rt60.py
 pyroomacoustics/libroom_src/common.hpp
 pyroomacoustics/libroom_src/geometry.cpp
 pyroomacoustics/libroom_src/geometry.hpp
 pyroomacoustics/libroom_src/libroom.cpp
 pyroomacoustics/libroom_src/microphone.hpp
+pyroomacoustics/libroom_src/rir_builder.cpp
+pyroomacoustics/libroom_src/rir_builder.hpp
 pyroomacoustics/libroom_src/room.cpp
 pyroomacoustics/libroom_src/room.hpp
+pyroomacoustics/libroom_src/threadpool.hpp
 pyroomacoustics/libroom_src/wall.cpp
 pyroomacoustics/libroom_src/wall.hpp
 pyroomacoustics/libroom_src/ext/eigen/COPYING.BSD
 pyroomacoustics/libroom_src/ext/eigen/COPYING.GPL
 pyroomacoustics/libroom_src/ext/eigen/COPYING.LGPL
 pyroomacoustics/libroom_src/ext/eigen/COPYING.MINPACK
 pyroomacoustics/libroom_src/ext/eigen/COPYING.MPL2
@@ -399,14 +402,15 @@
 pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/BlockMethods.h
 pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h
 pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h
 pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h
 pyroomacoustics/libroom_src/ext/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h
 pyroomacoustics/phase/__init__.py
 pyroomacoustics/phase/gl.py
+pyroomacoustics/tests/test_air_absorption.py
 pyroomacoustics/tests/test_anechoic_room.py
 pyroomacoustics/tests/test_angle_function.py
 pyroomacoustics/tests/test_autocorr.py
 pyroomacoustics/tests/test_bandpass_filterbank.py
 pyroomacoustics/tests/test_build_rir.py
 pyroomacoustics/tests/test_create_noisy_signal.py
 pyroomacoustics/tests/test_issue_115.py
```

### Comparing `pyroomacoustics-0.7.3/setup.py` & `pyroomacoustics-0.7.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,21 +47,24 @@
         "room.cpp",
         "wall.hpp",
         "wall.cpp",
         "microphone.hpp",
         "geometry.hpp",
         "geometry.cpp",
         "common.hpp",
+        "rir_builder.cpp",
+        "rir_builder.hpp",
         "libroom.cpp",
+        "threadpool.hpp",
     ]
 ]
 ext_modules = [
     Extension(
         "pyroomacoustics.libroom",
-        [os.path.join(libroom_src_dir, f) for f in ["libroom.cpp"]],
+        [os.path.join(libroom_src_dir, f) for f in ["libroom.cpp", "rir_builder.cpp"]],
         depends=libroom_files,
         include_dirs=[
             ".",
             libroom_src_dir,
             str(get_pybind_include()),
             str(get_pybind_include(user=True)),
             os.path.join(libroom_src_dir, "ext/eigen"),
@@ -82,14 +85,15 @@
 # Get the long description from the README file
 with open(path.join(here, "README.rst"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 ### Build Tools (taken from pybind11 example) ###
 
+
 # As of Python 3.6, CCompiler has a `has_flag` method.
 # cf http://bugs.python.org/issue26689
 def has_flag(compiler, flagname):
     """Return a boolean indicating whether a flag name is supported on
     the specified compiler.
     """
     import tempfile
@@ -180,16 +184,16 @@
         "Cython",
         "numpy>=1.13.0",
         "scipy>=0.18.0",
         "pybind11>=2.2",
     ],
     cmdclass={"build_ext": BuildExt},  # taken from pybind11 example
     zip_safe=False,
-    test_suite="nose.collector",
-    tests_require=["nose"],
+    test_suite="pytest",
+    tests_require=["pytest"],
     classifiers=[
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
         "Development Status :: 4 - Beta",
         # Indicate who your project is intended for
@@ -199,21 +203,18 @@
         "Topic :: Scientific/Engineering :: Physics",
         "Topic :: Multimedia :: Sound/Audio :: Speech",
         "Topic :: Multimedia :: Sound/Audio :: Analysis",
         # Pick your license as you wish (should match "license" above)
         "License :: OSI Approved :: MIT License",
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3",
-        #'Programming Language :: Python :: 3.3',
-        #'Programming Language :: Python :: 3.4',
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     # What does your project relate to?
     keywords="room acoustics signal processing doa beamforming adaptive",
 )
 
 setup(**setup_kwargs)
```


# Comparing `tmp/grss-4.0.0.tar.gz` & `tmp/grss-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grss-4.0.0.tar", last modified: Tue Apr 23 21:22:35 2024, max compression
+gzip compressed data, was "grss-4.0.1.tar", last modified: Thu Apr 25 18:14:55 2024, max compression
```

## Comparing `grss-4.0.0.tar` & `grss-4.0.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 21:22:35.652078 grss-4.0.0/
--rw-r--r--   0 runner     (501) staff       (20)     1909 2024-04-23 21:21:50.000000 grss-4.0.0/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     1070 2024-04-23 21:21:50.000000 grss-4.0.0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      192 2024-04-23 21:21:50.000000 grss-4.0.0/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     7681 2024-04-23 21:22:35.651754 grss-4.0.0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     4744 2024-04-23 21:21:50.000000 grss-4.0.0/README.md
--rwxr-xr-x   0 runner     (501) staff       (20)      590 2024-04-23 21:21:50.000000 grss-4.0.0/build_cpp.sh
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 21:22:35.610241 grss-4.0.0/docs/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 21:22:35.612868 grss-4.0.0/docs/source/
--rw-r--r--   0 runner     (501) staff       (20)     3688 2024-04-23 21:21:50.000000 grss-4.0.0/docs/source/conf.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 21:22:35.613348 grss-4.0.0/extern/
--rw-r--r--   0 runner     (501) staff       (20)    12707 2024-04-23 21:21:50.000000 grss-4.0.0/extern/get_cspice.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 21:22:35.614195 grss-4.0.0/grss/
--rw-r--r--   0 runner     (501) staff       (20)      266 2024-04-23 21:21:50.000000 grss-4.0.0/grss/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 21:22:35.614976 grss-4.0.0/grss/debias/
--rw-r--r--   0 runner     (501) staff       (20)     1589 2024-04-23 21:21:50.000000 grss-4.0.0/grss/debias/get_debiasing_data.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 21:22:35.618105 grss-4.0.0/grss/fit/
--rw-r--r--   0 runner     (501) staff       (20)      259 2024-04-23 21:21:50.000000 grss-4.0.0/grss/fit/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3211 2024-04-23 21:21:50.000000 grss-4.0.0/grss/fit/fit_ades.py
--rw-r--r--   0 runner     (501) staff       (20)    38504 2024-04-23 21:21:50.000000 grss-4.0.0/grss/fit/fit_optical.py
--rw-r--r--   0 runner     (501) staff       (20)     4085 2024-04-23 21:21:50.000000 grss-4.0.0/grss/fit/fit_radar.py
--rw-r--r--   0 runner     (501) staff       (20)    85476 2024-04-23 21:21:50.000000 grss-4.0.0/grss/fit/fit_simulation.py
--rw-r--r--   0 runner     (501) staff       (20)    19123 2024-04-23 21:21:50.000000 grss-4.0.0/grss/fit/fit_utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 21:22:35.619304 grss-4.0.0/grss/kernels/
--rw-r--r--   0 runner     (501) staff       (20)     3121 2024-04-23 21:21:50.000000 grss-4.0.0/grss/kernels/get_kernels.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 21:22:35.620590 grss-4.0.0/grss/prop/
--rw-r--r--   0 runner     (501) staff       (20)      156 2024-04-23 21:21:50.000000 grss-4.0.0/grss/prop/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    13650 2024-04-23 21:21:50.000000 grss-4.0.0/grss/prop/prop_parallel.py
--rw-r--r--   0 runner     (501) staff       (20)     6076 2024-04-23 21:21:50.000000 grss-4.0.0/grss/prop/prop_unscented.py
--rw-r--r--   0 runner     (501) staff       (20)    34211 2024-04-23 21:21:50.000000 grss-4.0.0/grss/prop/prop_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2612 2024-04-23 21:21:50.000000 grss-4.0.0/grss/utils.py
--rw-r--r--   0 runner     (501) staff       (20)        5 2024-04-23 21:21:50.000000 grss-4.0.0/grss/version.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 21:22:35.651359 grss-4.0.0/grss.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     7681 2024-04-23 21:22:35.000000 grss-4.0.0/grss.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1499 2024-04-23 21:22:35.000000 grss-4.0.0/grss.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-23 21:22:35.000000 grss-4.0.0/grss.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)      163 2024-04-23 21:22:35.000000 grss-4.0.0/grss.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       53 2024-04-23 21:22:35.000000 grss-4.0.0/grss.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 21:22:35.625147 grss-4.0.0/include/
--rw-r--r--   0 runner     (501) staff       (20)     1502 2024-04-23 21:21:50.000000 grss-4.0.0/include/approach.h
--rw-r--r--   0 runner     (501) staff       (20)     3334 2024-04-23 21:21:50.000000 grss-4.0.0/include/elements.h
--rw-r--r--   0 runner     (501) staff       (20)     1669 2024-04-23 21:21:50.000000 grss-4.0.0/include/force.h
--rw-r--r--   0 runner     (501) staff       (20)     4577 2024-04-23 21:21:50.000000 grss-4.0.0/include/gr15.h
--rw-r--r--   0 runner     (501) staff       (20)     1464 2024-04-23 21:21:50.000000 grss-4.0.0/include/grss.h
--rw-r--r--   0 runner     (501) staff       (20)     6190 2024-04-23 21:21:50.000000 grss-4.0.0/include/interpolate.h
--rw-r--r--   0 runner     (501) staff       (20)      356 2024-04-23 21:21:50.000000 grss-4.0.0/include/parallel.h
--rw-r--r--   0 runner     (501) staff       (20)     2714 2024-04-23 21:21:50.000000 grss-4.0.0/include/pck.h
--rw-r--r--   0 runner     (501) staff       (20)    19128 2024-04-23 21:21:50.000000 grss-4.0.0/include/simulation.h
--rw-r--r--   0 runner     (501) staff       (20)     3804 2024-04-23 21:21:50.000000 grss-4.0.0/include/spk.h
--rw-r--r--   0 runner     (501) staff       (20)     2685 2024-04-23 21:21:50.000000 grss-4.0.0/include/stm.h
--rw-r--r--   0 runner     (501) staff       (20)     1812 2024-04-23 21:21:50.000000 grss-4.0.0/include/timeconvert.h
--rw-r--r--   0 runner     (501) staff       (20)     5462 2024-04-23 21:21:50.000000 grss-4.0.0/include/utilities.h
--rw-r--r--   0 runner     (501) staff       (20)     2114 2024-04-23 21:21:50.000000 grss-4.0.0/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)      163 2024-04-23 21:21:50.000000 grss-4.0.0/requirements.txt
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-23 21:22:35.652139 grss-4.0.0/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1740 2024-04-23 21:21:50.000000 grss-4.0.0/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 21:22:35.633691 grss-4.0.0/src/
--rw-r--r--   0 runner     (501) staff       (20)      283 2024-04-23 21:21:50.000000 grss-4.0.0/src/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    31500 2024-04-23 21:21:50.000000 grss-4.0.0/src/approach.cpp
--rw-r--r--   0 runner     (501) staff       (20)    26087 2024-04-23 21:21:50.000000 grss-4.0.0/src/elements.cpp
--rw-r--r--   0 runner     (501) staff       (20)    29546 2024-04-23 21:21:50.000000 grss-4.0.0/src/force.cpp
--rw-r--r--   0 runner     (501) staff       (20)    20530 2024-04-23 21:21:50.000000 grss-4.0.0/src/gr15.cpp
--rw-r--r--   0 runner     (501) staff       (20)    45888 2024-04-23 21:21:50.000000 grss-4.0.0/src/grss.cpp
--rw-r--r--   0 runner     (501) staff       (20)    44803 2024-04-23 21:21:50.000000 grss-4.0.0/src/interpolate.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2722 2024-04-23 21:21:50.000000 grss-4.0.0/src/parallel.cpp
--rw-r--r--   0 runner     (501) staff       (20)    35824 2024-04-23 21:21:50.000000 grss-4.0.0/src/pck.cpp
--rw-r--r--   0 runner     (501) staff       (20)    68054 2024-04-23 21:21:50.000000 grss-4.0.0/src/simulation.cpp
--rw-r--r--   0 runner     (501) staff       (20)    15260 2024-04-23 21:21:50.000000 grss-4.0.0/src/spk.cpp
--rw-r--r--   0 runner     (501) staff       (20)    24181 2024-04-23 21:21:50.000000 grss-4.0.0/src/stm.cpp
--rw-r--r--   0 runner     (501) staff       (20)     6951 2024-04-23 21:21:50.000000 grss-4.0.0/src/timeconvert.cpp
--rw-r--r--   0 runner     (501) staff       (20)    12536 2024-04-23 21:21:50.000000 grss-4.0.0/src/utilities.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 21:22:35.611117 grss-4.0.0/tests/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 21:22:35.611053 grss-4.0.0/tests/cpp/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 21:22:35.635115 grss-4.0.0/tests/cpp/prop/
--rw-r--r--   0 runner     (501) staff       (20)      797 2024-04-23 21:21:50.000000 grss-4.0.0/tests/cpp/prop/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     3725 2024-04-23 21:21:50.000000 grss-4.0.0/tests/cpp/prop/apophis.cpp
--rw-r--r--   0 runner     (501) staff       (20)     5981 2024-04-23 21:21:50.000000 grss-4.0.0/tests/cpp/prop/didymos.cpp
--rw-r--r--   0 runner     (501) staff       (20)     3449 2024-04-23 21:21:50.000000 grss-4.0.0/tests/cpp/prop/pck_map.cpp
--rw-r--r--   0 runner     (501) staff       (20)     5917 2024-04-23 21:21:50.000000 grss-4.0.0/tests/cpp/prop/spk_map.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 21:22:35.635374 grss-4.0.0/tests/python/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 21:22:35.645175 grss-4.0.0/tests/python/fit/
--rw-r--r--   0 runner     (501) staff       (20)   743881 2024-04-23 21:21:50.000000 grss-4.0.0/tests/python/fit/chesley.ipynb
--rw-r--r--   0 runner     (501) staff       (20)   701963 2024-04-23 21:21:50.000000 grss-4.0.0/tests/python/fit/eggl.ipynb
--rw-r--r--   0 runner     (501) staff       (20)   635614 2024-04-23 21:21:50.000000 grss-4.0.0/tests/python/fit/farnocchia.ipynb
--rw-r--r--   0 runner     (501) staff       (20)   666353 2024-04-23 21:21:50.000000 grss-4.0.0/tests/python/fit/shantanunaidu.ipynb
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-23 21:22:35.650922 grss-4.0.0/tests/python/prop/
--rw-r--r--   0 runner     (501) staff       (20)   104846 2024-04-23 21:21:50.000000 grss-4.0.0/tests/python/prop/apophis.ipynb
--rw-r--r--   0 runner     (501) staff       (20)   102230 2024-04-23 21:21:50.000000 grss-4.0.0/tests/python/prop/didymos.ipynb
--rw-r--r--   0 runner     (501) staff       (20)   116221 2024-04-23 21:21:50.000000 grss-4.0.0/tests/python/prop/icarus.ipynb
--rw-r--r--   0 runner     (501) staff       (20)    77629 2024-04-23 21:21:50.000000 grss-4.0.0/tests/python/prop/moshup.ipynb
--rwxr-xr-x   0 runner     (501) staff       (20)      269 2024-04-23 21:21:50.000000 grss-4.0.0/tests/python/run_tests.sh
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.227516 grss-4.0.1/
+-rw-r--r--   0 runner     (501) staff       (20)     1909 2024-04-25 18:14:08.000000 grss-4.0.1/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1070 2024-04-25 18:14:08.000000 grss-4.0.1/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      192 2024-04-25 18:14:08.000000 grss-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     7681 2024-04-25 18:14:55.227242 grss-4.0.1/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     4744 2024-04-25 18:14:08.000000 grss-4.0.1/README.md
+-rwxr-xr-x   0 runner     (501) staff       (20)      590 2024-04-25 18:14:08.000000 grss-4.0.1/build_cpp.sh
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.184273 grss-4.0.1/docs/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.187110 grss-4.0.1/docs/source/
+-rw-r--r--   0 runner     (501) staff       (20)     3688 2024-04-25 18:14:08.000000 grss-4.0.1/docs/source/conf.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.187552 grss-4.0.1/extern/
+-rw-r--r--   0 runner     (501) staff       (20)    12707 2024-04-25 18:14:08.000000 grss-4.0.1/extern/get_cspice.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.188795 grss-4.0.1/grss/
+-rw-r--r--   0 runner     (501) staff       (20)      249 2024-04-25 18:14:08.000000 grss-4.0.1/grss/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.189616 grss-4.0.1/grss/debias/
+-rw-r--r--   0 runner     (501) staff       (20)     1589 2024-04-25 18:14:08.000000 grss-4.0.1/grss/debias/get_debiasing_data.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.192958 grss-4.0.1/grss/fit/
+-rw-r--r--   0 runner     (501) staff       (20)      259 2024-04-25 18:14:08.000000 grss-4.0.1/grss/fit/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3211 2024-04-25 18:14:08.000000 grss-4.0.1/grss/fit/fit_ades.py
+-rw-r--r--   0 runner     (501) staff       (20)    38604 2024-04-25 18:14:08.000000 grss-4.0.1/grss/fit/fit_optical.py
+-rw-r--r--   0 runner     (501) staff       (20)     4085 2024-04-25 18:14:08.000000 grss-4.0.1/grss/fit/fit_radar.py
+-rw-r--r--   0 runner     (501) staff       (20)    85476 2024-04-25 18:14:08.000000 grss-4.0.1/grss/fit/fit_simulation.py
+-rw-r--r--   0 runner     (501) staff       (20)    19123 2024-04-25 18:14:08.000000 grss-4.0.1/grss/fit/fit_utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.193315 grss-4.0.1/grss/kernels/
+-rw-r--r--   0 runner     (501) staff       (20)     3121 2024-04-25 18:14:08.000000 grss-4.0.1/grss/kernels/get_kernels.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.194553 grss-4.0.1/grss/prop/
+-rw-r--r--   0 runner     (501) staff       (20)      156 2024-04-25 18:14:08.000000 grss-4.0.1/grss/prop/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    13716 2024-04-25 18:14:08.000000 grss-4.0.1/grss/prop/prop_parallel.py
+-rw-r--r--   0 runner     (501) staff       (20)     6076 2024-04-25 18:14:08.000000 grss-4.0.1/grss/prop/prop_unscented.py
+-rw-r--r--   0 runner     (501) staff       (20)    34546 2024-04-25 18:14:08.000000 grss-4.0.1/grss/prop/prop_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2612 2024-04-25 18:14:08.000000 grss-4.0.1/grss/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)        5 2024-04-25 18:14:08.000000 grss-4.0.1/grss/version.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.226914 grss-4.0.1/grss.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     7681 2024-04-25 18:14:55.000000 grss-4.0.1/grss.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1499 2024-04-25 18:14:55.000000 grss-4.0.1/grss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-25 18:14:55.000000 grss-4.0.1/grss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)      163 2024-04-25 18:14:55.000000 grss-4.0.1/grss.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       53 2024-04-25 18:14:55.000000 grss-4.0.1/grss.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.198768 grss-4.0.1/include/
+-rw-r--r--   0 runner     (501) staff       (20)     1502 2024-04-25 18:14:08.000000 grss-4.0.1/include/approach.h
+-rw-r--r--   0 runner     (501) staff       (20)     3334 2024-04-25 18:14:08.000000 grss-4.0.1/include/elements.h
+-rw-r--r--   0 runner     (501) staff       (20)     1669 2024-04-25 18:14:08.000000 grss-4.0.1/include/force.h
+-rw-r--r--   0 runner     (501) staff       (20)     4577 2024-04-25 18:14:08.000000 grss-4.0.1/include/gr15.h
+-rw-r--r--   0 runner     (501) staff       (20)     1464 2024-04-25 18:14:08.000000 grss-4.0.1/include/grss.h
+-rw-r--r--   0 runner     (501) staff       (20)     6190 2024-04-25 18:14:08.000000 grss-4.0.1/include/interpolate.h
+-rw-r--r--   0 runner     (501) staff       (20)      356 2024-04-25 18:14:08.000000 grss-4.0.1/include/parallel.h
+-rw-r--r--   0 runner     (501) staff       (20)     2714 2024-04-25 18:14:08.000000 grss-4.0.1/include/pck.h
+-rw-r--r--   0 runner     (501) staff       (20)    19128 2024-04-25 18:14:08.000000 grss-4.0.1/include/simulation.h
+-rw-r--r--   0 runner     (501) staff       (20)     3804 2024-04-25 18:14:08.000000 grss-4.0.1/include/spk.h
+-rw-r--r--   0 runner     (501) staff       (20)     2685 2024-04-25 18:14:08.000000 grss-4.0.1/include/stm.h
+-rw-r--r--   0 runner     (501) staff       (20)     1812 2024-04-25 18:14:08.000000 grss-4.0.1/include/timeconvert.h
+-rw-r--r--   0 runner     (501) staff       (20)     5462 2024-04-25 18:14:08.000000 grss-4.0.1/include/utilities.h
+-rw-r--r--   0 runner     (501) staff       (20)     2114 2024-04-25 18:14:08.000000 grss-4.0.1/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)      163 2024-04-25 18:14:08.000000 grss-4.0.1/requirements.txt
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-25 18:14:55.227557 grss-4.0.1/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     1740 2024-04-25 18:14:08.000000 grss-4.0.1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.207184 grss-4.0.1/src/
+-rw-r--r--   0 runner     (501) staff       (20)      283 2024-04-25 18:14:08.000000 grss-4.0.1/src/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    31500 2024-04-25 18:14:08.000000 grss-4.0.1/src/approach.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    26087 2024-04-25 18:14:08.000000 grss-4.0.1/src/elements.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    29546 2024-04-25 18:14:08.000000 grss-4.0.1/src/force.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    20530 2024-04-25 18:14:08.000000 grss-4.0.1/src/gr15.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    45888 2024-04-25 18:14:08.000000 grss-4.0.1/src/grss.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    44803 2024-04-25 18:14:08.000000 grss-4.0.1/src/interpolate.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     2722 2024-04-25 18:14:08.000000 grss-4.0.1/src/parallel.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    35824 2024-04-25 18:14:08.000000 grss-4.0.1/src/pck.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    68054 2024-04-25 18:14:08.000000 grss-4.0.1/src/simulation.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    15260 2024-04-25 18:14:08.000000 grss-4.0.1/src/spk.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    24181 2024-04-25 18:14:08.000000 grss-4.0.1/src/stm.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     6951 2024-04-25 18:14:08.000000 grss-4.0.1/src/timeconvert.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    12536 2024-04-25 18:14:08.000000 grss-4.0.1/src/utilities.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.185328 grss-4.0.1/tests/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.185257 grss-4.0.1/tests/cpp/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.209187 grss-4.0.1/tests/cpp/prop/
+-rw-r--r--   0 runner     (501) staff       (20)      797 2024-04-25 18:14:08.000000 grss-4.0.1/tests/cpp/prop/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     3725 2024-04-25 18:14:08.000000 grss-4.0.1/tests/cpp/prop/apophis.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     5981 2024-04-25 18:14:08.000000 grss-4.0.1/tests/cpp/prop/didymos.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     3449 2024-04-25 18:14:08.000000 grss-4.0.1/tests/cpp/prop/pck_map.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     5917 2024-04-25 18:14:08.000000 grss-4.0.1/tests/cpp/prop/spk_map.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.209459 grss-4.0.1/tests/python/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.219120 grss-4.0.1/tests/python/fit/
+-rw-r--r--   0 runner     (501) staff       (20)   743881 2024-04-25 18:14:08.000000 grss-4.0.1/tests/python/fit/chesley.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)   701963 2024-04-25 18:14:08.000000 grss-4.0.1/tests/python/fit/eggl.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)   635614 2024-04-25 18:14:08.000000 grss-4.0.1/tests/python/fit/farnocchia.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)   666353 2024-04-25 18:14:08.000000 grss-4.0.1/tests/python/fit/shantanunaidu.ipynb
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-25 18:14:55.226000 grss-4.0.1/tests/python/prop/
+-rw-r--r--   0 runner     (501) staff       (20)   104846 2024-04-25 18:14:08.000000 grss-4.0.1/tests/python/prop/apophis.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)   102230 2024-04-25 18:14:08.000000 grss-4.0.1/tests/python/prop/didymos.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)   116221 2024-04-25 18:14:08.000000 grss-4.0.1/tests/python/prop/icarus.ipynb
+-rw-r--r--   0 runner     (501) staff       (20)    77629 2024-04-25 18:14:08.000000 grss-4.0.1/tests/python/prop/moshup.ipynb
+-rwxr-xr-x   0 runner     (501) staff       (20)      269 2024-04-25 18:14:08.000000 grss-4.0.1/tests/python/run_tests.sh
```

### Comparing `grss-4.0.0/CMakeLists.txt` & `grss-4.0.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/LICENSE` & `grss-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/PKG-INFO` & `grss-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grss
-Version: 4.0.0
+Version: 4.0.1
 Summary: GRSS: Gauss-Radau Small-body Simulator
 Author: Rahil Makadia
 Author-email: makadia2@illinois.edu
 Maintainer: Rahil Makadia
 Maintainer-email: makadia2@illinois.edu
 License: MIT License
```

### Comparing `grss-4.0.0/README.md` & `grss-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/build_cpp.sh` & `grss-4.0.1/build_cpp.sh`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/docs/source/conf.py` & `grss-4.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/extern/get_cspice.py` & `grss-4.0.1/extern/get_cspice.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/grss/debias/get_debiasing_data.py` & `grss-4.0.1/grss/debias/get_debiasing_data.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/grss/fit/fit_ades.py` & `grss-4.0.1/grss/fit/fit_ades.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/grss/fit/fit_optical.py` & `grss-4.0.1/grss/fit/fit_optical.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,14 +339,16 @@
         cov = transit_count*cov_sys + cov_rand
         ra_sig = cov[0,0]**0.5
         dec_sig = cov[1,1]**0.5
         corr = cov[0,1]/ra_sig/dec_sig
         obs_df.loc[idx, 'sigRA'] = ra_sig
         obs_df.loc[idx, 'sigDec'] = dec_sig
         obs_df.loc[idx, 'sigCorr'] = corr
+        obs_df.loc[idx, 'biasRA'] = 0.0
+        obs_df.loc[idx, 'biasDec'] = 0.0
         obs_df.loc[idx, 'ctr'] = ctr
         obs_df.loc[idx, 'sys'] = sys
         obs_df.loc[idx, 'pos1'] = data['x_gaia_geocentric']
         obs_df.loc[idx, 'pos2'] = data['y_gaia_geocentric']
         obs_df.loc[idx, 'pos3'] = data['z_gaia_geocentric']
     if verbose:
         print(f"\tFiltered to {gaia_add_counter} observations that",
@@ -483,17 +485,16 @@
         Packed program ID
     """
     # should be radix-52 with 0-1 first
     if len(code) != 2 or code[0] not in "01":
         raise RuntimeError ("Illegal packed prog ID " + code + " in xml")
     try:
         index = unpack_letters[code[1]]
-        if code[0] == 1:
-            index += 52
-        packed = prog_codes[index]
+        index += 62*unpack_letters[code[0]]
+        packed = prog_codes[index] if index <= 93 else ' '
     except Exception as exc:
         raise RuntimeError ("Illegal packed prog ID " + code + " in xml") from exc
     return packed
 
 # from ADES-Master/Python/bin/packUtil.py
 def get_unpacked_prog_id(code):
     """
@@ -510,16 +511,16 @@
         Full ADES Program code ID
     """
     # should be radix-52 with 0-1 first
     try:
         index = prog_codes.index(code)
     except Exception as exc:
         raise RuntimeError("Illegal program code " + code) from exc
-    first = '1' if index > 51 else '0'
-    second = pack_letters[index%52]
+    first = '1' if index > 61 else '0'
+    second = pack_letters[index%62]
     return first + second
 
 def apply_station_weight_rules(group, obs_df, cols, verbose):
     """
     Apply the station-specific weight rules to the observation data.
 
     Parameters
```

### Comparing `grss-4.0.0/grss/fit/fit_radar.py` & `grss-4.0.1/grss/fit/fit_radar.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/grss/fit/fit_simulation.py` & `grss-4.0.1/grss/fit/fit_simulation.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/grss/fit/fit_utils.py` & `grss-4.0.1/grss/fit/fit_utils.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/grss/kernels/get_kernels.py` & `grss-4.0.1/grss/kernels/get_kernels.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/grss/prop/prop_parallel.py` & `grss-4.0.1/grss/prop/prop_parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,14 +307,16 @@
     -------
     impact : libgrss.ImpactParameters
         ImpactParameters object.
     """
     impact = libgrss.ImpactParameters()
     impact.t = row['t']
     impact.xRel = row['xRel']
+    impact.tMap = row['tMap']
+    impact.xRelMap = row['xRelMap']
     impact.dist = row['dist']
     impact.vel = row['vel']
     impact.vInf = row['vInf']
     impact.flybyBody = row['flybyBody']
     impact.flybyBodyIdx = row['flybyBodyIdx']
     impact.centralBody = row['centralBody']
     impact.centralBodyIdx = row['centralBodyIdx']
```

### Comparing `grss-4.0.0/grss/prop/prop_unscented.py` & `grss-4.0.1/grss/prop/prop_unscented.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/grss/prop/prop_utils.py` & `grss-4.0.1/grss/prop/prop_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,23 +124,29 @@
     Returns
     -------
     scale_factor : float
         scale factor for plotting close approaches, in km
     units : str
         units of the scale factor
     """
-    if body_id in {1,199,"Mercury Barycenter"}:
+    if body_id in {10,"Sun"}:
+        scale_factor = 696000.0
+        units = r"R$_\odot$"
+    elif body_id in {1,199,"Mercury Barycenter"}:
         scale_factor = 2440.53
         units = "R$_{Mercury}$"
     elif body_id in {2,299,"Venus Barycenter"}:
         scale_factor = 6051.8
         units = "R$_{Venus}$"
     elif body_id in {399,"Earth"}:
         scale_factor = 6378.137
         units = r"R$_\oplus$"
+    elif body_id in {301,"Moon"}:
+        scale_factor = 1737.4
+        units = "R$_{Moon}$"
     elif body_id in {4,499,"Mars Barycenter"}:
         scale_factor = 3396.19
         units = "R$_{Mars}$"
     else:
         raise ValueError("Unknown body ID")
     return scale_factor, units
 
@@ -602,17 +608,19 @@
         t_dev = np.std(times)
         t_map_mean = np.mean(map_times)
     elif analytic_info is not None:
         t_mean = ca_list[0].t
         # t_dev computed in partials_to_ellipse
         t_map_mean = ca_list[0].tMap
     else:
-        t_mean = np.nan
-        t_dev = np.nan
-        t_map_mean = np.nan
+        print("WARNING: No sigma points, analytic info, or enough data",
+                "to reliably compute mean time")
+        t_mean = np.mean(times)
+        t_dev = np.std(times)
+        t_map_mean = np.mean(map_times)
     if impact_any:
         t_mean_str = Time(t_mean, format='mjd', scale='tdb').utc.iso
         t_map_mean = Time(t_map_mean, format='mjd', scale='tdb').utc.iso
     else:
         t_mean_str = Time(t_mean, format='mjd', scale='tdb').tdb.iso
         t_map_mean = Time(t_map_mean, format='mjd', scale='tdb').tdb.iso
     t_std = n_std*t_dev
```

### Comparing `grss-4.0.0/grss/utils.py` & `grss-4.0.1/grss/utils.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/grss.egg-info/PKG-INFO` & `grss-4.0.1/grss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grss
-Version: 4.0.0
+Version: 4.0.1
 Summary: GRSS: Gauss-Radau Small-body Simulator
 Author: Rahil Makadia
 Author-email: makadia2@illinois.edu
 Maintainer: Rahil Makadia
 Maintainer-email: makadia2@illinois.edu
 License: MIT License
```

### Comparing `grss-4.0.0/grss.egg-info/SOURCES.txt` & `grss-4.0.1/grss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/include/approach.h` & `grss-4.0.1/include/approach.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/include/elements.h` & `grss-4.0.1/include/elements.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/include/force.h` & `grss-4.0.1/include/force.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/include/gr15.h` & `grss-4.0.1/include/gr15.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/include/grss.h` & `grss-4.0.1/include/grss.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/include/interpolate.h` & `grss-4.0.1/include/interpolate.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/include/pck.h` & `grss-4.0.1/include/pck.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/include/simulation.h` & `grss-4.0.1/include/simulation.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/include/spk.h` & `grss-4.0.1/include/spk.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/include/stm.h` & `grss-4.0.1/include/stm.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/include/timeconvert.h` & `grss-4.0.1/include/timeconvert.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/include/utilities.h` & `grss-4.0.1/include/utilities.h`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/pyproject.toml` & `grss-4.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/setup.py` & `grss-4.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/src/approach.cpp` & `grss-4.0.1/src/approach.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/src/elements.cpp` & `grss-4.0.1/src/elements.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/src/force.cpp` & `grss-4.0.1/src/force.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/src/gr15.cpp` & `grss-4.0.1/src/gr15.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/src/grss.cpp` & `grss-4.0.1/src/grss.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/src/interpolate.cpp` & `grss-4.0.1/src/interpolate.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/src/parallel.cpp` & `grss-4.0.1/src/parallel.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/src/pck.cpp` & `grss-4.0.1/src/pck.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/src/simulation.cpp` & `grss-4.0.1/src/simulation.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/src/spk.cpp` & `grss-4.0.1/src/spk.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/src/stm.cpp` & `grss-4.0.1/src/stm.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/src/timeconvert.cpp` & `grss-4.0.1/src/timeconvert.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/src/utilities.cpp` & `grss-4.0.1/src/utilities.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/tests/cpp/prop/CMakeLists.txt` & `grss-4.0.1/tests/cpp/prop/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/tests/cpp/prop/apophis.cpp` & `grss-4.0.1/tests/cpp/prop/apophis.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/tests/cpp/prop/didymos.cpp` & `grss-4.0.1/tests/cpp/prop/didymos.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/tests/cpp/prop/pck_map.cpp` & `grss-4.0.1/tests/cpp/prop/pck_map.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/tests/cpp/prop/spk_map.cpp` & `grss-4.0.1/tests/cpp/prop/spk_map.cpp`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/tests/python/fit/chesley.ipynb` & `grss-4.0.1/tests/python/fit/chesley.ipynb`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/tests/python/fit/eggl.ipynb` & `grss-4.0.1/tests/python/fit/eggl.ipynb`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/tests/python/fit/farnocchia.ipynb` & `grss-4.0.1/tests/python/fit/farnocchia.ipynb`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/tests/python/fit/shantanunaidu.ipynb` & `grss-4.0.1/tests/python/fit/shantanunaidu.ipynb`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/tests/python/prop/apophis.ipynb` & `grss-4.0.1/tests/python/prop/apophis.ipynb`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/tests/python/prop/didymos.ipynb` & `grss-4.0.1/tests/python/prop/didymos.ipynb`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/tests/python/prop/icarus.ipynb` & `grss-4.0.1/tests/python/prop/icarus.ipynb`

 * *Files identical despite different names*

### Comparing `grss-4.0.0/tests/python/prop/moshup.ipynb` & `grss-4.0.1/tests/python/prop/moshup.ipynb`

 * *Files identical despite different names*


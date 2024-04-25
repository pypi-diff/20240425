# Comparing `tmp/pypromice-1.3.4.tar.gz` & `tmp/pypromice-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypromice-1.3.4.tar", last modified: Wed Apr 10 12:50:44 2024, max compression
+gzip compressed data, was "pypromice-1.3.5.tar", last modified: Thu Apr 25 06:17:06 2024, max compression
```

## Comparing `pypromice-1.3.4.tar` & `pypromice-1.3.5.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.438857 pypromice-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-10 12:50:37.000000 pypromice-1.3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-10 12:50:37.000000 pypromice-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-10 12:50:44.438857 pypromice-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-10 12:50:37.000000 pypromice-1.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 12:50:44.438857 pypromice-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-10 12:50:37.000000 pypromice-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.414857 pypromice-1.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.418857 pypromice-1.3.4/src/pypromice/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.418857 pypromice-1.3.4/src/pypromice/get/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/get/get.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1806 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/get/get_promice_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.422857 pypromice-1.3.4/src/pypromice/postprocess/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/postprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/postprocess/bufr_to_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)    17032 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/postprocess/bufr_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/postprocess/get_bufr.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/postprocess/positions_seed.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8710 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/postprocess/real_time_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    17025 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/postprocess/station_configurations.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.422857 pypromice-1.3.4/src/pypromice/process/
--rw-r--r--   0 runner    (1001) docker     (127)    22818 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/process/L0toL1.py
--rw-r--r--   0 runner    (1001) docker     (127)    25538 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/process/L1toL2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18238 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/process/L2toL3.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29844 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/process/aws.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1656 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/process/get_l3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/process/join_l3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/process/metadata.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/process/value_clipping.py
--rw-r--r--   0 runner    (1001) docker     (127)    13340 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/process/variables.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.422857 pypromice-1.3.4/src/pypromice/qc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13537 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/qc/github_data_issues.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.422857 pypromice-1.3.4/src/pypromice/qc/percentiles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/qc/percentiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/qc/percentiles/compute_thresholds.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/qc/percentiles/outlier_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/qc/percentiles/thresholds.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/qc/persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/qc/persistence_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.434857 pypromice-1.3.4/src/pypromice/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_config1.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_config2.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_email
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_payload_formats.csv
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_payload_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7504 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_percentile.py
--rw-r--r--   0 runner    (1001) docker     (127)  1626942 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_raw1.txt
--rw-r--r--   0 runner    (1001) docker     (127)  3337781 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_raw_DataTable2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   348047 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_raw_SlimTableMem1.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1993699 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_raw_transmitted1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/test/test_raw_transmitted2.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.438857 pypromice-1.3.4/src/pypromice/tx/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/tx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/tx/get_l0tx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/tx/get_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/tx/get_watsontx.py
--rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/tx/payload_formats.csv
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/tx/payload_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-04-10 12:50:37.000000 pypromice-1.3.4/src/pypromice/tx/tx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:50:44.438857 pypromice-1.3.4/src/pypromice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-10 12:50:44.000000 pypromice-1.3.4/src/pypromice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-10 12:50:44.000000 pypromice-1.3.4/src/pypromice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 12:50:44.000000 pypromice-1.3.4/src/pypromice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-10 12:50:44.000000 pypromice-1.3.4/src/pypromice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-10 12:50:44.000000 pypromice-1.3.4/src/pypromice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 12:50:44.000000 pypromice-1.3.4/src/pypromice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.272019 pypromice-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-25 06:17:02.000000 pypromice-1.3.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 06:17:02.000000 pypromice-1.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-25 06:17:06.272019 pypromice-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-25 06:17:02.000000 pypromice-1.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 06:17:06.272019 pypromice-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-25 06:17:02.000000 pypromice-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.248018 pypromice-1.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.252018 pypromice-1.3.5/src/pypromice/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.252018 pypromice-1.3.5/src/pypromice/get/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/get/get.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1806 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/get/get_promice_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.256018 pypromice-1.3.5/src/pypromice/postprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/postprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/postprocess/bufr_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17032 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/postprocess/bufr_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/postprocess/get_bufr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/postprocess/positions_seed.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8710 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/postprocess/real_time_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17025 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/postprocess/station_configurations.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.256018 pypromice-1.3.5/src/pypromice/process/
+-rw-r--r--   0 runner    (1001) docker     (127)    22818 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/process/L0toL1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25577 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/process/L1toL2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18238 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/process/L2toL3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29844 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/process/aws.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1656 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/process/get_l3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/process/join_l3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/process/metadata.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/process/value_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13340 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/process/variables.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.260018 pypromice-1.3.5/src/pypromice/qc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13537 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/qc/github_data_issues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.260018 pypromice-1.3.5/src/pypromice/qc/percentiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/qc/percentiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/qc/percentiles/compute_thresholds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/qc/percentiles/outlier_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/qc/percentiles/thresholds.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/qc/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/qc/persistence_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.268018 pypromice-1.3.5/src/pypromice/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_config1.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_config2.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_email
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_payload_formats.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_payload_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7504 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_percentile.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1626942 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_raw1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  3337781 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_raw_DataTable2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   348047 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_raw_SlimTableMem1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1993699 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_raw_transmitted1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/test/test_raw_transmitted2.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.272019 pypromice-1.3.5/src/pypromice/tx/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/tx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/tx/get_l0tx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/tx/get_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/tx/get_watsontx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/tx/payload_formats.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/tx/payload_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-04-25 06:17:02.000000 pypromice-1.3.5/src/pypromice/tx/tx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:17:06.272019 pypromice-1.3.5/src/pypromice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-25 06:17:06.000000 pypromice-1.3.5/src/pypromice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-25 06:17:06.000000 pypromice-1.3.5/src/pypromice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 06:17:06.000000 pypromice-1.3.5/src/pypromice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-25 06:17:06.000000 pypromice-1.3.5/src/pypromice.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-25 06:17:06.000000 pypromice-1.3.5/src/pypromice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 06:17:06.000000 pypromice-1.3.5/src/pypromice.egg-info/top_level.txt
```

### Comparing `pypromice-1.3.4/LICENSE.txt` & `pypromice-1.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/PKG-INFO` & `pypromice-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypromice
-Version: 1.3.4
+Version: 1.3.5
 Summary: PROMICE/GC-Net data processing toolbox
 Home-page: https://github.com/GEUS-Glaciology-and-Climate/pypromice
 Author: GEUS Glaciology and Climate
 Project-URL: Bug Tracker, https://github.com/GEUS-Glaciology-and-Climate/pypromice/issues
 Project-URL: Documentation, https://pypromice.readthedocs.io
 Project-URL: Source Code, https://github.com/GEUS-Glaciology-and-Climate/pypromice
 Keywords: promice gc-net aws climate glaciology greenland geus
```

### Comparing `pypromice-1.3.4/README.md` & `pypromice-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/setup.py` & `pypromice-1.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pypromice",
-    version="1.3.4",
+    version="1.3.5",
     author="GEUS Glaciology and Climate",
     description="PROMICE/GC-Net data processing toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/GEUS-Glaciology-and-Climate/pypromice",
     project_urls={
         "Bug Tracker": "https://github.com/GEUS-Glaciology-and-Climate/pypromice/issues",
```

### Comparing `pypromice-1.3.4/src/pypromice/get/get.py` & `pypromice-1.3.5/src/pypromice/get/get.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/get/get_promice_data.py` & `pypromice-1.3.5/src/pypromice/get/get_promice_data.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/postprocess/bufr_utilities.py` & `pypromice-1.3.5/src/pypromice/postprocess/bufr_utilities.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/postprocess/get_bufr.py` & `pypromice-1.3.5/src/pypromice/postprocess/get_bufr.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/postprocess/real_time_utilities.py` & `pypromice-1.3.5/src/pypromice/postprocess/real_time_utilities.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/postprocess/station_configurations.toml` & `pypromice-1.3.5/src/pypromice/postprocess/station_configurations.toml`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/process/L0toL1.py` & `pypromice-1.3.5/src/pypromice/process/L0toL1.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/process/L1toL2.py` & `pypromice-1.3.5/src/pypromice/process/L1toL2.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,14 +319,15 @@
                    + np.log10(ei0))
 
     # Define freezing point. Why > -100?
     freezing = (T < 0) & (T > -100).values
 
     # Set to Groff & Gratch values when freezing, otherwise just rh
     rh_cor = rh.where(~freezing, other = rh*(e_s_wtr / e_s_ice))
+    rh_cor = rh_cor.where(T.notnull())
     return rh_cor
 
 
 def correctPrecip(precip, wspd):
     '''Correct precipitation with the undercatch correction method used in
     Yang et al. (1999) and Box et al. (2022), based on Goodison et al. (1998)
```

### Comparing `pypromice-1.3.4/src/pypromice/process/L2toL3.py` & `pypromice-1.3.5/src/pypromice/process/L2toL3.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/process/aws.py` & `pypromice-1.3.5/src/pypromice/process/aws.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/process/get_l3.py` & `pypromice-1.3.5/src/pypromice/process/get_l3.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/process/join_l3.py` & `pypromice-1.3.5/src/pypromice/process/join_l3.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/process/metadata.csv` & `pypromice-1.3.5/src/pypromice/process/metadata.csv`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/process/value_clipping.py` & `pypromice-1.3.5/src/pypromice/process/value_clipping.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/process/variables.csv` & `pypromice-1.3.5/src/pypromice/process/variables.csv`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/qc/github_data_issues.py` & `pypromice-1.3.5/src/pypromice/qc/github_data_issues.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/qc/percentiles/compute_thresholds.py` & `pypromice-1.3.5/src/pypromice/qc/percentiles/compute_thresholds.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/qc/percentiles/outlier_detector.py` & `pypromice-1.3.5/src/pypromice/qc/percentiles/outlier_detector.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/qc/percentiles/thresholds.csv` & `pypromice-1.3.5/src/pypromice/qc/percentiles/thresholds.csv`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/qc/persistence.py` & `pypromice-1.3.5/src/pypromice/qc/persistence.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/qc/persistence_test.py` & `pypromice-1.3.5/src/pypromice/qc/persistence_test.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/test/test_config1.toml` & `pypromice-1.3.5/src/pypromice/test/test_config1.toml`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/test/test_config2.toml` & `pypromice-1.3.5/src/pypromice/test/test_config2.toml`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/test/test_email` & `pypromice-1.3.5/src/pypromice/test/test_email`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/test/test_percentile.py` & `pypromice-1.3.5/src/pypromice/test/test_percentile.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/test/test_raw1.txt` & `pypromice-1.3.5/src/pypromice/test/test_raw1.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/test/test_raw_DataTable2.txt` & `pypromice-1.3.5/src/pypromice/test/test_raw_DataTable2.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/test/test_raw_SlimTableMem1.txt` & `pypromice-1.3.5/src/pypromice/test/test_raw_SlimTableMem1.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/test/test_raw_transmitted1.txt` & `pypromice-1.3.5/src/pypromice/test/test_raw_transmitted1.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/test/test_raw_transmitted2.txt` & `pypromice-1.3.5/src/pypromice/test/test_raw_transmitted2.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/tx/get_l0tx.py` & `pypromice-1.3.5/src/pypromice/tx/get_l0tx.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/tx/get_msg.py` & `pypromice-1.3.5/src/pypromice/tx/get_msg.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/tx/get_watsontx.py` & `pypromice-1.3.5/src/pypromice/tx/get_watsontx.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/tx/payload_formats.csv` & `pypromice-1.3.5/src/pypromice/tx/payload_formats.csv`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice/tx/tx.py` & `pypromice-1.3.5/src/pypromice/tx/tx.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.3.4/src/pypromice.egg-info/PKG-INFO` & `pypromice-1.3.5/src/pypromice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypromice
-Version: 1.3.4
+Version: 1.3.5
 Summary: PROMICE/GC-Net data processing toolbox
 Home-page: https://github.com/GEUS-Glaciology-and-Climate/pypromice
 Author: GEUS Glaciology and Climate
 Project-URL: Bug Tracker, https://github.com/GEUS-Glaciology-and-Climate/pypromice/issues
 Project-URL: Documentation, https://pypromice.readthedocs.io
 Project-URL: Source Code, https://github.com/GEUS-Glaciology-and-Climate/pypromice
 Keywords: promice gc-net aws climate glaciology greenland geus
```

### Comparing `pypromice-1.3.4/src/pypromice.egg-info/SOURCES.txt` & `pypromice-1.3.5/src/pypromice.egg-info/SOURCES.txt`

 * *Files identical despite different names*


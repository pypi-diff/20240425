# Comparing `tmp/lifton-0.0.3.tar.gz` & `tmp/lifton-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifton-0.0.3.tar", last modified: Sun Apr 21 17:38:22 2024, max compression
+gzip compressed data, was "lifton-1.0.0.tar", last modified: Thu Apr 25 19:31:45 2024, max compression
```

## Comparing `lifton-0.0.3.tar` & `lifton-1.0.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-04-21 17:38:22.011859 lifton-0.0.3/
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    34599 2024-01-03 20:18:51.000000 lifton-0.0.3/LICENSE
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    22677 2024-04-21 17:38:22.000859 lifton-0.0.3/PKG-INFO
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    22382 2024-03-04 20:29:33.000000 lifton-0.0.3/README.md
-drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-04-21 17:38:20.587856 lifton-0.0.3/lifton/
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)       23 2024-04-21 17:37:16.000000 lifton-0.0.3/lifton/__init__.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     8659 2024-04-19 19:09:42.000000 lifton-0.0.3/lifton/align.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     6640 2024-04-19 19:09:51.000000 lifton-0.0.3/lifton/annotation.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     2620 2024-04-19 19:10:25.000000 lifton-0.0.3/lifton/extract_sequence.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     1823 2024-04-19 19:16:33.000000 lifton-0.0.3/lifton/get_id_fraction.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      578 2024-04-19 19:16:38.000000 lifton-0.0.3/lifton/intervals.py
-drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-04-21 17:38:21.822858 lifton-0.0.3/lifton/liftoff/
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2023-12-24 02:47:54.000000 lifton-0.0.3/lifton/liftoff/__init__.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    13175 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/align_features.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      597 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/aligned_seg.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    10276 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/extract_features.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      190 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/feature_hierarchy.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    19044 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/find_best_mapping.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     9361 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/fix_overlapping_features.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5664 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/lift_features.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    15486 2024-02-12 19:50:40.000000 lifton-0.0.3/lifton/liftoff/liftoff_main.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     4032 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/liftoff_utils.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5206 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/liftover_types.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     3945 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/merge_lifted_features.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      372 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/new_feature.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    14008 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/polish.py
-drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-04-21 17:38:21.949859 lifton-0.0.3/lifton/liftoff/tests/
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        1 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/tests/__init__.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     2058 2023-12-24 03:45:19.000000 lifton-0.0.3/lifton/liftoff/tests/test_advanced.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     1895 2023-12-24 03:45:19.000000 lifton-0.0.3/lifton/liftoff/tests/test_basic.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5428 2023-12-24 03:45:20.000000 lifton-0.0.3/lifton/liftoff/write_new_gff.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    20297 2024-04-21 13:55:31.000000 lifton-0.0.3/lifton/lifton.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    34194 2024-04-21 13:30:06.000000 lifton-0.0.3/lifton/lifton_class.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    19966 2024-04-21 13:29:00.000000 lifton-0.0.3/lifton/lifton_utils.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      233 2024-01-24 15:32:08.000000 lifton-0.0.3/lifton/logger.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     7585 2024-04-21 00:36:04.000000 lifton-0.0.3/lifton/protein_maximization.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     4261 2024-04-21 17:24:05.000000 lifton-0.0.3/lifton/run_evaluation.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     8967 2024-04-21 17:29:27.000000 lifton-0.0.3/lifton/run_liftoff.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     6576 2024-04-21 01:51:11.000000 lifton-0.0.3/lifton/run_miniprot.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5595 2024-04-21 01:28:11.000000 lifton-0.0.3/lifton/stats.py
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     4196 2024-04-21 13:22:57.000000 lifton-0.0.3/lifton/variants.py
-drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-04-21 17:38:20.907856 lifton-0.0.3/lifton.egg-info/
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    22677 2024-04-21 17:38:19.000000 lifton-0.0.3/lifton.egg-info/PKG-INFO
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     1154 2024-04-21 17:38:19.000000 lifton-0.0.3/lifton.egg-info/SOURCES.txt
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        1 2024-04-21 17:38:19.000000 lifton-0.0.3/lifton.egg-info/dependency_links.txt
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)       46 2024-04-21 17:38:19.000000 lifton-0.0.3/lifton.egg-info/entry_points.txt
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      168 2024-04-21 17:38:19.000000 lifton-0.0.3/lifton.egg-info/requires.txt
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        7 2024-04-21 17:38:19.000000 lifton-0.0.3/lifton.egg-info/top_level.txt
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)       38 2024-04-21 17:38:22.021859 lifton-0.0.3/setup.cfg
--rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      833 2024-04-21 17:37:41.000000 lifton-0.0.3/setup.py
+drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-04-25 19:31:45.271436 lifton-1.0.0/
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    34599 2024-01-03 20:18:51.000000 lifton-1.0.0/LICENSE
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    27871 2024-04-25 19:31:45.259436 lifton-1.0.0/PKG-INFO
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    27543 2024-04-25 19:31:21.000000 lifton-1.0.0/README.md
+drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-04-25 19:31:44.231434 lifton-1.0.0/lifton/
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)       23 2024-04-25 19:16:25.000000 lifton-1.0.0/lifton/__init__.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     8659 2024-04-19 19:09:42.000000 lifton-1.0.0/lifton/align.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     6640 2024-04-25 19:14:34.000000 lifton-1.0.0/lifton/annotation.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     2620 2024-04-21 18:41:09.000000 lifton-1.0.0/lifton/extract_sequence.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     1823 2024-04-21 18:41:11.000000 lifton-1.0.0/lifton/get_id_fraction.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      578 2024-04-19 19:16:38.000000 lifton-1.0.0/lifton/intervals.py
+drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-04-25 19:31:45.088436 lifton-1.0.0/lifton/liftoff/
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2023-12-24 02:47:54.000000 lifton-1.0.0/lifton/liftoff/__init__.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    13175 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/align_features.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      597 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/aligned_seg.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    10276 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/extract_features.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      190 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/feature_hierarchy.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    19044 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/find_best_mapping.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     9361 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/fix_overlapping_features.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5664 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/lift_features.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    15486 2024-02-12 19:50:40.000000 lifton-1.0.0/lifton/liftoff/liftoff_main.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     4032 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/liftoff_utils.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5206 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/liftover_types.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     3945 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/merge_lifted_features.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      372 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/new_feature.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    14008 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/polish.py
+drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-04-25 19:31:45.210436 lifton-1.0.0/lifton/liftoff/tests/
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        1 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/tests/__init__.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     2058 2023-12-24 03:45:19.000000 lifton-1.0.0/lifton/liftoff/tests/test_advanced.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     1895 2023-12-24 03:45:19.000000 lifton-1.0.0/lifton/liftoff/tests/test_basic.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5428 2023-12-24 03:45:20.000000 lifton-1.0.0/lifton/liftoff/write_new_gff.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    20402 2024-04-24 11:32:28.000000 lifton-1.0.0/lifton/lifton.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    34533 2024-04-21 22:08:34.000000 lifton-1.0.0/lifton/lifton_class.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    20597 2024-04-24 11:32:28.000000 lifton-1.0.0/lifton/lifton_utils.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      233 2024-01-24 15:32:08.000000 lifton-1.0.0/lifton/logger.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     7585 2024-04-21 00:36:04.000000 lifton-1.0.0/lifton/protein_maximization.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5764 2024-04-21 23:00:23.000000 lifton-1.0.0/lifton/run_evaluation.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     9031 2024-04-24 11:32:28.000000 lifton-1.0.0/lifton/run_liftoff.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     6507 2024-04-24 11:32:28.000000 lifton-1.0.0/lifton/run_miniprot.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     5595 2024-04-21 21:25:50.000000 lifton-1.0.0/lifton/stats.py
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     4191 2024-04-21 22:07:42.000000 lifton-1.0.0/lifton/variants.py
+drwxrwsr-x   0 kh.chao   (3822) salzberg_ifx  (5042)        0 2024-04-25 19:31:44.479434 lifton-1.0.0/lifton.egg-info/
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)    27871 2024-04-25 19:31:43.000000 lifton-1.0.0/lifton.egg-info/PKG-INFO
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)     1154 2024-04-25 19:31:43.000000 lifton-1.0.0/lifton.egg-info/SOURCES.txt
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        1 2024-04-25 19:31:43.000000 lifton-1.0.0/lifton.egg-info/dependency_links.txt
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)       46 2024-04-25 19:31:43.000000 lifton-1.0.0/lifton.egg-info/entry_points.txt
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      168 2024-04-25 19:31:43.000000 lifton-1.0.0/lifton.egg-info/requires.txt
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)        7 2024-04-25 19:31:43.000000 lifton-1.0.0/lifton.egg-info/top_level.txt
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)       38 2024-04-25 19:31:45.280436 lifton-1.0.0/setup.cfg
+-rw-rw-r--   0 kh.chao   (3822) salzberg_ifx  (5042)      865 2024-04-25 19:17:04.000000 lifton-1.0.0/setup.py
```

### Comparing `lifton-0.0.3/LICENSE` & `lifton-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/PKG-INFO` & `lifton-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,1418 +1,1742 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6c69 6674  : 2.1.Name: lift
-00000020: 6f6e 0a56 6572 7369 6f6e 3a20 302e 302e  on.Version: 0.0.
-00000030: 330a 5375 6d6d 6172 793a 2041 2070 726f  3.Summary: A pro
-00000040: 7465 696e 2d63 6f64 696e 6720 6765 6e65  tein-coding gene
-00000050: 2061 6e6e 6f74 6174 696f 6e20 6669 7869   annotation fixi
-00000060: 6e67 2074 6f6f 6c0a 486f 6d65 2d70 6167  ng tool.Home-pag
-00000070: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
-00000080: 622e 636f 6d2f 4b75 616e 6861 6f2d 4368  b.com/Kuanhao-Ch
-00000090: 616f 2f4c 6966 746f 6e0a 4175 7468 6f72  ao/Lifton.Author
-000000a0: 3a20 4b75 616e 2d48 616f 2043 6861 6f0a  : Kuan-Hao Chao.
-000000b0: 4175 7468 6f72 2d65 6d61 696c 3a20 6b68  Author-email: kh
-000000c0: 2e63 6861 6f40 6373 2e6a 6875 2e65 6475  .chao@cs.jhu.edu
-000000d0: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
-000000e0: 3a20 3e3d 332e 360a 4465 7363 7269 7074  : >=3.6.Descript
-000000f0: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-00000100: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
-00000110: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
-00000120: 4345 4e53 450a 0a3c 696d 6720 616c 743d  CENSE..<img alt=
-00000130: 224d 7920 4c6f 676f 2220 636c 6173 733d  "My Logo" class=
-00000140: 226c 6f67 6f20 6865 6164 6572 2d69 6d61  "logo header-ima
-00000150: 6765 206f 6e6c 792d 6c69 6768 7420 616c  ge only-light al
-00000160: 6967 6e2d 6365 6e74 6572 2220 7372 633d  ign-center" src=
-00000170: 2267 7261 7068 6963 732f 4c69 6674 4f6e  "graphics/LiftOn
-00000180: 5f63 6f6c 6f72 2e70 6e67 2220 7374 796c  _color.png" styl
-00000190: 653d 2277 6964 7468 3a39 3025 223e 0a0a  e="width:90%">..
-000001a0: 3c64 6976 2063 6c61 7373 3d22 636f 6e74  <div class="cont
-000001b0: 656e 7422 3e0a 0a3c 6469 7620 636c 6173  ent">..<div clas
-000001c0: 733d 226c 696e 6522 3e3c 6272 3e3c 2f64  s="line"><br></d
-000001d0: 6976 3e0a 3c2f 6469 763e 0a3c 7365 6374  iv>.</div>.<sect
-000001e0: 696f 6e20 6964 3d22 6c69 6674 6f6e 2d73  ion id="lifton-s
-000001f0: 2d74 7574 6f72 6961 6c22 3e0a 3c65 6d62  -tutorial">.<emb
-00000200: 6564 3e0a 3c61 2063 6c61 7373 3d22 7265  ed>.<a class="re
-00000210: 6665 7265 6e63 6520 6578 7465 726e 616c  ference external
-00000220: 2069 6d61 6765 2d72 6566 6572 656e 6365   image-reference
-00000230: 2220 6872 6566 3d22 6874 7470 733a 2f2f  " href="https://
-00000240: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00000250: 6164 6765 2f4c 6963 656e 7365 2d47 504c  adge/License-GPL
-00000260: 7633 2d79 656c 6c6f 772e 7376 6722 3e3c  v3-yellow.svg"><
-00000270: 696d 6720 616c 743d 2268 7474 7073 3a2f  img alt="https:/
-00000280: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000290: 6261 6467 652f 4c69 6365 6e73 652d 4750  badge/License-GP
-000002a0: 4c76 332d 7965 6c6c 6f77 2e73 7667 2220  Lv3-yellow.svg" 
-000002b0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-000002c0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-000002d0: 652f 4c69 6365 6e73 652d 4750 4c76 332d  e/License-GPLv3-
-000002e0: 7965 6c6c 6f77 2e73 7667 223e 3c2f 613e  yellow.svg"></a>
-000002f0: 0a3c 6120 636c 6173 733d 2272 6566 6572  .<a class="refer
-00000300: 656e 6365 2065 7874 6572 6e61 6c20 696d  ence external im
-00000310: 6167 652d 7265 6665 7265 6e63 6522 2068  age-reference" h
-00000320: 7265 663d 2268 7474 7073 3a2f 2f69 6d67  ref="https://img
-00000330: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000340: 652f 7665 7273 696f 6e2d 762e 302e 302e  e/version-v.0.0.
-00000350: 312d 626c 7565 223e 3c69 6d67 2061 6c74  1-blue"><img alt
-00000360: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00000370: 6965 6c64 732e 696f 2f62 6164 6765 2f76  ields.io/badge/v
-00000380: 6572 7369 6f6e 2d76 2e30 2e30 2e31 2d62  ersion-v.0.0.1-b
-00000390: 6c75 6522 2073 7263 3d22 6874 7470 733a  lue" src="https:
-000003a0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-000003b0: 2f62 6164 6765 2f76 6572 7369 6f6e 2d76  /badge/version-v
-000003c0: 2e30 2e30 2e31 2d62 6c75 6522 3e3c 2f61  .0.0.1-blue"></a
-000003d0: 3e0a 3c61 2063 6c61 7373 3d22 7265 6665  >.<a class="refe
-000003e0: 7265 6e63 6520 6578 7465 726e 616c 2069  rence external i
-000003f0: 6d61 6765 2d72 6566 6572 656e 6365 2220  mage-reference" 
-00000400: 6872 6566 3d22 6874 7470 733a 2f2f 7065  href="https://pe
-00000410: 7079 2e74 6563 682f 7072 6f6a 6563 742f  py.tech/project/
-00000420: 6c69 6674 6f6e 223e 3c69 6d67 2061 6c74  lifton"><img alt
-00000430: 3d22 6874 7470 733a 2f2f 7374 6174 6963  ="https://static
-00000440: 2e70 6570 792e 7465 6368 2f70 6572 736f  .pepy.tech/perso
-00000450: 6e61 6c69 7a65 642d 6261 6467 652f 6c69  nalized-badge/li
-00000460: 6674 6f6e 3f70 6572 696f 643d 746f 7461  fton?period=tota
-00000470: 6c26 616d 703b 756e 6974 733d 6162 6272  l&amp;units=abbr
-00000480: 6576 6961 7469 6f6e 2661 6d70 3b6c 6566  eviation&amp;lef
-00000490: 745f 636f 6c6f 723d 6772 6579 2661 6d70  t_color=grey&amp
-000004a0: 3b72 6967 6874 5f63 6f6c 6f72 3d62 6c75  ;right_color=blu
-000004b0: 6526 616d 703b 6c65 6674 5f74 6578 743d  e&amp;left_text=
-000004c0: 5079 5069 2532 3064 6f77 6e6c 6f61 6473  PyPi%20downloads
-000004d0: 2220 7372 633d 2268 7474 7073 3a2f 2f73  " src="https://s
-000004e0: 7461 7469 632e 7065 7079 2e74 6563 682f  tatic.pepy.tech/
-000004f0: 7065 7273 6f6e 616c 697a 6564 2d62 6164  personalized-bad
-00000500: 6765 2f6c 6966 746f 6e3f 7065 7269 6f64  ge/lifton?period
-00000510: 3d74 6f74 616c 2661 6d70 3b75 6e69 7473  =total&amp;units
-00000520: 3d61 6262 7265 7669 6174 696f 6e26 616d  =abbreviation&am
-00000530: 703b 6c65 6674 5f63 6f6c 6f72 3d67 7265  p;left_color=gre
-00000540: 7926 616d 703b 7269 6768 745f 636f 6c6f  y&amp;right_colo
-00000550: 723d 626c 7565 2661 6d70 3b6c 6566 745f  r=blue&amp;left_
-00000560: 7465 7874 3d50 7950 6925 3230 646f 776e  text=PyPi%20down
-00000570: 6c6f 6164 7322 3e3c 2f61 3e0a 3c61 2063  loads"></a>.<a c
-00000580: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
-00000590: 6578 7465 726e 616c 2069 6d61 6765 2d72  external image-r
-000005a0: 6566 6572 656e 6365 2220 6872 6566 3d22  eference" href="
-000005b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000005c0: 6f6d 2f4b 7561 6e68 616f 2d43 6861 6f2f  om/Kuanhao-Chao/
-000005d0: 6c69 6674 6f6e 2f72 656c 6561 7365 7322  lifton/releases"
-000005e0: 3e3c 696d 6720 616c 743d 2268 7474 7073  ><img alt="https
-000005f0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000600: 6f2f 6769 7468 7562 2f64 6f77 6e6c 6f61  o/github/downloa
-00000610: 6473 2f4b 7561 6e68 616f 2d43 6861 6f2f  ds/Kuanhao-Chao/
-00000620: 6c69 6674 6f6e 2f74 6f74 616c 2e73 7667  lifton/total.svg
-00000630: 3f73 7479 6c65 3d73 6f63 6961 6c26 616d  ?style=social&am
-00000640: 703b 6c6f 676f 3d67 6974 6875 6226 616d  p;logo=github&am
-00000650: 703b 6c61 6265 6c3d 446f 776e 6c6f 6164  p;label=Download
-00000660: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
-00000670: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
-00000680: 7468 7562 2f64 6f77 6e6c 6f61 6473 2f4b  thub/downloads/K
-00000690: 7561 6e68 616f 2d43 6861 6f2f 6c69 6674  uanhao-Chao/lift
-000006a0: 6f6e 2f74 6f74 616c 2e73 7667 3f73 7479  on/total.svg?sty
-000006b0: 6c65 3d73 6f63 6961 6c26 616d 703b 6c6f  le=social&amp;lo
-000006c0: 676f 3d67 6974 6875 6226 616d 703b 6c61  go=github&amp;la
-000006d0: 6265 6c3d 446f 776e 6c6f 6164 223e 3c2f  bel=Download"></
-000006e0: 613e 0a3c 6120 636c 6173 733d 2272 6566  a>.<a class="ref
-000006f0: 6572 656e 6365 2065 7874 6572 6e61 6c20  erence external 
-00000700: 696d 6167 652d 7265 6665 7265 6e63 6522  image-reference"
-00000710: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-00000720: 6974 6875 622e 636f 6d2f 4b75 616e 6861  ithub.com/Kuanha
-00000730: 6f2d 4368 616f 2f6c 6966 746f 6e2f 7265  o-Chao/lifton/re
-00000740: 6c65 6173 6573 223e 3c69 6d67 2061 6c74  leases"><img alt
-00000750: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00000760: 6965 6c64 732e 696f 2f62 6164 6765 2f70  ields.io/badge/p
-00000770: 6c61 7466 6f72 6d2d 6d61 634f 535f 2f4c  latform-macOS_/L
-00000780: 696e 7578 2d67 7265 656e 2e73 7667 2220  inux-green.svg" 
-00000790: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-000007a0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-000007b0: 652f 706c 6174 666f 726d 2d6d 6163 4f53  e/platform-macOS
-000007c0: 5f2f 4c69 6e75 782d 6772 6565 6e2e 7376  _/Linux-green.sv
-000007d0: 6722 3e3c 2f61 3e0a 3c61 2063 6c61 7373  g"></a>.<a class
-000007e0: 3d22 7265 6665 7265 6e63 6520 6578 7465  ="reference exte
-000007f0: 726e 616c 2069 6d61 6765 2d72 6566 6572  rnal image-refer
-00000800: 656e 6365 2220 6872 6566 3d22 6874 7470  ence" href="http
-00000810: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
-00000820: 6368 2e67 6f6f 676c 652e 636f 6d2f 6769  ch.google.com/gi
-00000830: 7468 7562 2f4b 7561 6e68 616f 2d43 6861  thub/Kuanhao-Cha
-00000840: 6f2f 6c69 6674 6f6e 2f62 6c6f 622f 6d61  o/lifton/blob/ma
-00000850: 696e 2f6e 6f74 6562 6f6f 6b2f 6c69 6674  in/notebook/lift
-00000860: 6f6e 5f65 7861 6d70 6c65 2e69 7079 6e62  on_example.ipynb
-00000870: 223e 3c69 6d67 2061 6c74 3d22 6874 7470  "><img alt="http
-00000880: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
-00000890: 6368 2e67 6f6f 676c 652e 636f 6d2f 6173  ch.google.com/as
-000008a0: 7365 7473 2f63 6f6c 6162 2d62 6164 6765  sets/colab-badge
-000008b0: 2e73 7667 2220 7372 633d 2268 7474 7073  .svg" src="https
-000008c0: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
-000008d0: 682e 676f 6f67 6c65 2e63 6f6d 2f61 7373  h.google.com/ass
-000008e0: 6574 732f 636f 6c61 622d 6261 6467 652e  ets/colab-badge.
-000008f0: 7376 6722 3e3c 2f61 3e0a 3c64 6976 2063  svg"></a>.<div c
-00000900: 6c61 7373 3d22 6c69 6e65 2d62 6c6f 636b  lass="line-block
-00000910: 223e 0a3c 6469 7620 636c 6173 733d 226c  ">.<div class="l
-00000920: 696e 6522 3e3c 6272 3e3c 2f64 6976 3e0a  ine"><br></div>.
-00000930: 3c2f 6469 763e 0a3c 703e 4c69 6674 4f6e  </div>.<p>LiftOn
-00000940: 2069 7320 6120 686f 6d6f 6c6f 6779 2d62   is a homology-b
-00000950: 6173 6564 206c 6966 742d 6f76 6572 2074  ased lift-over t
-00000960: 6f6f 6c20 6465 7369 676e 6564 2074 6f20  ool designed to 
-00000970: 6163 6375 7261 7465 6c79 206d 6170 2061  accurately map a
-00000980: 6e6e 6f74 6174 696f 6e73 2069 6e20 4746  nnotations in GF
-00000990: 4620 6f72 2047 5446 2062 6574 7765 656e  F or GTF between
-000009a0: 2061 7373 656d 626c 6965 732e 2049 7420   assemblies. It 
-000009b0: 6973 2062 7569 6c74 2075 706f 6e20 7468  is built upon th
-000009c0: 6520 6661 6e74 6173 7469 6320 3c61 2063  e fantastic <a c
-000009d0: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
-000009e0: 6578 7465 726e 616c 2220 6872 6566 3d22  external" href="
-000009f0: 6874 7470 733a 2f2f 6163 6164 656d 6963  https://academic
-00000a00: 2e6f 7570 2e63 6f6d 2f62 696f 696e 666f  .oup.com/bioinfo
-00000a10: 726d 6174 6963 732f 6172 7469 636c 652f  rmatics/article/
-00000a20: 3337 2f31 322f 3136 3339 2f36 3033 3531  37/12/1639/60351
-00000a30: 3238 3f6c 6f67 696e 3d74 7275 6522 3e4c  28?login=true">L
-00000a40: 6966 746f 6666 3c2f 613e 2028 6372 6564  iftoff</a> (cred
-00000a50: 6974 7320 746f 203c 6120 636c 6173 733d  its to <a class=
-00000a60: 2272 6566 6572 656e 6365 2065 7874 6572  "reference exter
-00000a70: 6e61 6c22 2068 7265 663d 2268 7474 7073  nal" href="https
-00000a80: 3a2f 2f73 6368 6f6c 6172 2e67 6f6f 676c  ://scholar.googl
-00000a90: 652e 636f 6d2f 6369 7461 7469 6f6e 733f  e.com/citations?
-00000aa0: 7573 6572 3d4e 3374 586b 3751 4141 4141  user=N3tXk7QAAAA
-00000ab0: 4a26 616d 703b 686c 3d65 6e22 3e44 722e  J&amp;hl=en">Dr.
-00000ac0: 2041 6c61 696e 6120 5368 756d 6174 653c   Alaina Shumate<
-00000ad0: 2f61 3e29 2061 6e64 203c 6120 636c 6173  /a>) and <a clas
-00000ae0: 733d 2272 6566 6572 656e 6365 2065 7874  s="reference ext
-00000af0: 6572 6e61 6c22 2068 7265 663d 2268 7474  ernal" href="htt
-00000b00: 7073 3a2f 2f61 6361 6465 6d69 632e 6f75  ps://academic.ou
-00000b10: 702e 636f 6d2f 6269 6f69 6e66 6f72 6d61  p.com/bioinforma
-00000b20: 7469 6373 2f61 7274 6963 6c65 2f33 392f  tics/article/39/
-00000b30: 312f 6274 6164 3031 342f 3639 3839 3632  1/btad014/698962
-00000b40: 3122 3e6d 696e 6970 726f 743c 2f61 3e20  1">miniprot</a> 
-00000b50: 2863 7265 6469 7473 2074 6f20 3c61 2063  (credits to <a c
-00000b60: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
-00000b70: 6578 7465 726e 616c 2220 6872 6566 3d22  external" href="
-00000b80: 6874 7470 3a2f 2f6c 6968 656e 672e 6f72  http://liheng.or
-00000b90: 6722 3e44 722e 2048 656e 6720 4c69 3c2f  g">Dr. Heng Li</
-00000ba0: 613e 292c 2061 6e64 2065 6d70 6c6f 7973  a>), and employs
-00000bb0: 2061 203c 6120 636c 6173 733d 2272 6566   a <a class="ref
-00000bc0: 6572 656e 6365 2069 6e74 6572 6e61 6c22  erence internal"
-00000bd0: 2068 7265 663d 2268 7474 703a 2f2f 6363   href="http://cc
-00000be0: 622e 6a68 752e 6564 752f 6c69 6674 6f6e  b.jhu.edu/lifton
-00000bf0: 2f63 6f6e 7465 6e74 2f62 6568 696e 645f  /content/behind_
-00000c00: 7363 656e 6573 2e68 746d 6c23 7072 6f74  scenes.html#prot
-00000c10: 6569 6e2d 6d61 7869 6d69 7a61 7469 6f6e  ein-maximization
-00000c20: 2d61 6c67 6f72 6974 686d 223e 3c73 7061  -algorithm"><spa
-00000c30: 6e20 636c 6173 733d 2273 7464 2073 7464  n class="std std
-00000c40: 2d72 6566 223e 5072 6f74 6569 6e2d 6d61  -ref">Protein-ma
-00000c50: 7869 6d69 7a61 7469 6f6e 2061 6c67 6f72  ximization algor
-00000c60: 6974 686d 3c2f 7370 616e 3e3c 2f61 3e20  ithm</span></a> 
-00000c70: 746f 2069 6d70 726f 7665 2074 6865 2070  to improve the p
-00000c80: 726f 7465 696e 2d63 6f64 696e 6720 6765  rotein-coding ge
-00000c90: 6e65 206c 6966 742d 6f76 6572 2070 726f  ne lift-over pro
-00000ca0: 6365 7373 2e3c 2f70 3e0a 3c73 6563 7469  cess.</p>.<secti
-00000cb0: 6f6e 2069 643d 2277 6879 2d6c 6966 746f  on id="why-lifto
-00000cc0: 6e22 2063 6c61 7373 3d22 223e 0a3c 6832  n" class="">.<h2
-00000cd0: 3e57 6879 204c 6966 744f 6ee2 9d93 3c61  >Why LiftOn...<a
-00000ce0: 2063 6c61 7373 3d22 6865 6164 6572 6c69   class="headerli
-00000cf0: 6e6b 2220 6872 6566 3d22 2377 6879 2d6c  nk" href="#why-l
-00000d00: 6966 746f 6e22 2074 6974 6c65 3d22 5065  ifton" title="Pe
-00000d10: 726d 616c 696e 6b20 746f 2074 6869 7320  rmalink to this 
-00000d20: 6865 6164 696e 6722 3e23 3c2f 613e 3c2f  heading">#</a></
-00000d30: 6832 3e0a 3c6f 6c20 636c 6173 733d 2261  h2>.<ol class="a
-00000d40: 7261 6269 6320 7369 6d70 6c65 223e 0a3c  rabic simple">.<
-00000d50: 6c69 3e3c 703e 3c73 7472 6f6e 673e 4275  li><p><strong>Bu
-00000d60: 7267 656f 6e69 6e67 206e 756d 6265 7220  rgeoning number 
-00000d70: 6f66 2067 656e 6f6d 6520 6173 7365 6d62  of genome assemb
-00000d80: 6c69 6573 3c2f 7374 726f 6e67 3e3a 2041  lies</strong>: A
-00000d90: 7320 6f66 2044 6563 656d 6265 7220 3230  s of December 20
-00000da0: 3233 2c20 616d 6f6e 6720 7468 6520 3135  23, among the 15
-00000db0: 2c35 3738 2064 6973 7469 6e63 7420 6575  ,578 distinct eu
-00000dc0: 6b61 7279 6f74 6963 2067 656e 6f6d 6573  karyotic genomes
-00000dd0: 2c20 6f6e 6c79 2031 2c31 3131 2068 6176  , only 1,111 hav
-00000de0: 6520 6265 656e 2061 6e6e 6f74 6174 6564  e been annotated
-00000df0: 2028 3c61 2063 6c61 7373 3d22 7265 6665   (<a class="refe
-00000e00: 7265 6e63 6520 6578 7465 726e 616c 2220  rence external" 
-00000e10: 6872 6566 3d22 6874 7470 733a 2f2f 7777  href="https://ww
-00000e20: 772e 6e63 6269 2e6e 6c6d 2e6e 6968 2e67  w.ncbi.nlm.nih.g
-00000e30: 6f76 2f67 656e 6f6d 652f 616e 6e6f 7461  ov/genome/annota
-00000e40: 7469 6f6e 5f65 756b 2f23 6772 6170 6873  tion_euk/#graphs
-00000e50: 223e 4575 6b61 7279 6f74 6963 2047 656e  ">Eukaryotic Gen
-00000e60: 6f6d 6520 416e 6e6f 7461 7469 6f6e 2061  ome Annotation a
-00000e70: 7420 4e43 4249 3c2f 613e 292e 204d 6f72  t NCBI</a>). Mor
-00000e80: 6520 616e 6420 6d6f 7265 2068 6967 6820  e and more high 
-00000e90: 7175 616c 6974 7920 6173 7365 6d62 6c69  quality assembli
-00000ea0: 6573 2061 7265 2067 656e 6572 6174 6564  es are generated
-00000eb0: 2e20 5765 206e 6565 6420 746f 2061 6363  . We need to acc
-00000ec0: 7572 6174 656c 7920 616e 6e6f 7461 7465  urately annotate
-00000ed0: 2074 6865 6d2e 3c2f 703e 3c2f 6c69 3e0a   them.</p></li>.
-00000ee0: 3c6c 693e 3c70 3e3c 7374 726f 6e67 3e49  <li><p><strong>I
-00000ef0: 6d70 726f 7665 6420 7072 6f74 6569 6e2d  mproved protein-
-00000f00: 636f 6469 6e67 2067 656e 6520 6d61 7070  coding gene mapp
-00000f10: 696e 673c 2f73 7472 6f6e 673e 3a20 5468  ing</strong>: Th
-00000f20: 6520 706f 7075 6c61 7220 3c61 2063 6c61  e popular <a cla
-00000f30: 7373 3d22 7265 6665 7265 6e63 6520 6578  ss="reference ex
-00000f40: 7465 726e 616c 2220 6872 6566 3d22 6874  ternal" href="ht
-00000f50: 7470 733a 2f2f 6163 6164 656d 6963 2e6f  tps://academic.o
-00000f60: 7570 2e63 6f6d 2f62 696f 696e 666f 726d  up.com/bioinform
-00000f70: 6174 6963 732f 6172 7469 636c 652f 3337  atics/article/37
-00000f80: 2f31 322f 3136 3339 2f36 3033 3531 3238  /12/1639/6035128
-00000f90: 3f6c 6f67 696e 3d74 7275 6522 3e4c 6966  ?login=true">Lif
-00000fa0: 746f 6666 3c2f 613e 206d 6170 2067 656e  toff</a> map gen
-00000fb0: 6573 206f 6e6c 7920 6261 7365 6420 6f6e  es only based on
-00000fc0: 2074 6865 2044 4e41 2061 6c69 676e 6d65   the DNA alignme
-00000fd0: 6e74 2e20 5769 7468 2074 6865 2070 726f  nt. With the pro
-00000fe0: 7465 696e 2d74 6f2d 6765 6e6f 6d65 2061  tein-to-genome a
-00000ff0: 6c69 676e 6d65 6e74 2c20 4c69 6674 4f6e  lignment, LiftOn
-00001000: 2069 7320 6162 6c65 2074 6f20 6675 7274   is able to furt
-00001010: 6865 7220 696d 7072 6f76 6520 7468 6520  her improve the 
-00001020: 6c69 6674 2d6f 7665 7220 7072 6f74 6569  lift-over protei
-00001030: 6e2d 636f 6469 6e67 2067 656e 6520 616e  n-coding gene an
-00001040: 6e6f 7461 7469 6f6e 732e 204c 6966 744f  notations. LiftO
-00001050: 6e20 696d 7072 6f76 6573 2074 6865 2063  n improves the c
-00001060: 7572 7265 6e74 2072 656c 6561 7365 6420  urrent released 
-00001070: 5432 542d 4348 4d31 3320 616e 6e6f 7461  T2T-CHM13 annota
-00001080: 7469 6f6e 2028 3c61 2063 6c61 7373 3d22  tion (<a class="
-00001090: 7265 6665 7265 6e63 6520 6578 7465 726e  reference extern
-000010a0: 616c 2220 6872 6566 3d22 6874 7470 733a  al" href="https:
-000010b0: 2f2f 7333 2d75 732d 7765 7374 2d32 2e61  //s3-us-west-2.a
-000010c0: 6d61 7a6f 6e61 7773 2e63 6f6d 2f68 756d  mazonaws.com/hum
-000010d0: 616e 2d70 616e 6765 6e6f 6d69 6373 2f54  an-pangenomics/T
-000010e0: 3254 2f43 484d 3133 2f61 7373 656d 626c  2T/CHM13/assembl
-000010f0: 6965 732f 616e 6e6f 7461 7469 6f6e 2f63  ies/annotation/c
-00001100: 686d 3133 7632 2e30 5f52 6566 5365 715f  hm13v2.0_RefSeq_
-00001110: 4c69 6674 6f66 665f 7635 2e31 2e67 6666  Liftoff_v5.1.gff
-00001120: 332e 677a 223e 4a48 5520 5265 6653 6571  3.gz">JHU RefSeq
-00001130: 7631 3130 202b 204c 6966 746f 6666 2076  v110 + Liftoff v
-00001140: 352e 313c 2f61 3e29 2e3c 2f70 3e3c 2f6c  5.1</a>).</p></l
-00001150: 693e 0a3c 6c69 3e3c 703e 3c73 7472 6f6e  i>.<li><p><stron
-00001160: 673e 496d 7072 6f76 6564 2064 6973 7461  g>Improved dista
-00001170: 6e74 2073 7065 6369 6573 206c 6966 742d  nt species lift-
-00001180: 6f76 6572 3c2f 7374 726f 6e67 3e3a 204c  over</strong>: L
-00001190: 6966 744f 6e20 6578 7465 6e64 7320 6672  iftOn extends fr
-000011a0: 6f6d 206c 6966 742d 6f76 6572 2062 6574  om lift-over bet
-000011b0: 7765 656e 2074 6865 2073 616d 6520 6f72  ween the same or
-000011c0: 2063 6c6f 7365 6c79 2072 656c 6174 6564   closely related
-000011d0: 2073 7065 6369 6573 2074 6f20 6d6f 7265   species to more
-000011e0: 2064 6973 7461 6e74 6c79 2072 656c 6174   distantly relat
-000011f0: 6564 2073 7065 6369 6573 2e20 5365 6520  ed species. See 
-00001200: 3c73 7061 6e20 636c 6173 733d 2278 7265  <span class="xre
-00001210: 6620 7374 6420 7374 642d 7265 6622 3e6d  f std std-ref">m
-00001220: 6f75 7365 5f32 5f72 6174 3c2f 7370 616e  ouse_2_rat</span
-00001230: 3e20 616e 6420 3c73 7061 6e20 636c 6173  > and <span clas
-00001240: 733d 2278 7265 6620 7374 6420 7374 642d  s="xref std std-
-00001250: 7265 6622 3e64 726f 736f 7068 696c 615f  ref">drosophila_
-00001260: 6d65 6c61 6e6f 6761 7374 6572 5f32 5f65  melanogaster_2_e
-00001270: 7265 6374 613c 2f73 7061 6e3e 206c 6966  recta</span> lif
-00001280: 742d 6f76 6572 2073 6563 7469 6f6e 732e  t-over sections.
-00001290: 3c2f 703e 3c2f 6c69 3e0a 3c2f 6f6c 3e0a  </p></li>.</ol>.
-000012a0: 3c70 3e4c 6966 744f 6e20 6973 2066 7265  <p>LiftOn is fre
-000012b0: 652c 2069 7427 7320 6f70 656e 2073 6f75  e, it's open sou
-000012c0: 7263 652c 2069 7427 7320 6561 7379 2074  rce, it's easy t
-000012d0: 6f20 696e 7374 616c 6c20 2c20 616e 6420  o install , and 
-000012e0: 6974 2773 2069 6e20 5079 7468 6f6e 213c  it's in Python!<
-000012f0: 2f70 3e0a 3c64 6976 2063 6c61 7373 3d22  /p>.<div class="
-00001300: 6c69 6e65 2d62 6c6f 636b 223e 0a3c 6469  line-block">.<di
-00001310: 7620 636c 6173 733d 226c 696e 6522 3e3c  v class="line"><
-00001320: 6272 3e3c 2f64 6976 3e0a 3c2f 6469 763e  br></div>.</div>
-00001330: 0a3c 2f73 6563 7469 6f6e 3e0a 3c73 6563  .</section>.<sec
-00001340: 7469 6f6e 2069 643d 2277 686f 2d69 732d  tion id="who-is-
-00001350: 6974 2d66 6f72 2220 636c 6173 733d 2222  it-for" class=""
-00001360: 3e0a 3c68 323e 5768 6f20 6973 2069 7420  >.<h2>Who is it 
-00001370: 666f 72e2 9d93 3c61 2063 6c61 7373 3d22  for...<a class="
-00001380: 6865 6164 6572 6c69 6e6b 2220 6872 6566  headerlink" href
-00001390: 3d22 2377 686f 2d69 732d 6974 2d66 6f72  ="#who-is-it-for
-000013a0: 2220 7469 746c 653d 2250 6572 6d61 6c69  " title="Permali
-000013b0: 6e6b 2074 6f20 7468 6973 2068 6561 6469  nk to this headi
-000013c0: 6e67 223e 233c 2f61 3e3c 2f68 323e 0a3c  ng">#</a></h2>.<
-000013d0: 6f6c 2063 6c61 7373 3d22 6172 6162 6963  ol class="arabic
-000013e0: 2073 696d 706c 6522 3e0a 3c6c 693e 3c70   simple">.<li><p
-000013f0: 3e49 6620 796f 7520 6861 7665 2073 6571  >If you have seq
-00001400: 7565 6e63 6564 2061 6e64 2061 7373 656d  uenced and assem
-00001410: 626c 6564 2061 206e 6577 2067 656e 6f6d  bled a new genom
-00001420: 6520 616e 6420 6e65 6564 2074 6f20 616e  e and need to an
-00001430: 6e6f 7461 7465 2069 742c 204c 6966 744f  notate it, LiftO
-00001440: 6e20 6973 2074 6865 2069 6465 616c 2063  n is the ideal c
-00001450: 686f 6963 6520 666f 7220 6765 6e65 7261  hoice for genera
-00001460: 7469 6e67 2061 6e6e 6f74 6174 696f 6e73  ting annotations
-00001470: 2e3c 2f70 3e3c 2f6c 693e 0a3c 6c69 3e3c  .</p></li>.<li><
-00001480: 703e 4966 2079 6f75 2077 616e 7420 746f  p>If you want to
-00001490: 2064 6f20 636f 6d70 6172 6174 6976 6520   do comparative 
-000014a0: 6765 6e6f 6d69 6373 2061 6e61 6c79 7369  genomics analysi
-000014b0: 732c 2072 756e 206c 6966 744f 6e20 746f  s, run liftOn to
-000014c0: 206c 6966 742d 6f76 6572 2061 6e64 2063   lift-over and c
-000014d0: 6f6d 7061 7265 2061 6e6e 6f74 6174 696f  ompare annotatio
-000014e0: 6e73 213c 2f70 3e3c 2f6c 693e 0a3c 6c69  ns!</p></li>.<li
-000014f0: 3e3c 703e 4966 2079 6f75 2077 6973 6820  ><p>If you wish 
-00001500: 746f 2075 7469 6c69 7a65 2074 6865 2066  to utilize the f
-00001510: 696e 6573 7420 4348 4d31 3320 616e 6e6f  inest CHM13 anno
-00001520: 7461 7469 6f6e 2c20 796f 7520 6361 6e20  tation, you can 
-00001530: 7275 6e20 4c69 6674 4f6e 2120 5765 2068  run LiftOn! We h
-00001540: 6176 6520 616c 736f 2070 7265 2d67 656e  ave also pre-gen
-00001550: 6572 6174 6564 2074 6865 203c 6120 636c  erated the <a cl
-00001560: 6173 733d 2272 6566 6572 656e 6365 2065  ass="reference e
-00001570: 7874 6572 6e61 6c22 2068 7265 663d 2268  xternal" href="h
-00001580: 7474 7073 3a2f 2f6b 6863 6861 6f2e 636f  ttps://khchao.co
-00001590: 6d22 3e54 3254 5f43 484d 3133 5f4c 6966  m">T2T_CHM13_Lif
-000015a0: 744f 6e2e 6766 6633 3c2f 613e 2066 696c  tOn.gff3</a> fil
-000015b0: 6520 666f 7220 796f 7572 2063 6f6e 7665  e for your conve
-000015c0: 6e69 656e 6365 2e3c 2f70 3e3c 2f6c 693e  nience.</p></li>
-000015d0: 0a3c 2f6f 6c3e 0a3c 6469 7620 636c 6173  .</ol>.<div clas
-000015e0: 733d 226c 696e 652d 626c 6f63 6b22 3e0a  s="line-block">.
-000015f0: 3c64 6976 2063 6c61 7373 3d22 6c69 6e65  <div class="line
-00001600: 223e 3c62 723e 3c2f 6469 763e 0a3c 2f64  "><br></div>.</d
-00001610: 6976 3e0a 3c2f 7365 6374 696f 6e3e 0a3c  iv>.</section>.<
-00001620: 7365 6374 696f 6e20 6964 3d22 7768 6174  section id="what
-00001630: 2d64 6f65 732d 6c69 6674 6f6e 2d64 6f22  -does-lifton-do"
-00001640: 2063 6c61 7373 3d22 223e 0a3c 6832 3e57   class="">.<h2>W
-00001650: 6861 7420 646f 6573 204c 6966 744f 6e20  hat does LiftOn 
-00001660: 646f e29d 933c 6120 636c 6173 733d 2268  do...<a class="h
-00001670: 6561 6465 726c 696e 6b22 2068 7265 663d  eaderlink" href=
-00001680: 2223 7768 6174 2d64 6f65 732d 6c69 6674  "#what-does-lift
-00001690: 6f6e 2d64 6f22 2074 6974 6c65 3d22 5065  on-do" title="Pe
-000016a0: 726d 616c 696e 6b20 746f 2074 6869 7320  rmalink to this 
-000016b0: 6865 6164 696e 6722 3e23 3c2f 613e 3c2f  heading">#</a></
-000016c0: 6832 3e0a 3c70 3e47 6976 656e 2061 2072  h2>.<p>Given a r
-000016d0: 6566 6572 656e 6365 203c 7374 726f 6e67  eference <strong
-000016e0: 3e47 656e 6f6d 653c 2f73 7472 6f6e 673e  >Genome</strong>
-000016f0: 203c 7370 616e 2063 6c61 7373 3d22 6d61   <span class="ma
-00001700: 7468 206e 6f74 7261 6e73 6c61 7465 206e  th notranslate n
-00001710: 6f68 6967 686c 6967 6874 223e 3c6d 6a78  ohighlight"><mjx
-00001720: 2d63 6f6e 7461 696e 6572 2063 6c61 7373  -container class
-00001730: 3d22 4d61 7468 4a61 7820 4374 7874 4d65  ="MathJax CtxtMe
-00001740: 6e75 5f41 7474 6163 6865 645f 3022 206a  nu_Attached_0" j
-00001750: 6178 3d22 4348 544d 4c22 2074 6162 696e  ax="CHTML" tabin
-00001760: 6465 783d 2230 2220 6374 7874 6d65 6e75  dex="0" ctxtmenu
-00001770: 5f63 6f75 6e74 6572 3d22 3022 2073 7479  _counter="0" sty
-00001780: 6c65 3d22 666f 6e74 2d73 697a 653a 2031  le="font-size: 1
-00001790: 3139 253b 2070 6f73 6974 696f 6e3a 2072  19%; position: r
-000017a0: 656c 6174 6976 653b 223e 3c6d 6a78 2d6d  elative;"><mjx-m
-000017b0: 6174 6820 636c 6173 733d 224d 4a58 2d54  ath class="MJX-T
-000017c0: 4558 2220 6172 6961 2d68 6964 6465 6e3d  EX" aria-hidden=
-000017d0: 2274 7275 6522 3e3c 6d6a 782d 6d69 2063  "true"><mjx-mi c
-000017e0: 6c61 7373 3d22 6d6a 782d 6922 3e3c 6d6a  lass="mjx-i"><mj
-000017f0: 782d 6320 636c 6173 733d 226d 6a78 2d63  x-c class="mjx-c
-00001800: 3144 3434 3520 5445 582d 4922 3e3c 2f6d  1D445 TEX-I"></m
-00001810: 6a78 2d63 3e3c 2f6d 6a78 2d6d 693e 3c2f  jx-c></mjx-mi></
-00001820: 6d6a 782d 6d61 7468 3e3c 6d6a 782d 6173  mjx-math><mjx-as
-00001830: 7369 7374 6976 652d 6d6d 6c20 756e 7365  sistive-mml unse
-00001840: 6c65 6374 6162 6c65 3d22 6f6e 2220 6469  lectable="on" di
-00001850: 7370 6c61 793d 2269 6e6c 696e 6522 3e3c  splay="inline"><
-00001860: 6d61 7468 2078 6d6c 6e73 3d22 6874 7470  math xmlns="http
-00001870: 3a2f 2f77 7777 2e77 332e 6f72 672f 3139  ://www.w3.org/19
-00001880: 3938 2f4d 6174 682f 4d61 7468 4d4c 223e  98/Math/MathML">
-00001890: 3c6d 693e 523c 2f6d 693e 3c2f 6d61 7468  <mi>R</mi></math
-000018a0: 3e3c 2f6d 6a78 2d61 7373 6973 7469 7665  ></mjx-assistive
-000018b0: 2d6d 6d6c 3e3c 2f6d 6a78 2d63 6f6e 7461  -mml></mjx-conta
-000018c0: 696e 6572 3e3c 2f73 7061 6e3e 2c20 616e  iner></span>, an
-000018d0: 203c 7374 726f 6e67 3e41 6e6e 6f74 6174   <strong>Annotat
-000018e0: 696f 6e3c 2f73 7472 6f6e 673e 203c 7370  ion</strong> <sp
-000018f0: 616e 2063 6c61 7373 3d22 6d61 7468 206e  an class="math n
-00001900: 6f74 7261 6e73 6c61 7465 206e 6f68 6967  otranslate nohig
-00001910: 686c 6967 6874 223e 3c6d 6a78 2d63 6f6e  hlight"><mjx-con
-00001920: 7461 696e 6572 2063 6c61 7373 3d22 4d61  tainer class="Ma
-00001930: 7468 4a61 7820 4374 7874 4d65 6e75 5f41  thJax CtxtMenu_A
-00001940: 7474 6163 6865 645f 3022 206a 6178 3d22  ttached_0" jax="
-00001950: 4348 544d 4c22 2074 6162 696e 6465 783d  CHTML" tabindex=
-00001960: 2230 2220 6374 7874 6d65 6e75 5f63 6f75  "0" ctxtmenu_cou
-00001970: 6e74 6572 3d22 3122 2073 7479 6c65 3d22  nter="1" style="
-00001980: 666f 6e74 2d73 697a 653a 2031 3139 253b  font-size: 119%;
-00001990: 2070 6f73 6974 696f 6e3a 2072 656c 6174   position: relat
-000019a0: 6976 653b 223e 3c6d 6a78 2d6d 6174 6820  ive;"><mjx-math 
-000019b0: 636c 6173 733d 224d 4a58 2d54 4558 2220  class="MJX-TEX" 
-000019c0: 6172 6961 2d68 6964 6465 6e3d 2274 7275  aria-hidden="tru
-000019d0: 6522 3e3c 6d6a 782d 6d73 7562 3e3c 6d6a  e"><mjx-msub><mj
-000019e0: 782d 6d69 2063 6c61 7373 3d22 6d6a 782d  x-mi class="mjx-
-000019f0: 6922 3e3c 6d6a 782d 6320 636c 6173 733d  i"><mjx-c class=
-00001a00: 226d 6a78 2d63 3144 3434 3520 5445 582d  "mjx-c1D445 TEX-
-00001a10: 4922 3e3c 2f6d 6a78 2d63 3e3c 2f6d 6a78  I"></mjx-c></mjx
-00001a20: 2d6d 693e 3c6d 6a78 2d73 6372 6970 7420  -mi><mjx-script 
-00001a30: 7374 796c 653d 2276 6572 7469 6361 6c2d  style="vertical-
-00001a40: 616c 6967 6e3a 202d 302e 3135 3365 6d3b  align: -0.153em;
-00001a50: 223e 3c6d 6a78 2d6d 6920 636c 6173 733d  "><mjx-mi class=
-00001a60: 226d 6a78 2d69 2220 7369 7a65 3d22 7322  "mjx-i" size="s"
-00001a70: 3e3c 6d6a 782d 6320 636c 6173 733d 226d  ><mjx-c class="m
-00001a80: 6a78 2d63 3144 3433 3420 5445 582d 4922  jx-c1D434 TEX-I"
-00001a90: 3e3c 2f6d 6a78 2d63 3e3c 2f6d 6a78 2d6d  ></mjx-c></mjx-m
-00001aa0: 693e 3c2f 6d6a 782d 7363 7269 7074 3e3c  i></mjx-script><
-00001ab0: 2f6d 6a78 2d6d 7375 623e 3c2f 6d6a 782d  /mjx-msub></mjx-
-00001ac0: 6d61 7468 3e3c 6d6a 782d 6173 7369 7374  math><mjx-assist
-00001ad0: 6976 652d 6d6d 6c20 756e 7365 6c65 6374  ive-mml unselect
-00001ae0: 6162 6c65 3d22 6f6e 2220 6469 7370 6c61  able="on" displa
-00001af0: 793d 2269 6e6c 696e 6522 3e3c 6d61 7468  y="inline"><math
-00001b00: 2078 6d6c 6e73 3d22 6874 7470 3a2f 2f77   xmlns="http://w
-00001b10: 7777 2e77 332e 6f72 672f 3139 3938 2f4d  ww.w3.org/1998/M
-00001b20: 6174 682f 4d61 7468 4d4c 223e 3c6d 7375  ath/MathML"><msu
-00001b30: 623e 3c6d 693e 523c 2f6d 693e 3c6d 693e  b><mi>R</mi><mi>
-00001b40: 413c 2f6d 693e 3c2f 6d73 7562 3e3c 2f6d  A</mi></msub></m
-00001b50: 6174 683e 3c2f 6d6a 782d 6173 7369 7374  ath></mjx-assist
-00001b60: 6976 652d 6d6d 6c3e 3c2f 6d6a 782d 636f  ive-mml></mjx-co
-00001b70: 6e74 6169 6e65 723e 3c2f 7370 616e 3e2c  ntainer></span>,
-00001b80: 2061 6e64 2061 2074 6172 6765 7420 3c73   and a target <s
-00001b90: 7472 6f6e 673e 4765 6e6f 6d65 3c2f 7374  trong>Genome</st
-00001ba0: 726f 6e67 3e20 3c73 7061 6e20 636c 6173  rong> <span clas
-00001bb0: 733d 226d 6174 6820 6e6f 7472 616e 736c  s="math notransl
-00001bc0: 6174 6520 6e6f 6869 6768 6c69 6768 7422  ate nohighlight"
-00001bd0: 3e3c 6d6a 782d 636f 6e74 6169 6e65 7220  ><mjx-container 
-00001be0: 636c 6173 733d 224d 6174 684a 6178 2043  class="MathJax C
-00001bf0: 7478 744d 656e 755f 4174 7461 6368 6564  txtMenu_Attached
-00001c00: 5f30 2220 6a61 783d 2243 4854 4d4c 2220  _0" jax="CHTML" 
-00001c10: 7461 6269 6e64 6578 3d22 3022 2063 7478  tabindex="0" ctx
-00001c20: 746d 656e 755f 636f 756e 7465 723d 2232  tmenu_counter="2
-00001c30: 2220 7374 796c 653d 2266 6f6e 742d 7369  " style="font-si
-00001c40: 7a65 3a20 3131 3925 3b20 706f 7369 7469  ze: 119%; positi
-00001c50: 6f6e 3a20 7265 6c61 7469 7665 3b22 3e3c  on: relative;"><
-00001c60: 6d6a 782d 6d61 7468 2063 6c61 7373 3d22  mjx-math class="
-00001c70: 4d4a 582d 5445 5822 2061 7269 612d 6869  MJX-TEX" aria-hi
-00001c80: 6464 656e 3d22 7472 7565 223e 3c6d 6a78  dden="true"><mjx
-00001c90: 2d6d 6920 636c 6173 733d 226d 6a78 2d69  -mi class="mjx-i
-00001ca0: 223e 3c6d 6a78 2d63 2063 6c61 7373 3d22  "><mjx-c class="
-00001cb0: 6d6a 782d 6331 4434 3437 2054 4558 2d49  mjx-c1D447 TEX-I
-00001cc0: 223e 3c2f 6d6a 782d 633e 3c2f 6d6a 782d  "></mjx-c></mjx-
-00001cd0: 6d69 3e3c 2f6d 6a78 2d6d 6174 683e 3c6d  mi></mjx-math><m
-00001ce0: 6a78 2d61 7373 6973 7469 7665 2d6d 6d6c  jx-assistive-mml
-00001cf0: 2075 6e73 656c 6563 7461 626c 653d 226f   unselectable="o
-00001d00: 6e22 2064 6973 706c 6179 3d22 696e 6c69  n" display="inli
-00001d10: 6e65 223e 3c6d 6174 6820 786d 6c6e 733d  ne"><math xmlns=
-00001d20: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
-00001d30: 7267 2f31 3939 382f 4d61 7468 2f4d 6174  rg/1998/Math/Mat
-00001d40: 684d 4c22 3e3c 6d69 3e54 3c2f 6d69 3e3c  hML"><mi>T</mi><
-00001d50: 2f6d 6174 683e 3c2f 6d6a 782d 6173 7369  /math></mjx-assi
-00001d60: 7374 6976 652d 6d6d 6c3e 3c2f 6d6a 782d  stive-mml></mjx-
-00001d70: 636f 6e74 6169 6e65 723e 3c2f 7370 616e  container></span
-00001d80: 3e2e 2054 6865 206c 6966 742d 6f76 6572  >. The lift-over
-00001d90: 2070 726f 626c 656d 2069 7320 6465 6669   problem is defi
-00001da0: 6e65 6420 6173 2074 6865 2070 726f 6365  ned as the proce
-00001db0: 7373 206f 6620 6368 616e 6769 6e67 2074  ss of changing t
-00001dc0: 6865 2063 6f6f 7264 696e 6174 6573 206f  he coordinates o
-00001dd0: 6620 3c73 7472 6f6e 673e 416e 6e6f 7461  f <strong>Annota
-00001de0: 7469 6f6e 3c2f 7374 726f 6e67 3e20 3c73  tion</strong> <s
-00001df0: 7061 6e20 636c 6173 733d 226d 6174 6820  pan class="math 
-00001e00: 6e6f 7472 616e 736c 6174 6520 6e6f 6869  notranslate nohi
-00001e10: 6768 6c69 6768 7422 3e3c 6d6a 782d 636f  ghlight"><mjx-co
-00001e20: 6e74 6169 6e65 7220 636c 6173 733d 224d  ntainer class="M
-00001e30: 6174 684a 6178 2043 7478 744d 656e 755f  athJax CtxtMenu_
-00001e40: 4174 7461 6368 6564 5f30 2220 6a61 783d  Attached_0" jax=
-00001e50: 2243 4854 4d4c 2220 7461 6269 6e64 6578  "CHTML" tabindex
-00001e60: 3d22 3022 2063 7478 746d 656e 755f 636f  ="0" ctxtmenu_co
-00001e70: 756e 7465 723d 2233 2220 7374 796c 653d  unter="3" style=
-00001e80: 2266 6f6e 742d 7369 7a65 3a20 3131 3925  "font-size: 119%
-00001e90: 3b20 706f 7369 7469 6f6e 3a20 7265 6c61  ; position: rela
-00001ea0: 7469 7665 3b22 3e3c 6d6a 782d 6d61 7468  tive;"><mjx-math
-00001eb0: 2063 6c61 7373 3d22 4d4a 582d 5445 5822   class="MJX-TEX"
-00001ec0: 2061 7269 612d 6869 6464 656e 3d22 7472   aria-hidden="tr
-00001ed0: 7565 223e 3c6d 6a78 2d6d 7375 623e 3c6d  ue"><mjx-msub><m
-00001ee0: 6a78 2d6d 6920 636c 6173 733d 226d 6a78  jx-mi class="mjx
-00001ef0: 2d69 223e 3c6d 6a78 2d63 2063 6c61 7373  -i"><mjx-c class
-00001f00: 3d22 6d6a 782d 6331 4434 3435 2054 4558  ="mjx-c1D445 TEX
-00001f10: 2d49 223e 3c2f 6d6a 782d 633e 3c2f 6d6a  -I"></mjx-c></mj
-00001f20: 782d 6d69 3e3c 6d6a 782d 7363 7269 7074  x-mi><mjx-script
-00001f30: 2073 7479 6c65 3d22 7665 7274 6963 616c   style="vertical
-00001f40: 2d61 6c69 676e 3a20 2d30 2e31 3533 656d  -align: -0.153em
-00001f50: 3b22 3e3c 6d6a 782d 6d69 2063 6c61 7373  ;"><mjx-mi class
-00001f60: 3d22 6d6a 782d 6922 2073 697a 653d 2273  ="mjx-i" size="s
-00001f70: 223e 3c6d 6a78 2d63 2063 6c61 7373 3d22  "><mjx-c class="
-00001f80: 6d6a 782d 6331 4434 3334 2054 4558 2d49  mjx-c1D434 TEX-I
-00001f90: 223e 3c2f 6d6a 782d 633e 3c2f 6d6a 782d  "></mjx-c></mjx-
-00001fa0: 6d69 3e3c 2f6d 6a78 2d73 6372 6970 743e  mi></mjx-script>
-00001fb0: 3c2f 6d6a 782d 6d73 7562 3e3c 2f6d 6a78  </mjx-msub></mjx
-00001fc0: 2d6d 6174 683e 3c6d 6a78 2d61 7373 6973  -math><mjx-assis
-00001fd0: 7469 7665 2d6d 6d6c 2075 6e73 656c 6563  tive-mml unselec
-00001fe0: 7461 626c 653d 226f 6e22 2064 6973 706c  table="on" displ
-00001ff0: 6179 3d22 696e 6c69 6e65 223e 3c6d 6174  ay="inline"><mat
-00002000: 6820 786d 6c6e 733d 2268 7474 703a 2f2f  h xmlns="http://
-00002010: 7777 772e 7733 2e6f 7267 2f31 3939 382f  www.w3.org/1998/
-00002020: 4d61 7468 2f4d 6174 684d 4c22 3e3c 6d73  Math/MathML"><ms
-00002030: 7562 3e3c 6d69 3e52 3c2f 6d69 3e3c 6d69  ub><mi>R</mi><mi
-00002040: 3e41 3c2f 6d69 3e3c 2f6d 7375 623e 3c2f  >A</mi></msub></
-00002050: 6d61 7468 3e3c 2f6d 6a78 2d61 7373 6973  math></mjx-assis
-00002060: 7469 7665 2d6d 6d6c 3e3c 2f6d 6a78 2d63  tive-mml></mjx-c
-00002070: 6f6e 7461 696e 6572 3e3c 2f73 7061 6e3e  ontainer></span>
-00002080: 2066 726f 6d20 3c73 7472 6f6e 673e 4765   from <strong>Ge
-00002090: 6e6f 6d65 3c2f 7374 726f 6e67 3e20 3c73  nome</strong> <s
-000020a0: 7061 6e20 636c 6173 733d 226d 6174 6820  pan class="math 
-000020b0: 6e6f 7472 616e 736c 6174 6520 6e6f 6869  notranslate nohi
-000020c0: 6768 6c69 6768 7422 3e3c 6d6a 782d 636f  ghlight"><mjx-co
-000020d0: 6e74 6169 6e65 7220 636c 6173 733d 224d  ntainer class="M
-000020e0: 6174 684a 6178 2043 7478 744d 656e 755f  athJax CtxtMenu_
-000020f0: 4174 7461 6368 6564 5f30 2220 6a61 783d  Attached_0" jax=
-00002100: 2243 4854 4d4c 2220 7461 6269 6e64 6578  "CHTML" tabindex
-00002110: 3d22 3022 2063 7478 746d 656e 755f 636f  ="0" ctxtmenu_co
-00002120: 756e 7465 723d 2234 2220 7374 796c 653d  unter="4" style=
-00002130: 2266 6f6e 742d 7369 7a65 3a20 3131 3925  "font-size: 119%
-00002140: 3b20 706f 7369 7469 6f6e 3a20 7265 6c61  ; position: rela
-00002150: 7469 7665 3b22 3e3c 6d6a 782d 6d61 7468  tive;"><mjx-math
-00002160: 2063 6c61 7373 3d22 4d4a 582d 5445 5822   class="MJX-TEX"
-00002170: 2061 7269 612d 6869 6464 656e 3d22 7472   aria-hidden="tr
-00002180: 7565 223e 3c6d 6a78 2d6d 6920 636c 6173  ue"><mjx-mi clas
-00002190: 733d 226d 6a78 2d69 223e 3c6d 6a78 2d63  s="mjx-i"><mjx-c
-000021a0: 2063 6c61 7373 3d22 6d6a 782d 6331 4434   class="mjx-c1D4
-000021b0: 3435 2054 4558 2d49 223e 3c2f 6d6a 782d  45 TEX-I"></mjx-
-000021c0: 633e 3c2f 6d6a 782d 6d69 3e3c 2f6d 6a78  c></mjx-mi></mjx
-000021d0: 2d6d 6174 683e 3c6d 6a78 2d61 7373 6973  -math><mjx-assis
-000021e0: 7469 7665 2d6d 6d6c 2075 6e73 656c 6563  tive-mml unselec
-000021f0: 7461 626c 653d 226f 6e22 2064 6973 706c  table="on" displ
-00002200: 6179 3d22 696e 6c69 6e65 223e 3c6d 6174  ay="inline"><mat
-00002210: 6820 786d 6c6e 733d 2268 7474 703a 2f2f  h xmlns="http://
-00002220: 7777 772e 7733 2e6f 7267 2f31 3939 382f  www.w3.org/1998/
-00002230: 4d61 7468 2f4d 6174 684d 4c22 3e3c 6d69  Math/MathML"><mi
-00002240: 3e52 3c2f 6d69 3e3c 2f6d 6174 683e 3c2f  >R</mi></math></
-00002250: 6d6a 782d 6173 7369 7374 6976 652d 6d6d  mjx-assistive-mm
-00002260: 6c3e 3c2f 6d6a 782d 636f 6e74 6169 6e65  l></mjx-containe
-00002270: 723e 3c2f 7370 616e 3e20 746f 203c 7374  r></span> to <st
-00002280: 726f 6e67 3e47 656e 6f6d 653c 2f73 7472  rong>Genome</str
-00002290: 6f6e 673e 203c 7370 616e 2063 6c61 7373  ong> <span class
-000022a0: 3d22 6d61 7468 206e 6f74 7261 6e73 6c61  ="math notransla
-000022b0: 7465 206e 6f68 6967 686c 6967 6874 223e  te nohighlight">
-000022c0: 3c6d 6a78 2d63 6f6e 7461 696e 6572 2063  <mjx-container c
-000022d0: 6c61 7373 3d22 4d61 7468 4a61 7820 4374  lass="MathJax Ct
-000022e0: 7874 4d65 6e75 5f41 7474 6163 6865 645f  xtMenu_Attached_
-000022f0: 3022 206a 6178 3d22 4348 544d 4c22 2074  0" jax="CHTML" t
-00002300: 6162 696e 6465 783d 2230 2220 6374 7874  abindex="0" ctxt
-00002310: 6d65 6e75 5f63 6f75 6e74 6572 3d22 3522  menu_counter="5"
-00002320: 2073 7479 6c65 3d22 666f 6e74 2d73 697a   style="font-siz
-00002330: 653a 2031 3139 253b 2070 6f73 6974 696f  e: 119%; positio
-00002340: 6e3a 2072 656c 6174 6976 653b 223e 3c6d  n: relative;"><m
-00002350: 6a78 2d6d 6174 6820 636c 6173 733d 224d  jx-math class="M
-00002360: 4a58 2d54 4558 2220 6172 6961 2d68 6964  JX-TEX" aria-hid
-00002370: 6465 6e3d 2274 7275 6522 3e3c 6d6a 782d  den="true"><mjx-
-00002380: 6d69 2063 6c61 7373 3d22 6d6a 782d 6922  mi class="mjx-i"
-00002390: 3e3c 6d6a 782d 6320 636c 6173 733d 226d  ><mjx-c class="m
-000023a0: 6a78 2d63 3144 3434 3720 5445 582d 4922  jx-c1D447 TEX-I"
-000023b0: 3e3c 2f6d 6a78 2d63 3e3c 2f6d 6a78 2d6d  ></mjx-c></mjx-m
-000023c0: 693e 3c2f 6d6a 782d 6d61 7468 3e3c 6d6a  i></mjx-math><mj
-000023d0: 782d 6173 7369 7374 6976 652d 6d6d 6c20  x-assistive-mml 
-000023e0: 756e 7365 6c65 6374 6162 6c65 3d22 6f6e  unselectable="on
-000023f0: 2220 6469 7370 6c61 793d 2269 6e6c 696e  " display="inlin
-00002400: 6522 3e3c 6d61 7468 2078 6d6c 6e73 3d22  e"><math xmlns="
-00002410: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
-00002420: 672f 3139 3938 2f4d 6174 682f 4d61 7468  g/1998/Math/Math
-00002430: 4d4c 223e 3c6d 693e 543c 2f6d 693e 3c2f  ML"><mi>T</mi></
-00002440: 6d61 7468 3e3c 2f6d 6a78 2d61 7373 6973  math></mjx-assis
-00002450: 7469 7665 2d6d 6d6c 3e3c 2f6d 6a78 2d63  tive-mml></mjx-c
-00002460: 6f6e 7461 696e 6572 3e3c 2f73 7061 6e3e  ontainer></span>
-00002470: 2c20 616e 6420 6765 6e65 7261 7465 2061  , and generate a
-00002480: 206e 6577 2061 6e6e 6f74 6174 696f 6e20   new annotation 
-00002490: 6669 6c65 203c 7374 726f 6e67 3e41 6e6e  file <strong>Ann
-000024a0: 6f74 6174 696f 6e3c 2f73 7472 6f6e 673e  otation</strong>
-000024b0: 203c 7370 616e 2063 6c61 7373 3d22 6d61   <span class="ma
-000024c0: 7468 206e 6f74 7261 6e73 6c61 7465 206e  th notranslate n
-000024d0: 6f68 6967 686c 6967 6874 223e 3c6d 6a78  ohighlight"><mjx
-000024e0: 2d63 6f6e 7461 696e 6572 2063 6c61 7373  -container class
-000024f0: 3d22 4d61 7468 4a61 7820 4374 7874 4d65  ="MathJax CtxtMe
-00002500: 6e75 5f41 7474 6163 6865 645f 3022 206a  nu_Attached_0" j
-00002510: 6178 3d22 4348 544d 4c22 2074 6162 696e  ax="CHTML" tabin
-00002520: 6465 783d 2230 2220 6374 7874 6d65 6e75  dex="0" ctxtmenu
-00002530: 5f63 6f75 6e74 6572 3d22 3622 2073 7479  _counter="6" sty
-00002540: 6c65 3d22 666f 6e74 2d73 697a 653a 2031  le="font-size: 1
-00002550: 3139 253b 2070 6f73 6974 696f 6e3a 2072  19%; position: r
-00002560: 656c 6174 6976 653b 223e 3c6d 6a78 2d6d  elative;"><mjx-m
-00002570: 6174 6820 636c 6173 733d 224d 4a58 2d54  ath class="MJX-T
-00002580: 4558 2220 6172 6961 2d68 6964 6465 6e3d  EX" aria-hidden=
-00002590: 2274 7275 6522 3e3c 6d6a 782d 6d73 7562  "true"><mjx-msub
-000025a0: 3e3c 6d6a 782d 6d69 2063 6c61 7373 3d22  ><mjx-mi class="
-000025b0: 6d6a 782d 6922 3e3c 6d6a 782d 6320 636c  mjx-i"><mjx-c cl
-000025c0: 6173 733d 226d 6a78 2d63 3144 3434 3720  ass="mjx-c1D447 
-000025d0: 5445 582d 4922 3e3c 2f6d 6a78 2d63 3e3c  TEX-I"></mjx-c><
-000025e0: 2f6d 6a78 2d6d 693e 3c6d 6a78 2d73 6372  /mjx-mi><mjx-scr
-000025f0: 6970 7420 7374 796c 653d 2276 6572 7469  ipt style="verti
-00002600: 6361 6c2d 616c 6967 6e3a 202d 302e 3135  cal-align: -0.15
-00002610: 3365 6d3b 206d 6172 6769 6e2d 6c65 6674  3em; margin-left
-00002620: 3a20 2d30 2e31 3265 6d3b 223e 3c6d 6a78  : -0.12em;"><mjx
-00002630: 2d6d 6920 636c 6173 733d 226d 6a78 2d69  -mi class="mjx-i
-00002640: 2220 7369 7a65 3d22 7322 3e3c 6d6a 782d  " size="s"><mjx-
-00002650: 6320 636c 6173 733d 226d 6a78 2d63 3144  c class="mjx-c1D
-00002660: 3433 3420 5445 582d 4922 3e3c 2f6d 6a78  434 TEX-I"></mjx
-00002670: 2d63 3e3c 2f6d 6a78 2d6d 693e 3c2f 6d6a  -c></mjx-mi></mj
-00002680: 782d 7363 7269 7074 3e3c 2f6d 6a78 2d6d  x-script></mjx-m
-00002690: 7375 623e 3c2f 6d6a 782d 6d61 7468 3e3c  sub></mjx-math><
-000026a0: 6d6a 782d 6173 7369 7374 6976 652d 6d6d  mjx-assistive-mm
-000026b0: 6c20 756e 7365 6c65 6374 6162 6c65 3d22  l unselectable="
-000026c0: 6f6e 2220 6469 7370 6c61 793d 2269 6e6c  on" display="inl
-000026d0: 696e 6522 3e3c 6d61 7468 2078 6d6c 6e73  ine"><math xmlns
-000026e0: 3d22 6874 7470 3a2f 2f77 7777 2e77 332e  ="http://www.w3.
-000026f0: 6f72 672f 3139 3938 2f4d 6174 682f 4d61  org/1998/Math/Ma
-00002700: 7468 4d4c 223e 3c6d 7375 623e 3c6d 693e  thML"><msub><mi>
-00002710: 543c 2f6d 693e 3c6d 693e 413c 2f6d 693e  T</mi><mi>A</mi>
-00002720: 3c2f 6d73 7562 3e3c 2f6d 6174 683e 3c2f  </msub></math></
-00002730: 6d6a 782d 6173 7369 7374 6976 652d 6d6d  mjx-assistive-mm
-00002740: 6c3e 3c2f 6d6a 782d 636f 6e74 6169 6e65  l></mjx-containe
-00002750: 723e 3c2f 7370 616e 3e2e 2041 2073 696d  r></span>. A sim
-00002760: 706c 6520 696c 6c75 7374 7261 7469 6f6e  ple illustration
-00002770: 206f 6620 7468 6520 6c69 6674 2d6f 7665   of the lift-ove
-00002780: 7220 7072 6f62 6c65 6d20 6973 2073 686f  r problem is sho
-00002790: 776e 2069 6e20 3c61 2063 6c61 7373 3d22  wn in <a class="
-000027a0: 7265 6665 7265 6e63 6520 696e 7465 726e  reference intern
-000027b0: 616c 2220 6872 6566 3d22 236c 6966 746f  al" href="#lifto
-000027c0: 7665 722d 696c 6c75 7374 7261 7469 6f6e  ver-illustration
-000027d0: 223e 3c73 7061 6e20 636c 6173 733d 2273  "><span class="s
-000027e0: 7464 2073 7464 2d6e 756d 7265 6622 3e46  td std-numref">F
-000027f0: 6967 7572 6520 313c 2f73 7061 6e3e 3c2f  igure 1</span></
-00002800: 613e 2e3c 2f70 3e0a 3c66 6967 7572 6520  a>.</p>.<figure 
-00002810: 636c 6173 733d 2261 6c69 676e 2d63 656e  class="align-cen
-00002820: 7465 7222 2069 643d 2269 6435 223e 0a3c  ter" id="id5">.<
-00002830: 7370 616e 2069 643d 226c 6966 746f 7665  span id="liftove
-00002840: 722d 696c 6c75 7374 7261 7469 6f6e 223e  r-illustration">
-00002850: 3c2f 7370 616e 3e3c 6120 636c 6173 733d  </span><a class=
-00002860: 2272 6566 6572 656e 6365 2069 6e74 6572  "reference inter
-00002870: 6e61 6c20 696d 6167 652d 7265 6665 7265  nal image-refere
-00002880: 6e63 6522 2068 7265 663d 2267 7261 7068  nce" href="graph
-00002890: 6963 732f 6c69 6674 6f76 6572 5f69 6c6c  ics/liftover_ill
-000028a0: 7573 7472 6174 696f 6e2e 6769 6622 3e3c  ustration.gif"><
-000028b0: 696d 6720 616c 743d 2267 7261 7068 6963  img alt="graphic
-000028c0: 732f 6c69 6674 6f76 6572 5f69 6c6c 7573  s/liftover_illus
-000028d0: 7472 6174 696f 6e2e 6769 6622 2073 7263  tration.gif" src
-000028e0: 3d22 6772 6170 6869 6373 2f6c 6966 746f  ="graphics/lifto
-000028f0: 7665 725f 696c 6c75 7374 7261 7469 6f6e  ver_illustration
-00002900: 2e67 6966 2220 7374 796c 653d 2277 6964  .gif" style="wid
-00002910: 7468 3a20 3637 322e 3570 783b 2068 6569  th: 672.5px; hei
-00002920: 6768 743a 2032 3730 2e30 7078 3b22 3e3c  ght: 270.0px;"><
-00002930: 2f61 3e0a 3c66 6967 6361 7074 696f 6e3e  /a>.<figcaption>
-00002940: 0a3c 703e 3c73 7061 6e20 636c 6173 733d  .<p><span class=
-00002950: 2263 6170 7469 6f6e 2d6e 756d 6265 7222  "caption-number"
-00002960: 3e46 6967 7572 6520 3120 3c2f 7370 616e  >Figure 1 </span
-00002970: 3e3c 7370 616e 2063 6c61 7373 3d22 6361  ><span class="ca
-00002980: 7074 696f 6e2d 7465 7874 223e 496c 6c75  ption-text">Illu
-00002990: 7374 7261 7469 6f6e 206f 6620 7468 6520  stration of the 
-000029a0: 6c69 6674 2d6f 7665 7220 7072 6f62 6c65  lift-over proble
-000029b0: 6d2e 2054 6865 2061 6e6e 6f74 6174 696f  m. The annotatio
-000029c0: 6e20 6669 6c65 2066 726f 6d20 7468 6520  n file from the 
-000029d0: 7265 6665 7265 6e63 6520 6765 6e6f 6d65  reference genome
-000029e0: 2028 746f 7029 2069 7320 6c69 6674 6564   (top) is lifted
-000029f0: 206f 7665 7220 746f 2074 6865 2074 6172   over to the tar
-00002a00: 6765 7420 6765 6e6f 6d65 2028 626f 7474  get genome (bott
-00002a10: 6f6d 292e 3c2f 7370 616e 3e3c 6120 636c  om).</span><a cl
-00002a20: 6173 733d 2268 6561 6465 726c 696e 6b22  ass="headerlink"
-00002a30: 2068 7265 663d 2223 6964 3522 2074 6974   href="#id5" tit
-00002a40: 6c65 3d22 5065 726d 616c 696e 6b20 746f  le="Permalink to
-00002a50: 2074 6869 7320 696d 6167 6522 3e23 3c2f   this image">#</
-00002a60: 613e 3c2f 703e 0a3c 2f66 6967 6361 7074  a></p>.</figcapt
-00002a70: 696f 6e3e 0a3c 2f66 6967 7572 653e 0a3c  ion>.</figure>.<
-00002a80: 6469 7620 636c 6173 733d 226c 696e 652d  div class="line-
-00002a90: 626c 6f63 6b22 3e0a 3c64 6976 2063 6c61  block">.<div cla
-00002aa0: 7373 3d22 6c69 6e65 223e 3c62 723e 3c2f  ss="line"><br></
-00002ab0: 6469 763e 0a3c 2f64 6976 3e0a 3c70 3e4c  div>.</div>.<p>L
-00002ac0: 6966 744f 6e20 6973 2074 6865 2062 6573  iftOn is the bes
-00002ad0: 7420 746f 6f6c 2074 6f20 6865 6c70 2079  t tool to help y
-00002ae0: 6f75 2073 6f6c 7665 2074 6869 7320 7072  ou solve this pr
-00002af0: 6f62 6c65 6d21 204c 6966 744f 6e20 656d  oblem! LiftOn em
-00002b00: 706c 6f79 7320 6120 7477 6f2d 7374 6570  ploys a two-step
-00002b10: 203c 6120 636c 6173 733d 2272 6566 6572   <a class="refer
-00002b20: 656e 6365 2069 6e74 6572 6e61 6c22 2068  ence internal" h
-00002b30: 7265 663d 2268 7474 703a 2f2f 6363 622e  ref="http://ccb.
-00002b40: 6a68 752e 6564 752f 6c69 6674 6f6e 2f63  jhu.edu/lifton/c
-00002b50: 6f6e 7465 6e74 2f62 6568 696e 645f 7363  ontent/behind_sc
-00002b60: 656e 6573 2e68 746d 6c23 7072 6f74 6569  enes.html#protei
-00002b70: 6e2d 6d61 7869 6d69 7a61 7469 6f6e 2d61  n-maximization-a
-00002b80: 6c67 6f72 6974 686d 223e 3c73 7061 6e20  lgorithm"><span 
-00002b90: 636c 6173 733d 2273 7464 2073 7464 2d72  class="std std-r
-00002ba0: 6566 223e 7072 6f74 6569 6e20 6d61 7869  ef">protein maxi
-00002bb0: 6d69 7a61 7469 6f6e 2061 6c67 6f72 6974  mization algorit
-00002bc0: 686d 3c2f 7370 616e 3e3c 2f61 3e20 2850  hm</span></a> (P
-00002bd0: 4d20 616c 676f 7269 7468 6d29 2e3c 2f70  M algorithm).</p
-00002be0: 3e0a 3c6f 6c20 636c 6173 733d 2261 7261  >.<ol class="ara
-00002bf0: 6269 6320 7369 6d70 6c65 223e 0a3c 6c69  bic simple">.<li
-00002c00: 3e3c 703e 5468 6520 6669 7273 7420 6d6f  ><p>The first mo
-00002c10: 6475 6c65 2069 7320 7468 6520 3c65 6d3e  dule is the <em>
-00002c20: 6368 6169 6e69 6e67 2061 6c67 6f72 6974  chaining algorit
-00002c30: 686d 3c2f 656d 3e2e 2049 7420 7374 6172  hm</em>. It star
-00002c40: 7473 2062 7920 6578 7472 6163 7469 6e67  ts by extracting
-00002c50: 2070 726f 7465 696e 2073 6571 7565 6e63   protein sequenc
-00002c60: 6573 2061 6e6e 6f74 6174 6564 2062 7920  es annotated by 
-00002c70: 4c69 6674 6f66 6620 616e 6420 6d69 6e69  Liftoff and mini
-00002c80: 7072 6f74 2e20 4c69 6674 4f6e 2074 6865  prot. LiftOn the
-00002c90: 6e20 616c 6967 6e73 2074 6865 7365 2073  n aligns these s
-00002ca0: 6571 7565 6e63 6573 2074 6f20 6675 6c6c  equences to full
-00002cb0: 2d6c 656e 6774 6820 7265 6665 7265 6e63  -length referenc
-00002cc0: 6520 7072 6f74 6569 6e73 2e20 466f 7220  e proteins. For 
-00002cd0: 6561 6368 2067 656e 6520 6c6f 6375 732c  each gene locus,
-00002ce0: 204c 6966 744f 6e20 636f 6d70 6172 6573   LiftOn compares
-00002cf0: 2065 6163 6820 7365 6374 696f 6e20 6f66   each section of
-00002d00: 2074 6865 2070 726f 7465 696e 2061 6c69   the protein ali
-00002d10: 676e 6d65 6e74 7320 6672 6f6d 204c 6966  gnments from Lif
-00002d20: 746f 6666 2061 6e64 206d 696e 6970 726f  toff and minipro
-00002d30: 742c 2063 6861 696e 696e 6720 746f 6765  t, chaining toge
-00002d40: 7468 6572 2074 6865 2062 6573 7420 636f  ther the best co
-00002d50: 6d62 696e 6174 696f 6e73 2e3c 2f70 3e3c  mbinations.</p><
-00002d60: 2f6c 693e 0a3c 6c69 3e3c 703e 5468 6520  /li>.<li><p>The 
-00002d70: 7365 636f 6e64 206d 6f64 756c 6520 6973  second module is
-00002d80: 2074 6865 203c 656d 3e6f 7065 6e2d 7265   the <em>open-re
-00002d90: 6164 696e 6720 6672 616d 6520 7365 6172  ading frame sear
-00002da0: 6368 2028 4f52 4620 7365 6172 6368 2920  ch (ORF search) 
-00002db0: 616c 676f 7269 7468 6d3c 2f65 6d3e 2e20  algorithm</em>. 
-00002dc0: 496e 2074 6865 2063 6173 6520 6f66 2074  In the case of t
-00002dd0: 7275 6e63 6174 6564 2070 726f 7465 696e  runcated protein
-00002de0: 2d63 6f64 696e 6720 7472 616e 7363 7269  -coding transcri
-00002df0: 7074 732c 2074 6869 7320 616c 676f 7269  pts, this algori
-00002e00: 7468 6d20 6578 616d 696e 6573 2061 6c74  thm examines alt
-00002e10: 6572 6e61 7469 7665 2066 7261 6d65 7320  ernative frames 
-00002e20: 746f 2069 6465 6e74 6966 7920 7468 6520  to identify the 
-00002e30: 4f52 4620 7468 6174 2070 726f 6475 6365  ORF that produce
-00002e40: 7320 7468 6520 6c6f 6e67 6573 7420 6d61  s the longest ma
-00002e50: 7463 6820 7769 7468 2074 6865 2072 6566  tch with the ref
-00002e60: 6572 656e 6365 2070 726f 7465 696e 2e3c  erence protein.<
-00002e70: 2f70 3e3c 2f6c 693e 0a3c 2f6f 6c3e 0a3c  /p></li>.</ol>.<
-00002e80: 756c 2063 6c61 7373 3d22 7369 6d70 6c65  ul class="simple
-00002e90: 223e 0a3c 6c69 3e3c 646c 2063 6c61 7373  ">.<li><dl class
-00002ea0: 3d22 7369 6d70 6c65 223e 0a3c 6474 3e3c  ="simple">.<dt><
-00002eb0: 7374 726f 6e67 3e49 6e70 7574 3c2f 7374  strong>Input</st
-00002ec0: 726f 6e67 3e3a 3c2f 6474 3e3c 6464 3e3c  rong>:</dt><dd><
-00002ed0: 6f6c 2063 6c61 7373 3d22 6172 6162 6963  ol class="arabic
-00002ee0: 2073 696d 706c 6522 3e0a 3c6c 693e 3c70   simple">.<li><p
-00002ef0: 3e74 6172 6765 7420 3c73 7472 6f6e 673e  >target <strong>
-00002f00: 4765 6e6f 6d65 3c2f 7374 726f 6e67 3e20  Genome</strong> 
-00002f10: 3c73 7061 6e20 636c 6173 733d 226d 6174  <span class="mat
-00002f20: 6820 6e6f 7472 616e 736c 6174 6520 6e6f  h notranslate no
-00002f30: 6869 6768 6c69 6768 7422 3e3c 6d6a 782d  highlight"><mjx-
-00002f40: 636f 6e74 6169 6e65 7220 636c 6173 733d  container class=
-00002f50: 224d 6174 684a 6178 2043 7478 744d 656e  "MathJax CtxtMen
-00002f60: 755f 4174 7461 6368 6564 5f30 2220 6a61  u_Attached_0" ja
-00002f70: 783d 2243 4854 4d4c 2220 7461 6269 6e64  x="CHTML" tabind
-00002f80: 6578 3d22 3022 2063 7478 746d 656e 755f  ex="0" ctxtmenu_
-00002f90: 636f 756e 7465 723d 2237 2220 7374 796c  counter="7" styl
-00002fa0: 653d 2266 6f6e 742d 7369 7a65 3a20 3131  e="font-size: 11
-00002fb0: 3925 3b20 706f 7369 7469 6f6e 3a20 7265  9%; position: re
-00002fc0: 6c61 7469 7665 3b22 3e3c 6d6a 782d 6d61  lative;"><mjx-ma
-00002fd0: 7468 2063 6c61 7373 3d22 4d4a 582d 5445  th class="MJX-TE
-00002fe0: 5822 2061 7269 612d 6869 6464 656e 3d22  X" aria-hidden="
-00002ff0: 7472 7565 223e 3c6d 6a78 2d6d 6920 636c  true"><mjx-mi cl
-00003000: 6173 733d 226d 6a78 2d69 223e 3c6d 6a78  ass="mjx-i"><mjx
-00003010: 2d63 2063 6c61 7373 3d22 6d6a 782d 6331  -c class="mjx-c1
-00003020: 4434 3437 2054 4558 2d49 223e 3c2f 6d6a  D447 TEX-I"></mj
-00003030: 782d 633e 3c2f 6d6a 782d 6d69 3e3c 2f6d  x-c></mjx-mi></m
-00003040: 6a78 2d6d 6174 683e 3c6d 6a78 2d61 7373  jx-math><mjx-ass
-00003050: 6973 7469 7665 2d6d 6d6c 2075 6e73 656c  istive-mml unsel
-00003060: 6563 7461 626c 653d 226f 6e22 2064 6973  ectable="on" dis
-00003070: 706c 6179 3d22 696e 6c69 6e65 223e 3c6d  play="inline"><m
-00003080: 6174 6820 786d 6c6e 733d 2268 7474 703a  ath xmlns="http:
-00003090: 2f2f 7777 772e 7733 2e6f 7267 2f31 3939  //www.w3.org/199
-000030a0: 382f 4d61 7468 2f4d 6174 684d 4c22 3e3c  8/Math/MathML"><
-000030b0: 6d69 3e54 3c2f 6d69 3e3c 2f6d 6174 683e  mi>T</mi></math>
-000030c0: 3c2f 6d6a 782d 6173 7369 7374 6976 652d  </mjx-assistive-
-000030d0: 6d6d 6c3e 3c2f 6d6a 782d 636f 6e74 6169  mml></mjx-contai
-000030e0: 6e65 723e 3c2f 7370 616e 3e20 696e 2046  ner></span> in F
-000030f0: 4153 5441 2e3c 2f70 3e3c 2f6c 693e 0a3c  ASTA.</p></li>.<
-00003100: 6c69 3e3c 703e 7265 6665 7265 6e63 6520  li><p>reference 
-00003110: 3c73 7472 6f6e 673e 4765 6e6f 6d65 3c2f  <strong>Genome</
-00003120: 7374 726f 6e67 3e20 3c73 7061 6e20 636c  strong> <span cl
-00003130: 6173 733d 226d 6174 6820 6e6f 7472 616e  ass="math notran
-00003140: 736c 6174 6520 6e6f 6869 6768 6c69 6768  slate nohighligh
-00003150: 7422 3e3c 6d6a 782d 636f 6e74 6169 6e65  t"><mjx-containe
-00003160: 7220 636c 6173 733d 224d 6174 684a 6178  r class="MathJax
-00003170: 2043 7478 744d 656e 755f 4174 7461 6368   CtxtMenu_Attach
-00003180: 6564 5f30 2220 6a61 783d 2243 4854 4d4c  ed_0" jax="CHTML
-00003190: 2220 7461 6269 6e64 6578 3d22 3022 2063  " tabindex="0" c
-000031a0: 7478 746d 656e 755f 636f 756e 7465 723d  txtmenu_counter=
-000031b0: 2238 2220 7374 796c 653d 2266 6f6e 742d  "8" style="font-
-000031c0: 7369 7a65 3a20 3131 3925 3b20 706f 7369  size: 119%; posi
-000031d0: 7469 6f6e 3a20 7265 6c61 7469 7665 3b22  tion: relative;"
-000031e0: 3e3c 6d6a 782d 6d61 7468 2063 6c61 7373  ><mjx-math class
-000031f0: 3d22 4d4a 582d 5445 5822 2061 7269 612d  ="MJX-TEX" aria-
-00003200: 6869 6464 656e 3d22 7472 7565 223e 3c6d  hidden="true"><m
-00003210: 6a78 2d6d 6920 636c 6173 733d 226d 6a78  jx-mi class="mjx
-00003220: 2d69 223e 3c6d 6a78 2d63 2063 6c61 7373  -i"><mjx-c class
-00003230: 3d22 6d6a 782d 6331 4434 3435 2054 4558  ="mjx-c1D445 TEX
-00003240: 2d49 223e 3c2f 6d6a 782d 633e 3c2f 6d6a  -I"></mjx-c></mj
-00003250: 782d 6d69 3e3c 2f6d 6a78 2d6d 6174 683e  x-mi></mjx-math>
-00003260: 3c6d 6a78 2d61 7373 6973 7469 7665 2d6d  <mjx-assistive-m
-00003270: 6d6c 2075 6e73 656c 6563 7461 626c 653d  ml unselectable=
-00003280: 226f 6e22 2064 6973 706c 6179 3d22 696e  "on" display="in
-00003290: 6c69 6e65 223e 3c6d 6174 6820 786d 6c6e  line"><math xmln
-000032a0: 733d 2268 7474 703a 2f2f 7777 772e 7733  s="http://www.w3
-000032b0: 2e6f 7267 2f31 3939 382f 4d61 7468 2f4d  .org/1998/Math/M
-000032c0: 6174 684d 4c22 3e3c 6d69 3e52 3c2f 6d69  athML"><mi>R</mi
-000032d0: 3e3c 2f6d 6174 683e 3c2f 6d6a 782d 6173  ></math></mjx-as
-000032e0: 7369 7374 6976 652d 6d6d 6c3e 3c2f 6d6a  sistive-mml></mj
-000032f0: 782d 636f 6e74 6169 6e65 723e 3c2f 7370  x-container></sp
-00003300: 616e 3e20 696e 2046 4153 5441 3c2f 703e  an> in FASTA</p>
-00003310: 3c2f 6c69 3e0a 3c6c 693e 3c70 3e72 6566  </li>.<li><p>ref
-00003320: 6572 656e 6365 203c 7374 726f 6e67 3e41  erence <strong>A
-00003330: 6e6e 6f74 6174 696f 6e3c 2f73 7472 6f6e  nnotation</stron
-00003340: 673e 203c 7370 616e 2063 6c61 7373 3d22  g> <span class="
-00003350: 6d61 7468 206e 6f74 7261 6e73 6c61 7465  math notranslate
-00003360: 206e 6f68 6967 686c 6967 6874 223e 3c6d   nohighlight"><m
-00003370: 6a78 2d63 6f6e 7461 696e 6572 2063 6c61  jx-container cla
-00003380: 7373 3d22 4d61 7468 4a61 7820 4374 7874  ss="MathJax Ctxt
-00003390: 4d65 6e75 5f41 7474 6163 6865 645f 3022  Menu_Attached_0"
-000033a0: 206a 6178 3d22 4348 544d 4c22 2074 6162   jax="CHTML" tab
-000033b0: 696e 6465 783d 2230 2220 6374 7874 6d65  index="0" ctxtme
-000033c0: 6e75 5f63 6f75 6e74 6572 3d22 3922 2073  nu_counter="9" s
-000033d0: 7479 6c65 3d22 666f 6e74 2d73 697a 653a  tyle="font-size:
-000033e0: 2031 3139 253b 2070 6f73 6974 696f 6e3a   119%; position:
-000033f0: 2072 656c 6174 6976 653b 223e 3c6d 6a78   relative;"><mjx
-00003400: 2d6d 6174 6820 636c 6173 733d 224d 4a58  -math class="MJX
-00003410: 2d54 4558 2220 6172 6961 2d68 6964 6465  -TEX" aria-hidde
-00003420: 6e3d 2274 7275 6522 3e3c 6d6a 782d 6d73  n="true"><mjx-ms
-00003430: 7562 3e3c 6d6a 782d 6d69 2063 6c61 7373  ub><mjx-mi class
-00003440: 3d22 6d6a 782d 6922 3e3c 6d6a 782d 6320  ="mjx-i"><mjx-c 
-00003450: 636c 6173 733d 226d 6a78 2d63 3144 3434  class="mjx-c1D44
-00003460: 3520 5445 582d 4922 3e3c 2f6d 6a78 2d63  5 TEX-I"></mjx-c
-00003470: 3e3c 2f6d 6a78 2d6d 693e 3c6d 6a78 2d73  ></mjx-mi><mjx-s
-00003480: 6372 6970 7420 7374 796c 653d 2276 6572  cript style="ver
-00003490: 7469 6361 6c2d 616c 6967 6e3a 202d 302e  tical-align: -0.
-000034a0: 3135 3365 6d3b 223e 3c6d 6a78 2d6d 6920  153em;"><mjx-mi 
-000034b0: 636c 6173 733d 226d 6a78 2d69 2220 7369  class="mjx-i" si
-000034c0: 7a65 3d22 7322 3e3c 6d6a 782d 6320 636c  ze="s"><mjx-c cl
-000034d0: 6173 733d 226d 6a78 2d63 3144 3433 3420  ass="mjx-c1D434 
-000034e0: 5445 582d 4922 3e3c 2f6d 6a78 2d63 3e3c  TEX-I"></mjx-c><
-000034f0: 2f6d 6a78 2d6d 693e 3c2f 6d6a 782d 7363  /mjx-mi></mjx-sc
-00003500: 7269 7074 3e3c 2f6d 6a78 2d6d 7375 623e  ript></mjx-msub>
-00003510: 3c2f 6d6a 782d 6d61 7468 3e3c 6d6a 782d  </mjx-math><mjx-
-00003520: 6173 7369 7374 6976 652d 6d6d 6c20 756e  assistive-mml un
-00003530: 7365 6c65 6374 6162 6c65 3d22 6f6e 2220  selectable="on" 
-00003540: 6469 7370 6c61 793d 2269 6e6c 696e 6522  display="inline"
-00003550: 3e3c 6d61 7468 2078 6d6c 6e73 3d22 6874  ><math xmlns="ht
-00003560: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
-00003570: 3139 3938 2f4d 6174 682f 4d61 7468 4d4c  1998/Math/MathML
-00003580: 223e 3c6d 7375 623e 3c6d 693e 523c 2f6d  "><msub><mi>R</m
-00003590: 693e 3c6d 693e 413c 2f6d 693e 3c2f 6d73  i><mi>A</mi></ms
-000035a0: 7562 3e3c 2f6d 6174 683e 3c2f 6d6a 782d  ub></math></mjx-
-000035b0: 6173 7369 7374 6976 652d 6d6d 6c3e 3c2f  assistive-mml></
-000035c0: 6d6a 782d 636f 6e74 6169 6e65 723e 3c2f  mjx-container></
-000035d0: 7370 616e 3e20 696e 2047 4646 333c 2f70  span> in GFF3</p
-000035e0: 3e3c 2f6c 693e 0a3c 2f6f 6c3e 0a3c 2f64  ></li>.</ol>.</d
-000035f0: 643e 0a3c 2f64 6c3e 0a3c 2f6c 693e 0a3c  d>.</dl>.</li>.<
-00003600: 6c69 3e3c 646c 2063 6c61 7373 3d22 7369  li><dl class="si
-00003610: 6d70 6c65 223e 0a3c 6474 3e3c 7374 726f  mple">.<dt><stro
-00003620: 6e67 3e4f 7574 7075 743c 2f73 7472 6f6e  ng>Output</stron
-00003630: 673e 3a3c 2f64 743e 3c64 643e 3c6f 6c20  g>:</dt><dd><ol 
-00003640: 636c 6173 733d 2261 7261 6269 6320 7369  class="arabic si
-00003650: 6d70 6c65 223e 0a3c 6c69 3e3c 703e 4c69  mple">.<li><p>Li
-00003660: 6674 4f6e 2061 6e6e 6f74 6174 696f 6e20  ftOn annotation 
-00003670: 6669 6c65 2c20 3c73 7472 6f6e 673e 416e  file, <strong>An
-00003680: 6e6f 7461 7469 6f6e 3c2f 7374 726f 6e67  notation</strong
-00003690: 3e20 3c73 7061 6e20 636c 6173 733d 226d  > <span class="m
-000036a0: 6174 6820 6e6f 7472 616e 736c 6174 6520  ath notranslate 
-000036b0: 6e6f 6869 6768 6c69 6768 7422 3e3c 6d6a  nohighlight"><mj
-000036c0: 782d 636f 6e74 6169 6e65 7220 636c 6173  x-container clas
-000036d0: 733d 224d 6174 684a 6178 2043 7478 744d  s="MathJax CtxtM
-000036e0: 656e 755f 4174 7461 6368 6564 5f30 2220  enu_Attached_0" 
-000036f0: 6a61 783d 2243 4854 4d4c 2220 7461 6269  jax="CHTML" tabi
-00003700: 6e64 6578 3d22 3022 2063 7478 746d 656e  ndex="0" ctxtmen
-00003710: 755f 636f 756e 7465 723d 2231 3022 2073  u_counter="10" s
-00003720: 7479 6c65 3d22 666f 6e74 2d73 697a 653a  tyle="font-size:
-00003730: 2031 3139 253b 2070 6f73 6974 696f 6e3a   119%; position:
-00003740: 2072 656c 6174 6976 653b 223e 3c6d 6a78   relative;"><mjx
-00003750: 2d6d 6174 6820 636c 6173 733d 224d 4a58  -math class="MJX
-00003760: 2d54 4558 2220 6172 6961 2d68 6964 6465  -TEX" aria-hidde
-00003770: 6e3d 2274 7275 6522 3e3c 6d6a 782d 6d73  n="true"><mjx-ms
-00003780: 7562 3e3c 6d6a 782d 6d69 2063 6c61 7373  ub><mjx-mi class
-00003790: 3d22 6d6a 782d 6922 3e3c 6d6a 782d 6320  ="mjx-i"><mjx-c 
-000037a0: 636c 6173 733d 226d 6a78 2d63 3144 3434  class="mjx-c1D44
-000037b0: 3720 5445 582d 4922 3e3c 2f6d 6a78 2d63  7 TEX-I"></mjx-c
-000037c0: 3e3c 2f6d 6a78 2d6d 693e 3c6d 6a78 2d73  ></mjx-mi><mjx-s
-000037d0: 6372 6970 7420 7374 796c 653d 2276 6572  cript style="ver
-000037e0: 7469 6361 6c2d 616c 6967 6e3a 202d 302e  tical-align: -0.
-000037f0: 3135 3365 6d3b 206d 6172 6769 6e2d 6c65  153em; margin-le
-00003800: 6674 3a20 2d30 2e31 3265 6d3b 223e 3c6d  ft: -0.12em;"><m
-00003810: 6a78 2d6d 6920 636c 6173 733d 226d 6a78  jx-mi class="mjx
-00003820: 2d69 2220 7369 7a65 3d22 7322 3e3c 6d6a  -i" size="s"><mj
-00003830: 782d 6320 636c 6173 733d 226d 6a78 2d63  x-c class="mjx-c
-00003840: 3144 3433 3420 5445 582d 4922 3e3c 2f6d  1D434 TEX-I"></m
-00003850: 6a78 2d63 3e3c 2f6d 6a78 2d6d 693e 3c2f  jx-c></mjx-mi></
-00003860: 6d6a 782d 7363 7269 7074 3e3c 2f6d 6a78  mjx-script></mjx
-00003870: 2d6d 7375 623e 3c2f 6d6a 782d 6d61 7468  -msub></mjx-math
-00003880: 3e3c 6d6a 782d 6173 7369 7374 6976 652d  ><mjx-assistive-
-00003890: 6d6d 6c20 756e 7365 6c65 6374 6162 6c65  mml unselectable
-000038a0: 3d22 6f6e 2220 6469 7370 6c61 793d 2269  ="on" display="i
-000038b0: 6e6c 696e 6522 3e3c 6d61 7468 2078 6d6c  nline"><math xml
-000038c0: 6e73 3d22 6874 7470 3a2f 2f77 7777 2e77  ns="http://www.w
-000038d0: 332e 6f72 672f 3139 3938 2f4d 6174 682f  3.org/1998/Math/
-000038e0: 4d61 7468 4d4c 223e 3c6d 7375 623e 3c6d  MathML"><msub><m
-000038f0: 693e 543c 2f6d 693e 3c6d 693e 413c 2f6d  i>T</mi><mi>A</m
-00003900: 693e 3c2f 6d73 7562 3e3c 2f6d 6174 683e  i></msub></math>
-00003910: 3c2f 6d6a 782d 6173 7369 7374 6976 652d  </mjx-assistive-
-00003920: 6d6d 6c3e 3c2f 6d6a 782d 636f 6e74 6169  mml></mjx-contai
-00003930: 6e65 723e 3c2f 7370 616e 3e2c 2069 6e20  ner></span>, in 
-00003940: 4746 4633 3c2f 703e 3c2f 6c69 3e0a 3c6c  GFF3</p></li>.<l
-00003950: 693e 3c70 3e50 726f 7465 696e 2073 6571  i><p>Protein seq
-00003960: 7565 6e63 6520 6964 656e 7469 7469 6573  uence identities
-00003970: 2026 616d 703b 206d 7574 6174 696f 6e20   &amp; mutation 
-00003980: 7479 7065 733c 2f70 3e3c 2f6c 693e 0a3c  types</p></li>.<
-00003990: 6c69 3e3c 703e 4665 6174 7572 6573 2077  li><p>Features w
-000039a0: 6974 6820 6578 7472 6120 636f 7069 6573  ith extra copies
-000039b0: 3c2f 703e 3c2f 6c69 3e0a 3c6c 693e 3c70  </p></li>.<li><p
-000039c0: 3e55 6e6d 6170 7065 6420 6665 6174 7572  >Unmapped featur
-000039d0: 6573 3c2f 703e 3c2f 6c69 3e0a 3c2f 6f6c  es</p></li>.</ol
-000039e0: 3e0a 3c2f 6464 3e0a 3c2f 646c 3e0a 3c2f  >.</dd>.</dl>.</
-000039f0: 6c69 3e0a 3c2f 756c 3e0a 3c64 6976 2063  li>.</ul>.<div c
-00003a00: 6c61 7373 3d22 6c69 6e65 2d62 6c6f 636b  lass="line-block
-00003a10: 223e 0a3c 6469 7620 636c 6173 733d 226c  ">.<div class="l
-00003a20: 696e 6522 3e3c 6272 3e3c 2f64 6976 3e0a  ine"><br></div>.
-00003a30: 3c2f 6469 763e 0a3c 2f73 6563 7469 6f6e  </div>.</section
-00003a40: 3e0a 3c73 6563 7469 6f6e 2069 643d 226c  >.<section id="l
-00003a50: 6966 746f 6e2d 732d 6c69 6d69 7461 7469  ifton-s-limitati
-00003a60: 6f6e 2220 636c 6173 733d 2261 6374 6976  on" class="activ
-00003a70: 6522 3e0a 3c68 323e 4c69 6674 4f6e 2773  e">.<h2>LiftOn's
-00003a80: 206c 696d 6974 6174 696f 6e3c 6120 636c   limitation<a cl
-00003a90: 6173 733d 2268 6561 6465 726c 696e 6b22  ass="headerlink"
-00003aa0: 2068 7265 663d 2223 6c69 6674 6f6e 2d73   href="#lifton-s
-00003ab0: 2d6c 696d 6974 6174 696f 6e22 2074 6974  -limitation" tit
-00003ac0: 6c65 3d22 5065 726d 616c 696e 6b20 746f  le="Permalink to
-00003ad0: 2074 6869 7320 6865 6164 696e 6722 3e23   this heading">#
-00003ae0: 3c2f 613e 3c2f 6832 3e0a 3c70 3e4c 6966  </a></h2>.<p>Lif
-00003af0: 744f 6e27 7320 3c65 6d3e 6368 6169 6e69  tOn's <em>chaini
-00003b00: 6e67 2061 6c67 6f72 6974 686d 3c2f 656d  ng algorithm</em
-00003b10: 3e20 6375 7272 656e 746c 7920 6f6e 6c79  > currently only
-00003b20: 2075 7469 6c69 7a65 7320 6d69 6e69 7072   utilizes minipr
-00003b30: 6f74 2061 6c69 676e 6d65 6e74 2072 6573  ot alignment res
-00003b40: 756c 7473 2074 6f20 6669 7820 7468 6520  ults to fix the 
-00003b50: 4c69 6674 6f66 6620 616e 6e6f 7461 7469  Liftoff annotati
-00003b60: 6f6e 2e20 486f 7765 7665 722c 2069 7420  on. However, it 
-00003b70: 6361 6e20 6265 2065 7874 656e 6465 6420  can be extended 
-00003b80: 746f 2063 6861 696e 2074 6f67 6574 6865  to chain togethe
-00003b90: 7220 6d75 6c74 6970 6c65 2070 726f 7465  r multiple prote
-00003ba0: 696e 2d62 6173 6564 2061 6e6e 6f74 6174  in-based annotat
-00003bb0: 696f 6e20 6669 6c65 7320 6f72 2061 6173  ion files or aas
-00003bc0: 656d 626c 6564 2052 4e41 2d53 6571 2074  embled RNA-Seq t
-00003bd0: 7261 6e73 6372 6970 7473 2e3c 2f70 3e0a  ranscripts.</p>.
-00003be0: 3c70 3e44 4e41 2d20 616e 6420 7072 6f74  <p>DNA- and prot
-00003bf0: 6569 6e2d 6261 7365 6420 6d65 7468 6f64  ein-based method
-00003c00: 7320 7374 696c 6c20 6861 7665 2073 6f6d  s still have som
-00003c10: 6520 6c69 6d69 7461 7469 6f6e 732e 2057  e limitations. W
-00003c20: 6520 6172 6520 6465 7665 6c6f 7069 6e67  e are developing
-00003c30: 2061 206d 6f64 756c 6520 746f 206d 6572   a module to mer
-00003c40: 6765 2074 6865 204c 6966 744f 6e20 616e  ge the LiftOn an
-00003c50: 6e6f 7461 7469 6f6e 2077 6974 6820 7468  notation with th
-00003c60: 6520 7265 6c65 6173 6564 2063 7572 6174  e released curat
-00003c70: 6564 2061 6e6e 6f74 6174 696f 6e73 2074  ed annotations t
-00003c80: 6f20 6765 6e65 7261 7465 2062 6574 7465  o generate bette
-00003c90: 7220 616e 6e6f 7461 7469 6f6e 732e 3c2f  r annotations.</
-00003ca0: 703e 0a3c 703e 5468 6520 4c69 6674 4f6e  p>.<p>The LiftOn
-00003cb0: 203c 656d 3e63 6861 696e 696e 6720 616c   <em>chaining al
-00003cc0: 676f 7269 7468 6d3c 2f65 6d3e 206e 6f77  gorithm</em> now
-00003cd0: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
-00003ce0: 7420 6d75 6c74 692d 7468 7265 6164 696e  t multi-threadin
-00003cf0: 672e 2054 6869 7320 6675 6e63 7469 6f6e  g. This function
-00003d00: 616c 6974 7920 7374 616e 6473 2061 7320  ality stands as 
-00003d10: 6f75 7220 6e65 7874 2074 6172 6765 7465  our next targete
-00003d20: 6420 6665 6174 7572 6520 6f6e 2074 6865  d feature on the
-00003d30: 2064 6576 656c 6f70 6d65 6e74 2068 6f72   development hor
-00003d40: 697a 6f6e 213c 2f70 3e0a 3c64 6976 2063  izon!</p>.<div c
-00003d50: 6c61 7373 3d22 6c69 6e65 2d62 6c6f 636b  lass="line-block
-00003d60: 223e 0a3c 6469 7620 636c 6173 733d 226c  ">.<div class="l
-00003d70: 696e 6522 3e3c 6272 3e3c 2f64 6976 3e0a  ine"><br></div>.
-00003d80: 3c2f 6469 763e 0a3c 2f73 6563 7469 6f6e  </div>.</section
-00003d90: 3e0a 3c73 6563 7469 6f6e 2069 643d 2275  >.<section id="u
-00003da0: 7365 722d 7375 7070 6f72 7422 3e0a 3c68  ser-support">.<h
-00003db0: 323e 5573 6572 2073 7570 706f 7274 3c61  2>User support<a
-00003dc0: 2063 6c61 7373 3d22 6865 6164 6572 6c69   class="headerli
-00003dd0: 6e6b 2220 6872 6566 3d22 2375 7365 722d  nk" href="#user-
-00003de0: 7375 7070 6f72 7422 2074 6974 6c65 3d22  support" title="
-00003df0: 5065 726d 616c 696e 6b20 746f 2074 6869  Permalink to thi
-00003e00: 7320 6865 6164 696e 6722 3e23 3c2f 613e  s heading">#</a>
-00003e10: 3c2f 6832 3e0a 3c70 3e50 6c65 6173 6520  </h2>.<p>Please 
-00003e20: 676f 2074 6872 6f75 6768 2074 6865 203c  go through the <
-00003e30: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
-00003e40: 6365 2069 6e74 6572 6e61 6c22 2068 7265  ce internal" hre
-00003e50: 663d 2223 7461 626c 652d 6f66 2d63 6f6e  f="#table-of-con
-00003e60: 7465 6e74 7322 3e3c 7370 616e 2063 6c61  tents"><span cla
-00003e70: 7373 3d22 7374 6420 7374 642d 7265 6622  ss="std std-ref"
-00003e80: 3e64 6f63 756d 656e 7461 7469 6f6e 3c2f  >documentation</
-00003e90: 7370 616e 3e3c 2f61 3e20 6265 6c6f 7720  span></a> below 
-00003ea0: 6669 7273 742e 2049 6620 796f 7520 6861  first. If you ha
-00003eb0: 7665 2071 7565 7374 696f 6e73 2061 626f  ve questions abo
-00003ec0: 7574 2075 7369 6e67 2074 6865 2070 6163  ut using the pac
-00003ed0: 6b61 6765 2c20 6120 6275 6720 7265 706f  kage, a bug repo
-00003ee0: 7274 2c20 6f72 2061 2066 6561 7475 7265  rt, or a feature
-00003ef0: 2072 6571 7565 7374 2c20 706c 6561 7365   request, please
-00003f00: 2075 7365 2074 6865 2047 6974 4875 6220   use the GitHub 
-00003f10: 6973 7375 6520 7472 6163 6b65 7220 6865  issue tracker he
-00003f20: 7265 3a3c 2f70 3e0a 3c70 3e3c 6120 636c  re:</p>.<p><a cl
-00003f30: 6173 733d 2272 6566 6572 656e 6365 2065  ass="reference e
-00003f40: 7874 6572 6e61 6c22 2068 7265 663d 2268  xternal" href="h
-00003f50: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00003f60: 6d2f 4b75 616e 6861 6f2d 4368 616f 2f4c  m/Kuanhao-Chao/L
-00003f70: 6966 744f 6e2f 6973 7375 6573 223e 6874  iftOn/issues">ht
-00003f80: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003f90: 2f4b 7561 6e68 616f 2d43 6861 6f2f 4c69  /Kuanhao-Chao/Li
-00003fa0: 6674 4f6e 2f69 7373 7565 733c 2f61 3e3c  ftOn/issues</a><
-00003fb0: 2f70 3e0a 3c64 6976 2063 6c61 7373 3d22  /p>.<div class="
-00003fc0: 6c69 6e65 2d62 6c6f 636b 223e 0a3c 6469  line-block">.<di
-00003fd0: 7620 636c 6173 733d 226c 696e 6522 3e3c  v class="line"><
-00003fe0: 6272 3e3c 2f64 6976 3e0a 3c2f 6469 763e  br></div>.</div>
-00003ff0: 0a3c 2f73 6563 7469 6f6e 3e0a 3c73 6563  .</section>.<sec
-00004000: 7469 6f6e 2069 643d 226b 6579 2d63 6f6e  tion id="key-con
-00004010: 7472 6962 7574 6f72 7322 3e0a 3c68 323e  tributors">.<h2>
-00004020: 4b65 7920 636f 6e74 7269 6275 746f 7273  Key contributors
-00004030: 3c61 2063 6c61 7373 3d22 6865 6164 6572  <a class="header
-00004040: 6c69 6e6b 2220 6872 6566 3d22 236b 6579  link" href="#key
-00004050: 2d63 6f6e 7472 6962 7574 6f72 7322 2074  -contributors" t
-00004060: 6974 6c65 3d22 5065 726d 616c 696e 6b20  itle="Permalink 
-00004070: 746f 2074 6869 7320 6865 6164 696e 6722  to this heading"
-00004080: 3e23 3c2f 613e 3c2f 6832 3e0a 3c70 3e4c  >#</a></h2>.<p>L
-00004090: 6966 744f 6e20 7761 7320 6465 7369 676e  iftOn was design
-000040a0: 6564 2061 6e64 2064 6576 656c 6f70 6564  ed and developed
-000040b0: 2062 7920 3c61 2063 6c61 7373 3d22 7265   by <a class="re
-000040c0: 6665 7265 6e63 6520 6578 7465 726e 616c  ference external
-000040d0: 2220 6872 6566 3d22 6874 7470 733a 2f2f  " href="https://
-000040e0: 6b68 6368 616f 2e63 6f6d 2f22 3e4b 7561  khchao.com/">Kua
-000040f0: 6e2d 4861 6f20 4368 616f 3c2f 613e 2e20  n-Hao Chao</a>. 
-00004100: 2054 6869 7320 646f 6375 6d65 6e74 6174   This documentat
-00004110: 696f 6e20 7761 7320 7772 6974 7465 6e20  ion was written 
-00004120: 6279 203c 6120 636c 6173 733d 2272 6566  by <a class="ref
-00004130: 6572 656e 6365 2065 7874 6572 6e61 6c22  erence external"
-00004140: 2068 7265 663d 2268 7474 7073 3a2f 2f6b   href="https://k
-00004150: 6863 6861 6f2e 636f 6d2f 223e 4b75 616e  hchao.com/">Kuan
-00004160: 2d48 616f 2043 6861 6f3c 2f61 3e2e 3c2f  -Hao Chao</a>.</
-00004170: 703e 0a3c 6469 7620 636c 6173 733d 226c  p>.<div class="l
-00004180: 696e 652d 626c 6f63 6b22 3e0a 3c64 6976  ine-block">.<div
-00004190: 2063 6c61 7373 3d22 6c69 6e65 223e 3c62   class="line"><b
-000041a0: 723e 3c2f 6469 763e 0a3c 2f64 6976 3e0a  r></div>.</div>.
-000041b0: 3c2f 7365 6374 696f 6e3e 0a3c 7365 6374  </section>.<sect
-000041c0: 696f 6e20 6964 3d22 7461 626c 652d 6f66  ion id="table-of
-000041d0: 2d63 6f6e 7465 6e74 7322 3e0a 3c73 7061  -contents">.<spa
-000041e0: 6e20 6964 3d22 6964 3322 3e3c 2f73 7061  n id="id3"></spa
-000041f0: 6e3e 3c68 323e 5461 626c 6520 6f66 2063  n><h2>Table of c
-00004200: 6f6e 7465 6e74 733c 6120 636c 6173 733d  ontents<a class=
-00004210: 2268 6561 6465 726c 696e 6b22 2068 7265  "headerlink" hre
-00004220: 663d 2223 7461 626c 652d 6f66 2d63 6f6e  f="#table-of-con
-00004230: 7465 6e74 7322 2074 6974 6c65 3d22 5065  tents" title="Pe
-00004240: 726d 616c 696e 6b20 746f 2074 6869 7320  rmalink to this 
-00004250: 6865 6164 696e 6722 3e23 3c2f 613e 3c2f  heading">#</a></
-00004260: 6832 3e0a 3c64 6976 2063 6c61 7373 3d22  h2>.<div class="
-00004270: 746f 6374 7265 652d 7772 6170 7065 7220  toctree-wrapper 
-00004280: 636f 6d70 6f75 6e64 223e 0a3c 756c 3e0a  compound">.<ul>.
-00004290: 3c6c 6920 636c 6173 733d 2274 6f63 7472  <li class="toctr
-000042a0: 6565 2d6c 3122 3e3c 6120 636c 6173 733d  ee-l1"><a class=
-000042b0: 2272 6566 6572 656e 6365 2069 6e74 6572  "reference inter
-000042c0: 6e61 6c22 2068 7265 663d 2268 7474 703a  nal" href="http:
-000042d0: 2f2f 6363 622e 6a68 752e 6564 752f 6c69  //ccb.jhu.edu/li
-000042e0: 6674 6f6e 2f63 6f6e 7465 6e74 2f69 6e73  fton/content/ins
-000042f0: 7461 6c6c 6174 696f 6e2e 6874 6d6c 223e  tallation.html">
-00004300: 496e 7374 616c 6c61 7469 6f6e 3c2f 613e  Installation</a>
-00004310: 3c75 6c3e 0a3c 6c69 2063 6c61 7373 3d22  <ul>.<li class="
-00004320: 746f 6374 7265 652d 6c32 223e 3c61 2063  toctree-l2"><a c
-00004330: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
-00004340: 696e 7465 726e 616c 2220 6872 6566 3d22  internal" href="
-00004350: 6874 7470 3a2f 2f63 6362 2e6a 6875 2e65  http://ccb.jhu.e
-00004360: 6475 2f6c 6966 746f 6e2f 636f 6e74 656e  du/lifton/conten
-00004370: 742f 696e 7374 616c 6c61 7469 6f6e 2e68  t/installation.h
-00004380: 746d 6c23 7379 7374 656d 2d72 6571 7569  tml#system-requi
-00004390: 7265 6d65 6e74 7322 3e53 7973 7465 6d20  rements">System 
-000043a0: 7265 7175 6972 656d 656e 7473 3c2f 613e  requirements</a>
-000043b0: 3c2f 6c69 3e0a 3c6c 6920 636c 6173 733d  </li>.<li class=
-000043c0: 2274 6f63 7472 6565 2d6c 3222 3e3c 6120  "toctree-l2"><a 
-000043d0: 636c 6173 733d 2272 6566 6572 656e 6365  class="reference
-000043e0: 2069 6e74 6572 6e61 6c22 2068 7265 663d   internal" href=
-000043f0: 2268 7474 703a 2f2f 6363 622e 6a68 752e  "http://ccb.jhu.
-00004400: 6564 752f 6c69 6674 6f6e 2f63 6f6e 7465  edu/lifton/conte
-00004410: 6e74 2f69 6e73 7461 6c6c 6174 696f 6e2e  nt/installation.
-00004420: 6874 6d6c 2369 6e73 7461 6c6c 2d74 6872  html#install-thr
-00004430: 6f75 6768 2d70 6970 223e 496e 7374 616c  ough-pip">Instal
-00004440: 6c20 7468 726f 7567 6820 7069 703c 2f61  l through pip</a
-00004450: 3e3c 2f6c 693e 0a3c 6c69 2063 6c61 7373  ></li>.<li class
-00004460: 3d22 746f 6374 7265 652d 6c32 223e 3c61  ="toctree-l2"><a
-00004470: 2063 6c61 7373 3d22 7265 6665 7265 6e63   class="referenc
-00004480: 6520 696e 7465 726e 616c 2220 6872 6566  e internal" href
-00004490: 3d22 6874 7470 3a2f 2f63 6362 2e6a 6875  ="http://ccb.jhu
-000044a0: 2e65 6475 2f6c 6966 746f 6e2f 636f 6e74  .edu/lifton/cont
-000044b0: 656e 742f 696e 7374 616c 6c61 7469 6f6e  ent/installation
-000044c0: 2e68 746d 6c23 696e 7374 616c 6c2d 7468  .html#install-th
-000044d0: 726f 7567 682d 636f 6e64 6122 3e49 6e73  rough-conda">Ins
-000044e0: 7461 6c6c 2074 6872 6f75 6768 2063 6f6e  tall through con
-000044f0: 6461 3c2f 613e 3c2f 6c69 3e0a 3c6c 6920  da</a></li>.<li 
-00004500: 636c 6173 733d 2274 6f63 7472 6565 2d6c  class="toctree-l
-00004510: 3222 3e3c 6120 636c 6173 733d 2272 6566  2"><a class="ref
-00004520: 6572 656e 6365 2069 6e74 6572 6e61 6c22  erence internal"
-00004530: 2068 7265 663d 2268 7474 703a 2f2f 6363   href="http://cc
-00004540: 622e 6a68 752e 6564 752f 6c69 6674 6f6e  b.jhu.edu/lifton
-00004550: 2f63 6f6e 7465 6e74 2f69 6e73 7461 6c6c  /content/install
-00004560: 6174 696f 6e2e 6874 6d6c 2369 6e73 7461  ation.html#insta
-00004570: 6c6c 2d66 726f 6d2d 736f 7572 6365 223e  ll-from-source">
-00004580: 496e 7374 616c 6c20 6672 6f6d 2073 6f75  Install from sou
-00004590: 7263 653c 2f61 3e3c 2f6c 693e 0a3c 6c69  rce</a></li>.<li
-000045a0: 2063 6c61 7373 3d22 746f 6374 7265 652d   class="toctree-
-000045b0: 6c32 223e 3c61 2063 6c61 7373 3d22 7265  l2"><a class="re
-000045c0: 6665 7265 6e63 6520 696e 7465 726e 616c  ference internal
-000045d0: 2220 6872 6566 3d22 6874 7470 3a2f 2f63  " href="http://c
-000045e0: 6362 2e6a 6875 2e65 6475 2f6c 6966 746f  cb.jhu.edu/lifto
-000045f0: 6e2f 636f 6e74 656e 742f 696e 7374 616c  n/content/instal
-00004600: 6c61 7469 6f6e 2e68 746d 6c23 6368 6563  lation.html#chec
-00004610: 6b2d 6c69 6674 6f6e 2d69 6e73 7461 6c6c  k-lifton-install
-00004620: 6174 696f 6e22 3e43 6865 636b 204c 6966  ation">Check Lif
-00004630: 744f 6e20 696e 7374 616c 6c61 7469 6f6e  tOn installation
-00004640: 3c2f 613e 3c2f 6c69 3e0a 3c6c 6920 636c  </a></li>.<li cl
-00004650: 6173 733d 2274 6f63 7472 6565 2d6c 3222  ass="toctree-l2"
-00004660: 3e3c 6120 636c 6173 733d 2272 6566 6572  ><a class="refer
-00004670: 656e 6365 2069 6e74 6572 6e61 6c22 2068  ence internal" h
-00004680: 7265 663d 2268 7474 703a 2f2f 6363 622e  ref="http://ccb.
-00004690: 6a68 752e 6564 752f 6c69 6674 6f6e 2f63  jhu.edu/lifton/c
-000046a0: 6f6e 7465 6e74 2f69 6e73 7461 6c6c 6174  ontent/installat
-000046b0: 696f 6e2e 6874 6d6c 236e 6f77 2d79 6f75  ion.html#now-you
-000046c0: 2d61 7265 2d72 6561 6479 2d74 6f2d 676f  -are-ready-to-go
-000046d0: 223e 4e6f 772c 2079 6f75 2061 7265 2072  ">Now, you are r
-000046e0: 6561 6479 2074 6f20 676f 2021 3c2f 613e  eady to go !</a>
-000046f0: 3c2f 6c69 3e0a 3c2f 756c 3e0a 3c2f 6c69  </li>.</ul>.</li
-00004700: 3e0a 3c6c 6920 636c 6173 733d 2274 6f63  >.<li class="toc
-00004710: 7472 6565 2d6c 3122 3e3c 6120 636c 6173  tree-l1"><a clas
-00004720: 733d 2272 6566 6572 656e 6365 2069 6e74  s="reference int
-00004730: 6572 6e61 6c22 2068 7265 663d 2268 7474  ernal" href="htt
-00004740: 703a 2f2f 6363 622e 6a68 752e 6564 752f  p://ccb.jhu.edu/
-00004750: 6c69 6674 6f6e 2f63 6f6e 7465 6e74 2f71  lifton/content/q
-00004760: 7569 636b 7374 6172 742e 6874 6d6c 223e  uickstart.html">
-00004770: 5175 6963 6b20 5374 6172 7420 4775 6964  Quick Start Guid
-00004780: 653c 2f61 3e3c 756c 3e0a 3c6c 6920 636c  e</a><ul>.<li cl
-00004790: 6173 733d 2274 6f63 7472 6565 2d6c 3222  ass="toctree-l2"
-000047a0: 3e3c 6120 636c 6173 733d 2272 6566 6572  ><a class="refer
-000047b0: 656e 6365 2069 6e74 6572 6e61 6c22 2068  ence internal" h
-000047c0: 7265 663d 2268 7474 703a 2f2f 6363 622e  ref="http://ccb.
-000047d0: 6a68 752e 6564 752f 6c69 6674 6f6e 2f63  jhu.edu/lifton/c
-000047e0: 6f6e 7465 6e74 2f71 7569 636b 7374 6172  ontent/quickstar
-000047f0: 742e 6874 6d6c 2373 7570 6572 2d71 7569  t.html#super-qui
-00004800: 636b 2d73 7461 7274 2d6f 6e65 2d6c 696e  ck-start-one-lin
-00004810: 6572 223e 5375 7065 722d 5175 6963 6b20  er">Super-Quick 
-00004820: 5374 6172 7420 286f 6e65 2d6c 696e 6572  Start (one-liner
-00004830: 293c 2f61 3e3c 2f6c 693e 0a3c 6c69 2063  )</a></li>.<li c
-00004840: 6c61 7373 3d22 746f 6374 7265 652d 6c32  lass="toctree-l2
-00004850: 223e 3c61 2063 6c61 7373 3d22 7265 6665  "><a class="refe
-00004860: 7265 6e63 6520 696e 7465 726e 616c 2220  rence internal" 
-00004870: 6872 6566 3d22 6874 7470 3a2f 2f63 6362  href="http://ccb
-00004880: 2e6a 6875 2e65 6475 2f6c 6966 746f 6e2f  .jhu.edu/lifton/
-00004890: 636f 6e74 656e 742f 7175 6963 6b73 7461  content/quicksta
-000048a0: 7274 2e68 746d 6c23 7472 792d 6c69 6674  rt.html#try-lift
-000048b0: 6f6e 2d6f 6e2d 676f 6f67 6c65 2d63 6f6c  on-on-google-col
-000048c0: 6162 223e 5472 7920 4c69 6674 4f6e 206f  ab">Try LiftOn o
-000048d0: 6e20 476f 6f67 6c65 2043 6f6c 6162 3c2f  n Google Colab</
-000048e0: 613e 3c2f 6c69 3e0a 3c2f 756c 3e0a 3c2f  a></li>.</ul>.</
-000048f0: 6c69 3e0a 3c2f 756c 3e0a 3c2f 6469 763e  li>.</ul>.</div>
-00004900: 0a3c 6469 7620 636c 6173 733d 2274 6f63  .<div class="toc
-00004910: 7472 6565 2d77 7261 7070 6572 2063 6f6d  tree-wrapper com
-00004920: 706f 756e 6422 3e0a 3c70 2063 6c61 7373  pound">.<p class
-00004930: 3d22 6361 7074 696f 6e22 2072 6f6c 653d  ="caption" role=
-00004940: 2268 6561 6469 6e67 223e 3c73 7061 6e20  "heading"><span 
-00004950: 636c 6173 733d 2263 6170 7469 6f6e 2d74  class="caption-t
-00004960: 6578 7422 3e45 7861 6d70 6c65 733c 2f73  ext">Examples</s
-00004970: 7061 6e3e 3c2f 703e 0a3c 756c 3e0a 3c6c  pan></p>.<ul>.<l
-00004980: 6920 636c 6173 733d 2274 6f63 7472 6565  i class="toctree
-00004990: 2d6c 3122 3e3c 6120 636c 6173 733d 2272  -l1"><a class="r
-000049a0: 6566 6572 656e 6365 2069 6e74 6572 6e61  eference interna
-000049b0: 6c22 2068 7265 663d 2268 7474 703a 2f2f  l" href="http://
-000049c0: 6363 622e 6a68 752e 6564 752f 6c69 6674  ccb.jhu.edu/lift
-000049d0: 6f6e 2f63 6f6e 7465 6e74 2f73 616d 655f  on/content/same_
-000049e0: 7370 6563 6965 735f 6c69 6674 6f76 6572  species_liftover
-000049f0: 2f69 6e64 6578 2e68 746d 6c22 3e53 616d  /index.html">Sam
-00004a00: 6520 7370 6563 6965 7320 6c69 6674 2d6f  e species lift-o
-00004a10: 7665 723c 2f61 3e3c 2f6c 693e 0a3c 6c69  ver</a></li>.<li
-00004a20: 2063 6c61 7373 3d22 746f 6374 7265 652d   class="toctree-
-00004a30: 6c31 223e 3c61 2063 6c61 7373 3d22 7265  l1"><a class="re
-00004a40: 6665 7265 6e63 6520 696e 7465 726e 616c  ference internal
-00004a50: 2220 6872 6566 3d22 6874 7470 3a2f 2f63  " href="http://c
-00004a60: 6362 2e6a 6875 2e65 6475 2f6c 6966 746f  cb.jhu.edu/lifto
-00004a70: 6e2f 636f 6e74 656e 742f 636c 6f73 655f  n/content/close_
-00004a80: 7370 6563 6965 735f 6c69 6674 6f76 6572  species_liftover
-00004a90: 2f69 6e64 6578 2e68 746d 6c22 3e43 6c6f  /index.html">Clo
-00004aa0: 7365 6c79 2d72 656c 6174 6564 2073 7065  sely-related spe
-00004ab0: 6369 6573 206c 6966 742d 6f76 6572 3c2f  cies lift-over</
-00004ac0: 613e 3c2f 6c69 3e0a 3c6c 6920 636c 6173  a></li>.<li clas
-00004ad0: 733d 2274 6f63 7472 6565 2d6c 3122 3e3c  s="toctree-l1"><
-00004ae0: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
-00004af0: 6365 2069 6e74 6572 6e61 6c22 2068 7265  ce internal" hre
-00004b00: 663d 2268 7474 703a 2f2f 6363 622e 6a68  f="http://ccb.jh
-00004b10: 752e 6564 752f 6c69 6674 6f6e 2f63 6f6e  u.edu/lifton/con
-00004b20: 7465 6e74 2f64 6973 7461 6e74 5f73 7065  tent/distant_spe
-00004b30: 6369 6573 5f6c 6966 746f 7665 722f 696e  cies_liftover/in
-00004b40: 6465 782e 6874 6d6c 223e 4469 7374 616e  dex.html">Distan
-00004b50: 7420 7370 6563 6965 7320 6c69 6674 2d6f  t species lift-o
-00004b60: 7665 723c 2f61 3e3c 2f6c 693e 0a3c 2f75  ver</a></li>.</u
-00004b70: 6c3e 0a3c 2f64 6976 3e0a 3c64 6976 2063  l>.</div>.<div c
-00004b80: 6c61 7373 3d22 746f 6374 7265 652d 7772  lass="toctree-wr
-00004b90: 6170 7065 7220 636f 6d70 6f75 6e64 223e  apper compound">
-00004ba0: 0a3c 7020 636c 6173 733d 2263 6170 7469  .<p class="capti
-00004bb0: 6f6e 2220 726f 6c65 3d22 6865 6164 696e  on" role="headin
-00004bc0: 6722 3e3c 7370 616e 2063 6c61 7373 3d22  g"><span class="
-00004bd0: 6361 7074 696f 6e2d 7465 7874 223e 496e  caption-text">In
-00004be0: 666f 3c2f 7370 616e 3e3c 2f70 3e0a 3c75  fo</span></p>.<u
-00004bf0: 6c3e 0a3c 6c69 2063 6c61 7373 3d22 746f  l>.<li class="to
-00004c00: 6374 7265 652d 6c31 223e 3c61 2063 6c61  ctree-l1"><a cla
-00004c10: 7373 3d22 7265 6665 7265 6e63 6520 696e  ss="reference in
-00004c20: 7465 726e 616c 2220 6872 6566 3d22 6874  ternal" href="ht
-00004c30: 7470 3a2f 2f63 6362 2e6a 6875 2e65 6475  tp://ccb.jhu.edu
-00004c40: 2f6c 6966 746f 6e2f 636f 6e74 656e 742f  /lifton/content/
-00004c50: 6f75 7470 7574 5f65 7870 6c61 6e61 7469  output_explanati
-00004c60: 6f6e 2e68 746d 6c22 3e4f 7574 7075 7420  on.html">Output 
-00004c70: 6669 6c65 733c 2f61 3e3c 756c 3e0a 3c6c  files</a><ul>.<l
-00004c80: 6920 636c 6173 733d 2274 6f63 7472 6565  i class="toctree
-00004c90: 2d6c 3222 3e3c 6120 636c 6173 733d 2272  -l2"><a class="r
-00004ca0: 6566 6572 656e 6365 2069 6e74 6572 6e61  eference interna
-00004cb0: 6c22 2068 7265 663d 2268 7474 703a 2f2f  l" href="http://
-00004cc0: 6363 622e 6a68 752e 6564 752f 6c69 6674  ccb.jhu.edu/lift
-00004cd0: 6f6e 2f63 6f6e 7465 6e74 2f6f 7574 7075  on/content/outpu
-00004ce0: 745f 6578 706c 616e 6174 696f 6e2e 6874  t_explanation.ht
-00004cf0: 6d6c 236c 6966 746f 6e2d 6766 6633 223e  ml#lifton-gff3">
-00004d00: 6c69 6674 6f6e 2e47 4646 333c 2f61 3e3c  lifton.GFF3</a><
-00004d10: 2f6c 693e 0a3c 6c69 2063 6c61 7373 3d22  /li>.<li class="
-00004d20: 746f 6374 7265 652d 6c32 223e 3c61 2063  toctree-l2"><a c
-00004d30: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
-00004d40: 696e 7465 726e 616c 2220 6872 6566 3d22  internal" href="
-00004d50: 6874 7470 3a2f 2f63 6362 2e6a 6875 2e65  http://ccb.jhu.e
-00004d60: 6475 2f6c 6966 746f 6e2f 636f 6e74 656e  du/lifton/conten
-00004d70: 742f 6f75 7470 7574 5f65 7870 6c61 6e61  t/output_explana
-00004d80: 7469 6f6e 2e68 746d 6c23 6c69 6674 6f6e  tion.html#lifton
-00004d90: 2d6f 7574 7075 7422 3e6c 6966 746f 6e5f  -output">lifton_
-00004da0: 6f75 7470 7574 2f3c 2f61 3e3c 2f6c 693e  output/</a></li>
-00004db0: 0a3c 2f75 6c3e 0a3c 2f6c 693e 0a3c 6c69  .</ul>.</li>.<li
-00004dc0: 2063 6c61 7373 3d22 746f 6374 7265 652d   class="toctree-
-00004dd0: 6c31 223e 3c61 2063 6c61 7373 3d22 7265  l1"><a class="re
-00004de0: 6665 7265 6e63 6520 696e 7465 726e 616c  ference internal
-00004df0: 2220 6872 6566 3d22 6874 7470 3a2f 2f63  " href="http://c
-00004e00: 6362 2e6a 6875 2e65 6475 2f6c 6966 746f  cb.jhu.edu/lifto
-00004e10: 6e2f 636f 6e74 656e 742f 6265 6869 6e64  n/content/behind
-00004e20: 5f73 6365 6e65 732e 6874 6d6c 223e 4265  _scenes.html">Be
-00004e30: 6869 6e64 2074 6865 2073 6365 6e65 733c  hind the scenes<
-00004e40: 2f61 3e3c 756c 3e0a 3c6c 6920 636c 6173  /a><ul>.<li clas
-00004e50: 733d 2274 6f63 7472 6565 2d6c 3222 3e3c  s="toctree-l2"><
-00004e60: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
-00004e70: 6365 2069 6e74 6572 6e61 6c22 2068 7265  ce internal" hre
-00004e80: 663d 2268 7474 703a 2f2f 6363 622e 6a68  f="http://ccb.jh
-00004e90: 752e 6564 752f 6c69 6674 6f6e 2f63 6f6e  u.edu/lifton/con
-00004ea0: 7465 6e74 2f62 6568 696e 645f 7363 656e  tent/behind_scen
-00004eb0: 6573 2e68 746d 6c23 6d61 7463 6869 6e67  es.html#matching
-00004ec0: 2d6d 696e 6970 726f 742d 6c69 6674 6f66  -miniprot-liftof
-00004ed0: 662d 6765 6e6f 6d65 2d61 6e6e 6f74 6174  f-genome-annotat
-00004ee0: 696f 6e22 3e4d 6174 6368 696e 6720 6d69  ion">Matching mi
-00004ef0: 6e69 7072 6f74 2026 616d 703b 204c 6966  niprot &amp; Lif
-00004f00: 746f 6666 2067 656e 6f6d 6520 616e 6e6f  toff genome anno
-00004f10: 7461 7469 6f6e 3c2f 613e 3c2f 6c69 3e0a  tation</a></li>.
-00004f20: 3c6c 6920 636c 6173 733d 2274 6f63 7472  <li class="toctr
-00004f30: 6565 2d6c 3222 3e3c 6120 636c 6173 733d  ee-l2"><a class=
-00004f40: 2272 6566 6572 656e 6365 2069 6e74 6572  "reference inter
-00004f50: 6e61 6c22 2068 7265 663d 2268 7474 703a  nal" href="http:
-00004f60: 2f2f 6363 622e 6a68 752e 6564 752f 6c69  //ccb.jhu.edu/li
-00004f70: 6674 6f6e 2f63 6f6e 7465 6e74 2f62 6568  fton/content/beh
-00004f80: 696e 645f 7363 656e 6573 2e68 746d 6c23  ind_scenes.html#
-00004f90: 7072 6f74 6569 6e2d 6d61 7869 6d69 7a61  protein-maximiza
-00004fa0: 7469 6f6e 2d61 6c67 6f72 6974 686d 223e  tion-algorithm">
-00004fb0: 3c65 6d3e 5072 6f74 6569 6e2d 6d61 7869  <em>Protein-maxi
-00004fc0: 6d69 7a61 7469 6f6e 2061 6c67 6f72 6974  mization algorit
-00004fd0: 686d 3c2f 656d 3e3c 2f61 3e3c 2f6c 693e  hm</em></a></li>
-00004fe0: 0a3c 6c69 2063 6c61 7373 3d22 746f 6374  .<li class="toct
-00004ff0: 7265 652d 6c32 223e 3c61 2063 6c61 7373  ree-l2"><a class
-00005000: 3d22 7265 6665 7265 6e63 6520 696e 7465  ="reference inte
-00005010: 726e 616c 2220 6872 6566 3d22 6874 7470  rnal" href="http
-00005020: 3a2f 2f63 6362 2e6a 6875 2e65 6475 2f6c  ://ccb.jhu.edu/l
-00005030: 6966 746f 6e2f 636f 6e74 656e 742f 6265  ifton/content/be
-00005040: 6869 6e64 5f73 6365 6e65 732e 6874 6d6c  hind_scenes.html
-00005050: 236d 7574 6174 696f 6e2d 7265 706f 7274  #mutation-report
-00005060: 223e 4d75 7461 7469 6f6e 2072 6570 6f72  ">Mutation repor
-00005070: 743c 2f61 3e3c 2f6c 693e 0a3c 6c69 2063  t</a></li>.<li c
-00005080: 6c61 7373 3d22 746f 6374 7265 652d 6c32  lass="toctree-l2
-00005090: 223e 3c61 2063 6c61 7373 3d22 7265 6665  "><a class="refe
-000050a0: 7265 6e63 6520 696e 7465 726e 616c 2220  rence internal" 
-000050b0: 6872 6566 3d22 6874 7470 3a2f 2f63 6362  href="http://ccb
-000050c0: 2e6a 6875 2e65 6475 2f6c 6966 746f 6e2f  .jhu.edu/lifton/
-000050d0: 636f 6e74 656e 742f 6265 6869 6e64 5f73  content/behind_s
-000050e0: 6365 6e65 732e 6874 6d6c 236f 7065 6e2d  cenes.html#open-
-000050f0: 7265 6164 696e 672d 6672 616d 652d 7365  reading-frame-se
-00005100: 6172 6368 223e 4f70 656e 2d72 6561 6469  arch">Open-readi
-00005110: 6e67 2d66 7261 6d65 2073 6561 7263 683c  ng-frame search<
-00005120: 2f61 3e3c 2f6c 693e 0a3c 6c69 2063 6c61  /a></li>.<li cla
-00005130: 7373 3d22 746f 6374 7265 652d 6c32 223e  ss="toctree-l2">
-00005140: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
-00005150: 6e63 6520 696e 7465 726e 616c 2220 6872  nce internal" hr
-00005160: 6566 3d22 6874 7470 3a2f 2f63 6362 2e6a  ef="http://ccb.j
-00005170: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
-00005180: 6e74 656e 742f 6265 6869 6e64 5f73 6365  ntent/behind_sce
-00005190: 6e65 732e 6874 6d6c 2364 6e61 2d70 726f  nes.html#dna-pro
-000051a0: 7465 696e 2d74 7261 6e73 6372 6970 742d  tein-transcript-
-000051b0: 7365 7175 656e 6365 2d69 6465 6e74 6974  sequence-identit
-000051c0: 792d 7363 6f72 652d 6361 6c63 756c 6174  y-score-calculat
-000051d0: 696f 6e22 3e44 4e41 2026 616d 703b 2070  ion">DNA &amp; p
-000051e0: 726f 7465 696e 2074 7261 6e73 6372 6970  rotein transcrip
-000051f0: 7420 7365 7175 656e 6365 2069 6465 6e74  t sequence ident
-00005200: 6974 7920 7363 6f72 6520 6361 6c63 756c  ity score calcul
-00005210: 6174 696f 6e3c 2f61 3e3c 2f6c 693e 0a3c  ation</a></li>.<
-00005220: 6c69 2063 6c61 7373 3d22 746f 6374 7265  li class="toctre
-00005230: 652d 6c32 223e 3c61 2063 6c61 7373 3d22  e-l2"><a class="
-00005240: 7265 6665 7265 6e63 6520 696e 7465 726e  reference intern
-00005250: 616c 2220 6872 6566 3d22 6874 7470 3a2f  al" href="http:/
-00005260: 2f63 6362 2e6a 6875 2e65 6475 2f6c 6966  /ccb.jhu.edu/lif
-00005270: 746f 6e2f 636f 6e74 656e 742f 6265 6869  ton/content/behi
-00005280: 6e64 5f73 6365 6e65 732e 6874 6d6c 2372  nd_scenes.html#r
-00005290: 6566 6572 656e 6365 223e 5265 6665 7265  eference">Refere
-000052a0: 6e63 653c 2f61 3e3c 2f6c 693e 0a3c 2f75  nce</a></li>.</u
-000052b0: 6c3e 0a3c 2f6c 693e 0a3c 6c69 2063 6c61  l>.</li>.<li cla
-000052c0: 7373 3d22 746f 6374 7265 652d 6c31 223e  ss="toctree-l1">
-000052d0: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
-000052e0: 6e63 6520 696e 7465 726e 616c 2220 6872  nce internal" hr
-000052f0: 6566 3d22 6874 7470 3a2f 2f63 6362 2e6a  ef="http://ccb.j
-00005300: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
-00005310: 6e74 656e 742f 686f 775f 746f 5f70 6167  ntent/how_to_pag
-00005320: 652e 6874 6d6c 223e 5120 2661 6d70 3b20  e.html">Q &amp; 
-00005330: 4120 2e2e 2e3c 2f61 3e3c 2f6c 693e 0a3c  A ...</a></li>.<
-00005340: 6c69 2063 6c61 7373 3d22 746f 6374 7265  li class="toctre
-00005350: 652d 6c31 223e 3c61 2063 6c61 7373 3d22  e-l1"><a class="
-00005360: 7265 6665 7265 6e63 6520 696e 7465 726e  reference intern
-00005370: 616c 2220 6872 6566 3d22 6874 7470 3a2f  al" href="http:/
-00005380: 2f63 6362 2e6a 6875 2e65 6475 2f6c 6966  /ccb.jhu.edu/lif
-00005390: 746f 6e2f 636f 6e74 656e 742f 6675 6e63  ton/content/func
-000053a0: 7469 6f6e 5f6d 616e 7561 6c2e 6874 6d6c  tion_manual.html
-000053b0: 223e 5573 6572 204d 616e 7561 6c3c 2f61  ">User Manual</a
-000053c0: 3e3c 756c 3e0a 3c6c 6920 636c 6173 733d  ><ul>.<li class=
-000053d0: 2274 6f63 7472 6565 2d6c 3222 3e3c 6120  "toctree-l2"><a 
-000053e0: 636c 6173 733d 2272 6566 6572 656e 6365  class="reference
-000053f0: 2069 6e74 6572 6e61 6c22 2068 7265 663d   internal" href=
-00005400: 2268 7474 703a 2f2f 6363 622e 6a68 752e  "http://ccb.jhu.
-00005410: 6564 752f 6c69 6674 6f6e 2f63 6f6e 7465  edu/lifton/conte
-00005420: 6e74 2f66 756e 6374 696f 6e5f 6d61 6e75  nt/function_manu
-00005430: 616c 2e68 746d 6c23 7370 6c61 6d22 3e73  al.html#splam">s
-00005440: 706c 616d 3c2f 613e 3c2f 6c69 3e0a 3c2f  plam</a></li>.</
-00005450: 756c 3e0a 3c2f 6c69 3e0a 3c6c 6920 636c  ul>.</li>.<li cl
-00005460: 6173 733d 2274 6f63 7472 6565 2d6c 3122  ass="toctree-l1"
-00005470: 3e3c 6120 636c 6173 733d 2272 6566 6572  ><a class="refer
-00005480: 656e 6365 2069 6e74 6572 6e61 6c22 2068  ence internal" h
-00005490: 7265 663d 2268 7474 703a 2f2f 6363 622e  ref="http://ccb.
-000054a0: 6a68 752e 6564 752f 6c69 6674 6f6e 2f63  jhu.edu/lifton/c
-000054b0: 6f6e 7465 6e74 2f63 6861 6e67 656c 6f67  ontent/changelog
-000054c0: 2e68 746d 6c22 3e43 6861 6e67 656c 6f67  .html">Changelog
-000054d0: 3c2f 613e 3c75 6c3e 0a3c 6c69 2063 6c61  </a><ul>.<li cla
-000054e0: 7373 3d22 746f 6374 7265 652d 6c32 223e  ss="toctree-l2">
-000054f0: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
-00005500: 6e63 6520 696e 7465 726e 616c 2220 6872  nce internal" hr
-00005510: 6566 3d22 6874 7470 3a2f 2f63 6362 2e6a  ef="http://ccb.j
-00005520: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
-00005530: 6e74 656e 742f 6368 616e 6765 6c6f 672e  ntent/changelog.
-00005540: 6874 6d6c 2376 312d 302d 3022 3e76 312e  html#v1-0-0">v1.
-00005550: 302e 303c 2f61 3e3c 2f6c 693e 0a3c 2f75  0.0</a></li>.</u
-00005560: 6c3e 0a3c 2f6c 693e 0a3c 6c69 2063 6c61  l>.</li>.<li cla
-00005570: 7373 3d22 746f 6374 7265 652d 6c31 223e  ss="toctree-l1">
-00005580: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
-00005590: 6e63 6520 696e 7465 726e 616c 2220 6872  nce internal" hr
-000055a0: 6566 3d22 6874 7470 3a2f 2f63 6362 2e6a  ef="http://ccb.j
-000055b0: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
-000055c0: 6e74 656e 742f 6c69 6365 6e73 652e 6874  ntent/license.ht
-000055d0: 6d6c 223e 4c69 6365 6e73 653c 2f61 3e3c  ml">License</a><
-000055e0: 2f6c 693e 0a3c 6c69 2063 6c61 7373 3d22  /li>.<li class="
-000055f0: 746f 6374 7265 652d 6c31 223e 3c61 2063  toctree-l1"><a c
-00005600: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
-00005610: 696e 7465 726e 616c 2220 6872 6566 3d22  internal" href="
-00005620: 6874 7470 3a2f 2f63 6362 2e6a 6875 2e65  http://ccb.jhu.e
-00005630: 6475 2f6c 6966 746f 6e2f 636f 6e74 656e  du/lifton/conten
-00005640: 742f 636f 6e74 6163 742e 6874 6d6c 223e  t/contact.html">
-00005650: 436f 6e74 6163 743c 2f61 3e3c 2f6c 693e  Contact</a></li>
-00005660: 0a3c 2f75 6c3e 0a3c 2f64 6976 3e0a 3c2f  .</ul>.</div>.</
-00005670: 7365 6374 696f 6e3e 0a3c 2f73 6563 7469  section>.</secti
-00005680: 6f6e 3e0a 0a3c 6272 3e0a 0a23 2320 3c61  on>..<br>..## <a
-00005690: 206e 616d 653d 2263 6974 6174 696f 6e22   name="citation"
-000056a0: 3e3c 2f61 3e43 6974 6174 696f 6e3c 6120  ></a>Citation<a 
-000056b0: 636c 6173 733d 2268 6561 6465 726c 696e  class="headerlin
-000056c0: 6b22 2068 7265 663d 2223 6369 7461 7469  k" href="#citati
-000056d0: 6f6e 2220 7469 746c 653d 2250 6572 6d61  on" title="Perma
-000056e0: 6c69 6e6b 2074 6f20 7468 6973 2068 6561  link to this hea
-000056f0: 6469 6e67 223e 233c 2f61 3e0a 0a0a 4b75  ding">#</a>...Ku
-00005700: 616e 2d48 616f 2043 6861 6f2a 2c20 4d69  an-Hao Chao*, Mi
-00005710: 6861 656c 6120 5065 7274 6561 2c20 5374  haela Pertea, St
-00005720: 6576 656e 204c 2053 616c 7a62 6572 672a  even L Salzberg*
-00005730: 2c20 224c 6966 744f 6e3a 2061 2074 6f6f  , "LiftOn: a too
-00005740: 6c20 746f 2069 6d70 726f 7665 2061 6e6e  l to improve ann
-00005750: 6f74 6174 696f 6e73 2066 6f72 2070 726f  otations for pro
-00005760: 7465 696e 2d63 6f64 696e 6720 6765 6e65  tein-coding gene
-00005770: 7320 6475 7269 6e67 2074 6865 206c 6966  s during the lif
-00005780: 742d 6f76 6572 2070 726f 6365 7373 2e22  t-over process."
-00005790: 2c20 3c69 3e62 696f 5278 6976 3c2f 693e  , <i>bioRxiv</i>
-000057a0: 203c 623e 3230 3233 2e30 372e 3237 2e35   <b>2023.07.27.5
-000057b0: 3530 3735 343c 2f62 3e2c 2064 6f69 3a20  50754</b>, doi: 
-000057c0: 5b68 7474 7073 3a2f 2f64 6f69 2e6f 7267  [https://doi.org
-000057d0: 2f31 302e 3131 3031 2f32 3032 332e 3037  /10.1101/2023.07
-000057e0: 2e32 372e 3535 3037 3534 5d28 6874 7470  .27.550754](http
-000057f0: 733a 2f2f 646f 692e 6f72 672f 3130 2e31  s://doi.org/10.1
-00005800: 3130 312f 3230 3233 2e30 372e 3237 2e35  101/2023.07.27.5
-00005810: 3530 3735 3429 2c20 3230 3233 0a0a 3c62  50754), 2023..<b
-00005820: 723e 0a3c 6272 3e0a 3c62 723e 0a0a 3c69  r>.<br>.<br>..<i
-00005830: 6d67 2061 6c74 3d22 4d79 204c 6f67 6f22  mg alt="My Logo"
-00005840: 2063 6c61 7373 3d22 6c6f 676f 2068 6561   class="logo hea
-00005850: 6465 722d 696d 6167 6520 6f6e 6c79 2d6c  der-image only-l
-00005860: 6967 6874 2061 6c69 676e 2d63 656e 7465  ight align-cente
-00005870: 7222 2073 7263 3d22 6772 6170 6869 6373  r" src="graphics
-00005880: 2f6a 6875 2d6c 6f67 6f2d 6461 726b 2e70  /jhu-logo-dark.p
-00005890: 6e67 223e 0a                             ng">.
+00000020: 6f6e 0a56 6572 7369 6f6e 3a20 312e 302e  on.Version: 1.0.
+00000030: 300a 5375 6d6d 6172 793a 2043 6f6d 6269  0.Summary: Combi
+00000040: 6e69 6e67 2044 4e41 2061 6e64 2070 726f  ning DNA and pro
+00000050: 7465 696e 2061 6c69 676e 6d65 6e74 7320  tein alignments 
+00000060: 746f 2069 6d70 726f 7665 2067 656e 6f6d  to improve genom
+00000070: 6520 616e 6e6f 7461 7469 6f6e 2077 6974  e annotation wit
+00000080: 6820 4c69 6674 4f6e 0a48 6f6d 652d 7061  h LiftOn.Home-pa
+00000090: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
+000000a0: 7562 2e63 6f6d 2f4b 7561 6e68 616f 2d43  ub.com/Kuanhao-C
+000000b0: 6861 6f2f 4c69 6674 6f6e 0a41 7574 686f  hao/Lifton.Autho
+000000c0: 723a 204b 7561 6e2d 4861 6f20 4368 616f  r: Kuan-Hao Chao
+000000d0: 0a41 7574 686f 722d 656d 6169 6c3a 206b  .Author-email: k
+000000e0: 682e 6368 616f 4063 732e 6a68 752e 6564  h.chao@cs.jhu.ed
+000000f0: 750a 5265 7175 6972 6573 2d50 7974 686f  u.Requires-Pytho
+00000100: 6e3a 203e 3d33 2e36 0a44 6573 6372 6970  n: >=3.6.Descrip
+00000110: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
+00000120: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
+00000130: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
+00000140: 4943 454e 5345 0a0a 3c69 6d67 2061 6c74  ICENSE..<img alt
+00000150: 3d22 4d79 204c 6f67 6f22 2063 6c61 7373  ="My Logo" class
+00000160: 3d22 6c6f 676f 2068 6561 6465 722d 696d  ="logo header-im
+00000170: 6167 6520 6f6e 6c79 2d6c 6967 6874 2061  age only-light a
+00000180: 6c69 676e 2d63 656e 7465 7222 2073 7263  lign-center" src
+00000190: 3d22 6874 7470 733a 2f2f 7374 6f72 6167  ="https://storag
+000001a0: 652e 676f 6f67 6c65 6170 6973 2e63 6f6d  e.googleapis.com
+000001b0: 2f73 746f 7261 6765 2e6b 6863 6861 6f2e  /storage.khchao.
+000001c0: 636f 6d2f 6669 6775 7265 732f 4c69 6674  com/figures/Lift
+000001d0: 4f6e 2f4c 6966 744f 6e5f 636f 6c6f 722e  On/LiftOn_color.
+000001e0: 706e 6722 2073 7479 6c65 3d22 7769 6474  png" style="widt
+000001f0: 683a 3930 2522 3e0a 0a3c 6469 7620 636c  h:90%">..<div cl
+00000200: 6173 733d 2263 6f6e 7465 6e74 223e 0a3c  ass="content">.<
+00000210: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
+00000220: 6365 2065 7874 6572 6e61 6c20 696d 6167  ce external imag
+00000230: 652d 7265 6665 7265 6e63 6522 2068 7265  e-reference" hre
+00000240: 663d 2268 7474 7073 3a2f 2f69 6d67 2e73  f="https://img.s
+00000250: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000260: 4c69 6365 6e73 652d 4750 4c76 332d 7965  License-GPLv3-ye
+00000270: 6c6c 6f77 2e73 7667 223e 3c69 6d67 2061  llow.svg"><img a
+00000280: 6c74 3d22 6874 7470 733a 2f2f 696d 672e  lt="https://img.
+00000290: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+000002a0: 2f4c 6963 656e 7365 2d47 504c 7633 2d79  /License-GPLv3-y
+000002b0: 656c 6c6f 772e 7376 6722 2073 7263 3d22  ellow.svg" src="
+000002c0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000002d0: 6c64 732e 696f 2f62 6164 6765 2f4c 6963  lds.io/badge/Lic
+000002e0: 656e 7365 2d47 504c 7633 2d79 656c 6c6f  ense-GPLv3-yello
+000002f0: 772e 7376 6722 3e3c 2f61 3e0a 3c61 2063  w.svg"></a>.<a c
+00000300: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
+00000310: 6578 7465 726e 616c 2069 6d61 6765 2d72  external image-r
+00000320: 6566 6572 656e 6365 2220 6872 6566 3d22  eference" href="
+00000330: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000340: 6c64 732e 696f 2f62 6164 6765 2f76 6572  lds.io/badge/ver
+00000350: 7369 6f6e 2d76 2e30 2e30 2e31 2d62 6c75  sion-v.0.0.1-blu
+00000360: 6522 3e3c 696d 6720 616c 743d 2268 7474  e"><img alt="htt
+00000370: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000380: 2e69 6f2f 6261 6467 652f 7665 7273 696f  .io/badge/versio
+00000390: 6e2d 762e 302e 302e 312d 626c 7565 2220  n-v.0.0.1-blue" 
+000003a0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+000003b0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+000003c0: 652f 7665 7273 696f 6e2d 762e 302e 302e  e/version-v.0.0.
+000003d0: 312d 626c 7565 223e 3c2f 613e 0a3c 6120  1-blue"></a>.<a 
+000003e0: 636c 6173 733d 2272 6566 6572 656e 6365  class="reference
+000003f0: 2065 7874 6572 6e61 6c20 696d 6167 652d   external image-
+00000400: 7265 6665 7265 6e63 6522 2068 7265 663d  reference" href=
+00000410: 2268 7474 7073 3a2f 2f70 6570 792e 7465  "https://pepy.te
+00000420: 6368 2f70 726f 6a65 6374 2f6c 6966 746f  ch/project/lifto
+00000430: 6e22 3e3c 696d 6720 616c 743d 2268 7474  n"><img alt="htt
+00000440: 7073 3a2f 2f73 7461 7469 632e 7065 7079  ps://static.pepy
+00000450: 2e74 6563 682f 7065 7273 6f6e 616c 697a  .tech/personaliz
+00000460: 6564 2d62 6164 6765 2f6c 6966 746f 6e3f  ed-badge/lifton?
+00000470: 7065 7269 6f64 3d74 6f74 616c 2661 6d70  period=total&amp
+00000480: 3b75 6e69 7473 3d61 6262 7265 7669 6174  ;units=abbreviat
+00000490: 696f 6e26 616d 703b 6c65 6674 5f63 6f6c  ion&amp;left_col
+000004a0: 6f72 3d67 7265 7926 616d 703b 7269 6768  or=grey&amp;righ
+000004b0: 745f 636f 6c6f 723d 626c 7565 2661 6d70  t_color=blue&amp
+000004c0: 3b6c 6566 745f 7465 7874 3d50 7950 6925  ;left_text=PyPi%
+000004d0: 3230 646f 776e 6c6f 6164 7322 2073 7263  20downloads" src
+000004e0: 3d22 6874 7470 733a 2f2f 7374 6174 6963  ="https://static
+000004f0: 2e70 6570 792e 7465 6368 2f70 6572 736f  .pepy.tech/perso
+00000500: 6e61 6c69 7a65 642d 6261 6467 652f 6c69  nalized-badge/li
+00000510: 6674 6f6e 3f70 6572 696f 643d 746f 7461  fton?period=tota
+00000520: 6c26 616d 703b 756e 6974 733d 6162 6272  l&amp;units=abbr
+00000530: 6576 6961 7469 6f6e 2661 6d70 3b6c 6566  eviation&amp;lef
+00000540: 745f 636f 6c6f 723d 6772 6579 2661 6d70  t_color=grey&amp
+00000550: 3b72 6967 6874 5f63 6f6c 6f72 3d62 6c75  ;right_color=blu
+00000560: 6526 616d 703b 6c65 6674 5f74 6578 743d  e&amp;left_text=
+00000570: 5079 5069 2532 3064 6f77 6e6c 6f61 6473  PyPi%20downloads
+00000580: 223e 3c2f 613e 0a3c 6120 636c 6173 733d  "></a>.<a class=
+00000590: 2272 6566 6572 656e 6365 2065 7874 6572  "reference exter
+000005a0: 6e61 6c20 696d 6167 652d 7265 6665 7265  nal image-refere
+000005b0: 6e63 6522 2068 7265 663d 2268 7474 7073  nce" href="https
+000005c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4b75  ://github.com/Ku
+000005d0: 616e 6861 6f2d 4368 616f 2f6c 6966 746f  anhao-Chao/lifto
+000005e0: 6e2f 7265 6c65 6173 6573 223e 3c69 6d67  n/releases"><img
+000005f0: 2061 6c74 3d22 6874 7470 733a 2f2f 696d   alt="https://im
+00000600: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+00000610: 6875 622f 646f 776e 6c6f 6164 732f 4b75  hub/downloads/Ku
+00000620: 616e 6861 6f2d 4368 616f 2f6c 6966 746f  anhao-Chao/lifto
+00000630: 6e2f 746f 7461 6c2e 7376 673f 7374 796c  n/total.svg?styl
+00000640: 653d 736f 6369 616c 2661 6d70 3b6c 6f67  e=social&amp;log
+00000650: 6f3d 6769 7468 7562 2661 6d70 3b6c 6162  o=github&amp;lab
+00000660: 656c 3d44 6f77 6e6c 6f61 6422 2073 7263  el=Download" src
+00000670: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000680: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00000690: 646f 776e 6c6f 6164 732f 4b75 616e 6861  downloads/Kuanha
+000006a0: 6f2d 4368 616f 2f6c 6966 746f 6e2f 746f  o-Chao/lifton/to
+000006b0: 7461 6c2e 7376 673f 7374 796c 653d 736f  tal.svg?style=so
+000006c0: 6369 616c 2661 6d70 3b6c 6f67 6f3d 6769  cial&amp;logo=gi
+000006d0: 7468 7562 2661 6d70 3b6c 6162 656c 3d44  thub&amp;label=D
+000006e0: 6f77 6e6c 6f61 6422 3e3c 2f61 3e0a 3c61  ownload"></a>.<a
+000006f0: 2063 6c61 7373 3d22 7265 6665 7265 6e63   class="referenc
+00000700: 6520 6578 7465 726e 616c 2069 6d61 6765  e external image
+00000710: 2d72 6566 6572 656e 6365 2220 6872 6566  -reference" href
+00000720: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000730: 2e63 6f6d 2f4b 7561 6e68 616f 2d43 6861  .com/Kuanhao-Cha
+00000740: 6f2f 6c69 6674 6f6e 2f72 656c 6561 7365  o/lifton/release
+00000750: 7322 3e3c 696d 6720 616c 743d 2268 7474  s"><img alt="htt
+00000760: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000770: 2e69 6f2f 6261 6467 652f 706c 6174 666f  .io/badge/platfo
+00000780: 726d 2d6d 6163 4f53 5f2f 4c69 6e75 782d  rm-macOS_/Linux-
+00000790: 6772 6565 6e2e 7376 6722 2073 7263 3d22  green.svg" src="
+000007a0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000007b0: 6c64 732e 696f 2f62 6164 6765 2f70 6c61  lds.io/badge/pla
+000007c0: 7466 6f72 6d2d 6d61 634f 535f 2f4c 696e  tform-macOS_/Lin
+000007d0: 7578 2d67 7265 656e 2e73 7667 223e 3c2f  ux-green.svg"></
+000007e0: 613e 0a3c 6120 636c 6173 733d 2272 6566  a>.<a class="ref
+000007f0: 6572 656e 6365 2065 7874 6572 6e61 6c20  erence external 
+00000800: 696d 6167 652d 7265 6665 7265 6e63 6522  image-reference"
+00000810: 2068 7265 663d 2268 7474 7073 3a2f 2f63   href="https://c
+00000820: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+00000830: 6f67 6c65 2e63 6f6d 2f67 6974 6875 622f  ogle.com/github/
+00000840: 4b75 616e 6861 6f2d 4368 616f 2f6c 6966  Kuanhao-Chao/lif
+00000850: 746f 6e2f 626c 6f62 2f6d 6169 6e2f 6e6f  ton/blob/main/no
+00000860: 7465 626f 6f6b 2f6c 6966 746f 6e5f 6578  tebook/lifton_ex
+00000870: 616d 706c 652e 6970 796e 6222 3e3c 696d  ample.ipynb"><im
+00000880: 6720 616c 743d 2268 7474 7073 3a2f 2f63  g alt="https://c
+00000890: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+000008a0: 6f67 6c65 2e63 6f6d 2f61 7373 6574 732f  ogle.com/assets/
+000008b0: 636f 6c61 622d 6261 6467 652e 7376 6722  colab-badge.svg"
+000008c0: 2073 7263 3d22 6874 7470 733a 2f2f 636f   src="https://co
+000008d0: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
+000008e0: 676c 652e 636f 6d2f 6173 7365 7473 2f63  gle.com/assets/c
+000008f0: 6f6c 6162 2d62 6164 6765 2e73 7667 223e  olab-badge.svg">
+00000900: 3c2f 613e 0a3c 6469 7620 636c 6173 733d  </a>.<div class=
+00000910: 226c 696e 652d 626c 6f63 6b22 3e0a 3c64  "line-block">.<d
+00000920: 6976 2063 6c61 7373 3d22 6c69 6e65 223e  iv class="line">
+00000930: 3c62 723e 3c2f 6469 763e 0a3c 2f64 6976  <br></div>.</div
+00000940: 3e0a 3c6c 696e 6b20 7265 6c3d 2273 7479  >.<link rel="sty
+00000950: 6c65 7368 6565 7422 2068 7265 663d 2268  lesheet" href="h
+00000960: 7474 7073 3a2f 2f63 646e 6a73 2e63 6c6f  ttps://cdnjs.clo
+00000970: 7564 666c 6172 652e 636f 6d2f 616a 6178  udflare.com/ajax
+00000980: 2f6c 6962 732f 666f 6e74 2d61 7765 736f  /libs/font-aweso
+00000990: 6d65 2f34 2e37 2e30 2f63 7373 2f66 6f6e  me/4.7.0/css/fon
+000009a0: 742d 6177 6573 6f6d 652e 6d69 6e2e 6373  t-awesome.min.cs
+000009b0: 7322 3e0a 0a4c 6966 744f 6e20 6973 2061  s">..LiftOn is a
+000009c0: 2068 6f6d 6f6c 6f67 792d 6261 7365 6420   homology-based 
+000009d0: 6c69 6674 2d6f 7665 7220 746f 6f6c 2075  lift-over tool u
+000009e0: 7369 6e67 2062 6f74 6820 444e 412d 444e  sing both DNA-DN
+000009f0: 4120 616c 6967 6e6d 656e 7473 2028 6672  A alignments (fr
+00000a00: 6f6d 203c 6120 6872 6566 3d22 6874 7470  om <a href="http
+00000a10: 733a 2f2f 6163 6164 656d 6963 2e6f 7570  s://academic.oup
+00000a20: 2e63 6f6d 2f62 696f 696e 666f 726d 6174  .com/bioinformat
+00000a30: 6963 732f 6172 7469 636c 652f 3337 2f31  ics/article/37/1
+00000a40: 322f 3136 3339 2f36 3033 3531 3238 3f6c  2/1639/6035128?l
+00000a50: 6f67 696e 3d74 7275 6522 2074 6172 6765  ogin=true" targe
+00000a60: 743d 225f 626c 616e 6b22 3e4c 6966 746f  t="_blank">Lifto
+00000a70: 6666 3c2f 613e 2c20 6372 6564 6974 7320  ff</a>, credits 
+00000a80: 746f 203c 6120 6872 6566 3d22 6874 7470  to <a href="http
+00000a90: 733a 2f2f 7363 686f 6c61 722e 676f 6f67  s://scholar.goog
+00000aa0: 6c65 2e63 6f6d 2f63 6974 6174 696f 6e73  le.com/citations
+00000ab0: 3f75 7365 723d 4e33 7458 6b37 5141 4141  ?user=N3tXk7QAAA
+00000ac0: 414a 2661 6d70 3b68 6c3d 656e 2220 7461  AJ&amp;hl=en" ta
+00000ad0: 7267 6574 3d22 5f62 6c61 6e6b 223e 4472  rget="_blank">Dr
+00000ae0: 2e20 416c 6169 6e61 2053 6875 6d61 7465  . Alaina Shumate
+00000af0: 3c2f 613e 2920 616e 6420 7072 6f74 6569  </a>) and protei
+00000b00: 6e2d 444e 4120 616c 6967 6e6d 656e 7473  n-DNA alignments
+00000b10: 2028 6672 6f6d 203c 6120 6872 6566 3d22   (from <a href="
+00000b20: 6874 7470 733a 2f2f 6163 6164 656d 6963  https://academic
+00000b30: 2e6f 7570 2e63 6f6d 2f62 696f 696e 666f  .oup.com/bioinfo
+00000b40: 726d 6174 6963 732f 6172 7469 636c 652f  rmatics/article/
+00000b50: 3339 2f31 2f62 7461 6430 3134 2f36 3938  39/1/btad014/698
+00000b60: 3936 3231 2220 7461 7267 6574 3d22 5f62  9621" target="_b
+00000b70: 6c61 6e6b 223e 6d69 6e69 7072 6f74 3c2f  lank">miniprot</
+00000b80: 613e 2c20 6372 6564 6974 7320 746f 203c  a>, credits to <
+00000b90: 6120 6872 6566 3d22 6874 7470 3a2f 2f6c  a href="http://l
+00000ba0: 6968 656e 672e 6f72 6722 2074 6172 6765  iheng.org" targe
+00000bb0: 743d 225f 626c 616e 6b22 3e44 722e 2048  t="_blank">Dr. H
+00000bc0: 656e 6720 4c69 3c2f 613e 2920 746f 2061  eng Li</a>) to a
+00000bd0: 6363 7572 6174 656c 7920 6d61 7020 616e  ccurately map an
+00000be0: 6e6f 7461 7469 6f6e 7320 6265 7477 6565  notations betwee
+00000bf0: 6e20 6765 6e6f 6d65 2061 7373 656d 626c  n genome assembl
+00000c00: 6965 7320 6f66 2074 6865 2073 616d 6520  ies of the same 
+00000c10: 6f72 2064 6966 6665 7265 6e74 2073 7065  or different spe
+00000c20: 6369 6573 2e20 4c69 6674 4f6e 2065 6d70  cies. LiftOn emp
+00000c30: 6c6f 7973 2061 2074 776f 2d73 7465 7020  loys a two-step 
+00000c40: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000c50: 2f63 6362 2e6a 6875 2e65 6475 2f6c 6966  /ccb.jhu.edu/lif
+00000c60: 746f 6e2f 636f 6e74 656e 742f 6265 6869  ton/content/behi
+00000c70: 6e64 5f73 6365 6e65 732e 6874 6d6c 2370  nd_scenes.html#p
+00000c80: 726f 7465 696e 2d6d 6178 696d 697a 6174  rotein-maximizat
+00000c90: 696f 6e2d 616c 676f 7269 7468 6d22 3e70  ion-algorithm">p
+00000ca0: 726f 7465 696e 206d 6178 696d 697a 6174  rotein maximizat
+00000cb0: 696f 6e20 616c 676f 7269 7468 6d3c 2f61  ion algorithm</a
+00000cc0: 3e20 746f 2069 6d70 726f 7665 2074 6865  > to improve the
+00000cd0: 2061 6e6e 6f74 6174 696f 6e20 6f66 2070   annotation of p
+00000ce0: 726f 7465 696e 2d63 6f64 696e 6720 6765  rotein-coding ge
+00000cf0: 6e65 7320 696e 2074 6865 2054 3254 2d43  nes in the T2T-C
+00000d00: 484d 3133 203c 6120 6872 6566 3d22 6874  HM13 <a href="ht
+00000d10: 7470 733a 2f2f 7333 2d75 732d 7765 7374  tps://s3-us-west
+00000d20: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
+00000d30: 2f68 756d 616e 2d70 616e 6765 6e6f 6d69  /human-pangenomi
+00000d40: 6373 2f54 3254 2f43 484d 3133 2f61 7373  cs/T2T/CHM13/ass
+00000d50: 656d 626c 6965 732f 616e 6e6f 7461 7469  emblies/annotati
+00000d60: 6f6e 2f63 686d 3133 7632 2e30 5f52 6566  on/chm13v2.0_Ref
+00000d70: 5365 715f 4c69 6674 6f66 665f 7635 2e31  Seq_Liftoff_v5.1
+00000d80: 2e67 6666 332e 677a 2220 7461 7267 6574  .gff3.gz" target
+00000d90: 3d22 5f62 6c61 6e6b 223e 4a48 5520 5265  ="_blank">JHU Re
+00000da0: 6653 6571 7631 3130 202b 204c 6966 746f  fSeqv110 + Lifto
+00000db0: 6666 2076 352e 313c 2f61 3e20 616e 6e6f  ff v5.1</a> anno
+00000dc0: 7461 7469 6f6e 2e0a 5468 6520 6c61 7465  tation..The late
+00000dd0: 7374 2054 3254 2d43 484d 3133 2061 6e6e  st T2T-CHM13 ann
+00000de0: 6f74 6174 696f 6e20 6765 6e65 7261 7465  otation generate
+00000df0: 6420 6279 204c 6966 744f 6e20 6973 2061  d by LiftOn is a
+00000e00: 7661 696c 6162 6c65 2061 7320 3c61 2068  vailable as <a h
+00000e10: 7265 663d 2268 7474 7073 3a2f 2f74 696e  ref="https://tin
+00000e20: 7975 726c 2e63 6f6d 2f34 7879 7774 7776  yurl.com/4xywtwv
+00000e30: 6522 2074 6172 6765 743d 225f 626c 616e  e" target="_blan
+00000e40: 6b22 3e4a 4855 5f4c 6966 744f 6e5f 7631  k">JHU_LiftOn_v1
+00000e50: 2e30 5f63 686d 3133 7632 2e30 2e67 6666  .0_chm13v2.0.gff
+00000e60: 3320 2866 7470 3a2f 2f66 7470 2e63 6362  3 (ftp://ftp.ccb
+00000e70: 2e6a 6875 2e65 6475 2f70 7562 2f64 6174  .jhu.edu/pub/dat
+00000e80: 612f 4c69 6674 4f6e 2f4a 4855 5f4c 6966  a/LiftOn/JHU_Lif
+00000e90: 744f 6e5f 7631 2e30 5f63 686d 3133 7632  tOn_v1.0_chm13v2
+00000ea0: 2e30 2e67 6666 3329 203c 6920 636c 6173  .0.gff3) <i clas
+00000eb0: 733d 2266 6120 6661 2d64 6f77 6e6c 6f61  s="fa fa-downloa
+00000ec0: 6422 3e3c 2f69 3e3c 2f61 3e2e 3c73 6563  d"></i></a>.<sec
+00000ed0: 7469 6f6e 2069 643d 2277 6879 2d6c 6966  tion id="why-lif
+00000ee0: 746f 6e22 2063 6c61 7373 3d22 223e 0a3c  ton" class="">.<
+00000ef0: 6832 3e57 6879 204c 6966 744f 6ee2 9d93  h2>Why LiftOn...
+00000f00: 3c61 2063 6c61 7373 3d22 6865 6164 6572  <a class="header
+00000f10: 6c69 6e6b 2220 6872 6566 3d22 2377 6879  link" href="#why
+00000f20: 2d6c 6966 746f 6e22 2074 6974 6c65 3d22  -lifton" title="
+00000f30: 5065 726d 616c 696e 6b20 746f 2074 6869  Permalink to thi
+00000f40: 7320 6865 6164 696e 6722 3e23 3c2f 613e  s heading">#</a>
+00000f50: 3c2f 6832 3e0a 3c6f 6c20 636c 6173 733d  </h2>.<ol class=
+00000f60: 2261 7261 6269 6320 7369 6d70 6c65 223e  "arabic simple">
+00000f70: 0a3c 6c69 3e3c 703e 3c73 7472 6f6e 673e  .<li><p><strong>
+00000f80: 4275 7267 656f 6e69 6e67 206e 756d 6265  Burgeoning numbe
+00000f90: 7220 6f66 2067 656e 6f6d 6520 6173 7365  r of genome asse
+00000fa0: 6d62 6c69 6573 3c2f 7374 726f 6e67 3e3a  mblies</strong>:
+00000fb0: 2041 7320 6f66 2044 6563 656d 6265 7220   As of December 
+00000fc0: 3230 3233 2c20 7468 6572 6520 6172 6520  2023, there are 
+00000fd0: 3330 2c35 3330 2065 756b 6172 796f 7469  30,530 eukaryoti
+00000fe0: 6320 6765 6e6f 6d65 732c 2035 3637 2c32  c genomes, 567,2
+00000ff0: 3238 2070 726f 6b61 7279 6f74 6963 2067  28 prokaryotic g
+00001000: 656e 6f6d 6573 2c20 616e 6420 3636 2c34  enomes, and 66,4
+00001010: 3239 2076 6972 7573 6573 206c 6973 7465  29 viruses liste
+00001020: 6420 6f6e 204e 4342 4920 283c 6120 636c  d on NCBI (<a cl
+00001030: 6173 733d 2272 6566 6572 656e 6365 2065  ass="reference e
+00001040: 7874 6572 6e61 6c22 2068 7265 663d 2268  xternal" href="h
+00001050: 7474 7073 3a2f 2f77 7777 2e6e 6362 692e  ttps://www.ncbi.
+00001060: 6e6c 6d2e 6e69 682e 676f 762f 6765 6e6f  nlm.nih.gov/geno
+00001070: 6d65 2f62 726f 7773 652f 2321 2f6f 7665  me/browse/#!/ove
+00001080: 7276 6965 772f 223e 4e43 4249 2067 656e  rview/">NCBI gen
+00001090: 6f6d 6520 6272 6f77 7365 723c 2f61 3e29  ome browser</a>)
+000010a0: 2e20 486f 7765 7665 722c 2067 656e 6f6d  . However, genom
+000010b0: 6520 616e 6e6f 7461 7469 6f6e 2069 7320  e annotation is 
+000010c0: 6c61 6767 696e 6720 6265 6869 6e64 2e20  lagging behind. 
+000010d0: 4173 206d 6f72 6520 6869 6768 2d71 7561  As more high-qua
+000010e0: 6c69 7479 2061 7373 656d 626c 6965 7320  lity assemblies 
+000010f0: 6172 6520 6765 6e65 7261 7465 642c 2077  are generated, w
+00001100: 6520 6e65 6564 2061 6e20 6163 6375 7261  e need an accura
+00001110: 7465 206c 6966 742d 6f76 6572 2074 6f6f  te lift-over too
+00001120: 6c20 746f 2061 6e6e 6f74 6174 6520 7468  l to annotate th
+00001130: 656d 2e3c 2f70 3e3c 2f6c 693e 0a3c 6c69  em.</p></li>.<li
+00001140: 3e3c 703e 3c73 7472 6f6e 673e 496d 7072  ><p><strong>Impr
+00001150: 6f76 6564 2070 726f 7465 696e 2d63 6f64  oved protein-cod
+00001160: 696e 6720 6765 6e65 206d 6170 7069 6e67  ing gene mapping
+00001170: 3c2f 7374 726f 6e67 3e3a 2054 6865 2070  </strong>: The p
+00001180: 6f70 756c 6172 203c 6120 636c 6173 733d  opular <a class=
+00001190: 2272 6566 6572 656e 6365 2065 7874 6572  "reference exter
+000011a0: 6e61 6c22 2068 7265 663d 2268 7474 7073  nal" href="https
+000011b0: 3a2f 2f61 6361 6465 6d69 632e 6f75 702e  ://academic.oup.
+000011c0: 636f 6d2f 6269 6f69 6e66 6f72 6d61 7469  com/bioinformati
+000011d0: 6373 2f61 7274 6963 6c65 2f33 372f 3132  cs/article/37/12
+000011e0: 2f31 3633 392f 3630 3335 3132 383f 6c6f  /1639/6035128?lo
+000011f0: 6769 6e3d 7472 7565 223e 4c69 6674 6f66  gin=true">Liftof
+00001200: 663c 2f61 3e20 746f 6f6c 206d 6170 7320  f</a> tool maps 
+00001210: 6765 6e65 7320 6261 7365 6420 6f6e 2044  genes based on D
+00001220: 4e41 2061 6c69 676e 6d65 6e74 7320 616c  NA alignments al
+00001230: 6f6e 652e 203c 6120 636c 6173 733d 2272  one. <a class="r
+00001240: 6566 6572 656e 6365 2065 7874 6572 6e61  eference externa
+00001250: 6c22 2068 7265 663d 2268 7474 7073 3a2f  l" href="https:/
+00001260: 2f67 6974 6875 622e 636f 6d2f 6c68 332f  /github.com/lh3/
+00001270: 6d69 6e69 7072 6f74 223e 4d69 6e69 7072  miniprot">Minipr
+00001280: 6f74 3c2f 613e 206d 6170 7320 6765 6e65  ot</a> maps gene
+00001290: 7320 6261 7365 6420 6f6e 2070 726f 7465  s based on prote
+000012a0: 696e 2061 6c69 676e 6d65 6e74 7320 6275  in alignments bu
+000012b0: 742c 2077 6974 686f 7574 2067 656e 6520  t, without gene 
+000012c0: 7374 7275 6374 7572 6520 696e 666f 726d  structure inform
+000012d0: 6174 696f 6e2c 206d 6179 206e 6f74 2062  ation, may not b
+000012e0: 6520 6173 2061 6363 7572 6174 6520 6f6e  e as accurate on
+000012f0: 2074 6865 6972 206f 776e 2028 5365 6520   their own (See 
+00001300: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
+00001310: 6e63 6520 696e 7465 726e 616c 2220 6872  nce internal" hr
+00001320: 6566 3d22 6874 7470 733a 2f2f 6363 622e  ef="https://ccb.
+00001330: 6a68 752e 6564 752f 6c69 6674 6f6e 2f63  jhu.edu/lifton/c
+00001340: 6f6e 7465 6e74 2f68 6f77 5f74 6f5f 7061  ontent/how_to_pa
+00001350: 6765 2e68 746d 6c23 7768 792d 6c69 6674  ge.html#why-lift
+00001360: 6f6e 2d71 6122 3e3c 7370 616e 2063 6c61  on-qa"><span cla
+00001370: 7373 3d22 7374 6420 7374 642d 7265 6622  ss="std std-ref"
+00001380: 3e46 4151 2043 6f6d 6d6f 6e20 6d69 7374  >FAQ Common mist
+00001390: 616b 6573 206f 6620 4c69 6674 6f66 6620  akes of Liftoff 
+000013a0: 616e 6420 6d69 6e69 7072 6f74 3c2f 7370  and miniprot</sp
+000013b0: 616e 3e3c 2f61 3e29 2e20 4c69 6674 4f6e  an></a>). LiftOn
+000013c0: 2063 6f6d 6269 6e65 7320 626f 7468 2044   combines both D
+000013d0: 4e41 2d74 6f2d 6765 6e6f 6d65 2061 6e64  NA-to-genome and
+000013e0: 2070 726f 7465 696e 2d74 6f2d 6765 6e6f   protein-to-geno
+000013f0: 6d65 2061 6c69 676e 6d65 6e74 7320 616e  me alignments an
+00001400: 6420 7072 6f64 7563 6573 2062 6574 7465  d produces bette
+00001410: 7220 6765 6e65 206d 6170 7069 6e67 2072  r gene mapping r
+00001420: 6573 756c 7473 2120 4c69 6674 4f6e 2069  esults! LiftOn i
+00001430: 6d70 726f 7665 7320 7570 6f6e 2074 6865  mproves upon the
+00001440: 2063 7572 7265 6e74 2072 656c 6561 7365   current release
+00001450: 6420 5432 542d 4348 4d31 3320 616e 6e6f  d T2T-CHM13 anno
+00001460: 7461 7469 6f6e 2028 3c61 2063 6c61 7373  tation (<a class
+00001470: 3d22 7265 6665 7265 6e63 6520 6578 7465  ="reference exte
+00001480: 726e 616c 2220 6872 6566 3d22 6874 7470  rnal" href="http
+00001490: 733a 2f2f 7333 2d75 732d 7765 7374 2d32  s://s3-us-west-2
+000014a0: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f68  .amazonaws.com/h
+000014b0: 756d 616e 2d70 616e 6765 6e6f 6d69 6373  uman-pangenomics
+000014c0: 2f54 3254 2f43 484d 3133 2f61 7373 656d  /T2T/CHM13/assem
+000014d0: 626c 6965 732f 616e 6e6f 7461 7469 6f6e  blies/annotation
+000014e0: 2f63 686d 3133 7632 2e30 5f52 6566 5365  /chm13v2.0_RefSe
+000014f0: 715f 4c69 6674 6f66 665f 7635 2e31 2e67  q_Liftoff_v5.1.g
+00001500: 6666 332e 677a 223e 4a48 5520 5265 6653  ff3.gz">JHU RefS
+00001510: 6571 7631 3130 202b 204c 6966 746f 6666  eqv110 + Liftoff
+00001520: 2076 352e 313c 2f61 3e29 2e3c 2f70 3e3c   v5.1</a>).</p><
+00001530: 2f6c 693e 0a3c 6c69 3e3c 703e 3c73 7472  /li>.<li><p><str
+00001540: 6f6e 673e 496d 7072 6f76 6564 2064 6973  ong>Improved dis
+00001550: 7461 6e74 6c79 2072 656c 6174 6564 2073  tantly related s
+00001560: 7065 6369 6573 206c 6966 742d 6f76 6572  pecies lift-over
+00001570: 3c2f 7374 726f 6e67 3e3a 2041 206b 6579  </strong>: A key
+00001580: 206c 696d 6974 6174 696f 6e20 6f66 2044   limitation of D
+00001590: 4e41 2d62 6173 6564 206c 6966 742d 6f76  NA-based lift-ov
+000015a0: 6572 2074 6f6f 6c73 2069 7320 7468 6174  er tools is that
+000015b0: 2074 6865 7920 646f 206e 6f74 2070 6572   they do not per
+000015c0: 666f 726d 2077 656c 6c20 7768 656e 2074  form well when t
+000015d0: 6865 2072 6566 6572 656e 6365 2061 6e64  he reference and
+000015e0: 2074 6172 6765 7420 6765 6e6f 6d65 7320   target genomes 
+000015f0: 6861 7665 2073 6967 6e69 6669 6361 6e74  have significant
+00001600: 6c79 2064 6976 6572 6765 642e 2057 6974  ly diverged. Wit
+00001610: 6820 7468 6520 6865 6c70 206f 6620 7072  h the help of pr
+00001620: 6f74 6569 6e20 616c 6967 6e6d 656e 7473  otein alignments
+00001630: 2061 6e64 2074 6865 2070 726f 7465 696e   and the protein
+00001640: 206d 6178 696d 697a 6174 696f 6e20 616c   maximization al
+00001650: 676f 7269 7468 6d2c 204c 6966 744f 6e20  gorithm, LiftOn 
+00001660: 696d 7072 6f76 6573 2074 6865 206c 6966  improves the lif
+00001670: 742d 6f76 6572 2070 726f 6365 7373 2062  t-over process b
+00001680: 6574 7765 656e 2064 6973 7461 6e74 6c79  etween distantly
+00001690: 2072 656c 6174 6564 2073 7065 6369 6573   related species
+000016a0: 2e20 5365 6520 223c 6120 636c 6173 733d  . See "<a class=
+000016b0: 2272 6566 6572 656e 6365 2069 6e74 6572  "reference inter
+000016c0: 6e61 6c22 2068 7265 663d 2268 7474 7073  nal" href="https
+000016d0: 3a2f 2f63 6362 2e6a 6875 2e65 6475 2f6c  ://ccb.jhu.edu/l
+000016e0: 6966 746f 6e2f 636f 6e74 656e 742f 6469  ifton/content/di
+000016f0: 7374 616e 745f 7370 6563 6965 735f 6c69  stant_species_li
+00001700: 6674 6f76 6572 2f6c 6966 746f 7665 725f  ftover/liftover_
+00001710: 6d6f 7573 655f 325f 7261 742e 6874 6d6c  mouse_2_rat.html
+00001720: 2364 6973 7461 6e74 2d73 7065 6369 6573  #distant-species
+00001730: 2d6c 6966 746f 7665 722d 6d6f 7573 652d  -liftover-mouse-
+00001740: 746f 2d72 6174 223e 3c73 7061 6e20 636c  to-rat"><span cl
+00001750: 6173 733d 2273 7464 2073 7464 2d72 6566  ass="std std-ref
+00001760: 223e 4d6f 7573 6520 746f 2052 6174 3c2f  ">Mouse to Rat</
+00001770: 7370 616e 3e3c 2f61 3e22 2061 6e64 2022  span></a>" and "
+00001780: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
+00001790: 6e63 6520 696e 7465 726e 616c 2220 6872  nce internal" hr
+000017a0: 6566 3d22 6874 7470 733a 2f2f 6363 622e  ef="https://ccb.
+000017b0: 6a68 752e 6564 752f 6c69 6674 6f6e 2f63  jhu.edu/lifton/c
+000017c0: 6f6e 7465 6e74 2f64 6973 7461 6e74 5f73  ontent/distant_s
+000017d0: 7065 6369 6573 5f6c 6966 746f 7665 722f  pecies_liftover/
+000017e0: 6c69 6674 6f76 6572 5f64 726f 736f 7068  liftover_drosoph
+000017f0: 696c 615f 6572 6563 7461 2e68 746d 6c23  ila_erecta.html#
+00001800: 6469 7374 616e 742d 7370 6563 6965 732d  distant-species-
+00001810: 6c69 6674 6f76 6572 2d64 726f 736f 7068  liftover-drosoph
+00001820: 696c 612d 6d65 6c61 6e6f 6761 7374 6572  ila-melanogaster
+00001830: 2d32 2d65 7265 6374 6122 3e3c 7370 616e  -2-erecta"><span
+00001840: 2063 6c61 7373 3d22 7374 6420 7374 642d   class="std std-
+00001850: 7265 6622 3e44 726f 736f 7068 696c 6120  ref">Drosophila 
+00001860: 6d65 6c61 6e6f 6761 7374 6572 2074 6f20  melanogaster to 
+00001870: 4472 6f73 6f70 6869 6c61 2065 7265 6374  Drosophila erect
+00001880: 613c 2f73 7061 6e3e 3c2f 613e 2220 7265  a</span></a>" re
+00001890: 7375 6c74 2073 6563 7469 6f6e 732e 3c2f  sult sections.</
+000018a0: 703e 3c2f 6c69 3e0a 3c2f 6f6c 3e0a 3c70  p></li>.</ol>.<p
+000018b0: 3e4c 6966 744f 6e20 6973 2066 7265 652c  >LiftOn is free,
+000018c0: 2069 7427 7320 6f70 656e 2073 6f75 7263   it's open sourc
+000018d0: 652c 2069 7427 7320 6561 7379 2074 6f20  e, it's easy to 
+000018e0: 696e 7374 616c 6c20 2c20 616e 6420 6974  install , and it
+000018f0: 2773 2069 6e20 5079 7468 6f6e 213c 2f70  's in Python!</p
+00001900: 3e0a 3c64 6976 2063 6c61 7373 3d22 6c69  >.<div class="li
+00001910: 6e65 2d62 6c6f 636b 223e 0a3c 6469 7620  ne-block">.<div 
+00001920: 636c 6173 733d 226c 696e 6522 3e3c 6272  class="line"><br
+00001930: 3e3c 2f64 6976 3e0a 3c2f 6469 763e 0a3c  ></div>.</div>.<
+00001940: 2f73 6563 7469 6f6e 3e0a 3c73 6563 7469  /section>.<secti
+00001950: 6f6e 2069 643d 2277 686f 2d69 732d 6974  on id="who-is-it
+00001960: 2d66 6f72 2220 636c 6173 733d 2222 3e0a  -for" class="">.
+00001970: 3c68 323e 5768 6f20 6973 2069 7420 666f  <h2>Who is it fo
+00001980: 72e2 9d93 3c61 2063 6c61 7373 3d22 6865  r...<a class="he
+00001990: 6164 6572 6c69 6e6b 2220 6872 6566 3d22  aderlink" href="
+000019a0: 2377 686f 2d69 732d 6974 2d66 6f72 2220  #who-is-it-for" 
+000019b0: 7469 746c 653d 2250 6572 6d61 6c69 6e6b  title="Permalink
+000019c0: 2074 6f20 7468 6973 2068 6561 6469 6e67   to this heading
+000019d0: 223e 233c 2f61 3e3c 2f68 323e 0a3c 703e  ">#</a></h2>.<p>
+000019e0: 4c69 6674 4f6e 2069 7320 6465 7369 676e  LiftOn is design
+000019f0: 6564 2066 6f72 2072 6573 6561 7263 6865  ed for researche
+00001a00: 7273 2061 6e64 2062 696f 696e 666f 726d  rs and bioinform
+00001a10: 6174 6963 6961 6e73 2077 686f 2061 7265  aticians who are
+00001a20: 2069 6e74 6572 6573 7465 6420 696e 2067   interested in g
+00001a30: 656e 6f6d 6520 616e 6e6f 7461 7469 6f6e  enome annotation
+00001a40: 2e20 4974 2069 7320 616e 2065 6173 792d  . It is an easy-
+00001a50: 746f 2d69 6e73 7461 6c6c 2061 6e64 2065  to-install and e
+00001a60: 6173 792d 746f 2d72 756e 2063 6f6d 6d61  asy-to-run comma
+00001a70: 6e64 2d6c 696e 6520 746f 6f6c 2e20 5370  nd-line tool. Sp
+00001a80: 6563 6966 6963 616c 6c79 2c20 6974 2069  ecifically, it i
+00001a90: 7320 6265 6e65 6669 6369 616c 2069 6e20  s beneficial in 
+00001aa0: 7468 6520 666f 6c6c 6f77 696e 6720 7363  the following sc
+00001ab0: 656e 6172 696f 733a 3c2f 703e 0a3c 6f6c  enarios:</p>.<ol
+00001ac0: 2063 6c61 7373 3d22 6172 6162 6963 2073   class="arabic s
+00001ad0: 696d 706c 6522 3e0a 3c6c 693e 3c70 3e49  imple">.<li><p>I
+00001ae0: 6620 796f 7520 6861 7665 2073 6571 7565  f you have seque
+00001af0: 6e63 6564 2061 6e64 2061 7373 656d 626c  nced and assembl
+00001b00: 6564 2061 206e 6577 2067 656e 6f6d 6520  ed a new genome 
+00001b10: 616e 6420 7265 7175 6972 6520 616e 6e6f  and require anno
+00001b20: 7461 7469 6f6e 2c20 4c69 6674 4f6e 2070  tation, LiftOn p
+00001b30: 726f 7669 6465 7320 616e 2065 6666 6963  rovides an effic
+00001b40: 6965 6e74 2073 6f6c 7574 696f 6e20 666f  ient solution fo
+00001b50: 7220 6765 6e65 7261 7469 6e67 2061 6e6e  r generating ann
+00001b60: 6f74 6174 696f 6e73 2066 6f72 2079 6f75  otations for you
+00001b70: 7220 6765 6e6f 6d65 2e3c 2f70 3e3c 2f6c  r genome.</p></l
+00001b80: 693e 0a3c 6c69 3e3c 703e 4c69 6674 4f6e  i>.<li><p>LiftOn
+00001b90: 2069 7320 616e 2065 7863 656c 6c65 6e74   is an excellent
+00001ba0: 2074 6f6f 6c20 666f 7220 7468 6f73 6520   tool for those 
+00001bb0: 6c6f 6f6b 696e 6720 746f 2070 6572 666f  looking to perfo
+00001bc0: 726d 2063 6f6d 7061 7261 7469 7665 2067  rm comparative g
+00001bd0: 656e 6f6d 6963 7320 616e 616c 7973 6973  enomics analysis
+00001be0: 2e20 4974 2066 6163 696c 6974 6174 6573  . It facilitates
+00001bf0: 2074 6865 206c 6966 7469 6e67 206f 7665   the lifting ove
+00001c00: 7220 616e 6420 636f 6d70 6172 6973 6f6e  r and comparison
+00001c10: 206f 6620 6765 6e65 2063 6f6e 7465 6e74   of gene content
+00001c20: 7320 6265 7477 6565 6e20 6469 6666 6572  s between differ
+00001c30: 656e 7420 6765 6e6f 6d65 732c 2061 6964  ent genomes, aid
+00001c40: 696e 6720 696e 2075 6e64 6572 7374 616e  ing in understan
+00001c50: 6469 6e67 2065 766f 6c75 7469 6f6e 6172  ding evolutionar
+00001c60: 7920 7265 6c61 7469 6f6e 7368 6970 7320  y relationships 
+00001c70: 616e 6420 6675 6e63 7469 6f6e 616c 2067  and functional g
+00001c80: 656e 6f6d 6963 732e 3c2f 703e 3c2f 6c69  enomics.</p></li
+00001c90: 3e0a 3c6c 693e 3c70 3e46 6f72 2072 6573  >.<li><p>For res
+00001ca0: 6561 7263 6865 7273 2069 6e74 6572 6573  earchers interes
+00001cb0: 7465 6420 696e 2075 7369 6e67 2054 3254  ted in using T2T
+00001cc0: 2d43 484d 3133 2061 6e6e 6f74 6174 696f  -CHM13 annotatio
+00001cd0: 6e73 2c20 7472 7920 4c69 6674 4f6e 2120  ns, try LiftOn! 
+00001ce0: 5765 2068 6176 6520 7072 652d 6765 6e65  We have pre-gene
+00001cf0: 7261 7465 6420 7468 6520 3c61 2063 6c61  rated the <a cla
+00001d00: 7373 3d22 7265 6665 7265 6e63 6520 6578  ss="reference ex
+00001d10: 7465 726e 616c 2220 6872 6566 3d22 6874  ternal" href="ht
+00001d20: 7470 733a 2f2f 7469 6e79 7572 6c2e 636f  tps://tinyurl.co
+00001d30: 6d2f 3478 7977 7477 7665 223e 4a48 555f  m/4xywtwve">JHU_
+00001d40: 4c69 6674 4f6e 5f76 312e 305f 6368 6d31  LiftOn_v1.0_chm1
+00001d50: 3376 322e 302e 6766 6633 3c2f 613e 2028  3v2.0.gff3</a> (
+00001d60: 6674 703a 2f2f 6674 702e 6363 622e 6a68  ftp://ftp.ccb.jh
+00001d70: 752e 6564 752f 7075 622f 6461 7461 2f4c  u.edu/pub/data/L
+00001d80: 6966 744f 6e2f 4a48 555f 4c69 6674 4f6e  iftOn/JHU_LiftOn
+00001d90: 5f76 312e 305f 6368 6d31 3376 322e 302e  _v1.0_chm13v2.0.
+00001da0: 6766 6633 2920 6669 6c65 2066 6f72 2079  gff3) file for y
+00001db0: 6f75 7220 636f 6e76 656e 6965 6e63 652e  our convenience.
+00001dc0: 3c2f 703e 3c2f 6c69 3e0a 3c2f 6f6c 3e0a  </p></li>.</ol>.
+00001dd0: 3c64 6976 2063 6c61 7373 3d22 6c69 6e65  <div class="line
+00001de0: 2d62 6c6f 636b 223e 0a3c 6469 7620 636c  -block">.<div cl
+00001df0: 6173 733d 226c 696e 6522 3e3c 6272 3e3c  ass="line"><br><
+00001e00: 2f64 6976 3e0a 3c2f 6469 763e 0a3c 2f73  /div>.</div>.</s
+00001e10: 6563 7469 6f6e 3e0a 3c73 6563 7469 6f6e  ection>.<section
+00001e20: 2069 643d 2277 6861 742d 646f 6573 2d6c   id="what-does-l
+00001e30: 6966 746f 6e2d 646f 2220 636c 6173 733d  ifton-do" class=
+00001e40: 2222 3e0a 3c68 323e 5768 6174 2064 6f65  "">.<h2>What doe
+00001e50: 7320 4c69 6674 4f6e 2064 6fe2 9d93 3c61  s LiftOn do...<a
+00001e60: 2063 6c61 7373 3d22 6865 6164 6572 6c69   class="headerli
+00001e70: 6e6b 2220 6872 6566 3d22 2377 6861 742d  nk" href="#what-
+00001e80: 646f 6573 2d6c 6966 746f 6e2d 646f 2220  does-lifton-do" 
+00001e90: 7469 746c 653d 2250 6572 6d61 6c69 6e6b  title="Permalink
+00001ea0: 2074 6f20 7468 6973 2068 6561 6469 6e67   to this heading
+00001eb0: 223e 233c 2f61 3e3c 2f68 323e 0a3c 703e  ">#</a></h2>.<p>
+00001ec0: 4c65 7427 7320 6669 7273 7420 6465 6669  Let's first defi
+00001ed0: 6e65 2074 6865 2070 726f 626c 656d 3a0a  ne the problem:.
+00001ee0: 4769 7665 6e20 6120 7265 6665 7265 6e63  Given a referenc
+00001ef0: 6520 3c73 7472 6f6e 673e 4765 6e6f 6d65  e <strong>Genome
+00001f00: 3c2f 7374 726f 6e67 3e20 3c73 7061 6e20  </strong> <span 
+00001f10: 636c 6173 733d 226d 6174 6820 6e6f 7472  class="math notr
+00001f20: 616e 736c 6174 6520 6e6f 6869 6768 6c69  anslate nohighli
+00001f30: 6768 7422 3e3c 6d6a 782d 636f 6e74 6169  ght"><mjx-contai
+00001f40: 6e65 7220 636c 6173 733d 224d 6174 684a  ner class="MathJ
+00001f50: 6178 2043 7478 744d 656e 755f 4174 7461  ax CtxtMenu_Atta
+00001f60: 6368 6564 5f30 2220 6a61 783d 2243 4854  ched_0" jax="CHT
+00001f70: 4d4c 2220 7461 6269 6e64 6578 3d22 3022  ML" tabindex="0"
+00001f80: 2063 7478 746d 656e 755f 636f 756e 7465   ctxtmenu_counte
+00001f90: 723d 2230 2220 7374 796c 653d 2266 6f6e  r="0" style="fon
+00001fa0: 742d 7369 7a65 3a20 3131 382e 3925 3b20  t-size: 118.9%; 
+00001fb0: 706f 7369 7469 6f6e 3a20 7265 6c61 7469  position: relati
+00001fc0: 7665 3b22 3e3c 6d6a 782d 6d61 7468 2063  ve;"><mjx-math c
+00001fd0: 6c61 7373 3d22 4d4a 582d 5445 5822 2061  lass="MJX-TEX" a
+00001fe0: 7269 612d 6869 6464 656e 3d22 7472 7565  ria-hidden="true
+00001ff0: 223e 3c6d 6a78 2d6d 6920 636c 6173 733d  "><mjx-mi class=
+00002000: 226d 6a78 2d69 223e 3c6d 6a78 2d63 2063  "mjx-i"><mjx-c c
+00002010: 6c61 7373 3d22 6d6a 782d 6331 4434 3435  lass="mjx-c1D445
+00002020: 2054 4558 2d49 223e 3c2f 6d6a 782d 633e   TEX-I"></mjx-c>
+00002030: 3c2f 6d6a 782d 6d69 3e3c 2f6d 6a78 2d6d  </mjx-mi></mjx-m
+00002040: 6174 683e 3c6d 6a78 2d61 7373 6973 7469  ath><mjx-assisti
+00002050: 7665 2d6d 6d6c 2075 6e73 656c 6563 7461  ve-mml unselecta
+00002060: 626c 653d 226f 6e22 2064 6973 706c 6179  ble="on" display
+00002070: 3d22 696e 6c69 6e65 223e 3c6d 6174 6820  ="inline"><math 
+00002080: 786d 6c6e 733d 2268 7474 703a 2f2f 7777  xmlns="http://ww
+00002090: 772e 7733 2e6f 7267 2f31 3939 382f 4d61  w.w3.org/1998/Ma
+000020a0: 7468 2f4d 6174 684d 4c22 3e3c 6d69 3e52  th/MathML"><mi>R
+000020b0: 3c2f 6d69 3e3c 2f6d 6174 683e 3c2f 6d6a  </mi></math></mj
+000020c0: 782d 6173 7369 7374 6976 652d 6d6d 6c3e  x-assistive-mml>
+000020d0: 3c2f 6d6a 782d 636f 6e74 6169 6e65 723e  </mjx-container>
+000020e0: 3c2f 7370 616e 3e2c 2061 6e20 3c73 7472  </span>, an <str
+000020f0: 6f6e 673e 416e 6e6f 7461 7469 6f6e 3c2f  ong>Annotation</
+00002100: 7374 726f 6e67 3e20 3c73 7061 6e20 636c  strong> <span cl
+00002110: 6173 733d 226d 6174 6820 6e6f 7472 616e  ass="math notran
+00002120: 736c 6174 6520 6e6f 6869 6768 6c69 6768  slate nohighligh
+00002130: 7422 3e3c 6d6a 782d 636f 6e74 6169 6e65  t"><mjx-containe
+00002140: 7220 636c 6173 733d 224d 6174 684a 6178  r class="MathJax
+00002150: 2043 7478 744d 656e 755f 4174 7461 6368   CtxtMenu_Attach
+00002160: 6564 5f30 2220 6a61 783d 2243 4854 4d4c  ed_0" jax="CHTML
+00002170: 2220 7461 6269 6e64 6578 3d22 3022 2063  " tabindex="0" c
+00002180: 7478 746d 656e 755f 636f 756e 7465 723d  txtmenu_counter=
+00002190: 2231 2220 7374 796c 653d 2266 6f6e 742d  "1" style="font-
+000021a0: 7369 7a65 3a20 3131 382e 3925 3b20 706f  size: 118.9%; po
+000021b0: 7369 7469 6f6e 3a20 7265 6c61 7469 7665  sition: relative
+000021c0: 3b22 3e3c 6d6a 782d 6d61 7468 2063 6c61  ;"><mjx-math cla
+000021d0: 7373 3d22 4d4a 582d 5445 5822 2061 7269  ss="MJX-TEX" ari
+000021e0: 612d 6869 6464 656e 3d22 7472 7565 223e  a-hidden="true">
+000021f0: 3c6d 6a78 2d6d 7375 623e 3c6d 6a78 2d6d  <mjx-msub><mjx-m
+00002200: 6920 636c 6173 733d 226d 6a78 2d69 223e  i class="mjx-i">
+00002210: 3c6d 6a78 2d63 2063 6c61 7373 3d22 6d6a  <mjx-c class="mj
+00002220: 782d 6331 4434 3435 2054 4558 2d49 223e  x-c1D445 TEX-I">
+00002230: 3c2f 6d6a 782d 633e 3c2f 6d6a 782d 6d69  </mjx-c></mjx-mi
+00002240: 3e3c 6d6a 782d 7363 7269 7074 2073 7479  ><mjx-script sty
+00002250: 6c65 3d22 7665 7274 6963 616c 2d61 6c69  le="vertical-ali
+00002260: 676e 3a20 2d30 2e31 3533 656d 3b22 3e3c  gn: -0.153em;"><
+00002270: 6d6a 782d 6d69 2063 6c61 7373 3d22 6d6a  mjx-mi class="mj
+00002280: 782d 6922 2073 697a 653d 2273 223e 3c6d  x-i" size="s"><m
+00002290: 6a78 2d63 2063 6c61 7373 3d22 6d6a 782d  jx-c class="mjx-
+000022a0: 6331 4434 3334 2054 4558 2d49 223e 3c2f  c1D434 TEX-I"></
+000022b0: 6d6a 782d 633e 3c2f 6d6a 782d 6d69 3e3c  mjx-c></mjx-mi><
+000022c0: 2f6d 6a78 2d73 6372 6970 743e 3c2f 6d6a  /mjx-script></mj
+000022d0: 782d 6d73 7562 3e3c 2f6d 6a78 2d6d 6174  x-msub></mjx-mat
+000022e0: 683e 3c6d 6a78 2d61 7373 6973 7469 7665  h><mjx-assistive
+000022f0: 2d6d 6d6c 2075 6e73 656c 6563 7461 626c  -mml unselectabl
+00002300: 653d 226f 6e22 2064 6973 706c 6179 3d22  e="on" display="
+00002310: 696e 6c69 6e65 223e 3c6d 6174 6820 786d  inline"><math xm
+00002320: 6c6e 733d 2268 7474 703a 2f2f 7777 772e  lns="http://www.
+00002330: 7733 2e6f 7267 2f31 3939 382f 4d61 7468  w3.org/1998/Math
+00002340: 2f4d 6174 684d 4c22 3e3c 6d73 7562 3e3c  /MathML"><msub><
+00002350: 6d69 3e52 3c2f 6d69 3e3c 6d69 3e41 3c2f  mi>R</mi><mi>A</
+00002360: 6d69 3e3c 2f6d 7375 623e 3c2f 6d61 7468  mi></msub></math
+00002370: 3e3c 2f6d 6a78 2d61 7373 6973 7469 7665  ></mjx-assistive
+00002380: 2d6d 6d6c 3e3c 2f6d 6a78 2d63 6f6e 7461  -mml></mjx-conta
+00002390: 696e 6572 3e3c 2f73 7061 6e3e 2c20 616e  iner></span>, an
+000023a0: 6420 6120 7461 7267 6574 203c 7374 726f  d a target <stro
+000023b0: 6e67 3e47 656e 6f6d 653c 2f73 7472 6f6e  ng>Genome</stron
+000023c0: 673e 203c 7370 616e 2063 6c61 7373 3d22  g> <span class="
+000023d0: 6d61 7468 206e 6f74 7261 6e73 6c61 7465  math notranslate
+000023e0: 206e 6f68 6967 686c 6967 6874 223e 3c6d   nohighlight"><m
+000023f0: 6a78 2d63 6f6e 7461 696e 6572 2063 6c61  jx-container cla
+00002400: 7373 3d22 4d61 7468 4a61 7820 4374 7874  ss="MathJax Ctxt
+00002410: 4d65 6e75 5f41 7474 6163 6865 645f 3022  Menu_Attached_0"
+00002420: 206a 6178 3d22 4348 544d 4c22 2074 6162   jax="CHTML" tab
+00002430: 696e 6465 783d 2230 2220 6374 7874 6d65  index="0" ctxtme
+00002440: 6e75 5f63 6f75 6e74 6572 3d22 3222 2073  nu_counter="2" s
+00002450: 7479 6c65 3d22 666f 6e74 2d73 697a 653a  tyle="font-size:
+00002460: 2031 3138 2e39 253b 2070 6f73 6974 696f   118.9%; positio
+00002470: 6e3a 2072 656c 6174 6976 653b 223e 3c6d  n: relative;"><m
+00002480: 6a78 2d6d 6174 6820 636c 6173 733d 224d  jx-math class="M
+00002490: 4a58 2d54 4558 2220 6172 6961 2d68 6964  JX-TEX" aria-hid
+000024a0: 6465 6e3d 2274 7275 6522 3e3c 6d6a 782d  den="true"><mjx-
+000024b0: 6d69 2063 6c61 7373 3d22 6d6a 782d 6922  mi class="mjx-i"
+000024c0: 3e3c 6d6a 782d 6320 636c 6173 733d 226d  ><mjx-c class="m
+000024d0: 6a78 2d63 3144 3434 3720 5445 582d 4922  jx-c1D447 TEX-I"
+000024e0: 3e3c 2f6d 6a78 2d63 3e3c 2f6d 6a78 2d6d  ></mjx-c></mjx-m
+000024f0: 693e 3c2f 6d6a 782d 6d61 7468 3e3c 6d6a  i></mjx-math><mj
+00002500: 782d 6173 7369 7374 6976 652d 6d6d 6c20  x-assistive-mml 
+00002510: 756e 7365 6c65 6374 6162 6c65 3d22 6f6e  unselectable="on
+00002520: 2220 6469 7370 6c61 793d 2269 6e6c 696e  " display="inlin
+00002530: 6522 3e3c 6d61 7468 2078 6d6c 6e73 3d22  e"><math xmlns="
+00002540: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
+00002550: 672f 3139 3938 2f4d 6174 682f 4d61 7468  g/1998/Math/Math
+00002560: 4d4c 223e 3c6d 693e 543c 2f6d 693e 3c2f  ML"><mi>T</mi></
+00002570: 6d61 7468 3e3c 2f6d 6a78 2d61 7373 6973  math></mjx-assis
+00002580: 7469 7665 2d6d 6d6c 3e3c 2f6d 6a78 2d63  tive-mml></mjx-c
+00002590: 6f6e 7461 696e 6572 3e3c 2f73 7061 6e3e  ontainer></span>
+000025a0: 2e20 5468 6520 6c69 6674 2d6f 7665 7220  . The lift-over 
+000025b0: 7072 6f62 6c65 6d20 6973 2064 6566 696e  problem is defin
+000025c0: 6564 2061 7320 7468 6520 7072 6f63 6573  ed as the proces
+000025d0: 7320 6f66 2063 6861 6e67 696e 6720 7468  s of changing th
+000025e0: 6520 636f 6f72 6469 6e61 7465 7320 6f66  e coordinates of
+000025f0: 203c 7374 726f 6e67 3e41 6e6e 6f74 6174   <strong>Annotat
+00002600: 696f 6e3c 2f73 7472 6f6e 673e 203c 7370  ion</strong> <sp
+00002610: 616e 2063 6c61 7373 3d22 6d61 7468 206e  an class="math n
+00002620: 6f74 7261 6e73 6c61 7465 206e 6f68 6967  otranslate nohig
+00002630: 686c 6967 6874 223e 3c6d 6a78 2d63 6f6e  hlight"><mjx-con
+00002640: 7461 696e 6572 2063 6c61 7373 3d22 4d61  tainer class="Ma
+00002650: 7468 4a61 7820 4374 7874 4d65 6e75 5f41  thJax CtxtMenu_A
+00002660: 7474 6163 6865 645f 3022 206a 6178 3d22  ttached_0" jax="
+00002670: 4348 544d 4c22 2074 6162 696e 6465 783d  CHTML" tabindex=
+00002680: 2230 2220 6374 7874 6d65 6e75 5f63 6f75  "0" ctxtmenu_cou
+00002690: 6e74 6572 3d22 3322 2073 7479 6c65 3d22  nter="3" style="
+000026a0: 666f 6e74 2d73 697a 653a 2031 3138 2e39  font-size: 118.9
+000026b0: 253b 2070 6f73 6974 696f 6e3a 2072 656c  %; position: rel
+000026c0: 6174 6976 653b 223e 3c6d 6a78 2d6d 6174  ative;"><mjx-mat
+000026d0: 6820 636c 6173 733d 224d 4a58 2d54 4558  h class="MJX-TEX
+000026e0: 2220 6172 6961 2d68 6964 6465 6e3d 2274  " aria-hidden="t
+000026f0: 7275 6522 3e3c 6d6a 782d 6d73 7562 3e3c  rue"><mjx-msub><
+00002700: 6d6a 782d 6d69 2063 6c61 7373 3d22 6d6a  mjx-mi class="mj
+00002710: 782d 6922 3e3c 6d6a 782d 6320 636c 6173  x-i"><mjx-c clas
+00002720: 733d 226d 6a78 2d63 3144 3434 3520 5445  s="mjx-c1D445 TE
+00002730: 582d 4922 3e3c 2f6d 6a78 2d63 3e3c 2f6d  X-I"></mjx-c></m
+00002740: 6a78 2d6d 693e 3c6d 6a78 2d73 6372 6970  jx-mi><mjx-scrip
+00002750: 7420 7374 796c 653d 2276 6572 7469 6361  t style="vertica
+00002760: 6c2d 616c 6967 6e3a 202d 302e 3135 3365  l-align: -0.153e
+00002770: 6d3b 223e 3c6d 6a78 2d6d 6920 636c 6173  m;"><mjx-mi clas
+00002780: 733d 226d 6a78 2d69 2220 7369 7a65 3d22  s="mjx-i" size="
+00002790: 7322 3e3c 6d6a 782d 6320 636c 6173 733d  s"><mjx-c class=
+000027a0: 226d 6a78 2d63 3144 3433 3420 5445 582d  "mjx-c1D434 TEX-
+000027b0: 4922 3e3c 2f6d 6a78 2d63 3e3c 2f6d 6a78  I"></mjx-c></mjx
+000027c0: 2d6d 693e 3c2f 6d6a 782d 7363 7269 7074  -mi></mjx-script
+000027d0: 3e3c 2f6d 6a78 2d6d 7375 623e 3c2f 6d6a  ></mjx-msub></mj
+000027e0: 782d 6d61 7468 3e3c 6d6a 782d 6173 7369  x-math><mjx-assi
+000027f0: 7374 6976 652d 6d6d 6c20 756e 7365 6c65  stive-mml unsele
+00002800: 6374 6162 6c65 3d22 6f6e 2220 6469 7370  ctable="on" disp
+00002810: 6c61 793d 2269 6e6c 696e 6522 3e3c 6d61  lay="inline"><ma
+00002820: 7468 2078 6d6c 6e73 3d22 6874 7470 3a2f  th xmlns="http:/
+00002830: 2f77 7777 2e77 332e 6f72 672f 3139 3938  /www.w3.org/1998
+00002840: 2f4d 6174 682f 4d61 7468 4d4c 223e 3c6d  /Math/MathML"><m
+00002850: 7375 623e 3c6d 693e 523c 2f6d 693e 3c6d  sub><mi>R</mi><m
+00002860: 693e 413c 2f6d 693e 3c2f 6d73 7562 3e3c  i>A</mi></msub><
+00002870: 2f6d 6174 683e 3c2f 6d6a 782d 6173 7369  /math></mjx-assi
+00002880: 7374 6976 652d 6d6d 6c3e 3c2f 6d6a 782d  stive-mml></mjx-
+00002890: 636f 6e74 6169 6e65 723e 3c2f 7370 616e  container></span
+000028a0: 3e20 6672 6f6d 203c 7374 726f 6e67 3e47  > from <strong>G
+000028b0: 656e 6f6d 653c 2f73 7472 6f6e 673e 203c  enome</strong> <
+000028c0: 7370 616e 2063 6c61 7373 3d22 6d61 7468  span class="math
+000028d0: 206e 6f74 7261 6e73 6c61 7465 206e 6f68   notranslate noh
+000028e0: 6967 686c 6967 6874 223e 3c6d 6a78 2d63  ighlight"><mjx-c
+000028f0: 6f6e 7461 696e 6572 2063 6c61 7373 3d22  ontainer class="
+00002900: 4d61 7468 4a61 7820 4374 7874 4d65 6e75  MathJax CtxtMenu
+00002910: 5f41 7474 6163 6865 645f 3022 206a 6178  _Attached_0" jax
+00002920: 3d22 4348 544d 4c22 2074 6162 696e 6465  ="CHTML" tabinde
+00002930: 783d 2230 2220 6374 7874 6d65 6e75 5f63  x="0" ctxtmenu_c
+00002940: 6f75 6e74 6572 3d22 3422 2073 7479 6c65  ounter="4" style
+00002950: 3d22 666f 6e74 2d73 697a 653a 2031 3138  ="font-size: 118
+00002960: 2e39 253b 2070 6f73 6974 696f 6e3a 2072  .9%; position: r
+00002970: 656c 6174 6976 653b 223e 3c6d 6a78 2d6d  elative;"><mjx-m
+00002980: 6174 6820 636c 6173 733d 224d 4a58 2d54  ath class="MJX-T
+00002990: 4558 2220 6172 6961 2d68 6964 6465 6e3d  EX" aria-hidden=
+000029a0: 2274 7275 6522 3e3c 6d6a 782d 6d69 2063  "true"><mjx-mi c
+000029b0: 6c61 7373 3d22 6d6a 782d 6922 3e3c 6d6a  lass="mjx-i"><mj
+000029c0: 782d 6320 636c 6173 733d 226d 6a78 2d63  x-c class="mjx-c
+000029d0: 3144 3434 3520 5445 582d 4922 3e3c 2f6d  1D445 TEX-I"></m
+000029e0: 6a78 2d63 3e3c 2f6d 6a78 2d6d 693e 3c2f  jx-c></mjx-mi></
+000029f0: 6d6a 782d 6d61 7468 3e3c 6d6a 782d 6173  mjx-math><mjx-as
+00002a00: 7369 7374 6976 652d 6d6d 6c20 756e 7365  sistive-mml unse
+00002a10: 6c65 6374 6162 6c65 3d22 6f6e 2220 6469  lectable="on" di
+00002a20: 7370 6c61 793d 2269 6e6c 696e 6522 3e3c  splay="inline"><
+00002a30: 6d61 7468 2078 6d6c 6e73 3d22 6874 7470  math xmlns="http
+00002a40: 3a2f 2f77 7777 2e77 332e 6f72 672f 3139  ://www.w3.org/19
+00002a50: 3938 2f4d 6174 682f 4d61 7468 4d4c 223e  98/Math/MathML">
+00002a60: 3c6d 693e 523c 2f6d 693e 3c2f 6d61 7468  <mi>R</mi></math
+00002a70: 3e3c 2f6d 6a78 2d61 7373 6973 7469 7665  ></mjx-assistive
+00002a80: 2d6d 6d6c 3e3c 2f6d 6a78 2d63 6f6e 7461  -mml></mjx-conta
+00002a90: 696e 6572 3e3c 2f73 7061 6e3e 2074 6f20  iner></span> to 
+00002aa0: 3c73 7472 6f6e 673e 4765 6e6f 6d65 3c2f  <strong>Genome</
+00002ab0: 7374 726f 6e67 3e20 3c73 7061 6e20 636c  strong> <span cl
+00002ac0: 6173 733d 226d 6174 6820 6e6f 7472 616e  ass="math notran
+00002ad0: 736c 6174 6520 6e6f 6869 6768 6c69 6768  slate nohighligh
+00002ae0: 7422 3e3c 6d6a 782d 636f 6e74 6169 6e65  t"><mjx-containe
+00002af0: 7220 636c 6173 733d 224d 6174 684a 6178  r class="MathJax
+00002b00: 2043 7478 744d 656e 755f 4174 7461 6368   CtxtMenu_Attach
+00002b10: 6564 5f30 2220 6a61 783d 2243 4854 4d4c  ed_0" jax="CHTML
+00002b20: 2220 7461 6269 6e64 6578 3d22 3022 2063  " tabindex="0" c
+00002b30: 7478 746d 656e 755f 636f 756e 7465 723d  txtmenu_counter=
+00002b40: 2235 2220 7374 796c 653d 2266 6f6e 742d  "5" style="font-
+00002b50: 7369 7a65 3a20 3131 382e 3925 3b20 706f  size: 118.9%; po
+00002b60: 7369 7469 6f6e 3a20 7265 6c61 7469 7665  sition: relative
+00002b70: 3b22 3e3c 6d6a 782d 6d61 7468 2063 6c61  ;"><mjx-math cla
+00002b80: 7373 3d22 4d4a 582d 5445 5822 2061 7269  ss="MJX-TEX" ari
+00002b90: 612d 6869 6464 656e 3d22 7472 7565 223e  a-hidden="true">
+00002ba0: 3c6d 6a78 2d6d 6920 636c 6173 733d 226d  <mjx-mi class="m
+00002bb0: 6a78 2d69 223e 3c6d 6a78 2d63 2063 6c61  jx-i"><mjx-c cla
+00002bc0: 7373 3d22 6d6a 782d 6331 4434 3437 2054  ss="mjx-c1D447 T
+00002bd0: 4558 2d49 223e 3c2f 6d6a 782d 633e 3c2f  EX-I"></mjx-c></
+00002be0: 6d6a 782d 6d69 3e3c 2f6d 6a78 2d6d 6174  mjx-mi></mjx-mat
+00002bf0: 683e 3c6d 6a78 2d61 7373 6973 7469 7665  h><mjx-assistive
+00002c00: 2d6d 6d6c 2075 6e73 656c 6563 7461 626c  -mml unselectabl
+00002c10: 653d 226f 6e22 2064 6973 706c 6179 3d22  e="on" display="
+00002c20: 696e 6c69 6e65 223e 3c6d 6174 6820 786d  inline"><math xm
+00002c30: 6c6e 733d 2268 7474 703a 2f2f 7777 772e  lns="http://www.
+00002c40: 7733 2e6f 7267 2f31 3939 382f 4d61 7468  w3.org/1998/Math
+00002c50: 2f4d 6174 684d 4c22 3e3c 6d69 3e54 3c2f  /MathML"><mi>T</
+00002c60: 6d69 3e3c 2f6d 6174 683e 3c2f 6d6a 782d  mi></math></mjx-
+00002c70: 6173 7369 7374 6976 652d 6d6d 6c3e 3c2f  assistive-mml></
+00002c80: 6d6a 782d 636f 6e74 6169 6e65 723e 3c2f  mjx-container></
+00002c90: 7370 616e 3e2c 2061 6e64 2067 656e 6572  span>, and gener
+00002ca0: 6174 6520 6120 6e65 7720 616e 6e6f 7461  ate a new annota
+00002cb0: 7469 6f6e 2066 696c 6520 3c73 7472 6f6e  tion file <stron
+00002cc0: 673e 416e 6e6f 7461 7469 6f6e 3c2f 7374  g>Annotation</st
+00002cd0: 726f 6e67 3e20 3c73 7061 6e20 636c 6173  rong> <span clas
+00002ce0: 733d 226d 6174 6820 6e6f 7472 616e 736c  s="math notransl
+00002cf0: 6174 6520 6e6f 6869 6768 6c69 6768 7422  ate nohighlight"
+00002d00: 3e3c 6d6a 782d 636f 6e74 6169 6e65 7220  ><mjx-container 
+00002d10: 636c 6173 733d 224d 6174 684a 6178 2043  class="MathJax C
+00002d20: 7478 744d 656e 755f 4174 7461 6368 6564  txtMenu_Attached
+00002d30: 5f30 2220 6a61 783d 2243 4854 4d4c 2220  _0" jax="CHTML" 
+00002d40: 7461 6269 6e64 6578 3d22 3022 2063 7478  tabindex="0" ctx
+00002d50: 746d 656e 755f 636f 756e 7465 723d 2236  tmenu_counter="6
+00002d60: 2220 7374 796c 653d 2266 6f6e 742d 7369  " style="font-si
+00002d70: 7a65 3a20 3131 382e 3925 3b20 706f 7369  ze: 118.9%; posi
+00002d80: 7469 6f6e 3a20 7265 6c61 7469 7665 3b22  tion: relative;"
+00002d90: 3e3c 6d6a 782d 6d61 7468 2063 6c61 7373  ><mjx-math class
+00002da0: 3d22 4d4a 582d 5445 5822 2061 7269 612d  ="MJX-TEX" aria-
+00002db0: 6869 6464 656e 3d22 7472 7565 223e 3c6d  hidden="true"><m
+00002dc0: 6a78 2d6d 7375 623e 3c6d 6a78 2d6d 6920  jx-msub><mjx-mi 
+00002dd0: 636c 6173 733d 226d 6a78 2d69 223e 3c6d  class="mjx-i"><m
+00002de0: 6a78 2d63 2063 6c61 7373 3d22 6d6a 782d  jx-c class="mjx-
+00002df0: 6331 4434 3437 2054 4558 2d49 223e 3c2f  c1D447 TEX-I"></
+00002e00: 6d6a 782d 633e 3c2f 6d6a 782d 6d69 3e3c  mjx-c></mjx-mi><
+00002e10: 6d6a 782d 7363 7269 7074 2073 7479 6c65  mjx-script style
+00002e20: 3d22 7665 7274 6963 616c 2d61 6c69 676e  ="vertical-align
+00002e30: 3a20 2d30 2e31 3533 656d 3b20 6d61 7267  : -0.153em; marg
+00002e40: 696e 2d6c 6566 743a 202d 302e 3132 656d  in-left: -0.12em
+00002e50: 3b22 3e3c 6d6a 782d 6d69 2063 6c61 7373  ;"><mjx-mi class
+00002e60: 3d22 6d6a 782d 6922 2073 697a 653d 2273  ="mjx-i" size="s
+00002e70: 223e 3c6d 6a78 2d63 2063 6c61 7373 3d22  "><mjx-c class="
+00002e80: 6d6a 782d 6331 4434 3334 2054 4558 2d49  mjx-c1D434 TEX-I
+00002e90: 223e 3c2f 6d6a 782d 633e 3c2f 6d6a 782d  "></mjx-c></mjx-
+00002ea0: 6d69 3e3c 2f6d 6a78 2d73 6372 6970 743e  mi></mjx-script>
+00002eb0: 3c2f 6d6a 782d 6d73 7562 3e3c 2f6d 6a78  </mjx-msub></mjx
+00002ec0: 2d6d 6174 683e 3c6d 6a78 2d61 7373 6973  -math><mjx-assis
+00002ed0: 7469 7665 2d6d 6d6c 2075 6e73 656c 6563  tive-mml unselec
+00002ee0: 7461 626c 653d 226f 6e22 2064 6973 706c  table="on" displ
+00002ef0: 6179 3d22 696e 6c69 6e65 223e 3c6d 6174  ay="inline"><mat
+00002f00: 6820 786d 6c6e 733d 2268 7474 703a 2f2f  h xmlns="http://
+00002f10: 7777 772e 7733 2e6f 7267 2f31 3939 382f  www.w3.org/1998/
+00002f20: 4d61 7468 2f4d 6174 684d 4c22 3e3c 6d73  Math/MathML"><ms
+00002f30: 7562 3e3c 6d69 3e54 3c2f 6d69 3e3c 6d69  ub><mi>T</mi><mi
+00002f40: 3e41 3c2f 6d69 3e3c 2f6d 7375 623e 3c2f  >A</mi></msub></
+00002f50: 6d61 7468 3e3c 2f6d 6a78 2d61 7373 6973  math></mjx-assis
+00002f60: 7469 7665 2d6d 6d6c 3e3c 2f6d 6a78 2d63  tive-mml></mjx-c
+00002f70: 6f6e 7461 696e 6572 3e3c 2f73 7061 6e3e  ontainer></span>
+00002f80: 2e20 4120 7369 6d70 6c65 2069 6c6c 7573  . A simple illus
+00002f90: 7472 6174 696f 6e20 6f66 2074 6865 206c  tration of the l
+00002fa0: 6966 742d 6f76 6572 2070 726f 626c 656d  ift-over problem
+00002fb0: 2069 7320 7368 6f77 6e20 696e 203c 6120   is shown in <a 
+00002fc0: 636c 6173 733d 2272 6566 6572 656e 6365  class="reference
+00002fd0: 2069 6e74 6572 6e61 6c22 2068 7265 663d   internal" href=
+00002fe0: 2223 6c69 6674 6f76 6572 2d69 6c6c 7573  "#liftover-illus
+00002ff0: 7472 6174 696f 6e22 3e3c 7370 616e 2063  tration"><span c
+00003000: 6c61 7373 3d22 7374 6420 7374 642d 6e75  lass="std std-nu
+00003010: 6d72 6566 223e 4669 6775 7265 2031 3c2f  mref">Figure 1</
+00003020: 7370 616e 3e3c 2f61 3e2e 3c2f 703e 0a3c  span></a>.</p>.<
+00003030: 6669 6775 7265 2063 6c61 7373 3d22 616c  figure class="al
+00003040: 6967 6e2d 6365 6e74 6572 2220 6964 3d22  ign-center" id="
+00003050: 6964 3422 3e0a 3c66 6967 6361 7074 696f  id4">.<figcaptio
+00003060: 6e3e 0a3c 7370 616e 2069 643d 226c 6966  n>.<span id="lif
+00003070: 746f 7665 722d 696c 6c75 7374 7261 7469  tover-illustrati
+00003080: 6f6e 223e 3c2f 7370 616e 3e3c 6120 636c  on"></span><a cl
+00003090: 6173 733d 2272 6566 6572 656e 6365 2069  ass="reference i
+000030a0: 6e74 6572 6e61 6c20 696d 6167 652d 7265  nternal image-re
+000030b0: 6665 7265 6e63 6522 2068 7265 663d 2268  ference" href="h
+000030c0: 7474 7073 3a2f 2f73 746f 7261 6765 2e67  ttps://storage.g
+000030d0: 6f6f 676c 6561 7069 732e 636f 6d2f 7374  oogleapis.com/st
+000030e0: 6f72 6167 652e 6b68 6368 616f 2e63 6f6d  orage.khchao.com
+000030f0: 2f66 6967 7572 6573 2f4c 6966 744f 6e2f  /figures/LiftOn/
+00003100: 6c69 6674 6f76 6572 5f69 6c6c 7573 7472  liftover_illustr
+00003110: 6174 696f 6e2e 6769 6622 3e3c 696d 6720  ation.gif"><img 
+00003120: 616c 743d 2267 7261 7068 6963 732f 6c69  alt="graphics/li
+00003130: 6674 6f76 6572 5f69 6c6c 7573 7472 6174  ftover_illustrat
+00003140: 696f 6e2e 6769 6622 2073 7263 3d22 6874  ion.gif" src="ht
+00003150: 7470 733a 2f2f 7374 6f72 6167 652e 676f  tps://storage.go
+00003160: 6f67 6c65 6170 6973 2e63 6f6d 2f73 746f  ogleapis.com/sto
+00003170: 7261 6765 2e6b 6863 6861 6f2e 636f 6d2f  rage.khchao.com/
+00003180: 6669 6775 7265 732f 4c69 6674 4f6e 2f6c  figures/LiftOn/l
+00003190: 6966 746f 7665 725f 696c 6c75 7374 7261  iftover_illustra
+000031a0: 7469 6f6e 2e67 6966 2220 7374 796c 653d  tion.gif" style=
+000031b0: 2277 6964 7468 3a20 3637 322e 3570 783b  "width: 672.5px;
+000031c0: 2068 6569 6768 743a 2032 3730 2e30 7078   height: 270.0px
+000031d0: 3b22 3e3c 2f61 3e0a 3c2f 6669 6763 6170  ;"></a>.</figcap
+000031e0: 7469 6f6e 3e0a 3c2f 6669 6775 7265 3e0a  tion>.</figure>.
+000031f0: 3c64 6976 2063 6c61 7373 3d22 6c69 6e65  <div class="line
+00003200: 2d62 6c6f 636b 223e 0a3c 6469 7620 636c  -block">.<div cl
+00003210: 6173 733d 226c 696e 6522 3e3c 6272 3e3c  ass="line"><br><
+00003220: 2f64 6976 3e0a 3c2f 6469 763e 0a3c 703e  /div>.</div>.<p>
+00003230: 4c69 6674 4f6e 2069 7320 7468 6520 6265  LiftOn is the be
+00003240: 7374 2074 6f6f 6c20 746f 2068 656c 7020  st tool to help 
+00003250: 796f 7520 736f 6c76 6520 7468 6973 2070  you solve this p
+00003260: 726f 626c 656d 2120 4c69 6674 4f6e 2065  roblem! LiftOn e
+00003270: 6d70 6c6f 7973 2061 2074 776f 2d73 7465  mploys a two-ste
+00003280: 7020 3c61 2063 6c61 7373 3d22 7265 6665  p <a class="refe
+00003290: 7265 6e63 6520 696e 7465 726e 616c 2220  rence internal" 
+000032a0: 6872 6566 3d22 6874 7470 733a 2f2f 6363  href="https://cc
+000032b0: 622e 6a68 752e 6564 752f 6c69 6674 6f6e  b.jhu.edu/lifton
+000032c0: 2f63 6f6e 7465 6e74 2f62 6568 696e 645f  /content/behind_
+000032d0: 7363 656e 6573 2e68 746d 6c23 7072 6f74  scenes.html#prot
+000032e0: 6569 6e2d 6d61 7869 6d69 7a61 7469 6f6e  ein-maximization
+000032f0: 2d61 6c67 6f72 6974 686d 223e 3c73 7061  -algorithm"><spa
+00003300: 6e20 636c 6173 733d 2273 7464 2073 7464  n class="std std
+00003310: 2d72 6566 223e 7072 6f74 6569 6e20 6d61  -ref">protein ma
+00003320: 7869 6d69 7a61 7469 6f6e 2061 6c67 6f72  ximization algor
+00003330: 6974 686d 3c2f 7370 616e 3e3c 2f61 3e20  ithm</span></a> 
+00003340: 2850 4d20 616c 676f 7269 7468 6d29 2e3c  (PM algorithm).<
+00003350: 2f70 3e0a 3c6f 6c20 636c 6173 733d 2261  /p>.<ol class="a
+00003360: 7261 6269 6320 7369 6d70 6c65 223e 0a3c  rabic simple">.<
+00003370: 6c69 3e3c 703e 5468 6520 6669 7273 7420  li><p>The first 
+00003380: 6d6f 6475 6c65 2069 7320 7468 6520 3c65  module is the <e
+00003390: 6d3e 6368 6169 6e69 6e67 2061 6c67 6f72  m>chaining algor
+000033a0: 6974 686d 3c2f 656d 3e2e 2049 7420 7374  ithm</em>. It st
+000033b0: 6172 7473 2062 7920 6578 7472 6163 7469  arts by extracti
+000033c0: 6e67 2070 726f 7465 696e 2073 6571 7565  ng protein seque
+000033d0: 6e63 6573 2061 6e6e 6f74 6174 6564 2062  nces annotated b
+000033e0: 7920 4c69 6674 6f66 6620 616e 6420 6d69  y Liftoff and mi
+000033f0: 6e69 7072 6f74 2e20 4c69 6674 4f6e 2074  niprot. LiftOn t
+00003400: 6865 6e20 616c 6967 6e73 2074 6865 7365  hen aligns these
+00003410: 2073 6571 7565 6e63 6573 2074 6f20 6675   sequences to fu
+00003420: 6c6c 2d6c 656e 6774 6820 7265 6665 7265  ll-length refere
+00003430: 6e63 6520 7072 6f74 6569 6e73 2e20 466f  nce proteins. Fo
+00003440: 7220 6561 6368 2067 656e 6520 6c6f 6375  r each gene locu
+00003450: 732c 204c 6966 744f 6e20 636f 6d70 6172  s, LiftOn compar
+00003460: 6573 2065 6163 6820 7365 6374 696f 6e20  es each section 
+00003470: 6f66 2074 6865 2070 726f 7465 696e 2061  of the protein a
+00003480: 6c69 676e 6d65 6e74 7320 6672 6f6d 204c  lignments from L
+00003490: 6966 746f 6666 2061 6e64 206d 696e 6970  iftoff and minip
+000034a0: 726f 742c 2063 6861 696e 696e 6720 746f  rot, chaining to
+000034b0: 6765 7468 6572 2074 6865 2062 6573 7420  gether the best 
+000034c0: 636f 6d62 696e 6174 696f 6e73 2e3c 2f70  combinations.</p
+000034d0: 3e3c 2f6c 693e 0a3c 6c69 3e3c 703e 5468  ></li>.<li><p>Th
+000034e0: 6520 7365 636f 6e64 206d 6f64 756c 6520  e second module 
+000034f0: 6973 2074 6865 203c 656d 3e6f 7065 6e2d  is the <em>open-
+00003500: 7265 6164 696e 6720 6672 616d 6520 7365  reading frame se
+00003510: 6172 6368 2028 4f52 4620 7365 6172 6368  arch (ORF search
+00003520: 2920 616c 676f 7269 7468 6d3c 2f65 6d3e  ) algorithm</em>
+00003530: 2e20 496e 2074 6865 2063 6173 6520 6f66  . In the case of
+00003540: 2074 7275 6e63 6174 6564 2070 726f 7465   truncated prote
+00003550: 696e 2d63 6f64 696e 6720 7472 616e 7363  in-coding transc
+00003560: 7269 7074 732c 2074 6869 7320 616c 676f  ripts, this algo
+00003570: 7269 7468 6d20 6578 616d 696e 6573 2061  rithm examines a
+00003580: 6c74 6572 6e61 7469 7665 2066 7261 6d65  lternative frame
+00003590: 7320 746f 2069 6465 6e74 6966 7920 7468  s to identify th
+000035a0: 6520 4f52 4620 7468 6174 2070 726f 6475  e ORF that produ
+000035b0: 6365 7320 7468 6520 6c6f 6e67 6573 7420  ces the longest 
+000035c0: 6d61 7463 6820 7769 7468 2074 6865 2072  match with the r
+000035d0: 6566 6572 656e 6365 2070 726f 7465 696e  eference protein
+000035e0: 2e3c 2f70 3e3c 2f6c 693e 0a3c 2f6f 6c3e  .</p></li>.</ol>
+000035f0: 0a3c 6469 7620 636c 6173 733d 226c 696e  .<div class="lin
+00003600: 652d 626c 6f63 6b22 3e0a 3c64 6976 2063  e-block">.<div c
+00003610: 6c61 7373 3d22 6c69 6e65 223e 3c62 723e  lass="line"><br>
+00003620: 3c2f 6469 763e 0a3c 2f64 6976 3e0a 3c2f  </div>.</div>.</
+00003630: 7365 6374 696f 6e3e 0a3c 7365 6374 696f  section>.<sectio
+00003640: 6e20 6964 3d22 696e 7075 7473 2d6f 7574  n id="inputs-out
+00003650: 7075 7473 2220 636c 6173 733d 2222 3e0a  puts" class="">.
+00003660: 3c68 323e 496e 7075 7473 2026 616d 703b  <h2>Inputs &amp;
+00003670: 206f 7574 7075 7473 3c61 2063 6c61 7373   outputs<a class
+00003680: 3d22 6865 6164 6572 6c69 6e6b 2220 6872  ="headerlink" hr
+00003690: 6566 3d22 2369 6e70 7574 732d 6f75 7470  ef="#inputs-outp
+000036a0: 7574 7322 2074 6974 6c65 3d22 5065 726d  uts" title="Perm
+000036b0: 616c 696e 6b20 746f 2074 6869 7320 6865  alink to this he
+000036c0: 6164 696e 6722 3e23 3c2f 613e 3c2f 6832  ading">#</a></h2
+000036d0: 3e0a 3c75 6c20 636c 6173 733d 2273 696d  >.<ul class="sim
+000036e0: 706c 6522 3e0a 3c6c 693e 3c64 6c20 636c  ple">.<li><dl cl
+000036f0: 6173 733d 2273 696d 706c 6522 3e0a 3c64  ass="simple">.<d
+00003700: 743e 3c73 7472 6f6e 673e 496e 7075 743c  t><strong>Input<
+00003710: 2f73 7472 6f6e 673e 3a3c 2f64 743e 3c64  /strong>:</dt><d
+00003720: 643e 3c6f 6c20 636c 6173 733d 2261 7261  d><ol class="ara
+00003730: 6269 6320 7369 6d70 6c65 223e 0a3c 6c69  bic simple">.<li
+00003740: 3e3c 703e 7461 7267 6574 203c 7374 726f  ><p>target <stro
+00003750: 6e67 3e47 656e 6f6d 653c 2f73 7472 6f6e  ng>Genome</stron
+00003760: 673e 203c 7370 616e 2063 6c61 7373 3d22  g> <span class="
+00003770: 6d61 7468 206e 6f74 7261 6e73 6c61 7465  math notranslate
+00003780: 206e 6f68 6967 686c 6967 6874 223e 3c6d   nohighlight"><m
+00003790: 6a78 2d63 6f6e 7461 696e 6572 2063 6c61  jx-container cla
+000037a0: 7373 3d22 4d61 7468 4a61 7820 4374 7874  ss="MathJax Ctxt
+000037b0: 4d65 6e75 5f41 7474 6163 6865 645f 3022  Menu_Attached_0"
+000037c0: 206a 6178 3d22 4348 544d 4c22 2074 6162   jax="CHTML" tab
+000037d0: 696e 6465 783d 2230 2220 6374 7874 6d65  index="0" ctxtme
+000037e0: 6e75 5f63 6f75 6e74 6572 3d22 3722 2073  nu_counter="7" s
+000037f0: 7479 6c65 3d22 666f 6e74 2d73 697a 653a  tyle="font-size:
+00003800: 2031 3138 2e39 253b 2070 6f73 6974 696f   118.9%; positio
+00003810: 6e3a 2072 656c 6174 6976 653b 223e 3c6d  n: relative;"><m
+00003820: 6a78 2d6d 6174 6820 636c 6173 733d 224d  jx-math class="M
+00003830: 4a58 2d54 4558 2220 6172 6961 2d68 6964  JX-TEX" aria-hid
+00003840: 6465 6e3d 2274 7275 6522 3e3c 6d6a 782d  den="true"><mjx-
+00003850: 6d69 2063 6c61 7373 3d22 6d6a 782d 6922  mi class="mjx-i"
+00003860: 3e3c 6d6a 782d 6320 636c 6173 733d 226d  ><mjx-c class="m
+00003870: 6a78 2d63 3144 3434 3720 5445 582d 4922  jx-c1D447 TEX-I"
+00003880: 3e3c 2f6d 6a78 2d63 3e3c 2f6d 6a78 2d6d  ></mjx-c></mjx-m
+00003890: 693e 3c2f 6d6a 782d 6d61 7468 3e3c 6d6a  i></mjx-math><mj
+000038a0: 782d 6173 7369 7374 6976 652d 6d6d 6c20  x-assistive-mml 
+000038b0: 756e 7365 6c65 6374 6162 6c65 3d22 6f6e  unselectable="on
+000038c0: 2220 6469 7370 6c61 793d 2269 6e6c 696e  " display="inlin
+000038d0: 6522 3e3c 6d61 7468 2078 6d6c 6e73 3d22  e"><math xmlns="
+000038e0: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
+000038f0: 672f 3139 3938 2f4d 6174 682f 4d61 7468  g/1998/Math/Math
+00003900: 4d4c 223e 3c6d 693e 543c 2f6d 693e 3c2f  ML"><mi>T</mi></
+00003910: 6d61 7468 3e3c 2f6d 6a78 2d61 7373 6973  math></mjx-assis
+00003920: 7469 7665 2d6d 6d6c 3e3c 2f6d 6a78 2d63  tive-mml></mjx-c
+00003930: 6f6e 7461 696e 6572 3e3c 2f73 7061 6e3e  ontainer></span>
+00003940: 2069 6e20 4641 5354 4120 666f 726d 6174   in FASTA format
+00003950: 2e3c 2f70 3e3c 2f6c 693e 0a3c 6c69 3e3c  .</p></li>.<li><
+00003960: 703e 7265 6665 7265 6e63 6520 3c73 7472  p>reference <str
+00003970: 6f6e 673e 4765 6e6f 6d65 3c2f 7374 726f  ong>Genome</stro
+00003980: 6e67 3e20 3c73 7061 6e20 636c 6173 733d  ng> <span class=
+00003990: 226d 6174 6820 6e6f 7472 616e 736c 6174  "math notranslat
+000039a0: 6520 6e6f 6869 6768 6c69 6768 7422 3e3c  e nohighlight"><
+000039b0: 6d6a 782d 636f 6e74 6169 6e65 7220 636c  mjx-container cl
+000039c0: 6173 733d 224d 6174 684a 6178 2043 7478  ass="MathJax Ctx
+000039d0: 744d 656e 755f 4174 7461 6368 6564 5f30  tMenu_Attached_0
+000039e0: 2220 6a61 783d 2243 4854 4d4c 2220 7461  " jax="CHTML" ta
+000039f0: 6269 6e64 6578 3d22 3022 2063 7478 746d  bindex="0" ctxtm
+00003a00: 656e 755f 636f 756e 7465 723d 2238 2220  enu_counter="8" 
+00003a10: 7374 796c 653d 2266 6f6e 742d 7369 7a65  style="font-size
+00003a20: 3a20 3131 382e 3925 3b20 706f 7369 7469  : 118.9%; positi
+00003a30: 6f6e 3a20 7265 6c61 7469 7665 3b22 3e3c  on: relative;"><
+00003a40: 6d6a 782d 6d61 7468 2063 6c61 7373 3d22  mjx-math class="
+00003a50: 4d4a 582d 5445 5822 2061 7269 612d 6869  MJX-TEX" aria-hi
+00003a60: 6464 656e 3d22 7472 7565 223e 3c6d 6a78  dden="true"><mjx
+00003a70: 2d6d 6920 636c 6173 733d 226d 6a78 2d69  -mi class="mjx-i
+00003a80: 223e 3c6d 6a78 2d63 2063 6c61 7373 3d22  "><mjx-c class="
+00003a90: 6d6a 782d 6331 4434 3435 2054 4558 2d49  mjx-c1D445 TEX-I
+00003aa0: 223e 3c2f 6d6a 782d 633e 3c2f 6d6a 782d  "></mjx-c></mjx-
+00003ab0: 6d69 3e3c 2f6d 6a78 2d6d 6174 683e 3c6d  mi></mjx-math><m
+00003ac0: 6a78 2d61 7373 6973 7469 7665 2d6d 6d6c  jx-assistive-mml
+00003ad0: 2075 6e73 656c 6563 7461 626c 653d 226f   unselectable="o
+00003ae0: 6e22 2064 6973 706c 6179 3d22 696e 6c69  n" display="inli
+00003af0: 6e65 223e 3c6d 6174 6820 786d 6c6e 733d  ne"><math xmlns=
+00003b00: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
+00003b10: 7267 2f31 3939 382f 4d61 7468 2f4d 6174  rg/1998/Math/Mat
+00003b20: 684d 4c22 3e3c 6d69 3e52 3c2f 6d69 3e3c  hML"><mi>R</mi><
+00003b30: 2f6d 6174 683e 3c2f 6d6a 782d 6173 7369  /math></mjx-assi
+00003b40: 7374 6976 652d 6d6d 6c3e 3c2f 6d6a 782d  stive-mml></mjx-
+00003b50: 636f 6e74 6169 6e65 723e 3c2f 7370 616e  container></span
+00003b60: 3e20 696e 2046 4153 5441 2066 6f72 6d61  > in FASTA forma
+00003b70: 742e 3c2f 703e 3c2f 6c69 3e0a 3c6c 693e  t.</p></li>.<li>
+00003b80: 3c70 3e72 6566 6572 656e 6365 203c 7374  <p>reference <st
+00003b90: 726f 6e67 3e41 6e6e 6f74 6174 696f 6e3c  rong>Annotation<
+00003ba0: 2f73 7472 6f6e 673e 203c 7370 616e 2063  /strong> <span c
+00003bb0: 6c61 7373 3d22 6d61 7468 206e 6f74 7261  lass="math notra
+00003bc0: 6e73 6c61 7465 206e 6f68 6967 686c 6967  nslate nohighlig
+00003bd0: 6874 223e 3c6d 6a78 2d63 6f6e 7461 696e  ht"><mjx-contain
+00003be0: 6572 2063 6c61 7373 3d22 4d61 7468 4a61  er class="MathJa
+00003bf0: 7820 4374 7874 4d65 6e75 5f41 7474 6163  x CtxtMenu_Attac
+00003c00: 6865 645f 3022 206a 6178 3d22 4348 544d  hed_0" jax="CHTM
+00003c10: 4c22 2074 6162 696e 6465 783d 2230 2220  L" tabindex="0" 
+00003c20: 6374 7874 6d65 6e75 5f63 6f75 6e74 6572  ctxtmenu_counter
+00003c30: 3d22 3922 2073 7479 6c65 3d22 666f 6e74  ="9" style="font
+00003c40: 2d73 697a 653a 2031 3138 2e39 253b 2070  -size: 118.9%; p
+00003c50: 6f73 6974 696f 6e3a 2072 656c 6174 6976  osition: relativ
+00003c60: 653b 223e 3c6d 6a78 2d6d 6174 6820 636c  e;"><mjx-math cl
+00003c70: 6173 733d 224d 4a58 2d54 4558 2220 6172  ass="MJX-TEX" ar
+00003c80: 6961 2d68 6964 6465 6e3d 2274 7275 6522  ia-hidden="true"
+00003c90: 3e3c 6d6a 782d 6d73 7562 3e3c 6d6a 782d  ><mjx-msub><mjx-
+00003ca0: 6d69 2063 6c61 7373 3d22 6d6a 782d 6922  mi class="mjx-i"
+00003cb0: 3e3c 6d6a 782d 6320 636c 6173 733d 226d  ><mjx-c class="m
+00003cc0: 6a78 2d63 3144 3434 3520 5445 582d 4922  jx-c1D445 TEX-I"
+00003cd0: 3e3c 2f6d 6a78 2d63 3e3c 2f6d 6a78 2d6d  ></mjx-c></mjx-m
+00003ce0: 693e 3c6d 6a78 2d73 6372 6970 7420 7374  i><mjx-script st
+00003cf0: 796c 653d 2276 6572 7469 6361 6c2d 616c  yle="vertical-al
+00003d00: 6967 6e3a 202d 302e 3135 3365 6d3b 223e  ign: -0.153em;">
+00003d10: 3c6d 6a78 2d6d 6920 636c 6173 733d 226d  <mjx-mi class="m
+00003d20: 6a78 2d69 2220 7369 7a65 3d22 7322 3e3c  jx-i" size="s"><
+00003d30: 6d6a 782d 6320 636c 6173 733d 226d 6a78  mjx-c class="mjx
+00003d40: 2d63 3144 3433 3420 5445 582d 4922 3e3c  -c1D434 TEX-I"><
+00003d50: 2f6d 6a78 2d63 3e3c 2f6d 6a78 2d6d 693e  /mjx-c></mjx-mi>
+00003d60: 3c2f 6d6a 782d 7363 7269 7074 3e3c 2f6d  </mjx-script></m
+00003d70: 6a78 2d6d 7375 623e 3c2f 6d6a 782d 6d61  jx-msub></mjx-ma
+00003d80: 7468 3e3c 6d6a 782d 6173 7369 7374 6976  th><mjx-assistiv
+00003d90: 652d 6d6d 6c20 756e 7365 6c65 6374 6162  e-mml unselectab
+00003da0: 6c65 3d22 6f6e 2220 6469 7370 6c61 793d  le="on" display=
+00003db0: 2269 6e6c 696e 6522 3e3c 6d61 7468 2078  "inline"><math x
+00003dc0: 6d6c 6e73 3d22 6874 7470 3a2f 2f77 7777  mlns="http://www
+00003dd0: 2e77 332e 6f72 672f 3139 3938 2f4d 6174  .w3.org/1998/Mat
+00003de0: 682f 4d61 7468 4d4c 223e 3c6d 7375 623e  h/MathML"><msub>
+00003df0: 3c6d 693e 523c 2f6d 693e 3c6d 693e 413c  <mi>R</mi><mi>A<
+00003e00: 2f6d 693e 3c2f 6d73 7562 3e3c 2f6d 6174  /mi></msub></mat
+00003e10: 683e 3c2f 6d6a 782d 6173 7369 7374 6976  h></mjx-assistiv
+00003e20: 652d 6d6d 6c3e 3c2f 6d6a 782d 636f 6e74  e-mml></mjx-cont
+00003e30: 6169 6e65 723e 3c2f 7370 616e 3e20 696e  ainer></span> in
+00003e40: 2047 4646 3320 666f 726d 6174 2e3c 2f70   GFF3 format.</p
+00003e50: 3e3c 2f6c 693e 0a3c 2f6f 6c3e 0a3c 2f64  ></li>.</ol>.</d
+00003e60: 643e 0a3c 2f64 6c3e 0a3c 2f6c 693e 0a3c  d>.</dl>.</li>.<
+00003e70: 6c69 3e3c 646c 2063 6c61 7373 3d22 7369  li><dl class="si
+00003e80: 6d70 6c65 223e 0a3c 6474 3e3c 7374 726f  mple">.<dt><stro
+00003e90: 6e67 3e4f 7574 7075 743c 2f73 7472 6f6e  ng>Output</stron
+00003ea0: 673e 3a3c 2f64 743e 3c64 643e 3c6f 6c20  g>:</dt><dd><ol 
+00003eb0: 636c 6173 733d 2261 7261 6269 6320 7369  class="arabic si
+00003ec0: 6d70 6c65 223e 0a3c 6c69 3e3c 703e 4c69  mple">.<li><p>Li
+00003ed0: 6674 4f6e 2061 6e6e 6f74 6174 696f 6e20  ftOn annotation 
+00003ee0: 6669 6c65 2c20 3c73 7472 6f6e 673e 416e  file, <strong>An
+00003ef0: 6e6f 7461 7469 6f6e 3c2f 7374 726f 6e67  notation</strong
+00003f00: 3e20 3c73 7061 6e20 636c 6173 733d 226d  > <span class="m
+00003f10: 6174 6820 6e6f 7472 616e 736c 6174 6520  ath notranslate 
+00003f20: 6e6f 6869 6768 6c69 6768 7422 3e3c 6d6a  nohighlight"><mj
+00003f30: 782d 636f 6e74 6169 6e65 7220 636c 6173  x-container clas
+00003f40: 733d 224d 6174 684a 6178 2043 7478 744d  s="MathJax CtxtM
+00003f50: 656e 755f 4174 7461 6368 6564 5f30 2220  enu_Attached_0" 
+00003f60: 6a61 783d 2243 4854 4d4c 2220 7461 6269  jax="CHTML" tabi
+00003f70: 6e64 6578 3d22 3022 2063 7478 746d 656e  ndex="0" ctxtmen
+00003f80: 755f 636f 756e 7465 723d 2231 3022 2073  u_counter="10" s
+00003f90: 7479 6c65 3d22 666f 6e74 2d73 697a 653a  tyle="font-size:
+00003fa0: 2031 3138 2e39 253b 2070 6f73 6974 696f   118.9%; positio
+00003fb0: 6e3a 2072 656c 6174 6976 653b 223e 3c6d  n: relative;"><m
+00003fc0: 6a78 2d6d 6174 6820 636c 6173 733d 224d  jx-math class="M
+00003fd0: 4a58 2d54 4558 2220 6172 6961 2d68 6964  JX-TEX" aria-hid
+00003fe0: 6465 6e3d 2274 7275 6522 3e3c 6d6a 782d  den="true"><mjx-
+00003ff0: 6d73 7562 3e3c 6d6a 782d 6d69 2063 6c61  msub><mjx-mi cla
+00004000: 7373 3d22 6d6a 782d 6922 3e3c 6d6a 782d  ss="mjx-i"><mjx-
+00004010: 6320 636c 6173 733d 226d 6a78 2d63 3144  c class="mjx-c1D
+00004020: 3434 3720 5445 582d 4922 3e3c 2f6d 6a78  447 TEX-I"></mjx
+00004030: 2d63 3e3c 2f6d 6a78 2d6d 693e 3c6d 6a78  -c></mjx-mi><mjx
+00004040: 2d73 6372 6970 7420 7374 796c 653d 2276  -script style="v
+00004050: 6572 7469 6361 6c2d 616c 6967 6e3a 202d  ertical-align: -
+00004060: 302e 3135 3365 6d3b 206d 6172 6769 6e2d  0.153em; margin-
+00004070: 6c65 6674 3a20 2d30 2e31 3265 6d3b 223e  left: -0.12em;">
+00004080: 3c6d 6a78 2d6d 6920 636c 6173 733d 226d  <mjx-mi class="m
+00004090: 6a78 2d69 2220 7369 7a65 3d22 7322 3e3c  jx-i" size="s"><
+000040a0: 6d6a 782d 6320 636c 6173 733d 226d 6a78  mjx-c class="mjx
+000040b0: 2d63 3144 3433 3420 5445 582d 4922 3e3c  -c1D434 TEX-I"><
+000040c0: 2f6d 6a78 2d63 3e3c 2f6d 6a78 2d6d 693e  /mjx-c></mjx-mi>
+000040d0: 3c2f 6d6a 782d 7363 7269 7074 3e3c 2f6d  </mjx-script></m
+000040e0: 6a78 2d6d 7375 623e 3c2f 6d6a 782d 6d61  jx-msub></mjx-ma
+000040f0: 7468 3e3c 6d6a 782d 6173 7369 7374 6976  th><mjx-assistiv
+00004100: 652d 6d6d 6c20 756e 7365 6c65 6374 6162  e-mml unselectab
+00004110: 6c65 3d22 6f6e 2220 6469 7370 6c61 793d  le="on" display=
+00004120: 2269 6e6c 696e 6522 3e3c 6d61 7468 2078  "inline"><math x
+00004130: 6d6c 6e73 3d22 6874 7470 3a2f 2f77 7777  mlns="http://www
+00004140: 2e77 332e 6f72 672f 3139 3938 2f4d 6174  .w3.org/1998/Mat
+00004150: 682f 4d61 7468 4d4c 223e 3c6d 7375 623e  h/MathML"><msub>
+00004160: 3c6d 693e 543c 2f6d 693e 3c6d 693e 413c  <mi>T</mi><mi>A<
+00004170: 2f6d 693e 3c2f 6d73 7562 3e3c 2f6d 6174  /mi></msub></mat
+00004180: 683e 3c2f 6d6a 782d 6173 7369 7374 6976  h></mjx-assistiv
+00004190: 652d 6d6d 6c3e 3c2f 6d6a 782d 636f 6e74  e-mml></mjx-cont
+000041a0: 6169 6e65 723e 3c2f 7370 616e 3e2c 2069  ainer></span>, i
+000041b0: 6e20 4746 4633 2066 6f72 6d61 742e 3c2f  n GFF3 format.</
+000041c0: 703e 3c2f 6c69 3e0a 3c6c 693e 3c70 3e50  p></li>.<li><p>P
+000041d0: 726f 7465 696e 2073 6571 7565 6e63 6520  rotein sequence 
+000041e0: 6964 656e 7469 7469 6573 2026 616d 703b  identities &amp;
+000041f0: 206d 7574 6174 696f 6e20 7479 7065 733c   mutation types<
+00004200: 2f70 3e3c 2f6c 693e 0a3c 6c69 3e3c 703e  /p></li>.<li><p>
+00004210: 4665 6174 7572 6573 2077 6974 6820 6578  Features with ex
+00004220: 7472 6120 636f 7069 6573 3c2f 703e 3c2f  tra copies</p></
+00004230: 6c69 3e0a 3c6c 693e 3c70 3e55 6e6d 6170  li>.<li><p>Unmap
+00004240: 7065 6420 6665 6174 7572 6573 3c2f 703e  ped features</p>
+00004250: 3c2f 6c69 3e0a 3c2f 6f6c 3e0a 3c2f 6464  </li>.</ol>.</dd
+00004260: 3e0a 3c2f 646c 3e0a 3c2f 6c69 3e0a 3c2f  >.</dl>.</li>.</
+00004270: 756c 3e0a 3c64 6976 2063 6c61 7373 3d22  ul>.<div class="
+00004280: 6c69 6e65 2d62 6c6f 636b 223e 0a3c 6469  line-block">.<di
+00004290: 7620 636c 6173 733d 226c 696e 6522 3e3c  v class="line"><
+000042a0: 6272 3e3c 2f64 6976 3e0a 3c2f 6469 763e  br></div>.</div>
+000042b0: 0a3c 2f73 6563 7469 6f6e 3e0a 3c73 6563  .</section>.<sec
+000042c0: 7469 6f6e 2069 643d 2263 6974 652d 7573  tion id="cite-us
+000042d0: 2220 636c 6173 733d 2222 3e0a 3c68 323e  " class="">.<h2>
+000042e0: 4369 7465 2075 733c 6120 636c 6173 733d  Cite us<a class=
+000042f0: 2268 6561 6465 726c 696e 6b22 2068 7265  "headerlink" hre
+00004300: 663d 2223 6369 7465 2d75 7322 2074 6974  f="#cite-us" tit
+00004310: 6c65 3d22 5065 726d 616c 696e 6b20 746f  le="Permalink to
+00004320: 2074 6869 7320 6865 6164 696e 6722 3e23   this heading">#
+00004330: 3c2f 613e 3c2f 6832 3e0a 3c70 3e4b 7561  </a></h2>.<p>Kua
+00004340: 2d48 616f 2043 6861 6f2c 204a 616b 6f62  -Hao Chao, Jakob
+00004350: 204d 2e20 4865 696e 7a2c 2043 656c 696e   M. Heinz, Celin
+00004360: 6520 486f 682c 2041 6c61 6e20 4d61 6f2c  e Hoh, Alan Mao,
+00004370: 2041 6c61 696e 6120 5368 756d 6174 652c   Alaina Shumate,
+00004380: 204d 6968 6165 6c61 2050 6572 7465 612c   Mihaela Pertea,
+00004390: 2061 6e64 2053 7465 7665 6e20 4c2e 2053   and Steven L. S
+000043a0: 616c 7a62 6572 672e 203c 693e 2243 6f6d  alzberg. <i>"Com
+000043b0: 6269 6e69 6e67 2044 4e41 2061 6e64 2070  bining DNA and p
+000043c0: 726f 7465 696e 2061 6c69 676e 6d65 6e74  rotein alignment
+000043d0: 7320 746f 2069 6d70 726f 7665 2067 656e  s to improve gen
+000043e0: 6f6d 6520 616e 6e6f 7461 7469 6f6e 2077  ome annotation w
+000043f0: 6974 6820 4c69 6674 4f6e 2e22 3c2f 693e  ith LiftOn."</i>
+00004400: 203c 623e 6269 6f52 7869 7620 636f 6d69   <b>bioRxiv comi
+00004410: 6e67 2073 6f6f 6e3c 2f62 3e2e 0a3c 6120  ng soon</b>..<a 
+00004420: 6872 6566 3d22 6874 7470 733a 2f2f 646f  href="https://do
+00004430: 692e 6f72 672f 3130 2e31 3039 332f 6269  i.org/10.1093/bi
+00004440: 6f69 6e66 6f72 6d61 7469 6373 2f62 7461  oinformatics/bta
+00004450: 6131 3031 3622 2074 6172 6765 743d 225f  a1016" target="_
+00004460: 626c 616e 6b22 3e20 3c73 7667 2078 6d6c  blank"> <svg xml
+00004470: 6e73 3d22 6874 7470 3a2f 2f77 7777 2e77  ns="http://www.w
+00004480: 332e 6f72 672f 3230 3030 2f73 7667 2220  3.org/2000/svg" 
+00004490: 6172 6961 2d68 6964 6465 6e3d 2274 7275  aria-hidden="tru
+000044a0: 6522 2078 3d22 3070 7822 2079 3d22 3070  e" x="0px" y="0p
+000044b0: 7822 2076 6965 7742 6f78 3d22 3020 3020  x" viewBox="0 0 
+000044c0: 3130 3020 3130 3022 2077 6964 7468 3d22  100 100" width="
+000044d0: 3135 2220 6865 6967 6874 3d22 3135 2220  15" height="15" 
+000044e0: 636c 6173 733d 2269 636f 6e20 6f75 7462  class="icon outb
+000044f0: 6f75 6e64 223e 3c70 6174 6820 6669 6c6c  ound"><path fill
+00004500: 3d22 6375 7272 656e 7443 6f6c 6f72 2220  ="currentColor" 
+00004510: 643d 224d 3138 2e38 2c38 352e 3168 3536  d="M18.8,85.1h56
+00004520: 6c30 2c30 6332 2e32 2c30 2c34 2d31 2e38  l0,0c2.2,0,4-1.8
+00004530: 2c34 2d34 762d 3332 682d 3876 3238 682d  ,4-4v-32h-8v28h-
+00004540: 3438 762d 3438 6832 3876 2d38 682d 3332  48v-48h28v-8h-32
+00004550: 6c30 2c30 632d 322e 322c 302d 342c 312e  l0,0c-2.2,0-4,1.
+00004560: 382d 342c 3476 3536 4331 342e 382c 3833  8-4,4v56C14.8,83
+00004570: 2e33 2c31 362e 362c 3835 2e31 2c31 382e  .3,16.6,85.1,18.
+00004580: 382c 3835 2e31 7a22 3e3c 2f70 6174 683e  8,85.1z"></path>
+00004590: 203c 706f 6c79 676f 6e20 6669 6c6c 3d22   <polygon fill="
+000045a0: 6375 7272 656e 7443 6f6c 6f72 2220 706f  currentColor" po
+000045b0: 696e 7473 3d22 3435 2e37 2c34 382e 3720  ints="45.7,48.7 
+000045c0: 3531 2e33 2c35 342e 3320 3737 2e32 2c32  51.3,54.3 77.2,2
+000045d0: 382e 3520 3737 2e32 2c33 372e 3220 3835  8.5 77.2,37.2 85
+000045e0: 2e32 2c33 372e 3220 3835 2e32 2c31 342e  .2,37.2 85.2,14.
+000045f0: 3920 3632 2e38 2c31 342e 3920 3632 2e38  9 62.8,14.9 62.8
+00004600: 2c32 322e 3920 3731 2e35 2c32 322e 3922  ,22.9 71.5,22.9"
+00004610: 3e3c 2f70 6f6c 7967 6f6e 3e3c 2f73 7667  ></polygon></svg
+00004620: 3e20 3c2f 613e 203c 2f70 3e0a 0a3c 703e  > </a> </p>..<p>
+00004630: 416c 6169 6e61 2053 6875 6d61 7465 2c20  Alaina Shumate, 
+00004640: 616e 6420 5374 6576 656e 204c 2e20 5361  and Steven L. Sa
+00004650: 6c7a 6265 7267 2e20 3c69 3e22 4c69 6674  lzberg. <i>"Lift
+00004660: 6f66 663a 2061 6363 7572 6174 6520 6d61  off: accurate ma
+00004670: 7070 696e 6720 6f66 2067 656e 6520 616e  pping of gene an
+00004680: 6e6f 7461 7469 6f6e 732e 223c 2f69 3e20  notations."</i> 
+00004690: 3c62 3e42 696f 696e 666f 726d 6174 6963  <b>Bioinformatic
+000046a0: 733c 2f62 3e20 3337 2e31 3220 2832 3032  s</b> 37.12 (202
+000046b0: 3129 3a20 3136 3339 2d31 3634 332e 0a0a  1): 1639-1643...
+000046c0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000046d0: 2f64 6f69 2e6f 7267 2f31 302e 3130 3933  /doi.org/10.1093
+000046e0: 2f62 696f 696e 666f 726d 6174 6963 732f  /bioinformatics/
+000046f0: 6274 6161 3130 3136 2220 7461 7267 6574  btaa1016" target
+00004700: 3d22 5f62 6c61 6e6b 223e 203c 7376 6720  ="_blank"> <svg 
+00004710: 786d 6c6e 733d 2268 7474 703a 2f2f 7777  xmlns="http://ww
+00004720: 772e 7733 2e6f 7267 2f32 3030 302f 7376  w.w3.org/2000/sv
+00004730: 6722 2061 7269 612d 6869 6464 656e 3d22  g" aria-hidden="
+00004740: 7472 7565 2220 783d 2230 7078 2220 793d  true" x="0px" y=
+00004750: 2230 7078 2220 7669 6577 426f 783d 2230  "0px" viewBox="0
+00004760: 2030 2031 3030 2031 3030 2220 7769 6474   0 100 100" widt
+00004770: 683d 2231 3522 2068 6569 6768 743d 2231  h="15" height="1
+00004780: 3522 2063 6c61 7373 3d22 6963 6f6e 206f  5" class="icon o
+00004790: 7574 626f 756e 6422 3e3c 7061 7468 2066  utbound"><path f
+000047a0: 696c 6c3d 2263 7572 7265 6e74 436f 6c6f  ill="currentColo
+000047b0: 7222 2064 3d22 4d31 382e 382c 3835 2e31  r" d="M18.8,85.1
+000047c0: 6835 366c 302c 3063 322e 322c 302c 342d  h56l0,0c2.2,0,4-
+000047d0: 312e 382c 342d 3476 2d33 3268 2d38 7632  1.8,4-4v-32h-8v2
+000047e0: 3868 2d34 3876 2d34 3868 3238 762d 3868  8h-48v-48h28v-8h
+000047f0: 2d33 326c 302c 3063 2d32 2e32 2c30 2d34  -32l0,0c-2.2,0-4
+00004800: 2c31 2e38 2d34 2c34 7635 3643 3134 2e38  ,1.8-4,4v56C14.8
+00004810: 2c38 332e 332c 3136 2e36 2c38 352e 312c  ,83.3,16.6,85.1,
+00004820: 3138 2e38 2c38 352e 317a 223e 3c2f 7061  18.8,85.1z"></pa
+00004830: 7468 3e20 3c70 6f6c 7967 6f6e 2066 696c  th> <polygon fil
+00004840: 6c3d 2263 7572 7265 6e74 436f 6c6f 7222  l="currentColor"
+00004850: 2070 6f69 6e74 733d 2234 352e 372c 3438   points="45.7,48
+00004860: 2e37 2035 312e 332c 3534 2e33 2037 372e  .7 51.3,54.3 77.
+00004870: 322c 3238 2e35 2037 372e 322c 3337 2e32  2,28.5 77.2,37.2
+00004880: 2038 352e 322c 3337 2e32 2038 352e 322c   85.2,37.2 85.2,
+00004890: 3134 2e39 2036 322e 382c 3134 2e39 2036  14.9 62.8,14.9 6
+000048a0: 322e 382c 3232 2e39 2037 312e 352c 3232  2.8,22.9 71.5,22
+000048b0: 2e39 223e 3c2f 706f 6c79 676f 6e3e 3c2f  .9"></polygon></
+000048c0: 7376 673e 0a3c 2f61 3e0a 3c2f 703e 3c64  svg>.</a>.</p><d
+000048d0: 6976 2063 6c61 7373 3d22 6c69 6e65 2d62  iv class="line-b
+000048e0: 6c6f 636b 223e 0a3c 6469 7620 636c 6173  lock">.<div clas
+000048f0: 733d 226c 696e 6522 3e3c 6272 3e3c 2f64  s="line"><br></d
+00004900: 6976 3e0a 3c2f 6469 763e 0a3c 2f73 6563  iv>.</div>.</sec
+00004910: 7469 6f6e 3e0a 3c73 6563 7469 6f6e 2069  tion>.<section i
+00004920: 643d 2275 7365 722d 7375 7070 6f72 7422  d="user-support"
+00004930: 2063 6c61 7373 3d22 223e 0a3c 6832 3e55   class="">.<h2>U
+00004940: 7365 7220 7375 7070 6f72 743c 6120 636c  ser support<a cl
+00004950: 6173 733d 2268 6561 6465 726c 696e 6b22  ass="headerlink"
+00004960: 2068 7265 663d 2223 7573 6572 2d73 7570   href="#user-sup
+00004970: 706f 7274 2220 7469 746c 653d 2250 6572  port" title="Per
+00004980: 6d61 6c69 6e6b 2074 6f20 7468 6973 2068  malink to this h
+00004990: 6561 6469 6e67 223e 233c 2f61 3e3c 2f68  eading">#</a></h
+000049a0: 323e 0a3c 703e 506c 6561 7365 2067 6f20  2>.<p>Please go 
+000049b0: 7468 726f 7567 6820 7468 6520 3c61 2063  through the <a c
+000049c0: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
+000049d0: 696e 7465 726e 616c 2220 6872 6566 3d22  internal" href="
+000049e0: 2374 6162 6c65 2d6f 662d 636f 6e74 656e  #table-of-conten
+000049f0: 7473 223e 3c73 7061 6e20 636c 6173 733d  ts"><span class=
+00004a00: 2273 7464 2073 7464 2d72 6566 223e 646f  "std std-ref">do
+00004a10: 6375 6d65 6e74 6174 696f 6e3c 2f73 7061  cumentation</spa
+00004a20: 6e3e 3c2f 613e 2062 656c 6f77 2066 6972  n></a> below fir
+00004a30: 7374 2e20 4966 2079 6f75 2068 6176 6520  st. If you have 
+00004a40: 7175 6573 7469 6f6e 7320 6162 6f75 7420  questions about 
+00004a50: 7573 696e 6720 7468 6520 7061 636b 6167  using the packag
+00004a60: 652c 2061 2062 7567 2072 6570 6f72 742c  e, a bug report,
+00004a70: 206f 7220 6120 6665 6174 7572 6520 7265   or a feature re
+00004a80: 7175 6573 742c 2070 6c65 6173 6520 7573  quest, please us
+00004a90: 6520 7468 6520 4769 7448 7562 2069 7373  e the GitHub iss
+00004aa0: 7565 2074 7261 636b 6572 2068 6572 653a  ue tracker here:
+00004ab0: 3c2f 703e 0a3c 703e 3c61 2063 6c61 7373  </p>.<p><a class
+00004ac0: 3d22 7265 6665 7265 6e63 6520 6578 7465  ="reference exte
+00004ad0: 726e 616c 2220 6872 6566 3d22 6874 7470  rnal" href="http
+00004ae0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4b  s://github.com/K
+00004af0: 7561 6e68 616f 2d43 6861 6f2f 4c69 6674  uanhao-Chao/Lift
+00004b00: 4f6e 2f69 7373 7565 7322 3e68 7474 7073  On/issues">https
+00004b10: 3a2f 2f67 6974 6875 622e 636f 6d2f 4b75  ://github.com/Ku
+00004b20: 616e 6861 6f2d 4368 616f 2f4c 6966 744f  anhao-Chao/LiftO
+00004b30: 6e2f 6973 7375 6573 3c2f 613e 3c2f 703e  n/issues</a></p>
+00004b40: 0a3c 6469 7620 636c 6173 733d 226c 696e  .<div class="lin
+00004b50: 652d 626c 6f63 6b22 3e0a 3c64 6976 2063  e-block">.<div c
+00004b60: 6c61 7373 3d22 6c69 6e65 223e 3c62 723e  lass="line"><br>
+00004b70: 3c2f 6469 763e 0a3c 2f64 6976 3e0a 3c2f  </div>.</div>.</
+00004b80: 7365 6374 696f 6e3e 0a3c 7365 6374 696f  section>.<sectio
+00004b90: 6e20 6964 3d22 6b65 792d 636f 6e74 7269  n id="key-contri
+00004ba0: 6275 746f 7273 2220 636c 6173 733d 2222  butors" class=""
+00004bb0: 3e0a 3c68 323e 4b65 7920 636f 6e74 7269  >.<h2>Key contri
+00004bc0: 6275 746f 7273 3c61 2063 6c61 7373 3d22  butors<a class="
+00004bd0: 6865 6164 6572 6c69 6e6b 2220 6872 6566  headerlink" href
+00004be0: 3d22 236b 6579 2d63 6f6e 7472 6962 7574  ="#key-contribut
+00004bf0: 6f72 7322 2074 6974 6c65 3d22 5065 726d  ors" title="Perm
+00004c00: 616c 696e 6b20 746f 2074 6869 7320 6865  alink to this he
+00004c10: 6164 696e 6722 3e23 3c2f 613e 3c2f 6832  ading">#</a></h2
+00004c20: 3e0a 3c70 3e4c 6966 744f 6e20 7761 7320  >.<p>LiftOn was 
+00004c30: 6465 7369 676e 6564 2061 6e64 2064 6576  designed and dev
+00004c40: 656c 6f70 6564 2062 7920 3c61 2063 6c61  eloped by <a cla
+00004c50: 7373 3d22 7265 6665 7265 6e63 6520 6578  ss="reference ex
+00004c60: 7465 726e 616c 2220 6872 6566 3d22 6874  ternal" href="ht
+00004c70: 7470 733a 2f2f 6b68 6368 616f 2e63 6f6d  tps://khchao.com
+00004c80: 2f22 3e4b 7561 6e2d 4861 6f20 4368 616f  /">Kuan-Hao Chao
+00004c90: 3c2f 613e 2e20 2054 6869 7320 646f 6375  </a>.  This docu
+00004ca0: 6d65 6e74 6174 696f 6e20 7761 7320 7772  mentation was wr
+00004cb0: 6974 7465 6e20 6279 203c 6120 636c 6173  itten by <a clas
+00004cc0: 733d 2272 6566 6572 656e 6365 2065 7874  s="reference ext
+00004cd0: 6572 6e61 6c22 2068 7265 663d 2268 7474  ernal" href="htt
+00004ce0: 7073 3a2f 2f6b 6863 6861 6f2e 636f 6d2f  ps://khchao.com/
+00004cf0: 223e 4b75 616e 2d48 616f 2043 6861 6f3c  ">Kuan-Hao Chao<
+00004d00: 2f61 3e20 616e 6420 3c61 2063 6c61 7373  /a> and <a class
+00004d10: 3d22 7265 6665 7265 6e63 6520 6578 7465  ="reference exte
+00004d20: 726e 616c 2220 6872 6566 3d22 6874 7470  rnal" href="http
+00004d30: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+00004d40: 6d31 3222 3e41 6c61 6e20 4d61 6e3c 2f61  m12">Alan Man</a
+00004d50: 3e2e 2054 6865 204c 6966 744f 6e20 6c6f  >. The LiftOn lo
+00004d60: 676f 2077 6173 2064 6573 6967 6e65 6420  go was designed 
+00004d70: 6279 203c 6120 636c 6173 733d 2272 6566  by <a class="ref
+00004d80: 6572 656e 6365 2065 7874 6572 6e61 6c22  erence external"
+00004d90: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00004da0: 6974 6875 622e 636f 6d2f 616d 3132 223e  ithub.com/am12">
+00004db0: 416c 616e 204d 616e 3c2f 613e 2e3c 2f70  Alan Man</a>.</p
+00004dc0: 3e0a 3c64 6976 2063 6c61 7373 3d22 6c69  >.<div class="li
+00004dd0: 6e65 2d62 6c6f 636b 223e 0a3c 6469 7620  ne-block">.<div 
+00004de0: 636c 6173 733d 226c 696e 6522 3e3c 6272  class="line"><br
+00004df0: 3e3c 2f64 6976 3e0a 3c2f 6469 763e 0a3c  ></div>.</div>.<
+00004e00: 2f73 6563 7469 6f6e 3e0a 3c73 6563 7469  /section>.<secti
+00004e10: 6f6e 2069 643d 2274 6162 6c65 2d6f 662d  on id="table-of-
+00004e20: 636f 6e74 656e 7473 2220 636c 6173 733d  contents" class=
+00004e30: 2222 3e0a 3c73 7061 6e20 6964 3d22 6964  "">.<span id="id
+00004e40: 3322 3e3c 2f73 7061 6e3e 3c68 323e 5461  3"></span><h2>Ta
+00004e50: 626c 6520 6f66 2063 6f6e 7465 6e74 733c  ble of contents<
+00004e60: 6120 636c 6173 733d 2268 6561 6465 726c  a class="headerl
+00004e70: 696e 6b22 2068 7265 663d 2223 7461 626c  ink" href="#tabl
+00004e80: 652d 6f66 2d63 6f6e 7465 6e74 7322 2074  e-of-contents" t
+00004e90: 6974 6c65 3d22 5065 726d 616c 696e 6b20  itle="Permalink 
+00004ea0: 746f 2074 6869 7320 6865 6164 696e 6722  to this heading"
+00004eb0: 3e23 3c2f 613e 3c2f 6832 3e0a 3c64 6976  >#</a></h2>.<div
+00004ec0: 2063 6c61 7373 3d22 746f 6374 7265 652d   class="toctree-
+00004ed0: 7772 6170 7065 7220 636f 6d70 6f75 6e64  wrapper compound
+00004ee0: 223e 0a3c 756c 3e0a 3c6c 6920 636c 6173  ">.<ul>.<li clas
+00004ef0: 733d 2274 6f63 7472 6565 2d6c 3122 3e3c  s="toctree-l1"><
+00004f00: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
+00004f10: 6365 2069 6e74 6572 6e61 6c22 2068 7265  ce internal" hre
+00004f20: 663d 2268 7474 7073 3a2f 2f63 6362 2e6a  f="https://ccb.j
+00004f30: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
+00004f40: 6e74 656e 742f 696e 7374 616c 6c61 7469  ntent/installati
+00004f50: 6f6e 2e68 746d 6c22 3e49 6e73 7461 6c6c  on.html">Install
+00004f60: 6174 696f 6e3c 2f61 3e3c 756c 3e0a 3c6c  ation</a><ul>.<l
+00004f70: 6920 636c 6173 733d 2274 6f63 7472 6565  i class="toctree
+00004f80: 2d6c 3222 3e3c 6120 636c 6173 733d 2272  -l2"><a class="r
+00004f90: 6566 6572 656e 6365 2069 6e74 6572 6e61  eference interna
+00004fa0: 6c22 2068 7265 663d 2268 7474 7073 3a2f  l" href="https:/
+00004fb0: 2f63 6362 2e6a 6875 2e65 6475 2f6c 6966  /ccb.jhu.edu/lif
+00004fc0: 746f 6e2f 636f 6e74 656e 742f 696e 7374  ton/content/inst
+00004fd0: 616c 6c61 7469 6f6e 2e68 746d 6c23 7379  allation.html#sy
+00004fe0: 7374 656d 2d72 6571 7569 7265 6d65 6e74  stem-requirement
+00004ff0: 7322 3e53 7973 7465 6d20 7265 7175 6972  s">System requir
+00005000: 656d 656e 7473 3c2f 613e 3c2f 6c69 3e0a  ements</a></li>.
+00005010: 3c6c 6920 636c 6173 733d 2274 6f63 7472  <li class="toctr
+00005020: 6565 2d6c 3222 3e3c 6120 636c 6173 733d  ee-l2"><a class=
+00005030: 2272 6566 6572 656e 6365 2069 6e74 6572  "reference inter
+00005040: 6e61 6c22 2068 7265 663d 2268 7474 7073  nal" href="https
+00005050: 3a2f 2f63 6362 2e6a 6875 2e65 6475 2f6c  ://ccb.jhu.edu/l
+00005060: 6966 746f 6e2f 636f 6e74 656e 742f 696e  ifton/content/in
+00005070: 7374 616c 6c61 7469 6f6e 2e68 746d 6c23  stallation.html#
+00005080: 696e 7374 616c 6c2d 7468 726f 7567 682d  install-through-
+00005090: 7069 7022 3e49 6e73 7461 6c6c 2074 6872  pip">Install thr
+000050a0: 6f75 6768 2070 6970 3c2f 613e 3c2f 6c69  ough pip</a></li
+000050b0: 3e0a 3c6c 6920 636c 6173 733d 2274 6f63  >.<li class="toc
+000050c0: 7472 6565 2d6c 3222 3e3c 6120 636c 6173  tree-l2"><a clas
+000050d0: 733d 2272 6566 6572 656e 6365 2069 6e74  s="reference int
+000050e0: 6572 6e61 6c22 2068 7265 663d 2268 7474  ernal" href="htt
+000050f0: 7073 3a2f 2f63 6362 2e6a 6875 2e65 6475  ps://ccb.jhu.edu
+00005100: 2f6c 6966 746f 6e2f 636f 6e74 656e 742f  /lifton/content/
+00005110: 696e 7374 616c 6c61 7469 6f6e 2e68 746d  installation.htm
+00005120: 6c23 696e 7374 616c 6c2d 7468 726f 7567  l#install-throug
+00005130: 682d 636f 6e64 6122 3e49 6e73 7461 6c6c  h-conda">Install
+00005140: 2074 6872 6f75 6768 2063 6f6e 6461 3c2f   through conda</
+00005150: 613e 3c2f 6c69 3e0a 3c6c 6920 636c 6173  a></li>.<li clas
+00005160: 733d 2274 6f63 7472 6565 2d6c 3222 3e3c  s="toctree-l2"><
+00005170: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
+00005180: 6365 2069 6e74 6572 6e61 6c22 2068 7265  ce internal" hre
+00005190: 663d 2268 7474 7073 3a2f 2f63 6362 2e6a  f="https://ccb.j
+000051a0: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
+000051b0: 6e74 656e 742f 696e 7374 616c 6c61 7469  ntent/installati
+000051c0: 6f6e 2e68 746d 6c23 696e 7374 616c 6c2d  on.html#install-
+000051d0: 6672 6f6d 2d73 6f75 7263 6522 3e49 6e73  from-source">Ins
+000051e0: 7461 6c6c 2066 726f 6d20 736f 7572 6365  tall from source
+000051f0: 3c2f 613e 3c2f 6c69 3e0a 3c6c 6920 636c  </a></li>.<li cl
+00005200: 6173 733d 2274 6f63 7472 6565 2d6c 3222  ass="toctree-l2"
+00005210: 3e3c 6120 636c 6173 733d 2272 6566 6572  ><a class="refer
+00005220: 656e 6365 2069 6e74 6572 6e61 6c22 2068  ence internal" h
+00005230: 7265 663d 2268 7474 7073 3a2f 2f63 6362  ref="https://ccb
+00005240: 2e6a 6875 2e65 6475 2f6c 6966 746f 6e2f  .jhu.edu/lifton/
+00005250: 636f 6e74 656e 742f 696e 7374 616c 6c61  content/installa
+00005260: 7469 6f6e 2e68 746d 6c23 6368 6563 6b2d  tion.html#check-
+00005270: 6c69 6674 6f6e 2d69 6e73 7461 6c6c 6174  lifton-installat
+00005280: 696f 6e22 3e43 6865 636b 204c 6966 744f  ion">Check LiftO
+00005290: 6e20 696e 7374 616c 6c61 7469 6f6e 3c2f  n installation</
+000052a0: 613e 3c2f 6c69 3e0a 3c6c 6920 636c 6173  a></li>.<li clas
+000052b0: 733d 2274 6f63 7472 6565 2d6c 3222 3e3c  s="toctree-l2"><
+000052c0: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
+000052d0: 6365 2069 6e74 6572 6e61 6c22 2068 7265  ce internal" hre
+000052e0: 663d 2268 7474 7073 3a2f 2f63 6362 2e6a  f="https://ccb.j
+000052f0: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
+00005300: 6e74 656e 742f 696e 7374 616c 6c61 7469  ntent/installati
+00005310: 6f6e 2e68 746d 6c23 6e6f 772d 796f 752d  on.html#now-you-
+00005320: 6172 652d 7265 6164 792d 746f 2d67 6f22  are-ready-to-go"
+00005330: 3e4e 6f77 2c20 796f 7520 6172 6520 7265  >Now, you are re
+00005340: 6164 7920 746f 2067 6f20 213c 2f61 3e3c  ady to go !</a><
+00005350: 2f6c 693e 0a3c 2f75 6c3e 0a3c 2f6c 693e  /li>.</ul>.</li>
+00005360: 0a3c 6c69 2063 6c61 7373 3d22 746f 6374  .<li class="toct
+00005370: 7265 652d 6c31 223e 3c61 2063 6c61 7373  ree-l1"><a class
+00005380: 3d22 7265 6665 7265 6e63 6520 696e 7465  ="reference inte
+00005390: 726e 616c 2220 6872 6566 3d22 6874 7470  rnal" href="http
+000053a0: 733a 2f2f 6363 622e 6a68 752e 6564 752f  s://ccb.jhu.edu/
+000053b0: 6c69 6674 6f6e 2f63 6f6e 7465 6e74 2f71  lifton/content/q
+000053c0: 7569 636b 7374 6172 742e 6874 6d6c 223e  uickstart.html">
+000053d0: 5175 6963 6b20 5374 6172 7420 4775 6964  Quick Start Guid
+000053e0: 653c 2f61 3e3c 756c 3e0a 3c6c 6920 636c  e</a><ul>.<li cl
+000053f0: 6173 733d 2274 6f63 7472 6565 2d6c 3222  ass="toctree-l2"
+00005400: 3e3c 6120 636c 6173 733d 2272 6566 6572  ><a class="refer
+00005410: 656e 6365 2069 6e74 6572 6e61 6c22 2068  ence internal" h
+00005420: 7265 663d 2268 7474 7073 3a2f 2f63 6362  ref="https://ccb
+00005430: 2e6a 6875 2e65 6475 2f6c 6966 746f 6e2f  .jhu.edu/lifton/
+00005440: 636f 6e74 656e 742f 7175 6963 6b73 7461  content/quicksta
+00005450: 7274 2e68 746d 6c23 7375 7065 722d 7175  rt.html#super-qu
+00005460: 6963 6b2d 7374 6172 742d 6f6e 652d 6c69  ick-start-one-li
+00005470: 6e65 7222 3e53 7570 6572 2d51 7569 636b  ner">Super-Quick
+00005480: 2053 7461 7274 2028 6f6e 652d 6c69 6e65   Start (one-line
+00005490: 7229 3c2f 613e 3c2f 6c69 3e0a 3c6c 6920  r)</a></li>.<li 
+000054a0: 636c 6173 733d 2274 6f63 7472 6565 2d6c  class="toctree-l
+000054b0: 3222 3e3c 6120 636c 6173 733d 2272 6566  2"><a class="ref
+000054c0: 6572 656e 6365 2069 6e74 6572 6e61 6c22  erence internal"
+000054d0: 2068 7265 663d 2268 7474 7073 3a2f 2f63   href="https://c
+000054e0: 6362 2e6a 6875 2e65 6475 2f6c 6966 746f  cb.jhu.edu/lifto
+000054f0: 6e2f 636f 6e74 656e 742f 7175 6963 6b73  n/content/quicks
+00005500: 7461 7274 2e68 746d 6c23 696e 7465 7270  tart.html#interp
+00005510: 7265 7469 6e67 2d6f 7574 7075 7473 2d6f  reting-outputs-o
+00005520: 6e2d 7468 652d 7465 726d 696e 616c 223e  n-the-terminal">
+00005530: 496e 7465 7270 7265 7469 6e67 206f 7574  Interpreting out
+00005540: 7075 7473 206f 6e20 7468 6520 7465 726d  puts on the term
+00005550: 696e 616c 3c2f 613e 3c2f 6c69 3e0a 3c6c  inal</a></li>.<l
+00005560: 6920 636c 6173 733d 2274 6f63 7472 6565  i class="toctree
+00005570: 2d6c 3222 3e3c 6120 636c 6173 733d 2272  -l2"><a class="r
+00005580: 6566 6572 656e 6365 2069 6e74 6572 6e61  eference interna
+00005590: 6c22 2068 7265 663d 2268 7474 7073 3a2f  l" href="https:/
+000055a0: 2f63 6362 2e6a 6875 2e65 6475 2f6c 6966  /ccb.jhu.edu/lif
+000055b0: 746f 6e2f 636f 6e74 656e 742f 7175 6963  ton/content/quic
+000055c0: 6b73 7461 7274 2e68 746d 6c23 7472 792d  kstart.html#try-
+000055d0: 6c69 6674 6f6e 2d6f 6e2d 676f 6f67 6c65  lifton-on-google
+000055e0: 2d63 6f6c 6162 223e 5472 7920 4c69 6674  -colab">Try Lift
+000055f0: 4f6e 206f 6e20 476f 6f67 6c65 2043 6f6c  On on Google Col
+00005600: 6162 3c2f 613e 3c2f 6c69 3e0a 3c2f 756c  ab</a></li>.</ul
+00005610: 3e0a 3c2f 6c69 3e0a 3c2f 756c 3e0a 3c2f  >.</li>.</ul>.</
+00005620: 6469 763e 0a3c 6469 7620 636c 6173 733d  div>.<div class=
+00005630: 2274 6f63 7472 6565 2d77 7261 7070 6572  "toctree-wrapper
+00005640: 2063 6f6d 706f 756e 6422 3e0a 3c70 2063   compound">.<p c
+00005650: 6c61 7373 3d22 6361 7074 696f 6e22 2072  lass="caption" r
+00005660: 6f6c 653d 2268 6561 6469 6e67 223e 3c73  ole="heading"><s
+00005670: 7061 6e20 636c 6173 733d 2263 6170 7469  pan class="capti
+00005680: 6f6e 2d74 6578 7422 3e45 7861 6d70 6c65  on-text">Example
+00005690: 733c 2f73 7061 6e3e 3c2f 703e 0a3c 756c  s</span></p>.<ul
+000056a0: 3e0a 3c6c 6920 636c 6173 733d 2274 6f63  >.<li class="toc
+000056b0: 7472 6565 2d6c 3122 3e3c 6120 636c 6173  tree-l1"><a clas
+000056c0: 733d 2272 6566 6572 656e 6365 2069 6e74  s="reference int
+000056d0: 6572 6e61 6c22 2068 7265 663d 2268 7474  ernal" href="htt
+000056e0: 7073 3a2f 2f63 6362 2e6a 6875 2e65 6475  ps://ccb.jhu.edu
+000056f0: 2f6c 6966 746f 6e2f 636f 6e74 656e 742f  /lifton/content/
+00005700: 7361 6d65 5f73 7065 6369 6573 5f6c 6966  same_species_lif
+00005710: 746f 7665 722f 696e 6465 782e 6874 6d6c  tover/index.html
+00005720: 223e 5361 6d65 2073 7065 6369 6573 206c  ">Same species l
+00005730: 6966 742d 6f76 6572 3c2f 613e 3c2f 6c69  ift-over</a></li
+00005740: 3e0a 3c6c 6920 636c 6173 733d 2274 6f63  >.<li class="toc
+00005750: 7472 6565 2d6c 3122 3e3c 6120 636c 6173  tree-l1"><a clas
+00005760: 733d 2272 6566 6572 656e 6365 2069 6e74  s="reference int
+00005770: 6572 6e61 6c22 2068 7265 663d 2268 7474  ernal" href="htt
+00005780: 7073 3a2f 2f63 6362 2e6a 6875 2e65 6475  ps://ccb.jhu.edu
+00005790: 2f6c 6966 746f 6e2f 636f 6e74 656e 742f  /lifton/content/
+000057a0: 636c 6f73 655f 7370 6563 6965 735f 6c69  close_species_li
+000057b0: 6674 6f76 6572 2f69 6e64 6578 2e68 746d  ftover/index.htm
+000057c0: 6c22 3e43 6c6f 7365 6c79 2072 656c 6174  l">Closely relat
+000057d0: 6564 2073 7065 6369 6573 206c 6966 742d  ed species lift-
+000057e0: 6f76 6572 3c2f 613e 3c2f 6c69 3e0a 3c6c  over</a></li>.<l
+000057f0: 6920 636c 6173 733d 2274 6f63 7472 6565  i class="toctree
+00005800: 2d6c 3122 3e3c 6120 636c 6173 733d 2272  -l1"><a class="r
+00005810: 6566 6572 656e 6365 2069 6e74 6572 6e61  eference interna
+00005820: 6c22 2068 7265 663d 2268 7474 7073 3a2f  l" href="https:/
+00005830: 2f63 6362 2e6a 6875 2e65 6475 2f6c 6966  /ccb.jhu.edu/lif
+00005840: 746f 6e2f 636f 6e74 656e 742f 6469 7374  ton/content/dist
+00005850: 616e 745f 7370 6563 6965 735f 6c69 6674  ant_species_lift
+00005860: 6f76 6572 2f69 6e64 6578 2e68 746d 6c22  over/index.html"
+00005870: 3e44 6973 7461 6e74 6c79 2072 656c 6174  >Distantly relat
+00005880: 6564 2073 7065 6369 6573 206c 6966 742d  ed species lift-
+00005890: 6f76 6572 3c2f 613e 3c2f 6c69 3e0a 3c2f  over</a></li>.</
+000058a0: 756c 3e0a 3c2f 6469 763e 0a3c 6469 7620  ul>.</div>.<div 
+000058b0: 636c 6173 733d 2274 6f63 7472 6565 2d77  class="toctree-w
+000058c0: 7261 7070 6572 2063 6f6d 706f 756e 6422  rapper compound"
+000058d0: 3e0a 3c70 2063 6c61 7373 3d22 6361 7074  >.<p class="capt
+000058e0: 696f 6e22 2072 6f6c 653d 2268 6561 6469  ion" role="headi
+000058f0: 6e67 223e 3c73 7061 6e20 636c 6173 733d  ng"><span class=
+00005900: 2263 6170 7469 6f6e 2d74 6578 7422 3e49  "caption-text">I
+00005910: 6e66 6f3c 2f73 7061 6e3e 3c2f 703e 0a3c  nfo</span></p>.<
+00005920: 756c 3e0a 3c6c 6920 636c 6173 733d 2274  ul>.<li class="t
+00005930: 6f63 7472 6565 2d6c 3122 3e3c 6120 636c  octree-l1"><a cl
+00005940: 6173 733d 2272 6566 6572 656e 6365 2069  ass="reference i
+00005950: 6e74 6572 6e61 6c22 2068 7265 663d 2268  nternal" href="h
+00005960: 7474 7073 3a2f 2f63 6362 2e6a 6875 2e65  ttps://ccb.jhu.e
+00005970: 6475 2f6c 6966 746f 6e2f 636f 6e74 656e  du/lifton/conten
+00005980: 742f 6f75 7470 7574 5f65 7870 6c61 6e61  t/output_explana
+00005990: 7469 6f6e 2e68 746d 6c22 3e4f 7574 7075  tion.html">Outpu
+000059a0: 7420 6669 6c65 733c 2f61 3e3c 756c 3e0a  t files</a><ul>.
+000059b0: 3c6c 6920 636c 6173 733d 2274 6f63 7472  <li class="toctr
+000059c0: 6565 2d6c 3222 3e3c 6120 636c 6173 733d  ee-l2"><a class=
+000059d0: 2272 6566 6572 656e 6365 2069 6e74 6572  "reference inter
+000059e0: 6e61 6c22 2068 7265 663d 2268 7474 7073  nal" href="https
+000059f0: 3a2f 2f63 6362 2e6a 6875 2e65 6475 2f6c  ://ccb.jhu.edu/l
+00005a00: 6966 746f 6e2f 636f 6e74 656e 742f 6f75  ifton/content/ou
+00005a10: 7470 7574 5f65 7870 6c61 6e61 7469 6f6e  tput_explanation
+00005a20: 2e68 746d 6c23 6c69 6674 6f6e 2d67 6666  .html#lifton-gff
+00005a30: 3322 3e6c 6966 746f 6e2e 6766 6633 3c2f  3">lifton.gff3</
+00005a40: 613e 3c2f 6c69 3e0a 3c6c 6920 636c 6173  a></li>.<li clas
+00005a50: 733d 2274 6f63 7472 6565 2d6c 3222 3e3c  s="toctree-l2"><
+00005a60: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
+00005a70: 6365 2069 6e74 6572 6e61 6c22 2068 7265  ce internal" hre
+00005a80: 663d 2268 7474 7073 3a2f 2f63 6362 2e6a  f="https://ccb.j
+00005a90: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
+00005aa0: 6e74 656e 742f 6f75 7470 7574 5f65 7870  ntent/output_exp
+00005ab0: 6c61 6e61 7469 6f6e 2e68 746d 6c23 6c69  lanation.html#li
+00005ac0: 6674 6f6e 2d6f 7574 7075 7422 3e6c 6966  fton-output">lif
+00005ad0: 746f 6e5f 6f75 7470 7574 2f3c 2f61 3e3c  ton_output/</a><
+00005ae0: 2f6c 693e 0a3c 2f75 6c3e 0a3c 2f6c 693e  /li>.</ul>.</li>
+00005af0: 0a3c 6c69 2063 6c61 7373 3d22 746f 6374  .<li class="toct
+00005b00: 7265 652d 6c31 223e 3c61 2063 6c61 7373  ree-l1"><a class
+00005b10: 3d22 7265 6665 7265 6e63 6520 696e 7465  ="reference inte
+00005b20: 726e 616c 2220 6872 6566 3d22 6874 7470  rnal" href="http
+00005b30: 733a 2f2f 6363 622e 6a68 752e 6564 752f  s://ccb.jhu.edu/
+00005b40: 6c69 6674 6f6e 2f63 6f6e 7465 6e74 2f66  lifton/content/f
+00005b50: 6561 7475 7265 5f63 6f75 6e74 696e 672e  eature_counting.
+00005b60: 6874 6d6c 223e 4765 6e65 202f 2054 7261  html">Gene / Tra
+00005b70: 6e73 6372 6970 7420 636f 756e 7469 6e67  nscript counting
+00005b80: 3c2f 613e 3c75 6c3e 0a3c 6c69 2063 6c61  </a><ul>.<li cla
+00005b90: 7373 3d22 746f 6374 7265 652d 6c32 223e  ss="toctree-l2">
+00005ba0: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
+00005bb0: 6e63 6520 696e 7465 726e 616c 2220 6872  nce internal" hr
+00005bc0: 6566 3d22 6874 7470 733a 2f2f 6363 622e  ef="https://ccb.
+00005bd0: 6a68 752e 6564 752f 6c69 6674 6f6e 2f63  jhu.edu/lifton/c
+00005be0: 6f6e 7465 6e74 2f66 6561 7475 7265 5f63  ontent/feature_c
+00005bf0: 6f75 6e74 696e 672e 6874 6d6c 2367 656e  ounting.html#gen
+00005c00: 652d 636f 756e 7469 6e67 223e 4765 6e65  e-counting">Gene
+00005c10: 2063 6f75 6e74 696e 673c 2f61 3e3c 2f6c   counting</a></l
+00005c20: 693e 0a3c 6c69 2063 6c61 7373 3d22 746f  i>.<li class="to
+00005c30: 6374 7265 652d 6c32 223e 3c61 2063 6c61  ctree-l2"><a cla
+00005c40: 7373 3d22 7265 6665 7265 6e63 6520 696e  ss="reference in
+00005c50: 7465 726e 616c 2220 6872 6566 3d22 6874  ternal" href="ht
+00005c60: 7470 733a 2f2f 6363 622e 6a68 752e 6564  tps://ccb.jhu.ed
+00005c70: 752f 6c69 6674 6f6e 2f63 6f6e 7465 6e74  u/lifton/content
+00005c80: 2f66 6561 7475 7265 5f63 6f75 6e74 696e  /feature_countin
+00005c90: 672e 6874 6d6c 2374 7261 6e73 6372 6970  g.html#transcrip
+00005ca0: 742d 636f 756e 7469 6e67 223e 5472 616e  t-counting">Tran
+00005cb0: 7363 7269 7074 2063 6f75 6e74 696e 673c  script counting<
+00005cc0: 2f61 3e3c 2f6c 693e 0a3c 2f75 6c3e 0a3c  /a></li>.</ul>.<
+00005cd0: 2f6c 693e 0a3c 6c69 2063 6c61 7373 3d22  /li>.<li class="
+00005ce0: 746f 6374 7265 652d 6c31 223e 3c61 2063  toctree-l1"><a c
+00005cf0: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
+00005d00: 696e 7465 726e 616c 2220 6872 6566 3d22  internal" href="
+00005d10: 6874 7470 733a 2f2f 6363 622e 6a68 752e  https://ccb.jhu.
+00005d20: 6564 752f 6c69 6674 6f6e 2f63 6f6e 7465  edu/lifton/conte
+00005d30: 6e74 2f65 7661 6c75 6174 696f 6e5f 6d65  nt/evaluation_me
+00005d40: 7472 6963 732e 6874 6d6c 223e 4576 616c  trics.html">Eval
+00005d50: 7561 7469 6f6e 206d 6574 7269 6373 202d  uation metrics -
+00005d60: 2073 6571 7565 6e63 6520 6964 656e 7469   sequence identi
+00005d70: 7479 3c2f 613e 3c75 6c3e 0a3c 6c69 2063  ty</a><ul>.<li c
+00005d80: 6c61 7373 3d22 746f 6374 7265 652d 6c32  lass="toctree-l2
+00005d90: 223e 3c61 2063 6c61 7373 3d22 7265 6665  "><a class="refe
+00005da0: 7265 6e63 6520 696e 7465 726e 616c 2220  rence internal" 
+00005db0: 6872 6566 3d22 6874 7470 733a 2f2f 6363  href="https://cc
+00005dc0: 622e 6a68 752e 6564 752f 6c69 6674 6f6e  b.jhu.edu/lifton
+00005dd0: 2f63 6f6e 7465 6e74 2f65 7661 6c75 6174  /content/evaluat
+00005de0: 696f 6e5f 6d65 7472 6963 732e 6874 6d6c  ion_metrics.html
+00005df0: 2364 6e61 2d73 6571 7565 6e63 652d 6964  #dna-sequence-id
+00005e00: 656e 7469 7479 2d73 636f 7265 223e 444e  entity-score">DN
+00005e10: 4120 7365 7175 656e 6365 2069 6465 6e74  A sequence ident
+00005e20: 6974 7920 7363 6f72 653c 2f61 3e3c 2f6c  ity score</a></l
+00005e30: 693e 0a3c 6c69 2063 6c61 7373 3d22 746f  i>.<li class="to
+00005e40: 6374 7265 652d 6c32 223e 3c61 2063 6c61  ctree-l2"><a cla
+00005e50: 7373 3d22 7265 6665 7265 6e63 6520 696e  ss="reference in
+00005e60: 7465 726e 616c 2220 6872 6566 3d22 6874  ternal" href="ht
+00005e70: 7470 733a 2f2f 6363 622e 6a68 752e 6564  tps://ccb.jhu.ed
+00005e80: 752f 6c69 6674 6f6e 2f63 6f6e 7465 6e74  u/lifton/content
+00005e90: 2f65 7661 6c75 6174 696f 6e5f 6d65 7472  /evaluation_metr
+00005ea0: 6963 732e 6874 6d6c 2370 726f 7465 696e  ics.html#protein
+00005eb0: 2d73 6571 7565 6e63 652d 6964 656e 7469  -sequence-identi
+00005ec0: 7479 2d73 636f 7265 223e 5072 6f74 6569  ty-score">Protei
+00005ed0: 6e20 7365 7175 656e 6365 2069 6465 6e74  n sequence ident
+00005ee0: 6974 7920 7363 6f72 653c 2f61 3e3c 2f6c  ity score</a></l
+00005ef0: 693e 0a3c 2f75 6c3e 0a3c 2f6c 693e 0a3c  i>.</ul>.</li>.<
+00005f00: 6c69 2063 6c61 7373 3d22 746f 6374 7265  li class="toctre
+00005f10: 652d 6c31 223e 3c61 2063 6c61 7373 3d22  e-l1"><a class="
+00005f20: 7265 6665 7265 6e63 6520 696e 7465 726e  reference intern
+00005f30: 616c 2220 6872 6566 3d22 6874 7470 733a  al" href="https:
+00005f40: 2f2f 6363 622e 6a68 752e 6564 752f 6c69  //ccb.jhu.edu/li
+00005f50: 6674 6f6e 2f63 6f6e 7465 6e74 2f62 6568  fton/content/beh
+00005f60: 696e 645f 7363 656e 6573 2e68 746d 6c22  ind_scenes.html"
+00005f70: 3e42 6568 696e 6420 7468 6520 7363 656e  >Behind the scen
+00005f80: 6573 3c2f 613e 3c75 6c3e 0a3c 6c69 2063  es</a><ul>.<li c
+00005f90: 6c61 7373 3d22 746f 6374 7265 652d 6c32  lass="toctree-l2
+00005fa0: 223e 3c61 2063 6c61 7373 3d22 7265 6665  "><a class="refe
+00005fb0: 7265 6e63 6520 696e 7465 726e 616c 2220  rence internal" 
+00005fc0: 6872 6566 3d22 6874 7470 733a 2f2f 6363  href="https://cc
+00005fd0: 622e 6a68 752e 6564 752f 6c69 6674 6f6e  b.jhu.edu/lifton
+00005fe0: 2f63 6f6e 7465 6e74 2f62 6568 696e 645f  /content/behind_
+00005ff0: 7363 656e 6573 2e68 746d 6c23 6465 6369  scenes.html#deci
+00006000: 6469 6e67 2d63 6872 6f6d 6f73 6f6d 6573  ding-chromosomes
+00006010: 2d61 6e64 2d66 6561 7475 7265 732d 666f  -and-features-fo
+00006020: 722d 616e 6e6f 7461 7469 6f6e 2d6c 6966  r-annotation-lif
+00006030: 742d 6f76 6572 223e 4465 6369 6469 6e67  t-over">Deciding
+00006040: 2063 6872 6f6d 6f73 6f6d 6573 2061 6e64   chromosomes and
+00006050: 2066 6561 7475 7265 7320 666f 7220 616e   features for an
+00006060: 6e6f 7461 7469 6f6e 206c 6966 742d 6f76  notation lift-ov
+00006070: 6572 3c2f 613e 3c2f 6c69 3e0a 3c6c 6920  er</a></li>.<li 
+00006080: 636c 6173 733d 2274 6f63 7472 6565 2d6c  class="toctree-l
+00006090: 3222 3e3c 6120 636c 6173 733d 2272 6566  2"><a class="ref
+000060a0: 6572 656e 6365 2069 6e74 6572 6e61 6c22  erence internal"
+000060b0: 2068 7265 663d 2268 7474 7073 3a2f 2f63   href="https://c
+000060c0: 6362 2e6a 6875 2e65 6475 2f6c 6966 746f  cb.jhu.edu/lifto
+000060d0: 6e2f 636f 6e74 656e 742f 6265 6869 6e64  n/content/behind
+000060e0: 5f73 6365 6e65 732e 6874 6d6c 236d 6174  _scenes.html#mat
+000060f0: 6368 696e 672d 6d69 6e69 7072 6f74 2d6c  ching-miniprot-l
+00006100: 6966 746f 6666 2d67 656e 6f6d 652d 616e  iftoff-genome-an
+00006110: 6e6f 7461 7469 6f6e 223e 4d61 7463 6869  notation">Matchi
+00006120: 6e67 206d 696e 6970 726f 7420 2661 6d70  ng miniprot &amp
+00006130: 3b20 4c69 6674 6f66 6620 6765 6e6f 6d65  ; Liftoff genome
+00006140: 2061 6e6e 6f74 6174 696f 6e3c 2f61 3e3c   annotation</a><
+00006150: 2f6c 693e 0a3c 6c69 2063 6c61 7373 3d22  /li>.<li class="
+00006160: 746f 6374 7265 652d 6c32 223e 3c61 2063  toctree-l2"><a c
+00006170: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
+00006180: 696e 7465 726e 616c 2220 6872 6566 3d22  internal" href="
+00006190: 6874 7470 733a 2f2f 6363 622e 6a68 752e  https://ccb.jhu.
+000061a0: 6564 752f 6c69 6674 6f6e 2f63 6f6e 7465  edu/lifton/conte
+000061b0: 6e74 2f62 6568 696e 645f 7363 656e 6573  nt/behind_scenes
+000061c0: 2e68 746d 6c23 7072 6f74 6569 6e2d 6d61  .html#protein-ma
+000061d0: 7869 6d69 7a61 7469 6f6e 2d61 6c67 6f72  ximization-algor
+000061e0: 6974 686d 223e 5072 6f74 6569 6e2d 6d61  ithm">Protein-ma
+000061f0: 7869 6d69 7a61 7469 6f6e 2061 6c67 6f72  ximization algor
+00006200: 6974 686d 3c2f 613e 3c2f 6c69 3e0a 3c6c  ithm</a></li>.<l
+00006210: 6920 636c 6173 733d 2274 6f63 7472 6565  i class="toctree
+00006220: 2d6c 3222 3e3c 6120 636c 6173 733d 2272  -l2"><a class="r
+00006230: 6566 6572 656e 6365 2069 6e74 6572 6e61  eference interna
+00006240: 6c22 2068 7265 663d 2268 7474 7073 3a2f  l" href="https:/
+00006250: 2f63 6362 2e6a 6875 2e65 6475 2f6c 6966  /ccb.jhu.edu/lif
+00006260: 746f 6e2f 636f 6e74 656e 742f 6265 6869  ton/content/behi
+00006270: 6e64 5f73 6365 6e65 732e 6874 6d6c 236d  nd_scenes.html#m
+00006280: 7574 6174 696f 6e2d 7265 706f 7274 223e  utation-report">
+00006290: 4d75 7461 7469 6f6e 2072 6570 6f72 743c  Mutation report<
+000062a0: 2f61 3e3c 2f6c 693e 0a3c 6c69 2063 6c61  /a></li>.<li cla
+000062b0: 7373 3d22 746f 6374 7265 652d 6c32 223e  ss="toctree-l2">
+000062c0: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
+000062d0: 6e63 6520 696e 7465 726e 616c 2220 6872  nce internal" hr
+000062e0: 6566 3d22 6874 7470 733a 2f2f 6363 622e  ef="https://ccb.
+000062f0: 6a68 752e 6564 752f 6c69 6674 6f6e 2f63  jhu.edu/lifton/c
+00006300: 6f6e 7465 6e74 2f62 6568 696e 645f 7363  ontent/behind_sc
+00006310: 656e 6573 2e68 746d 6c23 7265 6665 7265  enes.html#refere
+00006320: 6e63 6522 3e52 6566 6572 656e 6365 3c2f  nce">Reference</
+00006330: 613e 3c2f 6c69 3e0a 3c2f 756c 3e0a 3c2f  a></li>.</ul>.</
+00006340: 6c69 3e0a 3c6c 6920 636c 6173 733d 2274  li>.<li class="t
+00006350: 6f63 7472 6565 2d6c 3122 3e3c 6120 636c  octree-l1"><a cl
+00006360: 6173 733d 2272 6566 6572 656e 6365 2069  ass="reference i
+00006370: 6e74 6572 6e61 6c22 2068 7265 663d 2268  nternal" href="h
+00006380: 7474 7073 3a2f 2f63 6362 2e6a 6875 2e65  ttps://ccb.jhu.e
+00006390: 6475 2f6c 6966 746f 6e2f 636f 6e74 656e  du/lifton/conten
+000063a0: 742f 686f 775f 746f 5f70 6167 652e 6874  t/how_to_page.ht
+000063b0: 6d6c 223e 4641 5120 2e2e 2e3c 2f61 3e3c  ml">FAQ ...</a><
+000063c0: 2f6c 693e 0a3c 6c69 2063 6c61 7373 3d22  /li>.<li class="
+000063d0: 746f 6374 7265 652d 6c31 223e 3c61 2063  toctree-l1"><a c
+000063e0: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
+000063f0: 696e 7465 726e 616c 2220 6872 6566 3d22  internal" href="
+00006400: 6874 7470 733a 2f2f 6363 622e 6a68 752e  https://ccb.jhu.
+00006410: 6564 752f 6c69 6674 6f6e 2f63 6f6e 7465  edu/lifton/conte
+00006420: 6e74 2f66 756e 6374 696f 6e5f 6d61 6e75  nt/function_manu
+00006430: 616c 2e68 746d 6c22 3e55 7365 7220 4d61  al.html">User Ma
+00006440: 6e75 616c 3c2f 613e 3c75 6c3e 0a3c 6c69  nual</a><ul>.<li
+00006450: 2063 6c61 7373 3d22 746f 6374 7265 652d   class="toctree-
+00006460: 6c32 223e 3c61 2063 6c61 7373 3d22 7265  l2"><a class="re
+00006470: 6665 7265 6e63 6520 696e 7465 726e 616c  ference internal
+00006480: 2220 6872 6566 3d22 6874 7470 733a 2f2f  " href="https://
+00006490: 6363 622e 6a68 752e 6564 752f 6c69 6674  ccb.jhu.edu/lift
+000064a0: 6f6e 2f63 6f6e 7465 6e74 2f66 756e 6374  on/content/funct
+000064b0: 696f 6e5f 6d61 6e75 616c 2e68 746d 6c23  ion_manual.html#
+000064c0: 6c69 6674 6f6e 223e 4c69 6674 4f6e 3c2f  lifton">LiftOn</
+000064d0: 613e 3c2f 6c69 3e0a 3c2f 756c 3e0a 3c2f  a></li>.</ul>.</
+000064e0: 6c69 3e0a 3c6c 6920 636c 6173 733d 2274  li>.<li class="t
+000064f0: 6f63 7472 6565 2d6c 3122 3e3c 6120 636c  octree-l1"><a cl
+00006500: 6173 733d 2272 6566 6572 656e 6365 2069  ass="reference i
+00006510: 6e74 6572 6e61 6c22 2068 7265 663d 2268  nternal" href="h
+00006520: 7474 7073 3a2f 2f63 6362 2e6a 6875 2e65  ttps://ccb.jhu.e
+00006530: 6475 2f6c 6966 746f 6e2f 636f 6e74 656e  du/lifton/conten
+00006540: 742f 6368 616e 6765 6c6f 672e 6874 6d6c  t/changelog.html
+00006550: 223e 4368 616e 6765 6c6f 673c 2f61 3e3c  ">Changelog</a><
+00006560: 756c 3e0a 3c6c 6920 636c 6173 733d 2274  ul>.<li class="t
+00006570: 6f63 7472 6565 2d6c 3222 3e3c 6120 636c  octree-l2"><a cl
+00006580: 6173 733d 2272 6566 6572 656e 6365 2069  ass="reference i
+00006590: 6e74 6572 6e61 6c22 2068 7265 663d 2268  nternal" href="h
+000065a0: 7474 7073 3a2f 2f63 6362 2e6a 6875 2e65  ttps://ccb.jhu.e
+000065b0: 6475 2f6c 6966 746f 6e2f 636f 6e74 656e  du/lifton/conten
+000065c0: 742f 6368 616e 6765 6c6f 672e 6874 6d6c  t/changelog.html
+000065d0: 2376 312d 302d 3022 3e76 312e 302e 303c  #v1-0-0">v1.0.0<
+000065e0: 2f61 3e3c 2f6c 693e 0a3c 2f75 6c3e 0a3c  /a></li>.</ul>.<
+000065f0: 2f6c 693e 0a3c 6c69 2063 6c61 7373 3d22  /li>.<li class="
+00006600: 746f 6374 7265 652d 6c31 223e 3c61 2063  toctree-l1"><a c
+00006610: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
+00006620: 696e 7465 726e 616c 2220 6872 6566 3d22  internal" href="
+00006630: 6874 7470 733a 2f2f 6363 622e 6a68 752e  https://ccb.jhu.
+00006640: 6564 752f 6c69 6674 6f6e 2f63 6f6e 7465  edu/lifton/conte
+00006650: 6e74 2f6c 6963 656e 7365 2e68 746d 6c22  nt/license.html"
+00006660: 3e4c 6963 656e 7365 3c2f 613e 3c2f 6c69  >License</a></li
+00006670: 3e0a 3c6c 6920 636c 6173 733d 2274 6f63  >.<li class="toc
+00006680: 7472 6565 2d6c 3122 3e3c 6120 636c 6173  tree-l1"><a clas
+00006690: 733d 2272 6566 6572 656e 6365 2069 6e74  s="reference int
+000066a0: 6572 6e61 6c22 2068 7265 663d 2268 7474  ernal" href="htt
+000066b0: 7073 3a2f 2f63 6362 2e6a 6875 2e65 6475  ps://ccb.jhu.edu
+000066c0: 2f6c 6966 746f 6e2f 636f 6e74 656e 742f  /lifton/content/
+000066d0: 636f 6e74 6163 742e 6874 6d6c 223e 436f  contact.html">Co
+000066e0: 6e74 6163 743c 2f61 3e3c 2f6c 693e 0a3c  ntact</a></li>.<
+000066f0: 2f75 6c3e 0a3c 2f64 6976 3e0a 3c64 6976  /ul>.</div>.<div
+00006700: 2063 6c61 7373 3d22 6c69 6e65 2d62 6c6f   class="line-blo
+00006710: 636b 223e 0a3c 6469 7620 636c 6173 733d  ck">.<div class=
+00006720: 226c 696e 6522 3e3c 6272 3e3c 2f64 6976  "line"><br></div
+00006730: 3e0a 3c2f 6469 763e 0a3c 2f73 6563 7469  >.</div>.</secti
+00006740: 6f6e 3e0a 3c73 6563 7469 6f6e 2069 643d  on>.<section id=
+00006750: 226c 6966 746f 6e2d 732d 6c69 6d69 7461  "lifton-s-limita
+00006760: 7469 6f6e 223e 0a3c 6832 3e4c 6966 744f  tion">.<h2>LiftO
+00006770: 6e27 7320 6c69 6d69 7461 7469 6f6e 3c61  n's limitation<a
+00006780: 2063 6c61 7373 3d22 6865 6164 6572 6c69   class="headerli
+00006790: 6e6b 2220 6872 6566 3d22 236c 6966 746f  nk" href="#lifto
+000067a0: 6e2d 732d 6c69 6d69 7461 7469 6f6e 2220  n-s-limitation" 
+000067b0: 7469 746c 653d 2250 6572 6d61 6c69 6e6b  title="Permalink
+000067c0: 2074 6f20 7468 6973 2068 6561 6469 6e67   to this heading
+000067d0: 223e 233c 2f61 3e3c 2f68 323e 0a3c 703e  ">#</a></h2>.<p>
+000067e0: 4c69 6674 4f6e 2773 203c 656d 3e63 6861  LiftOn's <em>cha
+000067f0: 696e 696e 6720 616c 676f 7269 7468 6d3c  ining algorithm<
+00006800: 2f65 6d3e 2063 7572 7265 6e74 6c79 206f  /em> currently o
+00006810: 6e6c 7920 7574 696c 697a 6573 206d 696e  nly utilizes min
+00006820: 6970 726f 7420 616c 6967 6e6d 656e 7420  iprot alignment 
+00006830: 7265 7375 6c74 7320 746f 2066 6978 2074  results to fix t
+00006840: 6865 204c 6966 746f 6666 2061 6e6e 6f74  he Liftoff annot
+00006850: 6174 696f 6e2e 2048 6f77 6576 6572 2c20  ation. However, 
+00006860: 6974 2063 616e 2062 6520 6578 7465 6e64  it can be extend
+00006870: 6564 2074 6f20 6368 6169 6e20 746f 6765  ed to chain toge
+00006880: 7468 6572 206d 756c 7469 706c 6520 444e  ther multiple DN
+00006890: 412d 2061 6e64 2070 726f 7465 696e 2d62  A- and protein-b
+000068a0: 6173 6564 2061 6e6e 6f74 6174 696f 6e20  ased annotation 
+000068b0: 6669 6c65 7320 6f72 2061 6173 656d 626c  files or aasembl
+000068c0: 6564 2052 4e41 2d53 6571 2074 7261 6e73  ed RNA-Seq trans
+000068d0: 6372 6970 7473 2e3c 2f70 3e0a 3c70 3e44  cripts.</p>.<p>D
+000068e0: 4e41 2d20 616e 6420 7072 6f74 6569 6e2d  NA- and protein-
+000068f0: 6261 7365 6420 6d65 7468 6f64 7320 7374  based methods st
+00006900: 696c 6c20 6861 7665 2073 6f6d 6520 6c69  ill have some li
+00006910: 6d69 7461 7469 6f6e 732e 2057 6520 6172  mitations. We ar
+00006920: 6520 6465 7665 6c6f 7069 6e67 2061 206d  e developing a m
+00006930: 6f64 756c 6520 746f 206d 6572 6765 2074  odule to merge t
+00006940: 6865 204c 6966 744f 6e20 616e 6e6f 7461  he LiftOn annota
+00006950: 7469 6f6e 2077 6974 6820 7468 6520 7265  tion with the re
+00006960: 6c65 6173 6564 2063 7572 6174 6564 2061  leased curated a
+00006970: 6e6e 6f74 6174 696f 6e73 2074 6f20 6765  nnotations to ge
+00006980: 6e65 7261 7465 2062 6574 7465 7220 616e  nerate better an
+00006990: 6e6f 7461 7469 6f6e 732e 3c2f 703e 0a3c  notations.</p>.<
+000069a0: 703e 5468 6520 4c69 6674 4f6e 203c 656d  p>The LiftOn <em
+000069b0: 3e63 6861 696e 696e 6720 616c 676f 7269  >chaining algori
+000069c0: 7468 6d3c 2f65 6d3e 206e 6f77 2064 6f65  thm</em> now doe
+000069d0: 7320 6e6f 7420 7375 7070 6f72 7420 6d75  s not support mu
+000069e0: 6c74 692d 7468 7265 6164 696e 672e 2054  lti-threading. T
+000069f0: 6869 7320 6675 6e63 7469 6f6e 616c 6974  his functionalit
+00006a00: 7920 7374 616e 6473 2061 7320 6f75 7220  y stands as our 
+00006a10: 6e65 7874 2074 6172 6765 7465 6420 6665  next targeted fe
+00006a20: 6174 7572 6520 6f6e 2074 6865 2064 6576  ature on the dev
+00006a30: 656c 6f70 6d65 6e74 2068 6f72 697a 6f6e  elopment horizon
+00006a40: 213c 2f70 3e0a 3c64 6976 2063 6c61 7373  !</p>.<div class
+00006a50: 3d22 6c69 6e65 2d62 6c6f 636b 223e 0a3c  ="line-block">.<
+00006a60: 6469 7620 636c 6173 733d 226c 696e 6522  div class="line"
+00006a70: 3e3c 6272 3e3c 2f64 6976 3e0a 3c2f 6469  ><br></div>.</di
+00006a80: 763e 0a3c 2f73 6563 7469 6f6e 3e0a 3c2f  v>.</section>.</
+00006a90: 7365 6374 696f 6e3e 0a0a 2020 2020 2020  section>..      
+00006aa0: 2020 0a0a 2323 203c 6120 6e61 6d65 3d22    ..## <a name="
+00006ab0: 6369 7461 7469 6f6e 223e 3c2f 613e 4369  citation"></a>Ci
+00006ac0: 7461 7469 6f6e 3c61 2063 6c61 7373 3d22  tation<a class="
+00006ad0: 6865 6164 6572 6c69 6e6b 2220 6872 6566  headerlink" href
+00006ae0: 3d22 2363 6974 6174 696f 6e22 2074 6974  ="#citation" tit
+00006af0: 6c65 3d22 5065 726d 616c 696e 6b20 746f  le="Permalink to
+00006b00: 2074 6869 7320 6865 6164 696e 6722 3e23   this heading">#
+00006b10: 3c2f 613e 0a0a 0a4b 7561 6e2d 4861 6f20  </a>...Kuan-Hao 
+00006b20: 4368 616f 2a2c 204d 6968 6165 6c61 2050  Chao*, Mihaela P
+00006b30: 6572 7465 612c 2053 7465 7665 6e20 4c20  ertea, Steven L 
+00006b40: 5361 6c7a 6265 7267 2a2c 2022 4c69 6674  Salzberg*, "Lift
+00006b50: 4f6e 3a20 6120 746f 6f6c 2074 6f20 696d  On: a tool to im
+00006b60: 7072 6f76 6520 616e 6e6f 7461 7469 6f6e  prove annotation
+00006b70: 7320 666f 7220 7072 6f74 6569 6e2d 636f  s for protein-co
+00006b80: 6469 6e67 2067 656e 6573 2064 7572 696e  ding genes durin
+00006b90: 6720 7468 6520 6c69 6674 2d6f 7665 7220  g the lift-over 
+00006ba0: 7072 6f63 6573 732e 222c 203c 693e 6269  process.", <i>bi
+00006bb0: 6f52 7869 763c 2f69 3e20 3c62 3e32 3032  oRxiv</i> <b>202
+00006bc0: 332e 3037 2e32 372e 3535 3037 3534 3c2f  3.07.27.550754</
+00006bd0: 623e 2c20 646f 693a 205b 6874 7470 733a  b>, doi: [https:
+00006be0: 2f2f 646f 692e 6f72 672f 3130 2e31 3130  //doi.org/10.110
+00006bf0: 312f 3230 3233 2e30 372e 3237 2e35 3530  1/2023.07.27.550
+00006c00: 3735 345d 2868 7474 7073 3a2f 2f64 6f69  754](https://doi
+00006c10: 2e6f 7267 2f31 302e 3131 3031 2f32 3032  .org/10.1101/202
+00006c20: 332e 3037 2e32 372e 3535 3037 3534 292c  3.07.27.550754),
+00006c30: 2032 3032 330a 0a3c 6272 3e0a 3c62 723e   2023..<br>.<br>
+00006c40: 0a3c 6272 3e0a 0a3c 696d 6720 616c 743d  .<br>..<img alt=
+00006c50: 224d 7920 4c6f 676f 2220 636c 6173 733d  "My Logo" class=
+00006c60: 226c 6f67 6f20 6865 6164 6572 2d69 6d61  "logo header-ima
+00006c70: 6765 206f 6e6c 792d 6c69 6768 7420 616c  ge only-light al
+00006c80: 6967 6e2d 6365 6e74 6572 2220 7372 633d  ign-center" src=
+00006c90: 2268 7474 7073 3a2f 2f73 746f 7261 6765  "https://storage
+00006ca0: 2e67 6f6f 676c 6561 7069 732e 636f 6d2f  .googleapis.com/
+00006cb0: 7374 6f72 6167 652e 6b68 6368 616f 2e63  storage.khchao.c
+00006cc0: 6f6d 2f66 6967 7572 6573 2f6a 6875 2d6c  om/figures/jhu-l
+00006cd0: 6f67 6f2d 6461 726b 2e70 6e67 223e 0a    ogo-dark.png">.
```

### Comparing `lifton-0.0.3/README.md` & `lifton-1.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,1399 +1,1722 @@
 00000000: 3c69 6d67 2061 6c74 3d22 4d79 204c 6f67  <img alt="My Log
 00000010: 6f22 2063 6c61 7373 3d22 6c6f 676f 2068  o" class="logo h
 00000020: 6561 6465 722d 696d 6167 6520 6f6e 6c79  eader-image only
 00000030: 2d6c 6967 6874 2061 6c69 676e 2d63 656e  -light align-cen
-00000040: 7465 7222 2073 7263 3d22 6772 6170 6869  ter" src="graphi
-00000050: 6373 2f4c 6966 744f 6e5f 636f 6c6f 722e  cs/LiftOn_color.
-00000060: 706e 6722 2073 7479 6c65 3d22 7769 6474  png" style="widt
-00000070: 683a 3930 2522 3e0a 0a3c 6469 7620 636c  h:90%">..<div cl
-00000080: 6173 733d 2263 6f6e 7465 6e74 223e 0a0a  ass="content">..
-00000090: 3c64 6976 2063 6c61 7373 3d22 6c69 6e65  <div class="line
-000000a0: 223e 3c62 723e 3c2f 6469 763e 0a3c 2f64  "><br></div>.</d
-000000b0: 6976 3e0a 3c73 6563 7469 6f6e 2069 643d  iv>.<section id=
-000000c0: 226c 6966 746f 6e2d 732d 7475 746f 7269  "lifton-s-tutori
-000000d0: 616c 223e 0a3c 656d 6265 643e 0a3c 6120  al">.<embed>.<a 
-000000e0: 636c 6173 733d 2272 6566 6572 656e 6365  class="reference
-000000f0: 2065 7874 6572 6e61 6c20 696d 6167 652d   external image-
-00000100: 7265 6665 7265 6e63 6522 2068 7265 663d  reference" href=
-00000110: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-00000120: 656c 6473 2e69 6f2f 6261 6467 652f 4c69  elds.io/badge/Li
-00000130: 6365 6e73 652d 4750 4c76 332d 7965 6c6c  cense-GPLv3-yell
-00000140: 6f77 2e73 7667 223e 3c69 6d67 2061 6c74  ow.svg"><img alt
-00000150: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00000160: 6965 6c64 732e 696f 2f62 6164 6765 2f4c  ields.io/badge/L
-00000170: 6963 656e 7365 2d47 504c 7633 2d79 656c  icense-GPLv3-yel
-00000180: 6c6f 772e 7376 6722 2073 7263 3d22 6874  low.svg" src="ht
-00000190: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-000001a0: 732e 696f 2f62 6164 6765 2f4c 6963 656e  s.io/badge/Licen
-000001b0: 7365 2d47 504c 7633 2d79 656c 6c6f 772e  se-GPLv3-yellow.
-000001c0: 7376 6722 3e3c 2f61 3e0a 3c61 2063 6c61  svg"></a>.<a cla
-000001d0: 7373 3d22 7265 6665 7265 6e63 6520 6578  ss="reference ex
-000001e0: 7465 726e 616c 2069 6d61 6765 2d72 6566  ternal image-ref
-000001f0: 6572 656e 6365 2220 6872 6566 3d22 6874  erence" href="ht
-00000200: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000210: 732e 696f 2f62 6164 6765 2f76 6572 7369  s.io/badge/versi
-00000220: 6f6e 2d76 2e30 2e30 2e31 2d62 6c75 6522  on-v.0.0.1-blue"
-00000230: 3e3c 696d 6720 616c 743d 2268 7474 7073  ><img alt="https
-00000240: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000250: 6f2f 6261 6467 652f 7665 7273 696f 6e2d  o/badge/version-
-00000260: 762e 302e 302e 312d 626c 7565 2220 7372  v.0.0.1-blue" sr
-00000270: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-00000280: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00000290: 7665 7273 696f 6e2d 762e 302e 302e 312d  version-v.0.0.1-
-000002a0: 626c 7565 223e 3c2f 613e 0a3c 6120 636c  blue"></a>.<a cl
-000002b0: 6173 733d 2272 6566 6572 656e 6365 2065  ass="reference e
-000002c0: 7874 6572 6e61 6c20 696d 6167 652d 7265  xternal image-re
-000002d0: 6665 7265 6e63 6522 2068 7265 663d 2268  ference" href="h
-000002e0: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
-000002f0: 2f70 726f 6a65 6374 2f6c 6966 746f 6e22  /project/lifton"
-00000300: 3e3c 696d 6720 616c 743d 2268 7474 7073  ><img alt="https
-00000310: 3a2f 2f73 7461 7469 632e 7065 7079 2e74  ://static.pepy.t
-00000320: 6563 682f 7065 7273 6f6e 616c 697a 6564  ech/personalized
-00000330: 2d62 6164 6765 2f6c 6966 746f 6e3f 7065  -badge/lifton?pe
-00000340: 7269 6f64 3d74 6f74 616c 2661 6d70 3b75  riod=total&amp;u
-00000350: 6e69 7473 3d61 6262 7265 7669 6174 696f  nits=abbreviatio
-00000360: 6e26 616d 703b 6c65 6674 5f63 6f6c 6f72  n&amp;left_color
-00000370: 3d67 7265 7926 616d 703b 7269 6768 745f  =grey&amp;right_
-00000380: 636f 6c6f 723d 626c 7565 2661 6d70 3b6c  color=blue&amp;l
-00000390: 6566 745f 7465 7874 3d50 7950 6925 3230  eft_text=PyPi%20
-000003a0: 646f 776e 6c6f 6164 7322 2073 7263 3d22  downloads" src="
-000003b0: 6874 7470 733a 2f2f 7374 6174 6963 2e70  https://static.p
-000003c0: 6570 792e 7465 6368 2f70 6572 736f 6e61  epy.tech/persona
-000003d0: 6c69 7a65 642d 6261 6467 652f 6c69 6674  lized-badge/lift
-000003e0: 6f6e 3f70 6572 696f 643d 746f 7461 6c26  on?period=total&
-000003f0: 616d 703b 756e 6974 733d 6162 6272 6576  amp;units=abbrev
-00000400: 6961 7469 6f6e 2661 6d70 3b6c 6566 745f  iation&amp;left_
-00000410: 636f 6c6f 723d 6772 6579 2661 6d70 3b72  color=grey&amp;r
-00000420: 6967 6874 5f63 6f6c 6f72 3d62 6c75 6526  ight_color=blue&
-00000430: 616d 703b 6c65 6674 5f74 6578 743d 5079  amp;left_text=Py
-00000440: 5069 2532 3064 6f77 6e6c 6f61 6473 223e  Pi%20downloads">
-00000450: 3c2f 613e 0a3c 6120 636c 6173 733d 2272  </a>.<a class="r
-00000460: 6566 6572 656e 6365 2065 7874 6572 6e61  eference externa
-00000470: 6c20 696d 6167 652d 7265 6665 7265 6e63  l image-referenc
-00000480: 6522 2068 7265 663d 2268 7474 7073 3a2f  e" href="https:/
-00000490: 2f67 6974 6875 622e 636f 6d2f 4b75 616e  /github.com/Kuan
-000004a0: 6861 6f2d 4368 616f 2f6c 6966 746f 6e2f  hao-Chao/lifton/
-000004b0: 7265 6c65 6173 6573 223e 3c69 6d67 2061  releases"><img a
-000004c0: 6c74 3d22 6874 7470 733a 2f2f 696d 672e  lt="https://img.
-000004d0: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-000004e0: 622f 646f 776e 6c6f 6164 732f 4b75 616e  b/downloads/Kuan
-000004f0: 6861 6f2d 4368 616f 2f6c 6966 746f 6e2f  hao-Chao/lifton/
-00000500: 746f 7461 6c2e 7376 673f 7374 796c 653d  total.svg?style=
-00000510: 736f 6369 616c 2661 6d70 3b6c 6f67 6f3d  social&amp;logo=
-00000520: 6769 7468 7562 2661 6d70 3b6c 6162 656c  github&amp;label
-00000530: 3d44 6f77 6e6c 6f61 6422 2073 7263 3d22  =Download" src="
-00000540: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000550: 6c64 732e 696f 2f67 6974 6875 622f 646f  lds.io/github/do
-00000560: 776e 6c6f 6164 732f 4b75 616e 6861 6f2d  wnloads/Kuanhao-
-00000570: 4368 616f 2f6c 6966 746f 6e2f 746f 7461  Chao/lifton/tota
-00000580: 6c2e 7376 673f 7374 796c 653d 736f 6369  l.svg?style=soci
-00000590: 616c 2661 6d70 3b6c 6f67 6f3d 6769 7468  al&amp;logo=gith
-000005a0: 7562 2661 6d70 3b6c 6162 656c 3d44 6f77  ub&amp;label=Dow
-000005b0: 6e6c 6f61 6422 3e3c 2f61 3e0a 3c61 2063  nload"></a>.<a c
-000005c0: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
-000005d0: 6578 7465 726e 616c 2069 6d61 6765 2d72  external image-r
-000005e0: 6566 6572 656e 6365 2220 6872 6566 3d22  eference" href="
-000005f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000600: 6f6d 2f4b 7561 6e68 616f 2d43 6861 6f2f  om/Kuanhao-Chao/
-00000610: 6c69 6674 6f6e 2f72 656c 6561 7365 7322  lifton/releases"
-00000620: 3e3c 696d 6720 616c 743d 2268 7474 7073  ><img alt="https
-00000630: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000640: 6f2f 6261 6467 652f 706c 6174 666f 726d  o/badge/platform
-00000650: 2d6d 6163 4f53 5f2f 4c69 6e75 782d 6772  -macOS_/Linux-gr
-00000660: 6565 6e2e 7376 6722 2073 7263 3d22 6874  een.svg" src="ht
-00000670: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000680: 732e 696f 2f62 6164 6765 2f70 6c61 7466  s.io/badge/platf
-00000690: 6f72 6d2d 6d61 634f 535f 2f4c 696e 7578  orm-macOS_/Linux
-000006a0: 2d67 7265 656e 2e73 7667 223e 3c2f 613e  -green.svg"></a>
-000006b0: 0a3c 6120 636c 6173 733d 2272 6566 6572  .<a class="refer
-000006c0: 656e 6365 2065 7874 6572 6e61 6c20 696d  ence external im
-000006d0: 6167 652d 7265 6665 7265 6e63 6522 2068  age-reference" h
-000006e0: 7265 663d 2268 7474 7073 3a2f 2f63 6f6c  ref="https://col
-000006f0: 6162 2e72 6573 6561 7263 682e 676f 6f67  ab.research.goog
-00000700: 6c65 2e63 6f6d 2f67 6974 6875 622f 4b75  le.com/github/Ku
-00000710: 616e 6861 6f2d 4368 616f 2f6c 6966 746f  anhao-Chao/lifto
-00000720: 6e2f 626c 6f62 2f6d 6169 6e2f 6e6f 7465  n/blob/main/note
-00000730: 626f 6f6b 2f6c 6966 746f 6e5f 6578 616d  book/lifton_exam
-00000740: 706c 652e 6970 796e 6222 3e3c 696d 6720  ple.ipynb"><img 
-00000750: 616c 743d 2268 7474 7073 3a2f 2f63 6f6c  alt="https://col
-00000760: 6162 2e72 6573 6561 7263 682e 676f 6f67  ab.research.goog
-00000770: 6c65 2e63 6f6d 2f61 7373 6574 732f 636f  le.com/assets/co
-00000780: 6c61 622d 6261 6467 652e 7376 6722 2073  lab-badge.svg" s
-00000790: 7263 3d22 6874 7470 733a 2f2f 636f 6c61  rc="https://cola
-000007a0: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
-000007b0: 652e 636f 6d2f 6173 7365 7473 2f63 6f6c  e.com/assets/col
-000007c0: 6162 2d62 6164 6765 2e73 7667 223e 3c2f  ab-badge.svg"></
-000007d0: 613e 0a3c 6469 7620 636c 6173 733d 226c  a>.<div class="l
-000007e0: 696e 652d 626c 6f63 6b22 3e0a 3c64 6976  ine-block">.<div
-000007f0: 2063 6c61 7373 3d22 6c69 6e65 223e 3c62   class="line"><b
-00000800: 723e 3c2f 6469 763e 0a3c 2f64 6976 3e0a  r></div>.</div>.
-00000810: 3c70 3e4c 6966 744f 6e20 6973 2061 2068  <p>LiftOn is a h
-00000820: 6f6d 6f6c 6f67 792d 6261 7365 6420 6c69  omology-based li
-00000830: 6674 2d6f 7665 7220 746f 6f6c 2064 6573  ft-over tool des
-00000840: 6967 6e65 6420 746f 2061 6363 7572 6174  igned to accurat
-00000850: 656c 7920 6d61 7020 616e 6e6f 7461 7469  ely map annotati
-00000860: 6f6e 7320 696e 2047 4646 206f 7220 4754  ons in GFF or GT
-00000870: 4620 6265 7477 6565 6e20 6173 7365 6d62  F between assemb
-00000880: 6c69 6573 2e20 4974 2069 7320 6275 696c  lies. It is buil
-00000890: 7420 7570 6f6e 2074 6865 2066 616e 7461  t upon the fanta
-000008a0: 7374 6963 203c 6120 636c 6173 733d 2272  stic <a class="r
-000008b0: 6566 6572 656e 6365 2065 7874 6572 6e61  eference externa
-000008c0: 6c22 2068 7265 663d 2268 7474 7073 3a2f  l" href="https:/
-000008d0: 2f61 6361 6465 6d69 632e 6f75 702e 636f  /academic.oup.co
-000008e0: 6d2f 6269 6f69 6e66 6f72 6d61 7469 6373  m/bioinformatics
-000008f0: 2f61 7274 6963 6c65 2f33 372f 3132 2f31  /article/37/12/1
-00000900: 3633 392f 3630 3335 3132 383f 6c6f 6769  639/6035128?logi
-00000910: 6e3d 7472 7565 223e 4c69 6674 6f66 663c  n=true">Liftoff<
-00000920: 2f61 3e20 2863 7265 6469 7473 2074 6f20  /a> (credits to 
-00000930: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
-00000940: 6e63 6520 6578 7465 726e 616c 2220 6872  nce external" hr
-00000950: 6566 3d22 6874 7470 733a 2f2f 7363 686f  ef="https://scho
-00000960: 6c61 722e 676f 6f67 6c65 2e63 6f6d 2f63  lar.google.com/c
-00000970: 6974 6174 696f 6e73 3f75 7365 723d 4e33  itations?user=N3
-00000980: 7458 6b37 5141 4141 414a 2661 6d70 3b68  tXk7QAAAAJ&amp;h
-00000990: 6c3d 656e 223e 4472 2e20 416c 6169 6e61  l=en">Dr. Alaina
+00000040: 7465 7222 2073 7263 3d22 6874 7470 733a  ter" src="https:
+00000050: 2f2f 7374 6f72 6167 652e 676f 6f67 6c65  //storage.google
+00000060: 6170 6973 2e63 6f6d 2f73 746f 7261 6765  apis.com/storage
+00000070: 2e6b 6863 6861 6f2e 636f 6d2f 6669 6775  .khchao.com/figu
+00000080: 7265 732f 4c69 6674 4f6e 2f4c 6966 744f  res/LiftOn/LiftO
+00000090: 6e5f 636f 6c6f 722e 706e 6722 2073 7479  n_color.png" sty
+000000a0: 6c65 3d22 7769 6474 683a 3930 2522 3e0a  le="width:90%">.
+000000b0: 0a3c 6469 7620 636c 6173 733d 2263 6f6e  .<div class="con
+000000c0: 7465 6e74 223e 0a3c 6120 636c 6173 733d  tent">.<a class=
+000000d0: 2272 6566 6572 656e 6365 2065 7874 6572  "reference exter
+000000e0: 6e61 6c20 696d 6167 652d 7265 6665 7265  nal image-refere
+000000f0: 6e63 6522 2068 7265 663d 2268 7474 7073  nce" href="https
+00000100: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000110: 6f2f 6261 6467 652f 4c69 6365 6e73 652d  o/badge/License-
+00000120: 4750 4c76 332d 7965 6c6c 6f77 2e73 7667  GPLv3-yellow.svg
+00000130: 223e 3c69 6d67 2061 6c74 3d22 6874 7470  "><img alt="http
+00000140: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000150: 696f 2f62 6164 6765 2f4c 6963 656e 7365  io/badge/License
+00000160: 2d47 504c 7633 2d79 656c 6c6f 772e 7376  -GPLv3-yellow.sv
+00000170: 6722 2073 7263 3d22 6874 7470 733a 2f2f  g" src="https://
+00000180: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000190: 6164 6765 2f4c 6963 656e 7365 2d47 504c  adge/License-GPL
+000001a0: 7633 2d79 656c 6c6f 772e 7376 6722 3e3c  v3-yellow.svg"><
+000001b0: 2f61 3e0a 3c61 2063 6c61 7373 3d22 7265  /a>.<a class="re
+000001c0: 6665 7265 6e63 6520 6578 7465 726e 616c  ference external
+000001d0: 2069 6d61 6765 2d72 6566 6572 656e 6365   image-reference
+000001e0: 2220 6872 6566 3d22 6874 7470 733a 2f2f  " href="https://
+000001f0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000200: 6164 6765 2f76 6572 7369 6f6e 2d76 2e30  adge/version-v.0
+00000210: 2e30 2e31 2d62 6c75 6522 3e3c 696d 6720  .0.1-blue"><img 
+00000220: 616c 743d 2268 7474 7073 3a2f 2f69 6d67  alt="https://img
+00000230: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+00000240: 652f 7665 7273 696f 6e2d 762e 302e 302e  e/version-v.0.0.
+00000250: 312d 626c 7565 2220 7372 633d 2268 7474  1-blue" src="htt
+00000260: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000270: 2e69 6f2f 6261 6467 652f 7665 7273 696f  .io/badge/versio
+00000280: 6e2d 762e 302e 302e 312d 626c 7565 223e  n-v.0.0.1-blue">
+00000290: 3c2f 613e 0a3c 6120 636c 6173 733d 2272  </a>.<a class="r
+000002a0: 6566 6572 656e 6365 2065 7874 6572 6e61  eference externa
+000002b0: 6c20 696d 6167 652d 7265 6665 7265 6e63  l image-referenc
+000002c0: 6522 2068 7265 663d 2268 7474 7073 3a2f  e" href="https:/
+000002d0: 2f70 6570 792e 7465 6368 2f70 726f 6a65  /pepy.tech/proje
+000002e0: 6374 2f6c 6966 746f 6e22 3e3c 696d 6720  ct/lifton"><img 
+000002f0: 616c 743d 2268 7474 7073 3a2f 2f73 7461  alt="https://sta
+00000300: 7469 632e 7065 7079 2e74 6563 682f 7065  tic.pepy.tech/pe
+00000310: 7273 6f6e 616c 697a 6564 2d62 6164 6765  rsonalized-badge
+00000320: 2f6c 6966 746f 6e3f 7065 7269 6f64 3d74  /lifton?period=t
+00000330: 6f74 616c 2661 6d70 3b75 6e69 7473 3d61  otal&amp;units=a
+00000340: 6262 7265 7669 6174 696f 6e26 616d 703b  bbreviation&amp;
+00000350: 6c65 6674 5f63 6f6c 6f72 3d67 7265 7926  left_color=grey&
+00000360: 616d 703b 7269 6768 745f 636f 6c6f 723d  amp;right_color=
+00000370: 626c 7565 2661 6d70 3b6c 6566 745f 7465  blue&amp;left_te
+00000380: 7874 3d50 7950 6925 3230 646f 776e 6c6f  xt=PyPi%20downlo
+00000390: 6164 7322 2073 7263 3d22 6874 7470 733a  ads" src="https:
+000003a0: 2f2f 7374 6174 6963 2e70 6570 792e 7465  //static.pepy.te
+000003b0: 6368 2f70 6572 736f 6e61 6c69 7a65 642d  ch/personalized-
+000003c0: 6261 6467 652f 6c69 6674 6f6e 3f70 6572  badge/lifton?per
+000003d0: 696f 643d 746f 7461 6c26 616d 703b 756e  iod=total&amp;un
+000003e0: 6974 733d 6162 6272 6576 6961 7469 6f6e  its=abbreviation
+000003f0: 2661 6d70 3b6c 6566 745f 636f 6c6f 723d  &amp;left_color=
+00000400: 6772 6579 2661 6d70 3b72 6967 6874 5f63  grey&amp;right_c
+00000410: 6f6c 6f72 3d62 6c75 6526 616d 703b 6c65  olor=blue&amp;le
+00000420: 6674 5f74 6578 743d 5079 5069 2532 3064  ft_text=PyPi%20d
+00000430: 6f77 6e6c 6f61 6473 223e 3c2f 613e 0a3c  ownloads"></a>.<
+00000440: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
+00000450: 6365 2065 7874 6572 6e61 6c20 696d 6167  ce external imag
+00000460: 652d 7265 6665 7265 6e63 6522 2068 7265  e-reference" hre
+00000470: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00000480: 622e 636f 6d2f 4b75 616e 6861 6f2d 4368  b.com/Kuanhao-Ch
+00000490: 616f 2f6c 6966 746f 6e2f 7265 6c65 6173  ao/lifton/releas
+000004a0: 6573 223e 3c69 6d67 2061 6c74 3d22 6874  es"><img alt="ht
+000004b0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000004c0: 732e 696f 2f67 6974 6875 622f 646f 776e  s.io/github/down
+000004d0: 6c6f 6164 732f 4b75 616e 6861 6f2d 4368  loads/Kuanhao-Ch
+000004e0: 616f 2f6c 6966 746f 6e2f 746f 7461 6c2e  ao/lifton/total.
+000004f0: 7376 673f 7374 796c 653d 736f 6369 616c  svg?style=social
+00000500: 2661 6d70 3b6c 6f67 6f3d 6769 7468 7562  &amp;logo=github
+00000510: 2661 6d70 3b6c 6162 656c 3d44 6f77 6e6c  &amp;label=Downl
+00000520: 6f61 6422 2073 7263 3d22 6874 7470 733a  oad" src="https:
+00000530: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000540: 2f67 6974 6875 622f 646f 776e 6c6f 6164  /github/download
+00000550: 732f 4b75 616e 6861 6f2d 4368 616f 2f6c  s/Kuanhao-Chao/l
+00000560: 6966 746f 6e2f 746f 7461 6c2e 7376 673f  ifton/total.svg?
+00000570: 7374 796c 653d 736f 6369 616c 2661 6d70  style=social&amp
+00000580: 3b6c 6f67 6f3d 6769 7468 7562 2661 6d70  ;logo=github&amp
+00000590: 3b6c 6162 656c 3d44 6f77 6e6c 6f61 6422  ;label=Download"
+000005a0: 3e3c 2f61 3e0a 3c61 2063 6c61 7373 3d22  ></a>.<a class="
+000005b0: 7265 6665 7265 6e63 6520 6578 7465 726e  reference extern
+000005c0: 616c 2069 6d61 6765 2d72 6566 6572 656e  al image-referen
+000005d0: 6365 2220 6872 6566 3d22 6874 7470 733a  ce" href="https:
+000005e0: 2f2f 6769 7468 7562 2e63 6f6d 2f4b 7561  //github.com/Kua
+000005f0: 6e68 616f 2d43 6861 6f2f 6c69 6674 6f6e  nhao-Chao/lifton
+00000600: 2f72 656c 6561 7365 7322 3e3c 696d 6720  /releases"><img 
+00000610: 616c 743d 2268 7474 7073 3a2f 2f69 6d67  alt="https://img
+00000620: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+00000630: 652f 706c 6174 666f 726d 2d6d 6163 4f53  e/platform-macOS
+00000640: 5f2f 4c69 6e75 782d 6772 6565 6e2e 7376  _/Linux-green.sv
+00000650: 6722 2073 7263 3d22 6874 7470 733a 2f2f  g" src="https://
+00000660: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000670: 6164 6765 2f70 6c61 7466 6f72 6d2d 6d61  adge/platform-ma
+00000680: 634f 535f 2f4c 696e 7578 2d67 7265 656e  cOS_/Linux-green
+00000690: 2e73 7667 223e 3c2f 613e 0a3c 6120 636c  .svg"></a>.<a cl
+000006a0: 6173 733d 2272 6566 6572 656e 6365 2065  ass="reference e
+000006b0: 7874 6572 6e61 6c20 696d 6167 652d 7265  xternal image-re
+000006c0: 6665 7265 6e63 6522 2068 7265 663d 2268  ference" href="h
+000006d0: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
+000006e0: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
+000006f0: 2f67 6974 6875 622f 4b75 616e 6861 6f2d  /github/Kuanhao-
+00000700: 4368 616f 2f6c 6966 746f 6e2f 626c 6f62  Chao/lifton/blob
+00000710: 2f6d 6169 6e2f 6e6f 7465 626f 6f6b 2f6c  /main/notebook/l
+00000720: 6966 746f 6e5f 6578 616d 706c 652e 6970  ifton_example.ip
+00000730: 796e 6222 3e3c 696d 6720 616c 743d 2268  ynb"><img alt="h
+00000740: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
+00000750: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
+00000760: 2f61 7373 6574 732f 636f 6c61 622d 6261  /assets/colab-ba
+00000770: 6467 652e 7376 6722 2073 7263 3d22 6874  dge.svg" src="ht
+00000780: 7470 733a 2f2f 636f 6c61 622e 7265 7365  tps://colab.rese
+00000790: 6172 6368 2e67 6f6f 676c 652e 636f 6d2f  arch.google.com/
+000007a0: 6173 7365 7473 2f63 6f6c 6162 2d62 6164  assets/colab-bad
+000007b0: 6765 2e73 7667 223e 3c2f 613e 0a3c 6469  ge.svg"></a>.<di
+000007c0: 7620 636c 6173 733d 226c 696e 652d 626c  v class="line-bl
+000007d0: 6f63 6b22 3e0a 3c64 6976 2063 6c61 7373  ock">.<div class
+000007e0: 3d22 6c69 6e65 223e 3c62 723e 3c2f 6469  ="line"><br></di
+000007f0: 763e 0a3c 2f64 6976 3e0a 3c6c 696e 6b20  v>.</div>.<link 
+00000800: 7265 6c3d 2273 7479 6c65 7368 6565 7422  rel="stylesheet"
+00000810: 2068 7265 663d 2268 7474 7073 3a2f 2f63   href="https://c
+00000820: 646e 6a73 2e63 6c6f 7564 666c 6172 652e  dnjs.cloudflare.
+00000830: 636f 6d2f 616a 6178 2f6c 6962 732f 666f  com/ajax/libs/fo
+00000840: 6e74 2d61 7765 736f 6d65 2f34 2e37 2e30  nt-awesome/4.7.0
+00000850: 2f63 7373 2f66 6f6e 742d 6177 6573 6f6d  /css/font-awesom
+00000860: 652e 6d69 6e2e 6373 7322 3e0a 0a4c 6966  e.min.css">..Lif
+00000870: 744f 6e20 6973 2061 2068 6f6d 6f6c 6f67  tOn is a homolog
+00000880: 792d 6261 7365 6420 6c69 6674 2d6f 7665  y-based lift-ove
+00000890: 7220 746f 6f6c 2075 7369 6e67 2062 6f74  r tool using bot
+000008a0: 6820 444e 412d 444e 4120 616c 6967 6e6d  h DNA-DNA alignm
+000008b0: 656e 7473 2028 6672 6f6d 203c 6120 6872  ents (from <a hr
+000008c0: 6566 3d22 6874 7470 733a 2f2f 6163 6164  ef="https://acad
+000008d0: 656d 6963 2e6f 7570 2e63 6f6d 2f62 696f  emic.oup.com/bio
+000008e0: 696e 666f 726d 6174 6963 732f 6172 7469  informatics/arti
+000008f0: 636c 652f 3337 2f31 322f 3136 3339 2f36  cle/37/12/1639/6
+00000900: 3033 3531 3238 3f6c 6f67 696e 3d74 7275  035128?login=tru
+00000910: 6522 2074 6172 6765 743d 225f 626c 616e  e" target="_blan
+00000920: 6b22 3e4c 6966 746f 6666 3c2f 613e 2c20  k">Liftoff</a>, 
+00000930: 6372 6564 6974 7320 746f 203c 6120 6872  credits to <a hr
+00000940: 6566 3d22 6874 7470 733a 2f2f 7363 686f  ef="https://scho
+00000950: 6c61 722e 676f 6f67 6c65 2e63 6f6d 2f63  lar.google.com/c
+00000960: 6974 6174 696f 6e73 3f75 7365 723d 4e33  itations?user=N3
+00000970: 7458 6b37 5141 4141 414a 2661 6d70 3b68  tXk7QAAAAJ&amp;h
+00000980: 6c3d 656e 2220 7461 7267 6574 3d22 5f62  l=en" target="_b
+00000990: 6c61 6e6b 223e 4472 2e20 416c 6169 6e61  lank">Dr. Alaina
 000009a0: 2053 6875 6d61 7465 3c2f 613e 2920 616e   Shumate</a>) an
-000009b0: 6420 3c61 2063 6c61 7373 3d22 7265 6665  d <a class="refe
-000009c0: 7265 6e63 6520 6578 7465 726e 616c 2220  rence external" 
-000009d0: 6872 6566 3d22 6874 7470 733a 2f2f 6163  href="https://ac
-000009e0: 6164 656d 6963 2e6f 7570 2e63 6f6d 2f62  ademic.oup.com/b
-000009f0: 696f 696e 666f 726d 6174 6963 732f 6172  ioinformatics/ar
-00000a00: 7469 636c 652f 3339 2f31 2f62 7461 6430  ticle/39/1/btad0
-00000a10: 3134 2f36 3938 3936 3231 223e 6d69 6e69  14/6989621">mini
-00000a20: 7072 6f74 3c2f 613e 2028 6372 6564 6974  prot</a> (credit
-00000a30: 7320 746f 203c 6120 636c 6173 733d 2272  s to <a class="r
-00000a40: 6566 6572 656e 6365 2065 7874 6572 6e61  eference externa
-00000a50: 6c22 2068 7265 663d 2268 7474 703a 2f2f  l" href="http://
-00000a60: 6c69 6865 6e67 2e6f 7267 223e 4472 2e20  liheng.org">Dr. 
-00000a70: 4865 6e67 204c 693c 2f61 3e29 2c20 616e  Heng Li</a>), an
-00000a80: 6420 656d 706c 6f79 7320 6120 3c61 2063  d employs a <a c
-00000a90: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
-00000aa0: 696e 7465 726e 616c 2220 6872 6566 3d22  internal" href="
-00000ab0: 6874 7470 3a2f 2f63 6362 2e6a 6875 2e65  http://ccb.jhu.e
-00000ac0: 6475 2f6c 6966 746f 6e2f 636f 6e74 656e  du/lifton/conten
-00000ad0: 742f 6265 6869 6e64 5f73 6365 6e65 732e  t/behind_scenes.
-00000ae0: 6874 6d6c 2370 726f 7465 696e 2d6d 6178  html#protein-max
-00000af0: 696d 697a 6174 696f 6e2d 616c 676f 7269  imization-algori
-00000b00: 7468 6d22 3e3c 7370 616e 2063 6c61 7373  thm"><span class
-00000b10: 3d22 7374 6420 7374 642d 7265 6622 3e50  ="std std-ref">P
-00000b20: 726f 7465 696e 2d6d 6178 696d 697a 6174  rotein-maximizat
-00000b30: 696f 6e20 616c 676f 7269 7468 6d3c 2f73  ion algorithm</s
-00000b40: 7061 6e3e 3c2f 613e 2074 6f20 696d 7072  pan></a> to impr
-00000b50: 6f76 6520 7468 6520 7072 6f74 6569 6e2d  ove the protein-
-00000b60: 636f 6469 6e67 2067 656e 6520 6c69 6674  coding gene lift
-00000b70: 2d6f 7665 7220 7072 6f63 6573 732e 3c2f  -over process.</
-00000b80: 703e 0a3c 7365 6374 696f 6e20 6964 3d22  p>.<section id="
-00000b90: 7768 792d 6c69 6674 6f6e 2220 636c 6173  why-lifton" clas
-00000ba0: 733d 2222 3e0a 3c68 323e 5768 7920 4c69  s="">.<h2>Why Li
-00000bb0: 6674 4f6e e29d 933c 6120 636c 6173 733d  ftOn...<a class=
-00000bc0: 2268 6561 6465 726c 696e 6b22 2068 7265  "headerlink" hre
-00000bd0: 663d 2223 7768 792d 6c69 6674 6f6e 2220  f="#why-lifton" 
-00000be0: 7469 746c 653d 2250 6572 6d61 6c69 6e6b  title="Permalink
-00000bf0: 2074 6f20 7468 6973 2068 6561 6469 6e67   to this heading
-00000c00: 223e 233c 2f61 3e3c 2f68 323e 0a3c 6f6c  ">#</a></h2>.<ol
-00000c10: 2063 6c61 7373 3d22 6172 6162 6963 2073   class="arabic s
-00000c20: 696d 706c 6522 3e0a 3c6c 693e 3c70 3e3c  imple">.<li><p><
-00000c30: 7374 726f 6e67 3e42 7572 6765 6f6e 696e  strong>Burgeonin
-00000c40: 6720 6e75 6d62 6572 206f 6620 6765 6e6f  g number of geno
-00000c50: 6d65 2061 7373 656d 626c 6965 733c 2f73  me assemblies</s
-00000c60: 7472 6f6e 673e 3a20 4173 206f 6620 4465  trong>: As of De
-00000c70: 6365 6d62 6572 2032 3032 332c 2061 6d6f  cember 2023, amo
-00000c80: 6e67 2074 6865 2031 352c 3537 3820 6469  ng the 15,578 di
-00000c90: 7374 696e 6374 2065 756b 6172 796f 7469  stinct eukaryoti
-00000ca0: 6320 6765 6e6f 6d65 732c 206f 6e6c 7920  c genomes, only 
-00000cb0: 312c 3131 3120 6861 7665 2062 6565 6e20  1,111 have been 
-00000cc0: 616e 6e6f 7461 7465 6420 283c 6120 636c  annotated (<a cl
-00000cd0: 6173 733d 2272 6566 6572 656e 6365 2065  ass="reference e
-00000ce0: 7874 6572 6e61 6c22 2068 7265 663d 2268  xternal" href="h
-00000cf0: 7474 7073 3a2f 2f77 7777 2e6e 6362 692e  ttps://www.ncbi.
-00000d00: 6e6c 6d2e 6e69 682e 676f 762f 6765 6e6f  nlm.nih.gov/geno
-00000d10: 6d65 2f61 6e6e 6f74 6174 696f 6e5f 6575  me/annotation_eu
-00000d20: 6b2f 2367 7261 7068 7322 3e45 756b 6172  k/#graphs">Eukar
-00000d30: 796f 7469 6320 4765 6e6f 6d65 2041 6e6e  yotic Genome Ann
-00000d40: 6f74 6174 696f 6e20 6174 204e 4342 493c  otation at NCBI<
-00000d50: 2f61 3e29 2e20 4d6f 7265 2061 6e64 206d  /a>). More and m
-00000d60: 6f72 6520 6869 6768 2071 7561 6c69 7479  ore high quality
-00000d70: 2061 7373 656d 626c 6965 7320 6172 6520   assemblies are 
-00000d80: 6765 6e65 7261 7465 642e 2057 6520 6e65  generated. We ne
-00000d90: 6564 2074 6f20 6163 6375 7261 7465 6c79  ed to accurately
-00000da0: 2061 6e6e 6f74 6174 6520 7468 656d 2e3c   annotate them.<
-00000db0: 2f70 3e3c 2f6c 693e 0a3c 6c69 3e3c 703e  /p></li>.<li><p>
-00000dc0: 3c73 7472 6f6e 673e 496d 7072 6f76 6564  <strong>Improved
-00000dd0: 2070 726f 7465 696e 2d63 6f64 696e 6720   protein-coding 
-00000de0: 6765 6e65 206d 6170 7069 6e67 3c2f 7374  gene mapping</st
-00000df0: 726f 6e67 3e3a 2054 6865 2070 6f70 756c  rong>: The popul
-00000e00: 6172 203c 6120 636c 6173 733d 2272 6566  ar <a class="ref
-00000e10: 6572 656e 6365 2065 7874 6572 6e61 6c22  erence external"
-00000e20: 2068 7265 663d 2268 7474 7073 3a2f 2f61   href="https://a
-00000e30: 6361 6465 6d69 632e 6f75 702e 636f 6d2f  cademic.oup.com/
-00000e40: 6269 6f69 6e66 6f72 6d61 7469 6373 2f61  bioinformatics/a
-00000e50: 7274 6963 6c65 2f33 372f 3132 2f31 3633  rticle/37/12/163
-00000e60: 392f 3630 3335 3132 383f 6c6f 6769 6e3d  9/6035128?login=
-00000e70: 7472 7565 223e 4c69 6674 6f66 663c 2f61  true">Liftoff</a
-00000e80: 3e20 6d61 7020 6765 6e65 7320 6f6e 6c79  > map genes only
-00000e90: 2062 6173 6564 206f 6e20 7468 6520 444e   based on the DN
-00000ea0: 4120 616c 6967 6e6d 656e 742e 2057 6974  A alignment. Wit
-00000eb0: 6820 7468 6520 7072 6f74 6569 6e2d 746f  h the protein-to
-00000ec0: 2d67 656e 6f6d 6520 616c 6967 6e6d 656e  -genome alignmen
-00000ed0: 742c 204c 6966 744f 6e20 6973 2061 626c  t, LiftOn is abl
-00000ee0: 6520 746f 2066 7572 7468 6572 2069 6d70  e to further imp
-00000ef0: 726f 7665 2074 6865 206c 6966 742d 6f76  rove the lift-ov
-00000f00: 6572 2070 726f 7465 696e 2d63 6f64 696e  er protein-codin
-00000f10: 6720 6765 6e65 2061 6e6e 6f74 6174 696f  g gene annotatio
-00000f20: 6e73 2e20 4c69 6674 4f6e 2069 6d70 726f  ns. LiftOn impro
-00000f30: 7665 7320 7468 6520 6375 7272 656e 7420  ves the current 
-00000f40: 7265 6c65 6173 6564 2054 3254 2d43 484d  released T2T-CHM
-00000f50: 3133 2061 6e6e 6f74 6174 696f 6e20 283c  13 annotation (<
-00000f60: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
-00000f70: 6365 2065 7874 6572 6e61 6c22 2068 7265  ce external" hre
-00000f80: 663d 2268 7474 7073 3a2f 2f73 332d 7573  f="https://s3-us
-00000f90: 2d77 6573 742d 322e 616d 617a 6f6e 6177  -west-2.amazonaw
-00000fa0: 732e 636f 6d2f 6875 6d61 6e2d 7061 6e67  s.com/human-pang
-00000fb0: 656e 6f6d 6963 732f 5432 542f 4348 4d31  enomics/T2T/CHM1
-00000fc0: 332f 6173 7365 6d62 6c69 6573 2f61 6e6e  3/assemblies/ann
-00000fd0: 6f74 6174 696f 6e2f 6368 6d31 3376 322e  otation/chm13v2.
-00000fe0: 305f 5265 6653 6571 5f4c 6966 746f 6666  0_RefSeq_Liftoff
-00000ff0: 5f76 352e 312e 6766 6633 2e67 7a22 3e4a  _v5.1.gff3.gz">J
-00001000: 4855 2052 6566 5365 7176 3131 3020 2b20  HU RefSeqv110 + 
-00001010: 4c69 6674 6f66 6620 7635 2e31 3c2f 613e  Liftoff v5.1</a>
-00001020: 292e 3c2f 703e 3c2f 6c69 3e0a 3c6c 693e  ).</p></li>.<li>
-00001030: 3c70 3e3c 7374 726f 6e67 3e49 6d70 726f  <p><strong>Impro
-00001040: 7665 6420 6469 7374 616e 7420 7370 6563  ved distant spec
-00001050: 6965 7320 6c69 6674 2d6f 7665 723c 2f73  ies lift-over</s
-00001060: 7472 6f6e 673e 3a20 4c69 6674 4f6e 2065  trong>: LiftOn e
-00001070: 7874 656e 6473 2066 726f 6d20 6c69 6674  xtends from lift
-00001080: 2d6f 7665 7220 6265 7477 6565 6e20 7468  -over between th
-00001090: 6520 7361 6d65 206f 7220 636c 6f73 656c  e same or closel
-000010a0: 7920 7265 6c61 7465 6420 7370 6563 6965  y related specie
-000010b0: 7320 746f 206d 6f72 6520 6469 7374 616e  s to more distan
-000010c0: 746c 7920 7265 6c61 7465 6420 7370 6563  tly related spec
-000010d0: 6965 732e 2053 6565 203c 7370 616e 2063  ies. See <span c
-000010e0: 6c61 7373 3d22 7872 6566 2073 7464 2073  lass="xref std s
-000010f0: 7464 2d72 6566 223e 6d6f 7573 655f 325f  td-ref">mouse_2_
-00001100: 7261 743c 2f73 7061 6e3e 2061 6e64 203c  rat</span> and <
-00001110: 7370 616e 2063 6c61 7373 3d22 7872 6566  span class="xref
-00001120: 2073 7464 2073 7464 2d72 6566 223e 6472   std std-ref">dr
-00001130: 6f73 6f70 6869 6c61 5f6d 656c 616e 6f67  osophila_melanog
-00001140: 6173 7465 725f 325f 6572 6563 7461 3c2f  aster_2_erecta</
-00001150: 7370 616e 3e20 6c69 6674 2d6f 7665 7220  span> lift-over 
-00001160: 7365 6374 696f 6e73 2e3c 2f70 3e3c 2f6c  sections.</p></l
-00001170: 693e 0a3c 2f6f 6c3e 0a3c 703e 4c69 6674  i>.</ol>.<p>Lift
-00001180: 4f6e 2069 7320 6672 6565 2c20 6974 2773  On is free, it's
-00001190: 206f 7065 6e20 736f 7572 6365 2c20 6974   open source, it
-000011a0: 2773 2065 6173 7920 746f 2069 6e73 7461  's easy to insta
-000011b0: 6c6c 202c 2061 6e64 2069 7427 7320 696e  ll , and it's in
-000011c0: 2050 7974 686f 6e21 3c2f 703e 0a3c 6469   Python!</p>.<di
-000011d0: 7620 636c 6173 733d 226c 696e 652d 626c  v class="line-bl
-000011e0: 6f63 6b22 3e0a 3c64 6976 2063 6c61 7373  ock">.<div class
-000011f0: 3d22 6c69 6e65 223e 3c62 723e 3c2f 6469  ="line"><br></di
-00001200: 763e 0a3c 2f64 6976 3e0a 3c2f 7365 6374  v>.</div>.</sect
-00001210: 696f 6e3e 0a3c 7365 6374 696f 6e20 6964  ion>.<section id
-00001220: 3d22 7768 6f2d 6973 2d69 742d 666f 7222  ="who-is-it-for"
-00001230: 2063 6c61 7373 3d22 223e 0a3c 6832 3e57   class="">.<h2>W
-00001240: 686f 2069 7320 6974 2066 6f72 e29d 933c  ho is it for...<
-00001250: 6120 636c 6173 733d 2268 6561 6465 726c  a class="headerl
-00001260: 696e 6b22 2068 7265 663d 2223 7768 6f2d  ink" href="#who-
-00001270: 6973 2d69 742d 666f 7222 2074 6974 6c65  is-it-for" title
-00001280: 3d22 5065 726d 616c 696e 6b20 746f 2074  ="Permalink to t
-00001290: 6869 7320 6865 6164 696e 6722 3e23 3c2f  his heading">#</
-000012a0: 613e 3c2f 6832 3e0a 3c6f 6c20 636c 6173  a></h2>.<ol clas
-000012b0: 733d 2261 7261 6269 6320 7369 6d70 6c65  s="arabic simple
-000012c0: 223e 0a3c 6c69 3e3c 703e 4966 2079 6f75  ">.<li><p>If you
-000012d0: 2068 6176 6520 7365 7175 656e 6365 6420   have sequenced 
-000012e0: 616e 6420 6173 7365 6d62 6c65 6420 6120  and assembled a 
-000012f0: 6e65 7720 6765 6e6f 6d65 2061 6e64 206e  new genome and n
-00001300: 6565 6420 746f 2061 6e6e 6f74 6174 6520  eed to annotate 
-00001310: 6974 2c20 4c69 6674 4f6e 2069 7320 7468  it, LiftOn is th
-00001320: 6520 6964 6561 6c20 6368 6f69 6365 2066  e ideal choice f
-00001330: 6f72 2067 656e 6572 6174 696e 6720 616e  or generating an
-00001340: 6e6f 7461 7469 6f6e 732e 3c2f 703e 3c2f  notations.</p></
-00001350: 6c69 3e0a 3c6c 693e 3c70 3e49 6620 796f  li>.<li><p>If yo
-00001360: 7520 7761 6e74 2074 6f20 646f 2063 6f6d  u want to do com
-00001370: 7061 7261 7469 7665 2067 656e 6f6d 6963  parative genomic
-00001380: 7320 616e 616c 7973 6973 2c20 7275 6e20  s analysis, run 
-00001390: 6c69 6674 4f6e 2074 6f20 6c69 6674 2d6f  liftOn to lift-o
-000013a0: 7665 7220 616e 6420 636f 6d70 6172 6520  ver and compare 
-000013b0: 616e 6e6f 7461 7469 6f6e 7321 3c2f 703e  annotations!</p>
-000013c0: 3c2f 6c69 3e0a 3c6c 693e 3c70 3e49 6620  </li>.<li><p>If 
-000013d0: 796f 7520 7769 7368 2074 6f20 7574 696c  you wish to util
-000013e0: 697a 6520 7468 6520 6669 6e65 7374 2043  ize the finest C
-000013f0: 484d 3133 2061 6e6e 6f74 6174 696f 6e2c  HM13 annotation,
-00001400: 2079 6f75 2063 616e 2072 756e 204c 6966   you can run Lif
-00001410: 744f 6e21 2057 6520 6861 7665 2061 6c73  tOn! We have als
-00001420: 6f20 7072 652d 6765 6e65 7261 7465 6420  o pre-generated 
-00001430: 7468 6520 3c61 2063 6c61 7373 3d22 7265  the <a class="re
-00001440: 6665 7265 6e63 6520 6578 7465 726e 616c  ference external
-00001450: 2220 6872 6566 3d22 6874 7470 733a 2f2f  " href="https://
-00001460: 6b68 6368 616f 2e63 6f6d 223e 5432 545f  khchao.com">T2T_
-00001470: 4348 4d31 335f 4c69 6674 4f6e 2e67 6666  CHM13_LiftOn.gff
-00001480: 333c 2f61 3e20 6669 6c65 2066 6f72 2079  3</a> file for y
-00001490: 6f75 7220 636f 6e76 656e 6965 6e63 652e  our convenience.
-000014a0: 3c2f 703e 3c2f 6c69 3e0a 3c2f 6f6c 3e0a  </p></li>.</ol>.
-000014b0: 3c64 6976 2063 6c61 7373 3d22 6c69 6e65  <div class="line
-000014c0: 2d62 6c6f 636b 223e 0a3c 6469 7620 636c  -block">.<div cl
-000014d0: 6173 733d 226c 696e 6522 3e3c 6272 3e3c  ass="line"><br><
-000014e0: 2f64 6976 3e0a 3c2f 6469 763e 0a3c 2f73  /div>.</div>.</s
-000014f0: 6563 7469 6f6e 3e0a 3c73 6563 7469 6f6e  ection>.<section
-00001500: 2069 643d 2277 6861 742d 646f 6573 2d6c   id="what-does-l
-00001510: 6966 746f 6e2d 646f 2220 636c 6173 733d  ifton-do" class=
-00001520: 2222 3e0a 3c68 323e 5768 6174 2064 6f65  "">.<h2>What doe
-00001530: 7320 4c69 6674 4f6e 2064 6fe2 9d93 3c61  s LiftOn do...<a
-00001540: 2063 6c61 7373 3d22 6865 6164 6572 6c69   class="headerli
-00001550: 6e6b 2220 6872 6566 3d22 2377 6861 742d  nk" href="#what-
-00001560: 646f 6573 2d6c 6966 746f 6e2d 646f 2220  does-lifton-do" 
-00001570: 7469 746c 653d 2250 6572 6d61 6c69 6e6b  title="Permalink
-00001580: 2074 6f20 7468 6973 2068 6561 6469 6e67   to this heading
-00001590: 223e 233c 2f61 3e3c 2f68 323e 0a3c 703e  ">#</a></h2>.<p>
-000015a0: 4769 7665 6e20 6120 7265 6665 7265 6e63  Given a referenc
-000015b0: 6520 3c73 7472 6f6e 673e 4765 6e6f 6d65  e <strong>Genome
-000015c0: 3c2f 7374 726f 6e67 3e20 3c73 7061 6e20  </strong> <span 
-000015d0: 636c 6173 733d 226d 6174 6820 6e6f 7472  class="math notr
-000015e0: 616e 736c 6174 6520 6e6f 6869 6768 6c69  anslate nohighli
-000015f0: 6768 7422 3e3c 6d6a 782d 636f 6e74 6169  ght"><mjx-contai
-00001600: 6e65 7220 636c 6173 733d 224d 6174 684a  ner class="MathJ
-00001610: 6178 2043 7478 744d 656e 755f 4174 7461  ax CtxtMenu_Atta
-00001620: 6368 6564 5f30 2220 6a61 783d 2243 4854  ched_0" jax="CHT
-00001630: 4d4c 2220 7461 6269 6e64 6578 3d22 3022  ML" tabindex="0"
-00001640: 2063 7478 746d 656e 755f 636f 756e 7465   ctxtmenu_counte
-00001650: 723d 2230 2220 7374 796c 653d 2266 6f6e  r="0" style="fon
-00001660: 742d 7369 7a65 3a20 3131 3925 3b20 706f  t-size: 119%; po
-00001670: 7369 7469 6f6e 3a20 7265 6c61 7469 7665  sition: relative
-00001680: 3b22 3e3c 6d6a 782d 6d61 7468 2063 6c61  ;"><mjx-math cla
-00001690: 7373 3d22 4d4a 582d 5445 5822 2061 7269  ss="MJX-TEX" ari
-000016a0: 612d 6869 6464 656e 3d22 7472 7565 223e  a-hidden="true">
-000016b0: 3c6d 6a78 2d6d 6920 636c 6173 733d 226d  <mjx-mi class="m
-000016c0: 6a78 2d69 223e 3c6d 6a78 2d63 2063 6c61  jx-i"><mjx-c cla
-000016d0: 7373 3d22 6d6a 782d 6331 4434 3435 2054  ss="mjx-c1D445 T
-000016e0: 4558 2d49 223e 3c2f 6d6a 782d 633e 3c2f  EX-I"></mjx-c></
-000016f0: 6d6a 782d 6d69 3e3c 2f6d 6a78 2d6d 6174  mjx-mi></mjx-mat
-00001700: 683e 3c6d 6a78 2d61 7373 6973 7469 7665  h><mjx-assistive
-00001710: 2d6d 6d6c 2075 6e73 656c 6563 7461 626c  -mml unselectabl
-00001720: 653d 226f 6e22 2064 6973 706c 6179 3d22  e="on" display="
-00001730: 696e 6c69 6e65 223e 3c6d 6174 6820 786d  inline"><math xm
-00001740: 6c6e 733d 2268 7474 703a 2f2f 7777 772e  lns="http://www.
-00001750: 7733 2e6f 7267 2f31 3939 382f 4d61 7468  w3.org/1998/Math
-00001760: 2f4d 6174 684d 4c22 3e3c 6d69 3e52 3c2f  /MathML"><mi>R</
-00001770: 6d69 3e3c 2f6d 6174 683e 3c2f 6d6a 782d  mi></math></mjx-
-00001780: 6173 7369 7374 6976 652d 6d6d 6c3e 3c2f  assistive-mml></
-00001790: 6d6a 782d 636f 6e74 6169 6e65 723e 3c2f  mjx-container></
-000017a0: 7370 616e 3e2c 2061 6e20 3c73 7472 6f6e  span>, an <stron
-000017b0: 673e 416e 6e6f 7461 7469 6f6e 3c2f 7374  g>Annotation</st
-000017c0: 726f 6e67 3e20 3c73 7061 6e20 636c 6173  rong> <span clas
-000017d0: 733d 226d 6174 6820 6e6f 7472 616e 736c  s="math notransl
-000017e0: 6174 6520 6e6f 6869 6768 6c69 6768 7422  ate nohighlight"
-000017f0: 3e3c 6d6a 782d 636f 6e74 6169 6e65 7220  ><mjx-container 
-00001800: 636c 6173 733d 224d 6174 684a 6178 2043  class="MathJax C
-00001810: 7478 744d 656e 755f 4174 7461 6368 6564  txtMenu_Attached
-00001820: 5f30 2220 6a61 783d 2243 4854 4d4c 2220  _0" jax="CHTML" 
-00001830: 7461 6269 6e64 6578 3d22 3022 2063 7478  tabindex="0" ctx
-00001840: 746d 656e 755f 636f 756e 7465 723d 2231  tmenu_counter="1
-00001850: 2220 7374 796c 653d 2266 6f6e 742d 7369  " style="font-si
-00001860: 7a65 3a20 3131 3925 3b20 706f 7369 7469  ze: 119%; positi
-00001870: 6f6e 3a20 7265 6c61 7469 7665 3b22 3e3c  on: relative;"><
-00001880: 6d6a 782d 6d61 7468 2063 6c61 7373 3d22  mjx-math class="
-00001890: 4d4a 582d 5445 5822 2061 7269 612d 6869  MJX-TEX" aria-hi
-000018a0: 6464 656e 3d22 7472 7565 223e 3c6d 6a78  dden="true"><mjx
-000018b0: 2d6d 7375 623e 3c6d 6a78 2d6d 6920 636c  -msub><mjx-mi cl
-000018c0: 6173 733d 226d 6a78 2d69 223e 3c6d 6a78  ass="mjx-i"><mjx
-000018d0: 2d63 2063 6c61 7373 3d22 6d6a 782d 6331  -c class="mjx-c1
-000018e0: 4434 3435 2054 4558 2d49 223e 3c2f 6d6a  D445 TEX-I"></mj
-000018f0: 782d 633e 3c2f 6d6a 782d 6d69 3e3c 6d6a  x-c></mjx-mi><mj
-00001900: 782d 7363 7269 7074 2073 7479 6c65 3d22  x-script style="
-00001910: 7665 7274 6963 616c 2d61 6c69 676e 3a20  vertical-align: 
-00001920: 2d30 2e31 3533 656d 3b22 3e3c 6d6a 782d  -0.153em;"><mjx-
-00001930: 6d69 2063 6c61 7373 3d22 6d6a 782d 6922  mi class="mjx-i"
-00001940: 2073 697a 653d 2273 223e 3c6d 6a78 2d63   size="s"><mjx-c
-00001950: 2063 6c61 7373 3d22 6d6a 782d 6331 4434   class="mjx-c1D4
-00001960: 3334 2054 4558 2d49 223e 3c2f 6d6a 782d  34 TEX-I"></mjx-
-00001970: 633e 3c2f 6d6a 782d 6d69 3e3c 2f6d 6a78  c></mjx-mi></mjx
-00001980: 2d73 6372 6970 743e 3c2f 6d6a 782d 6d73  -script></mjx-ms
-00001990: 7562 3e3c 2f6d 6a78 2d6d 6174 683e 3c6d  ub></mjx-math><m
-000019a0: 6a78 2d61 7373 6973 7469 7665 2d6d 6d6c  jx-assistive-mml
-000019b0: 2075 6e73 656c 6563 7461 626c 653d 226f   unselectable="o
-000019c0: 6e22 2064 6973 706c 6179 3d22 696e 6c69  n" display="inli
-000019d0: 6e65 223e 3c6d 6174 6820 786d 6c6e 733d  ne"><math xmlns=
-000019e0: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
-000019f0: 7267 2f31 3939 382f 4d61 7468 2f4d 6174  rg/1998/Math/Mat
-00001a00: 684d 4c22 3e3c 6d73 7562 3e3c 6d69 3e52  hML"><msub><mi>R
-00001a10: 3c2f 6d69 3e3c 6d69 3e41 3c2f 6d69 3e3c  </mi><mi>A</mi><
-00001a20: 2f6d 7375 623e 3c2f 6d61 7468 3e3c 2f6d  /msub></math></m
-00001a30: 6a78 2d61 7373 6973 7469 7665 2d6d 6d6c  jx-assistive-mml
-00001a40: 3e3c 2f6d 6a78 2d63 6f6e 7461 696e 6572  ></mjx-container
-00001a50: 3e3c 2f73 7061 6e3e 2c20 616e 6420 6120  ></span>, and a 
-00001a60: 7461 7267 6574 203c 7374 726f 6e67 3e47  target <strong>G
-00001a70: 656e 6f6d 653c 2f73 7472 6f6e 673e 203c  enome</strong> <
-00001a80: 7370 616e 2063 6c61 7373 3d22 6d61 7468  span class="math
-00001a90: 206e 6f74 7261 6e73 6c61 7465 206e 6f68   notranslate noh
-00001aa0: 6967 686c 6967 6874 223e 3c6d 6a78 2d63  ighlight"><mjx-c
-00001ab0: 6f6e 7461 696e 6572 2063 6c61 7373 3d22  ontainer class="
-00001ac0: 4d61 7468 4a61 7820 4374 7874 4d65 6e75  MathJax CtxtMenu
-00001ad0: 5f41 7474 6163 6865 645f 3022 206a 6178  _Attached_0" jax
-00001ae0: 3d22 4348 544d 4c22 2074 6162 696e 6465  ="CHTML" tabinde
-00001af0: 783d 2230 2220 6374 7874 6d65 6e75 5f63  x="0" ctxtmenu_c
-00001b00: 6f75 6e74 6572 3d22 3222 2073 7479 6c65  ounter="2" style
-00001b10: 3d22 666f 6e74 2d73 697a 653a 2031 3139  ="font-size: 119
-00001b20: 253b 2070 6f73 6974 696f 6e3a 2072 656c  %; position: rel
-00001b30: 6174 6976 653b 223e 3c6d 6a78 2d6d 6174  ative;"><mjx-mat
-00001b40: 6820 636c 6173 733d 224d 4a58 2d54 4558  h class="MJX-TEX
-00001b50: 2220 6172 6961 2d68 6964 6465 6e3d 2274  " aria-hidden="t
-00001b60: 7275 6522 3e3c 6d6a 782d 6d69 2063 6c61  rue"><mjx-mi cla
-00001b70: 7373 3d22 6d6a 782d 6922 3e3c 6d6a 782d  ss="mjx-i"><mjx-
-00001b80: 6320 636c 6173 733d 226d 6a78 2d63 3144  c class="mjx-c1D
-00001b90: 3434 3720 5445 582d 4922 3e3c 2f6d 6a78  447 TEX-I"></mjx
-00001ba0: 2d63 3e3c 2f6d 6a78 2d6d 693e 3c2f 6d6a  -c></mjx-mi></mj
-00001bb0: 782d 6d61 7468 3e3c 6d6a 782d 6173 7369  x-math><mjx-assi
-00001bc0: 7374 6976 652d 6d6d 6c20 756e 7365 6c65  stive-mml unsele
-00001bd0: 6374 6162 6c65 3d22 6f6e 2220 6469 7370  ctable="on" disp
-00001be0: 6c61 793d 2269 6e6c 696e 6522 3e3c 6d61  lay="inline"><ma
-00001bf0: 7468 2078 6d6c 6e73 3d22 6874 7470 3a2f  th xmlns="http:/
-00001c00: 2f77 7777 2e77 332e 6f72 672f 3139 3938  /www.w3.org/1998
-00001c10: 2f4d 6174 682f 4d61 7468 4d4c 223e 3c6d  /Math/MathML"><m
-00001c20: 693e 543c 2f6d 693e 3c2f 6d61 7468 3e3c  i>T</mi></math><
-00001c30: 2f6d 6a78 2d61 7373 6973 7469 7665 2d6d  /mjx-assistive-m
-00001c40: 6d6c 3e3c 2f6d 6a78 2d63 6f6e 7461 696e  ml></mjx-contain
-00001c50: 6572 3e3c 2f73 7061 6e3e 2e20 5468 6520  er></span>. The 
-00001c60: 6c69 6674 2d6f 7665 7220 7072 6f62 6c65  lift-over proble
-00001c70: 6d20 6973 2064 6566 696e 6564 2061 7320  m is defined as 
-00001c80: 7468 6520 7072 6f63 6573 7320 6f66 2063  the process of c
-00001c90: 6861 6e67 696e 6720 7468 6520 636f 6f72  hanging the coor
-00001ca0: 6469 6e61 7465 7320 6f66 203c 7374 726f  dinates of <stro
-00001cb0: 6e67 3e41 6e6e 6f74 6174 696f 6e3c 2f73  ng>Annotation</s
-00001cc0: 7472 6f6e 673e 203c 7370 616e 2063 6c61  trong> <span cla
-00001cd0: 7373 3d22 6d61 7468 206e 6f74 7261 6e73  ss="math notrans
-00001ce0: 6c61 7465 206e 6f68 6967 686c 6967 6874  late nohighlight
-00001cf0: 223e 3c6d 6a78 2d63 6f6e 7461 696e 6572  "><mjx-container
-00001d00: 2063 6c61 7373 3d22 4d61 7468 4a61 7820   class="MathJax 
-00001d10: 4374 7874 4d65 6e75 5f41 7474 6163 6865  CtxtMenu_Attache
-00001d20: 645f 3022 206a 6178 3d22 4348 544d 4c22  d_0" jax="CHTML"
-00001d30: 2074 6162 696e 6465 783d 2230 2220 6374   tabindex="0" ct
-00001d40: 7874 6d65 6e75 5f63 6f75 6e74 6572 3d22  xtmenu_counter="
-00001d50: 3322 2073 7479 6c65 3d22 666f 6e74 2d73  3" style="font-s
-00001d60: 697a 653a 2031 3139 253b 2070 6f73 6974  ize: 119%; posit
-00001d70: 696f 6e3a 2072 656c 6174 6976 653b 223e  ion: relative;">
-00001d80: 3c6d 6a78 2d6d 6174 6820 636c 6173 733d  <mjx-math class=
-00001d90: 224d 4a58 2d54 4558 2220 6172 6961 2d68  "MJX-TEX" aria-h
-00001da0: 6964 6465 6e3d 2274 7275 6522 3e3c 6d6a  idden="true"><mj
-00001db0: 782d 6d73 7562 3e3c 6d6a 782d 6d69 2063  x-msub><mjx-mi c
-00001dc0: 6c61 7373 3d22 6d6a 782d 6922 3e3c 6d6a  lass="mjx-i"><mj
-00001dd0: 782d 6320 636c 6173 733d 226d 6a78 2d63  x-c class="mjx-c
-00001de0: 3144 3434 3520 5445 582d 4922 3e3c 2f6d  1D445 TEX-I"></m
-00001df0: 6a78 2d63 3e3c 2f6d 6a78 2d6d 693e 3c6d  jx-c></mjx-mi><m
-00001e00: 6a78 2d73 6372 6970 7420 7374 796c 653d  jx-script style=
-00001e10: 2276 6572 7469 6361 6c2d 616c 6967 6e3a  "vertical-align:
-00001e20: 202d 302e 3135 3365 6d3b 223e 3c6d 6a78   -0.153em;"><mjx
-00001e30: 2d6d 6920 636c 6173 733d 226d 6a78 2d69  -mi class="mjx-i
-00001e40: 2220 7369 7a65 3d22 7322 3e3c 6d6a 782d  " size="s"><mjx-
-00001e50: 6320 636c 6173 733d 226d 6a78 2d63 3144  c class="mjx-c1D
-00001e60: 3433 3420 5445 582d 4922 3e3c 2f6d 6a78  434 TEX-I"></mjx
-00001e70: 2d63 3e3c 2f6d 6a78 2d6d 693e 3c2f 6d6a  -c></mjx-mi></mj
-00001e80: 782d 7363 7269 7074 3e3c 2f6d 6a78 2d6d  x-script></mjx-m
-00001e90: 7375 623e 3c2f 6d6a 782d 6d61 7468 3e3c  sub></mjx-math><
-00001ea0: 6d6a 782d 6173 7369 7374 6976 652d 6d6d  mjx-assistive-mm
-00001eb0: 6c20 756e 7365 6c65 6374 6162 6c65 3d22  l unselectable="
-00001ec0: 6f6e 2220 6469 7370 6c61 793d 2269 6e6c  on" display="inl
-00001ed0: 696e 6522 3e3c 6d61 7468 2078 6d6c 6e73  ine"><math xmlns
-00001ee0: 3d22 6874 7470 3a2f 2f77 7777 2e77 332e  ="http://www.w3.
-00001ef0: 6f72 672f 3139 3938 2f4d 6174 682f 4d61  org/1998/Math/Ma
-00001f00: 7468 4d4c 223e 3c6d 7375 623e 3c6d 693e  thML"><msub><mi>
-00001f10: 523c 2f6d 693e 3c6d 693e 413c 2f6d 693e  R</mi><mi>A</mi>
-00001f20: 3c2f 6d73 7562 3e3c 2f6d 6174 683e 3c2f  </msub></math></
-00001f30: 6d6a 782d 6173 7369 7374 6976 652d 6d6d  mjx-assistive-mm
-00001f40: 6c3e 3c2f 6d6a 782d 636f 6e74 6169 6e65  l></mjx-containe
-00001f50: 723e 3c2f 7370 616e 3e20 6672 6f6d 203c  r></span> from <
-00001f60: 7374 726f 6e67 3e47 656e 6f6d 653c 2f73  strong>Genome</s
-00001f70: 7472 6f6e 673e 203c 7370 616e 2063 6c61  trong> <span cla
-00001f80: 7373 3d22 6d61 7468 206e 6f74 7261 6e73  ss="math notrans
-00001f90: 6c61 7465 206e 6f68 6967 686c 6967 6874  late nohighlight
-00001fa0: 223e 3c6d 6a78 2d63 6f6e 7461 696e 6572  "><mjx-container
-00001fb0: 2063 6c61 7373 3d22 4d61 7468 4a61 7820   class="MathJax 
-00001fc0: 4374 7874 4d65 6e75 5f41 7474 6163 6865  CtxtMenu_Attache
-00001fd0: 645f 3022 206a 6178 3d22 4348 544d 4c22  d_0" jax="CHTML"
-00001fe0: 2074 6162 696e 6465 783d 2230 2220 6374   tabindex="0" ct
-00001ff0: 7874 6d65 6e75 5f63 6f75 6e74 6572 3d22  xtmenu_counter="
-00002000: 3422 2073 7479 6c65 3d22 666f 6e74 2d73  4" style="font-s
-00002010: 697a 653a 2031 3139 253b 2070 6f73 6974  ize: 119%; posit
-00002020: 696f 6e3a 2072 656c 6174 6976 653b 223e  ion: relative;">
-00002030: 3c6d 6a78 2d6d 6174 6820 636c 6173 733d  <mjx-math class=
-00002040: 224d 4a58 2d54 4558 2220 6172 6961 2d68  "MJX-TEX" aria-h
-00002050: 6964 6465 6e3d 2274 7275 6522 3e3c 6d6a  idden="true"><mj
-00002060: 782d 6d69 2063 6c61 7373 3d22 6d6a 782d  x-mi class="mjx-
-00002070: 6922 3e3c 6d6a 782d 6320 636c 6173 733d  i"><mjx-c class=
-00002080: 226d 6a78 2d63 3144 3434 3520 5445 582d  "mjx-c1D445 TEX-
-00002090: 4922 3e3c 2f6d 6a78 2d63 3e3c 2f6d 6a78  I"></mjx-c></mjx
-000020a0: 2d6d 693e 3c2f 6d6a 782d 6d61 7468 3e3c  -mi></mjx-math><
-000020b0: 6d6a 782d 6173 7369 7374 6976 652d 6d6d  mjx-assistive-mm
-000020c0: 6c20 756e 7365 6c65 6374 6162 6c65 3d22  l unselectable="
-000020d0: 6f6e 2220 6469 7370 6c61 793d 2269 6e6c  on" display="inl
-000020e0: 696e 6522 3e3c 6d61 7468 2078 6d6c 6e73  ine"><math xmlns
-000020f0: 3d22 6874 7470 3a2f 2f77 7777 2e77 332e  ="http://www.w3.
-00002100: 6f72 672f 3139 3938 2f4d 6174 682f 4d61  org/1998/Math/Ma
-00002110: 7468 4d4c 223e 3c6d 693e 523c 2f6d 693e  thML"><mi>R</mi>
-00002120: 3c2f 6d61 7468 3e3c 2f6d 6a78 2d61 7373  </math></mjx-ass
-00002130: 6973 7469 7665 2d6d 6d6c 3e3c 2f6d 6a78  istive-mml></mjx
-00002140: 2d63 6f6e 7461 696e 6572 3e3c 2f73 7061  -container></spa
-00002150: 6e3e 2074 6f20 3c73 7472 6f6e 673e 4765  n> to <strong>Ge
-00002160: 6e6f 6d65 3c2f 7374 726f 6e67 3e20 3c73  nome</strong> <s
-00002170: 7061 6e20 636c 6173 733d 226d 6174 6820  pan class="math 
-00002180: 6e6f 7472 616e 736c 6174 6520 6e6f 6869  notranslate nohi
-00002190: 6768 6c69 6768 7422 3e3c 6d6a 782d 636f  ghlight"><mjx-co
-000021a0: 6e74 6169 6e65 7220 636c 6173 733d 224d  ntainer class="M
-000021b0: 6174 684a 6178 2043 7478 744d 656e 755f  athJax CtxtMenu_
-000021c0: 4174 7461 6368 6564 5f30 2220 6a61 783d  Attached_0" jax=
-000021d0: 2243 4854 4d4c 2220 7461 6269 6e64 6578  "CHTML" tabindex
-000021e0: 3d22 3022 2063 7478 746d 656e 755f 636f  ="0" ctxtmenu_co
-000021f0: 756e 7465 723d 2235 2220 7374 796c 653d  unter="5" style=
-00002200: 2266 6f6e 742d 7369 7a65 3a20 3131 3925  "font-size: 119%
-00002210: 3b20 706f 7369 7469 6f6e 3a20 7265 6c61  ; position: rela
-00002220: 7469 7665 3b22 3e3c 6d6a 782d 6d61 7468  tive;"><mjx-math
-00002230: 2063 6c61 7373 3d22 4d4a 582d 5445 5822   class="MJX-TEX"
-00002240: 2061 7269 612d 6869 6464 656e 3d22 7472   aria-hidden="tr
-00002250: 7565 223e 3c6d 6a78 2d6d 6920 636c 6173  ue"><mjx-mi clas
-00002260: 733d 226d 6a78 2d69 223e 3c6d 6a78 2d63  s="mjx-i"><mjx-c
-00002270: 2063 6c61 7373 3d22 6d6a 782d 6331 4434   class="mjx-c1D4
-00002280: 3437 2054 4558 2d49 223e 3c2f 6d6a 782d  47 TEX-I"></mjx-
-00002290: 633e 3c2f 6d6a 782d 6d69 3e3c 2f6d 6a78  c></mjx-mi></mjx
-000022a0: 2d6d 6174 683e 3c6d 6a78 2d61 7373 6973  -math><mjx-assis
-000022b0: 7469 7665 2d6d 6d6c 2075 6e73 656c 6563  tive-mml unselec
-000022c0: 7461 626c 653d 226f 6e22 2064 6973 706c  table="on" displ
-000022d0: 6179 3d22 696e 6c69 6e65 223e 3c6d 6174  ay="inline"><mat
-000022e0: 6820 786d 6c6e 733d 2268 7474 703a 2f2f  h xmlns="http://
-000022f0: 7777 772e 7733 2e6f 7267 2f31 3939 382f  www.w3.org/1998/
-00002300: 4d61 7468 2f4d 6174 684d 4c22 3e3c 6d69  Math/MathML"><mi
-00002310: 3e54 3c2f 6d69 3e3c 2f6d 6174 683e 3c2f  >T</mi></math></
-00002320: 6d6a 782d 6173 7369 7374 6976 652d 6d6d  mjx-assistive-mm
-00002330: 6c3e 3c2f 6d6a 782d 636f 6e74 6169 6e65  l></mjx-containe
-00002340: 723e 3c2f 7370 616e 3e2c 2061 6e64 2067  r></span>, and g
-00002350: 656e 6572 6174 6520 6120 6e65 7720 616e  enerate a new an
-00002360: 6e6f 7461 7469 6f6e 2066 696c 6520 3c73  notation file <s
-00002370: 7472 6f6e 673e 416e 6e6f 7461 7469 6f6e  trong>Annotation
-00002380: 3c2f 7374 726f 6e67 3e20 3c73 7061 6e20  </strong> <span 
-00002390: 636c 6173 733d 226d 6174 6820 6e6f 7472  class="math notr
-000023a0: 616e 736c 6174 6520 6e6f 6869 6768 6c69  anslate nohighli
-000023b0: 6768 7422 3e3c 6d6a 782d 636f 6e74 6169  ght"><mjx-contai
-000023c0: 6e65 7220 636c 6173 733d 224d 6174 684a  ner class="MathJ
-000023d0: 6178 2043 7478 744d 656e 755f 4174 7461  ax CtxtMenu_Atta
-000023e0: 6368 6564 5f30 2220 6a61 783d 2243 4854  ched_0" jax="CHT
-000023f0: 4d4c 2220 7461 6269 6e64 6578 3d22 3022  ML" tabindex="0"
-00002400: 2063 7478 746d 656e 755f 636f 756e 7465   ctxtmenu_counte
-00002410: 723d 2236 2220 7374 796c 653d 2266 6f6e  r="6" style="fon
-00002420: 742d 7369 7a65 3a20 3131 3925 3b20 706f  t-size: 119%; po
-00002430: 7369 7469 6f6e 3a20 7265 6c61 7469 7665  sition: relative
-00002440: 3b22 3e3c 6d6a 782d 6d61 7468 2063 6c61  ;"><mjx-math cla
-00002450: 7373 3d22 4d4a 582d 5445 5822 2061 7269  ss="MJX-TEX" ari
-00002460: 612d 6869 6464 656e 3d22 7472 7565 223e  a-hidden="true">
-00002470: 3c6d 6a78 2d6d 7375 623e 3c6d 6a78 2d6d  <mjx-msub><mjx-m
-00002480: 6920 636c 6173 733d 226d 6a78 2d69 223e  i class="mjx-i">
-00002490: 3c6d 6a78 2d63 2063 6c61 7373 3d22 6d6a  <mjx-c class="mj
-000024a0: 782d 6331 4434 3437 2054 4558 2d49 223e  x-c1D447 TEX-I">
-000024b0: 3c2f 6d6a 782d 633e 3c2f 6d6a 782d 6d69  </mjx-c></mjx-mi
-000024c0: 3e3c 6d6a 782d 7363 7269 7074 2073 7479  ><mjx-script sty
-000024d0: 6c65 3d22 7665 7274 6963 616c 2d61 6c69  le="vertical-ali
-000024e0: 676e 3a20 2d30 2e31 3533 656d 3b20 6d61  gn: -0.153em; ma
-000024f0: 7267 696e 2d6c 6566 743a 202d 302e 3132  rgin-left: -0.12
-00002500: 656d 3b22 3e3c 6d6a 782d 6d69 2063 6c61  em;"><mjx-mi cla
-00002510: 7373 3d22 6d6a 782d 6922 2073 697a 653d  ss="mjx-i" size=
-00002520: 2273 223e 3c6d 6a78 2d63 2063 6c61 7373  "s"><mjx-c class
-00002530: 3d22 6d6a 782d 6331 4434 3334 2054 4558  ="mjx-c1D434 TEX
-00002540: 2d49 223e 3c2f 6d6a 782d 633e 3c2f 6d6a  -I"></mjx-c></mj
-00002550: 782d 6d69 3e3c 2f6d 6a78 2d73 6372 6970  x-mi></mjx-scrip
-00002560: 743e 3c2f 6d6a 782d 6d73 7562 3e3c 2f6d  t></mjx-msub></m
-00002570: 6a78 2d6d 6174 683e 3c6d 6a78 2d61 7373  jx-math><mjx-ass
-00002580: 6973 7469 7665 2d6d 6d6c 2075 6e73 656c  istive-mml unsel
-00002590: 6563 7461 626c 653d 226f 6e22 2064 6973  ectable="on" dis
-000025a0: 706c 6179 3d22 696e 6c69 6e65 223e 3c6d  play="inline"><m
-000025b0: 6174 6820 786d 6c6e 733d 2268 7474 703a  ath xmlns="http:
-000025c0: 2f2f 7777 772e 7733 2e6f 7267 2f31 3939  //www.w3.org/199
-000025d0: 382f 4d61 7468 2f4d 6174 684d 4c22 3e3c  8/Math/MathML"><
-000025e0: 6d73 7562 3e3c 6d69 3e54 3c2f 6d69 3e3c  msub><mi>T</mi><
-000025f0: 6d69 3e41 3c2f 6d69 3e3c 2f6d 7375 623e  mi>A</mi></msub>
-00002600: 3c2f 6d61 7468 3e3c 2f6d 6a78 2d61 7373  </math></mjx-ass
-00002610: 6973 7469 7665 2d6d 6d6c 3e3c 2f6d 6a78  istive-mml></mjx
-00002620: 2d63 6f6e 7461 696e 6572 3e3c 2f73 7061  -container></spa
-00002630: 6e3e 2e20 4120 7369 6d70 6c65 2069 6c6c  n>. A simple ill
-00002640: 7573 7472 6174 696f 6e20 6f66 2074 6865  ustration of the
-00002650: 206c 6966 742d 6f76 6572 2070 726f 626c   lift-over probl
-00002660: 656d 2069 7320 7368 6f77 6e20 696e 203c  em is shown in <
-00002670: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
-00002680: 6365 2069 6e74 6572 6e61 6c22 2068 7265  ce internal" hre
-00002690: 663d 2223 6c69 6674 6f76 6572 2d69 6c6c  f="#liftover-ill
-000026a0: 7573 7472 6174 696f 6e22 3e3c 7370 616e  ustration"><span
-000026b0: 2063 6c61 7373 3d22 7374 6420 7374 642d   class="std std-
-000026c0: 6e75 6d72 6566 223e 4669 6775 7265 2031  numref">Figure 1
-000026d0: 3c2f 7370 616e 3e3c 2f61 3e2e 3c2f 703e  </span></a>.</p>
-000026e0: 0a3c 6669 6775 7265 2063 6c61 7373 3d22  .<figure class="
-000026f0: 616c 6967 6e2d 6365 6e74 6572 2220 6964  align-center" id
-00002700: 3d22 6964 3522 3e0a 3c73 7061 6e20 6964  ="id5">.<span id
-00002710: 3d22 6c69 6674 6f76 6572 2d69 6c6c 7573  ="liftover-illus
-00002720: 7472 6174 696f 6e22 3e3c 2f73 7061 6e3e  tration"></span>
-00002730: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
-00002740: 6e63 6520 696e 7465 726e 616c 2069 6d61  nce internal ima
-00002750: 6765 2d72 6566 6572 656e 6365 2220 6872  ge-reference" hr
-00002760: 6566 3d22 6772 6170 6869 6373 2f6c 6966  ef="graphics/lif
-00002770: 746f 7665 725f 696c 6c75 7374 7261 7469  tover_illustrati
-00002780: 6f6e 2e67 6966 223e 3c69 6d67 2061 6c74  on.gif"><img alt
-00002790: 3d22 6772 6170 6869 6373 2f6c 6966 746f  ="graphics/lifto
-000027a0: 7665 725f 696c 6c75 7374 7261 7469 6f6e  ver_illustration
-000027b0: 2e67 6966 2220 7372 633d 2267 7261 7068  .gif" src="graph
-000027c0: 6963 732f 6c69 6674 6f76 6572 5f69 6c6c  ics/liftover_ill
-000027d0: 7573 7472 6174 696f 6e2e 6769 6622 2073  ustration.gif" s
-000027e0: 7479 6c65 3d22 7769 6474 683a 2036 3732  tyle="width: 672
-000027f0: 2e35 7078 3b20 6865 6967 6874 3a20 3237  .5px; height: 27
-00002800: 302e 3070 783b 223e 3c2f 613e 0a3c 6669  0.0px;"></a>.<fi
-00002810: 6763 6170 7469 6f6e 3e0a 3c70 3e3c 7370  gcaption>.<p><sp
-00002820: 616e 2063 6c61 7373 3d22 6361 7074 696f  an class="captio
-00002830: 6e2d 6e75 6d62 6572 223e 4669 6775 7265  n-number">Figure
-00002840: 2031 203c 2f73 7061 6e3e 3c73 7061 6e20   1 </span><span 
-00002850: 636c 6173 733d 2263 6170 7469 6f6e 2d74  class="caption-t
-00002860: 6578 7422 3e49 6c6c 7573 7472 6174 696f  ext">Illustratio
-00002870: 6e20 6f66 2074 6865 206c 6966 742d 6f76  n of the lift-ov
-00002880: 6572 2070 726f 626c 656d 2e20 5468 6520  er problem. The 
-00002890: 616e 6e6f 7461 7469 6f6e 2066 696c 6520  annotation file 
-000028a0: 6672 6f6d 2074 6865 2072 6566 6572 656e  from the referen
-000028b0: 6365 2067 656e 6f6d 6520 2874 6f70 2920  ce genome (top) 
-000028c0: 6973 206c 6966 7465 6420 6f76 6572 2074  is lifted over t
-000028d0: 6f20 7468 6520 7461 7267 6574 2067 656e  o the target gen
-000028e0: 6f6d 6520 2862 6f74 746f 6d29 2e3c 2f73  ome (bottom).</s
-000028f0: 7061 6e3e 3c61 2063 6c61 7373 3d22 6865  pan><a class="he
-00002900: 6164 6572 6c69 6e6b 2220 6872 6566 3d22  aderlink" href="
-00002910: 2369 6435 2220 7469 746c 653d 2250 6572  #id5" title="Per
-00002920: 6d61 6c69 6e6b 2074 6f20 7468 6973 2069  malink to this i
-00002930: 6d61 6765 223e 233c 2f61 3e3c 2f70 3e0a  mage">#</a></p>.
-00002940: 3c2f 6669 6763 6170 7469 6f6e 3e0a 3c2f  </figcaption>.</
-00002950: 6669 6775 7265 3e0a 3c64 6976 2063 6c61  figure>.<div cla
-00002960: 7373 3d22 6c69 6e65 2d62 6c6f 636b 223e  ss="line-block">
-00002970: 0a3c 6469 7620 636c 6173 733d 226c 696e  .<div class="lin
-00002980: 6522 3e3c 6272 3e3c 2f64 6976 3e0a 3c2f  e"><br></div>.</
-00002990: 6469 763e 0a3c 703e 4c69 6674 4f6e 2069  div>.<p>LiftOn i
-000029a0: 7320 7468 6520 6265 7374 2074 6f6f 6c20  s the best tool 
-000029b0: 746f 2068 656c 7020 796f 7520 736f 6c76  to help you solv
-000029c0: 6520 7468 6973 2070 726f 626c 656d 2120  e this problem! 
-000029d0: 4c69 6674 4f6e 2065 6d70 6c6f 7973 2061  LiftOn employs a
-000029e0: 2074 776f 2d73 7465 7020 3c61 2063 6c61   two-step <a cla
-000029f0: 7373 3d22 7265 6665 7265 6e63 6520 696e  ss="reference in
-00002a00: 7465 726e 616c 2220 6872 6566 3d22 6874  ternal" href="ht
-00002a10: 7470 3a2f 2f63 6362 2e6a 6875 2e65 6475  tp://ccb.jhu.edu
-00002a20: 2f6c 6966 746f 6e2f 636f 6e74 656e 742f  /lifton/content/
-00002a30: 6265 6869 6e64 5f73 6365 6e65 732e 6874  behind_scenes.ht
-00002a40: 6d6c 2370 726f 7465 696e 2d6d 6178 696d  ml#protein-maxim
-00002a50: 697a 6174 696f 6e2d 616c 676f 7269 7468  ization-algorith
-00002a60: 6d22 3e3c 7370 616e 2063 6c61 7373 3d22  m"><span class="
-00002a70: 7374 6420 7374 642d 7265 6622 3e70 726f  std std-ref">pro
-00002a80: 7465 696e 206d 6178 696d 697a 6174 696f  tein maximizatio
-00002a90: 6e20 616c 676f 7269 7468 6d3c 2f73 7061  n algorithm</spa
-00002aa0: 6e3e 3c2f 613e 2028 504d 2061 6c67 6f72  n></a> (PM algor
-00002ab0: 6974 686d 292e 3c2f 703e 0a3c 6f6c 2063  ithm).</p>.<ol c
-00002ac0: 6c61 7373 3d22 6172 6162 6963 2073 696d  lass="arabic sim
-00002ad0: 706c 6522 3e0a 3c6c 693e 3c70 3e54 6865  ple">.<li><p>The
-00002ae0: 2066 6972 7374 206d 6f64 756c 6520 6973   first module is
-00002af0: 2074 6865 203c 656d 3e63 6861 696e 696e   the <em>chainin
-00002b00: 6720 616c 676f 7269 7468 6d3c 2f65 6d3e  g algorithm</em>
-00002b10: 2e20 4974 2073 7461 7274 7320 6279 2065  . It starts by e
-00002b20: 7874 7261 6374 696e 6720 7072 6f74 6569  xtracting protei
-00002b30: 6e20 7365 7175 656e 6365 7320 616e 6e6f  n sequences anno
-00002b40: 7461 7465 6420 6279 204c 6966 746f 6666  tated by Liftoff
-00002b50: 2061 6e64 206d 696e 6970 726f 742e 204c   and miniprot. L
-00002b60: 6966 744f 6e20 7468 656e 2061 6c69 676e  iftOn then align
-00002b70: 7320 7468 6573 6520 7365 7175 656e 6365  s these sequence
-00002b80: 7320 746f 2066 756c 6c2d 6c65 6e67 7468  s to full-length
-00002b90: 2072 6566 6572 656e 6365 2070 726f 7465   reference prote
-00002ba0: 696e 732e 2046 6f72 2065 6163 6820 6765  ins. For each ge
-00002bb0: 6e65 206c 6f63 7573 2c20 4c69 6674 4f6e  ne locus, LiftOn
-00002bc0: 2063 6f6d 7061 7265 7320 6561 6368 2073   compares each s
-00002bd0: 6563 7469 6f6e 206f 6620 7468 6520 7072  ection of the pr
-00002be0: 6f74 6569 6e20 616c 6967 6e6d 656e 7473  otein alignments
-00002bf0: 2066 726f 6d20 4c69 6674 6f66 6620 616e   from Liftoff an
-00002c00: 6420 6d69 6e69 7072 6f74 2c20 6368 6169  d miniprot, chai
-00002c10: 6e69 6e67 2074 6f67 6574 6865 7220 7468  ning together th
-00002c20: 6520 6265 7374 2063 6f6d 6269 6e61 7469  e best combinati
-00002c30: 6f6e 732e 3c2f 703e 3c2f 6c69 3e0a 3c6c  ons.</p></li>.<l
-00002c40: 693e 3c70 3e54 6865 2073 6563 6f6e 6420  i><p>The second 
-00002c50: 6d6f 6475 6c65 2069 7320 7468 6520 3c65  module is the <e
-00002c60: 6d3e 6f70 656e 2d72 6561 6469 6e67 2066  m>open-reading f
-00002c70: 7261 6d65 2073 6561 7263 6820 284f 5246  rame search (ORF
-00002c80: 2073 6561 7263 6829 2061 6c67 6f72 6974   search) algorit
-00002c90: 686d 3c2f 656d 3e2e 2049 6e20 7468 6520  hm</em>. In the 
-00002ca0: 6361 7365 206f 6620 7472 756e 6361 7465  case of truncate
-00002cb0: 6420 7072 6f74 6569 6e2d 636f 6469 6e67  d protein-coding
-00002cc0: 2074 7261 6e73 6372 6970 7473 2c20 7468   transcripts, th
-00002cd0: 6973 2061 6c67 6f72 6974 686d 2065 7861  is algorithm exa
-00002ce0: 6d69 6e65 7320 616c 7465 726e 6174 6976  mines alternativ
-00002cf0: 6520 6672 616d 6573 2074 6f20 6964 656e  e frames to iden
-00002d00: 7469 6679 2074 6865 204f 5246 2074 6861  tify the ORF tha
-00002d10: 7420 7072 6f64 7563 6573 2074 6865 206c  t produces the l
-00002d20: 6f6e 6765 7374 206d 6174 6368 2077 6974  ongest match wit
-00002d30: 6820 7468 6520 7265 6665 7265 6e63 6520  h the reference 
-00002d40: 7072 6f74 6569 6e2e 3c2f 703e 3c2f 6c69  protein.</p></li
-00002d50: 3e0a 3c2f 6f6c 3e0a 3c75 6c20 636c 6173  >.</ol>.<ul clas
-00002d60: 733d 2273 696d 706c 6522 3e0a 3c6c 693e  s="simple">.<li>
-00002d70: 3c64 6c20 636c 6173 733d 2273 696d 706c  <dl class="simpl
-00002d80: 6522 3e0a 3c64 743e 3c73 7472 6f6e 673e  e">.<dt><strong>
-00002d90: 496e 7075 743c 2f73 7472 6f6e 673e 3a3c  Input</strong>:<
-00002da0: 2f64 743e 3c64 643e 3c6f 6c20 636c 6173  /dt><dd><ol clas
-00002db0: 733d 2261 7261 6269 6320 7369 6d70 6c65  s="arabic simple
-00002dc0: 223e 0a3c 6c69 3e3c 703e 7461 7267 6574  ">.<li><p>target
-00002dd0: 203c 7374 726f 6e67 3e47 656e 6f6d 653c   <strong>Genome<
-00002de0: 2f73 7472 6f6e 673e 203c 7370 616e 2063  /strong> <span c
-00002df0: 6c61 7373 3d22 6d61 7468 206e 6f74 7261  lass="math notra
-00002e00: 6e73 6c61 7465 206e 6f68 6967 686c 6967  nslate nohighlig
-00002e10: 6874 223e 3c6d 6a78 2d63 6f6e 7461 696e  ht"><mjx-contain
-00002e20: 6572 2063 6c61 7373 3d22 4d61 7468 4a61  er class="MathJa
-00002e30: 7820 4374 7874 4d65 6e75 5f41 7474 6163  x CtxtMenu_Attac
-00002e40: 6865 645f 3022 206a 6178 3d22 4348 544d  hed_0" jax="CHTM
-00002e50: 4c22 2074 6162 696e 6465 783d 2230 2220  L" tabindex="0" 
-00002e60: 6374 7874 6d65 6e75 5f63 6f75 6e74 6572  ctxtmenu_counter
-00002e70: 3d22 3722 2073 7479 6c65 3d22 666f 6e74  ="7" style="font
-00002e80: 2d73 697a 653a 2031 3139 253b 2070 6f73  -size: 119%; pos
-00002e90: 6974 696f 6e3a 2072 656c 6174 6976 653b  ition: relative;
-00002ea0: 223e 3c6d 6a78 2d6d 6174 6820 636c 6173  "><mjx-math clas
-00002eb0: 733d 224d 4a58 2d54 4558 2220 6172 6961  s="MJX-TEX" aria
-00002ec0: 2d68 6964 6465 6e3d 2274 7275 6522 3e3c  -hidden="true"><
-00002ed0: 6d6a 782d 6d69 2063 6c61 7373 3d22 6d6a  mjx-mi class="mj
-00002ee0: 782d 6922 3e3c 6d6a 782d 6320 636c 6173  x-i"><mjx-c clas
-00002ef0: 733d 226d 6a78 2d63 3144 3434 3720 5445  s="mjx-c1D447 TE
-00002f00: 582d 4922 3e3c 2f6d 6a78 2d63 3e3c 2f6d  X-I"></mjx-c></m
-00002f10: 6a78 2d6d 693e 3c2f 6d6a 782d 6d61 7468  jx-mi></mjx-math
-00002f20: 3e3c 6d6a 782d 6173 7369 7374 6976 652d  ><mjx-assistive-
-00002f30: 6d6d 6c20 756e 7365 6c65 6374 6162 6c65  mml unselectable
-00002f40: 3d22 6f6e 2220 6469 7370 6c61 793d 2269  ="on" display="i
-00002f50: 6e6c 696e 6522 3e3c 6d61 7468 2078 6d6c  nline"><math xml
-00002f60: 6e73 3d22 6874 7470 3a2f 2f77 7777 2e77  ns="http://www.w
-00002f70: 332e 6f72 672f 3139 3938 2f4d 6174 682f  3.org/1998/Math/
-00002f80: 4d61 7468 4d4c 223e 3c6d 693e 543c 2f6d  MathML"><mi>T</m
-00002f90: 693e 3c2f 6d61 7468 3e3c 2f6d 6a78 2d61  i></math></mjx-a
-00002fa0: 7373 6973 7469 7665 2d6d 6d6c 3e3c 2f6d  ssistive-mml></m
-00002fb0: 6a78 2d63 6f6e 7461 696e 6572 3e3c 2f73  jx-container></s
-00002fc0: 7061 6e3e 2069 6e20 4641 5354 412e 3c2f  pan> in FASTA.</
-00002fd0: 703e 3c2f 6c69 3e0a 3c6c 693e 3c70 3e72  p></li>.<li><p>r
-00002fe0: 6566 6572 656e 6365 203c 7374 726f 6e67  eference <strong
-00002ff0: 3e47 656e 6f6d 653c 2f73 7472 6f6e 673e  >Genome</strong>
-00003000: 203c 7370 616e 2063 6c61 7373 3d22 6d61   <span class="ma
-00003010: 7468 206e 6f74 7261 6e73 6c61 7465 206e  th notranslate n
-00003020: 6f68 6967 686c 6967 6874 223e 3c6d 6a78  ohighlight"><mjx
-00003030: 2d63 6f6e 7461 696e 6572 2063 6c61 7373  -container class
-00003040: 3d22 4d61 7468 4a61 7820 4374 7874 4d65  ="MathJax CtxtMe
-00003050: 6e75 5f41 7474 6163 6865 645f 3022 206a  nu_Attached_0" j
-00003060: 6178 3d22 4348 544d 4c22 2074 6162 696e  ax="CHTML" tabin
-00003070: 6465 783d 2230 2220 6374 7874 6d65 6e75  dex="0" ctxtmenu
-00003080: 5f63 6f75 6e74 6572 3d22 3822 2073 7479  _counter="8" sty
-00003090: 6c65 3d22 666f 6e74 2d73 697a 653a 2031  le="font-size: 1
-000030a0: 3139 253b 2070 6f73 6974 696f 6e3a 2072  19%; position: r
-000030b0: 656c 6174 6976 653b 223e 3c6d 6a78 2d6d  elative;"><mjx-m
-000030c0: 6174 6820 636c 6173 733d 224d 4a58 2d54  ath class="MJX-T
-000030d0: 4558 2220 6172 6961 2d68 6964 6465 6e3d  EX" aria-hidden=
-000030e0: 2274 7275 6522 3e3c 6d6a 782d 6d69 2063  "true"><mjx-mi c
-000030f0: 6c61 7373 3d22 6d6a 782d 6922 3e3c 6d6a  lass="mjx-i"><mj
-00003100: 782d 6320 636c 6173 733d 226d 6a78 2d63  x-c class="mjx-c
-00003110: 3144 3434 3520 5445 582d 4922 3e3c 2f6d  1D445 TEX-I"></m
-00003120: 6a78 2d63 3e3c 2f6d 6a78 2d6d 693e 3c2f  jx-c></mjx-mi></
-00003130: 6d6a 782d 6d61 7468 3e3c 6d6a 782d 6173  mjx-math><mjx-as
-00003140: 7369 7374 6976 652d 6d6d 6c20 756e 7365  sistive-mml unse
-00003150: 6c65 6374 6162 6c65 3d22 6f6e 2220 6469  lectable="on" di
-00003160: 7370 6c61 793d 2269 6e6c 696e 6522 3e3c  splay="inline"><
-00003170: 6d61 7468 2078 6d6c 6e73 3d22 6874 7470  math xmlns="http
-00003180: 3a2f 2f77 7777 2e77 332e 6f72 672f 3139  ://www.w3.org/19
-00003190: 3938 2f4d 6174 682f 4d61 7468 4d4c 223e  98/Math/MathML">
-000031a0: 3c6d 693e 523c 2f6d 693e 3c2f 6d61 7468  <mi>R</mi></math
-000031b0: 3e3c 2f6d 6a78 2d61 7373 6973 7469 7665  ></mjx-assistive
-000031c0: 2d6d 6d6c 3e3c 2f6d 6a78 2d63 6f6e 7461  -mml></mjx-conta
-000031d0: 696e 6572 3e3c 2f73 7061 6e3e 2069 6e20  iner></span> in 
-000031e0: 4641 5354 413c 2f70 3e3c 2f6c 693e 0a3c  FASTA</p></li>.<
-000031f0: 6c69 3e3c 703e 7265 6665 7265 6e63 6520  li><p>reference 
-00003200: 3c73 7472 6f6e 673e 416e 6e6f 7461 7469  <strong>Annotati
-00003210: 6f6e 3c2f 7374 726f 6e67 3e20 3c73 7061  on</strong> <spa
-00003220: 6e20 636c 6173 733d 226d 6174 6820 6e6f  n class="math no
-00003230: 7472 616e 736c 6174 6520 6e6f 6869 6768  translate nohigh
-00003240: 6c69 6768 7422 3e3c 6d6a 782d 636f 6e74  light"><mjx-cont
-00003250: 6169 6e65 7220 636c 6173 733d 224d 6174  ainer class="Mat
-00003260: 684a 6178 2043 7478 744d 656e 755f 4174  hJax CtxtMenu_At
-00003270: 7461 6368 6564 5f30 2220 6a61 783d 2243  tached_0" jax="C
-00003280: 4854 4d4c 2220 7461 6269 6e64 6578 3d22  HTML" tabindex="
-00003290: 3022 2063 7478 746d 656e 755f 636f 756e  0" ctxtmenu_coun
-000032a0: 7465 723d 2239 2220 7374 796c 653d 2266  ter="9" style="f
-000032b0: 6f6e 742d 7369 7a65 3a20 3131 3925 3b20  ont-size: 119%; 
-000032c0: 706f 7369 7469 6f6e 3a20 7265 6c61 7469  position: relati
-000032d0: 7665 3b22 3e3c 6d6a 782d 6d61 7468 2063  ve;"><mjx-math c
-000032e0: 6c61 7373 3d22 4d4a 582d 5445 5822 2061  lass="MJX-TEX" a
-000032f0: 7269 612d 6869 6464 656e 3d22 7472 7565  ria-hidden="true
-00003300: 223e 3c6d 6a78 2d6d 7375 623e 3c6d 6a78  "><mjx-msub><mjx
-00003310: 2d6d 6920 636c 6173 733d 226d 6a78 2d69  -mi class="mjx-i
-00003320: 223e 3c6d 6a78 2d63 2063 6c61 7373 3d22  "><mjx-c class="
-00003330: 6d6a 782d 6331 4434 3435 2054 4558 2d49  mjx-c1D445 TEX-I
-00003340: 223e 3c2f 6d6a 782d 633e 3c2f 6d6a 782d  "></mjx-c></mjx-
-00003350: 6d69 3e3c 6d6a 782d 7363 7269 7074 2073  mi><mjx-script s
-00003360: 7479 6c65 3d22 7665 7274 6963 616c 2d61  tyle="vertical-a
-00003370: 6c69 676e 3a20 2d30 2e31 3533 656d 3b22  lign: -0.153em;"
-00003380: 3e3c 6d6a 782d 6d69 2063 6c61 7373 3d22  ><mjx-mi class="
-00003390: 6d6a 782d 6922 2073 697a 653d 2273 223e  mjx-i" size="s">
-000033a0: 3c6d 6a78 2d63 2063 6c61 7373 3d22 6d6a  <mjx-c class="mj
-000033b0: 782d 6331 4434 3334 2054 4558 2d49 223e  x-c1D434 TEX-I">
-000033c0: 3c2f 6d6a 782d 633e 3c2f 6d6a 782d 6d69  </mjx-c></mjx-mi
-000033d0: 3e3c 2f6d 6a78 2d73 6372 6970 743e 3c2f  ></mjx-script></
-000033e0: 6d6a 782d 6d73 7562 3e3c 2f6d 6a78 2d6d  mjx-msub></mjx-m
-000033f0: 6174 683e 3c6d 6a78 2d61 7373 6973 7469  ath><mjx-assisti
-00003400: 7665 2d6d 6d6c 2075 6e73 656c 6563 7461  ve-mml unselecta
-00003410: 626c 653d 226f 6e22 2064 6973 706c 6179  ble="on" display
-00003420: 3d22 696e 6c69 6e65 223e 3c6d 6174 6820  ="inline"><math 
-00003430: 786d 6c6e 733d 2268 7474 703a 2f2f 7777  xmlns="http://ww
-00003440: 772e 7733 2e6f 7267 2f31 3939 382f 4d61  w.w3.org/1998/Ma
-00003450: 7468 2f4d 6174 684d 4c22 3e3c 6d73 7562  th/MathML"><msub
-00003460: 3e3c 6d69 3e52 3c2f 6d69 3e3c 6d69 3e41  ><mi>R</mi><mi>A
-00003470: 3c2f 6d69 3e3c 2f6d 7375 623e 3c2f 6d61  </mi></msub></ma
-00003480: 7468 3e3c 2f6d 6a78 2d61 7373 6973 7469  th></mjx-assisti
-00003490: 7665 2d6d 6d6c 3e3c 2f6d 6a78 2d63 6f6e  ve-mml></mjx-con
-000034a0: 7461 696e 6572 3e3c 2f73 7061 6e3e 2069  tainer></span> i
-000034b0: 6e20 4746 4633 3c2f 703e 3c2f 6c69 3e0a  n GFF3</p></li>.
-000034c0: 3c2f 6f6c 3e0a 3c2f 6464 3e0a 3c2f 646c  </ol>.</dd>.</dl
-000034d0: 3e0a 3c2f 6c69 3e0a 3c6c 693e 3c64 6c20  >.</li>.<li><dl 
-000034e0: 636c 6173 733d 2273 696d 706c 6522 3e0a  class="simple">.
-000034f0: 3c64 743e 3c73 7472 6f6e 673e 4f75 7470  <dt><strong>Outp
-00003500: 7574 3c2f 7374 726f 6e67 3e3a 3c2f 6474  ut</strong>:</dt
-00003510: 3e3c 6464 3e3c 6f6c 2063 6c61 7373 3d22  ><dd><ol class="
-00003520: 6172 6162 6963 2073 696d 706c 6522 3e0a  arabic simple">.
-00003530: 3c6c 693e 3c70 3e4c 6966 744f 6e20 616e  <li><p>LiftOn an
-00003540: 6e6f 7461 7469 6f6e 2066 696c 652c 203c  notation file, <
-00003550: 7374 726f 6e67 3e41 6e6e 6f74 6174 696f  strong>Annotatio
-00003560: 6e3c 2f73 7472 6f6e 673e 203c 7370 616e  n</strong> <span
-00003570: 2063 6c61 7373 3d22 6d61 7468 206e 6f74   class="math not
-00003580: 7261 6e73 6c61 7465 206e 6f68 6967 686c  ranslate nohighl
-00003590: 6967 6874 223e 3c6d 6a78 2d63 6f6e 7461  ight"><mjx-conta
-000035a0: 696e 6572 2063 6c61 7373 3d22 4d61 7468  iner class="Math
-000035b0: 4a61 7820 4374 7874 4d65 6e75 5f41 7474  Jax CtxtMenu_Att
-000035c0: 6163 6865 645f 3022 206a 6178 3d22 4348  ached_0" jax="CH
-000035d0: 544d 4c22 2074 6162 696e 6465 783d 2230  TML" tabindex="0
-000035e0: 2220 6374 7874 6d65 6e75 5f63 6f75 6e74  " ctxtmenu_count
-000035f0: 6572 3d22 3130 2220 7374 796c 653d 2266  er="10" style="f
-00003600: 6f6e 742d 7369 7a65 3a20 3131 3925 3b20  ont-size: 119%; 
-00003610: 706f 7369 7469 6f6e 3a20 7265 6c61 7469  position: relati
-00003620: 7665 3b22 3e3c 6d6a 782d 6d61 7468 2063  ve;"><mjx-math c
-00003630: 6c61 7373 3d22 4d4a 582d 5445 5822 2061  lass="MJX-TEX" a
-00003640: 7269 612d 6869 6464 656e 3d22 7472 7565  ria-hidden="true
-00003650: 223e 3c6d 6a78 2d6d 7375 623e 3c6d 6a78  "><mjx-msub><mjx
-00003660: 2d6d 6920 636c 6173 733d 226d 6a78 2d69  -mi class="mjx-i
-00003670: 223e 3c6d 6a78 2d63 2063 6c61 7373 3d22  "><mjx-c class="
-00003680: 6d6a 782d 6331 4434 3437 2054 4558 2d49  mjx-c1D447 TEX-I
-00003690: 223e 3c2f 6d6a 782d 633e 3c2f 6d6a 782d  "></mjx-c></mjx-
-000036a0: 6d69 3e3c 6d6a 782d 7363 7269 7074 2073  mi><mjx-script s
-000036b0: 7479 6c65 3d22 7665 7274 6963 616c 2d61  tyle="vertical-a
-000036c0: 6c69 676e 3a20 2d30 2e31 3533 656d 3b20  lign: -0.153em; 
-000036d0: 6d61 7267 696e 2d6c 6566 743a 202d 302e  margin-left: -0.
-000036e0: 3132 656d 3b22 3e3c 6d6a 782d 6d69 2063  12em;"><mjx-mi c
-000036f0: 6c61 7373 3d22 6d6a 782d 6922 2073 697a  lass="mjx-i" siz
-00003700: 653d 2273 223e 3c6d 6a78 2d63 2063 6c61  e="s"><mjx-c cla
-00003710: 7373 3d22 6d6a 782d 6331 4434 3334 2054  ss="mjx-c1D434 T
-00003720: 4558 2d49 223e 3c2f 6d6a 782d 633e 3c2f  EX-I"></mjx-c></
-00003730: 6d6a 782d 6d69 3e3c 2f6d 6a78 2d73 6372  mjx-mi></mjx-scr
-00003740: 6970 743e 3c2f 6d6a 782d 6d73 7562 3e3c  ipt></mjx-msub><
-00003750: 2f6d 6a78 2d6d 6174 683e 3c6d 6a78 2d61  /mjx-math><mjx-a
-00003760: 7373 6973 7469 7665 2d6d 6d6c 2075 6e73  ssistive-mml uns
-00003770: 656c 6563 7461 626c 653d 226f 6e22 2064  electable="on" d
-00003780: 6973 706c 6179 3d22 696e 6c69 6e65 223e  isplay="inline">
-00003790: 3c6d 6174 6820 786d 6c6e 733d 2268 7474  <math xmlns="htt
-000037a0: 703a 2f2f 7777 772e 7733 2e6f 7267 2f31  p://www.w3.org/1
-000037b0: 3939 382f 4d61 7468 2f4d 6174 684d 4c22  998/Math/MathML"
-000037c0: 3e3c 6d73 7562 3e3c 6d69 3e54 3c2f 6d69  ><msub><mi>T</mi
-000037d0: 3e3c 6d69 3e41 3c2f 6d69 3e3c 2f6d 7375  ><mi>A</mi></msu
-000037e0: 623e 3c2f 6d61 7468 3e3c 2f6d 6a78 2d61  b></math></mjx-a
-000037f0: 7373 6973 7469 7665 2d6d 6d6c 3e3c 2f6d  ssistive-mml></m
-00003800: 6a78 2d63 6f6e 7461 696e 6572 3e3c 2f73  jx-container></s
-00003810: 7061 6e3e 2c20 696e 2047 4646 333c 2f70  pan>, in GFF3</p
-00003820: 3e3c 2f6c 693e 0a3c 6c69 3e3c 703e 5072  ></li>.<li><p>Pr
-00003830: 6f74 6569 6e20 7365 7175 656e 6365 2069  otein sequence i
-00003840: 6465 6e74 6974 6965 7320 2661 6d70 3b20  dentities &amp; 
-00003850: 6d75 7461 7469 6f6e 2074 7970 6573 3c2f  mutation types</
-00003860: 703e 3c2f 6c69 3e0a 3c6c 693e 3c70 3e46  p></li>.<li><p>F
-00003870: 6561 7475 7265 7320 7769 7468 2065 7874  eatures with ext
-00003880: 7261 2063 6f70 6965 733c 2f70 3e3c 2f6c  ra copies</p></l
-00003890: 693e 0a3c 6c69 3e3c 703e 556e 6d61 7070  i>.<li><p>Unmapp
-000038a0: 6564 2066 6561 7475 7265 733c 2f70 3e3c  ed features</p><
-000038b0: 2f6c 693e 0a3c 2f6f 6c3e 0a3c 2f64 643e  /li>.</ol>.</dd>
-000038c0: 0a3c 2f64 6c3e 0a3c 2f6c 693e 0a3c 2f75  .</dl>.</li>.</u
-000038d0: 6c3e 0a3c 6469 7620 636c 6173 733d 226c  l>.<div class="l
-000038e0: 696e 652d 626c 6f63 6b22 3e0a 3c64 6976  ine-block">.<div
-000038f0: 2063 6c61 7373 3d22 6c69 6e65 223e 3c62   class="line"><b
-00003900: 723e 3c2f 6469 763e 0a3c 2f64 6976 3e0a  r></div>.</div>.
-00003910: 3c2f 7365 6374 696f 6e3e 0a3c 7365 6374  </section>.<sect
-00003920: 696f 6e20 6964 3d22 6c69 6674 6f6e 2d73  ion id="lifton-s
-00003930: 2d6c 696d 6974 6174 696f 6e22 2063 6c61  -limitation" cla
-00003940: 7373 3d22 6163 7469 7665 223e 0a3c 6832  ss="active">.<h2
-00003950: 3e4c 6966 744f 6e27 7320 6c69 6d69 7461  >LiftOn's limita
-00003960: 7469 6f6e 3c61 2063 6c61 7373 3d22 6865  tion<a class="he
-00003970: 6164 6572 6c69 6e6b 2220 6872 6566 3d22  aderlink" href="
-00003980: 236c 6966 746f 6e2d 732d 6c69 6d69 7461  #lifton-s-limita
-00003990: 7469 6f6e 2220 7469 746c 653d 2250 6572  tion" title="Per
-000039a0: 6d61 6c69 6e6b 2074 6f20 7468 6973 2068  malink to this h
-000039b0: 6561 6469 6e67 223e 233c 2f61 3e3c 2f68  eading">#</a></h
-000039c0: 323e 0a3c 703e 4c69 6674 4f6e 2773 203c  2>.<p>LiftOn's <
-000039d0: 656d 3e63 6861 696e 696e 6720 616c 676f  em>chaining algo
-000039e0: 7269 7468 6d3c 2f65 6d3e 2063 7572 7265  rithm</em> curre
-000039f0: 6e74 6c79 206f 6e6c 7920 7574 696c 697a  ntly only utiliz
-00003a00: 6573 206d 696e 6970 726f 7420 616c 6967  es miniprot alig
-00003a10: 6e6d 656e 7420 7265 7375 6c74 7320 746f  nment results to
-00003a20: 2066 6978 2074 6865 204c 6966 746f 6666   fix the Liftoff
-00003a30: 2061 6e6e 6f74 6174 696f 6e2e 2048 6f77   annotation. How
-00003a40: 6576 6572 2c20 6974 2063 616e 2062 6520  ever, it can be 
-00003a50: 6578 7465 6e64 6564 2074 6f20 6368 6169  extended to chai
-00003a60: 6e20 746f 6765 7468 6572 206d 756c 7469  n together multi
-00003a70: 706c 6520 7072 6f74 6569 6e2d 6261 7365  ple protein-base
-00003a80: 6420 616e 6e6f 7461 7469 6f6e 2066 696c  d annotation fil
-00003a90: 6573 206f 7220 6161 7365 6d62 6c65 6420  es or aasembled 
-00003aa0: 524e 412d 5365 7120 7472 616e 7363 7269  RNA-Seq transcri
-00003ab0: 7074 732e 3c2f 703e 0a3c 703e 444e 412d  pts.</p>.<p>DNA-
-00003ac0: 2061 6e64 2070 726f 7465 696e 2d62 6173   and protein-bas
-00003ad0: 6564 206d 6574 686f 6473 2073 7469 6c6c  ed methods still
-00003ae0: 2068 6176 6520 736f 6d65 206c 696d 6974   have some limit
-00003af0: 6174 696f 6e73 2e20 5765 2061 7265 2064  ations. We are d
-00003b00: 6576 656c 6f70 696e 6720 6120 6d6f 6475  eveloping a modu
-00003b10: 6c65 2074 6f20 6d65 7267 6520 7468 6520  le to merge the 
-00003b20: 4c69 6674 4f6e 2061 6e6e 6f74 6174 696f  LiftOn annotatio
-00003b30: 6e20 7769 7468 2074 6865 2072 656c 6561  n with the relea
-00003b40: 7365 6420 6375 7261 7465 6420 616e 6e6f  sed curated anno
-00003b50: 7461 7469 6f6e 7320 746f 2067 656e 6572  tations to gener
-00003b60: 6174 6520 6265 7474 6572 2061 6e6e 6f74  ate better annot
-00003b70: 6174 696f 6e73 2e3c 2f70 3e0a 3c70 3e54  ations.</p>.<p>T
-00003b80: 6865 204c 6966 744f 6e20 3c65 6d3e 6368  he LiftOn <em>ch
-00003b90: 6169 6e69 6e67 2061 6c67 6f72 6974 686d  aining algorithm
-00003ba0: 3c2f 656d 3e20 6e6f 7720 646f 6573 206e  </em> now does n
-00003bb0: 6f74 2073 7570 706f 7274 206d 756c 7469  ot support multi
-00003bc0: 2d74 6872 6561 6469 6e67 2e20 5468 6973  -threading. This
-00003bd0: 2066 756e 6374 696f 6e61 6c69 7479 2073   functionality s
-00003be0: 7461 6e64 7320 6173 206f 7572 206e 6578  tands as our nex
-00003bf0: 7420 7461 7267 6574 6564 2066 6561 7475  t targeted featu
-00003c00: 7265 206f 6e20 7468 6520 6465 7665 6c6f  re on the develo
-00003c10: 706d 656e 7420 686f 7269 7a6f 6e21 3c2f  pment horizon!</
-00003c20: 703e 0a3c 6469 7620 636c 6173 733d 226c  p>.<div class="l
-00003c30: 696e 652d 626c 6f63 6b22 3e0a 3c64 6976  ine-block">.<div
-00003c40: 2063 6c61 7373 3d22 6c69 6e65 223e 3c62   class="line"><b
-00003c50: 723e 3c2f 6469 763e 0a3c 2f64 6976 3e0a  r></div>.</div>.
-00003c60: 3c2f 7365 6374 696f 6e3e 0a3c 7365 6374  </section>.<sect
-00003c70: 696f 6e20 6964 3d22 7573 6572 2d73 7570  ion id="user-sup
-00003c80: 706f 7274 223e 0a3c 6832 3e55 7365 7220  port">.<h2>User 
-00003c90: 7375 7070 6f72 743c 6120 636c 6173 733d  support<a class=
-00003ca0: 2268 6561 6465 726c 696e 6b22 2068 7265  "headerlink" hre
-00003cb0: 663d 2223 7573 6572 2d73 7570 706f 7274  f="#user-support
-00003cc0: 2220 7469 746c 653d 2250 6572 6d61 6c69  " title="Permali
-00003cd0: 6e6b 2074 6f20 7468 6973 2068 6561 6469  nk to this headi
-00003ce0: 6e67 223e 233c 2f61 3e3c 2f68 323e 0a3c  ng">#</a></h2>.<
-00003cf0: 703e 506c 6561 7365 2067 6f20 7468 726f  p>Please go thro
-00003d00: 7567 6820 7468 6520 3c61 2063 6c61 7373  ugh the <a class
-00003d10: 3d22 7265 6665 7265 6e63 6520 696e 7465  ="reference inte
-00003d20: 726e 616c 2220 6872 6566 3d22 2374 6162  rnal" href="#tab
-00003d30: 6c65 2d6f 662d 636f 6e74 656e 7473 223e  le-of-contents">
-00003d40: 3c73 7061 6e20 636c 6173 733d 2273 7464  <span class="std
-00003d50: 2073 7464 2d72 6566 223e 646f 6375 6d65   std-ref">docume
-00003d60: 6e74 6174 696f 6e3c 2f73 7061 6e3e 3c2f  ntation</span></
-00003d70: 613e 2062 656c 6f77 2066 6972 7374 2e20  a> below first. 
-00003d80: 4966 2079 6f75 2068 6176 6520 7175 6573  If you have ques
-00003d90: 7469 6f6e 7320 6162 6f75 7420 7573 696e  tions about usin
-00003da0: 6720 7468 6520 7061 636b 6167 652c 2061  g the package, a
-00003db0: 2062 7567 2072 6570 6f72 742c 206f 7220   bug report, or 
-00003dc0: 6120 6665 6174 7572 6520 7265 7175 6573  a feature reques
-00003dd0: 742c 2070 6c65 6173 6520 7573 6520 7468  t, please use th
-00003de0: 6520 4769 7448 7562 2069 7373 7565 2074  e GitHub issue t
-00003df0: 7261 636b 6572 2068 6572 653a 3c2f 703e  racker here:</p>
-00003e00: 0a3c 703e 3c61 2063 6c61 7373 3d22 7265  .<p><a class="re
-00003e10: 6665 7265 6e63 6520 6578 7465 726e 616c  ference external
-00003e20: 2220 6872 6566 3d22 6874 7470 733a 2f2f  " href="https://
-00003e30: 6769 7468 7562 2e63 6f6d 2f4b 7561 6e68  github.com/Kuanh
-00003e40: 616f 2d43 6861 6f2f 4c69 6674 4f6e 2f69  ao-Chao/LiftOn/i
-00003e50: 7373 7565 7322 3e68 7474 7073 3a2f 2f67  ssues">https://g
-00003e60: 6974 6875 622e 636f 6d2f 4b75 616e 6861  ithub.com/Kuanha
-00003e70: 6f2d 4368 616f 2f4c 6966 744f 6e2f 6973  o-Chao/LiftOn/is
-00003e80: 7375 6573 3c2f 613e 3c2f 703e 0a3c 6469  sues</a></p>.<di
-00003e90: 7620 636c 6173 733d 226c 696e 652d 626c  v class="line-bl
-00003ea0: 6f63 6b22 3e0a 3c64 6976 2063 6c61 7373  ock">.<div class
-00003eb0: 3d22 6c69 6e65 223e 3c62 723e 3c2f 6469  ="line"><br></di
-00003ec0: 763e 0a3c 2f64 6976 3e0a 3c2f 7365 6374  v>.</div>.</sect
-00003ed0: 696f 6e3e 0a3c 7365 6374 696f 6e20 6964  ion>.<section id
-00003ee0: 3d22 6b65 792d 636f 6e74 7269 6275 746f  ="key-contributo
-00003ef0: 7273 223e 0a3c 6832 3e4b 6579 2063 6f6e  rs">.<h2>Key con
-00003f00: 7472 6962 7574 6f72 733c 6120 636c 6173  tributors<a clas
-00003f10: 733d 2268 6561 6465 726c 696e 6b22 2068  s="headerlink" h
-00003f20: 7265 663d 2223 6b65 792d 636f 6e74 7269  ref="#key-contri
-00003f30: 6275 746f 7273 2220 7469 746c 653d 2250  butors" title="P
-00003f40: 6572 6d61 6c69 6e6b 2074 6f20 7468 6973  ermalink to this
-00003f50: 2068 6561 6469 6e67 223e 233c 2f61 3e3c   heading">#</a><
-00003f60: 2f68 323e 0a3c 703e 4c69 6674 4f6e 2077  /h2>.<p>LiftOn w
-00003f70: 6173 2064 6573 6967 6e65 6420 616e 6420  as designed and 
-00003f80: 6465 7665 6c6f 7065 6420 6279 203c 6120  developed by <a 
-00003f90: 636c 6173 733d 2272 6566 6572 656e 6365  class="reference
-00003fa0: 2065 7874 6572 6e61 6c22 2068 7265 663d   external" href=
-00003fb0: 2268 7474 7073 3a2f 2f6b 6863 6861 6f2e  "https://khchao.
-00003fc0: 636f 6d2f 223e 4b75 616e 2d48 616f 2043  com/">Kuan-Hao C
-00003fd0: 6861 6f3c 2f61 3e2e 2020 5468 6973 2064  hao</a>.  This d
-00003fe0: 6f63 756d 656e 7461 7469 6f6e 2077 6173  ocumentation was
-00003ff0: 2077 7269 7474 656e 2062 7920 3c61 2063   written by <a c
-00004000: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
-00004010: 6578 7465 726e 616c 2220 6872 6566 3d22  external" href="
-00004020: 6874 7470 733a 2f2f 6b68 6368 616f 2e63  https://khchao.c
-00004030: 6f6d 2f22 3e4b 7561 6e2d 4861 6f20 4368  om/">Kuan-Hao Ch
-00004040: 616f 3c2f 613e 2e3c 2f70 3e0a 3c64 6976  ao</a>.</p>.<div
-00004050: 2063 6c61 7373 3d22 6c69 6e65 2d62 6c6f   class="line-blo
-00004060: 636b 223e 0a3c 6469 7620 636c 6173 733d  ck">.<div class=
-00004070: 226c 696e 6522 3e3c 6272 3e3c 2f64 6976  "line"><br></div
-00004080: 3e0a 3c2f 6469 763e 0a3c 2f73 6563 7469  >.</div>.</secti
-00004090: 6f6e 3e0a 3c73 6563 7469 6f6e 2069 643d  on>.<section id=
-000040a0: 2274 6162 6c65 2d6f 662d 636f 6e74 656e  "table-of-conten
-000040b0: 7473 223e 0a3c 7370 616e 2069 643d 2269  ts">.<span id="i
-000040c0: 6433 223e 3c2f 7370 616e 3e3c 6832 3e54  d3"></span><h2>T
-000040d0: 6162 6c65 206f 6620 636f 6e74 656e 7473  able of contents
-000040e0: 3c61 2063 6c61 7373 3d22 6865 6164 6572  <a class="header
-000040f0: 6c69 6e6b 2220 6872 6566 3d22 2374 6162  link" href="#tab
-00004100: 6c65 2d6f 662d 636f 6e74 656e 7473 2220  le-of-contents" 
-00004110: 7469 746c 653d 2250 6572 6d61 6c69 6e6b  title="Permalink
-00004120: 2074 6f20 7468 6973 2068 6561 6469 6e67   to this heading
-00004130: 223e 233c 2f61 3e3c 2f68 323e 0a3c 6469  ">#</a></h2>.<di
-00004140: 7620 636c 6173 733d 2274 6f63 7472 6565  v class="toctree
-00004150: 2d77 7261 7070 6572 2063 6f6d 706f 756e  -wrapper compoun
-00004160: 6422 3e0a 3c75 6c3e 0a3c 6c69 2063 6c61  d">.<ul>.<li cla
-00004170: 7373 3d22 746f 6374 7265 652d 6c31 223e  ss="toctree-l1">
-00004180: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
-00004190: 6e63 6520 696e 7465 726e 616c 2220 6872  nce internal" hr
-000041a0: 6566 3d22 6874 7470 3a2f 2f63 6362 2e6a  ef="http://ccb.j
-000041b0: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
-000041c0: 6e74 656e 742f 696e 7374 616c 6c61 7469  ntent/installati
-000041d0: 6f6e 2e68 746d 6c22 3e49 6e73 7461 6c6c  on.html">Install
-000041e0: 6174 696f 6e3c 2f61 3e3c 756c 3e0a 3c6c  ation</a><ul>.<l
-000041f0: 6920 636c 6173 733d 2274 6f63 7472 6565  i class="toctree
-00004200: 2d6c 3222 3e3c 6120 636c 6173 733d 2272  -l2"><a class="r
-00004210: 6566 6572 656e 6365 2069 6e74 6572 6e61  eference interna
-00004220: 6c22 2068 7265 663d 2268 7474 703a 2f2f  l" href="http://
-00004230: 6363 622e 6a68 752e 6564 752f 6c69 6674  ccb.jhu.edu/lift
-00004240: 6f6e 2f63 6f6e 7465 6e74 2f69 6e73 7461  on/content/insta
-00004250: 6c6c 6174 696f 6e2e 6874 6d6c 2373 7973  llation.html#sys
-00004260: 7465 6d2d 7265 7175 6972 656d 656e 7473  tem-requirements
-00004270: 223e 5379 7374 656d 2072 6571 7569 7265  ">System require
-00004280: 6d65 6e74 733c 2f61 3e3c 2f6c 693e 0a3c  ments</a></li>.<
-00004290: 6c69 2063 6c61 7373 3d22 746f 6374 7265  li class="toctre
-000042a0: 652d 6c32 223e 3c61 2063 6c61 7373 3d22  e-l2"><a class="
-000042b0: 7265 6665 7265 6e63 6520 696e 7465 726e  reference intern
-000042c0: 616c 2220 6872 6566 3d22 6874 7470 3a2f  al" href="http:/
-000042d0: 2f63 6362 2e6a 6875 2e65 6475 2f6c 6966  /ccb.jhu.edu/lif
-000042e0: 746f 6e2f 636f 6e74 656e 742f 696e 7374  ton/content/inst
-000042f0: 616c 6c61 7469 6f6e 2e68 746d 6c23 696e  allation.html#in
-00004300: 7374 616c 6c2d 7468 726f 7567 682d 7069  stall-through-pi
-00004310: 7022 3e49 6e73 7461 6c6c 2074 6872 6f75  p">Install throu
-00004320: 6768 2070 6970 3c2f 613e 3c2f 6c69 3e0a  gh pip</a></li>.
-00004330: 3c6c 6920 636c 6173 733d 2274 6f63 7472  <li class="toctr
-00004340: 6565 2d6c 3222 3e3c 6120 636c 6173 733d  ee-l2"><a class=
-00004350: 2272 6566 6572 656e 6365 2069 6e74 6572  "reference inter
-00004360: 6e61 6c22 2068 7265 663d 2268 7474 703a  nal" href="http:
-00004370: 2f2f 6363 622e 6a68 752e 6564 752f 6c69  //ccb.jhu.edu/li
-00004380: 6674 6f6e 2f63 6f6e 7465 6e74 2f69 6e73  fton/content/ins
-00004390: 7461 6c6c 6174 696f 6e2e 6874 6d6c 2369  tallation.html#i
-000043a0: 6e73 7461 6c6c 2d74 6872 6f75 6768 2d63  nstall-through-c
-000043b0: 6f6e 6461 223e 496e 7374 616c 6c20 7468  onda">Install th
-000043c0: 726f 7567 6820 636f 6e64 613c 2f61 3e3c  rough conda</a><
-000043d0: 2f6c 693e 0a3c 6c69 2063 6c61 7373 3d22  /li>.<li class="
-000043e0: 746f 6374 7265 652d 6c32 223e 3c61 2063  toctree-l2"><a c
-000043f0: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
-00004400: 696e 7465 726e 616c 2220 6872 6566 3d22  internal" href="
-00004410: 6874 7470 3a2f 2f63 6362 2e6a 6875 2e65  http://ccb.jhu.e
-00004420: 6475 2f6c 6966 746f 6e2f 636f 6e74 656e  du/lifton/conten
-00004430: 742f 696e 7374 616c 6c61 7469 6f6e 2e68  t/installation.h
-00004440: 746d 6c23 696e 7374 616c 6c2d 6672 6f6d  tml#install-from
-00004450: 2d73 6f75 7263 6522 3e49 6e73 7461 6c6c  -source">Install
-00004460: 2066 726f 6d20 736f 7572 6365 3c2f 613e   from source</a>
-00004470: 3c2f 6c69 3e0a 3c6c 6920 636c 6173 733d  </li>.<li class=
-00004480: 2274 6f63 7472 6565 2d6c 3222 3e3c 6120  "toctree-l2"><a 
-00004490: 636c 6173 733d 2272 6566 6572 656e 6365  class="reference
-000044a0: 2069 6e74 6572 6e61 6c22 2068 7265 663d   internal" href=
-000044b0: 2268 7474 703a 2f2f 6363 622e 6a68 752e  "http://ccb.jhu.
-000044c0: 6564 752f 6c69 6674 6f6e 2f63 6f6e 7465  edu/lifton/conte
-000044d0: 6e74 2f69 6e73 7461 6c6c 6174 696f 6e2e  nt/installation.
-000044e0: 6874 6d6c 2363 6865 636b 2d6c 6966 746f  html#check-lifto
-000044f0: 6e2d 696e 7374 616c 6c61 7469 6f6e 223e  n-installation">
-00004500: 4368 6563 6b20 4c69 6674 4f6e 2069 6e73  Check LiftOn ins
-00004510: 7461 6c6c 6174 696f 6e3c 2f61 3e3c 2f6c  tallation</a></l
-00004520: 693e 0a3c 6c69 2063 6c61 7373 3d22 746f  i>.<li class="to
-00004530: 6374 7265 652d 6c32 223e 3c61 2063 6c61  ctree-l2"><a cla
-00004540: 7373 3d22 7265 6665 7265 6e63 6520 696e  ss="reference in
-00004550: 7465 726e 616c 2220 6872 6566 3d22 6874  ternal" href="ht
-00004560: 7470 3a2f 2f63 6362 2e6a 6875 2e65 6475  tp://ccb.jhu.edu
-00004570: 2f6c 6966 746f 6e2f 636f 6e74 656e 742f  /lifton/content/
-00004580: 696e 7374 616c 6c61 7469 6f6e 2e68 746d  installation.htm
-00004590: 6c23 6e6f 772d 796f 752d 6172 652d 7265  l#now-you-are-re
-000045a0: 6164 792d 746f 2d67 6f22 3e4e 6f77 2c20  ady-to-go">Now, 
-000045b0: 796f 7520 6172 6520 7265 6164 7920 746f  you are ready to
-000045c0: 2067 6f20 213c 2f61 3e3c 2f6c 693e 0a3c   go !</a></li>.<
-000045d0: 2f75 6c3e 0a3c 2f6c 693e 0a3c 6c69 2063  /ul>.</li>.<li c
-000045e0: 6c61 7373 3d22 746f 6374 7265 652d 6c31  lass="toctree-l1
-000045f0: 223e 3c61 2063 6c61 7373 3d22 7265 6665  "><a class="refe
-00004600: 7265 6e63 6520 696e 7465 726e 616c 2220  rence internal" 
-00004610: 6872 6566 3d22 6874 7470 3a2f 2f63 6362  href="http://ccb
-00004620: 2e6a 6875 2e65 6475 2f6c 6966 746f 6e2f  .jhu.edu/lifton/
-00004630: 636f 6e74 656e 742f 7175 6963 6b73 7461  content/quicksta
-00004640: 7274 2e68 746d 6c22 3e51 7569 636b 2053  rt.html">Quick S
-00004650: 7461 7274 2047 7569 6465 3c2f 613e 3c75  tart Guide</a><u
-00004660: 6c3e 0a3c 6c69 2063 6c61 7373 3d22 746f  l>.<li class="to
-00004670: 6374 7265 652d 6c32 223e 3c61 2063 6c61  ctree-l2"><a cla
-00004680: 7373 3d22 7265 6665 7265 6e63 6520 696e  ss="reference in
-00004690: 7465 726e 616c 2220 6872 6566 3d22 6874  ternal" href="ht
-000046a0: 7470 3a2f 2f63 6362 2e6a 6875 2e65 6475  tp://ccb.jhu.edu
-000046b0: 2f6c 6966 746f 6e2f 636f 6e74 656e 742f  /lifton/content/
-000046c0: 7175 6963 6b73 7461 7274 2e68 746d 6c23  quickstart.html#
-000046d0: 7375 7065 722d 7175 6963 6b2d 7374 6172  super-quick-star
-000046e0: 742d 6f6e 652d 6c69 6e65 7222 3e53 7570  t-one-liner">Sup
-000046f0: 6572 2d51 7569 636b 2053 7461 7274 2028  er-Quick Start (
-00004700: 6f6e 652d 6c69 6e65 7229 3c2f 613e 3c2f  one-liner)</a></
-00004710: 6c69 3e0a 3c6c 6920 636c 6173 733d 2274  li>.<li class="t
-00004720: 6f63 7472 6565 2d6c 3222 3e3c 6120 636c  octree-l2"><a cl
-00004730: 6173 733d 2272 6566 6572 656e 6365 2069  ass="reference i
-00004740: 6e74 6572 6e61 6c22 2068 7265 663d 2268  nternal" href="h
-00004750: 7474 703a 2f2f 6363 622e 6a68 752e 6564  ttp://ccb.jhu.ed
-00004760: 752f 6c69 6674 6f6e 2f63 6f6e 7465 6e74  u/lifton/content
-00004770: 2f71 7569 636b 7374 6172 742e 6874 6d6c  /quickstart.html
-00004780: 2374 7279 2d6c 6966 746f 6e2d 6f6e 2d67  #try-lifton-on-g
-00004790: 6f6f 676c 652d 636f 6c61 6222 3e54 7279  oogle-colab">Try
-000047a0: 204c 6966 744f 6e20 6f6e 2047 6f6f 676c   LiftOn on Googl
-000047b0: 6520 436f 6c61 623c 2f61 3e3c 2f6c 693e  e Colab</a></li>
-000047c0: 0a3c 2f75 6c3e 0a3c 2f6c 693e 0a3c 2f75  .</ul>.</li>.</u
-000047d0: 6c3e 0a3c 2f64 6976 3e0a 3c64 6976 2063  l>.</div>.<div c
-000047e0: 6c61 7373 3d22 746f 6374 7265 652d 7772  lass="toctree-wr
-000047f0: 6170 7065 7220 636f 6d70 6f75 6e64 223e  apper compound">
-00004800: 0a3c 7020 636c 6173 733d 2263 6170 7469  .<p class="capti
-00004810: 6f6e 2220 726f 6c65 3d22 6865 6164 696e  on" role="headin
-00004820: 6722 3e3c 7370 616e 2063 6c61 7373 3d22  g"><span class="
-00004830: 6361 7074 696f 6e2d 7465 7874 223e 4578  caption-text">Ex
-00004840: 616d 706c 6573 3c2f 7370 616e 3e3c 2f70  amples</span></p
-00004850: 3e0a 3c75 6c3e 0a3c 6c69 2063 6c61 7373  >.<ul>.<li class
-00004860: 3d22 746f 6374 7265 652d 6c31 223e 3c61  ="toctree-l1"><a
-00004870: 2063 6c61 7373 3d22 7265 6665 7265 6e63   class="referenc
-00004880: 6520 696e 7465 726e 616c 2220 6872 6566  e internal" href
-00004890: 3d22 6874 7470 3a2f 2f63 6362 2e6a 6875  ="http://ccb.jhu
-000048a0: 2e65 6475 2f6c 6966 746f 6e2f 636f 6e74  .edu/lifton/cont
-000048b0: 656e 742f 7361 6d65 5f73 7065 6369 6573  ent/same_species
-000048c0: 5f6c 6966 746f 7665 722f 696e 6465 782e  _liftover/index.
-000048d0: 6874 6d6c 223e 5361 6d65 2073 7065 6369  html">Same speci
-000048e0: 6573 206c 6966 742d 6f76 6572 3c2f 613e  es lift-over</a>
-000048f0: 3c2f 6c69 3e0a 3c6c 6920 636c 6173 733d  </li>.<li class=
-00004900: 2274 6f63 7472 6565 2d6c 3122 3e3c 6120  "toctree-l1"><a 
-00004910: 636c 6173 733d 2272 6566 6572 656e 6365  class="reference
-00004920: 2069 6e74 6572 6e61 6c22 2068 7265 663d   internal" href=
-00004930: 2268 7474 703a 2f2f 6363 622e 6a68 752e  "http://ccb.jhu.
-00004940: 6564 752f 6c69 6674 6f6e 2f63 6f6e 7465  edu/lifton/conte
-00004950: 6e74 2f63 6c6f 7365 5f73 7065 6369 6573  nt/close_species
-00004960: 5f6c 6966 746f 7665 722f 696e 6465 782e  _liftover/index.
-00004970: 6874 6d6c 223e 436c 6f73 656c 792d 7265  html">Closely-re
-00004980: 6c61 7465 6420 7370 6563 6965 7320 6c69  lated species li
-00004990: 6674 2d6f 7665 723c 2f61 3e3c 2f6c 693e  ft-over</a></li>
-000049a0: 0a3c 6c69 2063 6c61 7373 3d22 746f 6374  .<li class="toct
-000049b0: 7265 652d 6c31 223e 3c61 2063 6c61 7373  ree-l1"><a class
-000049c0: 3d22 7265 6665 7265 6e63 6520 696e 7465  ="reference inte
-000049d0: 726e 616c 2220 6872 6566 3d22 6874 7470  rnal" href="http
-000049e0: 3a2f 2f63 6362 2e6a 6875 2e65 6475 2f6c  ://ccb.jhu.edu/l
-000049f0: 6966 746f 6e2f 636f 6e74 656e 742f 6469  ifton/content/di
-00004a00: 7374 616e 745f 7370 6563 6965 735f 6c69  stant_species_li
-00004a10: 6674 6f76 6572 2f69 6e64 6578 2e68 746d  ftover/index.htm
-00004a20: 6c22 3e44 6973 7461 6e74 2073 7065 6369  l">Distant speci
-00004a30: 6573 206c 6966 742d 6f76 6572 3c2f 613e  es lift-over</a>
-00004a40: 3c2f 6c69 3e0a 3c2f 756c 3e0a 3c2f 6469  </li>.</ul>.</di
-00004a50: 763e 0a3c 6469 7620 636c 6173 733d 2274  v>.<div class="t
-00004a60: 6f63 7472 6565 2d77 7261 7070 6572 2063  octree-wrapper c
-00004a70: 6f6d 706f 756e 6422 3e0a 3c70 2063 6c61  ompound">.<p cla
-00004a80: 7373 3d22 6361 7074 696f 6e22 2072 6f6c  ss="caption" rol
-00004a90: 653d 2268 6561 6469 6e67 223e 3c73 7061  e="heading"><spa
-00004aa0: 6e20 636c 6173 733d 2263 6170 7469 6f6e  n class="caption
-00004ab0: 2d74 6578 7422 3e49 6e66 6f3c 2f73 7061  -text">Info</spa
-00004ac0: 6e3e 3c2f 703e 0a3c 756c 3e0a 3c6c 6920  n></p>.<ul>.<li 
-00004ad0: 636c 6173 733d 2274 6f63 7472 6565 2d6c  class="toctree-l
-00004ae0: 3122 3e3c 6120 636c 6173 733d 2272 6566  1"><a class="ref
-00004af0: 6572 656e 6365 2069 6e74 6572 6e61 6c22  erence internal"
-00004b00: 2068 7265 663d 2268 7474 703a 2f2f 6363   href="http://cc
-00004b10: 622e 6a68 752e 6564 752f 6c69 6674 6f6e  b.jhu.edu/lifton
-00004b20: 2f63 6f6e 7465 6e74 2f6f 7574 7075 745f  /content/output_
-00004b30: 6578 706c 616e 6174 696f 6e2e 6874 6d6c  explanation.html
-00004b40: 223e 4f75 7470 7574 2066 696c 6573 3c2f  ">Output files</
-00004b50: 613e 3c75 6c3e 0a3c 6c69 2063 6c61 7373  a><ul>.<li class
-00004b60: 3d22 746f 6374 7265 652d 6c32 223e 3c61  ="toctree-l2"><a
-00004b70: 2063 6c61 7373 3d22 7265 6665 7265 6e63   class="referenc
-00004b80: 6520 696e 7465 726e 616c 2220 6872 6566  e internal" href
-00004b90: 3d22 6874 7470 3a2f 2f63 6362 2e6a 6875  ="http://ccb.jhu
-00004ba0: 2e65 6475 2f6c 6966 746f 6e2f 636f 6e74  .edu/lifton/cont
-00004bb0: 656e 742f 6f75 7470 7574 5f65 7870 6c61  ent/output_expla
-00004bc0: 6e61 7469 6f6e 2e68 746d 6c23 6c69 6674  nation.html#lift
-00004bd0: 6f6e 2d67 6666 3322 3e6c 6966 746f 6e2e  on-gff3">lifton.
-00004be0: 4746 4633 3c2f 613e 3c2f 6c69 3e0a 3c6c  GFF3</a></li>.<l
-00004bf0: 6920 636c 6173 733d 2274 6f63 7472 6565  i class="toctree
-00004c00: 2d6c 3222 3e3c 6120 636c 6173 733d 2272  -l2"><a class="r
-00004c10: 6566 6572 656e 6365 2069 6e74 6572 6e61  eference interna
-00004c20: 6c22 2068 7265 663d 2268 7474 703a 2f2f  l" href="http://
-00004c30: 6363 622e 6a68 752e 6564 752f 6c69 6674  ccb.jhu.edu/lift
-00004c40: 6f6e 2f63 6f6e 7465 6e74 2f6f 7574 7075  on/content/outpu
-00004c50: 745f 6578 706c 616e 6174 696f 6e2e 6874  t_explanation.ht
-00004c60: 6d6c 236c 6966 746f 6e2d 6f75 7470 7574  ml#lifton-output
-00004c70: 223e 6c69 6674 6f6e 5f6f 7574 7075 742f  ">lifton_output/
-00004c80: 3c2f 613e 3c2f 6c69 3e0a 3c2f 756c 3e0a  </a></li>.</ul>.
-00004c90: 3c2f 6c69 3e0a 3c6c 6920 636c 6173 733d  </li>.<li class=
-00004ca0: 2274 6f63 7472 6565 2d6c 3122 3e3c 6120  "toctree-l1"><a 
-00004cb0: 636c 6173 733d 2272 6566 6572 656e 6365  class="reference
-00004cc0: 2069 6e74 6572 6e61 6c22 2068 7265 663d   internal" href=
-00004cd0: 2268 7474 703a 2f2f 6363 622e 6a68 752e  "http://ccb.jhu.
-00004ce0: 6564 752f 6c69 6674 6f6e 2f63 6f6e 7465  edu/lifton/conte
-00004cf0: 6e74 2f62 6568 696e 645f 7363 656e 6573  nt/behind_scenes
-00004d00: 2e68 746d 6c22 3e42 6568 696e 6420 7468  .html">Behind th
-00004d10: 6520 7363 656e 6573 3c2f 613e 3c75 6c3e  e scenes</a><ul>
-00004d20: 0a3c 6c69 2063 6c61 7373 3d22 746f 6374  .<li class="toct
-00004d30: 7265 652d 6c32 223e 3c61 2063 6c61 7373  ree-l2"><a class
-00004d40: 3d22 7265 6665 7265 6e63 6520 696e 7465  ="reference inte
-00004d50: 726e 616c 2220 6872 6566 3d22 6874 7470  rnal" href="http
-00004d60: 3a2f 2f63 6362 2e6a 6875 2e65 6475 2f6c  ://ccb.jhu.edu/l
-00004d70: 6966 746f 6e2f 636f 6e74 656e 742f 6265  ifton/content/be
-00004d80: 6869 6e64 5f73 6365 6e65 732e 6874 6d6c  hind_scenes.html
-00004d90: 236d 6174 6368 696e 672d 6d69 6e69 7072  #matching-minipr
-00004da0: 6f74 2d6c 6966 746f 6666 2d67 656e 6f6d  ot-liftoff-genom
-00004db0: 652d 616e 6e6f 7461 7469 6f6e 223e 4d61  e-annotation">Ma
-00004dc0: 7463 6869 6e67 206d 696e 6970 726f 7420  tching miniprot 
-00004dd0: 2661 6d70 3b20 4c69 6674 6f66 6620 6765  &amp; Liftoff ge
-00004de0: 6e6f 6d65 2061 6e6e 6f74 6174 696f 6e3c  nome annotation<
-00004df0: 2f61 3e3c 2f6c 693e 0a3c 6c69 2063 6c61  /a></li>.<li cla
-00004e00: 7373 3d22 746f 6374 7265 652d 6c32 223e  ss="toctree-l2">
-00004e10: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
-00004e20: 6e63 6520 696e 7465 726e 616c 2220 6872  nce internal" hr
-00004e30: 6566 3d22 6874 7470 3a2f 2f63 6362 2e6a  ef="http://ccb.j
-00004e40: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
-00004e50: 6e74 656e 742f 6265 6869 6e64 5f73 6365  ntent/behind_sce
-00004e60: 6e65 732e 6874 6d6c 2370 726f 7465 696e  nes.html#protein
-00004e70: 2d6d 6178 696d 697a 6174 696f 6e2d 616c  -maximization-al
-00004e80: 676f 7269 7468 6d22 3e3c 656d 3e50 726f  gorithm"><em>Pro
-00004e90: 7465 696e 2d6d 6178 696d 697a 6174 696f  tein-maximizatio
-00004ea0: 6e20 616c 676f 7269 7468 6d3c 2f65 6d3e  n algorithm</em>
-00004eb0: 3c2f 613e 3c2f 6c69 3e0a 3c6c 6920 636c  </a></li>.<li cl
-00004ec0: 6173 733d 2274 6f63 7472 6565 2d6c 3222  ass="toctree-l2"
-00004ed0: 3e3c 6120 636c 6173 733d 2272 6566 6572  ><a class="refer
-00004ee0: 656e 6365 2069 6e74 6572 6e61 6c22 2068  ence internal" h
-00004ef0: 7265 663d 2268 7474 703a 2f2f 6363 622e  ref="http://ccb.
-00004f00: 6a68 752e 6564 752f 6c69 6674 6f6e 2f63  jhu.edu/lifton/c
-00004f10: 6f6e 7465 6e74 2f62 6568 696e 645f 7363  ontent/behind_sc
-00004f20: 656e 6573 2e68 746d 6c23 6d75 7461 7469  enes.html#mutati
-00004f30: 6f6e 2d72 6570 6f72 7422 3e4d 7574 6174  on-report">Mutat
-00004f40: 696f 6e20 7265 706f 7274 3c2f 613e 3c2f  ion report</a></
-00004f50: 6c69 3e0a 3c6c 6920 636c 6173 733d 2274  li>.<li class="t
-00004f60: 6f63 7472 6565 2d6c 3222 3e3c 6120 636c  octree-l2"><a cl
-00004f70: 6173 733d 2272 6566 6572 656e 6365 2069  ass="reference i
-00004f80: 6e74 6572 6e61 6c22 2068 7265 663d 2268  nternal" href="h
-00004f90: 7474 703a 2f2f 6363 622e 6a68 752e 6564  ttp://ccb.jhu.ed
-00004fa0: 752f 6c69 6674 6f6e 2f63 6f6e 7465 6e74  u/lifton/content
-00004fb0: 2f62 6568 696e 645f 7363 656e 6573 2e68  /behind_scenes.h
-00004fc0: 746d 6c23 6f70 656e 2d72 6561 6469 6e67  tml#open-reading
-00004fd0: 2d66 7261 6d65 2d73 6561 7263 6822 3e4f  -frame-search">O
-00004fe0: 7065 6e2d 7265 6164 696e 672d 6672 616d  pen-reading-fram
-00004ff0: 6520 7365 6172 6368 3c2f 613e 3c2f 6c69  e search</a></li
-00005000: 3e0a 3c6c 6920 636c 6173 733d 2274 6f63  >.<li class="toc
-00005010: 7472 6565 2d6c 3222 3e3c 6120 636c 6173  tree-l2"><a clas
-00005020: 733d 2272 6566 6572 656e 6365 2069 6e74  s="reference int
-00005030: 6572 6e61 6c22 2068 7265 663d 2268 7474  ernal" href="htt
-00005040: 703a 2f2f 6363 622e 6a68 752e 6564 752f  p://ccb.jhu.edu/
-00005050: 6c69 6674 6f6e 2f63 6f6e 7465 6e74 2f62  lifton/content/b
-00005060: 6568 696e 645f 7363 656e 6573 2e68 746d  ehind_scenes.htm
-00005070: 6c23 646e 612d 7072 6f74 6569 6e2d 7472  l#dna-protein-tr
-00005080: 616e 7363 7269 7074 2d73 6571 7565 6e63  anscript-sequenc
-00005090: 652d 6964 656e 7469 7479 2d73 636f 7265  e-identity-score
-000050a0: 2d63 616c 6375 6c61 7469 6f6e 223e 444e  -calculation">DN
-000050b0: 4120 2661 6d70 3b20 7072 6f74 6569 6e20  A &amp; protein 
-000050c0: 7472 616e 7363 7269 7074 2073 6571 7565  transcript seque
-000050d0: 6e63 6520 6964 656e 7469 7479 2073 636f  nce identity sco
-000050e0: 7265 2063 616c 6375 6c61 7469 6f6e 3c2f  re calculation</
-000050f0: 613e 3c2f 6c69 3e0a 3c6c 6920 636c 6173  a></li>.<li clas
-00005100: 733d 2274 6f63 7472 6565 2d6c 3222 3e3c  s="toctree-l2"><
-00005110: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
-00005120: 6365 2069 6e74 6572 6e61 6c22 2068 7265  ce internal" hre
-00005130: 663d 2268 7474 703a 2f2f 6363 622e 6a68  f="http://ccb.jh
-00005140: 752e 6564 752f 6c69 6674 6f6e 2f63 6f6e  u.edu/lifton/con
-00005150: 7465 6e74 2f62 6568 696e 645f 7363 656e  tent/behind_scen
-00005160: 6573 2e68 746d 6c23 7265 6665 7265 6e63  es.html#referenc
-00005170: 6522 3e52 6566 6572 656e 6365 3c2f 613e  e">Reference</a>
-00005180: 3c2f 6c69 3e0a 3c2f 756c 3e0a 3c2f 6c69  </li>.</ul>.</li
-00005190: 3e0a 3c6c 6920 636c 6173 733d 2274 6f63  >.<li class="toc
-000051a0: 7472 6565 2d6c 3122 3e3c 6120 636c 6173  tree-l1"><a clas
-000051b0: 733d 2272 6566 6572 656e 6365 2069 6e74  s="reference int
-000051c0: 6572 6e61 6c22 2068 7265 663d 2268 7474  ernal" href="htt
-000051d0: 703a 2f2f 6363 622e 6a68 752e 6564 752f  p://ccb.jhu.edu/
-000051e0: 6c69 6674 6f6e 2f63 6f6e 7465 6e74 2f68  lifton/content/h
-000051f0: 6f77 5f74 6f5f 7061 6765 2e68 746d 6c22  ow_to_page.html"
-00005200: 3e51 2026 616d 703b 2041 202e 2e2e 3c2f  >Q &amp; A ...</
-00005210: 613e 3c2f 6c69 3e0a 3c6c 6920 636c 6173  a></li>.<li clas
-00005220: 733d 2274 6f63 7472 6565 2d6c 3122 3e3c  s="toctree-l1"><
-00005230: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
-00005240: 6365 2069 6e74 6572 6e61 6c22 2068 7265  ce internal" hre
-00005250: 663d 2268 7474 703a 2f2f 6363 622e 6a68  f="http://ccb.jh
-00005260: 752e 6564 752f 6c69 6674 6f6e 2f63 6f6e  u.edu/lifton/con
-00005270: 7465 6e74 2f66 756e 6374 696f 6e5f 6d61  tent/function_ma
-00005280: 6e75 616c 2e68 746d 6c22 3e55 7365 7220  nual.html">User 
-00005290: 4d61 6e75 616c 3c2f 613e 3c75 6c3e 0a3c  Manual</a><ul>.<
-000052a0: 6c69 2063 6c61 7373 3d22 746f 6374 7265  li class="toctre
-000052b0: 652d 6c32 223e 3c61 2063 6c61 7373 3d22  e-l2"><a class="
-000052c0: 7265 6665 7265 6e63 6520 696e 7465 726e  reference intern
-000052d0: 616c 2220 6872 6566 3d22 6874 7470 3a2f  al" href="http:/
-000052e0: 2f63 6362 2e6a 6875 2e65 6475 2f6c 6966  /ccb.jhu.edu/lif
-000052f0: 746f 6e2f 636f 6e74 656e 742f 6675 6e63  ton/content/func
-00005300: 7469 6f6e 5f6d 616e 7561 6c2e 6874 6d6c  tion_manual.html
-00005310: 2373 706c 616d 223e 7370 6c61 6d3c 2f61  #splam">splam</a
-00005320: 3e3c 2f6c 693e 0a3c 2f75 6c3e 0a3c 2f6c  ></li>.</ul>.</l
-00005330: 693e 0a3c 6c69 2063 6c61 7373 3d22 746f  i>.<li class="to
-00005340: 6374 7265 652d 6c31 223e 3c61 2063 6c61  ctree-l1"><a cla
-00005350: 7373 3d22 7265 6665 7265 6e63 6520 696e  ss="reference in
-00005360: 7465 726e 616c 2220 6872 6566 3d22 6874  ternal" href="ht
-00005370: 7470 3a2f 2f63 6362 2e6a 6875 2e65 6475  tp://ccb.jhu.edu
-00005380: 2f6c 6966 746f 6e2f 636f 6e74 656e 742f  /lifton/content/
-00005390: 6368 616e 6765 6c6f 672e 6874 6d6c 223e  changelog.html">
-000053a0: 4368 616e 6765 6c6f 673c 2f61 3e3c 756c  Changelog</a><ul
-000053b0: 3e0a 3c6c 6920 636c 6173 733d 2274 6f63  >.<li class="toc
-000053c0: 7472 6565 2d6c 3222 3e3c 6120 636c 6173  tree-l2"><a clas
-000053d0: 733d 2272 6566 6572 656e 6365 2069 6e74  s="reference int
-000053e0: 6572 6e61 6c22 2068 7265 663d 2268 7474  ernal" href="htt
-000053f0: 703a 2f2f 6363 622e 6a68 752e 6564 752f  p://ccb.jhu.edu/
-00005400: 6c69 6674 6f6e 2f63 6f6e 7465 6e74 2f63  lifton/content/c
-00005410: 6861 6e67 656c 6f67 2e68 746d 6c23 7631  hangelog.html#v1
-00005420: 2d30 2d30 223e 7631 2e30 2e30 3c2f 613e  -0-0">v1.0.0</a>
-00005430: 3c2f 6c69 3e0a 3c2f 756c 3e0a 3c2f 6c69  </li>.</ul>.</li
-00005440: 3e0a 3c6c 6920 636c 6173 733d 2274 6f63  >.<li class="toc
-00005450: 7472 6565 2d6c 3122 3e3c 6120 636c 6173  tree-l1"><a clas
-00005460: 733d 2272 6566 6572 656e 6365 2069 6e74  s="reference int
-00005470: 6572 6e61 6c22 2068 7265 663d 2268 7474  ernal" href="htt
-00005480: 703a 2f2f 6363 622e 6a68 752e 6564 752f  p://ccb.jhu.edu/
-00005490: 6c69 6674 6f6e 2f63 6f6e 7465 6e74 2f6c  lifton/content/l
-000054a0: 6963 656e 7365 2e68 746d 6c22 3e4c 6963  icense.html">Lic
-000054b0: 656e 7365 3c2f 613e 3c2f 6c69 3e0a 3c6c  ense</a></li>.<l
-000054c0: 6920 636c 6173 733d 2274 6f63 7472 6565  i class="toctree
-000054d0: 2d6c 3122 3e3c 6120 636c 6173 733d 2272  -l1"><a class="r
-000054e0: 6566 6572 656e 6365 2069 6e74 6572 6e61  eference interna
-000054f0: 6c22 2068 7265 663d 2268 7474 703a 2f2f  l" href="http://
-00005500: 6363 622e 6a68 752e 6564 752f 6c69 6674  ccb.jhu.edu/lift
-00005510: 6f6e 2f63 6f6e 7465 6e74 2f63 6f6e 7461  on/content/conta
-00005520: 6374 2e68 746d 6c22 3e43 6f6e 7461 6374  ct.html">Contact
-00005530: 3c2f 613e 3c2f 6c69 3e0a 3c2f 756c 3e0a  </a></li>.</ul>.
-00005540: 3c2f 6469 763e 0a3c 2f73 6563 7469 6f6e  </div>.</section
-00005550: 3e0a 3c2f 7365 6374 696f 6e3e 0a0a 3c62  >.</section>..<b
-00005560: 723e 0a0a 2323 203c 6120 6e61 6d65 3d22  r>..## <a name="
-00005570: 6369 7461 7469 6f6e 223e 3c2f 613e 4369  citation"></a>Ci
-00005580: 7461 7469 6f6e 3c61 2063 6c61 7373 3d22  tation<a class="
-00005590: 6865 6164 6572 6c69 6e6b 2220 6872 6566  headerlink" href
-000055a0: 3d22 2363 6974 6174 696f 6e22 2074 6974  ="#citation" tit
-000055b0: 6c65 3d22 5065 726d 616c 696e 6b20 746f  le="Permalink to
-000055c0: 2074 6869 7320 6865 6164 696e 6722 3e23   this heading">#
-000055d0: 3c2f 613e 0a0a 0a4b 7561 6e2d 4861 6f20  </a>...Kuan-Hao 
-000055e0: 4368 616f 2a2c 204d 6968 6165 6c61 2050  Chao*, Mihaela P
-000055f0: 6572 7465 612c 2053 7465 7665 6e20 4c20  ertea, Steven L 
-00005600: 5361 6c7a 6265 7267 2a2c 2022 4c69 6674  Salzberg*, "Lift
-00005610: 4f6e 3a20 6120 746f 6f6c 2074 6f20 696d  On: a tool to im
-00005620: 7072 6f76 6520 616e 6e6f 7461 7469 6f6e  prove annotation
-00005630: 7320 666f 7220 7072 6f74 6569 6e2d 636f  s for protein-co
-00005640: 6469 6e67 2067 656e 6573 2064 7572 696e  ding genes durin
-00005650: 6720 7468 6520 6c69 6674 2d6f 7665 7220  g the lift-over 
-00005660: 7072 6f63 6573 732e 222c 203c 693e 6269  process.", <i>bi
-00005670: 6f52 7869 763c 2f69 3e20 3c62 3e32 3032  oRxiv</i> <b>202
-00005680: 332e 3037 2e32 372e 3535 3037 3534 3c2f  3.07.27.550754</
-00005690: 623e 2c20 646f 693a 205b 6874 7470 733a  b>, doi: [https:
-000056a0: 2f2f 646f 692e 6f72 672f 3130 2e31 3130  //doi.org/10.110
-000056b0: 312f 3230 3233 2e30 372e 3237 2e35 3530  1/2023.07.27.550
-000056c0: 3735 345d 2868 7474 7073 3a2f 2f64 6f69  754](https://doi
-000056d0: 2e6f 7267 2f31 302e 3131 3031 2f32 3032  .org/10.1101/202
-000056e0: 332e 3037 2e32 372e 3535 3037 3534 292c  3.07.27.550754),
-000056f0: 2032 3032 330a 0a3c 6272 3e0a 3c62 723e   2023..<br>.<br>
-00005700: 0a3c 6272 3e0a 0a3c 696d 6720 616c 743d  .<br>..<img alt=
-00005710: 224d 7920 4c6f 676f 2220 636c 6173 733d  "My Logo" class=
-00005720: 226c 6f67 6f20 6865 6164 6572 2d69 6d61  "logo header-ima
-00005730: 6765 206f 6e6c 792d 6c69 6768 7420 616c  ge only-light al
-00005740: 6967 6e2d 6365 6e74 6572 2220 7372 633d  ign-center" src=
-00005750: 2267 7261 7068 6963 732f 6a68 752d 6c6f  "graphics/jhu-lo
-00005760: 676f 2d64 6172 6b2e 706e 6722 3e0a       go-dark.png">.
+000009b0: 6420 7072 6f74 6569 6e2d 444e 4120 616c  d protein-DNA al
+000009c0: 6967 6e6d 656e 7473 2028 6672 6f6d 203c  ignments (from <
+000009d0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000009e0: 6163 6164 656d 6963 2e6f 7570 2e63 6f6d  academic.oup.com
+000009f0: 2f62 696f 696e 666f 726d 6174 6963 732f  /bioinformatics/
+00000a00: 6172 7469 636c 652f 3339 2f31 2f62 7461  article/39/1/bta
+00000a10: 6430 3134 2f36 3938 3936 3231 2220 7461  d014/6989621" ta
+00000a20: 7267 6574 3d22 5f62 6c61 6e6b 223e 6d69  rget="_blank">mi
+00000a30: 6e69 7072 6f74 3c2f 613e 2c20 6372 6564  niprot</a>, cred
+00000a40: 6974 7320 746f 203c 6120 6872 6566 3d22  its to <a href="
+00000a50: 6874 7470 3a2f 2f6c 6968 656e 672e 6f72  http://liheng.or
+00000a60: 6722 2074 6172 6765 743d 225f 626c 616e  g" target="_blan
+00000a70: 6b22 3e44 722e 2048 656e 6720 4c69 3c2f  k">Dr. Heng Li</
+00000a80: 613e 2920 746f 2061 6363 7572 6174 656c  a>) to accuratel
+00000a90: 7920 6d61 7020 616e 6e6f 7461 7469 6f6e  y map annotation
+00000aa0: 7320 6265 7477 6565 6e20 6765 6e6f 6d65  s between genome
+00000ab0: 2061 7373 656d 626c 6965 7320 6f66 2074   assemblies of t
+00000ac0: 6865 2073 616d 6520 6f72 2064 6966 6665  he same or diffe
+00000ad0: 7265 6e74 2073 7065 6369 6573 2e20 4c69  rent species. Li
+00000ae0: 6674 4f6e 2065 6d70 6c6f 7973 2061 2074  ftOn employs a t
+00000af0: 776f 2d73 7465 7020 3c61 2068 7265 663d  wo-step <a href=
+00000b00: 2268 7474 7073 3a2f 2f63 6362 2e6a 6875  "https://ccb.jhu
+00000b10: 2e65 6475 2f6c 6966 746f 6e2f 636f 6e74  .edu/lifton/cont
+00000b20: 656e 742f 6265 6869 6e64 5f73 6365 6e65  ent/behind_scene
+00000b30: 732e 6874 6d6c 2370 726f 7465 696e 2d6d  s.html#protein-m
+00000b40: 6178 696d 697a 6174 696f 6e2d 616c 676f  aximization-algo
+00000b50: 7269 7468 6d22 3e70 726f 7465 696e 206d  rithm">protein m
+00000b60: 6178 696d 697a 6174 696f 6e20 616c 676f  aximization algo
+00000b70: 7269 7468 6d3c 2f61 3e20 746f 2069 6d70  rithm</a> to imp
+00000b80: 726f 7665 2074 6865 2061 6e6e 6f74 6174  rove the annotat
+00000b90: 696f 6e20 6f66 2070 726f 7465 696e 2d63  ion of protein-c
+00000ba0: 6f64 696e 6720 6765 6e65 7320 696e 2074  oding genes in t
+00000bb0: 6865 2054 3254 2d43 484d 3133 203c 6120  he T2T-CHM13 <a 
+00000bc0: 6872 6566 3d22 6874 7470 733a 2f2f 7333  href="https://s3
+00000bd0: 2d75 732d 7765 7374 2d32 2e61 6d61 7a6f  -us-west-2.amazo
+00000be0: 6e61 7773 2e63 6f6d 2f68 756d 616e 2d70  naws.com/human-p
+00000bf0: 616e 6765 6e6f 6d69 6373 2f54 3254 2f43  angenomics/T2T/C
+00000c00: 484d 3133 2f61 7373 656d 626c 6965 732f  HM13/assemblies/
+00000c10: 616e 6e6f 7461 7469 6f6e 2f63 686d 3133  annotation/chm13
+00000c20: 7632 2e30 5f52 6566 5365 715f 4c69 6674  v2.0_RefSeq_Lift
+00000c30: 6f66 665f 7635 2e31 2e67 6666 332e 677a  off_v5.1.gff3.gz
+00000c40: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000c50: 223e 4a48 5520 5265 6653 6571 7631 3130  ">JHU RefSeqv110
+00000c60: 202b 204c 6966 746f 6666 2076 352e 313c   + Liftoff v5.1<
+00000c70: 2f61 3e20 616e 6e6f 7461 7469 6f6e 2e0a  /a> annotation..
+00000c80: 5468 6520 6c61 7465 7374 2054 3254 2d43  The latest T2T-C
+00000c90: 484d 3133 2061 6e6e 6f74 6174 696f 6e20  HM13 annotation 
+00000ca0: 6765 6e65 7261 7465 6420 6279 204c 6966  generated by Lif
+00000cb0: 744f 6e20 6973 2061 7661 696c 6162 6c65  tOn is available
+00000cc0: 2061 7320 3c61 2068 7265 663d 2268 7474   as <a href="htt
+00000cd0: 7073 3a2f 2f74 696e 7975 726c 2e63 6f6d  ps://tinyurl.com
+00000ce0: 2f34 7879 7774 7776 6522 2074 6172 6765  /4xywtwve" targe
+00000cf0: 743d 225f 626c 616e 6b22 3e4a 4855 5f4c  t="_blank">JHU_L
+00000d00: 6966 744f 6e5f 7631 2e30 5f63 686d 3133  iftOn_v1.0_chm13
+00000d10: 7632 2e30 2e67 6666 3320 2866 7470 3a2f  v2.0.gff3 (ftp:/
+00000d20: 2f66 7470 2e63 6362 2e6a 6875 2e65 6475  /ftp.ccb.jhu.edu
+00000d30: 2f70 7562 2f64 6174 612f 4c69 6674 4f6e  /pub/data/LiftOn
+00000d40: 2f4a 4855 5f4c 6966 744f 6e5f 7631 2e30  /JHU_LiftOn_v1.0
+00000d50: 5f63 686d 3133 7632 2e30 2e67 6666 3329  _chm13v2.0.gff3)
+00000d60: 203c 6920 636c 6173 733d 2266 6120 6661   <i class="fa fa
+00000d70: 2d64 6f77 6e6c 6f61 6422 3e3c 2f69 3e3c  -download"></i><
+00000d80: 2f61 3e2e 3c73 6563 7469 6f6e 2069 643d  /a>.<section id=
+00000d90: 2277 6879 2d6c 6966 746f 6e22 2063 6c61  "why-lifton" cla
+00000da0: 7373 3d22 223e 0a3c 6832 3e57 6879 204c  ss="">.<h2>Why L
+00000db0: 6966 744f 6ee2 9d93 3c61 2063 6c61 7373  iftOn...<a class
+00000dc0: 3d22 6865 6164 6572 6c69 6e6b 2220 6872  ="headerlink" hr
+00000dd0: 6566 3d22 2377 6879 2d6c 6966 746f 6e22  ef="#why-lifton"
+00000de0: 2074 6974 6c65 3d22 5065 726d 616c 696e   title="Permalin
+00000df0: 6b20 746f 2074 6869 7320 6865 6164 696e  k to this headin
+00000e00: 6722 3e23 3c2f 613e 3c2f 6832 3e0a 3c6f  g">#</a></h2>.<o
+00000e10: 6c20 636c 6173 733d 2261 7261 6269 6320  l class="arabic 
+00000e20: 7369 6d70 6c65 223e 0a3c 6c69 3e3c 703e  simple">.<li><p>
+00000e30: 3c73 7472 6f6e 673e 4275 7267 656f 6e69  <strong>Burgeoni
+00000e40: 6e67 206e 756d 6265 7220 6f66 2067 656e  ng number of gen
+00000e50: 6f6d 6520 6173 7365 6d62 6c69 6573 3c2f  ome assemblies</
+00000e60: 7374 726f 6e67 3e3a 2041 7320 6f66 2044  strong>: As of D
+00000e70: 6563 656d 6265 7220 3230 3233 2c20 7468  ecember 2023, th
+00000e80: 6572 6520 6172 6520 3330 2c35 3330 2065  ere are 30,530 e
+00000e90: 756b 6172 796f 7469 6320 6765 6e6f 6d65  ukaryotic genome
+00000ea0: 732c 2035 3637 2c32 3238 2070 726f 6b61  s, 567,228 proka
+00000eb0: 7279 6f74 6963 2067 656e 6f6d 6573 2c20  ryotic genomes, 
+00000ec0: 616e 6420 3636 2c34 3239 2076 6972 7573  and 66,429 virus
+00000ed0: 6573 206c 6973 7465 6420 6f6e 204e 4342  es listed on NCB
+00000ee0: 4920 283c 6120 636c 6173 733d 2272 6566  I (<a class="ref
+00000ef0: 6572 656e 6365 2065 7874 6572 6e61 6c22  erence external"
+00000f00: 2068 7265 663d 2268 7474 7073 3a2f 2f77   href="https://w
+00000f10: 7777 2e6e 6362 692e 6e6c 6d2e 6e69 682e  ww.ncbi.nlm.nih.
+00000f20: 676f 762f 6765 6e6f 6d65 2f62 726f 7773  gov/genome/brows
+00000f30: 652f 2321 2f6f 7665 7276 6965 772f 223e  e/#!/overview/">
+00000f40: 4e43 4249 2067 656e 6f6d 6520 6272 6f77  NCBI genome brow
+00000f50: 7365 723c 2f61 3e29 2e20 486f 7765 7665  ser</a>). Howeve
+00000f60: 722c 2067 656e 6f6d 6520 616e 6e6f 7461  r, genome annota
+00000f70: 7469 6f6e 2069 7320 6c61 6767 696e 6720  tion is lagging 
+00000f80: 6265 6869 6e64 2e20 4173 206d 6f72 6520  behind. As more 
+00000f90: 6869 6768 2d71 7561 6c69 7479 2061 7373  high-quality ass
+00000fa0: 656d 626c 6965 7320 6172 6520 6765 6e65  emblies are gene
+00000fb0: 7261 7465 642c 2077 6520 6e65 6564 2061  rated, we need a
+00000fc0: 6e20 6163 6375 7261 7465 206c 6966 742d  n accurate lift-
+00000fd0: 6f76 6572 2074 6f6f 6c20 746f 2061 6e6e  over tool to ann
+00000fe0: 6f74 6174 6520 7468 656d 2e3c 2f70 3e3c  otate them.</p><
+00000ff0: 2f6c 693e 0a3c 6c69 3e3c 703e 3c73 7472  /li>.<li><p><str
+00001000: 6f6e 673e 496d 7072 6f76 6564 2070 726f  ong>Improved pro
+00001010: 7465 696e 2d63 6f64 696e 6720 6765 6e65  tein-coding gene
+00001020: 206d 6170 7069 6e67 3c2f 7374 726f 6e67   mapping</strong
+00001030: 3e3a 2054 6865 2070 6f70 756c 6172 203c  >: The popular <
+00001040: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
+00001050: 6365 2065 7874 6572 6e61 6c22 2068 7265  ce external" hre
+00001060: 663d 2268 7474 7073 3a2f 2f61 6361 6465  f="https://acade
+00001070: 6d69 632e 6f75 702e 636f 6d2f 6269 6f69  mic.oup.com/bioi
+00001080: 6e66 6f72 6d61 7469 6373 2f61 7274 6963  nformatics/artic
+00001090: 6c65 2f33 372f 3132 2f31 3633 392f 3630  le/37/12/1639/60
+000010a0: 3335 3132 383f 6c6f 6769 6e3d 7472 7565  35128?login=true
+000010b0: 223e 4c69 6674 6f66 663c 2f61 3e20 746f  ">Liftoff</a> to
+000010c0: 6f6c 206d 6170 7320 6765 6e65 7320 6261  ol maps genes ba
+000010d0: 7365 6420 6f6e 2044 4e41 2061 6c69 676e  sed on DNA align
+000010e0: 6d65 6e74 7320 616c 6f6e 652e 203c 6120  ments alone. <a 
+000010f0: 636c 6173 733d 2272 6566 6572 656e 6365  class="reference
+00001100: 2065 7874 6572 6e61 6c22 2068 7265 663d   external" href=
+00001110: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00001120: 636f 6d2f 6c68 332f 6d69 6e69 7072 6f74  com/lh3/miniprot
+00001130: 223e 4d69 6e69 7072 6f74 3c2f 613e 206d  ">Miniprot</a> m
+00001140: 6170 7320 6765 6e65 7320 6261 7365 6420  aps genes based 
+00001150: 6f6e 2070 726f 7465 696e 2061 6c69 676e  on protein align
+00001160: 6d65 6e74 7320 6275 742c 2077 6974 686f  ments but, witho
+00001170: 7574 2067 656e 6520 7374 7275 6374 7572  ut gene structur
+00001180: 6520 696e 666f 726d 6174 696f 6e2c 206d  e information, m
+00001190: 6179 206e 6f74 2062 6520 6173 2061 6363  ay not be as acc
+000011a0: 7572 6174 6520 6f6e 2074 6865 6972 206f  urate on their o
+000011b0: 776e 2028 5365 6520 3c61 2063 6c61 7373  wn (See <a class
+000011c0: 3d22 7265 6665 7265 6e63 6520 696e 7465  ="reference inte
+000011d0: 726e 616c 2220 6872 6566 3d22 6874 7470  rnal" href="http
+000011e0: 733a 2f2f 6363 622e 6a68 752e 6564 752f  s://ccb.jhu.edu/
+000011f0: 6c69 6674 6f6e 2f63 6f6e 7465 6e74 2f68  lifton/content/h
+00001200: 6f77 5f74 6f5f 7061 6765 2e68 746d 6c23  ow_to_page.html#
+00001210: 7768 792d 6c69 6674 6f6e 2d71 6122 3e3c  why-lifton-qa"><
+00001220: 7370 616e 2063 6c61 7373 3d22 7374 6420  span class="std 
+00001230: 7374 642d 7265 6622 3e46 4151 2043 6f6d  std-ref">FAQ Com
+00001240: 6d6f 6e20 6d69 7374 616b 6573 206f 6620  mon mistakes of 
+00001250: 4c69 6674 6f66 6620 616e 6420 6d69 6e69  Liftoff and mini
+00001260: 7072 6f74 3c2f 7370 616e 3e3c 2f61 3e29  prot</span></a>)
+00001270: 2e20 4c69 6674 4f6e 2063 6f6d 6269 6e65  . LiftOn combine
+00001280: 7320 626f 7468 2044 4e41 2d74 6f2d 6765  s both DNA-to-ge
+00001290: 6e6f 6d65 2061 6e64 2070 726f 7465 696e  nome and protein
+000012a0: 2d74 6f2d 6765 6e6f 6d65 2061 6c69 676e  -to-genome align
+000012b0: 6d65 6e74 7320 616e 6420 7072 6f64 7563  ments and produc
+000012c0: 6573 2062 6574 7465 7220 6765 6e65 206d  es better gene m
+000012d0: 6170 7069 6e67 2072 6573 756c 7473 2120  apping results! 
+000012e0: 4c69 6674 4f6e 2069 6d70 726f 7665 7320  LiftOn improves 
+000012f0: 7570 6f6e 2074 6865 2063 7572 7265 6e74  upon the current
+00001300: 2072 656c 6561 7365 6420 5432 542d 4348   released T2T-CH
+00001310: 4d31 3320 616e 6e6f 7461 7469 6f6e 2028  M13 annotation (
+00001320: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
+00001330: 6e63 6520 6578 7465 726e 616c 2220 6872  nce external" hr
+00001340: 6566 3d22 6874 7470 733a 2f2f 7333 2d75  ef="https://s3-u
+00001350: 732d 7765 7374 2d32 2e61 6d61 7a6f 6e61  s-west-2.amazona
+00001360: 7773 2e63 6f6d 2f68 756d 616e 2d70 616e  ws.com/human-pan
+00001370: 6765 6e6f 6d69 6373 2f54 3254 2f43 484d  genomics/T2T/CHM
+00001380: 3133 2f61 7373 656d 626c 6965 732f 616e  13/assemblies/an
+00001390: 6e6f 7461 7469 6f6e 2f63 686d 3133 7632  notation/chm13v2
+000013a0: 2e30 5f52 6566 5365 715f 4c69 6674 6f66  .0_RefSeq_Liftof
+000013b0: 665f 7635 2e31 2e67 6666 332e 677a 223e  f_v5.1.gff3.gz">
+000013c0: 4a48 5520 5265 6653 6571 7631 3130 202b  JHU RefSeqv110 +
+000013d0: 204c 6966 746f 6666 2076 352e 313c 2f61   Liftoff v5.1</a
+000013e0: 3e29 2e3c 2f70 3e3c 2f6c 693e 0a3c 6c69  >).</p></li>.<li
+000013f0: 3e3c 703e 3c73 7472 6f6e 673e 496d 7072  ><p><strong>Impr
+00001400: 6f76 6564 2064 6973 7461 6e74 6c79 2072  oved distantly r
+00001410: 656c 6174 6564 2073 7065 6369 6573 206c  elated species l
+00001420: 6966 742d 6f76 6572 3c2f 7374 726f 6e67  ift-over</strong
+00001430: 3e3a 2041 206b 6579 206c 696d 6974 6174  >: A key limitat
+00001440: 696f 6e20 6f66 2044 4e41 2d62 6173 6564  ion of DNA-based
+00001450: 206c 6966 742d 6f76 6572 2074 6f6f 6c73   lift-over tools
+00001460: 2069 7320 7468 6174 2074 6865 7920 646f   is that they do
+00001470: 206e 6f74 2070 6572 666f 726d 2077 656c   not perform wel
+00001480: 6c20 7768 656e 2074 6865 2072 6566 6572  l when the refer
+00001490: 656e 6365 2061 6e64 2074 6172 6765 7420  ence and target 
+000014a0: 6765 6e6f 6d65 7320 6861 7665 2073 6967  genomes have sig
+000014b0: 6e69 6669 6361 6e74 6c79 2064 6976 6572  nificantly diver
+000014c0: 6765 642e 2057 6974 6820 7468 6520 6865  ged. With the he
+000014d0: 6c70 206f 6620 7072 6f74 6569 6e20 616c  lp of protein al
+000014e0: 6967 6e6d 656e 7473 2061 6e64 2074 6865  ignments and the
+000014f0: 2070 726f 7465 696e 206d 6178 696d 697a   protein maximiz
+00001500: 6174 696f 6e20 616c 676f 7269 7468 6d2c  ation algorithm,
+00001510: 204c 6966 744f 6e20 696d 7072 6f76 6573   LiftOn improves
+00001520: 2074 6865 206c 6966 742d 6f76 6572 2070   the lift-over p
+00001530: 726f 6365 7373 2062 6574 7765 656e 2064  rocess between d
+00001540: 6973 7461 6e74 6c79 2072 656c 6174 6564  istantly related
+00001550: 2073 7065 6369 6573 2e20 5365 6520 223c   species. See "<
+00001560: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
+00001570: 6365 2069 6e74 6572 6e61 6c22 2068 7265  ce internal" hre
+00001580: 663d 2268 7474 7073 3a2f 2f63 6362 2e6a  f="https://ccb.j
+00001590: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
+000015a0: 6e74 656e 742f 6469 7374 616e 745f 7370  ntent/distant_sp
+000015b0: 6563 6965 735f 6c69 6674 6f76 6572 2f6c  ecies_liftover/l
+000015c0: 6966 746f 7665 725f 6d6f 7573 655f 325f  iftover_mouse_2_
+000015d0: 7261 742e 6874 6d6c 2364 6973 7461 6e74  rat.html#distant
+000015e0: 2d73 7065 6369 6573 2d6c 6966 746f 7665  -species-liftove
+000015f0: 722d 6d6f 7573 652d 746f 2d72 6174 223e  r-mouse-to-rat">
+00001600: 3c73 7061 6e20 636c 6173 733d 2273 7464  <span class="std
+00001610: 2073 7464 2d72 6566 223e 4d6f 7573 6520   std-ref">Mouse 
+00001620: 746f 2052 6174 3c2f 7370 616e 3e3c 2f61  to Rat</span></a
+00001630: 3e22 2061 6e64 2022 3c61 2063 6c61 7373  >" and "<a class
+00001640: 3d22 7265 6665 7265 6e63 6520 696e 7465  ="reference inte
+00001650: 726e 616c 2220 6872 6566 3d22 6874 7470  rnal" href="http
+00001660: 733a 2f2f 6363 622e 6a68 752e 6564 752f  s://ccb.jhu.edu/
+00001670: 6c69 6674 6f6e 2f63 6f6e 7465 6e74 2f64  lifton/content/d
+00001680: 6973 7461 6e74 5f73 7065 6369 6573 5f6c  istant_species_l
+00001690: 6966 746f 7665 722f 6c69 6674 6f76 6572  iftover/liftover
+000016a0: 5f64 726f 736f 7068 696c 615f 6572 6563  _drosophila_erec
+000016b0: 7461 2e68 746d 6c23 6469 7374 616e 742d  ta.html#distant-
+000016c0: 7370 6563 6965 732d 6c69 6674 6f76 6572  species-liftover
+000016d0: 2d64 726f 736f 7068 696c 612d 6d65 6c61  -drosophila-mela
+000016e0: 6e6f 6761 7374 6572 2d32 2d65 7265 6374  nogaster-2-erect
+000016f0: 6122 3e3c 7370 616e 2063 6c61 7373 3d22  a"><span class="
+00001700: 7374 6420 7374 642d 7265 6622 3e44 726f  std std-ref">Dro
+00001710: 736f 7068 696c 6120 6d65 6c61 6e6f 6761  sophila melanoga
+00001720: 7374 6572 2074 6f20 4472 6f73 6f70 6869  ster to Drosophi
+00001730: 6c61 2065 7265 6374 613c 2f73 7061 6e3e  la erecta</span>
+00001740: 3c2f 613e 2220 7265 7375 6c74 2073 6563  </a>" result sec
+00001750: 7469 6f6e 732e 3c2f 703e 3c2f 6c69 3e0a  tions.</p></li>.
+00001760: 3c2f 6f6c 3e0a 3c70 3e4c 6966 744f 6e20  </ol>.<p>LiftOn 
+00001770: 6973 2066 7265 652c 2069 7427 7320 6f70  is free, it's op
+00001780: 656e 2073 6f75 7263 652c 2069 7427 7320  en source, it's 
+00001790: 6561 7379 2074 6f20 696e 7374 616c 6c20  easy to install 
+000017a0: 2c20 616e 6420 6974 2773 2069 6e20 5079  , and it's in Py
+000017b0: 7468 6f6e 213c 2f70 3e0a 3c64 6976 2063  thon!</p>.<div c
+000017c0: 6c61 7373 3d22 6c69 6e65 2d62 6c6f 636b  lass="line-block
+000017d0: 223e 0a3c 6469 7620 636c 6173 733d 226c  ">.<div class="l
+000017e0: 696e 6522 3e3c 6272 3e3c 2f64 6976 3e0a  ine"><br></div>.
+000017f0: 3c2f 6469 763e 0a3c 2f73 6563 7469 6f6e  </div>.</section
+00001800: 3e0a 3c73 6563 7469 6f6e 2069 643d 2277  >.<section id="w
+00001810: 686f 2d69 732d 6974 2d66 6f72 2220 636c  ho-is-it-for" cl
+00001820: 6173 733d 2222 3e0a 3c68 323e 5768 6f20  ass="">.<h2>Who 
+00001830: 6973 2069 7420 666f 72e2 9d93 3c61 2063  is it for...<a c
+00001840: 6c61 7373 3d22 6865 6164 6572 6c69 6e6b  lass="headerlink
+00001850: 2220 6872 6566 3d22 2377 686f 2d69 732d  " href="#who-is-
+00001860: 6974 2d66 6f72 2220 7469 746c 653d 2250  it-for" title="P
+00001870: 6572 6d61 6c69 6e6b 2074 6f20 7468 6973  ermalink to this
+00001880: 2068 6561 6469 6e67 223e 233c 2f61 3e3c   heading">#</a><
+00001890: 2f68 323e 0a3c 703e 4c69 6674 4f6e 2069  /h2>.<p>LiftOn i
+000018a0: 7320 6465 7369 676e 6564 2066 6f72 2072  s designed for r
+000018b0: 6573 6561 7263 6865 7273 2061 6e64 2062  esearchers and b
+000018c0: 696f 696e 666f 726d 6174 6963 6961 6e73  ioinformaticians
+000018d0: 2077 686f 2061 7265 2069 6e74 6572 6573   who are interes
+000018e0: 7465 6420 696e 2067 656e 6f6d 6520 616e  ted in genome an
+000018f0: 6e6f 7461 7469 6f6e 2e20 4974 2069 7320  notation. It is 
+00001900: 616e 2065 6173 792d 746f 2d69 6e73 7461  an easy-to-insta
+00001910: 6c6c 2061 6e64 2065 6173 792d 746f 2d72  ll and easy-to-r
+00001920: 756e 2063 6f6d 6d61 6e64 2d6c 696e 6520  un command-line 
+00001930: 746f 6f6c 2e20 5370 6563 6966 6963 616c  tool. Specifical
+00001940: 6c79 2c20 6974 2069 7320 6265 6e65 6669  ly, it is benefi
+00001950: 6369 616c 2069 6e20 7468 6520 666f 6c6c  cial in the foll
+00001960: 6f77 696e 6720 7363 656e 6172 696f 733a  owing scenarios:
+00001970: 3c2f 703e 0a3c 6f6c 2063 6c61 7373 3d22  </p>.<ol class="
+00001980: 6172 6162 6963 2073 696d 706c 6522 3e0a  arabic simple">.
+00001990: 3c6c 693e 3c70 3e49 6620 796f 7520 6861  <li><p>If you ha
+000019a0: 7665 2073 6571 7565 6e63 6564 2061 6e64  ve sequenced and
+000019b0: 2061 7373 656d 626c 6564 2061 206e 6577   assembled a new
+000019c0: 2067 656e 6f6d 6520 616e 6420 7265 7175   genome and requ
+000019d0: 6972 6520 616e 6e6f 7461 7469 6f6e 2c20  ire annotation, 
+000019e0: 4c69 6674 4f6e 2070 726f 7669 6465 7320  LiftOn provides 
+000019f0: 616e 2065 6666 6963 6965 6e74 2073 6f6c  an efficient sol
+00001a00: 7574 696f 6e20 666f 7220 6765 6e65 7261  ution for genera
+00001a10: 7469 6e67 2061 6e6e 6f74 6174 696f 6e73  ting annotations
+00001a20: 2066 6f72 2079 6f75 7220 6765 6e6f 6d65   for your genome
+00001a30: 2e3c 2f70 3e3c 2f6c 693e 0a3c 6c69 3e3c  .</p></li>.<li><
+00001a40: 703e 4c69 6674 4f6e 2069 7320 616e 2065  p>LiftOn is an e
+00001a50: 7863 656c 6c65 6e74 2074 6f6f 6c20 666f  xcellent tool fo
+00001a60: 7220 7468 6f73 6520 6c6f 6f6b 696e 6720  r those looking 
+00001a70: 746f 2070 6572 666f 726d 2063 6f6d 7061  to perform compa
+00001a80: 7261 7469 7665 2067 656e 6f6d 6963 7320  rative genomics 
+00001a90: 616e 616c 7973 6973 2e20 4974 2066 6163  analysis. It fac
+00001aa0: 696c 6974 6174 6573 2074 6865 206c 6966  ilitates the lif
+00001ab0: 7469 6e67 206f 7665 7220 616e 6420 636f  ting over and co
+00001ac0: 6d70 6172 6973 6f6e 206f 6620 6765 6e65  mparison of gene
+00001ad0: 2063 6f6e 7465 6e74 7320 6265 7477 6565   contents betwee
+00001ae0: 6e20 6469 6666 6572 656e 7420 6765 6e6f  n different geno
+00001af0: 6d65 732c 2061 6964 696e 6720 696e 2075  mes, aiding in u
+00001b00: 6e64 6572 7374 616e 6469 6e67 2065 766f  nderstanding evo
+00001b10: 6c75 7469 6f6e 6172 7920 7265 6c61 7469  lutionary relati
+00001b20: 6f6e 7368 6970 7320 616e 6420 6675 6e63  onships and func
+00001b30: 7469 6f6e 616c 2067 656e 6f6d 6963 732e  tional genomics.
+00001b40: 3c2f 703e 3c2f 6c69 3e0a 3c6c 693e 3c70  </p></li>.<li><p
+00001b50: 3e46 6f72 2072 6573 6561 7263 6865 7273  >For researchers
+00001b60: 2069 6e74 6572 6573 7465 6420 696e 2075   interested in u
+00001b70: 7369 6e67 2054 3254 2d43 484d 3133 2061  sing T2T-CHM13 a
+00001b80: 6e6e 6f74 6174 696f 6e73 2c20 7472 7920  nnotations, try 
+00001b90: 4c69 6674 4f6e 2120 5765 2068 6176 6520  LiftOn! We have 
+00001ba0: 7072 652d 6765 6e65 7261 7465 6420 7468  pre-generated th
+00001bb0: 6520 3c61 2063 6c61 7373 3d22 7265 6665  e <a class="refe
+00001bc0: 7265 6e63 6520 6578 7465 726e 616c 2220  rence external" 
+00001bd0: 6872 6566 3d22 6874 7470 733a 2f2f 7469  href="https://ti
+00001be0: 6e79 7572 6c2e 636f 6d2f 3478 7977 7477  nyurl.com/4xywtw
+00001bf0: 7665 223e 4a48 555f 4c69 6674 4f6e 5f76  ve">JHU_LiftOn_v
+00001c00: 312e 305f 6368 6d31 3376 322e 302e 6766  1.0_chm13v2.0.gf
+00001c10: 6633 3c2f 613e 2028 6674 703a 2f2f 6674  f3</a> (ftp://ft
+00001c20: 702e 6363 622e 6a68 752e 6564 752f 7075  p.ccb.jhu.edu/pu
+00001c30: 622f 6461 7461 2f4c 6966 744f 6e2f 4a48  b/data/LiftOn/JH
+00001c40: 555f 4c69 6674 4f6e 5f76 312e 305f 6368  U_LiftOn_v1.0_ch
+00001c50: 6d31 3376 322e 302e 6766 6633 2920 6669  m13v2.0.gff3) fi
+00001c60: 6c65 2066 6f72 2079 6f75 7220 636f 6e76  le for your conv
+00001c70: 656e 6965 6e63 652e 3c2f 703e 3c2f 6c69  enience.</p></li
+00001c80: 3e0a 3c2f 6f6c 3e0a 3c64 6976 2063 6c61  >.</ol>.<div cla
+00001c90: 7373 3d22 6c69 6e65 2d62 6c6f 636b 223e  ss="line-block">
+00001ca0: 0a3c 6469 7620 636c 6173 733d 226c 696e  .<div class="lin
+00001cb0: 6522 3e3c 6272 3e3c 2f64 6976 3e0a 3c2f  e"><br></div>.</
+00001cc0: 6469 763e 0a3c 2f73 6563 7469 6f6e 3e0a  div>.</section>.
+00001cd0: 3c73 6563 7469 6f6e 2069 643d 2277 6861  <section id="wha
+00001ce0: 742d 646f 6573 2d6c 6966 746f 6e2d 646f  t-does-lifton-do
+00001cf0: 2220 636c 6173 733d 2222 3e0a 3c68 323e  " class="">.<h2>
+00001d00: 5768 6174 2064 6f65 7320 4c69 6674 4f6e  What does LiftOn
+00001d10: 2064 6fe2 9d93 3c61 2063 6c61 7373 3d22   do...<a class="
+00001d20: 6865 6164 6572 6c69 6e6b 2220 6872 6566  headerlink" href
+00001d30: 3d22 2377 6861 742d 646f 6573 2d6c 6966  ="#what-does-lif
+00001d40: 746f 6e2d 646f 2220 7469 746c 653d 2250  ton-do" title="P
+00001d50: 6572 6d61 6c69 6e6b 2074 6f20 7468 6973  ermalink to this
+00001d60: 2068 6561 6469 6e67 223e 233c 2f61 3e3c   heading">#</a><
+00001d70: 2f68 323e 0a3c 703e 4c65 7427 7320 6669  /h2>.<p>Let's fi
+00001d80: 7273 7420 6465 6669 6e65 2074 6865 2070  rst define the p
+00001d90: 726f 626c 656d 3a0a 4769 7665 6e20 6120  roblem:.Given a 
+00001da0: 7265 6665 7265 6e63 6520 3c73 7472 6f6e  reference <stron
+00001db0: 673e 4765 6e6f 6d65 3c2f 7374 726f 6e67  g>Genome</strong
+00001dc0: 3e20 3c73 7061 6e20 636c 6173 733d 226d  > <span class="m
+00001dd0: 6174 6820 6e6f 7472 616e 736c 6174 6520  ath notranslate 
+00001de0: 6e6f 6869 6768 6c69 6768 7422 3e3c 6d6a  nohighlight"><mj
+00001df0: 782d 636f 6e74 6169 6e65 7220 636c 6173  x-container clas
+00001e00: 733d 224d 6174 684a 6178 2043 7478 744d  s="MathJax CtxtM
+00001e10: 656e 755f 4174 7461 6368 6564 5f30 2220  enu_Attached_0" 
+00001e20: 6a61 783d 2243 4854 4d4c 2220 7461 6269  jax="CHTML" tabi
+00001e30: 6e64 6578 3d22 3022 2063 7478 746d 656e  ndex="0" ctxtmen
+00001e40: 755f 636f 756e 7465 723d 2230 2220 7374  u_counter="0" st
+00001e50: 796c 653d 2266 6f6e 742d 7369 7a65 3a20  yle="font-size: 
+00001e60: 3131 382e 3925 3b20 706f 7369 7469 6f6e  118.9%; position
+00001e70: 3a20 7265 6c61 7469 7665 3b22 3e3c 6d6a  : relative;"><mj
+00001e80: 782d 6d61 7468 2063 6c61 7373 3d22 4d4a  x-math class="MJ
+00001e90: 582d 5445 5822 2061 7269 612d 6869 6464  X-TEX" aria-hidd
+00001ea0: 656e 3d22 7472 7565 223e 3c6d 6a78 2d6d  en="true"><mjx-m
+00001eb0: 6920 636c 6173 733d 226d 6a78 2d69 223e  i class="mjx-i">
+00001ec0: 3c6d 6a78 2d63 2063 6c61 7373 3d22 6d6a  <mjx-c class="mj
+00001ed0: 782d 6331 4434 3435 2054 4558 2d49 223e  x-c1D445 TEX-I">
+00001ee0: 3c2f 6d6a 782d 633e 3c2f 6d6a 782d 6d69  </mjx-c></mjx-mi
+00001ef0: 3e3c 2f6d 6a78 2d6d 6174 683e 3c6d 6a78  ></mjx-math><mjx
+00001f00: 2d61 7373 6973 7469 7665 2d6d 6d6c 2075  -assistive-mml u
+00001f10: 6e73 656c 6563 7461 626c 653d 226f 6e22  nselectable="on"
+00001f20: 2064 6973 706c 6179 3d22 696e 6c69 6e65   display="inline
+00001f30: 223e 3c6d 6174 6820 786d 6c6e 733d 2268  "><math xmlns="h
+00001f40: 7474 703a 2f2f 7777 772e 7733 2e6f 7267  ttp://www.w3.org
+00001f50: 2f31 3939 382f 4d61 7468 2f4d 6174 684d  /1998/Math/MathM
+00001f60: 4c22 3e3c 6d69 3e52 3c2f 6d69 3e3c 2f6d  L"><mi>R</mi></m
+00001f70: 6174 683e 3c2f 6d6a 782d 6173 7369 7374  ath></mjx-assist
+00001f80: 6976 652d 6d6d 6c3e 3c2f 6d6a 782d 636f  ive-mml></mjx-co
+00001f90: 6e74 6169 6e65 723e 3c2f 7370 616e 3e2c  ntainer></span>,
+00001fa0: 2061 6e20 3c73 7472 6f6e 673e 416e 6e6f   an <strong>Anno
+00001fb0: 7461 7469 6f6e 3c2f 7374 726f 6e67 3e20  tation</strong> 
+00001fc0: 3c73 7061 6e20 636c 6173 733d 226d 6174  <span class="mat
+00001fd0: 6820 6e6f 7472 616e 736c 6174 6520 6e6f  h notranslate no
+00001fe0: 6869 6768 6c69 6768 7422 3e3c 6d6a 782d  highlight"><mjx-
+00001ff0: 636f 6e74 6169 6e65 7220 636c 6173 733d  container class=
+00002000: 224d 6174 684a 6178 2043 7478 744d 656e  "MathJax CtxtMen
+00002010: 755f 4174 7461 6368 6564 5f30 2220 6a61  u_Attached_0" ja
+00002020: 783d 2243 4854 4d4c 2220 7461 6269 6e64  x="CHTML" tabind
+00002030: 6578 3d22 3022 2063 7478 746d 656e 755f  ex="0" ctxtmenu_
+00002040: 636f 756e 7465 723d 2231 2220 7374 796c  counter="1" styl
+00002050: 653d 2266 6f6e 742d 7369 7a65 3a20 3131  e="font-size: 11
+00002060: 382e 3925 3b20 706f 7369 7469 6f6e 3a20  8.9%; position: 
+00002070: 7265 6c61 7469 7665 3b22 3e3c 6d6a 782d  relative;"><mjx-
+00002080: 6d61 7468 2063 6c61 7373 3d22 4d4a 582d  math class="MJX-
+00002090: 5445 5822 2061 7269 612d 6869 6464 656e  TEX" aria-hidden
+000020a0: 3d22 7472 7565 223e 3c6d 6a78 2d6d 7375  ="true"><mjx-msu
+000020b0: 623e 3c6d 6a78 2d6d 6920 636c 6173 733d  b><mjx-mi class=
+000020c0: 226d 6a78 2d69 223e 3c6d 6a78 2d63 2063  "mjx-i"><mjx-c c
+000020d0: 6c61 7373 3d22 6d6a 782d 6331 4434 3435  lass="mjx-c1D445
+000020e0: 2054 4558 2d49 223e 3c2f 6d6a 782d 633e   TEX-I"></mjx-c>
+000020f0: 3c2f 6d6a 782d 6d69 3e3c 6d6a 782d 7363  </mjx-mi><mjx-sc
+00002100: 7269 7074 2073 7479 6c65 3d22 7665 7274  ript style="vert
+00002110: 6963 616c 2d61 6c69 676e 3a20 2d30 2e31  ical-align: -0.1
+00002120: 3533 656d 3b22 3e3c 6d6a 782d 6d69 2063  53em;"><mjx-mi c
+00002130: 6c61 7373 3d22 6d6a 782d 6922 2073 697a  lass="mjx-i" siz
+00002140: 653d 2273 223e 3c6d 6a78 2d63 2063 6c61  e="s"><mjx-c cla
+00002150: 7373 3d22 6d6a 782d 6331 4434 3334 2054  ss="mjx-c1D434 T
+00002160: 4558 2d49 223e 3c2f 6d6a 782d 633e 3c2f  EX-I"></mjx-c></
+00002170: 6d6a 782d 6d69 3e3c 2f6d 6a78 2d73 6372  mjx-mi></mjx-scr
+00002180: 6970 743e 3c2f 6d6a 782d 6d73 7562 3e3c  ipt></mjx-msub><
+00002190: 2f6d 6a78 2d6d 6174 683e 3c6d 6a78 2d61  /mjx-math><mjx-a
+000021a0: 7373 6973 7469 7665 2d6d 6d6c 2075 6e73  ssistive-mml uns
+000021b0: 656c 6563 7461 626c 653d 226f 6e22 2064  electable="on" d
+000021c0: 6973 706c 6179 3d22 696e 6c69 6e65 223e  isplay="inline">
+000021d0: 3c6d 6174 6820 786d 6c6e 733d 2268 7474  <math xmlns="htt
+000021e0: 703a 2f2f 7777 772e 7733 2e6f 7267 2f31  p://www.w3.org/1
+000021f0: 3939 382f 4d61 7468 2f4d 6174 684d 4c22  998/Math/MathML"
+00002200: 3e3c 6d73 7562 3e3c 6d69 3e52 3c2f 6d69  ><msub><mi>R</mi
+00002210: 3e3c 6d69 3e41 3c2f 6d69 3e3c 2f6d 7375  ><mi>A</mi></msu
+00002220: 623e 3c2f 6d61 7468 3e3c 2f6d 6a78 2d61  b></math></mjx-a
+00002230: 7373 6973 7469 7665 2d6d 6d6c 3e3c 2f6d  ssistive-mml></m
+00002240: 6a78 2d63 6f6e 7461 696e 6572 3e3c 2f73  jx-container></s
+00002250: 7061 6e3e 2c20 616e 6420 6120 7461 7267  pan>, and a targ
+00002260: 6574 203c 7374 726f 6e67 3e47 656e 6f6d  et <strong>Genom
+00002270: 653c 2f73 7472 6f6e 673e 203c 7370 616e  e</strong> <span
+00002280: 2063 6c61 7373 3d22 6d61 7468 206e 6f74   class="math not
+00002290: 7261 6e73 6c61 7465 206e 6f68 6967 686c  ranslate nohighl
+000022a0: 6967 6874 223e 3c6d 6a78 2d63 6f6e 7461  ight"><mjx-conta
+000022b0: 696e 6572 2063 6c61 7373 3d22 4d61 7468  iner class="Math
+000022c0: 4a61 7820 4374 7874 4d65 6e75 5f41 7474  Jax CtxtMenu_Att
+000022d0: 6163 6865 645f 3022 206a 6178 3d22 4348  ached_0" jax="CH
+000022e0: 544d 4c22 2074 6162 696e 6465 783d 2230  TML" tabindex="0
+000022f0: 2220 6374 7874 6d65 6e75 5f63 6f75 6e74  " ctxtmenu_count
+00002300: 6572 3d22 3222 2073 7479 6c65 3d22 666f  er="2" style="fo
+00002310: 6e74 2d73 697a 653a 2031 3138 2e39 253b  nt-size: 118.9%;
+00002320: 2070 6f73 6974 696f 6e3a 2072 656c 6174   position: relat
+00002330: 6976 653b 223e 3c6d 6a78 2d6d 6174 6820  ive;"><mjx-math 
+00002340: 636c 6173 733d 224d 4a58 2d54 4558 2220  class="MJX-TEX" 
+00002350: 6172 6961 2d68 6964 6465 6e3d 2274 7275  aria-hidden="tru
+00002360: 6522 3e3c 6d6a 782d 6d69 2063 6c61 7373  e"><mjx-mi class
+00002370: 3d22 6d6a 782d 6922 3e3c 6d6a 782d 6320  ="mjx-i"><mjx-c 
+00002380: 636c 6173 733d 226d 6a78 2d63 3144 3434  class="mjx-c1D44
+00002390: 3720 5445 582d 4922 3e3c 2f6d 6a78 2d63  7 TEX-I"></mjx-c
+000023a0: 3e3c 2f6d 6a78 2d6d 693e 3c2f 6d6a 782d  ></mjx-mi></mjx-
+000023b0: 6d61 7468 3e3c 6d6a 782d 6173 7369 7374  math><mjx-assist
+000023c0: 6976 652d 6d6d 6c20 756e 7365 6c65 6374  ive-mml unselect
+000023d0: 6162 6c65 3d22 6f6e 2220 6469 7370 6c61  able="on" displa
+000023e0: 793d 2269 6e6c 696e 6522 3e3c 6d61 7468  y="inline"><math
+000023f0: 2078 6d6c 6e73 3d22 6874 7470 3a2f 2f77   xmlns="http://w
+00002400: 7777 2e77 332e 6f72 672f 3139 3938 2f4d  ww.w3.org/1998/M
+00002410: 6174 682f 4d61 7468 4d4c 223e 3c6d 693e  ath/MathML"><mi>
+00002420: 543c 2f6d 693e 3c2f 6d61 7468 3e3c 2f6d  T</mi></math></m
+00002430: 6a78 2d61 7373 6973 7469 7665 2d6d 6d6c  jx-assistive-mml
+00002440: 3e3c 2f6d 6a78 2d63 6f6e 7461 696e 6572  ></mjx-container
+00002450: 3e3c 2f73 7061 6e3e 2e20 5468 6520 6c69  ></span>. The li
+00002460: 6674 2d6f 7665 7220 7072 6f62 6c65 6d20  ft-over problem 
+00002470: 6973 2064 6566 696e 6564 2061 7320 7468  is defined as th
+00002480: 6520 7072 6f63 6573 7320 6f66 2063 6861  e process of cha
+00002490: 6e67 696e 6720 7468 6520 636f 6f72 6469  nging the coordi
+000024a0: 6e61 7465 7320 6f66 203c 7374 726f 6e67  nates of <strong
+000024b0: 3e41 6e6e 6f74 6174 696f 6e3c 2f73 7472  >Annotation</str
+000024c0: 6f6e 673e 203c 7370 616e 2063 6c61 7373  ong> <span class
+000024d0: 3d22 6d61 7468 206e 6f74 7261 6e73 6c61  ="math notransla
+000024e0: 7465 206e 6f68 6967 686c 6967 6874 223e  te nohighlight">
+000024f0: 3c6d 6a78 2d63 6f6e 7461 696e 6572 2063  <mjx-container c
+00002500: 6c61 7373 3d22 4d61 7468 4a61 7820 4374  lass="MathJax Ct
+00002510: 7874 4d65 6e75 5f41 7474 6163 6865 645f  xtMenu_Attached_
+00002520: 3022 206a 6178 3d22 4348 544d 4c22 2074  0" jax="CHTML" t
+00002530: 6162 696e 6465 783d 2230 2220 6374 7874  abindex="0" ctxt
+00002540: 6d65 6e75 5f63 6f75 6e74 6572 3d22 3322  menu_counter="3"
+00002550: 2073 7479 6c65 3d22 666f 6e74 2d73 697a   style="font-siz
+00002560: 653a 2031 3138 2e39 253b 2070 6f73 6974  e: 118.9%; posit
+00002570: 696f 6e3a 2072 656c 6174 6976 653b 223e  ion: relative;">
+00002580: 3c6d 6a78 2d6d 6174 6820 636c 6173 733d  <mjx-math class=
+00002590: 224d 4a58 2d54 4558 2220 6172 6961 2d68  "MJX-TEX" aria-h
+000025a0: 6964 6465 6e3d 2274 7275 6522 3e3c 6d6a  idden="true"><mj
+000025b0: 782d 6d73 7562 3e3c 6d6a 782d 6d69 2063  x-msub><mjx-mi c
+000025c0: 6c61 7373 3d22 6d6a 782d 6922 3e3c 6d6a  lass="mjx-i"><mj
+000025d0: 782d 6320 636c 6173 733d 226d 6a78 2d63  x-c class="mjx-c
+000025e0: 3144 3434 3520 5445 582d 4922 3e3c 2f6d  1D445 TEX-I"></m
+000025f0: 6a78 2d63 3e3c 2f6d 6a78 2d6d 693e 3c6d  jx-c></mjx-mi><m
+00002600: 6a78 2d73 6372 6970 7420 7374 796c 653d  jx-script style=
+00002610: 2276 6572 7469 6361 6c2d 616c 6967 6e3a  "vertical-align:
+00002620: 202d 302e 3135 3365 6d3b 223e 3c6d 6a78   -0.153em;"><mjx
+00002630: 2d6d 6920 636c 6173 733d 226d 6a78 2d69  -mi class="mjx-i
+00002640: 2220 7369 7a65 3d22 7322 3e3c 6d6a 782d  " size="s"><mjx-
+00002650: 6320 636c 6173 733d 226d 6a78 2d63 3144  c class="mjx-c1D
+00002660: 3433 3420 5445 582d 4922 3e3c 2f6d 6a78  434 TEX-I"></mjx
+00002670: 2d63 3e3c 2f6d 6a78 2d6d 693e 3c2f 6d6a  -c></mjx-mi></mj
+00002680: 782d 7363 7269 7074 3e3c 2f6d 6a78 2d6d  x-script></mjx-m
+00002690: 7375 623e 3c2f 6d6a 782d 6d61 7468 3e3c  sub></mjx-math><
+000026a0: 6d6a 782d 6173 7369 7374 6976 652d 6d6d  mjx-assistive-mm
+000026b0: 6c20 756e 7365 6c65 6374 6162 6c65 3d22  l unselectable="
+000026c0: 6f6e 2220 6469 7370 6c61 793d 2269 6e6c  on" display="inl
+000026d0: 696e 6522 3e3c 6d61 7468 2078 6d6c 6e73  ine"><math xmlns
+000026e0: 3d22 6874 7470 3a2f 2f77 7777 2e77 332e  ="http://www.w3.
+000026f0: 6f72 672f 3139 3938 2f4d 6174 682f 4d61  org/1998/Math/Ma
+00002700: 7468 4d4c 223e 3c6d 7375 623e 3c6d 693e  thML"><msub><mi>
+00002710: 523c 2f6d 693e 3c6d 693e 413c 2f6d 693e  R</mi><mi>A</mi>
+00002720: 3c2f 6d73 7562 3e3c 2f6d 6174 683e 3c2f  </msub></math></
+00002730: 6d6a 782d 6173 7369 7374 6976 652d 6d6d  mjx-assistive-mm
+00002740: 6c3e 3c2f 6d6a 782d 636f 6e74 6169 6e65  l></mjx-containe
+00002750: 723e 3c2f 7370 616e 3e20 6672 6f6d 203c  r></span> from <
+00002760: 7374 726f 6e67 3e47 656e 6f6d 653c 2f73  strong>Genome</s
+00002770: 7472 6f6e 673e 203c 7370 616e 2063 6c61  trong> <span cla
+00002780: 7373 3d22 6d61 7468 206e 6f74 7261 6e73  ss="math notrans
+00002790: 6c61 7465 206e 6f68 6967 686c 6967 6874  late nohighlight
+000027a0: 223e 3c6d 6a78 2d63 6f6e 7461 696e 6572  "><mjx-container
+000027b0: 2063 6c61 7373 3d22 4d61 7468 4a61 7820   class="MathJax 
+000027c0: 4374 7874 4d65 6e75 5f41 7474 6163 6865  CtxtMenu_Attache
+000027d0: 645f 3022 206a 6178 3d22 4348 544d 4c22  d_0" jax="CHTML"
+000027e0: 2074 6162 696e 6465 783d 2230 2220 6374   tabindex="0" ct
+000027f0: 7874 6d65 6e75 5f63 6f75 6e74 6572 3d22  xtmenu_counter="
+00002800: 3422 2073 7479 6c65 3d22 666f 6e74 2d73  4" style="font-s
+00002810: 697a 653a 2031 3138 2e39 253b 2070 6f73  ize: 118.9%; pos
+00002820: 6974 696f 6e3a 2072 656c 6174 6976 653b  ition: relative;
+00002830: 223e 3c6d 6a78 2d6d 6174 6820 636c 6173  "><mjx-math clas
+00002840: 733d 224d 4a58 2d54 4558 2220 6172 6961  s="MJX-TEX" aria
+00002850: 2d68 6964 6465 6e3d 2274 7275 6522 3e3c  -hidden="true"><
+00002860: 6d6a 782d 6d69 2063 6c61 7373 3d22 6d6a  mjx-mi class="mj
+00002870: 782d 6922 3e3c 6d6a 782d 6320 636c 6173  x-i"><mjx-c clas
+00002880: 733d 226d 6a78 2d63 3144 3434 3520 5445  s="mjx-c1D445 TE
+00002890: 582d 4922 3e3c 2f6d 6a78 2d63 3e3c 2f6d  X-I"></mjx-c></m
+000028a0: 6a78 2d6d 693e 3c2f 6d6a 782d 6d61 7468  jx-mi></mjx-math
+000028b0: 3e3c 6d6a 782d 6173 7369 7374 6976 652d  ><mjx-assistive-
+000028c0: 6d6d 6c20 756e 7365 6c65 6374 6162 6c65  mml unselectable
+000028d0: 3d22 6f6e 2220 6469 7370 6c61 793d 2269  ="on" display="i
+000028e0: 6e6c 696e 6522 3e3c 6d61 7468 2078 6d6c  nline"><math xml
+000028f0: 6e73 3d22 6874 7470 3a2f 2f77 7777 2e77  ns="http://www.w
+00002900: 332e 6f72 672f 3139 3938 2f4d 6174 682f  3.org/1998/Math/
+00002910: 4d61 7468 4d4c 223e 3c6d 693e 523c 2f6d  MathML"><mi>R</m
+00002920: 693e 3c2f 6d61 7468 3e3c 2f6d 6a78 2d61  i></math></mjx-a
+00002930: 7373 6973 7469 7665 2d6d 6d6c 3e3c 2f6d  ssistive-mml></m
+00002940: 6a78 2d63 6f6e 7461 696e 6572 3e3c 2f73  jx-container></s
+00002950: 7061 6e3e 2074 6f20 3c73 7472 6f6e 673e  pan> to <strong>
+00002960: 4765 6e6f 6d65 3c2f 7374 726f 6e67 3e20  Genome</strong> 
+00002970: 3c73 7061 6e20 636c 6173 733d 226d 6174  <span class="mat
+00002980: 6820 6e6f 7472 616e 736c 6174 6520 6e6f  h notranslate no
+00002990: 6869 6768 6c69 6768 7422 3e3c 6d6a 782d  highlight"><mjx-
+000029a0: 636f 6e74 6169 6e65 7220 636c 6173 733d  container class=
+000029b0: 224d 6174 684a 6178 2043 7478 744d 656e  "MathJax CtxtMen
+000029c0: 755f 4174 7461 6368 6564 5f30 2220 6a61  u_Attached_0" ja
+000029d0: 783d 2243 4854 4d4c 2220 7461 6269 6e64  x="CHTML" tabind
+000029e0: 6578 3d22 3022 2063 7478 746d 656e 755f  ex="0" ctxtmenu_
+000029f0: 636f 756e 7465 723d 2235 2220 7374 796c  counter="5" styl
+00002a00: 653d 2266 6f6e 742d 7369 7a65 3a20 3131  e="font-size: 11
+00002a10: 382e 3925 3b20 706f 7369 7469 6f6e 3a20  8.9%; position: 
+00002a20: 7265 6c61 7469 7665 3b22 3e3c 6d6a 782d  relative;"><mjx-
+00002a30: 6d61 7468 2063 6c61 7373 3d22 4d4a 582d  math class="MJX-
+00002a40: 5445 5822 2061 7269 612d 6869 6464 656e  TEX" aria-hidden
+00002a50: 3d22 7472 7565 223e 3c6d 6a78 2d6d 6920  ="true"><mjx-mi 
+00002a60: 636c 6173 733d 226d 6a78 2d69 223e 3c6d  class="mjx-i"><m
+00002a70: 6a78 2d63 2063 6c61 7373 3d22 6d6a 782d  jx-c class="mjx-
+00002a80: 6331 4434 3437 2054 4558 2d49 223e 3c2f  c1D447 TEX-I"></
+00002a90: 6d6a 782d 633e 3c2f 6d6a 782d 6d69 3e3c  mjx-c></mjx-mi><
+00002aa0: 2f6d 6a78 2d6d 6174 683e 3c6d 6a78 2d61  /mjx-math><mjx-a
+00002ab0: 7373 6973 7469 7665 2d6d 6d6c 2075 6e73  ssistive-mml uns
+00002ac0: 656c 6563 7461 626c 653d 226f 6e22 2064  electable="on" d
+00002ad0: 6973 706c 6179 3d22 696e 6c69 6e65 223e  isplay="inline">
+00002ae0: 3c6d 6174 6820 786d 6c6e 733d 2268 7474  <math xmlns="htt
+00002af0: 703a 2f2f 7777 772e 7733 2e6f 7267 2f31  p://www.w3.org/1
+00002b00: 3939 382f 4d61 7468 2f4d 6174 684d 4c22  998/Math/MathML"
+00002b10: 3e3c 6d69 3e54 3c2f 6d69 3e3c 2f6d 6174  ><mi>T</mi></mat
+00002b20: 683e 3c2f 6d6a 782d 6173 7369 7374 6976  h></mjx-assistiv
+00002b30: 652d 6d6d 6c3e 3c2f 6d6a 782d 636f 6e74  e-mml></mjx-cont
+00002b40: 6169 6e65 723e 3c2f 7370 616e 3e2c 2061  ainer></span>, a
+00002b50: 6e64 2067 656e 6572 6174 6520 6120 6e65  nd generate a ne
+00002b60: 7720 616e 6e6f 7461 7469 6f6e 2066 696c  w annotation fil
+00002b70: 6520 3c73 7472 6f6e 673e 416e 6e6f 7461  e <strong>Annota
+00002b80: 7469 6f6e 3c2f 7374 726f 6e67 3e20 3c73  tion</strong> <s
+00002b90: 7061 6e20 636c 6173 733d 226d 6174 6820  pan class="math 
+00002ba0: 6e6f 7472 616e 736c 6174 6520 6e6f 6869  notranslate nohi
+00002bb0: 6768 6c69 6768 7422 3e3c 6d6a 782d 636f  ghlight"><mjx-co
+00002bc0: 6e74 6169 6e65 7220 636c 6173 733d 224d  ntainer class="M
+00002bd0: 6174 684a 6178 2043 7478 744d 656e 755f  athJax CtxtMenu_
+00002be0: 4174 7461 6368 6564 5f30 2220 6a61 783d  Attached_0" jax=
+00002bf0: 2243 4854 4d4c 2220 7461 6269 6e64 6578  "CHTML" tabindex
+00002c00: 3d22 3022 2063 7478 746d 656e 755f 636f  ="0" ctxtmenu_co
+00002c10: 756e 7465 723d 2236 2220 7374 796c 653d  unter="6" style=
+00002c20: 2266 6f6e 742d 7369 7a65 3a20 3131 382e  "font-size: 118.
+00002c30: 3925 3b20 706f 7369 7469 6f6e 3a20 7265  9%; position: re
+00002c40: 6c61 7469 7665 3b22 3e3c 6d6a 782d 6d61  lative;"><mjx-ma
+00002c50: 7468 2063 6c61 7373 3d22 4d4a 582d 5445  th class="MJX-TE
+00002c60: 5822 2061 7269 612d 6869 6464 656e 3d22  X" aria-hidden="
+00002c70: 7472 7565 223e 3c6d 6a78 2d6d 7375 623e  true"><mjx-msub>
+00002c80: 3c6d 6a78 2d6d 6920 636c 6173 733d 226d  <mjx-mi class="m
+00002c90: 6a78 2d69 223e 3c6d 6a78 2d63 2063 6c61  jx-i"><mjx-c cla
+00002ca0: 7373 3d22 6d6a 782d 6331 4434 3437 2054  ss="mjx-c1D447 T
+00002cb0: 4558 2d49 223e 3c2f 6d6a 782d 633e 3c2f  EX-I"></mjx-c></
+00002cc0: 6d6a 782d 6d69 3e3c 6d6a 782d 7363 7269  mjx-mi><mjx-scri
+00002cd0: 7074 2073 7479 6c65 3d22 7665 7274 6963  pt style="vertic
+00002ce0: 616c 2d61 6c69 676e 3a20 2d30 2e31 3533  al-align: -0.153
+00002cf0: 656d 3b20 6d61 7267 696e 2d6c 6566 743a  em; margin-left:
+00002d00: 202d 302e 3132 656d 3b22 3e3c 6d6a 782d   -0.12em;"><mjx-
+00002d10: 6d69 2063 6c61 7373 3d22 6d6a 782d 6922  mi class="mjx-i"
+00002d20: 2073 697a 653d 2273 223e 3c6d 6a78 2d63   size="s"><mjx-c
+00002d30: 2063 6c61 7373 3d22 6d6a 782d 6331 4434   class="mjx-c1D4
+00002d40: 3334 2054 4558 2d49 223e 3c2f 6d6a 782d  34 TEX-I"></mjx-
+00002d50: 633e 3c2f 6d6a 782d 6d69 3e3c 2f6d 6a78  c></mjx-mi></mjx
+00002d60: 2d73 6372 6970 743e 3c2f 6d6a 782d 6d73  -script></mjx-ms
+00002d70: 7562 3e3c 2f6d 6a78 2d6d 6174 683e 3c6d  ub></mjx-math><m
+00002d80: 6a78 2d61 7373 6973 7469 7665 2d6d 6d6c  jx-assistive-mml
+00002d90: 2075 6e73 656c 6563 7461 626c 653d 226f   unselectable="o
+00002da0: 6e22 2064 6973 706c 6179 3d22 696e 6c69  n" display="inli
+00002db0: 6e65 223e 3c6d 6174 6820 786d 6c6e 733d  ne"><math xmlns=
+00002dc0: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
+00002dd0: 7267 2f31 3939 382f 4d61 7468 2f4d 6174  rg/1998/Math/Mat
+00002de0: 684d 4c22 3e3c 6d73 7562 3e3c 6d69 3e54  hML"><msub><mi>T
+00002df0: 3c2f 6d69 3e3c 6d69 3e41 3c2f 6d69 3e3c  </mi><mi>A</mi><
+00002e00: 2f6d 7375 623e 3c2f 6d61 7468 3e3c 2f6d  /msub></math></m
+00002e10: 6a78 2d61 7373 6973 7469 7665 2d6d 6d6c  jx-assistive-mml
+00002e20: 3e3c 2f6d 6a78 2d63 6f6e 7461 696e 6572  ></mjx-container
+00002e30: 3e3c 2f73 7061 6e3e 2e20 4120 7369 6d70  ></span>. A simp
+00002e40: 6c65 2069 6c6c 7573 7472 6174 696f 6e20  le illustration 
+00002e50: 6f66 2074 6865 206c 6966 742d 6f76 6572  of the lift-over
+00002e60: 2070 726f 626c 656d 2069 7320 7368 6f77   problem is show
+00002e70: 6e20 696e 203c 6120 636c 6173 733d 2272  n in <a class="r
+00002e80: 6566 6572 656e 6365 2069 6e74 6572 6e61  eference interna
+00002e90: 6c22 2068 7265 663d 2223 6c69 6674 6f76  l" href="#liftov
+00002ea0: 6572 2d69 6c6c 7573 7472 6174 696f 6e22  er-illustration"
+00002eb0: 3e3c 7370 616e 2063 6c61 7373 3d22 7374  ><span class="st
+00002ec0: 6420 7374 642d 6e75 6d72 6566 223e 4669  d std-numref">Fi
+00002ed0: 6775 7265 2031 3c2f 7370 616e 3e3c 2f61  gure 1</span></a
+00002ee0: 3e2e 3c2f 703e 0a3c 6669 6775 7265 2063  >.</p>.<figure c
+00002ef0: 6c61 7373 3d22 616c 6967 6e2d 6365 6e74  lass="align-cent
+00002f00: 6572 2220 6964 3d22 6964 3422 3e0a 3c66  er" id="id4">.<f
+00002f10: 6967 6361 7074 696f 6e3e 0a3c 7370 616e  igcaption>.<span
+00002f20: 2069 643d 226c 6966 746f 7665 722d 696c   id="liftover-il
+00002f30: 6c75 7374 7261 7469 6f6e 223e 3c2f 7370  lustration"></sp
+00002f40: 616e 3e3c 6120 636c 6173 733d 2272 6566  an><a class="ref
+00002f50: 6572 656e 6365 2069 6e74 6572 6e61 6c20  erence internal 
+00002f60: 696d 6167 652d 7265 6665 7265 6e63 6522  image-reference"
+00002f70: 2068 7265 663d 2268 7474 7073 3a2f 2f73   href="https://s
+00002f80: 746f 7261 6765 2e67 6f6f 676c 6561 7069  torage.googleapi
+00002f90: 732e 636f 6d2f 7374 6f72 6167 652e 6b68  s.com/storage.kh
+00002fa0: 6368 616f 2e63 6f6d 2f66 6967 7572 6573  chao.com/figures
+00002fb0: 2f4c 6966 744f 6e2f 6c69 6674 6f76 6572  /LiftOn/liftover
+00002fc0: 5f69 6c6c 7573 7472 6174 696f 6e2e 6769  _illustration.gi
+00002fd0: 6622 3e3c 696d 6720 616c 743d 2267 7261  f"><img alt="gra
+00002fe0: 7068 6963 732f 6c69 6674 6f76 6572 5f69  phics/liftover_i
+00002ff0: 6c6c 7573 7472 6174 696f 6e2e 6769 6622  llustration.gif"
+00003000: 2073 7263 3d22 6874 7470 733a 2f2f 7374   src="https://st
+00003010: 6f72 6167 652e 676f 6f67 6c65 6170 6973  orage.googleapis
+00003020: 2e63 6f6d 2f73 746f 7261 6765 2e6b 6863  .com/storage.khc
+00003030: 6861 6f2e 636f 6d2f 6669 6775 7265 732f  hao.com/figures/
+00003040: 4c69 6674 4f6e 2f6c 6966 746f 7665 725f  LiftOn/liftover_
+00003050: 696c 6c75 7374 7261 7469 6f6e 2e67 6966  illustration.gif
+00003060: 2220 7374 796c 653d 2277 6964 7468 3a20  " style="width: 
+00003070: 3637 322e 3570 783b 2068 6569 6768 743a  672.5px; height:
+00003080: 2032 3730 2e30 7078 3b22 3e3c 2f61 3e0a   270.0px;"></a>.
+00003090: 3c2f 6669 6763 6170 7469 6f6e 3e0a 3c2f  </figcaption>.</
+000030a0: 6669 6775 7265 3e0a 3c64 6976 2063 6c61  figure>.<div cla
+000030b0: 7373 3d22 6c69 6e65 2d62 6c6f 636b 223e  ss="line-block">
+000030c0: 0a3c 6469 7620 636c 6173 733d 226c 696e  .<div class="lin
+000030d0: 6522 3e3c 6272 3e3c 2f64 6976 3e0a 3c2f  e"><br></div>.</
+000030e0: 6469 763e 0a3c 703e 4c69 6674 4f6e 2069  div>.<p>LiftOn i
+000030f0: 7320 7468 6520 6265 7374 2074 6f6f 6c20  s the best tool 
+00003100: 746f 2068 656c 7020 796f 7520 736f 6c76  to help you solv
+00003110: 6520 7468 6973 2070 726f 626c 656d 2120  e this problem! 
+00003120: 4c69 6674 4f6e 2065 6d70 6c6f 7973 2061  LiftOn employs a
+00003130: 2074 776f 2d73 7465 7020 3c61 2063 6c61   two-step <a cla
+00003140: 7373 3d22 7265 6665 7265 6e63 6520 696e  ss="reference in
+00003150: 7465 726e 616c 2220 6872 6566 3d22 6874  ternal" href="ht
+00003160: 7470 733a 2f2f 6363 622e 6a68 752e 6564  tps://ccb.jhu.ed
+00003170: 752f 6c69 6674 6f6e 2f63 6f6e 7465 6e74  u/lifton/content
+00003180: 2f62 6568 696e 645f 7363 656e 6573 2e68  /behind_scenes.h
+00003190: 746d 6c23 7072 6f74 6569 6e2d 6d61 7869  tml#protein-maxi
+000031a0: 6d69 7a61 7469 6f6e 2d61 6c67 6f72 6974  mization-algorit
+000031b0: 686d 223e 3c73 7061 6e20 636c 6173 733d  hm"><span class=
+000031c0: 2273 7464 2073 7464 2d72 6566 223e 7072  "std std-ref">pr
+000031d0: 6f74 6569 6e20 6d61 7869 6d69 7a61 7469  otein maximizati
+000031e0: 6f6e 2061 6c67 6f72 6974 686d 3c2f 7370  on algorithm</sp
+000031f0: 616e 3e3c 2f61 3e20 2850 4d20 616c 676f  an></a> (PM algo
+00003200: 7269 7468 6d29 2e3c 2f70 3e0a 3c6f 6c20  rithm).</p>.<ol 
+00003210: 636c 6173 733d 2261 7261 6269 6320 7369  class="arabic si
+00003220: 6d70 6c65 223e 0a3c 6c69 3e3c 703e 5468  mple">.<li><p>Th
+00003230: 6520 6669 7273 7420 6d6f 6475 6c65 2069  e first module i
+00003240: 7320 7468 6520 3c65 6d3e 6368 6169 6e69  s the <em>chaini
+00003250: 6e67 2061 6c67 6f72 6974 686d 3c2f 656d  ng algorithm</em
+00003260: 3e2e 2049 7420 7374 6172 7473 2062 7920  >. It starts by 
+00003270: 6578 7472 6163 7469 6e67 2070 726f 7465  extracting prote
+00003280: 696e 2073 6571 7565 6e63 6573 2061 6e6e  in sequences ann
+00003290: 6f74 6174 6564 2062 7920 4c69 6674 6f66  otated by Liftof
+000032a0: 6620 616e 6420 6d69 6e69 7072 6f74 2e20  f and miniprot. 
+000032b0: 4c69 6674 4f6e 2074 6865 6e20 616c 6967  LiftOn then alig
+000032c0: 6e73 2074 6865 7365 2073 6571 7565 6e63  ns these sequenc
+000032d0: 6573 2074 6f20 6675 6c6c 2d6c 656e 6774  es to full-lengt
+000032e0: 6820 7265 6665 7265 6e63 6520 7072 6f74  h reference prot
+000032f0: 6569 6e73 2e20 466f 7220 6561 6368 2067  eins. For each g
+00003300: 656e 6520 6c6f 6375 732c 204c 6966 744f  ene locus, LiftO
+00003310: 6e20 636f 6d70 6172 6573 2065 6163 6820  n compares each 
+00003320: 7365 6374 696f 6e20 6f66 2074 6865 2070  section of the p
+00003330: 726f 7465 696e 2061 6c69 676e 6d65 6e74  rotein alignment
+00003340: 7320 6672 6f6d 204c 6966 746f 6666 2061  s from Liftoff a
+00003350: 6e64 206d 696e 6970 726f 742c 2063 6861  nd miniprot, cha
+00003360: 696e 696e 6720 746f 6765 7468 6572 2074  ining together t
+00003370: 6865 2062 6573 7420 636f 6d62 696e 6174  he best combinat
+00003380: 696f 6e73 2e3c 2f70 3e3c 2f6c 693e 0a3c  ions.</p></li>.<
+00003390: 6c69 3e3c 703e 5468 6520 7365 636f 6e64  li><p>The second
+000033a0: 206d 6f64 756c 6520 6973 2074 6865 203c   module is the <
+000033b0: 656d 3e6f 7065 6e2d 7265 6164 696e 6720  em>open-reading 
+000033c0: 6672 616d 6520 7365 6172 6368 2028 4f52  frame search (OR
+000033d0: 4620 7365 6172 6368 2920 616c 676f 7269  F search) algori
+000033e0: 7468 6d3c 2f65 6d3e 2e20 496e 2074 6865  thm</em>. In the
+000033f0: 2063 6173 6520 6f66 2074 7275 6e63 6174   case of truncat
+00003400: 6564 2070 726f 7465 696e 2d63 6f64 696e  ed protein-codin
+00003410: 6720 7472 616e 7363 7269 7074 732c 2074  g transcripts, t
+00003420: 6869 7320 616c 676f 7269 7468 6d20 6578  his algorithm ex
+00003430: 616d 696e 6573 2061 6c74 6572 6e61 7469  amines alternati
+00003440: 7665 2066 7261 6d65 7320 746f 2069 6465  ve frames to ide
+00003450: 6e74 6966 7920 7468 6520 4f52 4620 7468  ntify the ORF th
+00003460: 6174 2070 726f 6475 6365 7320 7468 6520  at produces the 
+00003470: 6c6f 6e67 6573 7420 6d61 7463 6820 7769  longest match wi
+00003480: 7468 2074 6865 2072 6566 6572 656e 6365  th the reference
+00003490: 2070 726f 7465 696e 2e3c 2f70 3e3c 2f6c   protein.</p></l
+000034a0: 693e 0a3c 2f6f 6c3e 0a3c 6469 7620 636c  i>.</ol>.<div cl
+000034b0: 6173 733d 226c 696e 652d 626c 6f63 6b22  ass="line-block"
+000034c0: 3e0a 3c64 6976 2063 6c61 7373 3d22 6c69  >.<div class="li
+000034d0: 6e65 223e 3c62 723e 3c2f 6469 763e 0a3c  ne"><br></div>.<
+000034e0: 2f64 6976 3e0a 3c2f 7365 6374 696f 6e3e  /div>.</section>
+000034f0: 0a3c 7365 6374 696f 6e20 6964 3d22 696e  .<section id="in
+00003500: 7075 7473 2d6f 7574 7075 7473 2220 636c  puts-outputs" cl
+00003510: 6173 733d 2222 3e0a 3c68 323e 496e 7075  ass="">.<h2>Inpu
+00003520: 7473 2026 616d 703b 206f 7574 7075 7473  ts &amp; outputs
+00003530: 3c61 2063 6c61 7373 3d22 6865 6164 6572  <a class="header
+00003540: 6c69 6e6b 2220 6872 6566 3d22 2369 6e70  link" href="#inp
+00003550: 7574 732d 6f75 7470 7574 7322 2074 6974  uts-outputs" tit
+00003560: 6c65 3d22 5065 726d 616c 696e 6b20 746f  le="Permalink to
+00003570: 2074 6869 7320 6865 6164 696e 6722 3e23   this heading">#
+00003580: 3c2f 613e 3c2f 6832 3e0a 3c75 6c20 636c  </a></h2>.<ul cl
+00003590: 6173 733d 2273 696d 706c 6522 3e0a 3c6c  ass="simple">.<l
+000035a0: 693e 3c64 6c20 636c 6173 733d 2273 696d  i><dl class="sim
+000035b0: 706c 6522 3e0a 3c64 743e 3c73 7472 6f6e  ple">.<dt><stron
+000035c0: 673e 496e 7075 743c 2f73 7472 6f6e 673e  g>Input</strong>
+000035d0: 3a3c 2f64 743e 3c64 643e 3c6f 6c20 636c  :</dt><dd><ol cl
+000035e0: 6173 733d 2261 7261 6269 6320 7369 6d70  ass="arabic simp
+000035f0: 6c65 223e 0a3c 6c69 3e3c 703e 7461 7267  le">.<li><p>targ
+00003600: 6574 203c 7374 726f 6e67 3e47 656e 6f6d  et <strong>Genom
+00003610: 653c 2f73 7472 6f6e 673e 203c 7370 616e  e</strong> <span
+00003620: 2063 6c61 7373 3d22 6d61 7468 206e 6f74   class="math not
+00003630: 7261 6e73 6c61 7465 206e 6f68 6967 686c  ranslate nohighl
+00003640: 6967 6874 223e 3c6d 6a78 2d63 6f6e 7461  ight"><mjx-conta
+00003650: 696e 6572 2063 6c61 7373 3d22 4d61 7468  iner class="Math
+00003660: 4a61 7820 4374 7874 4d65 6e75 5f41 7474  Jax CtxtMenu_Att
+00003670: 6163 6865 645f 3022 206a 6178 3d22 4348  ached_0" jax="CH
+00003680: 544d 4c22 2074 6162 696e 6465 783d 2230  TML" tabindex="0
+00003690: 2220 6374 7874 6d65 6e75 5f63 6f75 6e74  " ctxtmenu_count
+000036a0: 6572 3d22 3722 2073 7479 6c65 3d22 666f  er="7" style="fo
+000036b0: 6e74 2d73 697a 653a 2031 3138 2e39 253b  nt-size: 118.9%;
+000036c0: 2070 6f73 6974 696f 6e3a 2072 656c 6174   position: relat
+000036d0: 6976 653b 223e 3c6d 6a78 2d6d 6174 6820  ive;"><mjx-math 
+000036e0: 636c 6173 733d 224d 4a58 2d54 4558 2220  class="MJX-TEX" 
+000036f0: 6172 6961 2d68 6964 6465 6e3d 2274 7275  aria-hidden="tru
+00003700: 6522 3e3c 6d6a 782d 6d69 2063 6c61 7373  e"><mjx-mi class
+00003710: 3d22 6d6a 782d 6922 3e3c 6d6a 782d 6320  ="mjx-i"><mjx-c 
+00003720: 636c 6173 733d 226d 6a78 2d63 3144 3434  class="mjx-c1D44
+00003730: 3720 5445 582d 4922 3e3c 2f6d 6a78 2d63  7 TEX-I"></mjx-c
+00003740: 3e3c 2f6d 6a78 2d6d 693e 3c2f 6d6a 782d  ></mjx-mi></mjx-
+00003750: 6d61 7468 3e3c 6d6a 782d 6173 7369 7374  math><mjx-assist
+00003760: 6976 652d 6d6d 6c20 756e 7365 6c65 6374  ive-mml unselect
+00003770: 6162 6c65 3d22 6f6e 2220 6469 7370 6c61  able="on" displa
+00003780: 793d 2269 6e6c 696e 6522 3e3c 6d61 7468  y="inline"><math
+00003790: 2078 6d6c 6e73 3d22 6874 7470 3a2f 2f77   xmlns="http://w
+000037a0: 7777 2e77 332e 6f72 672f 3139 3938 2f4d  ww.w3.org/1998/M
+000037b0: 6174 682f 4d61 7468 4d4c 223e 3c6d 693e  ath/MathML"><mi>
+000037c0: 543c 2f6d 693e 3c2f 6d61 7468 3e3c 2f6d  T</mi></math></m
+000037d0: 6a78 2d61 7373 6973 7469 7665 2d6d 6d6c  jx-assistive-mml
+000037e0: 3e3c 2f6d 6a78 2d63 6f6e 7461 696e 6572  ></mjx-container
+000037f0: 3e3c 2f73 7061 6e3e 2069 6e20 4641 5354  ></span> in FAST
+00003800: 4120 666f 726d 6174 2e3c 2f70 3e3c 2f6c  A format.</p></l
+00003810: 693e 0a3c 6c69 3e3c 703e 7265 6665 7265  i>.<li><p>refere
+00003820: 6e63 6520 3c73 7472 6f6e 673e 4765 6e6f  nce <strong>Geno
+00003830: 6d65 3c2f 7374 726f 6e67 3e20 3c73 7061  me</strong> <spa
+00003840: 6e20 636c 6173 733d 226d 6174 6820 6e6f  n class="math no
+00003850: 7472 616e 736c 6174 6520 6e6f 6869 6768  translate nohigh
+00003860: 6c69 6768 7422 3e3c 6d6a 782d 636f 6e74  light"><mjx-cont
+00003870: 6169 6e65 7220 636c 6173 733d 224d 6174  ainer class="Mat
+00003880: 684a 6178 2043 7478 744d 656e 755f 4174  hJax CtxtMenu_At
+00003890: 7461 6368 6564 5f30 2220 6a61 783d 2243  tached_0" jax="C
+000038a0: 4854 4d4c 2220 7461 6269 6e64 6578 3d22  HTML" tabindex="
+000038b0: 3022 2063 7478 746d 656e 755f 636f 756e  0" ctxtmenu_coun
+000038c0: 7465 723d 2238 2220 7374 796c 653d 2266  ter="8" style="f
+000038d0: 6f6e 742d 7369 7a65 3a20 3131 382e 3925  ont-size: 118.9%
+000038e0: 3b20 706f 7369 7469 6f6e 3a20 7265 6c61  ; position: rela
+000038f0: 7469 7665 3b22 3e3c 6d6a 782d 6d61 7468  tive;"><mjx-math
+00003900: 2063 6c61 7373 3d22 4d4a 582d 5445 5822   class="MJX-TEX"
+00003910: 2061 7269 612d 6869 6464 656e 3d22 7472   aria-hidden="tr
+00003920: 7565 223e 3c6d 6a78 2d6d 6920 636c 6173  ue"><mjx-mi clas
+00003930: 733d 226d 6a78 2d69 223e 3c6d 6a78 2d63  s="mjx-i"><mjx-c
+00003940: 2063 6c61 7373 3d22 6d6a 782d 6331 4434   class="mjx-c1D4
+00003950: 3435 2054 4558 2d49 223e 3c2f 6d6a 782d  45 TEX-I"></mjx-
+00003960: 633e 3c2f 6d6a 782d 6d69 3e3c 2f6d 6a78  c></mjx-mi></mjx
+00003970: 2d6d 6174 683e 3c6d 6a78 2d61 7373 6973  -math><mjx-assis
+00003980: 7469 7665 2d6d 6d6c 2075 6e73 656c 6563  tive-mml unselec
+00003990: 7461 626c 653d 226f 6e22 2064 6973 706c  table="on" displ
+000039a0: 6179 3d22 696e 6c69 6e65 223e 3c6d 6174  ay="inline"><mat
+000039b0: 6820 786d 6c6e 733d 2268 7474 703a 2f2f  h xmlns="http://
+000039c0: 7777 772e 7733 2e6f 7267 2f31 3939 382f  www.w3.org/1998/
+000039d0: 4d61 7468 2f4d 6174 684d 4c22 3e3c 6d69  Math/MathML"><mi
+000039e0: 3e52 3c2f 6d69 3e3c 2f6d 6174 683e 3c2f  >R</mi></math></
+000039f0: 6d6a 782d 6173 7369 7374 6976 652d 6d6d  mjx-assistive-mm
+00003a00: 6c3e 3c2f 6d6a 782d 636f 6e74 6169 6e65  l></mjx-containe
+00003a10: 723e 3c2f 7370 616e 3e20 696e 2046 4153  r></span> in FAS
+00003a20: 5441 2066 6f72 6d61 742e 3c2f 703e 3c2f  TA format.</p></
+00003a30: 6c69 3e0a 3c6c 693e 3c70 3e72 6566 6572  li>.<li><p>refer
+00003a40: 656e 6365 203c 7374 726f 6e67 3e41 6e6e  ence <strong>Ann
+00003a50: 6f74 6174 696f 6e3c 2f73 7472 6f6e 673e  otation</strong>
+00003a60: 203c 7370 616e 2063 6c61 7373 3d22 6d61   <span class="ma
+00003a70: 7468 206e 6f74 7261 6e73 6c61 7465 206e  th notranslate n
+00003a80: 6f68 6967 686c 6967 6874 223e 3c6d 6a78  ohighlight"><mjx
+00003a90: 2d63 6f6e 7461 696e 6572 2063 6c61 7373  -container class
+00003aa0: 3d22 4d61 7468 4a61 7820 4374 7874 4d65  ="MathJax CtxtMe
+00003ab0: 6e75 5f41 7474 6163 6865 645f 3022 206a  nu_Attached_0" j
+00003ac0: 6178 3d22 4348 544d 4c22 2074 6162 696e  ax="CHTML" tabin
+00003ad0: 6465 783d 2230 2220 6374 7874 6d65 6e75  dex="0" ctxtmenu
+00003ae0: 5f63 6f75 6e74 6572 3d22 3922 2073 7479  _counter="9" sty
+00003af0: 6c65 3d22 666f 6e74 2d73 697a 653a 2031  le="font-size: 1
+00003b00: 3138 2e39 253b 2070 6f73 6974 696f 6e3a  18.9%; position:
+00003b10: 2072 656c 6174 6976 653b 223e 3c6d 6a78   relative;"><mjx
+00003b20: 2d6d 6174 6820 636c 6173 733d 224d 4a58  -math class="MJX
+00003b30: 2d54 4558 2220 6172 6961 2d68 6964 6465  -TEX" aria-hidde
+00003b40: 6e3d 2274 7275 6522 3e3c 6d6a 782d 6d73  n="true"><mjx-ms
+00003b50: 7562 3e3c 6d6a 782d 6d69 2063 6c61 7373  ub><mjx-mi class
+00003b60: 3d22 6d6a 782d 6922 3e3c 6d6a 782d 6320  ="mjx-i"><mjx-c 
+00003b70: 636c 6173 733d 226d 6a78 2d63 3144 3434  class="mjx-c1D44
+00003b80: 3520 5445 582d 4922 3e3c 2f6d 6a78 2d63  5 TEX-I"></mjx-c
+00003b90: 3e3c 2f6d 6a78 2d6d 693e 3c6d 6a78 2d73  ></mjx-mi><mjx-s
+00003ba0: 6372 6970 7420 7374 796c 653d 2276 6572  cript style="ver
+00003bb0: 7469 6361 6c2d 616c 6967 6e3a 202d 302e  tical-align: -0.
+00003bc0: 3135 3365 6d3b 223e 3c6d 6a78 2d6d 6920  153em;"><mjx-mi 
+00003bd0: 636c 6173 733d 226d 6a78 2d69 2220 7369  class="mjx-i" si
+00003be0: 7a65 3d22 7322 3e3c 6d6a 782d 6320 636c  ze="s"><mjx-c cl
+00003bf0: 6173 733d 226d 6a78 2d63 3144 3433 3420  ass="mjx-c1D434 
+00003c00: 5445 582d 4922 3e3c 2f6d 6a78 2d63 3e3c  TEX-I"></mjx-c><
+00003c10: 2f6d 6a78 2d6d 693e 3c2f 6d6a 782d 7363  /mjx-mi></mjx-sc
+00003c20: 7269 7074 3e3c 2f6d 6a78 2d6d 7375 623e  ript></mjx-msub>
+00003c30: 3c2f 6d6a 782d 6d61 7468 3e3c 6d6a 782d  </mjx-math><mjx-
+00003c40: 6173 7369 7374 6976 652d 6d6d 6c20 756e  assistive-mml un
+00003c50: 7365 6c65 6374 6162 6c65 3d22 6f6e 2220  selectable="on" 
+00003c60: 6469 7370 6c61 793d 2269 6e6c 696e 6522  display="inline"
+00003c70: 3e3c 6d61 7468 2078 6d6c 6e73 3d22 6874  ><math xmlns="ht
+00003c80: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
+00003c90: 3139 3938 2f4d 6174 682f 4d61 7468 4d4c  1998/Math/MathML
+00003ca0: 223e 3c6d 7375 623e 3c6d 693e 523c 2f6d  "><msub><mi>R</m
+00003cb0: 693e 3c6d 693e 413c 2f6d 693e 3c2f 6d73  i><mi>A</mi></ms
+00003cc0: 7562 3e3c 2f6d 6174 683e 3c2f 6d6a 782d  ub></math></mjx-
+00003cd0: 6173 7369 7374 6976 652d 6d6d 6c3e 3c2f  assistive-mml></
+00003ce0: 6d6a 782d 636f 6e74 6169 6e65 723e 3c2f  mjx-container></
+00003cf0: 7370 616e 3e20 696e 2047 4646 3320 666f  span> in GFF3 fo
+00003d00: 726d 6174 2e3c 2f70 3e3c 2f6c 693e 0a3c  rmat.</p></li>.<
+00003d10: 2f6f 6c3e 0a3c 2f64 643e 0a3c 2f64 6c3e  /ol>.</dd>.</dl>
+00003d20: 0a3c 2f6c 693e 0a3c 6c69 3e3c 646c 2063  .</li>.<li><dl c
+00003d30: 6c61 7373 3d22 7369 6d70 6c65 223e 0a3c  lass="simple">.<
+00003d40: 6474 3e3c 7374 726f 6e67 3e4f 7574 7075  dt><strong>Outpu
+00003d50: 743c 2f73 7472 6f6e 673e 3a3c 2f64 743e  t</strong>:</dt>
+00003d60: 3c64 643e 3c6f 6c20 636c 6173 733d 2261  <dd><ol class="a
+00003d70: 7261 6269 6320 7369 6d70 6c65 223e 0a3c  rabic simple">.<
+00003d80: 6c69 3e3c 703e 4c69 6674 4f6e 2061 6e6e  li><p>LiftOn ann
+00003d90: 6f74 6174 696f 6e20 6669 6c65 2c20 3c73  otation file, <s
+00003da0: 7472 6f6e 673e 416e 6e6f 7461 7469 6f6e  trong>Annotation
+00003db0: 3c2f 7374 726f 6e67 3e20 3c73 7061 6e20  </strong> <span 
+00003dc0: 636c 6173 733d 226d 6174 6820 6e6f 7472  class="math notr
+00003dd0: 616e 736c 6174 6520 6e6f 6869 6768 6c69  anslate nohighli
+00003de0: 6768 7422 3e3c 6d6a 782d 636f 6e74 6169  ght"><mjx-contai
+00003df0: 6e65 7220 636c 6173 733d 224d 6174 684a  ner class="MathJ
+00003e00: 6178 2043 7478 744d 656e 755f 4174 7461  ax CtxtMenu_Atta
+00003e10: 6368 6564 5f30 2220 6a61 783d 2243 4854  ched_0" jax="CHT
+00003e20: 4d4c 2220 7461 6269 6e64 6578 3d22 3022  ML" tabindex="0"
+00003e30: 2063 7478 746d 656e 755f 636f 756e 7465   ctxtmenu_counte
+00003e40: 723d 2231 3022 2073 7479 6c65 3d22 666f  r="10" style="fo
+00003e50: 6e74 2d73 697a 653a 2031 3138 2e39 253b  nt-size: 118.9%;
+00003e60: 2070 6f73 6974 696f 6e3a 2072 656c 6174   position: relat
+00003e70: 6976 653b 223e 3c6d 6a78 2d6d 6174 6820  ive;"><mjx-math 
+00003e80: 636c 6173 733d 224d 4a58 2d54 4558 2220  class="MJX-TEX" 
+00003e90: 6172 6961 2d68 6964 6465 6e3d 2274 7275  aria-hidden="tru
+00003ea0: 6522 3e3c 6d6a 782d 6d73 7562 3e3c 6d6a  e"><mjx-msub><mj
+00003eb0: 782d 6d69 2063 6c61 7373 3d22 6d6a 782d  x-mi class="mjx-
+00003ec0: 6922 3e3c 6d6a 782d 6320 636c 6173 733d  i"><mjx-c class=
+00003ed0: 226d 6a78 2d63 3144 3434 3720 5445 582d  "mjx-c1D447 TEX-
+00003ee0: 4922 3e3c 2f6d 6a78 2d63 3e3c 2f6d 6a78  I"></mjx-c></mjx
+00003ef0: 2d6d 693e 3c6d 6a78 2d73 6372 6970 7420  -mi><mjx-script 
+00003f00: 7374 796c 653d 2276 6572 7469 6361 6c2d  style="vertical-
+00003f10: 616c 6967 6e3a 202d 302e 3135 3365 6d3b  align: -0.153em;
+00003f20: 206d 6172 6769 6e2d 6c65 6674 3a20 2d30   margin-left: -0
+00003f30: 2e31 3265 6d3b 223e 3c6d 6a78 2d6d 6920  .12em;"><mjx-mi 
+00003f40: 636c 6173 733d 226d 6a78 2d69 2220 7369  class="mjx-i" si
+00003f50: 7a65 3d22 7322 3e3c 6d6a 782d 6320 636c  ze="s"><mjx-c cl
+00003f60: 6173 733d 226d 6a78 2d63 3144 3433 3420  ass="mjx-c1D434 
+00003f70: 5445 582d 4922 3e3c 2f6d 6a78 2d63 3e3c  TEX-I"></mjx-c><
+00003f80: 2f6d 6a78 2d6d 693e 3c2f 6d6a 782d 7363  /mjx-mi></mjx-sc
+00003f90: 7269 7074 3e3c 2f6d 6a78 2d6d 7375 623e  ript></mjx-msub>
+00003fa0: 3c2f 6d6a 782d 6d61 7468 3e3c 6d6a 782d  </mjx-math><mjx-
+00003fb0: 6173 7369 7374 6976 652d 6d6d 6c20 756e  assistive-mml un
+00003fc0: 7365 6c65 6374 6162 6c65 3d22 6f6e 2220  selectable="on" 
+00003fd0: 6469 7370 6c61 793d 2269 6e6c 696e 6522  display="inline"
+00003fe0: 3e3c 6d61 7468 2078 6d6c 6e73 3d22 6874  ><math xmlns="ht
+00003ff0: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
+00004000: 3139 3938 2f4d 6174 682f 4d61 7468 4d4c  1998/Math/MathML
+00004010: 223e 3c6d 7375 623e 3c6d 693e 543c 2f6d  "><msub><mi>T</m
+00004020: 693e 3c6d 693e 413c 2f6d 693e 3c2f 6d73  i><mi>A</mi></ms
+00004030: 7562 3e3c 2f6d 6174 683e 3c2f 6d6a 782d  ub></math></mjx-
+00004040: 6173 7369 7374 6976 652d 6d6d 6c3e 3c2f  assistive-mml></
+00004050: 6d6a 782d 636f 6e74 6169 6e65 723e 3c2f  mjx-container></
+00004060: 7370 616e 3e2c 2069 6e20 4746 4633 2066  span>, in GFF3 f
+00004070: 6f72 6d61 742e 3c2f 703e 3c2f 6c69 3e0a  ormat.</p></li>.
+00004080: 3c6c 693e 3c70 3e50 726f 7465 696e 2073  <li><p>Protein s
+00004090: 6571 7565 6e63 6520 6964 656e 7469 7469  equence identiti
+000040a0: 6573 2026 616d 703b 206d 7574 6174 696f  es &amp; mutatio
+000040b0: 6e20 7479 7065 733c 2f70 3e3c 2f6c 693e  n types</p></li>
+000040c0: 0a3c 6c69 3e3c 703e 4665 6174 7572 6573  .<li><p>Features
+000040d0: 2077 6974 6820 6578 7472 6120 636f 7069   with extra copi
+000040e0: 6573 3c2f 703e 3c2f 6c69 3e0a 3c6c 693e  es</p></li>.<li>
+000040f0: 3c70 3e55 6e6d 6170 7065 6420 6665 6174  <p>Unmapped feat
+00004100: 7572 6573 3c2f 703e 3c2f 6c69 3e0a 3c2f  ures</p></li>.</
+00004110: 6f6c 3e0a 3c2f 6464 3e0a 3c2f 646c 3e0a  ol>.</dd>.</dl>.
+00004120: 3c2f 6c69 3e0a 3c2f 756c 3e0a 3c64 6976  </li>.</ul>.<div
+00004130: 2063 6c61 7373 3d22 6c69 6e65 2d62 6c6f   class="line-blo
+00004140: 636b 223e 0a3c 6469 7620 636c 6173 733d  ck">.<div class=
+00004150: 226c 696e 6522 3e3c 6272 3e3c 2f64 6976  "line"><br></div
+00004160: 3e0a 3c2f 6469 763e 0a3c 2f73 6563 7469  >.</div>.</secti
+00004170: 6f6e 3e0a 3c73 6563 7469 6f6e 2069 643d  on>.<section id=
+00004180: 2263 6974 652d 7573 2220 636c 6173 733d  "cite-us" class=
+00004190: 2222 3e0a 3c68 323e 4369 7465 2075 733c  "">.<h2>Cite us<
+000041a0: 6120 636c 6173 733d 2268 6561 6465 726c  a class="headerl
+000041b0: 696e 6b22 2068 7265 663d 2223 6369 7465  ink" href="#cite
+000041c0: 2d75 7322 2074 6974 6c65 3d22 5065 726d  -us" title="Perm
+000041d0: 616c 696e 6b20 746f 2074 6869 7320 6865  alink to this he
+000041e0: 6164 696e 6722 3e23 3c2f 613e 3c2f 6832  ading">#</a></h2
+000041f0: 3e0a 3c70 3e4b 7561 2d48 616f 2043 6861  >.<p>Kua-Hao Cha
+00004200: 6f2c 204a 616b 6f62 204d 2e20 4865 696e  o, Jakob M. Hein
+00004210: 7a2c 2043 656c 696e 6520 486f 682c 2041  z, Celine Hoh, A
+00004220: 6c61 6e20 4d61 6f2c 2041 6c61 696e 6120  lan Mao, Alaina 
+00004230: 5368 756d 6174 652c 204d 6968 6165 6c61  Shumate, Mihaela
+00004240: 2050 6572 7465 612c 2061 6e64 2053 7465   Pertea, and Ste
+00004250: 7665 6e20 4c2e 2053 616c 7a62 6572 672e  ven L. Salzberg.
+00004260: 203c 693e 2243 6f6d 6269 6e69 6e67 2044   <i>"Combining D
+00004270: 4e41 2061 6e64 2070 726f 7465 696e 2061  NA and protein a
+00004280: 6c69 676e 6d65 6e74 7320 746f 2069 6d70  lignments to imp
+00004290: 726f 7665 2067 656e 6f6d 6520 616e 6e6f  rove genome anno
+000042a0: 7461 7469 6f6e 2077 6974 6820 4c69 6674  tation with Lift
+000042b0: 4f6e 2e22 3c2f 693e 203c 623e 6269 6f52  On."</i> <b>bioR
+000042c0: 7869 7620 636f 6d69 6e67 2073 6f6f 6e3c  xiv coming soon<
+000042d0: 2f62 3e2e 0a3c 6120 6872 6566 3d22 6874  /b>..<a href="ht
+000042e0: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
+000042f0: 2e31 3039 332f 6269 6f69 6e66 6f72 6d61  .1093/bioinforma
+00004300: 7469 6373 2f62 7461 6131 3031 3622 2074  tics/btaa1016" t
+00004310: 6172 6765 743d 225f 626c 616e 6b22 3e20  arget="_blank"> 
+00004320: 3c73 7667 2078 6d6c 6e73 3d22 6874 7470  <svg xmlns="http
+00004330: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
+00004340: 3030 2f73 7667 2220 6172 6961 2d68 6964  00/svg" aria-hid
+00004350: 6465 6e3d 2274 7275 6522 2078 3d22 3070  den="true" x="0p
+00004360: 7822 2079 3d22 3070 7822 2076 6965 7742  x" y="0px" viewB
+00004370: 6f78 3d22 3020 3020 3130 3020 3130 3022  ox="0 0 100 100"
+00004380: 2077 6964 7468 3d22 3135 2220 6865 6967   width="15" heig
+00004390: 6874 3d22 3135 2220 636c 6173 733d 2269  ht="15" class="i
+000043a0: 636f 6e20 6f75 7462 6f75 6e64 223e 3c70  con outbound"><p
+000043b0: 6174 6820 6669 6c6c 3d22 6375 7272 656e  ath fill="curren
+000043c0: 7443 6f6c 6f72 2220 643d 224d 3138 2e38  tColor" d="M18.8
+000043d0: 2c38 352e 3168 3536 6c30 2c30 6332 2e32  ,85.1h56l0,0c2.2
+000043e0: 2c30 2c34 2d31 2e38 2c34 2d34 762d 3332  ,0,4-1.8,4-4v-32
+000043f0: 682d 3876 3238 682d 3438 762d 3438 6832  h-8v28h-48v-48h2
+00004400: 3876 2d38 682d 3332 6c30 2c30 632d 322e  8v-8h-32l0,0c-2.
+00004410: 322c 302d 342c 312e 382d 342c 3476 3536  2,0-4,1.8-4,4v56
+00004420: 4331 342e 382c 3833 2e33 2c31 362e 362c  C14.8,83.3,16.6,
+00004430: 3835 2e31 2c31 382e 382c 3835 2e31 7a22  85.1,18.8,85.1z"
+00004440: 3e3c 2f70 6174 683e 203c 706f 6c79 676f  ></path> <polygo
+00004450: 6e20 6669 6c6c 3d22 6375 7272 656e 7443  n fill="currentC
+00004460: 6f6c 6f72 2220 706f 696e 7473 3d22 3435  olor" points="45
+00004470: 2e37 2c34 382e 3720 3531 2e33 2c35 342e  .7,48.7 51.3,54.
+00004480: 3320 3737 2e32 2c32 382e 3520 3737 2e32  3 77.2,28.5 77.2
+00004490: 2c33 372e 3220 3835 2e32 2c33 372e 3220  ,37.2 85.2,37.2 
+000044a0: 3835 2e32 2c31 342e 3920 3632 2e38 2c31  85.2,14.9 62.8,1
+000044b0: 342e 3920 3632 2e38 2c32 322e 3920 3731  4.9 62.8,22.9 71
+000044c0: 2e35 2c32 322e 3922 3e3c 2f70 6f6c 7967  .5,22.9"></polyg
+000044d0: 6f6e 3e3c 2f73 7667 3e20 3c2f 613e 203c  on></svg> </a> <
+000044e0: 2f70 3e0a 0a3c 703e 416c 6169 6e61 2053  /p>..<p>Alaina S
+000044f0: 6875 6d61 7465 2c20 616e 6420 5374 6576  humate, and Stev
+00004500: 656e 204c 2e20 5361 6c7a 6265 7267 2e20  en L. Salzberg. 
+00004510: 3c69 3e22 4c69 6674 6f66 663a 2061 6363  <i>"Liftoff: acc
+00004520: 7572 6174 6520 6d61 7070 696e 6720 6f66  urate mapping of
+00004530: 2067 656e 6520 616e 6e6f 7461 7469 6f6e   gene annotation
+00004540: 732e 223c 2f69 3e20 3c62 3e42 696f 696e  s."</i> <b>Bioin
+00004550: 666f 726d 6174 6963 733c 2f62 3e20 3337  formatics</b> 37
+00004560: 2e31 3220 2832 3032 3129 3a20 3136 3339  .12 (2021): 1639
+00004570: 2d31 3634 332e 0a0a 3c61 2068 7265 663d  -1643...<a href=
+00004580: 2268 7474 7073 3a2f 2f64 6f69 2e6f 7267  "https://doi.org
+00004590: 2f31 302e 3130 3933 2f62 696f 696e 666f  /10.1093/bioinfo
+000045a0: 726d 6174 6963 732f 6274 6161 3130 3136  rmatics/btaa1016
+000045b0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+000045c0: 223e 203c 7376 6720 786d 6c6e 733d 2268  "> <svg xmlns="h
+000045d0: 7474 703a 2f2f 7777 772e 7733 2e6f 7267  ttp://www.w3.org
+000045e0: 2f32 3030 302f 7376 6722 2061 7269 612d  /2000/svg" aria-
+000045f0: 6869 6464 656e 3d22 7472 7565 2220 783d  hidden="true" x=
+00004600: 2230 7078 2220 793d 2230 7078 2220 7669  "0px" y="0px" vi
+00004610: 6577 426f 783d 2230 2030 2031 3030 2031  ewBox="0 0 100 1
+00004620: 3030 2220 7769 6474 683d 2231 3522 2068  00" width="15" h
+00004630: 6569 6768 743d 2231 3522 2063 6c61 7373  eight="15" class
+00004640: 3d22 6963 6f6e 206f 7574 626f 756e 6422  ="icon outbound"
+00004650: 3e3c 7061 7468 2066 696c 6c3d 2263 7572  ><path fill="cur
+00004660: 7265 6e74 436f 6c6f 7222 2064 3d22 4d31  rentColor" d="M1
+00004670: 382e 382c 3835 2e31 6835 366c 302c 3063  8.8,85.1h56l0,0c
+00004680: 322e 322c 302c 342d 312e 382c 342d 3476  2.2,0,4-1.8,4-4v
+00004690: 2d33 3268 2d38 7632 3868 2d34 3876 2d34  -32h-8v28h-48v-4
+000046a0: 3868 3238 762d 3868 2d33 326c 302c 3063  8h28v-8h-32l0,0c
+000046b0: 2d32 2e32 2c30 2d34 2c31 2e38 2d34 2c34  -2.2,0-4,1.8-4,4
+000046c0: 7635 3643 3134 2e38 2c38 332e 332c 3136  v56C14.8,83.3,16
+000046d0: 2e36 2c38 352e 312c 3138 2e38 2c38 352e  .6,85.1,18.8,85.
+000046e0: 317a 223e 3c2f 7061 7468 3e20 3c70 6f6c  1z"></path> <pol
+000046f0: 7967 6f6e 2066 696c 6c3d 2263 7572 7265  ygon fill="curre
+00004700: 6e74 436f 6c6f 7222 2070 6f69 6e74 733d  ntColor" points=
+00004710: 2234 352e 372c 3438 2e37 2035 312e 332c  "45.7,48.7 51.3,
+00004720: 3534 2e33 2037 372e 322c 3238 2e35 2037  54.3 77.2,28.5 7
+00004730: 372e 322c 3337 2e32 2038 352e 322c 3337  7.2,37.2 85.2,37
+00004740: 2e32 2038 352e 322c 3134 2e39 2036 322e  .2 85.2,14.9 62.
+00004750: 382c 3134 2e39 2036 322e 382c 3232 2e39  8,14.9 62.8,22.9
+00004760: 2037 312e 352c 3232 2e39 223e 3c2f 706f   71.5,22.9"></po
+00004770: 6c79 676f 6e3e 3c2f 7376 673e 0a3c 2f61  lygon></svg>.</a
+00004780: 3e0a 3c2f 703e 3c64 6976 2063 6c61 7373  >.</p><div class
+00004790: 3d22 6c69 6e65 2d62 6c6f 636b 223e 0a3c  ="line-block">.<
+000047a0: 6469 7620 636c 6173 733d 226c 696e 6522  div class="line"
+000047b0: 3e3c 6272 3e3c 2f64 6976 3e0a 3c2f 6469  ><br></div>.</di
+000047c0: 763e 0a3c 2f73 6563 7469 6f6e 3e0a 3c73  v>.</section>.<s
+000047d0: 6563 7469 6f6e 2069 643d 2275 7365 722d  ection id="user-
+000047e0: 7375 7070 6f72 7422 2063 6c61 7373 3d22  support" class="
+000047f0: 223e 0a3c 6832 3e55 7365 7220 7375 7070  ">.<h2>User supp
+00004800: 6f72 743c 6120 636c 6173 733d 2268 6561  ort<a class="hea
+00004810: 6465 726c 696e 6b22 2068 7265 663d 2223  derlink" href="#
+00004820: 7573 6572 2d73 7570 706f 7274 2220 7469  user-support" ti
+00004830: 746c 653d 2250 6572 6d61 6c69 6e6b 2074  tle="Permalink t
+00004840: 6f20 7468 6973 2068 6561 6469 6e67 223e  o this heading">
+00004850: 233c 2f61 3e3c 2f68 323e 0a3c 703e 506c  #</a></h2>.<p>Pl
+00004860: 6561 7365 2067 6f20 7468 726f 7567 6820  ease go through 
+00004870: 7468 6520 3c61 2063 6c61 7373 3d22 7265  the <a class="re
+00004880: 6665 7265 6e63 6520 696e 7465 726e 616c  ference internal
+00004890: 2220 6872 6566 3d22 2374 6162 6c65 2d6f  " href="#table-o
+000048a0: 662d 636f 6e74 656e 7473 223e 3c73 7061  f-contents"><spa
+000048b0: 6e20 636c 6173 733d 2273 7464 2073 7464  n class="std std
+000048c0: 2d72 6566 223e 646f 6375 6d65 6e74 6174  -ref">documentat
+000048d0: 696f 6e3c 2f73 7061 6e3e 3c2f 613e 2062  ion</span></a> b
+000048e0: 656c 6f77 2066 6972 7374 2e20 4966 2079  elow first. If y
+000048f0: 6f75 2068 6176 6520 7175 6573 7469 6f6e  ou have question
+00004900: 7320 6162 6f75 7420 7573 696e 6720 7468  s about using th
+00004910: 6520 7061 636b 6167 652c 2061 2062 7567  e package, a bug
+00004920: 2072 6570 6f72 742c 206f 7220 6120 6665   report, or a fe
+00004930: 6174 7572 6520 7265 7175 6573 742c 2070  ature request, p
+00004940: 6c65 6173 6520 7573 6520 7468 6520 4769  lease use the Gi
+00004950: 7448 7562 2069 7373 7565 2074 7261 636b  tHub issue track
+00004960: 6572 2068 6572 653a 3c2f 703e 0a3c 703e  er here:</p>.<p>
+00004970: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
+00004980: 6e63 6520 6578 7465 726e 616c 2220 6872  nce external" hr
+00004990: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000049a0: 7562 2e63 6f6d 2f4b 7561 6e68 616f 2d43  ub.com/Kuanhao-C
+000049b0: 6861 6f2f 4c69 6674 4f6e 2f69 7373 7565  hao/LiftOn/issue
+000049c0: 7322 3e68 7474 7073 3a2f 2f67 6974 6875  s">https://githu
+000049d0: 622e 636f 6d2f 4b75 616e 6861 6f2d 4368  b.com/Kuanhao-Ch
+000049e0: 616f 2f4c 6966 744f 6e2f 6973 7375 6573  ao/LiftOn/issues
+000049f0: 3c2f 613e 3c2f 703e 0a3c 6469 7620 636c  </a></p>.<div cl
+00004a00: 6173 733d 226c 696e 652d 626c 6f63 6b22  ass="line-block"
+00004a10: 3e0a 3c64 6976 2063 6c61 7373 3d22 6c69  >.<div class="li
+00004a20: 6e65 223e 3c62 723e 3c2f 6469 763e 0a3c  ne"><br></div>.<
+00004a30: 2f64 6976 3e0a 3c2f 7365 6374 696f 6e3e  /div>.</section>
+00004a40: 0a3c 7365 6374 696f 6e20 6964 3d22 6b65  .<section id="ke
+00004a50: 792d 636f 6e74 7269 6275 746f 7273 2220  y-contributors" 
+00004a60: 636c 6173 733d 2222 3e0a 3c68 323e 4b65  class="">.<h2>Ke
+00004a70: 7920 636f 6e74 7269 6275 746f 7273 3c61  y contributors<a
+00004a80: 2063 6c61 7373 3d22 6865 6164 6572 6c69   class="headerli
+00004a90: 6e6b 2220 6872 6566 3d22 236b 6579 2d63  nk" href="#key-c
+00004aa0: 6f6e 7472 6962 7574 6f72 7322 2074 6974  ontributors" tit
+00004ab0: 6c65 3d22 5065 726d 616c 696e 6b20 746f  le="Permalink to
+00004ac0: 2074 6869 7320 6865 6164 696e 6722 3e23   this heading">#
+00004ad0: 3c2f 613e 3c2f 6832 3e0a 3c70 3e4c 6966  </a></h2>.<p>Lif
+00004ae0: 744f 6e20 7761 7320 6465 7369 676e 6564  tOn was designed
+00004af0: 2061 6e64 2064 6576 656c 6f70 6564 2062   and developed b
+00004b00: 7920 3c61 2063 6c61 7373 3d22 7265 6665  y <a class="refe
+00004b10: 7265 6e63 6520 6578 7465 726e 616c 2220  rence external" 
+00004b20: 6872 6566 3d22 6874 7470 733a 2f2f 6b68  href="https://kh
+00004b30: 6368 616f 2e63 6f6d 2f22 3e4b 7561 6e2d  chao.com/">Kuan-
+00004b40: 4861 6f20 4368 616f 3c2f 613e 2e20 2054  Hao Chao</a>.  T
+00004b50: 6869 7320 646f 6375 6d65 6e74 6174 696f  his documentatio
+00004b60: 6e20 7761 7320 7772 6974 7465 6e20 6279  n was written by
+00004b70: 203c 6120 636c 6173 733d 2272 6566 6572   <a class="refer
+00004b80: 656e 6365 2065 7874 6572 6e61 6c22 2068  ence external" h
+00004b90: 7265 663d 2268 7474 7073 3a2f 2f6b 6863  ref="https://khc
+00004ba0: 6861 6f2e 636f 6d2f 223e 4b75 616e 2d48  hao.com/">Kuan-H
+00004bb0: 616f 2043 6861 6f3c 2f61 3e20 616e 6420  ao Chao</a> and 
+00004bc0: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
+00004bd0: 6e63 6520 6578 7465 726e 616c 2220 6872  nce external" hr
+00004be0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00004bf0: 7562 2e63 6f6d 2f61 6d31 3222 3e41 6c61  ub.com/am12">Ala
+00004c00: 6e20 4d61 6e3c 2f61 3e2e 2054 6865 204c  n Man</a>. The L
+00004c10: 6966 744f 6e20 6c6f 676f 2077 6173 2064  iftOn logo was d
+00004c20: 6573 6967 6e65 6420 6279 203c 6120 636c  esigned by <a cl
+00004c30: 6173 733d 2272 6566 6572 656e 6365 2065  ass="reference e
+00004c40: 7874 6572 6e61 6c22 2068 7265 663d 2268  xternal" href="h
+00004c50: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00004c60: 6d2f 616d 3132 223e 416c 616e 204d 616e  m/am12">Alan Man
+00004c70: 3c2f 613e 2e3c 2f70 3e0a 3c64 6976 2063  </a>.</p>.<div c
+00004c80: 6c61 7373 3d22 6c69 6e65 2d62 6c6f 636b  lass="line-block
+00004c90: 223e 0a3c 6469 7620 636c 6173 733d 226c  ">.<div class="l
+00004ca0: 696e 6522 3e3c 6272 3e3c 2f64 6976 3e0a  ine"><br></div>.
+00004cb0: 3c2f 6469 763e 0a3c 2f73 6563 7469 6f6e  </div>.</section
+00004cc0: 3e0a 3c73 6563 7469 6f6e 2069 643d 2274  >.<section id="t
+00004cd0: 6162 6c65 2d6f 662d 636f 6e74 656e 7473  able-of-contents
+00004ce0: 2220 636c 6173 733d 2222 3e0a 3c73 7061  " class="">.<spa
+00004cf0: 6e20 6964 3d22 6964 3322 3e3c 2f73 7061  n id="id3"></spa
+00004d00: 6e3e 3c68 323e 5461 626c 6520 6f66 2063  n><h2>Table of c
+00004d10: 6f6e 7465 6e74 733c 6120 636c 6173 733d  ontents<a class=
+00004d20: 2268 6561 6465 726c 696e 6b22 2068 7265  "headerlink" hre
+00004d30: 663d 2223 7461 626c 652d 6f66 2d63 6f6e  f="#table-of-con
+00004d40: 7465 6e74 7322 2074 6974 6c65 3d22 5065  tents" title="Pe
+00004d50: 726d 616c 696e 6b20 746f 2074 6869 7320  rmalink to this 
+00004d60: 6865 6164 696e 6722 3e23 3c2f 613e 3c2f  heading">#</a></
+00004d70: 6832 3e0a 3c64 6976 2063 6c61 7373 3d22  h2>.<div class="
+00004d80: 746f 6374 7265 652d 7772 6170 7065 7220  toctree-wrapper 
+00004d90: 636f 6d70 6f75 6e64 223e 0a3c 756c 3e0a  compound">.<ul>.
+00004da0: 3c6c 6920 636c 6173 733d 2274 6f63 7472  <li class="toctr
+00004db0: 6565 2d6c 3122 3e3c 6120 636c 6173 733d  ee-l1"><a class=
+00004dc0: 2272 6566 6572 656e 6365 2069 6e74 6572  "reference inter
+00004dd0: 6e61 6c22 2068 7265 663d 2268 7474 7073  nal" href="https
+00004de0: 3a2f 2f63 6362 2e6a 6875 2e65 6475 2f6c  ://ccb.jhu.edu/l
+00004df0: 6966 746f 6e2f 636f 6e74 656e 742f 696e  ifton/content/in
+00004e00: 7374 616c 6c61 7469 6f6e 2e68 746d 6c22  stallation.html"
+00004e10: 3e49 6e73 7461 6c6c 6174 696f 6e3c 2f61  >Installation</a
+00004e20: 3e3c 756c 3e0a 3c6c 6920 636c 6173 733d  ><ul>.<li class=
+00004e30: 2274 6f63 7472 6565 2d6c 3222 3e3c 6120  "toctree-l2"><a 
+00004e40: 636c 6173 733d 2272 6566 6572 656e 6365  class="reference
+00004e50: 2069 6e74 6572 6e61 6c22 2068 7265 663d   internal" href=
+00004e60: 2268 7474 7073 3a2f 2f63 6362 2e6a 6875  "https://ccb.jhu
+00004e70: 2e65 6475 2f6c 6966 746f 6e2f 636f 6e74  .edu/lifton/cont
+00004e80: 656e 742f 696e 7374 616c 6c61 7469 6f6e  ent/installation
+00004e90: 2e68 746d 6c23 7379 7374 656d 2d72 6571  .html#system-req
+00004ea0: 7569 7265 6d65 6e74 7322 3e53 7973 7465  uirements">Syste
+00004eb0: 6d20 7265 7175 6972 656d 656e 7473 3c2f  m requirements</
+00004ec0: 613e 3c2f 6c69 3e0a 3c6c 6920 636c 6173  a></li>.<li clas
+00004ed0: 733d 2274 6f63 7472 6565 2d6c 3222 3e3c  s="toctree-l2"><
+00004ee0: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
+00004ef0: 6365 2069 6e74 6572 6e61 6c22 2068 7265  ce internal" hre
+00004f00: 663d 2268 7474 7073 3a2f 2f63 6362 2e6a  f="https://ccb.j
+00004f10: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
+00004f20: 6e74 656e 742f 696e 7374 616c 6c61 7469  ntent/installati
+00004f30: 6f6e 2e68 746d 6c23 696e 7374 616c 6c2d  on.html#install-
+00004f40: 7468 726f 7567 682d 7069 7022 3e49 6e73  through-pip">Ins
+00004f50: 7461 6c6c 2074 6872 6f75 6768 2070 6970  tall through pip
+00004f60: 3c2f 613e 3c2f 6c69 3e0a 3c6c 6920 636c  </a></li>.<li cl
+00004f70: 6173 733d 2274 6f63 7472 6565 2d6c 3222  ass="toctree-l2"
+00004f80: 3e3c 6120 636c 6173 733d 2272 6566 6572  ><a class="refer
+00004f90: 656e 6365 2069 6e74 6572 6e61 6c22 2068  ence internal" h
+00004fa0: 7265 663d 2268 7474 7073 3a2f 2f63 6362  ref="https://ccb
+00004fb0: 2e6a 6875 2e65 6475 2f6c 6966 746f 6e2f  .jhu.edu/lifton/
+00004fc0: 636f 6e74 656e 742f 696e 7374 616c 6c61  content/installa
+00004fd0: 7469 6f6e 2e68 746d 6c23 696e 7374 616c  tion.html#instal
+00004fe0: 6c2d 7468 726f 7567 682d 636f 6e64 6122  l-through-conda"
+00004ff0: 3e49 6e73 7461 6c6c 2074 6872 6f75 6768  >Install through
+00005000: 2063 6f6e 6461 3c2f 613e 3c2f 6c69 3e0a   conda</a></li>.
+00005010: 3c6c 6920 636c 6173 733d 2274 6f63 7472  <li class="toctr
+00005020: 6565 2d6c 3222 3e3c 6120 636c 6173 733d  ee-l2"><a class=
+00005030: 2272 6566 6572 656e 6365 2069 6e74 6572  "reference inter
+00005040: 6e61 6c22 2068 7265 663d 2268 7474 7073  nal" href="https
+00005050: 3a2f 2f63 6362 2e6a 6875 2e65 6475 2f6c  ://ccb.jhu.edu/l
+00005060: 6966 746f 6e2f 636f 6e74 656e 742f 696e  ifton/content/in
+00005070: 7374 616c 6c61 7469 6f6e 2e68 746d 6c23  stallation.html#
+00005080: 696e 7374 616c 6c2d 6672 6f6d 2d73 6f75  install-from-sou
+00005090: 7263 6522 3e49 6e73 7461 6c6c 2066 726f  rce">Install fro
+000050a0: 6d20 736f 7572 6365 3c2f 613e 3c2f 6c69  m source</a></li
+000050b0: 3e0a 3c6c 6920 636c 6173 733d 2274 6f63  >.<li class="toc
+000050c0: 7472 6565 2d6c 3222 3e3c 6120 636c 6173  tree-l2"><a clas
+000050d0: 733d 2272 6566 6572 656e 6365 2069 6e74  s="reference int
+000050e0: 6572 6e61 6c22 2068 7265 663d 2268 7474  ernal" href="htt
+000050f0: 7073 3a2f 2f63 6362 2e6a 6875 2e65 6475  ps://ccb.jhu.edu
+00005100: 2f6c 6966 746f 6e2f 636f 6e74 656e 742f  /lifton/content/
+00005110: 696e 7374 616c 6c61 7469 6f6e 2e68 746d  installation.htm
+00005120: 6c23 6368 6563 6b2d 6c69 6674 6f6e 2d69  l#check-lifton-i
+00005130: 6e73 7461 6c6c 6174 696f 6e22 3e43 6865  nstallation">Che
+00005140: 636b 204c 6966 744f 6e20 696e 7374 616c  ck LiftOn instal
+00005150: 6c61 7469 6f6e 3c2f 613e 3c2f 6c69 3e0a  lation</a></li>.
+00005160: 3c6c 6920 636c 6173 733d 2274 6f63 7472  <li class="toctr
+00005170: 6565 2d6c 3222 3e3c 6120 636c 6173 733d  ee-l2"><a class=
+00005180: 2272 6566 6572 656e 6365 2069 6e74 6572  "reference inter
+00005190: 6e61 6c22 2068 7265 663d 2268 7474 7073  nal" href="https
+000051a0: 3a2f 2f63 6362 2e6a 6875 2e65 6475 2f6c  ://ccb.jhu.edu/l
+000051b0: 6966 746f 6e2f 636f 6e74 656e 742f 696e  ifton/content/in
+000051c0: 7374 616c 6c61 7469 6f6e 2e68 746d 6c23  stallation.html#
+000051d0: 6e6f 772d 796f 752d 6172 652d 7265 6164  now-you-are-read
+000051e0: 792d 746f 2d67 6f22 3e4e 6f77 2c20 796f  y-to-go">Now, yo
+000051f0: 7520 6172 6520 7265 6164 7920 746f 2067  u are ready to g
+00005200: 6f20 213c 2f61 3e3c 2f6c 693e 0a3c 2f75  o !</a></li>.</u
+00005210: 6c3e 0a3c 2f6c 693e 0a3c 6c69 2063 6c61  l>.</li>.<li cla
+00005220: 7373 3d22 746f 6374 7265 652d 6c31 223e  ss="toctree-l1">
+00005230: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
+00005240: 6e63 6520 696e 7465 726e 616c 2220 6872  nce internal" hr
+00005250: 6566 3d22 6874 7470 733a 2f2f 6363 622e  ef="https://ccb.
+00005260: 6a68 752e 6564 752f 6c69 6674 6f6e 2f63  jhu.edu/lifton/c
+00005270: 6f6e 7465 6e74 2f71 7569 636b 7374 6172  ontent/quickstar
+00005280: 742e 6874 6d6c 223e 5175 6963 6b20 5374  t.html">Quick St
+00005290: 6172 7420 4775 6964 653c 2f61 3e3c 756c  art Guide</a><ul
+000052a0: 3e0a 3c6c 6920 636c 6173 733d 2274 6f63  >.<li class="toc
+000052b0: 7472 6565 2d6c 3222 3e3c 6120 636c 6173  tree-l2"><a clas
+000052c0: 733d 2272 6566 6572 656e 6365 2069 6e74  s="reference int
+000052d0: 6572 6e61 6c22 2068 7265 663d 2268 7474  ernal" href="htt
+000052e0: 7073 3a2f 2f63 6362 2e6a 6875 2e65 6475  ps://ccb.jhu.edu
+000052f0: 2f6c 6966 746f 6e2f 636f 6e74 656e 742f  /lifton/content/
+00005300: 7175 6963 6b73 7461 7274 2e68 746d 6c23  quickstart.html#
+00005310: 7375 7065 722d 7175 6963 6b2d 7374 6172  super-quick-star
+00005320: 742d 6f6e 652d 6c69 6e65 7222 3e53 7570  t-one-liner">Sup
+00005330: 6572 2d51 7569 636b 2053 7461 7274 2028  er-Quick Start (
+00005340: 6f6e 652d 6c69 6e65 7229 3c2f 613e 3c2f  one-liner)</a></
+00005350: 6c69 3e0a 3c6c 6920 636c 6173 733d 2274  li>.<li class="t
+00005360: 6f63 7472 6565 2d6c 3222 3e3c 6120 636c  octree-l2"><a cl
+00005370: 6173 733d 2272 6566 6572 656e 6365 2069  ass="reference i
+00005380: 6e74 6572 6e61 6c22 2068 7265 663d 2268  nternal" href="h
+00005390: 7474 7073 3a2f 2f63 6362 2e6a 6875 2e65  ttps://ccb.jhu.e
+000053a0: 6475 2f6c 6966 746f 6e2f 636f 6e74 656e  du/lifton/conten
+000053b0: 742f 7175 6963 6b73 7461 7274 2e68 746d  t/quickstart.htm
+000053c0: 6c23 696e 7465 7270 7265 7469 6e67 2d6f  l#interpreting-o
+000053d0: 7574 7075 7473 2d6f 6e2d 7468 652d 7465  utputs-on-the-te
+000053e0: 726d 696e 616c 223e 496e 7465 7270 7265  rminal">Interpre
+000053f0: 7469 6e67 206f 7574 7075 7473 206f 6e20  ting outputs on 
+00005400: 7468 6520 7465 726d 696e 616c 3c2f 613e  the terminal</a>
+00005410: 3c2f 6c69 3e0a 3c6c 6920 636c 6173 733d  </li>.<li class=
+00005420: 2274 6f63 7472 6565 2d6c 3222 3e3c 6120  "toctree-l2"><a 
+00005430: 636c 6173 733d 2272 6566 6572 656e 6365  class="reference
+00005440: 2069 6e74 6572 6e61 6c22 2068 7265 663d   internal" href=
+00005450: 2268 7474 7073 3a2f 2f63 6362 2e6a 6875  "https://ccb.jhu
+00005460: 2e65 6475 2f6c 6966 746f 6e2f 636f 6e74  .edu/lifton/cont
+00005470: 656e 742f 7175 6963 6b73 7461 7274 2e68  ent/quickstart.h
+00005480: 746d 6c23 7472 792d 6c69 6674 6f6e 2d6f  tml#try-lifton-o
+00005490: 6e2d 676f 6f67 6c65 2d63 6f6c 6162 223e  n-google-colab">
+000054a0: 5472 7920 4c69 6674 4f6e 206f 6e20 476f  Try LiftOn on Go
+000054b0: 6f67 6c65 2043 6f6c 6162 3c2f 613e 3c2f  ogle Colab</a></
+000054c0: 6c69 3e0a 3c2f 756c 3e0a 3c2f 6c69 3e0a  li>.</ul>.</li>.
+000054d0: 3c2f 756c 3e0a 3c2f 6469 763e 0a3c 6469  </ul>.</div>.<di
+000054e0: 7620 636c 6173 733d 2274 6f63 7472 6565  v class="toctree
+000054f0: 2d77 7261 7070 6572 2063 6f6d 706f 756e  -wrapper compoun
+00005500: 6422 3e0a 3c70 2063 6c61 7373 3d22 6361  d">.<p class="ca
+00005510: 7074 696f 6e22 2072 6f6c 653d 2268 6561  ption" role="hea
+00005520: 6469 6e67 223e 3c73 7061 6e20 636c 6173  ding"><span clas
+00005530: 733d 2263 6170 7469 6f6e 2d74 6578 7422  s="caption-text"
+00005540: 3e45 7861 6d70 6c65 733c 2f73 7061 6e3e  >Examples</span>
+00005550: 3c2f 703e 0a3c 756c 3e0a 3c6c 6920 636c  </p>.<ul>.<li cl
+00005560: 6173 733d 2274 6f63 7472 6565 2d6c 3122  ass="toctree-l1"
+00005570: 3e3c 6120 636c 6173 733d 2272 6566 6572  ><a class="refer
+00005580: 656e 6365 2069 6e74 6572 6e61 6c22 2068  ence internal" h
+00005590: 7265 663d 2268 7474 7073 3a2f 2f63 6362  ref="https://ccb
+000055a0: 2e6a 6875 2e65 6475 2f6c 6966 746f 6e2f  .jhu.edu/lifton/
+000055b0: 636f 6e74 656e 742f 7361 6d65 5f73 7065  content/same_spe
+000055c0: 6369 6573 5f6c 6966 746f 7665 722f 696e  cies_liftover/in
+000055d0: 6465 782e 6874 6d6c 223e 5361 6d65 2073  dex.html">Same s
+000055e0: 7065 6369 6573 206c 6966 742d 6f76 6572  pecies lift-over
+000055f0: 3c2f 613e 3c2f 6c69 3e0a 3c6c 6920 636c  </a></li>.<li cl
+00005600: 6173 733d 2274 6f63 7472 6565 2d6c 3122  ass="toctree-l1"
+00005610: 3e3c 6120 636c 6173 733d 2272 6566 6572  ><a class="refer
+00005620: 656e 6365 2069 6e74 6572 6e61 6c22 2068  ence internal" h
+00005630: 7265 663d 2268 7474 7073 3a2f 2f63 6362  ref="https://ccb
+00005640: 2e6a 6875 2e65 6475 2f6c 6966 746f 6e2f  .jhu.edu/lifton/
+00005650: 636f 6e74 656e 742f 636c 6f73 655f 7370  content/close_sp
+00005660: 6563 6965 735f 6c69 6674 6f76 6572 2f69  ecies_liftover/i
+00005670: 6e64 6578 2e68 746d 6c22 3e43 6c6f 7365  ndex.html">Close
+00005680: 6c79 2072 656c 6174 6564 2073 7065 6369  ly related speci
+00005690: 6573 206c 6966 742d 6f76 6572 3c2f 613e  es lift-over</a>
+000056a0: 3c2f 6c69 3e0a 3c6c 6920 636c 6173 733d  </li>.<li class=
+000056b0: 2274 6f63 7472 6565 2d6c 3122 3e3c 6120  "toctree-l1"><a 
+000056c0: 636c 6173 733d 2272 6566 6572 656e 6365  class="reference
+000056d0: 2069 6e74 6572 6e61 6c22 2068 7265 663d   internal" href=
+000056e0: 2268 7474 7073 3a2f 2f63 6362 2e6a 6875  "https://ccb.jhu
+000056f0: 2e65 6475 2f6c 6966 746f 6e2f 636f 6e74  .edu/lifton/cont
+00005700: 656e 742f 6469 7374 616e 745f 7370 6563  ent/distant_spec
+00005710: 6965 735f 6c69 6674 6f76 6572 2f69 6e64  ies_liftover/ind
+00005720: 6578 2e68 746d 6c22 3e44 6973 7461 6e74  ex.html">Distant
+00005730: 6c79 2072 656c 6174 6564 2073 7065 6369  ly related speci
+00005740: 6573 206c 6966 742d 6f76 6572 3c2f 613e  es lift-over</a>
+00005750: 3c2f 6c69 3e0a 3c2f 756c 3e0a 3c2f 6469  </li>.</ul>.</di
+00005760: 763e 0a3c 6469 7620 636c 6173 733d 2274  v>.<div class="t
+00005770: 6f63 7472 6565 2d77 7261 7070 6572 2063  octree-wrapper c
+00005780: 6f6d 706f 756e 6422 3e0a 3c70 2063 6c61  ompound">.<p cla
+00005790: 7373 3d22 6361 7074 696f 6e22 2072 6f6c  ss="caption" rol
+000057a0: 653d 2268 6561 6469 6e67 223e 3c73 7061  e="heading"><spa
+000057b0: 6e20 636c 6173 733d 2263 6170 7469 6f6e  n class="caption
+000057c0: 2d74 6578 7422 3e49 6e66 6f3c 2f73 7061  -text">Info</spa
+000057d0: 6e3e 3c2f 703e 0a3c 756c 3e0a 3c6c 6920  n></p>.<ul>.<li 
+000057e0: 636c 6173 733d 2274 6f63 7472 6565 2d6c  class="toctree-l
+000057f0: 3122 3e3c 6120 636c 6173 733d 2272 6566  1"><a class="ref
+00005800: 6572 656e 6365 2069 6e74 6572 6e61 6c22  erence internal"
+00005810: 2068 7265 663d 2268 7474 7073 3a2f 2f63   href="https://c
+00005820: 6362 2e6a 6875 2e65 6475 2f6c 6966 746f  cb.jhu.edu/lifto
+00005830: 6e2f 636f 6e74 656e 742f 6f75 7470 7574  n/content/output
+00005840: 5f65 7870 6c61 6e61 7469 6f6e 2e68 746d  _explanation.htm
+00005850: 6c22 3e4f 7574 7075 7420 6669 6c65 733c  l">Output files<
+00005860: 2f61 3e3c 756c 3e0a 3c6c 6920 636c 6173  /a><ul>.<li clas
+00005870: 733d 2274 6f63 7472 6565 2d6c 3222 3e3c  s="toctree-l2"><
+00005880: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
+00005890: 6365 2069 6e74 6572 6e61 6c22 2068 7265  ce internal" hre
+000058a0: 663d 2268 7474 7073 3a2f 2f63 6362 2e6a  f="https://ccb.j
+000058b0: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
+000058c0: 6e74 656e 742f 6f75 7470 7574 5f65 7870  ntent/output_exp
+000058d0: 6c61 6e61 7469 6f6e 2e68 746d 6c23 6c69  lanation.html#li
+000058e0: 6674 6f6e 2d67 6666 3322 3e6c 6966 746f  fton-gff3">lifto
+000058f0: 6e2e 6766 6633 3c2f 613e 3c2f 6c69 3e0a  n.gff3</a></li>.
+00005900: 3c6c 6920 636c 6173 733d 2274 6f63 7472  <li class="toctr
+00005910: 6565 2d6c 3222 3e3c 6120 636c 6173 733d  ee-l2"><a class=
+00005920: 2272 6566 6572 656e 6365 2069 6e74 6572  "reference inter
+00005930: 6e61 6c22 2068 7265 663d 2268 7474 7073  nal" href="https
+00005940: 3a2f 2f63 6362 2e6a 6875 2e65 6475 2f6c  ://ccb.jhu.edu/l
+00005950: 6966 746f 6e2f 636f 6e74 656e 742f 6f75  ifton/content/ou
+00005960: 7470 7574 5f65 7870 6c61 6e61 7469 6f6e  tput_explanation
+00005970: 2e68 746d 6c23 6c69 6674 6f6e 2d6f 7574  .html#lifton-out
+00005980: 7075 7422 3e6c 6966 746f 6e5f 6f75 7470  put">lifton_outp
+00005990: 7574 2f3c 2f61 3e3c 2f6c 693e 0a3c 2f75  ut/</a></li>.</u
+000059a0: 6c3e 0a3c 2f6c 693e 0a3c 6c69 2063 6c61  l>.</li>.<li cla
+000059b0: 7373 3d22 746f 6374 7265 652d 6c31 223e  ss="toctree-l1">
+000059c0: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
+000059d0: 6e63 6520 696e 7465 726e 616c 2220 6872  nce internal" hr
+000059e0: 6566 3d22 6874 7470 733a 2f2f 6363 622e  ef="https://ccb.
+000059f0: 6a68 752e 6564 752f 6c69 6674 6f6e 2f63  jhu.edu/lifton/c
+00005a00: 6f6e 7465 6e74 2f66 6561 7475 7265 5f63  ontent/feature_c
+00005a10: 6f75 6e74 696e 672e 6874 6d6c 223e 4765  ounting.html">Ge
+00005a20: 6e65 202f 2054 7261 6e73 6372 6970 7420  ne / Transcript 
+00005a30: 636f 756e 7469 6e67 3c2f 613e 3c75 6c3e  counting</a><ul>
+00005a40: 0a3c 6c69 2063 6c61 7373 3d22 746f 6374  .<li class="toct
+00005a50: 7265 652d 6c32 223e 3c61 2063 6c61 7373  ree-l2"><a class
+00005a60: 3d22 7265 6665 7265 6e63 6520 696e 7465  ="reference inte
+00005a70: 726e 616c 2220 6872 6566 3d22 6874 7470  rnal" href="http
+00005a80: 733a 2f2f 6363 622e 6a68 752e 6564 752f  s://ccb.jhu.edu/
+00005a90: 6c69 6674 6f6e 2f63 6f6e 7465 6e74 2f66  lifton/content/f
+00005aa0: 6561 7475 7265 5f63 6f75 6e74 696e 672e  eature_counting.
+00005ab0: 6874 6d6c 2367 656e 652d 636f 756e 7469  html#gene-counti
+00005ac0: 6e67 223e 4765 6e65 2063 6f75 6e74 696e  ng">Gene countin
+00005ad0: 673c 2f61 3e3c 2f6c 693e 0a3c 6c69 2063  g</a></li>.<li c
+00005ae0: 6c61 7373 3d22 746f 6374 7265 652d 6c32  lass="toctree-l2
+00005af0: 223e 3c61 2063 6c61 7373 3d22 7265 6665  "><a class="refe
+00005b00: 7265 6e63 6520 696e 7465 726e 616c 2220  rence internal" 
+00005b10: 6872 6566 3d22 6874 7470 733a 2f2f 6363  href="https://cc
+00005b20: 622e 6a68 752e 6564 752f 6c69 6674 6f6e  b.jhu.edu/lifton
+00005b30: 2f63 6f6e 7465 6e74 2f66 6561 7475 7265  /content/feature
+00005b40: 5f63 6f75 6e74 696e 672e 6874 6d6c 2374  _counting.html#t
+00005b50: 7261 6e73 6372 6970 742d 636f 756e 7469  ranscript-counti
+00005b60: 6e67 223e 5472 616e 7363 7269 7074 2063  ng">Transcript c
+00005b70: 6f75 6e74 696e 673c 2f61 3e3c 2f6c 693e  ounting</a></li>
+00005b80: 0a3c 2f75 6c3e 0a3c 2f6c 693e 0a3c 6c69  .</ul>.</li>.<li
+00005b90: 2063 6c61 7373 3d22 746f 6374 7265 652d   class="toctree-
+00005ba0: 6c31 223e 3c61 2063 6c61 7373 3d22 7265  l1"><a class="re
+00005bb0: 6665 7265 6e63 6520 696e 7465 726e 616c  ference internal
+00005bc0: 2220 6872 6566 3d22 6874 7470 733a 2f2f  " href="https://
+00005bd0: 6363 622e 6a68 752e 6564 752f 6c69 6674  ccb.jhu.edu/lift
+00005be0: 6f6e 2f63 6f6e 7465 6e74 2f65 7661 6c75  on/content/evalu
+00005bf0: 6174 696f 6e5f 6d65 7472 6963 732e 6874  ation_metrics.ht
+00005c00: 6d6c 223e 4576 616c 7561 7469 6f6e 206d  ml">Evaluation m
+00005c10: 6574 7269 6373 202d 2073 6571 7565 6e63  etrics - sequenc
+00005c20: 6520 6964 656e 7469 7479 3c2f 613e 3c75  e identity</a><u
+00005c30: 6c3e 0a3c 6c69 2063 6c61 7373 3d22 746f  l>.<li class="to
+00005c40: 6374 7265 652d 6c32 223e 3c61 2063 6c61  ctree-l2"><a cla
+00005c50: 7373 3d22 7265 6665 7265 6e63 6520 696e  ss="reference in
+00005c60: 7465 726e 616c 2220 6872 6566 3d22 6874  ternal" href="ht
+00005c70: 7470 733a 2f2f 6363 622e 6a68 752e 6564  tps://ccb.jhu.ed
+00005c80: 752f 6c69 6674 6f6e 2f63 6f6e 7465 6e74  u/lifton/content
+00005c90: 2f65 7661 6c75 6174 696f 6e5f 6d65 7472  /evaluation_metr
+00005ca0: 6963 732e 6874 6d6c 2364 6e61 2d73 6571  ics.html#dna-seq
+00005cb0: 7565 6e63 652d 6964 656e 7469 7479 2d73  uence-identity-s
+00005cc0: 636f 7265 223e 444e 4120 7365 7175 656e  core">DNA sequen
+00005cd0: 6365 2069 6465 6e74 6974 7920 7363 6f72  ce identity scor
+00005ce0: 653c 2f61 3e3c 2f6c 693e 0a3c 6c69 2063  e</a></li>.<li c
+00005cf0: 6c61 7373 3d22 746f 6374 7265 652d 6c32  lass="toctree-l2
+00005d00: 223e 3c61 2063 6c61 7373 3d22 7265 6665  "><a class="refe
+00005d10: 7265 6e63 6520 696e 7465 726e 616c 2220  rence internal" 
+00005d20: 6872 6566 3d22 6874 7470 733a 2f2f 6363  href="https://cc
+00005d30: 622e 6a68 752e 6564 752f 6c69 6674 6f6e  b.jhu.edu/lifton
+00005d40: 2f63 6f6e 7465 6e74 2f65 7661 6c75 6174  /content/evaluat
+00005d50: 696f 6e5f 6d65 7472 6963 732e 6874 6d6c  ion_metrics.html
+00005d60: 2370 726f 7465 696e 2d73 6571 7565 6e63  #protein-sequenc
+00005d70: 652d 6964 656e 7469 7479 2d73 636f 7265  e-identity-score
+00005d80: 223e 5072 6f74 6569 6e20 7365 7175 656e  ">Protein sequen
+00005d90: 6365 2069 6465 6e74 6974 7920 7363 6f72  ce identity scor
+00005da0: 653c 2f61 3e3c 2f6c 693e 0a3c 2f75 6c3e  e</a></li>.</ul>
+00005db0: 0a3c 2f6c 693e 0a3c 6c69 2063 6c61 7373  .</li>.<li class
+00005dc0: 3d22 746f 6374 7265 652d 6c31 223e 3c61  ="toctree-l1"><a
+00005dd0: 2063 6c61 7373 3d22 7265 6665 7265 6e63   class="referenc
+00005de0: 6520 696e 7465 726e 616c 2220 6872 6566  e internal" href
+00005df0: 3d22 6874 7470 733a 2f2f 6363 622e 6a68  ="https://ccb.jh
+00005e00: 752e 6564 752f 6c69 6674 6f6e 2f63 6f6e  u.edu/lifton/con
+00005e10: 7465 6e74 2f62 6568 696e 645f 7363 656e  tent/behind_scen
+00005e20: 6573 2e68 746d 6c22 3e42 6568 696e 6420  es.html">Behind 
+00005e30: 7468 6520 7363 656e 6573 3c2f 613e 3c75  the scenes</a><u
+00005e40: 6c3e 0a3c 6c69 2063 6c61 7373 3d22 746f  l>.<li class="to
+00005e50: 6374 7265 652d 6c32 223e 3c61 2063 6c61  ctree-l2"><a cla
+00005e60: 7373 3d22 7265 6665 7265 6e63 6520 696e  ss="reference in
+00005e70: 7465 726e 616c 2220 6872 6566 3d22 6874  ternal" href="ht
+00005e80: 7470 733a 2f2f 6363 622e 6a68 752e 6564  tps://ccb.jhu.ed
+00005e90: 752f 6c69 6674 6f6e 2f63 6f6e 7465 6e74  u/lifton/content
+00005ea0: 2f62 6568 696e 645f 7363 656e 6573 2e68  /behind_scenes.h
+00005eb0: 746d 6c23 6465 6369 6469 6e67 2d63 6872  tml#deciding-chr
+00005ec0: 6f6d 6f73 6f6d 6573 2d61 6e64 2d66 6561  omosomes-and-fea
+00005ed0: 7475 7265 732d 666f 722d 616e 6e6f 7461  tures-for-annota
+00005ee0: 7469 6f6e 2d6c 6966 742d 6f76 6572 223e  tion-lift-over">
+00005ef0: 4465 6369 6469 6e67 2063 6872 6f6d 6f73  Deciding chromos
+00005f00: 6f6d 6573 2061 6e64 2066 6561 7475 7265  omes and feature
+00005f10: 7320 666f 7220 616e 6e6f 7461 7469 6f6e  s for annotation
+00005f20: 206c 6966 742d 6f76 6572 3c2f 613e 3c2f   lift-over</a></
+00005f30: 6c69 3e0a 3c6c 6920 636c 6173 733d 2274  li>.<li class="t
+00005f40: 6f63 7472 6565 2d6c 3222 3e3c 6120 636c  octree-l2"><a cl
+00005f50: 6173 733d 2272 6566 6572 656e 6365 2069  ass="reference i
+00005f60: 6e74 6572 6e61 6c22 2068 7265 663d 2268  nternal" href="h
+00005f70: 7474 7073 3a2f 2f63 6362 2e6a 6875 2e65  ttps://ccb.jhu.e
+00005f80: 6475 2f6c 6966 746f 6e2f 636f 6e74 656e  du/lifton/conten
+00005f90: 742f 6265 6869 6e64 5f73 6365 6e65 732e  t/behind_scenes.
+00005fa0: 6874 6d6c 236d 6174 6368 696e 672d 6d69  html#matching-mi
+00005fb0: 6e69 7072 6f74 2d6c 6966 746f 6666 2d67  niprot-liftoff-g
+00005fc0: 656e 6f6d 652d 616e 6e6f 7461 7469 6f6e  enome-annotation
+00005fd0: 223e 4d61 7463 6869 6e67 206d 696e 6970  ">Matching minip
+00005fe0: 726f 7420 2661 6d70 3b20 4c69 6674 6f66  rot &amp; Liftof
+00005ff0: 6620 6765 6e6f 6d65 2061 6e6e 6f74 6174  f genome annotat
+00006000: 696f 6e3c 2f61 3e3c 2f6c 693e 0a3c 6c69  ion</a></li>.<li
+00006010: 2063 6c61 7373 3d22 746f 6374 7265 652d   class="toctree-
+00006020: 6c32 223e 3c61 2063 6c61 7373 3d22 7265  l2"><a class="re
+00006030: 6665 7265 6e63 6520 696e 7465 726e 616c  ference internal
+00006040: 2220 6872 6566 3d22 6874 7470 733a 2f2f  " href="https://
+00006050: 6363 622e 6a68 752e 6564 752f 6c69 6674  ccb.jhu.edu/lift
+00006060: 6f6e 2f63 6f6e 7465 6e74 2f62 6568 696e  on/content/behin
+00006070: 645f 7363 656e 6573 2e68 746d 6c23 7072  d_scenes.html#pr
+00006080: 6f74 6569 6e2d 6d61 7869 6d69 7a61 7469  otein-maximizati
+00006090: 6f6e 2d61 6c67 6f72 6974 686d 223e 5072  on-algorithm">Pr
+000060a0: 6f74 6569 6e2d 6d61 7869 6d69 7a61 7469  otein-maximizati
+000060b0: 6f6e 2061 6c67 6f72 6974 686d 3c2f 613e  on algorithm</a>
+000060c0: 3c2f 6c69 3e0a 3c6c 6920 636c 6173 733d  </li>.<li class=
+000060d0: 2274 6f63 7472 6565 2d6c 3222 3e3c 6120  "toctree-l2"><a 
+000060e0: 636c 6173 733d 2272 6566 6572 656e 6365  class="reference
+000060f0: 2069 6e74 6572 6e61 6c22 2068 7265 663d   internal" href=
+00006100: 2268 7474 7073 3a2f 2f63 6362 2e6a 6875  "https://ccb.jhu
+00006110: 2e65 6475 2f6c 6966 746f 6e2f 636f 6e74  .edu/lifton/cont
+00006120: 656e 742f 6265 6869 6e64 5f73 6365 6e65  ent/behind_scene
+00006130: 732e 6874 6d6c 236d 7574 6174 696f 6e2d  s.html#mutation-
+00006140: 7265 706f 7274 223e 4d75 7461 7469 6f6e  report">Mutation
+00006150: 2072 6570 6f72 743c 2f61 3e3c 2f6c 693e   report</a></li>
+00006160: 0a3c 6c69 2063 6c61 7373 3d22 746f 6374  .<li class="toct
+00006170: 7265 652d 6c32 223e 3c61 2063 6c61 7373  ree-l2"><a class
+00006180: 3d22 7265 6665 7265 6e63 6520 696e 7465  ="reference inte
+00006190: 726e 616c 2220 6872 6566 3d22 6874 7470  rnal" href="http
+000061a0: 733a 2f2f 6363 622e 6a68 752e 6564 752f  s://ccb.jhu.edu/
+000061b0: 6c69 6674 6f6e 2f63 6f6e 7465 6e74 2f62  lifton/content/b
+000061c0: 6568 696e 645f 7363 656e 6573 2e68 746d  ehind_scenes.htm
+000061d0: 6c23 7265 6665 7265 6e63 6522 3e52 6566  l#reference">Ref
+000061e0: 6572 656e 6365 3c2f 613e 3c2f 6c69 3e0a  erence</a></li>.
+000061f0: 3c2f 756c 3e0a 3c2f 6c69 3e0a 3c6c 6920  </ul>.</li>.<li 
+00006200: 636c 6173 733d 2274 6f63 7472 6565 2d6c  class="toctree-l
+00006210: 3122 3e3c 6120 636c 6173 733d 2272 6566  1"><a class="ref
+00006220: 6572 656e 6365 2069 6e74 6572 6e61 6c22  erence internal"
+00006230: 2068 7265 663d 2268 7474 7073 3a2f 2f63   href="https://c
+00006240: 6362 2e6a 6875 2e65 6475 2f6c 6966 746f  cb.jhu.edu/lifto
+00006250: 6e2f 636f 6e74 656e 742f 686f 775f 746f  n/content/how_to
+00006260: 5f70 6167 652e 6874 6d6c 223e 4641 5120  _page.html">FAQ 
+00006270: 2e2e 2e3c 2f61 3e3c 2f6c 693e 0a3c 6c69  ...</a></li>.<li
+00006280: 2063 6c61 7373 3d22 746f 6374 7265 652d   class="toctree-
+00006290: 6c31 223e 3c61 2063 6c61 7373 3d22 7265  l1"><a class="re
+000062a0: 6665 7265 6e63 6520 696e 7465 726e 616c  ference internal
+000062b0: 2220 6872 6566 3d22 6874 7470 733a 2f2f  " href="https://
+000062c0: 6363 622e 6a68 752e 6564 752f 6c69 6674  ccb.jhu.edu/lift
+000062d0: 6f6e 2f63 6f6e 7465 6e74 2f66 756e 6374  on/content/funct
+000062e0: 696f 6e5f 6d61 6e75 616c 2e68 746d 6c22  ion_manual.html"
+000062f0: 3e55 7365 7220 4d61 6e75 616c 3c2f 613e  >User Manual</a>
+00006300: 3c75 6c3e 0a3c 6c69 2063 6c61 7373 3d22  <ul>.<li class="
+00006310: 746f 6374 7265 652d 6c32 223e 3c61 2063  toctree-l2"><a c
+00006320: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
+00006330: 696e 7465 726e 616c 2220 6872 6566 3d22  internal" href="
+00006340: 6874 7470 733a 2f2f 6363 622e 6a68 752e  https://ccb.jhu.
+00006350: 6564 752f 6c69 6674 6f6e 2f63 6f6e 7465  edu/lifton/conte
+00006360: 6e74 2f66 756e 6374 696f 6e5f 6d61 6e75  nt/function_manu
+00006370: 616c 2e68 746d 6c23 6c69 6674 6f6e 223e  al.html#lifton">
+00006380: 4c69 6674 4f6e 3c2f 613e 3c2f 6c69 3e0a  LiftOn</a></li>.
+00006390: 3c2f 756c 3e0a 3c2f 6c69 3e0a 3c6c 6920  </ul>.</li>.<li 
+000063a0: 636c 6173 733d 2274 6f63 7472 6565 2d6c  class="toctree-l
+000063b0: 3122 3e3c 6120 636c 6173 733d 2272 6566  1"><a class="ref
+000063c0: 6572 656e 6365 2069 6e74 6572 6e61 6c22  erence internal"
+000063d0: 2068 7265 663d 2268 7474 7073 3a2f 2f63   href="https://c
+000063e0: 6362 2e6a 6875 2e65 6475 2f6c 6966 746f  cb.jhu.edu/lifto
+000063f0: 6e2f 636f 6e74 656e 742f 6368 616e 6765  n/content/change
+00006400: 6c6f 672e 6874 6d6c 223e 4368 616e 6765  log.html">Change
+00006410: 6c6f 673c 2f61 3e3c 756c 3e0a 3c6c 6920  log</a><ul>.<li 
+00006420: 636c 6173 733d 2274 6f63 7472 6565 2d6c  class="toctree-l
+00006430: 3222 3e3c 6120 636c 6173 733d 2272 6566  2"><a class="ref
+00006440: 6572 656e 6365 2069 6e74 6572 6e61 6c22  erence internal"
+00006450: 2068 7265 663d 2268 7474 7073 3a2f 2f63   href="https://c
+00006460: 6362 2e6a 6875 2e65 6475 2f6c 6966 746f  cb.jhu.edu/lifto
+00006470: 6e2f 636f 6e74 656e 742f 6368 616e 6765  n/content/change
+00006480: 6c6f 672e 6874 6d6c 2376 312d 302d 3022  log.html#v1-0-0"
+00006490: 3e76 312e 302e 303c 2f61 3e3c 2f6c 693e  >v1.0.0</a></li>
+000064a0: 0a3c 2f75 6c3e 0a3c 2f6c 693e 0a3c 6c69  .</ul>.</li>.<li
+000064b0: 2063 6c61 7373 3d22 746f 6374 7265 652d   class="toctree-
+000064c0: 6c31 223e 3c61 2063 6c61 7373 3d22 7265  l1"><a class="re
+000064d0: 6665 7265 6e63 6520 696e 7465 726e 616c  ference internal
+000064e0: 2220 6872 6566 3d22 6874 7470 733a 2f2f  " href="https://
+000064f0: 6363 622e 6a68 752e 6564 752f 6c69 6674  ccb.jhu.edu/lift
+00006500: 6f6e 2f63 6f6e 7465 6e74 2f6c 6963 656e  on/content/licen
+00006510: 7365 2e68 746d 6c22 3e4c 6963 656e 7365  se.html">License
+00006520: 3c2f 613e 3c2f 6c69 3e0a 3c6c 6920 636c  </a></li>.<li cl
+00006530: 6173 733d 2274 6f63 7472 6565 2d6c 3122  ass="toctree-l1"
+00006540: 3e3c 6120 636c 6173 733d 2272 6566 6572  ><a class="refer
+00006550: 656e 6365 2069 6e74 6572 6e61 6c22 2068  ence internal" h
+00006560: 7265 663d 2268 7474 7073 3a2f 2f63 6362  ref="https://ccb
+00006570: 2e6a 6875 2e65 6475 2f6c 6966 746f 6e2f  .jhu.edu/lifton/
+00006580: 636f 6e74 656e 742f 636f 6e74 6163 742e  content/contact.
+00006590: 6874 6d6c 223e 436f 6e74 6163 743c 2f61  html">Contact</a
+000065a0: 3e3c 2f6c 693e 0a3c 2f75 6c3e 0a3c 2f64  ></li>.</ul>.</d
+000065b0: 6976 3e0a 3c64 6976 2063 6c61 7373 3d22  iv>.<div class="
+000065c0: 6c69 6e65 2d62 6c6f 636b 223e 0a3c 6469  line-block">.<di
+000065d0: 7620 636c 6173 733d 226c 696e 6522 3e3c  v class="line"><
+000065e0: 6272 3e3c 2f64 6976 3e0a 3c2f 6469 763e  br></div>.</div>
+000065f0: 0a3c 2f73 6563 7469 6f6e 3e0a 3c73 6563  .</section>.<sec
+00006600: 7469 6f6e 2069 643d 226c 6966 746f 6e2d  tion id="lifton-
+00006610: 732d 6c69 6d69 7461 7469 6f6e 223e 0a3c  s-limitation">.<
+00006620: 6832 3e4c 6966 744f 6e27 7320 6c69 6d69  h2>LiftOn's limi
+00006630: 7461 7469 6f6e 3c61 2063 6c61 7373 3d22  tation<a class="
+00006640: 6865 6164 6572 6c69 6e6b 2220 6872 6566  headerlink" href
+00006650: 3d22 236c 6966 746f 6e2d 732d 6c69 6d69  ="#lifton-s-limi
+00006660: 7461 7469 6f6e 2220 7469 746c 653d 2250  tation" title="P
+00006670: 6572 6d61 6c69 6e6b 2074 6f20 7468 6973  ermalink to this
+00006680: 2068 6561 6469 6e67 223e 233c 2f61 3e3c   heading">#</a><
+00006690: 2f68 323e 0a3c 703e 4c69 6674 4f6e 2773  /h2>.<p>LiftOn's
+000066a0: 203c 656d 3e63 6861 696e 696e 6720 616c   <em>chaining al
+000066b0: 676f 7269 7468 6d3c 2f65 6d3e 2063 7572  gorithm</em> cur
+000066c0: 7265 6e74 6c79 206f 6e6c 7920 7574 696c  rently only util
+000066d0: 697a 6573 206d 696e 6970 726f 7420 616c  izes miniprot al
+000066e0: 6967 6e6d 656e 7420 7265 7375 6c74 7320  ignment results 
+000066f0: 746f 2066 6978 2074 6865 204c 6966 746f  to fix the Lifto
+00006700: 6666 2061 6e6e 6f74 6174 696f 6e2e 2048  ff annotation. H
+00006710: 6f77 6576 6572 2c20 6974 2063 616e 2062  owever, it can b
+00006720: 6520 6578 7465 6e64 6564 2074 6f20 6368  e extended to ch
+00006730: 6169 6e20 746f 6765 7468 6572 206d 756c  ain together mul
+00006740: 7469 706c 6520 444e 412d 2061 6e64 2070  tiple DNA- and p
+00006750: 726f 7465 696e 2d62 6173 6564 2061 6e6e  rotein-based ann
+00006760: 6f74 6174 696f 6e20 6669 6c65 7320 6f72  otation files or
+00006770: 2061 6173 656d 626c 6564 2052 4e41 2d53   aasembled RNA-S
+00006780: 6571 2074 7261 6e73 6372 6970 7473 2e3c  eq transcripts.<
+00006790: 2f70 3e0a 3c70 3e44 4e41 2d20 616e 6420  /p>.<p>DNA- and 
+000067a0: 7072 6f74 6569 6e2d 6261 7365 6420 6d65  protein-based me
+000067b0: 7468 6f64 7320 7374 696c 6c20 6861 7665  thods still have
+000067c0: 2073 6f6d 6520 6c69 6d69 7461 7469 6f6e   some limitation
+000067d0: 732e 2057 6520 6172 6520 6465 7665 6c6f  s. We are develo
+000067e0: 7069 6e67 2061 206d 6f64 756c 6520 746f  ping a module to
+000067f0: 206d 6572 6765 2074 6865 204c 6966 744f   merge the LiftO
+00006800: 6e20 616e 6e6f 7461 7469 6f6e 2077 6974  n annotation wit
+00006810: 6820 7468 6520 7265 6c65 6173 6564 2063  h the released c
+00006820: 7572 6174 6564 2061 6e6e 6f74 6174 696f  urated annotatio
+00006830: 6e73 2074 6f20 6765 6e65 7261 7465 2062  ns to generate b
+00006840: 6574 7465 7220 616e 6e6f 7461 7469 6f6e  etter annotation
+00006850: 732e 3c2f 703e 0a3c 703e 5468 6520 4c69  s.</p>.<p>The Li
+00006860: 6674 4f6e 203c 656d 3e63 6861 696e 696e  ftOn <em>chainin
+00006870: 6720 616c 676f 7269 7468 6d3c 2f65 6d3e  g algorithm</em>
+00006880: 206e 6f77 2064 6f65 7320 6e6f 7420 7375   now does not su
+00006890: 7070 6f72 7420 6d75 6c74 692d 7468 7265  pport multi-thre
+000068a0: 6164 696e 672e 2054 6869 7320 6675 6e63  ading. This func
+000068b0: 7469 6f6e 616c 6974 7920 7374 616e 6473  tionality stands
+000068c0: 2061 7320 6f75 7220 6e65 7874 2074 6172   as our next tar
+000068d0: 6765 7465 6420 6665 6174 7572 6520 6f6e  geted feature on
+000068e0: 2074 6865 2064 6576 656c 6f70 6d65 6e74   the development
+000068f0: 2068 6f72 697a 6f6e 213c 2f70 3e0a 3c64   horizon!</p>.<d
+00006900: 6976 2063 6c61 7373 3d22 6c69 6e65 2d62  iv class="line-b
+00006910: 6c6f 636b 223e 0a3c 6469 7620 636c 6173  lock">.<div clas
+00006920: 733d 226c 696e 6522 3e3c 6272 3e3c 2f64  s="line"><br></d
+00006930: 6976 3e0a 3c2f 6469 763e 0a3c 2f73 6563  iv>.</div>.</sec
+00006940: 7469 6f6e 3e0a 3c2f 7365 6374 696f 6e3e  tion>.</section>
+00006950: 0a0a 2020 2020 2020 2020 0a0a 2323 203c  ..        ..## <
+00006960: 6120 6e61 6d65 3d22 6369 7461 7469 6f6e  a name="citation
+00006970: 223e 3c2f 613e 4369 7461 7469 6f6e 3c61  "></a>Citation<a
+00006980: 2063 6c61 7373 3d22 6865 6164 6572 6c69   class="headerli
+00006990: 6e6b 2220 6872 6566 3d22 2363 6974 6174  nk" href="#citat
+000069a0: 696f 6e22 2074 6974 6c65 3d22 5065 726d  ion" title="Perm
+000069b0: 616c 696e 6b20 746f 2074 6869 7320 6865  alink to this he
+000069c0: 6164 696e 6722 3e23 3c2f 613e 0a0a 0a4b  ading">#</a>...K
+000069d0: 7561 6e2d 4861 6f20 4368 616f 2a2c 204d  uan-Hao Chao*, M
+000069e0: 6968 6165 6c61 2050 6572 7465 612c 2053  ihaela Pertea, S
+000069f0: 7465 7665 6e20 4c20 5361 6c7a 6265 7267  teven L Salzberg
+00006a00: 2a2c 2022 4c69 6674 4f6e 3a20 6120 746f  *, "LiftOn: a to
+00006a10: 6f6c 2074 6f20 696d 7072 6f76 6520 616e  ol to improve an
+00006a20: 6e6f 7461 7469 6f6e 7320 666f 7220 7072  notations for pr
+00006a30: 6f74 6569 6e2d 636f 6469 6e67 2067 656e  otein-coding gen
+00006a40: 6573 2064 7572 696e 6720 7468 6520 6c69  es during the li
+00006a50: 6674 2d6f 7665 7220 7072 6f63 6573 732e  ft-over process.
+00006a60: 222c 203c 693e 6269 6f52 7869 763c 2f69  ", <i>bioRxiv</i
+00006a70: 3e20 3c62 3e32 3032 332e 3037 2e32 372e  > <b>2023.07.27.
+00006a80: 3535 3037 3534 3c2f 623e 2c20 646f 693a  550754</b>, doi:
+00006a90: 205b 6874 7470 733a 2f2f 646f 692e 6f72   [https://doi.or
+00006aa0: 672f 3130 2e31 3130 312f 3230 3233 2e30  g/10.1101/2023.0
+00006ab0: 372e 3237 2e35 3530 3735 345d 2868 7474  7.27.550754](htt
+00006ac0: 7073 3a2f 2f64 6f69 2e6f 7267 2f31 302e  ps://doi.org/10.
+00006ad0: 3131 3031 2f32 3032 332e 3037 2e32 372e  1101/2023.07.27.
+00006ae0: 3535 3037 3534 292c 2032 3032 330a 0a3c  550754), 2023..<
+00006af0: 6272 3e0a 3c62 723e 0a3c 6272 3e0a 0a3c  br>.<br>.<br>..<
+00006b00: 696d 6720 616c 743d 224d 7920 4c6f 676f  img alt="My Logo
+00006b10: 2220 636c 6173 733d 226c 6f67 6f20 6865  " class="logo he
+00006b20: 6164 6572 2d69 6d61 6765 206f 6e6c 792d  ader-image only-
+00006b30: 6c69 6768 7420 616c 6967 6e2d 6365 6e74  light align-cent
+00006b40: 6572 2220 7372 633d 2268 7474 7073 3a2f  er" src="https:/
+00006b50: 2f73 746f 7261 6765 2e67 6f6f 676c 6561  /storage.googlea
+00006b60: 7069 732e 636f 6d2f 7374 6f72 6167 652e  pis.com/storage.
+00006b70: 6b68 6368 616f 2e63 6f6d 2f66 6967 7572  khchao.com/figur
+00006b80: 6573 2f6a 6875 2d6c 6f67 6f2d 6461 726b  es/jhu-logo-dark
+00006b90: 2e70 6e67 223e 0a                        .png">.
```

### Comparing `lifton-0.0.3/lifton/align.py` & `lifton-1.0.0/lifton/align.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/annotation.py` & `lifton-1.0.0/lifton/annotation.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/extract_sequence.py` & `lifton-1.0.0/lifton/extract_sequence.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/get_id_fraction.py` & `lifton-1.0.0/lifton/get_id_fraction.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/intervals.py` & `lifton-1.0.0/lifton/intervals.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/liftoff/align_features.py` & `lifton-1.0.0/lifton/liftoff/align_features.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/liftoff/aligned_seg.py` & `lifton-1.0.0/lifton/liftoff/aligned_seg.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/liftoff/extract_features.py` & `lifton-1.0.0/lifton/liftoff/extract_features.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/liftoff/find_best_mapping.py` & `lifton-1.0.0/lifton/liftoff/find_best_mapping.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/liftoff/fix_overlapping_features.py` & `lifton-1.0.0/lifton/liftoff/fix_overlapping_features.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/liftoff/lift_features.py` & `lifton-1.0.0/lifton/liftoff/lift_features.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/liftoff/liftoff_main.py` & `lifton-1.0.0/lifton/liftoff/liftoff_main.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/liftoff/liftoff_utils.py` & `lifton-1.0.0/lifton/liftoff/liftoff_utils.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/liftoff/liftover_types.py` & `lifton-1.0.0/lifton/liftoff/liftover_types.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/liftoff/merge_lifted_features.py` & `lifton-1.0.0/lifton/liftoff/merge_lifted_features.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/liftoff/polish.py` & `lifton-1.0.0/lifton/liftoff/polish.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/liftoff/tests/test_advanced.py` & `lifton-1.0.0/lifton/liftoff/tests/test_advanced.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/liftoff/tests/test_basic.py` & `lifton-1.0.0/lifton/liftoff/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/liftoff/write_new_gff.py` & `lifton-1.0.0/lifton/liftoff/write_new_gff.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/lifton.py` & `lifton-1.0.0/lifton/lifton.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 
 
 def parse_args(arglist):
     parser = argparse.ArgumentParser(description='Lift features from one genome assembly to another')
     parser.add_argument('target', help='target fasta genome to lift genes to')
     parser.add_argument('reference', help='reference fasta genome to lift genes from')
     parser.add_argument('-E', '--evaluation', help='Run LiftOn in evaluation mode', action='store_true', default = False)
+    parser.add_argument('-EL', '--evaluation-liftoff-chm13', help='Run LiftOn in evaluation mode', action='store_true', default = False)
     parser.add_argument('-c', '--write_chains', help='Write chaining files', action='store_true', default = True)
     parser_outgrp = args_outgrp(parser)
     parser_aligngrp = args_aligngrp(parser)
     args_optional(parser)
     referencegrp = parser.add_argument_group('* Required input (Reference annotation)')    
     referencegrp.add_argument(
         '-g', '--reference-annotation', metavar='GFF',  required=True,
@@ -185,16 +186,16 @@
     else:
         outdir = os.path.dirname(args.output)
         outdir = outdir if outdir != "" else "."
         os.makedirs(outdir, exist_ok=True)
     lifton_outdir = f"{outdir}/lifton_output/"
     args.directory = "intermediate_files/"
     intermediate_dir = f"{outdir}/lifton_output/{args.directory}"
-    stats_dir= f"{outdir}/lifton_output/stats/"
     os.makedirs(intermediate_dir, exist_ok=True)
+    stats_dir= f"{outdir}/lifton_output/stats/"
     os.makedirs(stats_dir, exist_ok=True)
     args.directory = intermediate_dir
     logger.log(">> Reading target genome ...", debug=True)
     tgt_fai = Fasta(tgt_genome)
     logger.log(">> Reading reference genome ...", debug=True)
     ref_fai = Fasta(ref_genome)    
 
@@ -249,15 +250,14 @@
         os.makedirs(lifton_outdir, exist_ok=True)
         tgt_feature_db = annotation.Annotation(tgt_annotation, args.infer_genes).db_connection
         fw_score = open(lifton_outdir+"/eval.txt", "w")
         tree_dict = {}
         processed_features = 0
         for feature in features:
             for locus in tgt_feature_db.features_of_type(feature):#, limit=("chr1", 146652669, 146708545)):
-                # evaluation.tgt_evaluate(None, locus, ref_db.db_connection, tgt_feature_db, tree_dict, tgt_fai, ref_features_dict, ref_proteins, ref_trans, fw_score, args.debug)
                 lifton_gene = run_evaluation.evaluation(None, locus, ref_db.db_connection, tgt_feature_db, tree_dict, tgt_fai, ref_proteins, ref_trans, ref_features_dict, fw_score, args, ENTRY_FEATURE=True)
                 if processed_features % 20 == 0:
                     sys.stdout.write("\r>> LiftOn evaluated: %i features." % processed_features)
                 processed_features += 1
         fw_score.close()
         return
 
@@ -343,8 +343,10 @@
     ██║     ██║██╔══╝     ██║   ██║   ██║██║╚██╗██║
     ███████╗██║██║        ██║   ╚██████╔╝██║ ╚████║
     ╚══════╝╚═╝╚═╝        ╚═╝    ╚═════╝ ╚═╝  ╚═══╝
     '''
     print(banner, file=sys.stderr)
     print(f"{__version__}\n", file=sys.stderr)
     args = parse_args(arglist)
+    if not run_miniprot.check_miniprot_installed(): 
+        sys.exit("miniprot is not installed. Please install miniprot before running LiftOn.")
     run_all_lifton_steps(args)
```

### Comparing `lifton-0.0.3/lifton/lifton_class.py` & `lifton-1.0.0/lifton/lifton_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,19 +129,23 @@
 
     def add_exon(self, trans_id, gffutil_entry_exon):
         self.transcripts[trans_id].add_exon(gffutil_entry_exon)
 
     def add_cds(self, trans_id, gffutil_entry_cds):
         self.transcripts[trans_id].add_cds(gffutil_entry_cds)
                             
-    def orf_search_protein(self, trans_id, ref_trans_id, fai, ref_proteins, fai_trans, lifton_status, eval_only=False):
+    def orf_search_protein(self, trans_id, ref_trans_id, fai, ref_proteins, fai_trans, lifton_status, eval_only=False, eval_liftoff_chm13=False):
         if trans_id not in self.transcripts.keys():
             return None, False
-        ref_protein_seq = str(ref_proteins[ref_trans_id]) if ref_trans_id in ref_proteins else None
-        ref_trans_seq = str(fai_trans[ref_trans_id]) if ref_trans_id in fai_trans else None
+        if not eval_liftoff_chm13:
+            ref_protein_seq = str(ref_proteins[ref_trans_id]) if ref_trans_id in ref_proteins.keys() else None
+            ref_trans_seq = str(fai_trans[ref_trans_id]) if ref_trans_id in fai_trans.keys() else None
+        else:
+            ref_protein_seq = str(ref_proteins["rna-"+ref_trans_id]) if "rna-"+ref_trans_id in ref_proteins.keys() else None
+            ref_trans_seq = str(fai_trans["rna-"+ref_trans_id]) if "rna-"+ref_trans_id in fai_trans.keys() else None
         lifton_aln, good_trans = self.transcripts[trans_id].orf_search_protein(fai, ref_protein_seq, ref_trans_seq, lifton_status, is_non_coding=self.is_non_coding, eval_only=eval_only)
         return lifton_aln, good_trans
 
     def update_cds_list(self, trans_id, cds_list):
         self.transcripts[trans_id].update_cds_list(cds_list)
         self.update_boundaries()
```

### Comparing `lifton-0.0.3/lifton/lifton_utils.py` & `lifton-1.0.0/lifton/lifton_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,14 @@
     ref_trans_exon_num_dict = {}
     new_gene_feature = lifton_class.Lifton_feature("Lifton-gene")
     ref_features_dict["LiftOn-gene"] = new_gene_feature
     for f_itr in features:
         for locus in ref_db.db_connection.features_of_type(f_itr):
             CDS_children = list(ref_db.db_connection.children(locus, featuretype='CDS'))
             feature = lifton_class.Lifton_feature(locus.id)
-
             # Write out reference gene features IDs
             # Decide if its type
             gene_type_key = ""
             if args.annotation_database.upper() == "REFSEQ":
                 gene_type_key = "gene_biotype"
             elif args.annotation_database.upper() == "GENCODE" or args.annotation_database.upper() == "ENSEMBL" or args.annotation_database.upper() == "CHESS":
                 gene_type_key = "gene_type"
@@ -345,33 +344,33 @@
             exon_children = list(ref_db.db_connection.children(locus, featuretype='exon', level=1, order_by='start'))
             if len(exon_children) > 0:
                 __process_ref_liffover_features(locus, ref_db, None)
             else:
                 transcripts = ref_db.db_connection.children(locus, level=1)
                 for transcript in list(transcripts):
                     __process_ref_liffover_features(transcript, ref_db, feature)
-                    ref_features_reverse_dict[transcript.id] = locus.id
+                    ref_features_reverse_dict[transcript.id if not args.evaluation_liftoff_chm13 else locus.id[4:]] = locus.id
                     all_CDS_in_trans = list(ref_db.db_connection.children(transcript, featuretype='CDS', order_by='start'))
                     if len(all_CDS_in_trans) > 0:
-                        ref_trans_exon_num_dict[transcript.id] = len(all_CDS_in_trans)
+                        ref_trans_exon_num_dict[transcript.id if not args.evaluation_liftoff_chm13 else locus.id[4:]] = len(all_CDS_in_trans)
                     else:
-                        ref_trans_exon_num_dict[transcript.id] = 0
+                        ref_trans_exon_num_dict[transcript.id if not args.evaluation_liftoff_chm13 else locus.id[4:]] = 0
                     # Write out reference trans feature IDs
                     if feature.is_protein_coding and transcript.featuretype == "mRNA":
                         fw_trans.write(f"{transcript.id}\tcoding\n")
                     elif feature.is_non_coding and (transcript.featuretype == "ncRNA" or transcript.featuretype == "nc_RNA" or transcript.featuretype == "lncRNA" or transcript.featuretype == "lnc_RNA"):
                         fw_trans.write(f"{transcript.id}\tnon-coding\n")
                     else:
                         fw_trans.write(f"{transcript.id}\tother\n")
-            ref_features_dict[locus.id] = feature
+            ref_features_dict[locus.id if not args.evaluation_liftoff_chm13 else locus.id[5:]] = feature
             all_CDS_children = list(ref_db.db_connection.children(locus, featuretype='CDS', order_by='start'))
             if len(all_CDS_children) > 0:
-                ref_features_len_dict[locus.id] = all_CDS_children[-1].end - all_CDS_children[0].start + 1
+                ref_features_len_dict[locus.id if not args.evaluation_liftoff_chm13 else locus.id[5:]] = all_CDS_children[-1].end - all_CDS_children[0].start + 1
             else:
-                ref_features_len_dict[locus.id] = 0
+                ref_features_len_dict[locus.id if not args.evaluation_liftoff_chm13 else locus.id[5:]] = 0
     fw_gene.close()
     fw_trans.close()
     return ref_features_dict, ref_features_len_dict, ref_features_reverse_dict, ref_trans_exon_num_dict
 
 
 def __process_ref_liffover_features(locus, ref_db, feature):
     if feature != None:
@@ -464,14 +463,19 @@
 
 
 def write_lifton_status(fw_score, transcript_id, transcript, lifton_status):
     final_status = ";".join(lifton_status.status)
     fw_score.write(f"{transcript_id}\t{lifton_status.liftoff}\t{lifton_status.miniprot}\t{lifton_status.lifton_dna}\t{lifton_status.lifton_aa}\t{lifton_status.annotation}\t{final_status}\t{transcript.seqid}:{transcript.start}-{transcript.end}\n")
 
 
+def write_lifton_eval_status(fw_score, transcript_id, transcript, lifton_status):
+    final_status = ";".join(lifton_status.status)
+    fw_score.write(f"{transcript_id}\t{lifton_status.lifton_dna}\t{lifton_status.lifton_aa}\t{final_status}\t{transcript.seqid}:{transcript.start}-{transcript.end}\n")
+
+
 def write_lifton_chains(fw_chain, transcript_id, chains):
     chain_ls = ";".join(chains)
     fw_chain.write(f"{transcript_id}\t{chain_ls}\n")
 
 
 def segments_overlap_length(segment1, segment2):
     """
```

### Comparing `lifton-0.0.3/lifton/protein_maximization.py` & `lifton-1.0.0/lifton/protein_maximization.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/run_evaluation.py` & `lifton-1.0.0/lifton/run_evaluation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,81 @@
 import copy 
-from lifton import lifton_class, lifton_utils, run_liftoff
+from lifton import lifton_class, lifton_utils
 
-def evaluation_with_protein(locus, lifton_trans, tgt_fai, ref_trans_id, ref_proteins, lifton_status):
+def initialize_lifton_gene_eval(locus, ref_db, tree_dict, ref_features_dict, args, with_exons=False):
     """
-        This function process evaluated gene locus with protein.
+        This function initializes Lifton gene instance.
 
         Parameters:
         - locus: gffutils feature instance
-        - lifton_gene: Lifton gene instance
-        - lifton_trans: Lifton transcript instance
-        - ref_id_2_m_id_trans_dict: reference id to miniprot transcript ids dictionary
-        - m_feature_db: miniprot feature database
+        - ref_db: reference database
         - tree_dict: intervaltree dictionary for each chromosome
-        - tgt_fai: target fasta index
+        - ref_features_dict: reference features dictionary
+        - with_exons: True if the gene has exons, False otherwise
+
+        Returns:
+        lifton_gene: Lifton gene instance
+        ref_gene_id: reference gene
+        ref_trans_id: reference transcript
+    """
+    ref_gene_id, ref_trans_id = lifton_utils.get_ref_ids_liftoff(ref_features_dict, locus.id, None)
+    if ref_gene_id is None: return None, None, None
+    if not args.evaluation_liftoff_chm13:
+        lifton_gene = lifton_class.Lifton_GENE(ref_gene_id, copy.deepcopy(locus), copy.deepcopy(ref_db[ref_gene_id].attributes), tree_dict, ref_features_dict, args, tmp=with_exons)
+    else:
+        lifton_gene = lifton_class.Lifton_GENE(ref_gene_id, copy.deepcopy(locus), copy.deepcopy(ref_db["gene-"+ref_gene_id].attributes), tree_dict, ref_features_dict, args, tmp=with_exons)
+    return lifton_gene, ref_gene_id, ref_trans_id
+
+
+def lifton_add_trans_exon_cds_eval(lifton_gene, locus, ref_db, tgt_db, ref_trans_id, args):
+    """
+        This function adds transcript, exons, and CDSs to the Lifton gene instance.
+
+        Parameters:
+        - lifton_gene: Lifton gene instance
+        - locus: gffutils feature instance
+        - ref_db: reference database
+        - tgt_db: liftoff feature database
         - ref_trans_id: reference transcript ID
-        - ref_proteins: reference proteins dictionary
-        - ref_trans: reference transcript dictionary
-        - fw_chain: file writer for chains
-        - write_chains: write chains or not
-        - lifton_status: Lifton_Status instance
-        - DEBUG: debug mode
+
+        Returns:
+        lifton_trans: Lifton transcript instance
+        len(cdss_list): number of CDSs
     """
-    # Liftoff alignment
-    eval_aln = lifton_utils.LiftOn_eval_alignment(lifton_trans, locus, tgt_fai, ref_proteins, ref_trans_id, lifton_status)
-    # miniprot alignment
-    if eval_aln is None:
-        lifton_status.annotation = "no_ref_protein"
+    try:
+        ref_db["rna-"+ref_trans_id]
+    except:
+        return None, 0
+    if not args.evaluation_liftoff_chm13:
+        lifton_trans = lifton_gene.add_transcript(ref_trans_id, copy.deepcopy(locus), copy.deepcopy(ref_db[ref_trans_id].attributes))
+    else:
+        try:
+            ref_db["rna-"+ref_trans_id]
+        except:
+            return None, 0
+        lifton_trans = lifton_gene.add_transcript(ref_trans_id, copy.deepcopy(locus), copy.deepcopy(ref_db["rna-"+ref_trans_id].attributes))
+    exons = tgt_db.children(locus, featuretype='exon', order_by='start')
+    for exon in list(exons):
+        lifton_gene.add_exon(lifton_trans.entry.id, exon)
+    cdss = tgt_db.children(locus, featuretype=('CDS', 'stop_codon'), order_by='start') 
+    cdss_list = list(cdss)
+    for cds in cdss_list:
+        lifton_gene.add_cds(lifton_trans.entry.id, cds)
+    return lifton_trans, len(cdss_list)
 
 
-def evaluation(lifton_gene, locus, ref_db, l_feature_db, tree_dict, tgt_fai, ref_proteins, ref_trans, ref_features_dict, fw_score, args, ENTRY_FEATURE=False):
+def evaluation(lifton_gene, locus, ref_db, tgt_db, tree_dict, tgt_fai, ref_proteins, ref_trans, ref_features_dict, fw_score, args, ENTRY_FEATURE=False):
     """
         This function evaluates annotation.
 
         Parameters:
         - lifton_gene: Lifton gene instance
         - locus: feature instance 
         - ref_db: reference database
-        - l_feature_db: liftoff feature database
+        - tgt_db: liftoff feature database
         - ref_id_2_m_id_trans_dict: reference id to miniprot transcript ids dictionary
         - m_feature_db: miniprot feature database
         - tree_dict: intervaltree dictionary for each chromosome
         - tgt_fai: target fasta index
         - ref_proteins: reference protein dictionary
         - ref_trans: reference transcript dictionary
         - ref_features_dict: reference features dictionary
@@ -49,34 +84,33 @@
         - write_chains: write chains or not
         - DEBUG: debug mode
         - ENTRY_FEATURE: True if the feature is the root feature for a gene locus
 
         Returns:
         lifton_gene: LiftOn gene instance
     """
-    exon_children = list(l_feature_db.children(locus, featuretype='exon', level=1, order_by='start'))
+    exon_children = list(tgt_db.children(locus, featuretype='exon', level=1, order_by='start'))
     if lifton_gene is None and ENTRY_FEATURE:   
         # Gene (1st) features
-        lifton_gene, ref_gene_id, ref_trans_id = run_liftoff.initialize_lifton_gene(locus, ref_db, tree_dict, ref_features_dict, args, with_exons=len(exon_children)>0)
-        if lifton_gene.ref_gene_id is None: return None            
+        lifton_gene, ref_gene_id, ref_trans_id = initialize_lifton_gene_eval(locus, ref_db, tree_dict, ref_features_dict, args, with_exons=len(exon_children)>0)
+        if lifton_gene is None or lifton_gene.ref_gene_id is None: return None            
     if len(exon_children) == 0:
         parent_feature = None
         if ENTRY_FEATURE: # Gene (1st) features without direct exons 
             parent_feature = lifton_gene
         else: # Middle features without exons
             parent_feature = lifton_gene.add_feature(copy.deepcopy(locus))
-        features = l_feature_db.children(locus, level=1)
+        features = tgt_db.children(locus, level=1)
         for feature in list(features):
-            lifton_gene = evaluation(parent_feature, feature, ref_db, l_feature_db, tree_dict, tgt_fai, ref_proteins, ref_trans, ref_features_dict, fw_score, args)
+            lifton_gene = evaluation(parent_feature, feature, ref_db, tgt_db, tree_dict, tgt_fai, ref_proteins, ref_trans, ref_features_dict, fw_score, args)
     else:
         if ENTRY_FEATURE: # Gene (1st) features with direct exons 
             ref_trans_id = ref_gene_id
         else: # Transcript features with direct exons 
             ref_gene_id, ref_trans_id = lifton_utils.get_ref_ids_liftoff(ref_features_dict, lifton_gene.entry.id, locus.id)
         lifton_status = lifton_class.Lifton_Status()
-        lifton_status.annotation = "Evaluation"
-        lifton_trans, cds_num = run_liftoff.lifton_add_trans_exon_cds(lifton_gene, locus, ref_db, l_feature_db, ref_trans_id)
-        if cds_num > 0:
-            evaluation_with_protein(locus, lifton_trans, tgt_fai, ref_trans_id, ref_proteins, lifton_status)
-        lifton_trans_aln, lifton_aa_aln = lifton_gene.orf_search_protein(lifton_trans.entry.id, ref_trans_id, tgt_fai, ref_proteins, ref_trans, lifton_status, eval_only=True)
+        lifton_trans, cds_num = lifton_add_trans_exon_cds_eval(lifton_gene, locus, ref_db, tgt_db, ref_trans_id, args)
+        if lifton_trans == None: return lifton_gene
+        lifton_trans_aln, lifton_aa_aln = lifton_gene.orf_search_protein(lifton_trans.entry.id, ref_trans_id, tgt_fai, ref_proteins, ref_trans, lifton_status, eval_only=True, eval_liftoff_chm13=args.evaluation_liftoff_chm13)
         lifton_utils.print_lifton_status(lifton_trans.entry.id, locus, lifton_status, DEBUG=args.debug)
+        lifton_utils.write_lifton_eval_status(fw_score, lifton_trans.entry.id, locus, lifton_status)
     return lifton_gene
```

### Comparing `lifton-0.0.3/lifton/run_liftoff.py` & `lifton-1.0.0/lifton/run_liftoff.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         liftoff_annotation: liftoff annotation file path
     """
     liftoff_args = copy.deepcopy(args)
     liftoff_outdir = output_dir + "liftoff/"    
     os.makedirs(liftoff_outdir, exist_ok=True)
     liftoff_annotation = liftoff_outdir + "liftoff.gff3"
     liftoff_args.output = liftoff_annotation
+    liftoff_args.u = liftoff_outdir + "unmapped_features.txt"
     liftoff_main.run_all_liftoff_steps(liftoff_args)
     if args.polish:
         liftoff_annotation += "_polished"
     # test_basic.test_yeast(liftoff_outdir + "test_basic/")
     # test_advanced.test_yeast(liftoff_outdir + "test_advance/")
     return liftoff_annotation
 
@@ -169,12 +170,12 @@
         lifton_trans, cds_num = lifton_add_trans_exon_cds(lifton_gene, locus, ref_db, l_feature_db, ref_trans_id)
         if cds_num > 0:
             process_liftoff_with_protein(locus, lifton_gene, lifton_trans,
                                         ref_id_2_m_id_trans_dict, m_feature_db, tree_dict,
                                         tgt_fai, ref_trans_id, ref_proteins, ref_trans,
                                         fw_chain, args.write_chains, lifton_status, args.debug)
         lifton_trans_aln, lifton_aa_aln = lifton_gene.orf_search_protein(lifton_trans.entry.id, ref_trans_id, tgt_fai, ref_proteins, ref_trans, lifton_status)
-        lifton_utils.print_lifton_status(lifton_trans.entry.id, locus, lifton_status, DEBUG=args.debug)
+        # lifton_utils.print_lifton_status(lifton_trans.entry.id, locus, lifton_status, DEBUG=args.debug)
         lifton_gene.add_lifton_gene_status_attrs("Liftoff")
         lifton_gene.add_lifton_trans_status_attrs(lifton_trans.entry.id, lifton_status)
         lifton_utils.write_lifton_status(fw_score, lifton_trans.entry.id, locus, lifton_status)
     return lifton_gene
```

### Comparing `lifton-0.0.3/lifton/run_miniprot.py` & `lifton-1.0.0/lifton/run_miniprot.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,14 @@
     return lifton_gene, Lifton_trans, Lifton_trans.entry.id, lifton_status
 
 
 def process_miniprot(mtrans, ref_db, m_feature_db, tree_dict, tgt_fai, ref_proteins, ref_trans, ref_features_dict, fw_score, m_id_2_ref_id_trans_dict, ref_features_len_dict, ref_trans_exon_num_dict, ref_features_reverse_dict, args):
     mtrans_id = mtrans.attributes["ID"][0]
     mtrans_interval = Interval(mtrans.start, mtrans.end, mtrans_id)
     is_overlapped = lifton_utils.check_ovps_ratio(mtrans, mtrans_interval, args.overlap, tree_dict)
-    print(f"mtrans_id: {mtrans_id}, is_overlapped: {is_overlapped}")
     lifton_gene = None
     lifton_trans = None
     if not is_overlapped:
         ref_trans_id = m_id_2_ref_id_trans_dict[mtrans_id]            
         ref_gene_id, ref_trans_id = lifton_utils.get_ref_ids_miniprot(ref_features_reverse_dict, mtrans_id, m_id_2_ref_id_trans_dict)
         if ref_gene_id is None:
             return None
```

### Comparing `lifton-0.0.3/lifton/stats.py` & `lifton-1.0.0/lifton/stats.py`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/lifton/variants.py` & `lifton-1.0.0/lifton/variants.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         lifton_status.status = mutation_type
         return
     if align_dna == None:
         mutation_type.append('full_transcript_loss')
         lifton_status.status = mutation_type
         return 
     if align_protein == None:
-        mutation_type.append('no_protein_loss')
+        mutation_type.append('no_protein')
         lifton_status.status = mutation_type
         return 
     # 1. return cases
     if align_dna.identity == 1.0:
         mutation_type.append('identical')
         lifton_status.status = mutation_type
         return
```

### Comparing `lifton-0.0.3/lifton.egg-info/PKG-INFO` & `lifton-1.0.0/lifton.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,1418 +1,1742 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6c69 6674  : 2.1.Name: lift
-00000020: 6f6e 0a56 6572 7369 6f6e 3a20 302e 302e  on.Version: 0.0.
-00000030: 330a 5375 6d6d 6172 793a 2041 2070 726f  3.Summary: A pro
-00000040: 7465 696e 2d63 6f64 696e 6720 6765 6e65  tein-coding gene
-00000050: 2061 6e6e 6f74 6174 696f 6e20 6669 7869   annotation fixi
-00000060: 6e67 2074 6f6f 6c0a 486f 6d65 2d70 6167  ng tool.Home-pag
-00000070: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
-00000080: 622e 636f 6d2f 4b75 616e 6861 6f2d 4368  b.com/Kuanhao-Ch
-00000090: 616f 2f4c 6966 746f 6e0a 4175 7468 6f72  ao/Lifton.Author
-000000a0: 3a20 4b75 616e 2d48 616f 2043 6861 6f0a  : Kuan-Hao Chao.
-000000b0: 4175 7468 6f72 2d65 6d61 696c 3a20 6b68  Author-email: kh
-000000c0: 2e63 6861 6f40 6373 2e6a 6875 2e65 6475  .chao@cs.jhu.edu
-000000d0: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
-000000e0: 3a20 3e3d 332e 360a 4465 7363 7269 7074  : >=3.6.Descript
-000000f0: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-00000100: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
-00000110: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
-00000120: 4345 4e53 450a 0a3c 696d 6720 616c 743d  CENSE..<img alt=
-00000130: 224d 7920 4c6f 676f 2220 636c 6173 733d  "My Logo" class=
-00000140: 226c 6f67 6f20 6865 6164 6572 2d69 6d61  "logo header-ima
-00000150: 6765 206f 6e6c 792d 6c69 6768 7420 616c  ge only-light al
-00000160: 6967 6e2d 6365 6e74 6572 2220 7372 633d  ign-center" src=
-00000170: 2267 7261 7068 6963 732f 4c69 6674 4f6e  "graphics/LiftOn
-00000180: 5f63 6f6c 6f72 2e70 6e67 2220 7374 796c  _color.png" styl
-00000190: 653d 2277 6964 7468 3a39 3025 223e 0a0a  e="width:90%">..
-000001a0: 3c64 6976 2063 6c61 7373 3d22 636f 6e74  <div class="cont
-000001b0: 656e 7422 3e0a 0a3c 6469 7620 636c 6173  ent">..<div clas
-000001c0: 733d 226c 696e 6522 3e3c 6272 3e3c 2f64  s="line"><br></d
-000001d0: 6976 3e0a 3c2f 6469 763e 0a3c 7365 6374  iv>.</div>.<sect
-000001e0: 696f 6e20 6964 3d22 6c69 6674 6f6e 2d73  ion id="lifton-s
-000001f0: 2d74 7574 6f72 6961 6c22 3e0a 3c65 6d62  -tutorial">.<emb
-00000200: 6564 3e0a 3c61 2063 6c61 7373 3d22 7265  ed>.<a class="re
-00000210: 6665 7265 6e63 6520 6578 7465 726e 616c  ference external
-00000220: 2069 6d61 6765 2d72 6566 6572 656e 6365   image-reference
-00000230: 2220 6872 6566 3d22 6874 7470 733a 2f2f  " href="https://
-00000240: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00000250: 6164 6765 2f4c 6963 656e 7365 2d47 504c  adge/License-GPL
-00000260: 7633 2d79 656c 6c6f 772e 7376 6722 3e3c  v3-yellow.svg"><
-00000270: 696d 6720 616c 743d 2268 7474 7073 3a2f  img alt="https:/
-00000280: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000290: 6261 6467 652f 4c69 6365 6e73 652d 4750  badge/License-GP
-000002a0: 4c76 332d 7965 6c6c 6f77 2e73 7667 2220  Lv3-yellow.svg" 
-000002b0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-000002c0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-000002d0: 652f 4c69 6365 6e73 652d 4750 4c76 332d  e/License-GPLv3-
-000002e0: 7965 6c6c 6f77 2e73 7667 223e 3c2f 613e  yellow.svg"></a>
-000002f0: 0a3c 6120 636c 6173 733d 2272 6566 6572  .<a class="refer
-00000300: 656e 6365 2065 7874 6572 6e61 6c20 696d  ence external im
-00000310: 6167 652d 7265 6665 7265 6e63 6522 2068  age-reference" h
-00000320: 7265 663d 2268 7474 7073 3a2f 2f69 6d67  ref="https://img
-00000330: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000340: 652f 7665 7273 696f 6e2d 762e 302e 302e  e/version-v.0.0.
-00000350: 312d 626c 7565 223e 3c69 6d67 2061 6c74  1-blue"><img alt
-00000360: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00000370: 6965 6c64 732e 696f 2f62 6164 6765 2f76  ields.io/badge/v
-00000380: 6572 7369 6f6e 2d76 2e30 2e30 2e31 2d62  ersion-v.0.0.1-b
-00000390: 6c75 6522 2073 7263 3d22 6874 7470 733a  lue" src="https:
-000003a0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-000003b0: 2f62 6164 6765 2f76 6572 7369 6f6e 2d76  /badge/version-v
-000003c0: 2e30 2e30 2e31 2d62 6c75 6522 3e3c 2f61  .0.0.1-blue"></a
-000003d0: 3e0a 3c61 2063 6c61 7373 3d22 7265 6665  >.<a class="refe
-000003e0: 7265 6e63 6520 6578 7465 726e 616c 2069  rence external i
-000003f0: 6d61 6765 2d72 6566 6572 656e 6365 2220  mage-reference" 
-00000400: 6872 6566 3d22 6874 7470 733a 2f2f 7065  href="https://pe
-00000410: 7079 2e74 6563 682f 7072 6f6a 6563 742f  py.tech/project/
-00000420: 6c69 6674 6f6e 223e 3c69 6d67 2061 6c74  lifton"><img alt
-00000430: 3d22 6874 7470 733a 2f2f 7374 6174 6963  ="https://static
-00000440: 2e70 6570 792e 7465 6368 2f70 6572 736f  .pepy.tech/perso
-00000450: 6e61 6c69 7a65 642d 6261 6467 652f 6c69  nalized-badge/li
-00000460: 6674 6f6e 3f70 6572 696f 643d 746f 7461  fton?period=tota
-00000470: 6c26 616d 703b 756e 6974 733d 6162 6272  l&amp;units=abbr
-00000480: 6576 6961 7469 6f6e 2661 6d70 3b6c 6566  eviation&amp;lef
-00000490: 745f 636f 6c6f 723d 6772 6579 2661 6d70  t_color=grey&amp
-000004a0: 3b72 6967 6874 5f63 6f6c 6f72 3d62 6c75  ;right_color=blu
-000004b0: 6526 616d 703b 6c65 6674 5f74 6578 743d  e&amp;left_text=
-000004c0: 5079 5069 2532 3064 6f77 6e6c 6f61 6473  PyPi%20downloads
-000004d0: 2220 7372 633d 2268 7474 7073 3a2f 2f73  " src="https://s
-000004e0: 7461 7469 632e 7065 7079 2e74 6563 682f  tatic.pepy.tech/
-000004f0: 7065 7273 6f6e 616c 697a 6564 2d62 6164  personalized-bad
-00000500: 6765 2f6c 6966 746f 6e3f 7065 7269 6f64  ge/lifton?period
-00000510: 3d74 6f74 616c 2661 6d70 3b75 6e69 7473  =total&amp;units
-00000520: 3d61 6262 7265 7669 6174 696f 6e26 616d  =abbreviation&am
-00000530: 703b 6c65 6674 5f63 6f6c 6f72 3d67 7265  p;left_color=gre
-00000540: 7926 616d 703b 7269 6768 745f 636f 6c6f  y&amp;right_colo
-00000550: 723d 626c 7565 2661 6d70 3b6c 6566 745f  r=blue&amp;left_
-00000560: 7465 7874 3d50 7950 6925 3230 646f 776e  text=PyPi%20down
-00000570: 6c6f 6164 7322 3e3c 2f61 3e0a 3c61 2063  loads"></a>.<a c
-00000580: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
-00000590: 6578 7465 726e 616c 2069 6d61 6765 2d72  external image-r
-000005a0: 6566 6572 656e 6365 2220 6872 6566 3d22  eference" href="
-000005b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000005c0: 6f6d 2f4b 7561 6e68 616f 2d43 6861 6f2f  om/Kuanhao-Chao/
-000005d0: 6c69 6674 6f6e 2f72 656c 6561 7365 7322  lifton/releases"
-000005e0: 3e3c 696d 6720 616c 743d 2268 7474 7073  ><img alt="https
-000005f0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000600: 6f2f 6769 7468 7562 2f64 6f77 6e6c 6f61  o/github/downloa
-00000610: 6473 2f4b 7561 6e68 616f 2d43 6861 6f2f  ds/Kuanhao-Chao/
-00000620: 6c69 6674 6f6e 2f74 6f74 616c 2e73 7667  lifton/total.svg
-00000630: 3f73 7479 6c65 3d73 6f63 6961 6c26 616d  ?style=social&am
-00000640: 703b 6c6f 676f 3d67 6974 6875 6226 616d  p;logo=github&am
-00000650: 703b 6c61 6265 6c3d 446f 776e 6c6f 6164  p;label=Download
-00000660: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
-00000670: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
-00000680: 7468 7562 2f64 6f77 6e6c 6f61 6473 2f4b  thub/downloads/K
-00000690: 7561 6e68 616f 2d43 6861 6f2f 6c69 6674  uanhao-Chao/lift
-000006a0: 6f6e 2f74 6f74 616c 2e73 7667 3f73 7479  on/total.svg?sty
-000006b0: 6c65 3d73 6f63 6961 6c26 616d 703b 6c6f  le=social&amp;lo
-000006c0: 676f 3d67 6974 6875 6226 616d 703b 6c61  go=github&amp;la
-000006d0: 6265 6c3d 446f 776e 6c6f 6164 223e 3c2f  bel=Download"></
-000006e0: 613e 0a3c 6120 636c 6173 733d 2272 6566  a>.<a class="ref
-000006f0: 6572 656e 6365 2065 7874 6572 6e61 6c20  erence external 
-00000700: 696d 6167 652d 7265 6665 7265 6e63 6522  image-reference"
-00000710: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-00000720: 6974 6875 622e 636f 6d2f 4b75 616e 6861  ithub.com/Kuanha
-00000730: 6f2d 4368 616f 2f6c 6966 746f 6e2f 7265  o-Chao/lifton/re
-00000740: 6c65 6173 6573 223e 3c69 6d67 2061 6c74  leases"><img alt
-00000750: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00000760: 6965 6c64 732e 696f 2f62 6164 6765 2f70  ields.io/badge/p
-00000770: 6c61 7466 6f72 6d2d 6d61 634f 535f 2f4c  latform-macOS_/L
-00000780: 696e 7578 2d67 7265 656e 2e73 7667 2220  inux-green.svg" 
-00000790: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-000007a0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-000007b0: 652f 706c 6174 666f 726d 2d6d 6163 4f53  e/platform-macOS
-000007c0: 5f2f 4c69 6e75 782d 6772 6565 6e2e 7376  _/Linux-green.sv
-000007d0: 6722 3e3c 2f61 3e0a 3c61 2063 6c61 7373  g"></a>.<a class
-000007e0: 3d22 7265 6665 7265 6e63 6520 6578 7465  ="reference exte
-000007f0: 726e 616c 2069 6d61 6765 2d72 6566 6572  rnal image-refer
-00000800: 656e 6365 2220 6872 6566 3d22 6874 7470  ence" href="http
-00000810: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
-00000820: 6368 2e67 6f6f 676c 652e 636f 6d2f 6769  ch.google.com/gi
-00000830: 7468 7562 2f4b 7561 6e68 616f 2d43 6861  thub/Kuanhao-Cha
-00000840: 6f2f 6c69 6674 6f6e 2f62 6c6f 622f 6d61  o/lifton/blob/ma
-00000850: 696e 2f6e 6f74 6562 6f6f 6b2f 6c69 6674  in/notebook/lift
-00000860: 6f6e 5f65 7861 6d70 6c65 2e69 7079 6e62  on_example.ipynb
-00000870: 223e 3c69 6d67 2061 6c74 3d22 6874 7470  "><img alt="http
-00000880: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
-00000890: 6368 2e67 6f6f 676c 652e 636f 6d2f 6173  ch.google.com/as
-000008a0: 7365 7473 2f63 6f6c 6162 2d62 6164 6765  sets/colab-badge
-000008b0: 2e73 7667 2220 7372 633d 2268 7474 7073  .svg" src="https
-000008c0: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
-000008d0: 682e 676f 6f67 6c65 2e63 6f6d 2f61 7373  h.google.com/ass
-000008e0: 6574 732f 636f 6c61 622d 6261 6467 652e  ets/colab-badge.
-000008f0: 7376 6722 3e3c 2f61 3e0a 3c64 6976 2063  svg"></a>.<div c
-00000900: 6c61 7373 3d22 6c69 6e65 2d62 6c6f 636b  lass="line-block
-00000910: 223e 0a3c 6469 7620 636c 6173 733d 226c  ">.<div class="l
-00000920: 696e 6522 3e3c 6272 3e3c 2f64 6976 3e0a  ine"><br></div>.
-00000930: 3c2f 6469 763e 0a3c 703e 4c69 6674 4f6e  </div>.<p>LiftOn
-00000940: 2069 7320 6120 686f 6d6f 6c6f 6779 2d62   is a homology-b
-00000950: 6173 6564 206c 6966 742d 6f76 6572 2074  ased lift-over t
-00000960: 6f6f 6c20 6465 7369 676e 6564 2074 6f20  ool designed to 
-00000970: 6163 6375 7261 7465 6c79 206d 6170 2061  accurately map a
-00000980: 6e6e 6f74 6174 696f 6e73 2069 6e20 4746  nnotations in GF
-00000990: 4620 6f72 2047 5446 2062 6574 7765 656e  F or GTF between
-000009a0: 2061 7373 656d 626c 6965 732e 2049 7420   assemblies. It 
-000009b0: 6973 2062 7569 6c74 2075 706f 6e20 7468  is built upon th
-000009c0: 6520 6661 6e74 6173 7469 6320 3c61 2063  e fantastic <a c
-000009d0: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
-000009e0: 6578 7465 726e 616c 2220 6872 6566 3d22  external" href="
-000009f0: 6874 7470 733a 2f2f 6163 6164 656d 6963  https://academic
-00000a00: 2e6f 7570 2e63 6f6d 2f62 696f 696e 666f  .oup.com/bioinfo
-00000a10: 726d 6174 6963 732f 6172 7469 636c 652f  rmatics/article/
-00000a20: 3337 2f31 322f 3136 3339 2f36 3033 3531  37/12/1639/60351
-00000a30: 3238 3f6c 6f67 696e 3d74 7275 6522 3e4c  28?login=true">L
-00000a40: 6966 746f 6666 3c2f 613e 2028 6372 6564  iftoff</a> (cred
-00000a50: 6974 7320 746f 203c 6120 636c 6173 733d  its to <a class=
-00000a60: 2272 6566 6572 656e 6365 2065 7874 6572  "reference exter
-00000a70: 6e61 6c22 2068 7265 663d 2268 7474 7073  nal" href="https
-00000a80: 3a2f 2f73 6368 6f6c 6172 2e67 6f6f 676c  ://scholar.googl
-00000a90: 652e 636f 6d2f 6369 7461 7469 6f6e 733f  e.com/citations?
-00000aa0: 7573 6572 3d4e 3374 586b 3751 4141 4141  user=N3tXk7QAAAA
-00000ab0: 4a26 616d 703b 686c 3d65 6e22 3e44 722e  J&amp;hl=en">Dr.
-00000ac0: 2041 6c61 696e 6120 5368 756d 6174 653c   Alaina Shumate<
-00000ad0: 2f61 3e29 2061 6e64 203c 6120 636c 6173  /a>) and <a clas
-00000ae0: 733d 2272 6566 6572 656e 6365 2065 7874  s="reference ext
-00000af0: 6572 6e61 6c22 2068 7265 663d 2268 7474  ernal" href="htt
-00000b00: 7073 3a2f 2f61 6361 6465 6d69 632e 6f75  ps://academic.ou
-00000b10: 702e 636f 6d2f 6269 6f69 6e66 6f72 6d61  p.com/bioinforma
-00000b20: 7469 6373 2f61 7274 6963 6c65 2f33 392f  tics/article/39/
-00000b30: 312f 6274 6164 3031 342f 3639 3839 3632  1/btad014/698962
-00000b40: 3122 3e6d 696e 6970 726f 743c 2f61 3e20  1">miniprot</a> 
-00000b50: 2863 7265 6469 7473 2074 6f20 3c61 2063  (credits to <a c
-00000b60: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
-00000b70: 6578 7465 726e 616c 2220 6872 6566 3d22  external" href="
-00000b80: 6874 7470 3a2f 2f6c 6968 656e 672e 6f72  http://liheng.or
-00000b90: 6722 3e44 722e 2048 656e 6720 4c69 3c2f  g">Dr. Heng Li</
-00000ba0: 613e 292c 2061 6e64 2065 6d70 6c6f 7973  a>), and employs
-00000bb0: 2061 203c 6120 636c 6173 733d 2272 6566   a <a class="ref
-00000bc0: 6572 656e 6365 2069 6e74 6572 6e61 6c22  erence internal"
-00000bd0: 2068 7265 663d 2268 7474 703a 2f2f 6363   href="http://cc
-00000be0: 622e 6a68 752e 6564 752f 6c69 6674 6f6e  b.jhu.edu/lifton
-00000bf0: 2f63 6f6e 7465 6e74 2f62 6568 696e 645f  /content/behind_
-00000c00: 7363 656e 6573 2e68 746d 6c23 7072 6f74  scenes.html#prot
-00000c10: 6569 6e2d 6d61 7869 6d69 7a61 7469 6f6e  ein-maximization
-00000c20: 2d61 6c67 6f72 6974 686d 223e 3c73 7061  -algorithm"><spa
-00000c30: 6e20 636c 6173 733d 2273 7464 2073 7464  n class="std std
-00000c40: 2d72 6566 223e 5072 6f74 6569 6e2d 6d61  -ref">Protein-ma
-00000c50: 7869 6d69 7a61 7469 6f6e 2061 6c67 6f72  ximization algor
-00000c60: 6974 686d 3c2f 7370 616e 3e3c 2f61 3e20  ithm</span></a> 
-00000c70: 746f 2069 6d70 726f 7665 2074 6865 2070  to improve the p
-00000c80: 726f 7465 696e 2d63 6f64 696e 6720 6765  rotein-coding ge
-00000c90: 6e65 206c 6966 742d 6f76 6572 2070 726f  ne lift-over pro
-00000ca0: 6365 7373 2e3c 2f70 3e0a 3c73 6563 7469  cess.</p>.<secti
-00000cb0: 6f6e 2069 643d 2277 6879 2d6c 6966 746f  on id="why-lifto
-00000cc0: 6e22 2063 6c61 7373 3d22 223e 0a3c 6832  n" class="">.<h2
-00000cd0: 3e57 6879 204c 6966 744f 6ee2 9d93 3c61  >Why LiftOn...<a
-00000ce0: 2063 6c61 7373 3d22 6865 6164 6572 6c69   class="headerli
-00000cf0: 6e6b 2220 6872 6566 3d22 2377 6879 2d6c  nk" href="#why-l
-00000d00: 6966 746f 6e22 2074 6974 6c65 3d22 5065  ifton" title="Pe
-00000d10: 726d 616c 696e 6b20 746f 2074 6869 7320  rmalink to this 
-00000d20: 6865 6164 696e 6722 3e23 3c2f 613e 3c2f  heading">#</a></
-00000d30: 6832 3e0a 3c6f 6c20 636c 6173 733d 2261  h2>.<ol class="a
-00000d40: 7261 6269 6320 7369 6d70 6c65 223e 0a3c  rabic simple">.<
-00000d50: 6c69 3e3c 703e 3c73 7472 6f6e 673e 4275  li><p><strong>Bu
-00000d60: 7267 656f 6e69 6e67 206e 756d 6265 7220  rgeoning number 
-00000d70: 6f66 2067 656e 6f6d 6520 6173 7365 6d62  of genome assemb
-00000d80: 6c69 6573 3c2f 7374 726f 6e67 3e3a 2041  lies</strong>: A
-00000d90: 7320 6f66 2044 6563 656d 6265 7220 3230  s of December 20
-00000da0: 3233 2c20 616d 6f6e 6720 7468 6520 3135  23, among the 15
-00000db0: 2c35 3738 2064 6973 7469 6e63 7420 6575  ,578 distinct eu
-00000dc0: 6b61 7279 6f74 6963 2067 656e 6f6d 6573  karyotic genomes
-00000dd0: 2c20 6f6e 6c79 2031 2c31 3131 2068 6176  , only 1,111 hav
-00000de0: 6520 6265 656e 2061 6e6e 6f74 6174 6564  e been annotated
-00000df0: 2028 3c61 2063 6c61 7373 3d22 7265 6665   (<a class="refe
-00000e00: 7265 6e63 6520 6578 7465 726e 616c 2220  rence external" 
-00000e10: 6872 6566 3d22 6874 7470 733a 2f2f 7777  href="https://ww
-00000e20: 772e 6e63 6269 2e6e 6c6d 2e6e 6968 2e67  w.ncbi.nlm.nih.g
-00000e30: 6f76 2f67 656e 6f6d 652f 616e 6e6f 7461  ov/genome/annota
-00000e40: 7469 6f6e 5f65 756b 2f23 6772 6170 6873  tion_euk/#graphs
-00000e50: 223e 4575 6b61 7279 6f74 6963 2047 656e  ">Eukaryotic Gen
-00000e60: 6f6d 6520 416e 6e6f 7461 7469 6f6e 2061  ome Annotation a
-00000e70: 7420 4e43 4249 3c2f 613e 292e 204d 6f72  t NCBI</a>). Mor
-00000e80: 6520 616e 6420 6d6f 7265 2068 6967 6820  e and more high 
-00000e90: 7175 616c 6974 7920 6173 7365 6d62 6c69  quality assembli
-00000ea0: 6573 2061 7265 2067 656e 6572 6174 6564  es are generated
-00000eb0: 2e20 5765 206e 6565 6420 746f 2061 6363  . We need to acc
-00000ec0: 7572 6174 656c 7920 616e 6e6f 7461 7465  urately annotate
-00000ed0: 2074 6865 6d2e 3c2f 703e 3c2f 6c69 3e0a   them.</p></li>.
-00000ee0: 3c6c 693e 3c70 3e3c 7374 726f 6e67 3e49  <li><p><strong>I
-00000ef0: 6d70 726f 7665 6420 7072 6f74 6569 6e2d  mproved protein-
-00000f00: 636f 6469 6e67 2067 656e 6520 6d61 7070  coding gene mapp
-00000f10: 696e 673c 2f73 7472 6f6e 673e 3a20 5468  ing</strong>: Th
-00000f20: 6520 706f 7075 6c61 7220 3c61 2063 6c61  e popular <a cla
-00000f30: 7373 3d22 7265 6665 7265 6e63 6520 6578  ss="reference ex
-00000f40: 7465 726e 616c 2220 6872 6566 3d22 6874  ternal" href="ht
-00000f50: 7470 733a 2f2f 6163 6164 656d 6963 2e6f  tps://academic.o
-00000f60: 7570 2e63 6f6d 2f62 696f 696e 666f 726d  up.com/bioinform
-00000f70: 6174 6963 732f 6172 7469 636c 652f 3337  atics/article/37
-00000f80: 2f31 322f 3136 3339 2f36 3033 3531 3238  /12/1639/6035128
-00000f90: 3f6c 6f67 696e 3d74 7275 6522 3e4c 6966  ?login=true">Lif
-00000fa0: 746f 6666 3c2f 613e 206d 6170 2067 656e  toff</a> map gen
-00000fb0: 6573 206f 6e6c 7920 6261 7365 6420 6f6e  es only based on
-00000fc0: 2074 6865 2044 4e41 2061 6c69 676e 6d65   the DNA alignme
-00000fd0: 6e74 2e20 5769 7468 2074 6865 2070 726f  nt. With the pro
-00000fe0: 7465 696e 2d74 6f2d 6765 6e6f 6d65 2061  tein-to-genome a
-00000ff0: 6c69 676e 6d65 6e74 2c20 4c69 6674 4f6e  lignment, LiftOn
-00001000: 2069 7320 6162 6c65 2074 6f20 6675 7274   is able to furt
-00001010: 6865 7220 696d 7072 6f76 6520 7468 6520  her improve the 
-00001020: 6c69 6674 2d6f 7665 7220 7072 6f74 6569  lift-over protei
-00001030: 6e2d 636f 6469 6e67 2067 656e 6520 616e  n-coding gene an
-00001040: 6e6f 7461 7469 6f6e 732e 204c 6966 744f  notations. LiftO
-00001050: 6e20 696d 7072 6f76 6573 2074 6865 2063  n improves the c
-00001060: 7572 7265 6e74 2072 656c 6561 7365 6420  urrent released 
-00001070: 5432 542d 4348 4d31 3320 616e 6e6f 7461  T2T-CHM13 annota
-00001080: 7469 6f6e 2028 3c61 2063 6c61 7373 3d22  tion (<a class="
-00001090: 7265 6665 7265 6e63 6520 6578 7465 726e  reference extern
-000010a0: 616c 2220 6872 6566 3d22 6874 7470 733a  al" href="https:
-000010b0: 2f2f 7333 2d75 732d 7765 7374 2d32 2e61  //s3-us-west-2.a
-000010c0: 6d61 7a6f 6e61 7773 2e63 6f6d 2f68 756d  mazonaws.com/hum
-000010d0: 616e 2d70 616e 6765 6e6f 6d69 6373 2f54  an-pangenomics/T
-000010e0: 3254 2f43 484d 3133 2f61 7373 656d 626c  2T/CHM13/assembl
-000010f0: 6965 732f 616e 6e6f 7461 7469 6f6e 2f63  ies/annotation/c
-00001100: 686d 3133 7632 2e30 5f52 6566 5365 715f  hm13v2.0_RefSeq_
-00001110: 4c69 6674 6f66 665f 7635 2e31 2e67 6666  Liftoff_v5.1.gff
-00001120: 332e 677a 223e 4a48 5520 5265 6653 6571  3.gz">JHU RefSeq
-00001130: 7631 3130 202b 204c 6966 746f 6666 2076  v110 + Liftoff v
-00001140: 352e 313c 2f61 3e29 2e3c 2f70 3e3c 2f6c  5.1</a>).</p></l
-00001150: 693e 0a3c 6c69 3e3c 703e 3c73 7472 6f6e  i>.<li><p><stron
-00001160: 673e 496d 7072 6f76 6564 2064 6973 7461  g>Improved dista
-00001170: 6e74 2073 7065 6369 6573 206c 6966 742d  nt species lift-
-00001180: 6f76 6572 3c2f 7374 726f 6e67 3e3a 204c  over</strong>: L
-00001190: 6966 744f 6e20 6578 7465 6e64 7320 6672  iftOn extends fr
-000011a0: 6f6d 206c 6966 742d 6f76 6572 2062 6574  om lift-over bet
-000011b0: 7765 656e 2074 6865 2073 616d 6520 6f72  ween the same or
-000011c0: 2063 6c6f 7365 6c79 2072 656c 6174 6564   closely related
-000011d0: 2073 7065 6369 6573 2074 6f20 6d6f 7265   species to more
-000011e0: 2064 6973 7461 6e74 6c79 2072 656c 6174   distantly relat
-000011f0: 6564 2073 7065 6369 6573 2e20 5365 6520  ed species. See 
-00001200: 3c73 7061 6e20 636c 6173 733d 2278 7265  <span class="xre
-00001210: 6620 7374 6420 7374 642d 7265 6622 3e6d  f std std-ref">m
-00001220: 6f75 7365 5f32 5f72 6174 3c2f 7370 616e  ouse_2_rat</span
-00001230: 3e20 616e 6420 3c73 7061 6e20 636c 6173  > and <span clas
-00001240: 733d 2278 7265 6620 7374 6420 7374 642d  s="xref std std-
-00001250: 7265 6622 3e64 726f 736f 7068 696c 615f  ref">drosophila_
-00001260: 6d65 6c61 6e6f 6761 7374 6572 5f32 5f65  melanogaster_2_e
-00001270: 7265 6374 613c 2f73 7061 6e3e 206c 6966  recta</span> lif
-00001280: 742d 6f76 6572 2073 6563 7469 6f6e 732e  t-over sections.
-00001290: 3c2f 703e 3c2f 6c69 3e0a 3c2f 6f6c 3e0a  </p></li>.</ol>.
-000012a0: 3c70 3e4c 6966 744f 6e20 6973 2066 7265  <p>LiftOn is fre
-000012b0: 652c 2069 7427 7320 6f70 656e 2073 6f75  e, it's open sou
-000012c0: 7263 652c 2069 7427 7320 6561 7379 2074  rce, it's easy t
-000012d0: 6f20 696e 7374 616c 6c20 2c20 616e 6420  o install , and 
-000012e0: 6974 2773 2069 6e20 5079 7468 6f6e 213c  it's in Python!<
-000012f0: 2f70 3e0a 3c64 6976 2063 6c61 7373 3d22  /p>.<div class="
-00001300: 6c69 6e65 2d62 6c6f 636b 223e 0a3c 6469  line-block">.<di
-00001310: 7620 636c 6173 733d 226c 696e 6522 3e3c  v class="line"><
-00001320: 6272 3e3c 2f64 6976 3e0a 3c2f 6469 763e  br></div>.</div>
-00001330: 0a3c 2f73 6563 7469 6f6e 3e0a 3c73 6563  .</section>.<sec
-00001340: 7469 6f6e 2069 643d 2277 686f 2d69 732d  tion id="who-is-
-00001350: 6974 2d66 6f72 2220 636c 6173 733d 2222  it-for" class=""
-00001360: 3e0a 3c68 323e 5768 6f20 6973 2069 7420  >.<h2>Who is it 
-00001370: 666f 72e2 9d93 3c61 2063 6c61 7373 3d22  for...<a class="
-00001380: 6865 6164 6572 6c69 6e6b 2220 6872 6566  headerlink" href
-00001390: 3d22 2377 686f 2d69 732d 6974 2d66 6f72  ="#who-is-it-for
-000013a0: 2220 7469 746c 653d 2250 6572 6d61 6c69  " title="Permali
-000013b0: 6e6b 2074 6f20 7468 6973 2068 6561 6469  nk to this headi
-000013c0: 6e67 223e 233c 2f61 3e3c 2f68 323e 0a3c  ng">#</a></h2>.<
-000013d0: 6f6c 2063 6c61 7373 3d22 6172 6162 6963  ol class="arabic
-000013e0: 2073 696d 706c 6522 3e0a 3c6c 693e 3c70   simple">.<li><p
-000013f0: 3e49 6620 796f 7520 6861 7665 2073 6571  >If you have seq
-00001400: 7565 6e63 6564 2061 6e64 2061 7373 656d  uenced and assem
-00001410: 626c 6564 2061 206e 6577 2067 656e 6f6d  bled a new genom
-00001420: 6520 616e 6420 6e65 6564 2074 6f20 616e  e and need to an
-00001430: 6e6f 7461 7465 2069 742c 204c 6966 744f  notate it, LiftO
-00001440: 6e20 6973 2074 6865 2069 6465 616c 2063  n is the ideal c
-00001450: 686f 6963 6520 666f 7220 6765 6e65 7261  hoice for genera
-00001460: 7469 6e67 2061 6e6e 6f74 6174 696f 6e73  ting annotations
-00001470: 2e3c 2f70 3e3c 2f6c 693e 0a3c 6c69 3e3c  .</p></li>.<li><
-00001480: 703e 4966 2079 6f75 2077 616e 7420 746f  p>If you want to
-00001490: 2064 6f20 636f 6d70 6172 6174 6976 6520   do comparative 
-000014a0: 6765 6e6f 6d69 6373 2061 6e61 6c79 7369  genomics analysi
-000014b0: 732c 2072 756e 206c 6966 744f 6e20 746f  s, run liftOn to
-000014c0: 206c 6966 742d 6f76 6572 2061 6e64 2063   lift-over and c
-000014d0: 6f6d 7061 7265 2061 6e6e 6f74 6174 696f  ompare annotatio
-000014e0: 6e73 213c 2f70 3e3c 2f6c 693e 0a3c 6c69  ns!</p></li>.<li
-000014f0: 3e3c 703e 4966 2079 6f75 2077 6973 6820  ><p>If you wish 
-00001500: 746f 2075 7469 6c69 7a65 2074 6865 2066  to utilize the f
-00001510: 696e 6573 7420 4348 4d31 3320 616e 6e6f  inest CHM13 anno
-00001520: 7461 7469 6f6e 2c20 796f 7520 6361 6e20  tation, you can 
-00001530: 7275 6e20 4c69 6674 4f6e 2120 5765 2068  run LiftOn! We h
-00001540: 6176 6520 616c 736f 2070 7265 2d67 656e  ave also pre-gen
-00001550: 6572 6174 6564 2074 6865 203c 6120 636c  erated the <a cl
-00001560: 6173 733d 2272 6566 6572 656e 6365 2065  ass="reference e
-00001570: 7874 6572 6e61 6c22 2068 7265 663d 2268  xternal" href="h
-00001580: 7474 7073 3a2f 2f6b 6863 6861 6f2e 636f  ttps://khchao.co
-00001590: 6d22 3e54 3254 5f43 484d 3133 5f4c 6966  m">T2T_CHM13_Lif
-000015a0: 744f 6e2e 6766 6633 3c2f 613e 2066 696c  tOn.gff3</a> fil
-000015b0: 6520 666f 7220 796f 7572 2063 6f6e 7665  e for your conve
-000015c0: 6e69 656e 6365 2e3c 2f70 3e3c 2f6c 693e  nience.</p></li>
-000015d0: 0a3c 2f6f 6c3e 0a3c 6469 7620 636c 6173  .</ol>.<div clas
-000015e0: 733d 226c 696e 652d 626c 6f63 6b22 3e0a  s="line-block">.
-000015f0: 3c64 6976 2063 6c61 7373 3d22 6c69 6e65  <div class="line
-00001600: 223e 3c62 723e 3c2f 6469 763e 0a3c 2f64  "><br></div>.</d
-00001610: 6976 3e0a 3c2f 7365 6374 696f 6e3e 0a3c  iv>.</section>.<
-00001620: 7365 6374 696f 6e20 6964 3d22 7768 6174  section id="what
-00001630: 2d64 6f65 732d 6c69 6674 6f6e 2d64 6f22  -does-lifton-do"
-00001640: 2063 6c61 7373 3d22 223e 0a3c 6832 3e57   class="">.<h2>W
-00001650: 6861 7420 646f 6573 204c 6966 744f 6e20  hat does LiftOn 
-00001660: 646f e29d 933c 6120 636c 6173 733d 2268  do...<a class="h
-00001670: 6561 6465 726c 696e 6b22 2068 7265 663d  eaderlink" href=
-00001680: 2223 7768 6174 2d64 6f65 732d 6c69 6674  "#what-does-lift
-00001690: 6f6e 2d64 6f22 2074 6974 6c65 3d22 5065  on-do" title="Pe
-000016a0: 726d 616c 696e 6b20 746f 2074 6869 7320  rmalink to this 
-000016b0: 6865 6164 696e 6722 3e23 3c2f 613e 3c2f  heading">#</a></
-000016c0: 6832 3e0a 3c70 3e47 6976 656e 2061 2072  h2>.<p>Given a r
-000016d0: 6566 6572 656e 6365 203c 7374 726f 6e67  eference <strong
-000016e0: 3e47 656e 6f6d 653c 2f73 7472 6f6e 673e  >Genome</strong>
-000016f0: 203c 7370 616e 2063 6c61 7373 3d22 6d61   <span class="ma
-00001700: 7468 206e 6f74 7261 6e73 6c61 7465 206e  th notranslate n
-00001710: 6f68 6967 686c 6967 6874 223e 3c6d 6a78  ohighlight"><mjx
-00001720: 2d63 6f6e 7461 696e 6572 2063 6c61 7373  -container class
-00001730: 3d22 4d61 7468 4a61 7820 4374 7874 4d65  ="MathJax CtxtMe
-00001740: 6e75 5f41 7474 6163 6865 645f 3022 206a  nu_Attached_0" j
-00001750: 6178 3d22 4348 544d 4c22 2074 6162 696e  ax="CHTML" tabin
-00001760: 6465 783d 2230 2220 6374 7874 6d65 6e75  dex="0" ctxtmenu
-00001770: 5f63 6f75 6e74 6572 3d22 3022 2073 7479  _counter="0" sty
-00001780: 6c65 3d22 666f 6e74 2d73 697a 653a 2031  le="font-size: 1
-00001790: 3139 253b 2070 6f73 6974 696f 6e3a 2072  19%; position: r
-000017a0: 656c 6174 6976 653b 223e 3c6d 6a78 2d6d  elative;"><mjx-m
-000017b0: 6174 6820 636c 6173 733d 224d 4a58 2d54  ath class="MJX-T
-000017c0: 4558 2220 6172 6961 2d68 6964 6465 6e3d  EX" aria-hidden=
-000017d0: 2274 7275 6522 3e3c 6d6a 782d 6d69 2063  "true"><mjx-mi c
-000017e0: 6c61 7373 3d22 6d6a 782d 6922 3e3c 6d6a  lass="mjx-i"><mj
-000017f0: 782d 6320 636c 6173 733d 226d 6a78 2d63  x-c class="mjx-c
-00001800: 3144 3434 3520 5445 582d 4922 3e3c 2f6d  1D445 TEX-I"></m
-00001810: 6a78 2d63 3e3c 2f6d 6a78 2d6d 693e 3c2f  jx-c></mjx-mi></
-00001820: 6d6a 782d 6d61 7468 3e3c 6d6a 782d 6173  mjx-math><mjx-as
-00001830: 7369 7374 6976 652d 6d6d 6c20 756e 7365  sistive-mml unse
-00001840: 6c65 6374 6162 6c65 3d22 6f6e 2220 6469  lectable="on" di
-00001850: 7370 6c61 793d 2269 6e6c 696e 6522 3e3c  splay="inline"><
-00001860: 6d61 7468 2078 6d6c 6e73 3d22 6874 7470  math xmlns="http
-00001870: 3a2f 2f77 7777 2e77 332e 6f72 672f 3139  ://www.w3.org/19
-00001880: 3938 2f4d 6174 682f 4d61 7468 4d4c 223e  98/Math/MathML">
-00001890: 3c6d 693e 523c 2f6d 693e 3c2f 6d61 7468  <mi>R</mi></math
-000018a0: 3e3c 2f6d 6a78 2d61 7373 6973 7469 7665  ></mjx-assistive
-000018b0: 2d6d 6d6c 3e3c 2f6d 6a78 2d63 6f6e 7461  -mml></mjx-conta
-000018c0: 696e 6572 3e3c 2f73 7061 6e3e 2c20 616e  iner></span>, an
-000018d0: 203c 7374 726f 6e67 3e41 6e6e 6f74 6174   <strong>Annotat
-000018e0: 696f 6e3c 2f73 7472 6f6e 673e 203c 7370  ion</strong> <sp
-000018f0: 616e 2063 6c61 7373 3d22 6d61 7468 206e  an class="math n
-00001900: 6f74 7261 6e73 6c61 7465 206e 6f68 6967  otranslate nohig
-00001910: 686c 6967 6874 223e 3c6d 6a78 2d63 6f6e  hlight"><mjx-con
-00001920: 7461 696e 6572 2063 6c61 7373 3d22 4d61  tainer class="Ma
-00001930: 7468 4a61 7820 4374 7874 4d65 6e75 5f41  thJax CtxtMenu_A
-00001940: 7474 6163 6865 645f 3022 206a 6178 3d22  ttached_0" jax="
-00001950: 4348 544d 4c22 2074 6162 696e 6465 783d  CHTML" tabindex=
-00001960: 2230 2220 6374 7874 6d65 6e75 5f63 6f75  "0" ctxtmenu_cou
-00001970: 6e74 6572 3d22 3122 2073 7479 6c65 3d22  nter="1" style="
-00001980: 666f 6e74 2d73 697a 653a 2031 3139 253b  font-size: 119%;
-00001990: 2070 6f73 6974 696f 6e3a 2072 656c 6174   position: relat
-000019a0: 6976 653b 223e 3c6d 6a78 2d6d 6174 6820  ive;"><mjx-math 
-000019b0: 636c 6173 733d 224d 4a58 2d54 4558 2220  class="MJX-TEX" 
-000019c0: 6172 6961 2d68 6964 6465 6e3d 2274 7275  aria-hidden="tru
-000019d0: 6522 3e3c 6d6a 782d 6d73 7562 3e3c 6d6a  e"><mjx-msub><mj
-000019e0: 782d 6d69 2063 6c61 7373 3d22 6d6a 782d  x-mi class="mjx-
-000019f0: 6922 3e3c 6d6a 782d 6320 636c 6173 733d  i"><mjx-c class=
-00001a00: 226d 6a78 2d63 3144 3434 3520 5445 582d  "mjx-c1D445 TEX-
-00001a10: 4922 3e3c 2f6d 6a78 2d63 3e3c 2f6d 6a78  I"></mjx-c></mjx
-00001a20: 2d6d 693e 3c6d 6a78 2d73 6372 6970 7420  -mi><mjx-script 
-00001a30: 7374 796c 653d 2276 6572 7469 6361 6c2d  style="vertical-
-00001a40: 616c 6967 6e3a 202d 302e 3135 3365 6d3b  align: -0.153em;
-00001a50: 223e 3c6d 6a78 2d6d 6920 636c 6173 733d  "><mjx-mi class=
-00001a60: 226d 6a78 2d69 2220 7369 7a65 3d22 7322  "mjx-i" size="s"
-00001a70: 3e3c 6d6a 782d 6320 636c 6173 733d 226d  ><mjx-c class="m
-00001a80: 6a78 2d63 3144 3433 3420 5445 582d 4922  jx-c1D434 TEX-I"
-00001a90: 3e3c 2f6d 6a78 2d63 3e3c 2f6d 6a78 2d6d  ></mjx-c></mjx-m
-00001aa0: 693e 3c2f 6d6a 782d 7363 7269 7074 3e3c  i></mjx-script><
-00001ab0: 2f6d 6a78 2d6d 7375 623e 3c2f 6d6a 782d  /mjx-msub></mjx-
-00001ac0: 6d61 7468 3e3c 6d6a 782d 6173 7369 7374  math><mjx-assist
-00001ad0: 6976 652d 6d6d 6c20 756e 7365 6c65 6374  ive-mml unselect
-00001ae0: 6162 6c65 3d22 6f6e 2220 6469 7370 6c61  able="on" displa
-00001af0: 793d 2269 6e6c 696e 6522 3e3c 6d61 7468  y="inline"><math
-00001b00: 2078 6d6c 6e73 3d22 6874 7470 3a2f 2f77   xmlns="http://w
-00001b10: 7777 2e77 332e 6f72 672f 3139 3938 2f4d  ww.w3.org/1998/M
-00001b20: 6174 682f 4d61 7468 4d4c 223e 3c6d 7375  ath/MathML"><msu
-00001b30: 623e 3c6d 693e 523c 2f6d 693e 3c6d 693e  b><mi>R</mi><mi>
-00001b40: 413c 2f6d 693e 3c2f 6d73 7562 3e3c 2f6d  A</mi></msub></m
-00001b50: 6174 683e 3c2f 6d6a 782d 6173 7369 7374  ath></mjx-assist
-00001b60: 6976 652d 6d6d 6c3e 3c2f 6d6a 782d 636f  ive-mml></mjx-co
-00001b70: 6e74 6169 6e65 723e 3c2f 7370 616e 3e2c  ntainer></span>,
-00001b80: 2061 6e64 2061 2074 6172 6765 7420 3c73   and a target <s
-00001b90: 7472 6f6e 673e 4765 6e6f 6d65 3c2f 7374  trong>Genome</st
-00001ba0: 726f 6e67 3e20 3c73 7061 6e20 636c 6173  rong> <span clas
-00001bb0: 733d 226d 6174 6820 6e6f 7472 616e 736c  s="math notransl
-00001bc0: 6174 6520 6e6f 6869 6768 6c69 6768 7422  ate nohighlight"
-00001bd0: 3e3c 6d6a 782d 636f 6e74 6169 6e65 7220  ><mjx-container 
-00001be0: 636c 6173 733d 224d 6174 684a 6178 2043  class="MathJax C
-00001bf0: 7478 744d 656e 755f 4174 7461 6368 6564  txtMenu_Attached
-00001c00: 5f30 2220 6a61 783d 2243 4854 4d4c 2220  _0" jax="CHTML" 
-00001c10: 7461 6269 6e64 6578 3d22 3022 2063 7478  tabindex="0" ctx
-00001c20: 746d 656e 755f 636f 756e 7465 723d 2232  tmenu_counter="2
-00001c30: 2220 7374 796c 653d 2266 6f6e 742d 7369  " style="font-si
-00001c40: 7a65 3a20 3131 3925 3b20 706f 7369 7469  ze: 119%; positi
-00001c50: 6f6e 3a20 7265 6c61 7469 7665 3b22 3e3c  on: relative;"><
-00001c60: 6d6a 782d 6d61 7468 2063 6c61 7373 3d22  mjx-math class="
-00001c70: 4d4a 582d 5445 5822 2061 7269 612d 6869  MJX-TEX" aria-hi
-00001c80: 6464 656e 3d22 7472 7565 223e 3c6d 6a78  dden="true"><mjx
-00001c90: 2d6d 6920 636c 6173 733d 226d 6a78 2d69  -mi class="mjx-i
-00001ca0: 223e 3c6d 6a78 2d63 2063 6c61 7373 3d22  "><mjx-c class="
-00001cb0: 6d6a 782d 6331 4434 3437 2054 4558 2d49  mjx-c1D447 TEX-I
-00001cc0: 223e 3c2f 6d6a 782d 633e 3c2f 6d6a 782d  "></mjx-c></mjx-
-00001cd0: 6d69 3e3c 2f6d 6a78 2d6d 6174 683e 3c6d  mi></mjx-math><m
-00001ce0: 6a78 2d61 7373 6973 7469 7665 2d6d 6d6c  jx-assistive-mml
-00001cf0: 2075 6e73 656c 6563 7461 626c 653d 226f   unselectable="o
-00001d00: 6e22 2064 6973 706c 6179 3d22 696e 6c69  n" display="inli
-00001d10: 6e65 223e 3c6d 6174 6820 786d 6c6e 733d  ne"><math xmlns=
-00001d20: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
-00001d30: 7267 2f31 3939 382f 4d61 7468 2f4d 6174  rg/1998/Math/Mat
-00001d40: 684d 4c22 3e3c 6d69 3e54 3c2f 6d69 3e3c  hML"><mi>T</mi><
-00001d50: 2f6d 6174 683e 3c2f 6d6a 782d 6173 7369  /math></mjx-assi
-00001d60: 7374 6976 652d 6d6d 6c3e 3c2f 6d6a 782d  stive-mml></mjx-
-00001d70: 636f 6e74 6169 6e65 723e 3c2f 7370 616e  container></span
-00001d80: 3e2e 2054 6865 206c 6966 742d 6f76 6572  >. The lift-over
-00001d90: 2070 726f 626c 656d 2069 7320 6465 6669   problem is defi
-00001da0: 6e65 6420 6173 2074 6865 2070 726f 6365  ned as the proce
-00001db0: 7373 206f 6620 6368 616e 6769 6e67 2074  ss of changing t
-00001dc0: 6865 2063 6f6f 7264 696e 6174 6573 206f  he coordinates o
-00001dd0: 6620 3c73 7472 6f6e 673e 416e 6e6f 7461  f <strong>Annota
-00001de0: 7469 6f6e 3c2f 7374 726f 6e67 3e20 3c73  tion</strong> <s
-00001df0: 7061 6e20 636c 6173 733d 226d 6174 6820  pan class="math 
-00001e00: 6e6f 7472 616e 736c 6174 6520 6e6f 6869  notranslate nohi
-00001e10: 6768 6c69 6768 7422 3e3c 6d6a 782d 636f  ghlight"><mjx-co
-00001e20: 6e74 6169 6e65 7220 636c 6173 733d 224d  ntainer class="M
-00001e30: 6174 684a 6178 2043 7478 744d 656e 755f  athJax CtxtMenu_
-00001e40: 4174 7461 6368 6564 5f30 2220 6a61 783d  Attached_0" jax=
-00001e50: 2243 4854 4d4c 2220 7461 6269 6e64 6578  "CHTML" tabindex
-00001e60: 3d22 3022 2063 7478 746d 656e 755f 636f  ="0" ctxtmenu_co
-00001e70: 756e 7465 723d 2233 2220 7374 796c 653d  unter="3" style=
-00001e80: 2266 6f6e 742d 7369 7a65 3a20 3131 3925  "font-size: 119%
-00001e90: 3b20 706f 7369 7469 6f6e 3a20 7265 6c61  ; position: rela
-00001ea0: 7469 7665 3b22 3e3c 6d6a 782d 6d61 7468  tive;"><mjx-math
-00001eb0: 2063 6c61 7373 3d22 4d4a 582d 5445 5822   class="MJX-TEX"
-00001ec0: 2061 7269 612d 6869 6464 656e 3d22 7472   aria-hidden="tr
-00001ed0: 7565 223e 3c6d 6a78 2d6d 7375 623e 3c6d  ue"><mjx-msub><m
-00001ee0: 6a78 2d6d 6920 636c 6173 733d 226d 6a78  jx-mi class="mjx
-00001ef0: 2d69 223e 3c6d 6a78 2d63 2063 6c61 7373  -i"><mjx-c class
-00001f00: 3d22 6d6a 782d 6331 4434 3435 2054 4558  ="mjx-c1D445 TEX
-00001f10: 2d49 223e 3c2f 6d6a 782d 633e 3c2f 6d6a  -I"></mjx-c></mj
-00001f20: 782d 6d69 3e3c 6d6a 782d 7363 7269 7074  x-mi><mjx-script
-00001f30: 2073 7479 6c65 3d22 7665 7274 6963 616c   style="vertical
-00001f40: 2d61 6c69 676e 3a20 2d30 2e31 3533 656d  -align: -0.153em
-00001f50: 3b22 3e3c 6d6a 782d 6d69 2063 6c61 7373  ;"><mjx-mi class
-00001f60: 3d22 6d6a 782d 6922 2073 697a 653d 2273  ="mjx-i" size="s
-00001f70: 223e 3c6d 6a78 2d63 2063 6c61 7373 3d22  "><mjx-c class="
-00001f80: 6d6a 782d 6331 4434 3334 2054 4558 2d49  mjx-c1D434 TEX-I
-00001f90: 223e 3c2f 6d6a 782d 633e 3c2f 6d6a 782d  "></mjx-c></mjx-
-00001fa0: 6d69 3e3c 2f6d 6a78 2d73 6372 6970 743e  mi></mjx-script>
-00001fb0: 3c2f 6d6a 782d 6d73 7562 3e3c 2f6d 6a78  </mjx-msub></mjx
-00001fc0: 2d6d 6174 683e 3c6d 6a78 2d61 7373 6973  -math><mjx-assis
-00001fd0: 7469 7665 2d6d 6d6c 2075 6e73 656c 6563  tive-mml unselec
-00001fe0: 7461 626c 653d 226f 6e22 2064 6973 706c  table="on" displ
-00001ff0: 6179 3d22 696e 6c69 6e65 223e 3c6d 6174  ay="inline"><mat
-00002000: 6820 786d 6c6e 733d 2268 7474 703a 2f2f  h xmlns="http://
-00002010: 7777 772e 7733 2e6f 7267 2f31 3939 382f  www.w3.org/1998/
-00002020: 4d61 7468 2f4d 6174 684d 4c22 3e3c 6d73  Math/MathML"><ms
-00002030: 7562 3e3c 6d69 3e52 3c2f 6d69 3e3c 6d69  ub><mi>R</mi><mi
-00002040: 3e41 3c2f 6d69 3e3c 2f6d 7375 623e 3c2f  >A</mi></msub></
-00002050: 6d61 7468 3e3c 2f6d 6a78 2d61 7373 6973  math></mjx-assis
-00002060: 7469 7665 2d6d 6d6c 3e3c 2f6d 6a78 2d63  tive-mml></mjx-c
-00002070: 6f6e 7461 696e 6572 3e3c 2f73 7061 6e3e  ontainer></span>
-00002080: 2066 726f 6d20 3c73 7472 6f6e 673e 4765   from <strong>Ge
-00002090: 6e6f 6d65 3c2f 7374 726f 6e67 3e20 3c73  nome</strong> <s
-000020a0: 7061 6e20 636c 6173 733d 226d 6174 6820  pan class="math 
-000020b0: 6e6f 7472 616e 736c 6174 6520 6e6f 6869  notranslate nohi
-000020c0: 6768 6c69 6768 7422 3e3c 6d6a 782d 636f  ghlight"><mjx-co
-000020d0: 6e74 6169 6e65 7220 636c 6173 733d 224d  ntainer class="M
-000020e0: 6174 684a 6178 2043 7478 744d 656e 755f  athJax CtxtMenu_
-000020f0: 4174 7461 6368 6564 5f30 2220 6a61 783d  Attached_0" jax=
-00002100: 2243 4854 4d4c 2220 7461 6269 6e64 6578  "CHTML" tabindex
-00002110: 3d22 3022 2063 7478 746d 656e 755f 636f  ="0" ctxtmenu_co
-00002120: 756e 7465 723d 2234 2220 7374 796c 653d  unter="4" style=
-00002130: 2266 6f6e 742d 7369 7a65 3a20 3131 3925  "font-size: 119%
-00002140: 3b20 706f 7369 7469 6f6e 3a20 7265 6c61  ; position: rela
-00002150: 7469 7665 3b22 3e3c 6d6a 782d 6d61 7468  tive;"><mjx-math
-00002160: 2063 6c61 7373 3d22 4d4a 582d 5445 5822   class="MJX-TEX"
-00002170: 2061 7269 612d 6869 6464 656e 3d22 7472   aria-hidden="tr
-00002180: 7565 223e 3c6d 6a78 2d6d 6920 636c 6173  ue"><mjx-mi clas
-00002190: 733d 226d 6a78 2d69 223e 3c6d 6a78 2d63  s="mjx-i"><mjx-c
-000021a0: 2063 6c61 7373 3d22 6d6a 782d 6331 4434   class="mjx-c1D4
-000021b0: 3435 2054 4558 2d49 223e 3c2f 6d6a 782d  45 TEX-I"></mjx-
-000021c0: 633e 3c2f 6d6a 782d 6d69 3e3c 2f6d 6a78  c></mjx-mi></mjx
-000021d0: 2d6d 6174 683e 3c6d 6a78 2d61 7373 6973  -math><mjx-assis
-000021e0: 7469 7665 2d6d 6d6c 2075 6e73 656c 6563  tive-mml unselec
-000021f0: 7461 626c 653d 226f 6e22 2064 6973 706c  table="on" displ
-00002200: 6179 3d22 696e 6c69 6e65 223e 3c6d 6174  ay="inline"><mat
-00002210: 6820 786d 6c6e 733d 2268 7474 703a 2f2f  h xmlns="http://
-00002220: 7777 772e 7733 2e6f 7267 2f31 3939 382f  www.w3.org/1998/
-00002230: 4d61 7468 2f4d 6174 684d 4c22 3e3c 6d69  Math/MathML"><mi
-00002240: 3e52 3c2f 6d69 3e3c 2f6d 6174 683e 3c2f  >R</mi></math></
-00002250: 6d6a 782d 6173 7369 7374 6976 652d 6d6d  mjx-assistive-mm
-00002260: 6c3e 3c2f 6d6a 782d 636f 6e74 6169 6e65  l></mjx-containe
-00002270: 723e 3c2f 7370 616e 3e20 746f 203c 7374  r></span> to <st
-00002280: 726f 6e67 3e47 656e 6f6d 653c 2f73 7472  rong>Genome</str
-00002290: 6f6e 673e 203c 7370 616e 2063 6c61 7373  ong> <span class
-000022a0: 3d22 6d61 7468 206e 6f74 7261 6e73 6c61  ="math notransla
-000022b0: 7465 206e 6f68 6967 686c 6967 6874 223e  te nohighlight">
-000022c0: 3c6d 6a78 2d63 6f6e 7461 696e 6572 2063  <mjx-container c
-000022d0: 6c61 7373 3d22 4d61 7468 4a61 7820 4374  lass="MathJax Ct
-000022e0: 7874 4d65 6e75 5f41 7474 6163 6865 645f  xtMenu_Attached_
-000022f0: 3022 206a 6178 3d22 4348 544d 4c22 2074  0" jax="CHTML" t
-00002300: 6162 696e 6465 783d 2230 2220 6374 7874  abindex="0" ctxt
-00002310: 6d65 6e75 5f63 6f75 6e74 6572 3d22 3522  menu_counter="5"
-00002320: 2073 7479 6c65 3d22 666f 6e74 2d73 697a   style="font-siz
-00002330: 653a 2031 3139 253b 2070 6f73 6974 696f  e: 119%; positio
-00002340: 6e3a 2072 656c 6174 6976 653b 223e 3c6d  n: relative;"><m
-00002350: 6a78 2d6d 6174 6820 636c 6173 733d 224d  jx-math class="M
-00002360: 4a58 2d54 4558 2220 6172 6961 2d68 6964  JX-TEX" aria-hid
-00002370: 6465 6e3d 2274 7275 6522 3e3c 6d6a 782d  den="true"><mjx-
-00002380: 6d69 2063 6c61 7373 3d22 6d6a 782d 6922  mi class="mjx-i"
-00002390: 3e3c 6d6a 782d 6320 636c 6173 733d 226d  ><mjx-c class="m
-000023a0: 6a78 2d63 3144 3434 3720 5445 582d 4922  jx-c1D447 TEX-I"
-000023b0: 3e3c 2f6d 6a78 2d63 3e3c 2f6d 6a78 2d6d  ></mjx-c></mjx-m
-000023c0: 693e 3c2f 6d6a 782d 6d61 7468 3e3c 6d6a  i></mjx-math><mj
-000023d0: 782d 6173 7369 7374 6976 652d 6d6d 6c20  x-assistive-mml 
-000023e0: 756e 7365 6c65 6374 6162 6c65 3d22 6f6e  unselectable="on
-000023f0: 2220 6469 7370 6c61 793d 2269 6e6c 696e  " display="inlin
-00002400: 6522 3e3c 6d61 7468 2078 6d6c 6e73 3d22  e"><math xmlns="
-00002410: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
-00002420: 672f 3139 3938 2f4d 6174 682f 4d61 7468  g/1998/Math/Math
-00002430: 4d4c 223e 3c6d 693e 543c 2f6d 693e 3c2f  ML"><mi>T</mi></
-00002440: 6d61 7468 3e3c 2f6d 6a78 2d61 7373 6973  math></mjx-assis
-00002450: 7469 7665 2d6d 6d6c 3e3c 2f6d 6a78 2d63  tive-mml></mjx-c
-00002460: 6f6e 7461 696e 6572 3e3c 2f73 7061 6e3e  ontainer></span>
-00002470: 2c20 616e 6420 6765 6e65 7261 7465 2061  , and generate a
-00002480: 206e 6577 2061 6e6e 6f74 6174 696f 6e20   new annotation 
-00002490: 6669 6c65 203c 7374 726f 6e67 3e41 6e6e  file <strong>Ann
-000024a0: 6f74 6174 696f 6e3c 2f73 7472 6f6e 673e  otation</strong>
-000024b0: 203c 7370 616e 2063 6c61 7373 3d22 6d61   <span class="ma
-000024c0: 7468 206e 6f74 7261 6e73 6c61 7465 206e  th notranslate n
-000024d0: 6f68 6967 686c 6967 6874 223e 3c6d 6a78  ohighlight"><mjx
-000024e0: 2d63 6f6e 7461 696e 6572 2063 6c61 7373  -container class
-000024f0: 3d22 4d61 7468 4a61 7820 4374 7874 4d65  ="MathJax CtxtMe
-00002500: 6e75 5f41 7474 6163 6865 645f 3022 206a  nu_Attached_0" j
-00002510: 6178 3d22 4348 544d 4c22 2074 6162 696e  ax="CHTML" tabin
-00002520: 6465 783d 2230 2220 6374 7874 6d65 6e75  dex="0" ctxtmenu
-00002530: 5f63 6f75 6e74 6572 3d22 3622 2073 7479  _counter="6" sty
-00002540: 6c65 3d22 666f 6e74 2d73 697a 653a 2031  le="font-size: 1
-00002550: 3139 253b 2070 6f73 6974 696f 6e3a 2072  19%; position: r
-00002560: 656c 6174 6976 653b 223e 3c6d 6a78 2d6d  elative;"><mjx-m
-00002570: 6174 6820 636c 6173 733d 224d 4a58 2d54  ath class="MJX-T
-00002580: 4558 2220 6172 6961 2d68 6964 6465 6e3d  EX" aria-hidden=
-00002590: 2274 7275 6522 3e3c 6d6a 782d 6d73 7562  "true"><mjx-msub
-000025a0: 3e3c 6d6a 782d 6d69 2063 6c61 7373 3d22  ><mjx-mi class="
-000025b0: 6d6a 782d 6922 3e3c 6d6a 782d 6320 636c  mjx-i"><mjx-c cl
-000025c0: 6173 733d 226d 6a78 2d63 3144 3434 3720  ass="mjx-c1D447 
-000025d0: 5445 582d 4922 3e3c 2f6d 6a78 2d63 3e3c  TEX-I"></mjx-c><
-000025e0: 2f6d 6a78 2d6d 693e 3c6d 6a78 2d73 6372  /mjx-mi><mjx-scr
-000025f0: 6970 7420 7374 796c 653d 2276 6572 7469  ipt style="verti
-00002600: 6361 6c2d 616c 6967 6e3a 202d 302e 3135  cal-align: -0.15
-00002610: 3365 6d3b 206d 6172 6769 6e2d 6c65 6674  3em; margin-left
-00002620: 3a20 2d30 2e31 3265 6d3b 223e 3c6d 6a78  : -0.12em;"><mjx
-00002630: 2d6d 6920 636c 6173 733d 226d 6a78 2d69  -mi class="mjx-i
-00002640: 2220 7369 7a65 3d22 7322 3e3c 6d6a 782d  " size="s"><mjx-
-00002650: 6320 636c 6173 733d 226d 6a78 2d63 3144  c class="mjx-c1D
-00002660: 3433 3420 5445 582d 4922 3e3c 2f6d 6a78  434 TEX-I"></mjx
-00002670: 2d63 3e3c 2f6d 6a78 2d6d 693e 3c2f 6d6a  -c></mjx-mi></mj
-00002680: 782d 7363 7269 7074 3e3c 2f6d 6a78 2d6d  x-script></mjx-m
-00002690: 7375 623e 3c2f 6d6a 782d 6d61 7468 3e3c  sub></mjx-math><
-000026a0: 6d6a 782d 6173 7369 7374 6976 652d 6d6d  mjx-assistive-mm
-000026b0: 6c20 756e 7365 6c65 6374 6162 6c65 3d22  l unselectable="
-000026c0: 6f6e 2220 6469 7370 6c61 793d 2269 6e6c  on" display="inl
-000026d0: 696e 6522 3e3c 6d61 7468 2078 6d6c 6e73  ine"><math xmlns
-000026e0: 3d22 6874 7470 3a2f 2f77 7777 2e77 332e  ="http://www.w3.
-000026f0: 6f72 672f 3139 3938 2f4d 6174 682f 4d61  org/1998/Math/Ma
-00002700: 7468 4d4c 223e 3c6d 7375 623e 3c6d 693e  thML"><msub><mi>
-00002710: 543c 2f6d 693e 3c6d 693e 413c 2f6d 693e  T</mi><mi>A</mi>
-00002720: 3c2f 6d73 7562 3e3c 2f6d 6174 683e 3c2f  </msub></math></
-00002730: 6d6a 782d 6173 7369 7374 6976 652d 6d6d  mjx-assistive-mm
-00002740: 6c3e 3c2f 6d6a 782d 636f 6e74 6169 6e65  l></mjx-containe
-00002750: 723e 3c2f 7370 616e 3e2e 2041 2073 696d  r></span>. A sim
-00002760: 706c 6520 696c 6c75 7374 7261 7469 6f6e  ple illustration
-00002770: 206f 6620 7468 6520 6c69 6674 2d6f 7665   of the lift-ove
-00002780: 7220 7072 6f62 6c65 6d20 6973 2073 686f  r problem is sho
-00002790: 776e 2069 6e20 3c61 2063 6c61 7373 3d22  wn in <a class="
-000027a0: 7265 6665 7265 6e63 6520 696e 7465 726e  reference intern
-000027b0: 616c 2220 6872 6566 3d22 236c 6966 746f  al" href="#lifto
-000027c0: 7665 722d 696c 6c75 7374 7261 7469 6f6e  ver-illustration
-000027d0: 223e 3c73 7061 6e20 636c 6173 733d 2273  "><span class="s
-000027e0: 7464 2073 7464 2d6e 756d 7265 6622 3e46  td std-numref">F
-000027f0: 6967 7572 6520 313c 2f73 7061 6e3e 3c2f  igure 1</span></
-00002800: 613e 2e3c 2f70 3e0a 3c66 6967 7572 6520  a>.</p>.<figure 
-00002810: 636c 6173 733d 2261 6c69 676e 2d63 656e  class="align-cen
-00002820: 7465 7222 2069 643d 2269 6435 223e 0a3c  ter" id="id5">.<
-00002830: 7370 616e 2069 643d 226c 6966 746f 7665  span id="liftove
-00002840: 722d 696c 6c75 7374 7261 7469 6f6e 223e  r-illustration">
-00002850: 3c2f 7370 616e 3e3c 6120 636c 6173 733d  </span><a class=
-00002860: 2272 6566 6572 656e 6365 2069 6e74 6572  "reference inter
-00002870: 6e61 6c20 696d 6167 652d 7265 6665 7265  nal image-refere
-00002880: 6e63 6522 2068 7265 663d 2267 7261 7068  nce" href="graph
-00002890: 6963 732f 6c69 6674 6f76 6572 5f69 6c6c  ics/liftover_ill
-000028a0: 7573 7472 6174 696f 6e2e 6769 6622 3e3c  ustration.gif"><
-000028b0: 696d 6720 616c 743d 2267 7261 7068 6963  img alt="graphic
-000028c0: 732f 6c69 6674 6f76 6572 5f69 6c6c 7573  s/liftover_illus
-000028d0: 7472 6174 696f 6e2e 6769 6622 2073 7263  tration.gif" src
-000028e0: 3d22 6772 6170 6869 6373 2f6c 6966 746f  ="graphics/lifto
-000028f0: 7665 725f 696c 6c75 7374 7261 7469 6f6e  ver_illustration
-00002900: 2e67 6966 2220 7374 796c 653d 2277 6964  .gif" style="wid
-00002910: 7468 3a20 3637 322e 3570 783b 2068 6569  th: 672.5px; hei
-00002920: 6768 743a 2032 3730 2e30 7078 3b22 3e3c  ght: 270.0px;"><
-00002930: 2f61 3e0a 3c66 6967 6361 7074 696f 6e3e  /a>.<figcaption>
-00002940: 0a3c 703e 3c73 7061 6e20 636c 6173 733d  .<p><span class=
-00002950: 2263 6170 7469 6f6e 2d6e 756d 6265 7222  "caption-number"
-00002960: 3e46 6967 7572 6520 3120 3c2f 7370 616e  >Figure 1 </span
-00002970: 3e3c 7370 616e 2063 6c61 7373 3d22 6361  ><span class="ca
-00002980: 7074 696f 6e2d 7465 7874 223e 496c 6c75  ption-text">Illu
-00002990: 7374 7261 7469 6f6e 206f 6620 7468 6520  stration of the 
-000029a0: 6c69 6674 2d6f 7665 7220 7072 6f62 6c65  lift-over proble
-000029b0: 6d2e 2054 6865 2061 6e6e 6f74 6174 696f  m. The annotatio
-000029c0: 6e20 6669 6c65 2066 726f 6d20 7468 6520  n file from the 
-000029d0: 7265 6665 7265 6e63 6520 6765 6e6f 6d65  reference genome
-000029e0: 2028 746f 7029 2069 7320 6c69 6674 6564   (top) is lifted
-000029f0: 206f 7665 7220 746f 2074 6865 2074 6172   over to the tar
-00002a00: 6765 7420 6765 6e6f 6d65 2028 626f 7474  get genome (bott
-00002a10: 6f6d 292e 3c2f 7370 616e 3e3c 6120 636c  om).</span><a cl
-00002a20: 6173 733d 2268 6561 6465 726c 696e 6b22  ass="headerlink"
-00002a30: 2068 7265 663d 2223 6964 3522 2074 6974   href="#id5" tit
-00002a40: 6c65 3d22 5065 726d 616c 696e 6b20 746f  le="Permalink to
-00002a50: 2074 6869 7320 696d 6167 6522 3e23 3c2f   this image">#</
-00002a60: 613e 3c2f 703e 0a3c 2f66 6967 6361 7074  a></p>.</figcapt
-00002a70: 696f 6e3e 0a3c 2f66 6967 7572 653e 0a3c  ion>.</figure>.<
-00002a80: 6469 7620 636c 6173 733d 226c 696e 652d  div class="line-
-00002a90: 626c 6f63 6b22 3e0a 3c64 6976 2063 6c61  block">.<div cla
-00002aa0: 7373 3d22 6c69 6e65 223e 3c62 723e 3c2f  ss="line"><br></
-00002ab0: 6469 763e 0a3c 2f64 6976 3e0a 3c70 3e4c  div>.</div>.<p>L
-00002ac0: 6966 744f 6e20 6973 2074 6865 2062 6573  iftOn is the bes
-00002ad0: 7420 746f 6f6c 2074 6f20 6865 6c70 2079  t tool to help y
-00002ae0: 6f75 2073 6f6c 7665 2074 6869 7320 7072  ou solve this pr
-00002af0: 6f62 6c65 6d21 204c 6966 744f 6e20 656d  oblem! LiftOn em
-00002b00: 706c 6f79 7320 6120 7477 6f2d 7374 6570  ploys a two-step
-00002b10: 203c 6120 636c 6173 733d 2272 6566 6572   <a class="refer
-00002b20: 656e 6365 2069 6e74 6572 6e61 6c22 2068  ence internal" h
-00002b30: 7265 663d 2268 7474 703a 2f2f 6363 622e  ref="http://ccb.
-00002b40: 6a68 752e 6564 752f 6c69 6674 6f6e 2f63  jhu.edu/lifton/c
-00002b50: 6f6e 7465 6e74 2f62 6568 696e 645f 7363  ontent/behind_sc
-00002b60: 656e 6573 2e68 746d 6c23 7072 6f74 6569  enes.html#protei
-00002b70: 6e2d 6d61 7869 6d69 7a61 7469 6f6e 2d61  n-maximization-a
-00002b80: 6c67 6f72 6974 686d 223e 3c73 7061 6e20  lgorithm"><span 
-00002b90: 636c 6173 733d 2273 7464 2073 7464 2d72  class="std std-r
-00002ba0: 6566 223e 7072 6f74 6569 6e20 6d61 7869  ef">protein maxi
-00002bb0: 6d69 7a61 7469 6f6e 2061 6c67 6f72 6974  mization algorit
-00002bc0: 686d 3c2f 7370 616e 3e3c 2f61 3e20 2850  hm</span></a> (P
-00002bd0: 4d20 616c 676f 7269 7468 6d29 2e3c 2f70  M algorithm).</p
-00002be0: 3e0a 3c6f 6c20 636c 6173 733d 2261 7261  >.<ol class="ara
-00002bf0: 6269 6320 7369 6d70 6c65 223e 0a3c 6c69  bic simple">.<li
-00002c00: 3e3c 703e 5468 6520 6669 7273 7420 6d6f  ><p>The first mo
-00002c10: 6475 6c65 2069 7320 7468 6520 3c65 6d3e  dule is the <em>
-00002c20: 6368 6169 6e69 6e67 2061 6c67 6f72 6974  chaining algorit
-00002c30: 686d 3c2f 656d 3e2e 2049 7420 7374 6172  hm</em>. It star
-00002c40: 7473 2062 7920 6578 7472 6163 7469 6e67  ts by extracting
-00002c50: 2070 726f 7465 696e 2073 6571 7565 6e63   protein sequenc
-00002c60: 6573 2061 6e6e 6f74 6174 6564 2062 7920  es annotated by 
-00002c70: 4c69 6674 6f66 6620 616e 6420 6d69 6e69  Liftoff and mini
-00002c80: 7072 6f74 2e20 4c69 6674 4f6e 2074 6865  prot. LiftOn the
-00002c90: 6e20 616c 6967 6e73 2074 6865 7365 2073  n aligns these s
-00002ca0: 6571 7565 6e63 6573 2074 6f20 6675 6c6c  equences to full
-00002cb0: 2d6c 656e 6774 6820 7265 6665 7265 6e63  -length referenc
-00002cc0: 6520 7072 6f74 6569 6e73 2e20 466f 7220  e proteins. For 
-00002cd0: 6561 6368 2067 656e 6520 6c6f 6375 732c  each gene locus,
-00002ce0: 204c 6966 744f 6e20 636f 6d70 6172 6573   LiftOn compares
-00002cf0: 2065 6163 6820 7365 6374 696f 6e20 6f66   each section of
-00002d00: 2074 6865 2070 726f 7465 696e 2061 6c69   the protein ali
-00002d10: 676e 6d65 6e74 7320 6672 6f6d 204c 6966  gnments from Lif
-00002d20: 746f 6666 2061 6e64 206d 696e 6970 726f  toff and minipro
-00002d30: 742c 2063 6861 696e 696e 6720 746f 6765  t, chaining toge
-00002d40: 7468 6572 2074 6865 2062 6573 7420 636f  ther the best co
-00002d50: 6d62 696e 6174 696f 6e73 2e3c 2f70 3e3c  mbinations.</p><
-00002d60: 2f6c 693e 0a3c 6c69 3e3c 703e 5468 6520  /li>.<li><p>The 
-00002d70: 7365 636f 6e64 206d 6f64 756c 6520 6973  second module is
-00002d80: 2074 6865 203c 656d 3e6f 7065 6e2d 7265   the <em>open-re
-00002d90: 6164 696e 6720 6672 616d 6520 7365 6172  ading frame sear
-00002da0: 6368 2028 4f52 4620 7365 6172 6368 2920  ch (ORF search) 
-00002db0: 616c 676f 7269 7468 6d3c 2f65 6d3e 2e20  algorithm</em>. 
-00002dc0: 496e 2074 6865 2063 6173 6520 6f66 2074  In the case of t
-00002dd0: 7275 6e63 6174 6564 2070 726f 7465 696e  runcated protein
-00002de0: 2d63 6f64 696e 6720 7472 616e 7363 7269  -coding transcri
-00002df0: 7074 732c 2074 6869 7320 616c 676f 7269  pts, this algori
-00002e00: 7468 6d20 6578 616d 696e 6573 2061 6c74  thm examines alt
-00002e10: 6572 6e61 7469 7665 2066 7261 6d65 7320  ernative frames 
-00002e20: 746f 2069 6465 6e74 6966 7920 7468 6520  to identify the 
-00002e30: 4f52 4620 7468 6174 2070 726f 6475 6365  ORF that produce
-00002e40: 7320 7468 6520 6c6f 6e67 6573 7420 6d61  s the longest ma
-00002e50: 7463 6820 7769 7468 2074 6865 2072 6566  tch with the ref
-00002e60: 6572 656e 6365 2070 726f 7465 696e 2e3c  erence protein.<
-00002e70: 2f70 3e3c 2f6c 693e 0a3c 2f6f 6c3e 0a3c  /p></li>.</ol>.<
-00002e80: 756c 2063 6c61 7373 3d22 7369 6d70 6c65  ul class="simple
-00002e90: 223e 0a3c 6c69 3e3c 646c 2063 6c61 7373  ">.<li><dl class
-00002ea0: 3d22 7369 6d70 6c65 223e 0a3c 6474 3e3c  ="simple">.<dt><
-00002eb0: 7374 726f 6e67 3e49 6e70 7574 3c2f 7374  strong>Input</st
-00002ec0: 726f 6e67 3e3a 3c2f 6474 3e3c 6464 3e3c  rong>:</dt><dd><
-00002ed0: 6f6c 2063 6c61 7373 3d22 6172 6162 6963  ol class="arabic
-00002ee0: 2073 696d 706c 6522 3e0a 3c6c 693e 3c70   simple">.<li><p
-00002ef0: 3e74 6172 6765 7420 3c73 7472 6f6e 673e  >target <strong>
-00002f00: 4765 6e6f 6d65 3c2f 7374 726f 6e67 3e20  Genome</strong> 
-00002f10: 3c73 7061 6e20 636c 6173 733d 226d 6174  <span class="mat
-00002f20: 6820 6e6f 7472 616e 736c 6174 6520 6e6f  h notranslate no
-00002f30: 6869 6768 6c69 6768 7422 3e3c 6d6a 782d  highlight"><mjx-
-00002f40: 636f 6e74 6169 6e65 7220 636c 6173 733d  container class=
-00002f50: 224d 6174 684a 6178 2043 7478 744d 656e  "MathJax CtxtMen
-00002f60: 755f 4174 7461 6368 6564 5f30 2220 6a61  u_Attached_0" ja
-00002f70: 783d 2243 4854 4d4c 2220 7461 6269 6e64  x="CHTML" tabind
-00002f80: 6578 3d22 3022 2063 7478 746d 656e 755f  ex="0" ctxtmenu_
-00002f90: 636f 756e 7465 723d 2237 2220 7374 796c  counter="7" styl
-00002fa0: 653d 2266 6f6e 742d 7369 7a65 3a20 3131  e="font-size: 11
-00002fb0: 3925 3b20 706f 7369 7469 6f6e 3a20 7265  9%; position: re
-00002fc0: 6c61 7469 7665 3b22 3e3c 6d6a 782d 6d61  lative;"><mjx-ma
-00002fd0: 7468 2063 6c61 7373 3d22 4d4a 582d 5445  th class="MJX-TE
-00002fe0: 5822 2061 7269 612d 6869 6464 656e 3d22  X" aria-hidden="
-00002ff0: 7472 7565 223e 3c6d 6a78 2d6d 6920 636c  true"><mjx-mi cl
-00003000: 6173 733d 226d 6a78 2d69 223e 3c6d 6a78  ass="mjx-i"><mjx
-00003010: 2d63 2063 6c61 7373 3d22 6d6a 782d 6331  -c class="mjx-c1
-00003020: 4434 3437 2054 4558 2d49 223e 3c2f 6d6a  D447 TEX-I"></mj
-00003030: 782d 633e 3c2f 6d6a 782d 6d69 3e3c 2f6d  x-c></mjx-mi></m
-00003040: 6a78 2d6d 6174 683e 3c6d 6a78 2d61 7373  jx-math><mjx-ass
-00003050: 6973 7469 7665 2d6d 6d6c 2075 6e73 656c  istive-mml unsel
-00003060: 6563 7461 626c 653d 226f 6e22 2064 6973  ectable="on" dis
-00003070: 706c 6179 3d22 696e 6c69 6e65 223e 3c6d  play="inline"><m
-00003080: 6174 6820 786d 6c6e 733d 2268 7474 703a  ath xmlns="http:
-00003090: 2f2f 7777 772e 7733 2e6f 7267 2f31 3939  //www.w3.org/199
-000030a0: 382f 4d61 7468 2f4d 6174 684d 4c22 3e3c  8/Math/MathML"><
-000030b0: 6d69 3e54 3c2f 6d69 3e3c 2f6d 6174 683e  mi>T</mi></math>
-000030c0: 3c2f 6d6a 782d 6173 7369 7374 6976 652d  </mjx-assistive-
-000030d0: 6d6d 6c3e 3c2f 6d6a 782d 636f 6e74 6169  mml></mjx-contai
-000030e0: 6e65 723e 3c2f 7370 616e 3e20 696e 2046  ner></span> in F
-000030f0: 4153 5441 2e3c 2f70 3e3c 2f6c 693e 0a3c  ASTA.</p></li>.<
-00003100: 6c69 3e3c 703e 7265 6665 7265 6e63 6520  li><p>reference 
-00003110: 3c73 7472 6f6e 673e 4765 6e6f 6d65 3c2f  <strong>Genome</
-00003120: 7374 726f 6e67 3e20 3c73 7061 6e20 636c  strong> <span cl
-00003130: 6173 733d 226d 6174 6820 6e6f 7472 616e  ass="math notran
-00003140: 736c 6174 6520 6e6f 6869 6768 6c69 6768  slate nohighligh
-00003150: 7422 3e3c 6d6a 782d 636f 6e74 6169 6e65  t"><mjx-containe
-00003160: 7220 636c 6173 733d 224d 6174 684a 6178  r class="MathJax
-00003170: 2043 7478 744d 656e 755f 4174 7461 6368   CtxtMenu_Attach
-00003180: 6564 5f30 2220 6a61 783d 2243 4854 4d4c  ed_0" jax="CHTML
-00003190: 2220 7461 6269 6e64 6578 3d22 3022 2063  " tabindex="0" c
-000031a0: 7478 746d 656e 755f 636f 756e 7465 723d  txtmenu_counter=
-000031b0: 2238 2220 7374 796c 653d 2266 6f6e 742d  "8" style="font-
-000031c0: 7369 7a65 3a20 3131 3925 3b20 706f 7369  size: 119%; posi
-000031d0: 7469 6f6e 3a20 7265 6c61 7469 7665 3b22  tion: relative;"
-000031e0: 3e3c 6d6a 782d 6d61 7468 2063 6c61 7373  ><mjx-math class
-000031f0: 3d22 4d4a 582d 5445 5822 2061 7269 612d  ="MJX-TEX" aria-
-00003200: 6869 6464 656e 3d22 7472 7565 223e 3c6d  hidden="true"><m
-00003210: 6a78 2d6d 6920 636c 6173 733d 226d 6a78  jx-mi class="mjx
-00003220: 2d69 223e 3c6d 6a78 2d63 2063 6c61 7373  -i"><mjx-c class
-00003230: 3d22 6d6a 782d 6331 4434 3435 2054 4558  ="mjx-c1D445 TEX
-00003240: 2d49 223e 3c2f 6d6a 782d 633e 3c2f 6d6a  -I"></mjx-c></mj
-00003250: 782d 6d69 3e3c 2f6d 6a78 2d6d 6174 683e  x-mi></mjx-math>
-00003260: 3c6d 6a78 2d61 7373 6973 7469 7665 2d6d  <mjx-assistive-m
-00003270: 6d6c 2075 6e73 656c 6563 7461 626c 653d  ml unselectable=
-00003280: 226f 6e22 2064 6973 706c 6179 3d22 696e  "on" display="in
-00003290: 6c69 6e65 223e 3c6d 6174 6820 786d 6c6e  line"><math xmln
-000032a0: 733d 2268 7474 703a 2f2f 7777 772e 7733  s="http://www.w3
-000032b0: 2e6f 7267 2f31 3939 382f 4d61 7468 2f4d  .org/1998/Math/M
-000032c0: 6174 684d 4c22 3e3c 6d69 3e52 3c2f 6d69  athML"><mi>R</mi
-000032d0: 3e3c 2f6d 6174 683e 3c2f 6d6a 782d 6173  ></math></mjx-as
-000032e0: 7369 7374 6976 652d 6d6d 6c3e 3c2f 6d6a  sistive-mml></mj
-000032f0: 782d 636f 6e74 6169 6e65 723e 3c2f 7370  x-container></sp
-00003300: 616e 3e20 696e 2046 4153 5441 3c2f 703e  an> in FASTA</p>
-00003310: 3c2f 6c69 3e0a 3c6c 693e 3c70 3e72 6566  </li>.<li><p>ref
-00003320: 6572 656e 6365 203c 7374 726f 6e67 3e41  erence <strong>A
-00003330: 6e6e 6f74 6174 696f 6e3c 2f73 7472 6f6e  nnotation</stron
-00003340: 673e 203c 7370 616e 2063 6c61 7373 3d22  g> <span class="
-00003350: 6d61 7468 206e 6f74 7261 6e73 6c61 7465  math notranslate
-00003360: 206e 6f68 6967 686c 6967 6874 223e 3c6d   nohighlight"><m
-00003370: 6a78 2d63 6f6e 7461 696e 6572 2063 6c61  jx-container cla
-00003380: 7373 3d22 4d61 7468 4a61 7820 4374 7874  ss="MathJax Ctxt
-00003390: 4d65 6e75 5f41 7474 6163 6865 645f 3022  Menu_Attached_0"
-000033a0: 206a 6178 3d22 4348 544d 4c22 2074 6162   jax="CHTML" tab
-000033b0: 696e 6465 783d 2230 2220 6374 7874 6d65  index="0" ctxtme
-000033c0: 6e75 5f63 6f75 6e74 6572 3d22 3922 2073  nu_counter="9" s
-000033d0: 7479 6c65 3d22 666f 6e74 2d73 697a 653a  tyle="font-size:
-000033e0: 2031 3139 253b 2070 6f73 6974 696f 6e3a   119%; position:
-000033f0: 2072 656c 6174 6976 653b 223e 3c6d 6a78   relative;"><mjx
-00003400: 2d6d 6174 6820 636c 6173 733d 224d 4a58  -math class="MJX
-00003410: 2d54 4558 2220 6172 6961 2d68 6964 6465  -TEX" aria-hidde
-00003420: 6e3d 2274 7275 6522 3e3c 6d6a 782d 6d73  n="true"><mjx-ms
-00003430: 7562 3e3c 6d6a 782d 6d69 2063 6c61 7373  ub><mjx-mi class
-00003440: 3d22 6d6a 782d 6922 3e3c 6d6a 782d 6320  ="mjx-i"><mjx-c 
-00003450: 636c 6173 733d 226d 6a78 2d63 3144 3434  class="mjx-c1D44
-00003460: 3520 5445 582d 4922 3e3c 2f6d 6a78 2d63  5 TEX-I"></mjx-c
-00003470: 3e3c 2f6d 6a78 2d6d 693e 3c6d 6a78 2d73  ></mjx-mi><mjx-s
-00003480: 6372 6970 7420 7374 796c 653d 2276 6572  cript style="ver
-00003490: 7469 6361 6c2d 616c 6967 6e3a 202d 302e  tical-align: -0.
-000034a0: 3135 3365 6d3b 223e 3c6d 6a78 2d6d 6920  153em;"><mjx-mi 
-000034b0: 636c 6173 733d 226d 6a78 2d69 2220 7369  class="mjx-i" si
-000034c0: 7a65 3d22 7322 3e3c 6d6a 782d 6320 636c  ze="s"><mjx-c cl
-000034d0: 6173 733d 226d 6a78 2d63 3144 3433 3420  ass="mjx-c1D434 
-000034e0: 5445 582d 4922 3e3c 2f6d 6a78 2d63 3e3c  TEX-I"></mjx-c><
-000034f0: 2f6d 6a78 2d6d 693e 3c2f 6d6a 782d 7363  /mjx-mi></mjx-sc
-00003500: 7269 7074 3e3c 2f6d 6a78 2d6d 7375 623e  ript></mjx-msub>
-00003510: 3c2f 6d6a 782d 6d61 7468 3e3c 6d6a 782d  </mjx-math><mjx-
-00003520: 6173 7369 7374 6976 652d 6d6d 6c20 756e  assistive-mml un
-00003530: 7365 6c65 6374 6162 6c65 3d22 6f6e 2220  selectable="on" 
-00003540: 6469 7370 6c61 793d 2269 6e6c 696e 6522  display="inline"
-00003550: 3e3c 6d61 7468 2078 6d6c 6e73 3d22 6874  ><math xmlns="ht
-00003560: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
-00003570: 3139 3938 2f4d 6174 682f 4d61 7468 4d4c  1998/Math/MathML
-00003580: 223e 3c6d 7375 623e 3c6d 693e 523c 2f6d  "><msub><mi>R</m
-00003590: 693e 3c6d 693e 413c 2f6d 693e 3c2f 6d73  i><mi>A</mi></ms
-000035a0: 7562 3e3c 2f6d 6174 683e 3c2f 6d6a 782d  ub></math></mjx-
-000035b0: 6173 7369 7374 6976 652d 6d6d 6c3e 3c2f  assistive-mml></
-000035c0: 6d6a 782d 636f 6e74 6169 6e65 723e 3c2f  mjx-container></
-000035d0: 7370 616e 3e20 696e 2047 4646 333c 2f70  span> in GFF3</p
-000035e0: 3e3c 2f6c 693e 0a3c 2f6f 6c3e 0a3c 2f64  ></li>.</ol>.</d
-000035f0: 643e 0a3c 2f64 6c3e 0a3c 2f6c 693e 0a3c  d>.</dl>.</li>.<
-00003600: 6c69 3e3c 646c 2063 6c61 7373 3d22 7369  li><dl class="si
-00003610: 6d70 6c65 223e 0a3c 6474 3e3c 7374 726f  mple">.<dt><stro
-00003620: 6e67 3e4f 7574 7075 743c 2f73 7472 6f6e  ng>Output</stron
-00003630: 673e 3a3c 2f64 743e 3c64 643e 3c6f 6c20  g>:</dt><dd><ol 
-00003640: 636c 6173 733d 2261 7261 6269 6320 7369  class="arabic si
-00003650: 6d70 6c65 223e 0a3c 6c69 3e3c 703e 4c69  mple">.<li><p>Li
-00003660: 6674 4f6e 2061 6e6e 6f74 6174 696f 6e20  ftOn annotation 
-00003670: 6669 6c65 2c20 3c73 7472 6f6e 673e 416e  file, <strong>An
-00003680: 6e6f 7461 7469 6f6e 3c2f 7374 726f 6e67  notation</strong
-00003690: 3e20 3c73 7061 6e20 636c 6173 733d 226d  > <span class="m
-000036a0: 6174 6820 6e6f 7472 616e 736c 6174 6520  ath notranslate 
-000036b0: 6e6f 6869 6768 6c69 6768 7422 3e3c 6d6a  nohighlight"><mj
-000036c0: 782d 636f 6e74 6169 6e65 7220 636c 6173  x-container clas
-000036d0: 733d 224d 6174 684a 6178 2043 7478 744d  s="MathJax CtxtM
-000036e0: 656e 755f 4174 7461 6368 6564 5f30 2220  enu_Attached_0" 
-000036f0: 6a61 783d 2243 4854 4d4c 2220 7461 6269  jax="CHTML" tabi
-00003700: 6e64 6578 3d22 3022 2063 7478 746d 656e  ndex="0" ctxtmen
-00003710: 755f 636f 756e 7465 723d 2231 3022 2073  u_counter="10" s
-00003720: 7479 6c65 3d22 666f 6e74 2d73 697a 653a  tyle="font-size:
-00003730: 2031 3139 253b 2070 6f73 6974 696f 6e3a   119%; position:
-00003740: 2072 656c 6174 6976 653b 223e 3c6d 6a78   relative;"><mjx
-00003750: 2d6d 6174 6820 636c 6173 733d 224d 4a58  -math class="MJX
-00003760: 2d54 4558 2220 6172 6961 2d68 6964 6465  -TEX" aria-hidde
-00003770: 6e3d 2274 7275 6522 3e3c 6d6a 782d 6d73  n="true"><mjx-ms
-00003780: 7562 3e3c 6d6a 782d 6d69 2063 6c61 7373  ub><mjx-mi class
-00003790: 3d22 6d6a 782d 6922 3e3c 6d6a 782d 6320  ="mjx-i"><mjx-c 
-000037a0: 636c 6173 733d 226d 6a78 2d63 3144 3434  class="mjx-c1D44
-000037b0: 3720 5445 582d 4922 3e3c 2f6d 6a78 2d63  7 TEX-I"></mjx-c
-000037c0: 3e3c 2f6d 6a78 2d6d 693e 3c6d 6a78 2d73  ></mjx-mi><mjx-s
-000037d0: 6372 6970 7420 7374 796c 653d 2276 6572  cript style="ver
-000037e0: 7469 6361 6c2d 616c 6967 6e3a 202d 302e  tical-align: -0.
-000037f0: 3135 3365 6d3b 206d 6172 6769 6e2d 6c65  153em; margin-le
-00003800: 6674 3a20 2d30 2e31 3265 6d3b 223e 3c6d  ft: -0.12em;"><m
-00003810: 6a78 2d6d 6920 636c 6173 733d 226d 6a78  jx-mi class="mjx
-00003820: 2d69 2220 7369 7a65 3d22 7322 3e3c 6d6a  -i" size="s"><mj
-00003830: 782d 6320 636c 6173 733d 226d 6a78 2d63  x-c class="mjx-c
-00003840: 3144 3433 3420 5445 582d 4922 3e3c 2f6d  1D434 TEX-I"></m
-00003850: 6a78 2d63 3e3c 2f6d 6a78 2d6d 693e 3c2f  jx-c></mjx-mi></
-00003860: 6d6a 782d 7363 7269 7074 3e3c 2f6d 6a78  mjx-script></mjx
-00003870: 2d6d 7375 623e 3c2f 6d6a 782d 6d61 7468  -msub></mjx-math
-00003880: 3e3c 6d6a 782d 6173 7369 7374 6976 652d  ><mjx-assistive-
-00003890: 6d6d 6c20 756e 7365 6c65 6374 6162 6c65  mml unselectable
-000038a0: 3d22 6f6e 2220 6469 7370 6c61 793d 2269  ="on" display="i
-000038b0: 6e6c 696e 6522 3e3c 6d61 7468 2078 6d6c  nline"><math xml
-000038c0: 6e73 3d22 6874 7470 3a2f 2f77 7777 2e77  ns="http://www.w
-000038d0: 332e 6f72 672f 3139 3938 2f4d 6174 682f  3.org/1998/Math/
-000038e0: 4d61 7468 4d4c 223e 3c6d 7375 623e 3c6d  MathML"><msub><m
-000038f0: 693e 543c 2f6d 693e 3c6d 693e 413c 2f6d  i>T</mi><mi>A</m
-00003900: 693e 3c2f 6d73 7562 3e3c 2f6d 6174 683e  i></msub></math>
-00003910: 3c2f 6d6a 782d 6173 7369 7374 6976 652d  </mjx-assistive-
-00003920: 6d6d 6c3e 3c2f 6d6a 782d 636f 6e74 6169  mml></mjx-contai
-00003930: 6e65 723e 3c2f 7370 616e 3e2c 2069 6e20  ner></span>, in 
-00003940: 4746 4633 3c2f 703e 3c2f 6c69 3e0a 3c6c  GFF3</p></li>.<l
-00003950: 693e 3c70 3e50 726f 7465 696e 2073 6571  i><p>Protein seq
-00003960: 7565 6e63 6520 6964 656e 7469 7469 6573  uence identities
-00003970: 2026 616d 703b 206d 7574 6174 696f 6e20   &amp; mutation 
-00003980: 7479 7065 733c 2f70 3e3c 2f6c 693e 0a3c  types</p></li>.<
-00003990: 6c69 3e3c 703e 4665 6174 7572 6573 2077  li><p>Features w
-000039a0: 6974 6820 6578 7472 6120 636f 7069 6573  ith extra copies
-000039b0: 3c2f 703e 3c2f 6c69 3e0a 3c6c 693e 3c70  </p></li>.<li><p
-000039c0: 3e55 6e6d 6170 7065 6420 6665 6174 7572  >Unmapped featur
-000039d0: 6573 3c2f 703e 3c2f 6c69 3e0a 3c2f 6f6c  es</p></li>.</ol
-000039e0: 3e0a 3c2f 6464 3e0a 3c2f 646c 3e0a 3c2f  >.</dd>.</dl>.</
-000039f0: 6c69 3e0a 3c2f 756c 3e0a 3c64 6976 2063  li>.</ul>.<div c
-00003a00: 6c61 7373 3d22 6c69 6e65 2d62 6c6f 636b  lass="line-block
-00003a10: 223e 0a3c 6469 7620 636c 6173 733d 226c  ">.<div class="l
-00003a20: 696e 6522 3e3c 6272 3e3c 2f64 6976 3e0a  ine"><br></div>.
-00003a30: 3c2f 6469 763e 0a3c 2f73 6563 7469 6f6e  </div>.</section
-00003a40: 3e0a 3c73 6563 7469 6f6e 2069 643d 226c  >.<section id="l
-00003a50: 6966 746f 6e2d 732d 6c69 6d69 7461 7469  ifton-s-limitati
-00003a60: 6f6e 2220 636c 6173 733d 2261 6374 6976  on" class="activ
-00003a70: 6522 3e0a 3c68 323e 4c69 6674 4f6e 2773  e">.<h2>LiftOn's
-00003a80: 206c 696d 6974 6174 696f 6e3c 6120 636c   limitation<a cl
-00003a90: 6173 733d 2268 6561 6465 726c 696e 6b22  ass="headerlink"
-00003aa0: 2068 7265 663d 2223 6c69 6674 6f6e 2d73   href="#lifton-s
-00003ab0: 2d6c 696d 6974 6174 696f 6e22 2074 6974  -limitation" tit
-00003ac0: 6c65 3d22 5065 726d 616c 696e 6b20 746f  le="Permalink to
-00003ad0: 2074 6869 7320 6865 6164 696e 6722 3e23   this heading">#
-00003ae0: 3c2f 613e 3c2f 6832 3e0a 3c70 3e4c 6966  </a></h2>.<p>Lif
-00003af0: 744f 6e27 7320 3c65 6d3e 6368 6169 6e69  tOn's <em>chaini
-00003b00: 6e67 2061 6c67 6f72 6974 686d 3c2f 656d  ng algorithm</em
-00003b10: 3e20 6375 7272 656e 746c 7920 6f6e 6c79  > currently only
-00003b20: 2075 7469 6c69 7a65 7320 6d69 6e69 7072   utilizes minipr
-00003b30: 6f74 2061 6c69 676e 6d65 6e74 2072 6573  ot alignment res
-00003b40: 756c 7473 2074 6f20 6669 7820 7468 6520  ults to fix the 
-00003b50: 4c69 6674 6f66 6620 616e 6e6f 7461 7469  Liftoff annotati
-00003b60: 6f6e 2e20 486f 7765 7665 722c 2069 7420  on. However, it 
-00003b70: 6361 6e20 6265 2065 7874 656e 6465 6420  can be extended 
-00003b80: 746f 2063 6861 696e 2074 6f67 6574 6865  to chain togethe
-00003b90: 7220 6d75 6c74 6970 6c65 2070 726f 7465  r multiple prote
-00003ba0: 696e 2d62 6173 6564 2061 6e6e 6f74 6174  in-based annotat
-00003bb0: 696f 6e20 6669 6c65 7320 6f72 2061 6173  ion files or aas
-00003bc0: 656d 626c 6564 2052 4e41 2d53 6571 2074  embled RNA-Seq t
-00003bd0: 7261 6e73 6372 6970 7473 2e3c 2f70 3e0a  ranscripts.</p>.
-00003be0: 3c70 3e44 4e41 2d20 616e 6420 7072 6f74  <p>DNA- and prot
-00003bf0: 6569 6e2d 6261 7365 6420 6d65 7468 6f64  ein-based method
-00003c00: 7320 7374 696c 6c20 6861 7665 2073 6f6d  s still have som
-00003c10: 6520 6c69 6d69 7461 7469 6f6e 732e 2057  e limitations. W
-00003c20: 6520 6172 6520 6465 7665 6c6f 7069 6e67  e are developing
-00003c30: 2061 206d 6f64 756c 6520 746f 206d 6572   a module to mer
-00003c40: 6765 2074 6865 204c 6966 744f 6e20 616e  ge the LiftOn an
-00003c50: 6e6f 7461 7469 6f6e 2077 6974 6820 7468  notation with th
-00003c60: 6520 7265 6c65 6173 6564 2063 7572 6174  e released curat
-00003c70: 6564 2061 6e6e 6f74 6174 696f 6e73 2074  ed annotations t
-00003c80: 6f20 6765 6e65 7261 7465 2062 6574 7465  o generate bette
-00003c90: 7220 616e 6e6f 7461 7469 6f6e 732e 3c2f  r annotations.</
-00003ca0: 703e 0a3c 703e 5468 6520 4c69 6674 4f6e  p>.<p>The LiftOn
-00003cb0: 203c 656d 3e63 6861 696e 696e 6720 616c   <em>chaining al
-00003cc0: 676f 7269 7468 6d3c 2f65 6d3e 206e 6f77  gorithm</em> now
-00003cd0: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
-00003ce0: 7420 6d75 6c74 692d 7468 7265 6164 696e  t multi-threadin
-00003cf0: 672e 2054 6869 7320 6675 6e63 7469 6f6e  g. This function
-00003d00: 616c 6974 7920 7374 616e 6473 2061 7320  ality stands as 
-00003d10: 6f75 7220 6e65 7874 2074 6172 6765 7465  our next targete
-00003d20: 6420 6665 6174 7572 6520 6f6e 2074 6865  d feature on the
-00003d30: 2064 6576 656c 6f70 6d65 6e74 2068 6f72   development hor
-00003d40: 697a 6f6e 213c 2f70 3e0a 3c64 6976 2063  izon!</p>.<div c
-00003d50: 6c61 7373 3d22 6c69 6e65 2d62 6c6f 636b  lass="line-block
-00003d60: 223e 0a3c 6469 7620 636c 6173 733d 226c  ">.<div class="l
-00003d70: 696e 6522 3e3c 6272 3e3c 2f64 6976 3e0a  ine"><br></div>.
-00003d80: 3c2f 6469 763e 0a3c 2f73 6563 7469 6f6e  </div>.</section
-00003d90: 3e0a 3c73 6563 7469 6f6e 2069 643d 2275  >.<section id="u
-00003da0: 7365 722d 7375 7070 6f72 7422 3e0a 3c68  ser-support">.<h
-00003db0: 323e 5573 6572 2073 7570 706f 7274 3c61  2>User support<a
-00003dc0: 2063 6c61 7373 3d22 6865 6164 6572 6c69   class="headerli
-00003dd0: 6e6b 2220 6872 6566 3d22 2375 7365 722d  nk" href="#user-
-00003de0: 7375 7070 6f72 7422 2074 6974 6c65 3d22  support" title="
-00003df0: 5065 726d 616c 696e 6b20 746f 2074 6869  Permalink to thi
-00003e00: 7320 6865 6164 696e 6722 3e23 3c2f 613e  s heading">#</a>
-00003e10: 3c2f 6832 3e0a 3c70 3e50 6c65 6173 6520  </h2>.<p>Please 
-00003e20: 676f 2074 6872 6f75 6768 2074 6865 203c  go through the <
-00003e30: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
-00003e40: 6365 2069 6e74 6572 6e61 6c22 2068 7265  ce internal" hre
-00003e50: 663d 2223 7461 626c 652d 6f66 2d63 6f6e  f="#table-of-con
-00003e60: 7465 6e74 7322 3e3c 7370 616e 2063 6c61  tents"><span cla
-00003e70: 7373 3d22 7374 6420 7374 642d 7265 6622  ss="std std-ref"
-00003e80: 3e64 6f63 756d 656e 7461 7469 6f6e 3c2f  >documentation</
-00003e90: 7370 616e 3e3c 2f61 3e20 6265 6c6f 7720  span></a> below 
-00003ea0: 6669 7273 742e 2049 6620 796f 7520 6861  first. If you ha
-00003eb0: 7665 2071 7565 7374 696f 6e73 2061 626f  ve questions abo
-00003ec0: 7574 2075 7369 6e67 2074 6865 2070 6163  ut using the pac
-00003ed0: 6b61 6765 2c20 6120 6275 6720 7265 706f  kage, a bug repo
-00003ee0: 7274 2c20 6f72 2061 2066 6561 7475 7265  rt, or a feature
-00003ef0: 2072 6571 7565 7374 2c20 706c 6561 7365   request, please
-00003f00: 2075 7365 2074 6865 2047 6974 4875 6220   use the GitHub 
-00003f10: 6973 7375 6520 7472 6163 6b65 7220 6865  issue tracker he
-00003f20: 7265 3a3c 2f70 3e0a 3c70 3e3c 6120 636c  re:</p>.<p><a cl
-00003f30: 6173 733d 2272 6566 6572 656e 6365 2065  ass="reference e
-00003f40: 7874 6572 6e61 6c22 2068 7265 663d 2268  xternal" href="h
-00003f50: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00003f60: 6d2f 4b75 616e 6861 6f2d 4368 616f 2f4c  m/Kuanhao-Chao/L
-00003f70: 6966 744f 6e2f 6973 7375 6573 223e 6874  iftOn/issues">ht
-00003f80: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003f90: 2f4b 7561 6e68 616f 2d43 6861 6f2f 4c69  /Kuanhao-Chao/Li
-00003fa0: 6674 4f6e 2f69 7373 7565 733c 2f61 3e3c  ftOn/issues</a><
-00003fb0: 2f70 3e0a 3c64 6976 2063 6c61 7373 3d22  /p>.<div class="
-00003fc0: 6c69 6e65 2d62 6c6f 636b 223e 0a3c 6469  line-block">.<di
-00003fd0: 7620 636c 6173 733d 226c 696e 6522 3e3c  v class="line"><
-00003fe0: 6272 3e3c 2f64 6976 3e0a 3c2f 6469 763e  br></div>.</div>
-00003ff0: 0a3c 2f73 6563 7469 6f6e 3e0a 3c73 6563  .</section>.<sec
-00004000: 7469 6f6e 2069 643d 226b 6579 2d63 6f6e  tion id="key-con
-00004010: 7472 6962 7574 6f72 7322 3e0a 3c68 323e  tributors">.<h2>
-00004020: 4b65 7920 636f 6e74 7269 6275 746f 7273  Key contributors
-00004030: 3c61 2063 6c61 7373 3d22 6865 6164 6572  <a class="header
-00004040: 6c69 6e6b 2220 6872 6566 3d22 236b 6579  link" href="#key
-00004050: 2d63 6f6e 7472 6962 7574 6f72 7322 2074  -contributors" t
-00004060: 6974 6c65 3d22 5065 726d 616c 696e 6b20  itle="Permalink 
-00004070: 746f 2074 6869 7320 6865 6164 696e 6722  to this heading"
-00004080: 3e23 3c2f 613e 3c2f 6832 3e0a 3c70 3e4c  >#</a></h2>.<p>L
-00004090: 6966 744f 6e20 7761 7320 6465 7369 676e  iftOn was design
-000040a0: 6564 2061 6e64 2064 6576 656c 6f70 6564  ed and developed
-000040b0: 2062 7920 3c61 2063 6c61 7373 3d22 7265   by <a class="re
-000040c0: 6665 7265 6e63 6520 6578 7465 726e 616c  ference external
-000040d0: 2220 6872 6566 3d22 6874 7470 733a 2f2f  " href="https://
-000040e0: 6b68 6368 616f 2e63 6f6d 2f22 3e4b 7561  khchao.com/">Kua
-000040f0: 6e2d 4861 6f20 4368 616f 3c2f 613e 2e20  n-Hao Chao</a>. 
-00004100: 2054 6869 7320 646f 6375 6d65 6e74 6174   This documentat
-00004110: 696f 6e20 7761 7320 7772 6974 7465 6e20  ion was written 
-00004120: 6279 203c 6120 636c 6173 733d 2272 6566  by <a class="ref
-00004130: 6572 656e 6365 2065 7874 6572 6e61 6c22  erence external"
-00004140: 2068 7265 663d 2268 7474 7073 3a2f 2f6b   href="https://k
-00004150: 6863 6861 6f2e 636f 6d2f 223e 4b75 616e  hchao.com/">Kuan
-00004160: 2d48 616f 2043 6861 6f3c 2f61 3e2e 3c2f  -Hao Chao</a>.</
-00004170: 703e 0a3c 6469 7620 636c 6173 733d 226c  p>.<div class="l
-00004180: 696e 652d 626c 6f63 6b22 3e0a 3c64 6976  ine-block">.<div
-00004190: 2063 6c61 7373 3d22 6c69 6e65 223e 3c62   class="line"><b
-000041a0: 723e 3c2f 6469 763e 0a3c 2f64 6976 3e0a  r></div>.</div>.
-000041b0: 3c2f 7365 6374 696f 6e3e 0a3c 7365 6374  </section>.<sect
-000041c0: 696f 6e20 6964 3d22 7461 626c 652d 6f66  ion id="table-of
-000041d0: 2d63 6f6e 7465 6e74 7322 3e0a 3c73 7061  -contents">.<spa
-000041e0: 6e20 6964 3d22 6964 3322 3e3c 2f73 7061  n id="id3"></spa
-000041f0: 6e3e 3c68 323e 5461 626c 6520 6f66 2063  n><h2>Table of c
-00004200: 6f6e 7465 6e74 733c 6120 636c 6173 733d  ontents<a class=
-00004210: 2268 6561 6465 726c 696e 6b22 2068 7265  "headerlink" hre
-00004220: 663d 2223 7461 626c 652d 6f66 2d63 6f6e  f="#table-of-con
-00004230: 7465 6e74 7322 2074 6974 6c65 3d22 5065  tents" title="Pe
-00004240: 726d 616c 696e 6b20 746f 2074 6869 7320  rmalink to this 
-00004250: 6865 6164 696e 6722 3e23 3c2f 613e 3c2f  heading">#</a></
-00004260: 6832 3e0a 3c64 6976 2063 6c61 7373 3d22  h2>.<div class="
-00004270: 746f 6374 7265 652d 7772 6170 7065 7220  toctree-wrapper 
-00004280: 636f 6d70 6f75 6e64 223e 0a3c 756c 3e0a  compound">.<ul>.
-00004290: 3c6c 6920 636c 6173 733d 2274 6f63 7472  <li class="toctr
-000042a0: 6565 2d6c 3122 3e3c 6120 636c 6173 733d  ee-l1"><a class=
-000042b0: 2272 6566 6572 656e 6365 2069 6e74 6572  "reference inter
-000042c0: 6e61 6c22 2068 7265 663d 2268 7474 703a  nal" href="http:
-000042d0: 2f2f 6363 622e 6a68 752e 6564 752f 6c69  //ccb.jhu.edu/li
-000042e0: 6674 6f6e 2f63 6f6e 7465 6e74 2f69 6e73  fton/content/ins
-000042f0: 7461 6c6c 6174 696f 6e2e 6874 6d6c 223e  tallation.html">
-00004300: 496e 7374 616c 6c61 7469 6f6e 3c2f 613e  Installation</a>
-00004310: 3c75 6c3e 0a3c 6c69 2063 6c61 7373 3d22  <ul>.<li class="
-00004320: 746f 6374 7265 652d 6c32 223e 3c61 2063  toctree-l2"><a c
-00004330: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
-00004340: 696e 7465 726e 616c 2220 6872 6566 3d22  internal" href="
-00004350: 6874 7470 3a2f 2f63 6362 2e6a 6875 2e65  http://ccb.jhu.e
-00004360: 6475 2f6c 6966 746f 6e2f 636f 6e74 656e  du/lifton/conten
-00004370: 742f 696e 7374 616c 6c61 7469 6f6e 2e68  t/installation.h
-00004380: 746d 6c23 7379 7374 656d 2d72 6571 7569  tml#system-requi
-00004390: 7265 6d65 6e74 7322 3e53 7973 7465 6d20  rements">System 
-000043a0: 7265 7175 6972 656d 656e 7473 3c2f 613e  requirements</a>
-000043b0: 3c2f 6c69 3e0a 3c6c 6920 636c 6173 733d  </li>.<li class=
-000043c0: 2274 6f63 7472 6565 2d6c 3222 3e3c 6120  "toctree-l2"><a 
-000043d0: 636c 6173 733d 2272 6566 6572 656e 6365  class="reference
-000043e0: 2069 6e74 6572 6e61 6c22 2068 7265 663d   internal" href=
-000043f0: 2268 7474 703a 2f2f 6363 622e 6a68 752e  "http://ccb.jhu.
-00004400: 6564 752f 6c69 6674 6f6e 2f63 6f6e 7465  edu/lifton/conte
-00004410: 6e74 2f69 6e73 7461 6c6c 6174 696f 6e2e  nt/installation.
-00004420: 6874 6d6c 2369 6e73 7461 6c6c 2d74 6872  html#install-thr
-00004430: 6f75 6768 2d70 6970 223e 496e 7374 616c  ough-pip">Instal
-00004440: 6c20 7468 726f 7567 6820 7069 703c 2f61  l through pip</a
-00004450: 3e3c 2f6c 693e 0a3c 6c69 2063 6c61 7373  ></li>.<li class
-00004460: 3d22 746f 6374 7265 652d 6c32 223e 3c61  ="toctree-l2"><a
-00004470: 2063 6c61 7373 3d22 7265 6665 7265 6e63   class="referenc
-00004480: 6520 696e 7465 726e 616c 2220 6872 6566  e internal" href
-00004490: 3d22 6874 7470 3a2f 2f63 6362 2e6a 6875  ="http://ccb.jhu
-000044a0: 2e65 6475 2f6c 6966 746f 6e2f 636f 6e74  .edu/lifton/cont
-000044b0: 656e 742f 696e 7374 616c 6c61 7469 6f6e  ent/installation
-000044c0: 2e68 746d 6c23 696e 7374 616c 6c2d 7468  .html#install-th
-000044d0: 726f 7567 682d 636f 6e64 6122 3e49 6e73  rough-conda">Ins
-000044e0: 7461 6c6c 2074 6872 6f75 6768 2063 6f6e  tall through con
-000044f0: 6461 3c2f 613e 3c2f 6c69 3e0a 3c6c 6920  da</a></li>.<li 
-00004500: 636c 6173 733d 2274 6f63 7472 6565 2d6c  class="toctree-l
-00004510: 3222 3e3c 6120 636c 6173 733d 2272 6566  2"><a class="ref
-00004520: 6572 656e 6365 2069 6e74 6572 6e61 6c22  erence internal"
-00004530: 2068 7265 663d 2268 7474 703a 2f2f 6363   href="http://cc
-00004540: 622e 6a68 752e 6564 752f 6c69 6674 6f6e  b.jhu.edu/lifton
-00004550: 2f63 6f6e 7465 6e74 2f69 6e73 7461 6c6c  /content/install
-00004560: 6174 696f 6e2e 6874 6d6c 2369 6e73 7461  ation.html#insta
-00004570: 6c6c 2d66 726f 6d2d 736f 7572 6365 223e  ll-from-source">
-00004580: 496e 7374 616c 6c20 6672 6f6d 2073 6f75  Install from sou
-00004590: 7263 653c 2f61 3e3c 2f6c 693e 0a3c 6c69  rce</a></li>.<li
-000045a0: 2063 6c61 7373 3d22 746f 6374 7265 652d   class="toctree-
-000045b0: 6c32 223e 3c61 2063 6c61 7373 3d22 7265  l2"><a class="re
-000045c0: 6665 7265 6e63 6520 696e 7465 726e 616c  ference internal
-000045d0: 2220 6872 6566 3d22 6874 7470 3a2f 2f63  " href="http://c
-000045e0: 6362 2e6a 6875 2e65 6475 2f6c 6966 746f  cb.jhu.edu/lifto
-000045f0: 6e2f 636f 6e74 656e 742f 696e 7374 616c  n/content/instal
-00004600: 6c61 7469 6f6e 2e68 746d 6c23 6368 6563  lation.html#chec
-00004610: 6b2d 6c69 6674 6f6e 2d69 6e73 7461 6c6c  k-lifton-install
-00004620: 6174 696f 6e22 3e43 6865 636b 204c 6966  ation">Check Lif
-00004630: 744f 6e20 696e 7374 616c 6c61 7469 6f6e  tOn installation
-00004640: 3c2f 613e 3c2f 6c69 3e0a 3c6c 6920 636c  </a></li>.<li cl
-00004650: 6173 733d 2274 6f63 7472 6565 2d6c 3222  ass="toctree-l2"
-00004660: 3e3c 6120 636c 6173 733d 2272 6566 6572  ><a class="refer
-00004670: 656e 6365 2069 6e74 6572 6e61 6c22 2068  ence internal" h
-00004680: 7265 663d 2268 7474 703a 2f2f 6363 622e  ref="http://ccb.
-00004690: 6a68 752e 6564 752f 6c69 6674 6f6e 2f63  jhu.edu/lifton/c
-000046a0: 6f6e 7465 6e74 2f69 6e73 7461 6c6c 6174  ontent/installat
-000046b0: 696f 6e2e 6874 6d6c 236e 6f77 2d79 6f75  ion.html#now-you
-000046c0: 2d61 7265 2d72 6561 6479 2d74 6f2d 676f  -are-ready-to-go
-000046d0: 223e 4e6f 772c 2079 6f75 2061 7265 2072  ">Now, you are r
-000046e0: 6561 6479 2074 6f20 676f 2021 3c2f 613e  eady to go !</a>
-000046f0: 3c2f 6c69 3e0a 3c2f 756c 3e0a 3c2f 6c69  </li>.</ul>.</li
-00004700: 3e0a 3c6c 6920 636c 6173 733d 2274 6f63  >.<li class="toc
-00004710: 7472 6565 2d6c 3122 3e3c 6120 636c 6173  tree-l1"><a clas
-00004720: 733d 2272 6566 6572 656e 6365 2069 6e74  s="reference int
-00004730: 6572 6e61 6c22 2068 7265 663d 2268 7474  ernal" href="htt
-00004740: 703a 2f2f 6363 622e 6a68 752e 6564 752f  p://ccb.jhu.edu/
-00004750: 6c69 6674 6f6e 2f63 6f6e 7465 6e74 2f71  lifton/content/q
-00004760: 7569 636b 7374 6172 742e 6874 6d6c 223e  uickstart.html">
-00004770: 5175 6963 6b20 5374 6172 7420 4775 6964  Quick Start Guid
-00004780: 653c 2f61 3e3c 756c 3e0a 3c6c 6920 636c  e</a><ul>.<li cl
-00004790: 6173 733d 2274 6f63 7472 6565 2d6c 3222  ass="toctree-l2"
-000047a0: 3e3c 6120 636c 6173 733d 2272 6566 6572  ><a class="refer
-000047b0: 656e 6365 2069 6e74 6572 6e61 6c22 2068  ence internal" h
-000047c0: 7265 663d 2268 7474 703a 2f2f 6363 622e  ref="http://ccb.
-000047d0: 6a68 752e 6564 752f 6c69 6674 6f6e 2f63  jhu.edu/lifton/c
-000047e0: 6f6e 7465 6e74 2f71 7569 636b 7374 6172  ontent/quickstar
-000047f0: 742e 6874 6d6c 2373 7570 6572 2d71 7569  t.html#super-qui
-00004800: 636b 2d73 7461 7274 2d6f 6e65 2d6c 696e  ck-start-one-lin
-00004810: 6572 223e 5375 7065 722d 5175 6963 6b20  er">Super-Quick 
-00004820: 5374 6172 7420 286f 6e65 2d6c 696e 6572  Start (one-liner
-00004830: 293c 2f61 3e3c 2f6c 693e 0a3c 6c69 2063  )</a></li>.<li c
-00004840: 6c61 7373 3d22 746f 6374 7265 652d 6c32  lass="toctree-l2
-00004850: 223e 3c61 2063 6c61 7373 3d22 7265 6665  "><a class="refe
-00004860: 7265 6e63 6520 696e 7465 726e 616c 2220  rence internal" 
-00004870: 6872 6566 3d22 6874 7470 3a2f 2f63 6362  href="http://ccb
-00004880: 2e6a 6875 2e65 6475 2f6c 6966 746f 6e2f  .jhu.edu/lifton/
-00004890: 636f 6e74 656e 742f 7175 6963 6b73 7461  content/quicksta
-000048a0: 7274 2e68 746d 6c23 7472 792d 6c69 6674  rt.html#try-lift
-000048b0: 6f6e 2d6f 6e2d 676f 6f67 6c65 2d63 6f6c  on-on-google-col
-000048c0: 6162 223e 5472 7920 4c69 6674 4f6e 206f  ab">Try LiftOn o
-000048d0: 6e20 476f 6f67 6c65 2043 6f6c 6162 3c2f  n Google Colab</
-000048e0: 613e 3c2f 6c69 3e0a 3c2f 756c 3e0a 3c2f  a></li>.</ul>.</
-000048f0: 6c69 3e0a 3c2f 756c 3e0a 3c2f 6469 763e  li>.</ul>.</div>
-00004900: 0a3c 6469 7620 636c 6173 733d 2274 6f63  .<div class="toc
-00004910: 7472 6565 2d77 7261 7070 6572 2063 6f6d  tree-wrapper com
-00004920: 706f 756e 6422 3e0a 3c70 2063 6c61 7373  pound">.<p class
-00004930: 3d22 6361 7074 696f 6e22 2072 6f6c 653d  ="caption" role=
-00004940: 2268 6561 6469 6e67 223e 3c73 7061 6e20  "heading"><span 
-00004950: 636c 6173 733d 2263 6170 7469 6f6e 2d74  class="caption-t
-00004960: 6578 7422 3e45 7861 6d70 6c65 733c 2f73  ext">Examples</s
-00004970: 7061 6e3e 3c2f 703e 0a3c 756c 3e0a 3c6c  pan></p>.<ul>.<l
-00004980: 6920 636c 6173 733d 2274 6f63 7472 6565  i class="toctree
-00004990: 2d6c 3122 3e3c 6120 636c 6173 733d 2272  -l1"><a class="r
-000049a0: 6566 6572 656e 6365 2069 6e74 6572 6e61  eference interna
-000049b0: 6c22 2068 7265 663d 2268 7474 703a 2f2f  l" href="http://
-000049c0: 6363 622e 6a68 752e 6564 752f 6c69 6674  ccb.jhu.edu/lift
-000049d0: 6f6e 2f63 6f6e 7465 6e74 2f73 616d 655f  on/content/same_
-000049e0: 7370 6563 6965 735f 6c69 6674 6f76 6572  species_liftover
-000049f0: 2f69 6e64 6578 2e68 746d 6c22 3e53 616d  /index.html">Sam
-00004a00: 6520 7370 6563 6965 7320 6c69 6674 2d6f  e species lift-o
-00004a10: 7665 723c 2f61 3e3c 2f6c 693e 0a3c 6c69  ver</a></li>.<li
-00004a20: 2063 6c61 7373 3d22 746f 6374 7265 652d   class="toctree-
-00004a30: 6c31 223e 3c61 2063 6c61 7373 3d22 7265  l1"><a class="re
-00004a40: 6665 7265 6e63 6520 696e 7465 726e 616c  ference internal
-00004a50: 2220 6872 6566 3d22 6874 7470 3a2f 2f63  " href="http://c
-00004a60: 6362 2e6a 6875 2e65 6475 2f6c 6966 746f  cb.jhu.edu/lifto
-00004a70: 6e2f 636f 6e74 656e 742f 636c 6f73 655f  n/content/close_
-00004a80: 7370 6563 6965 735f 6c69 6674 6f76 6572  species_liftover
-00004a90: 2f69 6e64 6578 2e68 746d 6c22 3e43 6c6f  /index.html">Clo
-00004aa0: 7365 6c79 2d72 656c 6174 6564 2073 7065  sely-related spe
-00004ab0: 6369 6573 206c 6966 742d 6f76 6572 3c2f  cies lift-over</
-00004ac0: 613e 3c2f 6c69 3e0a 3c6c 6920 636c 6173  a></li>.<li clas
-00004ad0: 733d 2274 6f63 7472 6565 2d6c 3122 3e3c  s="toctree-l1"><
-00004ae0: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
-00004af0: 6365 2069 6e74 6572 6e61 6c22 2068 7265  ce internal" hre
-00004b00: 663d 2268 7474 703a 2f2f 6363 622e 6a68  f="http://ccb.jh
-00004b10: 752e 6564 752f 6c69 6674 6f6e 2f63 6f6e  u.edu/lifton/con
-00004b20: 7465 6e74 2f64 6973 7461 6e74 5f73 7065  tent/distant_spe
-00004b30: 6369 6573 5f6c 6966 746f 7665 722f 696e  cies_liftover/in
-00004b40: 6465 782e 6874 6d6c 223e 4469 7374 616e  dex.html">Distan
-00004b50: 7420 7370 6563 6965 7320 6c69 6674 2d6f  t species lift-o
-00004b60: 7665 723c 2f61 3e3c 2f6c 693e 0a3c 2f75  ver</a></li>.</u
-00004b70: 6c3e 0a3c 2f64 6976 3e0a 3c64 6976 2063  l>.</div>.<div c
-00004b80: 6c61 7373 3d22 746f 6374 7265 652d 7772  lass="toctree-wr
-00004b90: 6170 7065 7220 636f 6d70 6f75 6e64 223e  apper compound">
-00004ba0: 0a3c 7020 636c 6173 733d 2263 6170 7469  .<p class="capti
-00004bb0: 6f6e 2220 726f 6c65 3d22 6865 6164 696e  on" role="headin
-00004bc0: 6722 3e3c 7370 616e 2063 6c61 7373 3d22  g"><span class="
-00004bd0: 6361 7074 696f 6e2d 7465 7874 223e 496e  caption-text">In
-00004be0: 666f 3c2f 7370 616e 3e3c 2f70 3e0a 3c75  fo</span></p>.<u
-00004bf0: 6c3e 0a3c 6c69 2063 6c61 7373 3d22 746f  l>.<li class="to
-00004c00: 6374 7265 652d 6c31 223e 3c61 2063 6c61  ctree-l1"><a cla
-00004c10: 7373 3d22 7265 6665 7265 6e63 6520 696e  ss="reference in
-00004c20: 7465 726e 616c 2220 6872 6566 3d22 6874  ternal" href="ht
-00004c30: 7470 3a2f 2f63 6362 2e6a 6875 2e65 6475  tp://ccb.jhu.edu
-00004c40: 2f6c 6966 746f 6e2f 636f 6e74 656e 742f  /lifton/content/
-00004c50: 6f75 7470 7574 5f65 7870 6c61 6e61 7469  output_explanati
-00004c60: 6f6e 2e68 746d 6c22 3e4f 7574 7075 7420  on.html">Output 
-00004c70: 6669 6c65 733c 2f61 3e3c 756c 3e0a 3c6c  files</a><ul>.<l
-00004c80: 6920 636c 6173 733d 2274 6f63 7472 6565  i class="toctree
-00004c90: 2d6c 3222 3e3c 6120 636c 6173 733d 2272  -l2"><a class="r
-00004ca0: 6566 6572 656e 6365 2069 6e74 6572 6e61  eference interna
-00004cb0: 6c22 2068 7265 663d 2268 7474 703a 2f2f  l" href="http://
-00004cc0: 6363 622e 6a68 752e 6564 752f 6c69 6674  ccb.jhu.edu/lift
-00004cd0: 6f6e 2f63 6f6e 7465 6e74 2f6f 7574 7075  on/content/outpu
-00004ce0: 745f 6578 706c 616e 6174 696f 6e2e 6874  t_explanation.ht
-00004cf0: 6d6c 236c 6966 746f 6e2d 6766 6633 223e  ml#lifton-gff3">
-00004d00: 6c69 6674 6f6e 2e47 4646 333c 2f61 3e3c  lifton.GFF3</a><
-00004d10: 2f6c 693e 0a3c 6c69 2063 6c61 7373 3d22  /li>.<li class="
-00004d20: 746f 6374 7265 652d 6c32 223e 3c61 2063  toctree-l2"><a c
-00004d30: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
-00004d40: 696e 7465 726e 616c 2220 6872 6566 3d22  internal" href="
-00004d50: 6874 7470 3a2f 2f63 6362 2e6a 6875 2e65  http://ccb.jhu.e
-00004d60: 6475 2f6c 6966 746f 6e2f 636f 6e74 656e  du/lifton/conten
-00004d70: 742f 6f75 7470 7574 5f65 7870 6c61 6e61  t/output_explana
-00004d80: 7469 6f6e 2e68 746d 6c23 6c69 6674 6f6e  tion.html#lifton
-00004d90: 2d6f 7574 7075 7422 3e6c 6966 746f 6e5f  -output">lifton_
-00004da0: 6f75 7470 7574 2f3c 2f61 3e3c 2f6c 693e  output/</a></li>
-00004db0: 0a3c 2f75 6c3e 0a3c 2f6c 693e 0a3c 6c69  .</ul>.</li>.<li
-00004dc0: 2063 6c61 7373 3d22 746f 6374 7265 652d   class="toctree-
-00004dd0: 6c31 223e 3c61 2063 6c61 7373 3d22 7265  l1"><a class="re
-00004de0: 6665 7265 6e63 6520 696e 7465 726e 616c  ference internal
-00004df0: 2220 6872 6566 3d22 6874 7470 3a2f 2f63  " href="http://c
-00004e00: 6362 2e6a 6875 2e65 6475 2f6c 6966 746f  cb.jhu.edu/lifto
-00004e10: 6e2f 636f 6e74 656e 742f 6265 6869 6e64  n/content/behind
-00004e20: 5f73 6365 6e65 732e 6874 6d6c 223e 4265  _scenes.html">Be
-00004e30: 6869 6e64 2074 6865 2073 6365 6e65 733c  hind the scenes<
-00004e40: 2f61 3e3c 756c 3e0a 3c6c 6920 636c 6173  /a><ul>.<li clas
-00004e50: 733d 2274 6f63 7472 6565 2d6c 3222 3e3c  s="toctree-l2"><
-00004e60: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
-00004e70: 6365 2069 6e74 6572 6e61 6c22 2068 7265  ce internal" hre
-00004e80: 663d 2268 7474 703a 2f2f 6363 622e 6a68  f="http://ccb.jh
-00004e90: 752e 6564 752f 6c69 6674 6f6e 2f63 6f6e  u.edu/lifton/con
-00004ea0: 7465 6e74 2f62 6568 696e 645f 7363 656e  tent/behind_scen
-00004eb0: 6573 2e68 746d 6c23 6d61 7463 6869 6e67  es.html#matching
-00004ec0: 2d6d 696e 6970 726f 742d 6c69 6674 6f66  -miniprot-liftof
-00004ed0: 662d 6765 6e6f 6d65 2d61 6e6e 6f74 6174  f-genome-annotat
-00004ee0: 696f 6e22 3e4d 6174 6368 696e 6720 6d69  ion">Matching mi
-00004ef0: 6e69 7072 6f74 2026 616d 703b 204c 6966  niprot &amp; Lif
-00004f00: 746f 6666 2067 656e 6f6d 6520 616e 6e6f  toff genome anno
-00004f10: 7461 7469 6f6e 3c2f 613e 3c2f 6c69 3e0a  tation</a></li>.
-00004f20: 3c6c 6920 636c 6173 733d 2274 6f63 7472  <li class="toctr
-00004f30: 6565 2d6c 3222 3e3c 6120 636c 6173 733d  ee-l2"><a class=
-00004f40: 2272 6566 6572 656e 6365 2069 6e74 6572  "reference inter
-00004f50: 6e61 6c22 2068 7265 663d 2268 7474 703a  nal" href="http:
-00004f60: 2f2f 6363 622e 6a68 752e 6564 752f 6c69  //ccb.jhu.edu/li
-00004f70: 6674 6f6e 2f63 6f6e 7465 6e74 2f62 6568  fton/content/beh
-00004f80: 696e 645f 7363 656e 6573 2e68 746d 6c23  ind_scenes.html#
-00004f90: 7072 6f74 6569 6e2d 6d61 7869 6d69 7a61  protein-maximiza
-00004fa0: 7469 6f6e 2d61 6c67 6f72 6974 686d 223e  tion-algorithm">
-00004fb0: 3c65 6d3e 5072 6f74 6569 6e2d 6d61 7869  <em>Protein-maxi
-00004fc0: 6d69 7a61 7469 6f6e 2061 6c67 6f72 6974  mization algorit
-00004fd0: 686d 3c2f 656d 3e3c 2f61 3e3c 2f6c 693e  hm</em></a></li>
-00004fe0: 0a3c 6c69 2063 6c61 7373 3d22 746f 6374  .<li class="toct
-00004ff0: 7265 652d 6c32 223e 3c61 2063 6c61 7373  ree-l2"><a class
-00005000: 3d22 7265 6665 7265 6e63 6520 696e 7465  ="reference inte
-00005010: 726e 616c 2220 6872 6566 3d22 6874 7470  rnal" href="http
-00005020: 3a2f 2f63 6362 2e6a 6875 2e65 6475 2f6c  ://ccb.jhu.edu/l
-00005030: 6966 746f 6e2f 636f 6e74 656e 742f 6265  ifton/content/be
-00005040: 6869 6e64 5f73 6365 6e65 732e 6874 6d6c  hind_scenes.html
-00005050: 236d 7574 6174 696f 6e2d 7265 706f 7274  #mutation-report
-00005060: 223e 4d75 7461 7469 6f6e 2072 6570 6f72  ">Mutation repor
-00005070: 743c 2f61 3e3c 2f6c 693e 0a3c 6c69 2063  t</a></li>.<li c
-00005080: 6c61 7373 3d22 746f 6374 7265 652d 6c32  lass="toctree-l2
-00005090: 223e 3c61 2063 6c61 7373 3d22 7265 6665  "><a class="refe
-000050a0: 7265 6e63 6520 696e 7465 726e 616c 2220  rence internal" 
-000050b0: 6872 6566 3d22 6874 7470 3a2f 2f63 6362  href="http://ccb
-000050c0: 2e6a 6875 2e65 6475 2f6c 6966 746f 6e2f  .jhu.edu/lifton/
-000050d0: 636f 6e74 656e 742f 6265 6869 6e64 5f73  content/behind_s
-000050e0: 6365 6e65 732e 6874 6d6c 236f 7065 6e2d  cenes.html#open-
-000050f0: 7265 6164 696e 672d 6672 616d 652d 7365  reading-frame-se
-00005100: 6172 6368 223e 4f70 656e 2d72 6561 6469  arch">Open-readi
-00005110: 6e67 2d66 7261 6d65 2073 6561 7263 683c  ng-frame search<
-00005120: 2f61 3e3c 2f6c 693e 0a3c 6c69 2063 6c61  /a></li>.<li cla
-00005130: 7373 3d22 746f 6374 7265 652d 6c32 223e  ss="toctree-l2">
-00005140: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
-00005150: 6e63 6520 696e 7465 726e 616c 2220 6872  nce internal" hr
-00005160: 6566 3d22 6874 7470 3a2f 2f63 6362 2e6a  ef="http://ccb.j
-00005170: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
-00005180: 6e74 656e 742f 6265 6869 6e64 5f73 6365  ntent/behind_sce
-00005190: 6e65 732e 6874 6d6c 2364 6e61 2d70 726f  nes.html#dna-pro
-000051a0: 7465 696e 2d74 7261 6e73 6372 6970 742d  tein-transcript-
-000051b0: 7365 7175 656e 6365 2d69 6465 6e74 6974  sequence-identit
-000051c0: 792d 7363 6f72 652d 6361 6c63 756c 6174  y-score-calculat
-000051d0: 696f 6e22 3e44 4e41 2026 616d 703b 2070  ion">DNA &amp; p
-000051e0: 726f 7465 696e 2074 7261 6e73 6372 6970  rotein transcrip
-000051f0: 7420 7365 7175 656e 6365 2069 6465 6e74  t sequence ident
-00005200: 6974 7920 7363 6f72 6520 6361 6c63 756c  ity score calcul
-00005210: 6174 696f 6e3c 2f61 3e3c 2f6c 693e 0a3c  ation</a></li>.<
-00005220: 6c69 2063 6c61 7373 3d22 746f 6374 7265  li class="toctre
-00005230: 652d 6c32 223e 3c61 2063 6c61 7373 3d22  e-l2"><a class="
-00005240: 7265 6665 7265 6e63 6520 696e 7465 726e  reference intern
-00005250: 616c 2220 6872 6566 3d22 6874 7470 3a2f  al" href="http:/
-00005260: 2f63 6362 2e6a 6875 2e65 6475 2f6c 6966  /ccb.jhu.edu/lif
-00005270: 746f 6e2f 636f 6e74 656e 742f 6265 6869  ton/content/behi
-00005280: 6e64 5f73 6365 6e65 732e 6874 6d6c 2372  nd_scenes.html#r
-00005290: 6566 6572 656e 6365 223e 5265 6665 7265  eference">Refere
-000052a0: 6e63 653c 2f61 3e3c 2f6c 693e 0a3c 2f75  nce</a></li>.</u
-000052b0: 6c3e 0a3c 2f6c 693e 0a3c 6c69 2063 6c61  l>.</li>.<li cla
-000052c0: 7373 3d22 746f 6374 7265 652d 6c31 223e  ss="toctree-l1">
-000052d0: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
-000052e0: 6e63 6520 696e 7465 726e 616c 2220 6872  nce internal" hr
-000052f0: 6566 3d22 6874 7470 3a2f 2f63 6362 2e6a  ef="http://ccb.j
-00005300: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
-00005310: 6e74 656e 742f 686f 775f 746f 5f70 6167  ntent/how_to_pag
-00005320: 652e 6874 6d6c 223e 5120 2661 6d70 3b20  e.html">Q &amp; 
-00005330: 4120 2e2e 2e3c 2f61 3e3c 2f6c 693e 0a3c  A ...</a></li>.<
-00005340: 6c69 2063 6c61 7373 3d22 746f 6374 7265  li class="toctre
-00005350: 652d 6c31 223e 3c61 2063 6c61 7373 3d22  e-l1"><a class="
-00005360: 7265 6665 7265 6e63 6520 696e 7465 726e  reference intern
-00005370: 616c 2220 6872 6566 3d22 6874 7470 3a2f  al" href="http:/
-00005380: 2f63 6362 2e6a 6875 2e65 6475 2f6c 6966  /ccb.jhu.edu/lif
-00005390: 746f 6e2f 636f 6e74 656e 742f 6675 6e63  ton/content/func
-000053a0: 7469 6f6e 5f6d 616e 7561 6c2e 6874 6d6c  tion_manual.html
-000053b0: 223e 5573 6572 204d 616e 7561 6c3c 2f61  ">User Manual</a
-000053c0: 3e3c 756c 3e0a 3c6c 6920 636c 6173 733d  ><ul>.<li class=
-000053d0: 2274 6f63 7472 6565 2d6c 3222 3e3c 6120  "toctree-l2"><a 
-000053e0: 636c 6173 733d 2272 6566 6572 656e 6365  class="reference
-000053f0: 2069 6e74 6572 6e61 6c22 2068 7265 663d   internal" href=
-00005400: 2268 7474 703a 2f2f 6363 622e 6a68 752e  "http://ccb.jhu.
-00005410: 6564 752f 6c69 6674 6f6e 2f63 6f6e 7465  edu/lifton/conte
-00005420: 6e74 2f66 756e 6374 696f 6e5f 6d61 6e75  nt/function_manu
-00005430: 616c 2e68 746d 6c23 7370 6c61 6d22 3e73  al.html#splam">s
-00005440: 706c 616d 3c2f 613e 3c2f 6c69 3e0a 3c2f  plam</a></li>.</
-00005450: 756c 3e0a 3c2f 6c69 3e0a 3c6c 6920 636c  ul>.</li>.<li cl
-00005460: 6173 733d 2274 6f63 7472 6565 2d6c 3122  ass="toctree-l1"
-00005470: 3e3c 6120 636c 6173 733d 2272 6566 6572  ><a class="refer
-00005480: 656e 6365 2069 6e74 6572 6e61 6c22 2068  ence internal" h
-00005490: 7265 663d 2268 7474 703a 2f2f 6363 622e  ref="http://ccb.
-000054a0: 6a68 752e 6564 752f 6c69 6674 6f6e 2f63  jhu.edu/lifton/c
-000054b0: 6f6e 7465 6e74 2f63 6861 6e67 656c 6f67  ontent/changelog
-000054c0: 2e68 746d 6c22 3e43 6861 6e67 656c 6f67  .html">Changelog
-000054d0: 3c2f 613e 3c75 6c3e 0a3c 6c69 2063 6c61  </a><ul>.<li cla
-000054e0: 7373 3d22 746f 6374 7265 652d 6c32 223e  ss="toctree-l2">
-000054f0: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
-00005500: 6e63 6520 696e 7465 726e 616c 2220 6872  nce internal" hr
-00005510: 6566 3d22 6874 7470 3a2f 2f63 6362 2e6a  ef="http://ccb.j
-00005520: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
-00005530: 6e74 656e 742f 6368 616e 6765 6c6f 672e  ntent/changelog.
-00005540: 6874 6d6c 2376 312d 302d 3022 3e76 312e  html#v1-0-0">v1.
-00005550: 302e 303c 2f61 3e3c 2f6c 693e 0a3c 2f75  0.0</a></li>.</u
-00005560: 6c3e 0a3c 2f6c 693e 0a3c 6c69 2063 6c61  l>.</li>.<li cla
-00005570: 7373 3d22 746f 6374 7265 652d 6c31 223e  ss="toctree-l1">
-00005580: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
-00005590: 6e63 6520 696e 7465 726e 616c 2220 6872  nce internal" hr
-000055a0: 6566 3d22 6874 7470 3a2f 2f63 6362 2e6a  ef="http://ccb.j
-000055b0: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
-000055c0: 6e74 656e 742f 6c69 6365 6e73 652e 6874  ntent/license.ht
-000055d0: 6d6c 223e 4c69 6365 6e73 653c 2f61 3e3c  ml">License</a><
-000055e0: 2f6c 693e 0a3c 6c69 2063 6c61 7373 3d22  /li>.<li class="
-000055f0: 746f 6374 7265 652d 6c31 223e 3c61 2063  toctree-l1"><a c
-00005600: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
-00005610: 696e 7465 726e 616c 2220 6872 6566 3d22  internal" href="
-00005620: 6874 7470 3a2f 2f63 6362 2e6a 6875 2e65  http://ccb.jhu.e
-00005630: 6475 2f6c 6966 746f 6e2f 636f 6e74 656e  du/lifton/conten
-00005640: 742f 636f 6e74 6163 742e 6874 6d6c 223e  t/contact.html">
-00005650: 436f 6e74 6163 743c 2f61 3e3c 2f6c 693e  Contact</a></li>
-00005660: 0a3c 2f75 6c3e 0a3c 2f64 6976 3e0a 3c2f  .</ul>.</div>.</
-00005670: 7365 6374 696f 6e3e 0a3c 2f73 6563 7469  section>.</secti
-00005680: 6f6e 3e0a 0a3c 6272 3e0a 0a23 2320 3c61  on>..<br>..## <a
-00005690: 206e 616d 653d 2263 6974 6174 696f 6e22   name="citation"
-000056a0: 3e3c 2f61 3e43 6974 6174 696f 6e3c 6120  ></a>Citation<a 
-000056b0: 636c 6173 733d 2268 6561 6465 726c 696e  class="headerlin
-000056c0: 6b22 2068 7265 663d 2223 6369 7461 7469  k" href="#citati
-000056d0: 6f6e 2220 7469 746c 653d 2250 6572 6d61  on" title="Perma
-000056e0: 6c69 6e6b 2074 6f20 7468 6973 2068 6561  link to this hea
-000056f0: 6469 6e67 223e 233c 2f61 3e0a 0a0a 4b75  ding">#</a>...Ku
-00005700: 616e 2d48 616f 2043 6861 6f2a 2c20 4d69  an-Hao Chao*, Mi
-00005710: 6861 656c 6120 5065 7274 6561 2c20 5374  haela Pertea, St
-00005720: 6576 656e 204c 2053 616c 7a62 6572 672a  even L Salzberg*
-00005730: 2c20 224c 6966 744f 6e3a 2061 2074 6f6f  , "LiftOn: a too
-00005740: 6c20 746f 2069 6d70 726f 7665 2061 6e6e  l to improve ann
-00005750: 6f74 6174 696f 6e73 2066 6f72 2070 726f  otations for pro
-00005760: 7465 696e 2d63 6f64 696e 6720 6765 6e65  tein-coding gene
-00005770: 7320 6475 7269 6e67 2074 6865 206c 6966  s during the lif
-00005780: 742d 6f76 6572 2070 726f 6365 7373 2e22  t-over process."
-00005790: 2c20 3c69 3e62 696f 5278 6976 3c2f 693e  , <i>bioRxiv</i>
-000057a0: 203c 623e 3230 3233 2e30 372e 3237 2e35   <b>2023.07.27.5
-000057b0: 3530 3735 343c 2f62 3e2c 2064 6f69 3a20  50754</b>, doi: 
-000057c0: 5b68 7474 7073 3a2f 2f64 6f69 2e6f 7267  [https://doi.org
-000057d0: 2f31 302e 3131 3031 2f32 3032 332e 3037  /10.1101/2023.07
-000057e0: 2e32 372e 3535 3037 3534 5d28 6874 7470  .27.550754](http
-000057f0: 733a 2f2f 646f 692e 6f72 672f 3130 2e31  s://doi.org/10.1
-00005800: 3130 312f 3230 3233 2e30 372e 3237 2e35  101/2023.07.27.5
-00005810: 3530 3735 3429 2c20 3230 3233 0a0a 3c62  50754), 2023..<b
-00005820: 723e 0a3c 6272 3e0a 3c62 723e 0a0a 3c69  r>.<br>.<br>..<i
-00005830: 6d67 2061 6c74 3d22 4d79 204c 6f67 6f22  mg alt="My Logo"
-00005840: 2063 6c61 7373 3d22 6c6f 676f 2068 6561   class="logo hea
-00005850: 6465 722d 696d 6167 6520 6f6e 6c79 2d6c  der-image only-l
-00005860: 6967 6874 2061 6c69 676e 2d63 656e 7465  ight align-cente
-00005870: 7222 2073 7263 3d22 6772 6170 6869 6373  r" src="graphics
-00005880: 2f6a 6875 2d6c 6f67 6f2d 6461 726b 2e70  /jhu-logo-dark.p
-00005890: 6e67 223e 0a                             ng">.
+00000020: 6f6e 0a56 6572 7369 6f6e 3a20 312e 302e  on.Version: 1.0.
+00000030: 300a 5375 6d6d 6172 793a 2043 6f6d 6269  0.Summary: Combi
+00000040: 6e69 6e67 2044 4e41 2061 6e64 2070 726f  ning DNA and pro
+00000050: 7465 696e 2061 6c69 676e 6d65 6e74 7320  tein alignments 
+00000060: 746f 2069 6d70 726f 7665 2067 656e 6f6d  to improve genom
+00000070: 6520 616e 6e6f 7461 7469 6f6e 2077 6974  e annotation wit
+00000080: 6820 4c69 6674 4f6e 0a48 6f6d 652d 7061  h LiftOn.Home-pa
+00000090: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
+000000a0: 7562 2e63 6f6d 2f4b 7561 6e68 616f 2d43  ub.com/Kuanhao-C
+000000b0: 6861 6f2f 4c69 6674 6f6e 0a41 7574 686f  hao/Lifton.Autho
+000000c0: 723a 204b 7561 6e2d 4861 6f20 4368 616f  r: Kuan-Hao Chao
+000000d0: 0a41 7574 686f 722d 656d 6169 6c3a 206b  .Author-email: k
+000000e0: 682e 6368 616f 4063 732e 6a68 752e 6564  h.chao@cs.jhu.ed
+000000f0: 750a 5265 7175 6972 6573 2d50 7974 686f  u.Requires-Pytho
+00000100: 6e3a 203e 3d33 2e36 0a44 6573 6372 6970  n: >=3.6.Descrip
+00000110: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
+00000120: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
+00000130: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
+00000140: 4943 454e 5345 0a0a 3c69 6d67 2061 6c74  ICENSE..<img alt
+00000150: 3d22 4d79 204c 6f67 6f22 2063 6c61 7373  ="My Logo" class
+00000160: 3d22 6c6f 676f 2068 6561 6465 722d 696d  ="logo header-im
+00000170: 6167 6520 6f6e 6c79 2d6c 6967 6874 2061  age only-light a
+00000180: 6c69 676e 2d63 656e 7465 7222 2073 7263  lign-center" src
+00000190: 3d22 6874 7470 733a 2f2f 7374 6f72 6167  ="https://storag
+000001a0: 652e 676f 6f67 6c65 6170 6973 2e63 6f6d  e.googleapis.com
+000001b0: 2f73 746f 7261 6765 2e6b 6863 6861 6f2e  /storage.khchao.
+000001c0: 636f 6d2f 6669 6775 7265 732f 4c69 6674  com/figures/Lift
+000001d0: 4f6e 2f4c 6966 744f 6e5f 636f 6c6f 722e  On/LiftOn_color.
+000001e0: 706e 6722 2073 7479 6c65 3d22 7769 6474  png" style="widt
+000001f0: 683a 3930 2522 3e0a 0a3c 6469 7620 636c  h:90%">..<div cl
+00000200: 6173 733d 2263 6f6e 7465 6e74 223e 0a3c  ass="content">.<
+00000210: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
+00000220: 6365 2065 7874 6572 6e61 6c20 696d 6167  ce external imag
+00000230: 652d 7265 6665 7265 6e63 6522 2068 7265  e-reference" hre
+00000240: 663d 2268 7474 7073 3a2f 2f69 6d67 2e73  f="https://img.s
+00000250: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000260: 4c69 6365 6e73 652d 4750 4c76 332d 7965  License-GPLv3-ye
+00000270: 6c6c 6f77 2e73 7667 223e 3c69 6d67 2061  llow.svg"><img a
+00000280: 6c74 3d22 6874 7470 733a 2f2f 696d 672e  lt="https://img.
+00000290: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+000002a0: 2f4c 6963 656e 7365 2d47 504c 7633 2d79  /License-GPLv3-y
+000002b0: 656c 6c6f 772e 7376 6722 2073 7263 3d22  ellow.svg" src="
+000002c0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000002d0: 6c64 732e 696f 2f62 6164 6765 2f4c 6963  lds.io/badge/Lic
+000002e0: 656e 7365 2d47 504c 7633 2d79 656c 6c6f  ense-GPLv3-yello
+000002f0: 772e 7376 6722 3e3c 2f61 3e0a 3c61 2063  w.svg"></a>.<a c
+00000300: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
+00000310: 6578 7465 726e 616c 2069 6d61 6765 2d72  external image-r
+00000320: 6566 6572 656e 6365 2220 6872 6566 3d22  eference" href="
+00000330: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000340: 6c64 732e 696f 2f62 6164 6765 2f76 6572  lds.io/badge/ver
+00000350: 7369 6f6e 2d76 2e30 2e30 2e31 2d62 6c75  sion-v.0.0.1-blu
+00000360: 6522 3e3c 696d 6720 616c 743d 2268 7474  e"><img alt="htt
+00000370: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000380: 2e69 6f2f 6261 6467 652f 7665 7273 696f  .io/badge/versio
+00000390: 6e2d 762e 302e 302e 312d 626c 7565 2220  n-v.0.0.1-blue" 
+000003a0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+000003b0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+000003c0: 652f 7665 7273 696f 6e2d 762e 302e 302e  e/version-v.0.0.
+000003d0: 312d 626c 7565 223e 3c2f 613e 0a3c 6120  1-blue"></a>.<a 
+000003e0: 636c 6173 733d 2272 6566 6572 656e 6365  class="reference
+000003f0: 2065 7874 6572 6e61 6c20 696d 6167 652d   external image-
+00000400: 7265 6665 7265 6e63 6522 2068 7265 663d  reference" href=
+00000410: 2268 7474 7073 3a2f 2f70 6570 792e 7465  "https://pepy.te
+00000420: 6368 2f70 726f 6a65 6374 2f6c 6966 746f  ch/project/lifto
+00000430: 6e22 3e3c 696d 6720 616c 743d 2268 7474  n"><img alt="htt
+00000440: 7073 3a2f 2f73 7461 7469 632e 7065 7079  ps://static.pepy
+00000450: 2e74 6563 682f 7065 7273 6f6e 616c 697a  .tech/personaliz
+00000460: 6564 2d62 6164 6765 2f6c 6966 746f 6e3f  ed-badge/lifton?
+00000470: 7065 7269 6f64 3d74 6f74 616c 2661 6d70  period=total&amp
+00000480: 3b75 6e69 7473 3d61 6262 7265 7669 6174  ;units=abbreviat
+00000490: 696f 6e26 616d 703b 6c65 6674 5f63 6f6c  ion&amp;left_col
+000004a0: 6f72 3d67 7265 7926 616d 703b 7269 6768  or=grey&amp;righ
+000004b0: 745f 636f 6c6f 723d 626c 7565 2661 6d70  t_color=blue&amp
+000004c0: 3b6c 6566 745f 7465 7874 3d50 7950 6925  ;left_text=PyPi%
+000004d0: 3230 646f 776e 6c6f 6164 7322 2073 7263  20downloads" src
+000004e0: 3d22 6874 7470 733a 2f2f 7374 6174 6963  ="https://static
+000004f0: 2e70 6570 792e 7465 6368 2f70 6572 736f  .pepy.tech/perso
+00000500: 6e61 6c69 7a65 642d 6261 6467 652f 6c69  nalized-badge/li
+00000510: 6674 6f6e 3f70 6572 696f 643d 746f 7461  fton?period=tota
+00000520: 6c26 616d 703b 756e 6974 733d 6162 6272  l&amp;units=abbr
+00000530: 6576 6961 7469 6f6e 2661 6d70 3b6c 6566  eviation&amp;lef
+00000540: 745f 636f 6c6f 723d 6772 6579 2661 6d70  t_color=grey&amp
+00000550: 3b72 6967 6874 5f63 6f6c 6f72 3d62 6c75  ;right_color=blu
+00000560: 6526 616d 703b 6c65 6674 5f74 6578 743d  e&amp;left_text=
+00000570: 5079 5069 2532 3064 6f77 6e6c 6f61 6473  PyPi%20downloads
+00000580: 223e 3c2f 613e 0a3c 6120 636c 6173 733d  "></a>.<a class=
+00000590: 2272 6566 6572 656e 6365 2065 7874 6572  "reference exter
+000005a0: 6e61 6c20 696d 6167 652d 7265 6665 7265  nal image-refere
+000005b0: 6e63 6522 2068 7265 663d 2268 7474 7073  nce" href="https
+000005c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4b75  ://github.com/Ku
+000005d0: 616e 6861 6f2d 4368 616f 2f6c 6966 746f  anhao-Chao/lifto
+000005e0: 6e2f 7265 6c65 6173 6573 223e 3c69 6d67  n/releases"><img
+000005f0: 2061 6c74 3d22 6874 7470 733a 2f2f 696d   alt="https://im
+00000600: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+00000610: 6875 622f 646f 776e 6c6f 6164 732f 4b75  hub/downloads/Ku
+00000620: 616e 6861 6f2d 4368 616f 2f6c 6966 746f  anhao-Chao/lifto
+00000630: 6e2f 746f 7461 6c2e 7376 673f 7374 796c  n/total.svg?styl
+00000640: 653d 736f 6369 616c 2661 6d70 3b6c 6f67  e=social&amp;log
+00000650: 6f3d 6769 7468 7562 2661 6d70 3b6c 6162  o=github&amp;lab
+00000660: 656c 3d44 6f77 6e6c 6f61 6422 2073 7263  el=Download" src
+00000670: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000680: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00000690: 646f 776e 6c6f 6164 732f 4b75 616e 6861  downloads/Kuanha
+000006a0: 6f2d 4368 616f 2f6c 6966 746f 6e2f 746f  o-Chao/lifton/to
+000006b0: 7461 6c2e 7376 673f 7374 796c 653d 736f  tal.svg?style=so
+000006c0: 6369 616c 2661 6d70 3b6c 6f67 6f3d 6769  cial&amp;logo=gi
+000006d0: 7468 7562 2661 6d70 3b6c 6162 656c 3d44  thub&amp;label=D
+000006e0: 6f77 6e6c 6f61 6422 3e3c 2f61 3e0a 3c61  ownload"></a>.<a
+000006f0: 2063 6c61 7373 3d22 7265 6665 7265 6e63   class="referenc
+00000700: 6520 6578 7465 726e 616c 2069 6d61 6765  e external image
+00000710: 2d72 6566 6572 656e 6365 2220 6872 6566  -reference" href
+00000720: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000730: 2e63 6f6d 2f4b 7561 6e68 616f 2d43 6861  .com/Kuanhao-Cha
+00000740: 6f2f 6c69 6674 6f6e 2f72 656c 6561 7365  o/lifton/release
+00000750: 7322 3e3c 696d 6720 616c 743d 2268 7474  s"><img alt="htt
+00000760: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000770: 2e69 6f2f 6261 6467 652f 706c 6174 666f  .io/badge/platfo
+00000780: 726d 2d6d 6163 4f53 5f2f 4c69 6e75 782d  rm-macOS_/Linux-
+00000790: 6772 6565 6e2e 7376 6722 2073 7263 3d22  green.svg" src="
+000007a0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000007b0: 6c64 732e 696f 2f62 6164 6765 2f70 6c61  lds.io/badge/pla
+000007c0: 7466 6f72 6d2d 6d61 634f 535f 2f4c 696e  tform-macOS_/Lin
+000007d0: 7578 2d67 7265 656e 2e73 7667 223e 3c2f  ux-green.svg"></
+000007e0: 613e 0a3c 6120 636c 6173 733d 2272 6566  a>.<a class="ref
+000007f0: 6572 656e 6365 2065 7874 6572 6e61 6c20  erence external 
+00000800: 696d 6167 652d 7265 6665 7265 6e63 6522  image-reference"
+00000810: 2068 7265 663d 2268 7474 7073 3a2f 2f63   href="https://c
+00000820: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+00000830: 6f67 6c65 2e63 6f6d 2f67 6974 6875 622f  ogle.com/github/
+00000840: 4b75 616e 6861 6f2d 4368 616f 2f6c 6966  Kuanhao-Chao/lif
+00000850: 746f 6e2f 626c 6f62 2f6d 6169 6e2f 6e6f  ton/blob/main/no
+00000860: 7465 626f 6f6b 2f6c 6966 746f 6e5f 6578  tebook/lifton_ex
+00000870: 616d 706c 652e 6970 796e 6222 3e3c 696d  ample.ipynb"><im
+00000880: 6720 616c 743d 2268 7474 7073 3a2f 2f63  g alt="https://c
+00000890: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+000008a0: 6f67 6c65 2e63 6f6d 2f61 7373 6574 732f  ogle.com/assets/
+000008b0: 636f 6c61 622d 6261 6467 652e 7376 6722  colab-badge.svg"
+000008c0: 2073 7263 3d22 6874 7470 733a 2f2f 636f   src="https://co
+000008d0: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
+000008e0: 676c 652e 636f 6d2f 6173 7365 7473 2f63  gle.com/assets/c
+000008f0: 6f6c 6162 2d62 6164 6765 2e73 7667 223e  olab-badge.svg">
+00000900: 3c2f 613e 0a3c 6469 7620 636c 6173 733d  </a>.<div class=
+00000910: 226c 696e 652d 626c 6f63 6b22 3e0a 3c64  "line-block">.<d
+00000920: 6976 2063 6c61 7373 3d22 6c69 6e65 223e  iv class="line">
+00000930: 3c62 723e 3c2f 6469 763e 0a3c 2f64 6976  <br></div>.</div
+00000940: 3e0a 3c6c 696e 6b20 7265 6c3d 2273 7479  >.<link rel="sty
+00000950: 6c65 7368 6565 7422 2068 7265 663d 2268  lesheet" href="h
+00000960: 7474 7073 3a2f 2f63 646e 6a73 2e63 6c6f  ttps://cdnjs.clo
+00000970: 7564 666c 6172 652e 636f 6d2f 616a 6178  udflare.com/ajax
+00000980: 2f6c 6962 732f 666f 6e74 2d61 7765 736f  /libs/font-aweso
+00000990: 6d65 2f34 2e37 2e30 2f63 7373 2f66 6f6e  me/4.7.0/css/fon
+000009a0: 742d 6177 6573 6f6d 652e 6d69 6e2e 6373  t-awesome.min.cs
+000009b0: 7322 3e0a 0a4c 6966 744f 6e20 6973 2061  s">..LiftOn is a
+000009c0: 2068 6f6d 6f6c 6f67 792d 6261 7365 6420   homology-based 
+000009d0: 6c69 6674 2d6f 7665 7220 746f 6f6c 2075  lift-over tool u
+000009e0: 7369 6e67 2062 6f74 6820 444e 412d 444e  sing both DNA-DN
+000009f0: 4120 616c 6967 6e6d 656e 7473 2028 6672  A alignments (fr
+00000a00: 6f6d 203c 6120 6872 6566 3d22 6874 7470  om <a href="http
+00000a10: 733a 2f2f 6163 6164 656d 6963 2e6f 7570  s://academic.oup
+00000a20: 2e63 6f6d 2f62 696f 696e 666f 726d 6174  .com/bioinformat
+00000a30: 6963 732f 6172 7469 636c 652f 3337 2f31  ics/article/37/1
+00000a40: 322f 3136 3339 2f36 3033 3531 3238 3f6c  2/1639/6035128?l
+00000a50: 6f67 696e 3d74 7275 6522 2074 6172 6765  ogin=true" targe
+00000a60: 743d 225f 626c 616e 6b22 3e4c 6966 746f  t="_blank">Lifto
+00000a70: 6666 3c2f 613e 2c20 6372 6564 6974 7320  ff</a>, credits 
+00000a80: 746f 203c 6120 6872 6566 3d22 6874 7470  to <a href="http
+00000a90: 733a 2f2f 7363 686f 6c61 722e 676f 6f67  s://scholar.goog
+00000aa0: 6c65 2e63 6f6d 2f63 6974 6174 696f 6e73  le.com/citations
+00000ab0: 3f75 7365 723d 4e33 7458 6b37 5141 4141  ?user=N3tXk7QAAA
+00000ac0: 414a 2661 6d70 3b68 6c3d 656e 2220 7461  AJ&amp;hl=en" ta
+00000ad0: 7267 6574 3d22 5f62 6c61 6e6b 223e 4472  rget="_blank">Dr
+00000ae0: 2e20 416c 6169 6e61 2053 6875 6d61 7465  . Alaina Shumate
+00000af0: 3c2f 613e 2920 616e 6420 7072 6f74 6569  </a>) and protei
+00000b00: 6e2d 444e 4120 616c 6967 6e6d 656e 7473  n-DNA alignments
+00000b10: 2028 6672 6f6d 203c 6120 6872 6566 3d22   (from <a href="
+00000b20: 6874 7470 733a 2f2f 6163 6164 656d 6963  https://academic
+00000b30: 2e6f 7570 2e63 6f6d 2f62 696f 696e 666f  .oup.com/bioinfo
+00000b40: 726d 6174 6963 732f 6172 7469 636c 652f  rmatics/article/
+00000b50: 3339 2f31 2f62 7461 6430 3134 2f36 3938  39/1/btad014/698
+00000b60: 3936 3231 2220 7461 7267 6574 3d22 5f62  9621" target="_b
+00000b70: 6c61 6e6b 223e 6d69 6e69 7072 6f74 3c2f  lank">miniprot</
+00000b80: 613e 2c20 6372 6564 6974 7320 746f 203c  a>, credits to <
+00000b90: 6120 6872 6566 3d22 6874 7470 3a2f 2f6c  a href="http://l
+00000ba0: 6968 656e 672e 6f72 6722 2074 6172 6765  iheng.org" targe
+00000bb0: 743d 225f 626c 616e 6b22 3e44 722e 2048  t="_blank">Dr. H
+00000bc0: 656e 6720 4c69 3c2f 613e 2920 746f 2061  eng Li</a>) to a
+00000bd0: 6363 7572 6174 656c 7920 6d61 7020 616e  ccurately map an
+00000be0: 6e6f 7461 7469 6f6e 7320 6265 7477 6565  notations betwee
+00000bf0: 6e20 6765 6e6f 6d65 2061 7373 656d 626c  n genome assembl
+00000c00: 6965 7320 6f66 2074 6865 2073 616d 6520  ies of the same 
+00000c10: 6f72 2064 6966 6665 7265 6e74 2073 7065  or different spe
+00000c20: 6369 6573 2e20 4c69 6674 4f6e 2065 6d70  cies. LiftOn emp
+00000c30: 6c6f 7973 2061 2074 776f 2d73 7465 7020  loys a two-step 
+00000c40: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000c50: 2f63 6362 2e6a 6875 2e65 6475 2f6c 6966  /ccb.jhu.edu/lif
+00000c60: 746f 6e2f 636f 6e74 656e 742f 6265 6869  ton/content/behi
+00000c70: 6e64 5f73 6365 6e65 732e 6874 6d6c 2370  nd_scenes.html#p
+00000c80: 726f 7465 696e 2d6d 6178 696d 697a 6174  rotein-maximizat
+00000c90: 696f 6e2d 616c 676f 7269 7468 6d22 3e70  ion-algorithm">p
+00000ca0: 726f 7465 696e 206d 6178 696d 697a 6174  rotein maximizat
+00000cb0: 696f 6e20 616c 676f 7269 7468 6d3c 2f61  ion algorithm</a
+00000cc0: 3e20 746f 2069 6d70 726f 7665 2074 6865  > to improve the
+00000cd0: 2061 6e6e 6f74 6174 696f 6e20 6f66 2070   annotation of p
+00000ce0: 726f 7465 696e 2d63 6f64 696e 6720 6765  rotein-coding ge
+00000cf0: 6e65 7320 696e 2074 6865 2054 3254 2d43  nes in the T2T-C
+00000d00: 484d 3133 203c 6120 6872 6566 3d22 6874  HM13 <a href="ht
+00000d10: 7470 733a 2f2f 7333 2d75 732d 7765 7374  tps://s3-us-west
+00000d20: 2d32 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  -2.amazonaws.com
+00000d30: 2f68 756d 616e 2d70 616e 6765 6e6f 6d69  /human-pangenomi
+00000d40: 6373 2f54 3254 2f43 484d 3133 2f61 7373  cs/T2T/CHM13/ass
+00000d50: 656d 626c 6965 732f 616e 6e6f 7461 7469  emblies/annotati
+00000d60: 6f6e 2f63 686d 3133 7632 2e30 5f52 6566  on/chm13v2.0_Ref
+00000d70: 5365 715f 4c69 6674 6f66 665f 7635 2e31  Seq_Liftoff_v5.1
+00000d80: 2e67 6666 332e 677a 2220 7461 7267 6574  .gff3.gz" target
+00000d90: 3d22 5f62 6c61 6e6b 223e 4a48 5520 5265  ="_blank">JHU Re
+00000da0: 6653 6571 7631 3130 202b 204c 6966 746f  fSeqv110 + Lifto
+00000db0: 6666 2076 352e 313c 2f61 3e20 616e 6e6f  ff v5.1</a> anno
+00000dc0: 7461 7469 6f6e 2e0a 5468 6520 6c61 7465  tation..The late
+00000dd0: 7374 2054 3254 2d43 484d 3133 2061 6e6e  st T2T-CHM13 ann
+00000de0: 6f74 6174 696f 6e20 6765 6e65 7261 7465  otation generate
+00000df0: 6420 6279 204c 6966 744f 6e20 6973 2061  d by LiftOn is a
+00000e00: 7661 696c 6162 6c65 2061 7320 3c61 2068  vailable as <a h
+00000e10: 7265 663d 2268 7474 7073 3a2f 2f74 696e  ref="https://tin
+00000e20: 7975 726c 2e63 6f6d 2f34 7879 7774 7776  yurl.com/4xywtwv
+00000e30: 6522 2074 6172 6765 743d 225f 626c 616e  e" target="_blan
+00000e40: 6b22 3e4a 4855 5f4c 6966 744f 6e5f 7631  k">JHU_LiftOn_v1
+00000e50: 2e30 5f63 686d 3133 7632 2e30 2e67 6666  .0_chm13v2.0.gff
+00000e60: 3320 2866 7470 3a2f 2f66 7470 2e63 6362  3 (ftp://ftp.ccb
+00000e70: 2e6a 6875 2e65 6475 2f70 7562 2f64 6174  .jhu.edu/pub/dat
+00000e80: 612f 4c69 6674 4f6e 2f4a 4855 5f4c 6966  a/LiftOn/JHU_Lif
+00000e90: 744f 6e5f 7631 2e30 5f63 686d 3133 7632  tOn_v1.0_chm13v2
+00000ea0: 2e30 2e67 6666 3329 203c 6920 636c 6173  .0.gff3) <i clas
+00000eb0: 733d 2266 6120 6661 2d64 6f77 6e6c 6f61  s="fa fa-downloa
+00000ec0: 6422 3e3c 2f69 3e3c 2f61 3e2e 3c73 6563  d"></i></a>.<sec
+00000ed0: 7469 6f6e 2069 643d 2277 6879 2d6c 6966  tion id="why-lif
+00000ee0: 746f 6e22 2063 6c61 7373 3d22 223e 0a3c  ton" class="">.<
+00000ef0: 6832 3e57 6879 204c 6966 744f 6ee2 9d93  h2>Why LiftOn...
+00000f00: 3c61 2063 6c61 7373 3d22 6865 6164 6572  <a class="header
+00000f10: 6c69 6e6b 2220 6872 6566 3d22 2377 6879  link" href="#why
+00000f20: 2d6c 6966 746f 6e22 2074 6974 6c65 3d22  -lifton" title="
+00000f30: 5065 726d 616c 696e 6b20 746f 2074 6869  Permalink to thi
+00000f40: 7320 6865 6164 696e 6722 3e23 3c2f 613e  s heading">#</a>
+00000f50: 3c2f 6832 3e0a 3c6f 6c20 636c 6173 733d  </h2>.<ol class=
+00000f60: 2261 7261 6269 6320 7369 6d70 6c65 223e  "arabic simple">
+00000f70: 0a3c 6c69 3e3c 703e 3c73 7472 6f6e 673e  .<li><p><strong>
+00000f80: 4275 7267 656f 6e69 6e67 206e 756d 6265  Burgeoning numbe
+00000f90: 7220 6f66 2067 656e 6f6d 6520 6173 7365  r of genome asse
+00000fa0: 6d62 6c69 6573 3c2f 7374 726f 6e67 3e3a  mblies</strong>:
+00000fb0: 2041 7320 6f66 2044 6563 656d 6265 7220   As of December 
+00000fc0: 3230 3233 2c20 7468 6572 6520 6172 6520  2023, there are 
+00000fd0: 3330 2c35 3330 2065 756b 6172 796f 7469  30,530 eukaryoti
+00000fe0: 6320 6765 6e6f 6d65 732c 2035 3637 2c32  c genomes, 567,2
+00000ff0: 3238 2070 726f 6b61 7279 6f74 6963 2067  28 prokaryotic g
+00001000: 656e 6f6d 6573 2c20 616e 6420 3636 2c34  enomes, and 66,4
+00001010: 3239 2076 6972 7573 6573 206c 6973 7465  29 viruses liste
+00001020: 6420 6f6e 204e 4342 4920 283c 6120 636c  d on NCBI (<a cl
+00001030: 6173 733d 2272 6566 6572 656e 6365 2065  ass="reference e
+00001040: 7874 6572 6e61 6c22 2068 7265 663d 2268  xternal" href="h
+00001050: 7474 7073 3a2f 2f77 7777 2e6e 6362 692e  ttps://www.ncbi.
+00001060: 6e6c 6d2e 6e69 682e 676f 762f 6765 6e6f  nlm.nih.gov/geno
+00001070: 6d65 2f62 726f 7773 652f 2321 2f6f 7665  me/browse/#!/ove
+00001080: 7276 6965 772f 223e 4e43 4249 2067 656e  rview/">NCBI gen
+00001090: 6f6d 6520 6272 6f77 7365 723c 2f61 3e29  ome browser</a>)
+000010a0: 2e20 486f 7765 7665 722c 2067 656e 6f6d  . However, genom
+000010b0: 6520 616e 6e6f 7461 7469 6f6e 2069 7320  e annotation is 
+000010c0: 6c61 6767 696e 6720 6265 6869 6e64 2e20  lagging behind. 
+000010d0: 4173 206d 6f72 6520 6869 6768 2d71 7561  As more high-qua
+000010e0: 6c69 7479 2061 7373 656d 626c 6965 7320  lity assemblies 
+000010f0: 6172 6520 6765 6e65 7261 7465 642c 2077  are generated, w
+00001100: 6520 6e65 6564 2061 6e20 6163 6375 7261  e need an accura
+00001110: 7465 206c 6966 742d 6f76 6572 2074 6f6f  te lift-over too
+00001120: 6c20 746f 2061 6e6e 6f74 6174 6520 7468  l to annotate th
+00001130: 656d 2e3c 2f70 3e3c 2f6c 693e 0a3c 6c69  em.</p></li>.<li
+00001140: 3e3c 703e 3c73 7472 6f6e 673e 496d 7072  ><p><strong>Impr
+00001150: 6f76 6564 2070 726f 7465 696e 2d63 6f64  oved protein-cod
+00001160: 696e 6720 6765 6e65 206d 6170 7069 6e67  ing gene mapping
+00001170: 3c2f 7374 726f 6e67 3e3a 2054 6865 2070  </strong>: The p
+00001180: 6f70 756c 6172 203c 6120 636c 6173 733d  opular <a class=
+00001190: 2272 6566 6572 656e 6365 2065 7874 6572  "reference exter
+000011a0: 6e61 6c22 2068 7265 663d 2268 7474 7073  nal" href="https
+000011b0: 3a2f 2f61 6361 6465 6d69 632e 6f75 702e  ://academic.oup.
+000011c0: 636f 6d2f 6269 6f69 6e66 6f72 6d61 7469  com/bioinformati
+000011d0: 6373 2f61 7274 6963 6c65 2f33 372f 3132  cs/article/37/12
+000011e0: 2f31 3633 392f 3630 3335 3132 383f 6c6f  /1639/6035128?lo
+000011f0: 6769 6e3d 7472 7565 223e 4c69 6674 6f66  gin=true">Liftof
+00001200: 663c 2f61 3e20 746f 6f6c 206d 6170 7320  f</a> tool maps 
+00001210: 6765 6e65 7320 6261 7365 6420 6f6e 2044  genes based on D
+00001220: 4e41 2061 6c69 676e 6d65 6e74 7320 616c  NA alignments al
+00001230: 6f6e 652e 203c 6120 636c 6173 733d 2272  one. <a class="r
+00001240: 6566 6572 656e 6365 2065 7874 6572 6e61  eference externa
+00001250: 6c22 2068 7265 663d 2268 7474 7073 3a2f  l" href="https:/
+00001260: 2f67 6974 6875 622e 636f 6d2f 6c68 332f  /github.com/lh3/
+00001270: 6d69 6e69 7072 6f74 223e 4d69 6e69 7072  miniprot">Minipr
+00001280: 6f74 3c2f 613e 206d 6170 7320 6765 6e65  ot</a> maps gene
+00001290: 7320 6261 7365 6420 6f6e 2070 726f 7465  s based on prote
+000012a0: 696e 2061 6c69 676e 6d65 6e74 7320 6275  in alignments bu
+000012b0: 742c 2077 6974 686f 7574 2067 656e 6520  t, without gene 
+000012c0: 7374 7275 6374 7572 6520 696e 666f 726d  structure inform
+000012d0: 6174 696f 6e2c 206d 6179 206e 6f74 2062  ation, may not b
+000012e0: 6520 6173 2061 6363 7572 6174 6520 6f6e  e as accurate on
+000012f0: 2074 6865 6972 206f 776e 2028 5365 6520   their own (See 
+00001300: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
+00001310: 6e63 6520 696e 7465 726e 616c 2220 6872  nce internal" hr
+00001320: 6566 3d22 6874 7470 733a 2f2f 6363 622e  ef="https://ccb.
+00001330: 6a68 752e 6564 752f 6c69 6674 6f6e 2f63  jhu.edu/lifton/c
+00001340: 6f6e 7465 6e74 2f68 6f77 5f74 6f5f 7061  ontent/how_to_pa
+00001350: 6765 2e68 746d 6c23 7768 792d 6c69 6674  ge.html#why-lift
+00001360: 6f6e 2d71 6122 3e3c 7370 616e 2063 6c61  on-qa"><span cla
+00001370: 7373 3d22 7374 6420 7374 642d 7265 6622  ss="std std-ref"
+00001380: 3e46 4151 2043 6f6d 6d6f 6e20 6d69 7374  >FAQ Common mist
+00001390: 616b 6573 206f 6620 4c69 6674 6f66 6620  akes of Liftoff 
+000013a0: 616e 6420 6d69 6e69 7072 6f74 3c2f 7370  and miniprot</sp
+000013b0: 616e 3e3c 2f61 3e29 2e20 4c69 6674 4f6e  an></a>). LiftOn
+000013c0: 2063 6f6d 6269 6e65 7320 626f 7468 2044   combines both D
+000013d0: 4e41 2d74 6f2d 6765 6e6f 6d65 2061 6e64  NA-to-genome and
+000013e0: 2070 726f 7465 696e 2d74 6f2d 6765 6e6f   protein-to-geno
+000013f0: 6d65 2061 6c69 676e 6d65 6e74 7320 616e  me alignments an
+00001400: 6420 7072 6f64 7563 6573 2062 6574 7465  d produces bette
+00001410: 7220 6765 6e65 206d 6170 7069 6e67 2072  r gene mapping r
+00001420: 6573 756c 7473 2120 4c69 6674 4f6e 2069  esults! LiftOn i
+00001430: 6d70 726f 7665 7320 7570 6f6e 2074 6865  mproves upon the
+00001440: 2063 7572 7265 6e74 2072 656c 6561 7365   current release
+00001450: 6420 5432 542d 4348 4d31 3320 616e 6e6f  d T2T-CHM13 anno
+00001460: 7461 7469 6f6e 2028 3c61 2063 6c61 7373  tation (<a class
+00001470: 3d22 7265 6665 7265 6e63 6520 6578 7465  ="reference exte
+00001480: 726e 616c 2220 6872 6566 3d22 6874 7470  rnal" href="http
+00001490: 733a 2f2f 7333 2d75 732d 7765 7374 2d32  s://s3-us-west-2
+000014a0: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f68  .amazonaws.com/h
+000014b0: 756d 616e 2d70 616e 6765 6e6f 6d69 6373  uman-pangenomics
+000014c0: 2f54 3254 2f43 484d 3133 2f61 7373 656d  /T2T/CHM13/assem
+000014d0: 626c 6965 732f 616e 6e6f 7461 7469 6f6e  blies/annotation
+000014e0: 2f63 686d 3133 7632 2e30 5f52 6566 5365  /chm13v2.0_RefSe
+000014f0: 715f 4c69 6674 6f66 665f 7635 2e31 2e67  q_Liftoff_v5.1.g
+00001500: 6666 332e 677a 223e 4a48 5520 5265 6653  ff3.gz">JHU RefS
+00001510: 6571 7631 3130 202b 204c 6966 746f 6666  eqv110 + Liftoff
+00001520: 2076 352e 313c 2f61 3e29 2e3c 2f70 3e3c   v5.1</a>).</p><
+00001530: 2f6c 693e 0a3c 6c69 3e3c 703e 3c73 7472  /li>.<li><p><str
+00001540: 6f6e 673e 496d 7072 6f76 6564 2064 6973  ong>Improved dis
+00001550: 7461 6e74 6c79 2072 656c 6174 6564 2073  tantly related s
+00001560: 7065 6369 6573 206c 6966 742d 6f76 6572  pecies lift-over
+00001570: 3c2f 7374 726f 6e67 3e3a 2041 206b 6579  </strong>: A key
+00001580: 206c 696d 6974 6174 696f 6e20 6f66 2044   limitation of D
+00001590: 4e41 2d62 6173 6564 206c 6966 742d 6f76  NA-based lift-ov
+000015a0: 6572 2074 6f6f 6c73 2069 7320 7468 6174  er tools is that
+000015b0: 2074 6865 7920 646f 206e 6f74 2070 6572   they do not per
+000015c0: 666f 726d 2077 656c 6c20 7768 656e 2074  form well when t
+000015d0: 6865 2072 6566 6572 656e 6365 2061 6e64  he reference and
+000015e0: 2074 6172 6765 7420 6765 6e6f 6d65 7320   target genomes 
+000015f0: 6861 7665 2073 6967 6e69 6669 6361 6e74  have significant
+00001600: 6c79 2064 6976 6572 6765 642e 2057 6974  ly diverged. Wit
+00001610: 6820 7468 6520 6865 6c70 206f 6620 7072  h the help of pr
+00001620: 6f74 6569 6e20 616c 6967 6e6d 656e 7473  otein alignments
+00001630: 2061 6e64 2074 6865 2070 726f 7465 696e   and the protein
+00001640: 206d 6178 696d 697a 6174 696f 6e20 616c   maximization al
+00001650: 676f 7269 7468 6d2c 204c 6966 744f 6e20  gorithm, LiftOn 
+00001660: 696d 7072 6f76 6573 2074 6865 206c 6966  improves the lif
+00001670: 742d 6f76 6572 2070 726f 6365 7373 2062  t-over process b
+00001680: 6574 7765 656e 2064 6973 7461 6e74 6c79  etween distantly
+00001690: 2072 656c 6174 6564 2073 7065 6369 6573   related species
+000016a0: 2e20 5365 6520 223c 6120 636c 6173 733d  . See "<a class=
+000016b0: 2272 6566 6572 656e 6365 2069 6e74 6572  "reference inter
+000016c0: 6e61 6c22 2068 7265 663d 2268 7474 7073  nal" href="https
+000016d0: 3a2f 2f63 6362 2e6a 6875 2e65 6475 2f6c  ://ccb.jhu.edu/l
+000016e0: 6966 746f 6e2f 636f 6e74 656e 742f 6469  ifton/content/di
+000016f0: 7374 616e 745f 7370 6563 6965 735f 6c69  stant_species_li
+00001700: 6674 6f76 6572 2f6c 6966 746f 7665 725f  ftover/liftover_
+00001710: 6d6f 7573 655f 325f 7261 742e 6874 6d6c  mouse_2_rat.html
+00001720: 2364 6973 7461 6e74 2d73 7065 6369 6573  #distant-species
+00001730: 2d6c 6966 746f 7665 722d 6d6f 7573 652d  -liftover-mouse-
+00001740: 746f 2d72 6174 223e 3c73 7061 6e20 636c  to-rat"><span cl
+00001750: 6173 733d 2273 7464 2073 7464 2d72 6566  ass="std std-ref
+00001760: 223e 4d6f 7573 6520 746f 2052 6174 3c2f  ">Mouse to Rat</
+00001770: 7370 616e 3e3c 2f61 3e22 2061 6e64 2022  span></a>" and "
+00001780: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
+00001790: 6e63 6520 696e 7465 726e 616c 2220 6872  nce internal" hr
+000017a0: 6566 3d22 6874 7470 733a 2f2f 6363 622e  ef="https://ccb.
+000017b0: 6a68 752e 6564 752f 6c69 6674 6f6e 2f63  jhu.edu/lifton/c
+000017c0: 6f6e 7465 6e74 2f64 6973 7461 6e74 5f73  ontent/distant_s
+000017d0: 7065 6369 6573 5f6c 6966 746f 7665 722f  pecies_liftover/
+000017e0: 6c69 6674 6f76 6572 5f64 726f 736f 7068  liftover_drosoph
+000017f0: 696c 615f 6572 6563 7461 2e68 746d 6c23  ila_erecta.html#
+00001800: 6469 7374 616e 742d 7370 6563 6965 732d  distant-species-
+00001810: 6c69 6674 6f76 6572 2d64 726f 736f 7068  liftover-drosoph
+00001820: 696c 612d 6d65 6c61 6e6f 6761 7374 6572  ila-melanogaster
+00001830: 2d32 2d65 7265 6374 6122 3e3c 7370 616e  -2-erecta"><span
+00001840: 2063 6c61 7373 3d22 7374 6420 7374 642d   class="std std-
+00001850: 7265 6622 3e44 726f 736f 7068 696c 6120  ref">Drosophila 
+00001860: 6d65 6c61 6e6f 6761 7374 6572 2074 6f20  melanogaster to 
+00001870: 4472 6f73 6f70 6869 6c61 2065 7265 6374  Drosophila erect
+00001880: 613c 2f73 7061 6e3e 3c2f 613e 2220 7265  a</span></a>" re
+00001890: 7375 6c74 2073 6563 7469 6f6e 732e 3c2f  sult sections.</
+000018a0: 703e 3c2f 6c69 3e0a 3c2f 6f6c 3e0a 3c70  p></li>.</ol>.<p
+000018b0: 3e4c 6966 744f 6e20 6973 2066 7265 652c  >LiftOn is free,
+000018c0: 2069 7427 7320 6f70 656e 2073 6f75 7263   it's open sourc
+000018d0: 652c 2069 7427 7320 6561 7379 2074 6f20  e, it's easy to 
+000018e0: 696e 7374 616c 6c20 2c20 616e 6420 6974  install , and it
+000018f0: 2773 2069 6e20 5079 7468 6f6e 213c 2f70  's in Python!</p
+00001900: 3e0a 3c64 6976 2063 6c61 7373 3d22 6c69  >.<div class="li
+00001910: 6e65 2d62 6c6f 636b 223e 0a3c 6469 7620  ne-block">.<div 
+00001920: 636c 6173 733d 226c 696e 6522 3e3c 6272  class="line"><br
+00001930: 3e3c 2f64 6976 3e0a 3c2f 6469 763e 0a3c  ></div>.</div>.<
+00001940: 2f73 6563 7469 6f6e 3e0a 3c73 6563 7469  /section>.<secti
+00001950: 6f6e 2069 643d 2277 686f 2d69 732d 6974  on id="who-is-it
+00001960: 2d66 6f72 2220 636c 6173 733d 2222 3e0a  -for" class="">.
+00001970: 3c68 323e 5768 6f20 6973 2069 7420 666f  <h2>Who is it fo
+00001980: 72e2 9d93 3c61 2063 6c61 7373 3d22 6865  r...<a class="he
+00001990: 6164 6572 6c69 6e6b 2220 6872 6566 3d22  aderlink" href="
+000019a0: 2377 686f 2d69 732d 6974 2d66 6f72 2220  #who-is-it-for" 
+000019b0: 7469 746c 653d 2250 6572 6d61 6c69 6e6b  title="Permalink
+000019c0: 2074 6f20 7468 6973 2068 6561 6469 6e67   to this heading
+000019d0: 223e 233c 2f61 3e3c 2f68 323e 0a3c 703e  ">#</a></h2>.<p>
+000019e0: 4c69 6674 4f6e 2069 7320 6465 7369 676e  LiftOn is design
+000019f0: 6564 2066 6f72 2072 6573 6561 7263 6865  ed for researche
+00001a00: 7273 2061 6e64 2062 696f 696e 666f 726d  rs and bioinform
+00001a10: 6174 6963 6961 6e73 2077 686f 2061 7265  aticians who are
+00001a20: 2069 6e74 6572 6573 7465 6420 696e 2067   interested in g
+00001a30: 656e 6f6d 6520 616e 6e6f 7461 7469 6f6e  enome annotation
+00001a40: 2e20 4974 2069 7320 616e 2065 6173 792d  . It is an easy-
+00001a50: 746f 2d69 6e73 7461 6c6c 2061 6e64 2065  to-install and e
+00001a60: 6173 792d 746f 2d72 756e 2063 6f6d 6d61  asy-to-run comma
+00001a70: 6e64 2d6c 696e 6520 746f 6f6c 2e20 5370  nd-line tool. Sp
+00001a80: 6563 6966 6963 616c 6c79 2c20 6974 2069  ecifically, it i
+00001a90: 7320 6265 6e65 6669 6369 616c 2069 6e20  s beneficial in 
+00001aa0: 7468 6520 666f 6c6c 6f77 696e 6720 7363  the following sc
+00001ab0: 656e 6172 696f 733a 3c2f 703e 0a3c 6f6c  enarios:</p>.<ol
+00001ac0: 2063 6c61 7373 3d22 6172 6162 6963 2073   class="arabic s
+00001ad0: 696d 706c 6522 3e0a 3c6c 693e 3c70 3e49  imple">.<li><p>I
+00001ae0: 6620 796f 7520 6861 7665 2073 6571 7565  f you have seque
+00001af0: 6e63 6564 2061 6e64 2061 7373 656d 626c  nced and assembl
+00001b00: 6564 2061 206e 6577 2067 656e 6f6d 6520  ed a new genome 
+00001b10: 616e 6420 7265 7175 6972 6520 616e 6e6f  and require anno
+00001b20: 7461 7469 6f6e 2c20 4c69 6674 4f6e 2070  tation, LiftOn p
+00001b30: 726f 7669 6465 7320 616e 2065 6666 6963  rovides an effic
+00001b40: 6965 6e74 2073 6f6c 7574 696f 6e20 666f  ient solution fo
+00001b50: 7220 6765 6e65 7261 7469 6e67 2061 6e6e  r generating ann
+00001b60: 6f74 6174 696f 6e73 2066 6f72 2079 6f75  otations for you
+00001b70: 7220 6765 6e6f 6d65 2e3c 2f70 3e3c 2f6c  r genome.</p></l
+00001b80: 693e 0a3c 6c69 3e3c 703e 4c69 6674 4f6e  i>.<li><p>LiftOn
+00001b90: 2069 7320 616e 2065 7863 656c 6c65 6e74   is an excellent
+00001ba0: 2074 6f6f 6c20 666f 7220 7468 6f73 6520   tool for those 
+00001bb0: 6c6f 6f6b 696e 6720 746f 2070 6572 666f  looking to perfo
+00001bc0: 726d 2063 6f6d 7061 7261 7469 7665 2067  rm comparative g
+00001bd0: 656e 6f6d 6963 7320 616e 616c 7973 6973  enomics analysis
+00001be0: 2e20 4974 2066 6163 696c 6974 6174 6573  . It facilitates
+00001bf0: 2074 6865 206c 6966 7469 6e67 206f 7665   the lifting ove
+00001c00: 7220 616e 6420 636f 6d70 6172 6973 6f6e  r and comparison
+00001c10: 206f 6620 6765 6e65 2063 6f6e 7465 6e74   of gene content
+00001c20: 7320 6265 7477 6565 6e20 6469 6666 6572  s between differ
+00001c30: 656e 7420 6765 6e6f 6d65 732c 2061 6964  ent genomes, aid
+00001c40: 696e 6720 696e 2075 6e64 6572 7374 616e  ing in understan
+00001c50: 6469 6e67 2065 766f 6c75 7469 6f6e 6172  ding evolutionar
+00001c60: 7920 7265 6c61 7469 6f6e 7368 6970 7320  y relationships 
+00001c70: 616e 6420 6675 6e63 7469 6f6e 616c 2067  and functional g
+00001c80: 656e 6f6d 6963 732e 3c2f 703e 3c2f 6c69  enomics.</p></li
+00001c90: 3e0a 3c6c 693e 3c70 3e46 6f72 2072 6573  >.<li><p>For res
+00001ca0: 6561 7263 6865 7273 2069 6e74 6572 6573  earchers interes
+00001cb0: 7465 6420 696e 2075 7369 6e67 2054 3254  ted in using T2T
+00001cc0: 2d43 484d 3133 2061 6e6e 6f74 6174 696f  -CHM13 annotatio
+00001cd0: 6e73 2c20 7472 7920 4c69 6674 4f6e 2120  ns, try LiftOn! 
+00001ce0: 5765 2068 6176 6520 7072 652d 6765 6e65  We have pre-gene
+00001cf0: 7261 7465 6420 7468 6520 3c61 2063 6c61  rated the <a cla
+00001d00: 7373 3d22 7265 6665 7265 6e63 6520 6578  ss="reference ex
+00001d10: 7465 726e 616c 2220 6872 6566 3d22 6874  ternal" href="ht
+00001d20: 7470 733a 2f2f 7469 6e79 7572 6c2e 636f  tps://tinyurl.co
+00001d30: 6d2f 3478 7977 7477 7665 223e 4a48 555f  m/4xywtwve">JHU_
+00001d40: 4c69 6674 4f6e 5f76 312e 305f 6368 6d31  LiftOn_v1.0_chm1
+00001d50: 3376 322e 302e 6766 6633 3c2f 613e 2028  3v2.0.gff3</a> (
+00001d60: 6674 703a 2f2f 6674 702e 6363 622e 6a68  ftp://ftp.ccb.jh
+00001d70: 752e 6564 752f 7075 622f 6461 7461 2f4c  u.edu/pub/data/L
+00001d80: 6966 744f 6e2f 4a48 555f 4c69 6674 4f6e  iftOn/JHU_LiftOn
+00001d90: 5f76 312e 305f 6368 6d31 3376 322e 302e  _v1.0_chm13v2.0.
+00001da0: 6766 6633 2920 6669 6c65 2066 6f72 2079  gff3) file for y
+00001db0: 6f75 7220 636f 6e76 656e 6965 6e63 652e  our convenience.
+00001dc0: 3c2f 703e 3c2f 6c69 3e0a 3c2f 6f6c 3e0a  </p></li>.</ol>.
+00001dd0: 3c64 6976 2063 6c61 7373 3d22 6c69 6e65  <div class="line
+00001de0: 2d62 6c6f 636b 223e 0a3c 6469 7620 636c  -block">.<div cl
+00001df0: 6173 733d 226c 696e 6522 3e3c 6272 3e3c  ass="line"><br><
+00001e00: 2f64 6976 3e0a 3c2f 6469 763e 0a3c 2f73  /div>.</div>.</s
+00001e10: 6563 7469 6f6e 3e0a 3c73 6563 7469 6f6e  ection>.<section
+00001e20: 2069 643d 2277 6861 742d 646f 6573 2d6c   id="what-does-l
+00001e30: 6966 746f 6e2d 646f 2220 636c 6173 733d  ifton-do" class=
+00001e40: 2222 3e0a 3c68 323e 5768 6174 2064 6f65  "">.<h2>What doe
+00001e50: 7320 4c69 6674 4f6e 2064 6fe2 9d93 3c61  s LiftOn do...<a
+00001e60: 2063 6c61 7373 3d22 6865 6164 6572 6c69   class="headerli
+00001e70: 6e6b 2220 6872 6566 3d22 2377 6861 742d  nk" href="#what-
+00001e80: 646f 6573 2d6c 6966 746f 6e2d 646f 2220  does-lifton-do" 
+00001e90: 7469 746c 653d 2250 6572 6d61 6c69 6e6b  title="Permalink
+00001ea0: 2074 6f20 7468 6973 2068 6561 6469 6e67   to this heading
+00001eb0: 223e 233c 2f61 3e3c 2f68 323e 0a3c 703e  ">#</a></h2>.<p>
+00001ec0: 4c65 7427 7320 6669 7273 7420 6465 6669  Let's first defi
+00001ed0: 6e65 2074 6865 2070 726f 626c 656d 3a0a  ne the problem:.
+00001ee0: 4769 7665 6e20 6120 7265 6665 7265 6e63  Given a referenc
+00001ef0: 6520 3c73 7472 6f6e 673e 4765 6e6f 6d65  e <strong>Genome
+00001f00: 3c2f 7374 726f 6e67 3e20 3c73 7061 6e20  </strong> <span 
+00001f10: 636c 6173 733d 226d 6174 6820 6e6f 7472  class="math notr
+00001f20: 616e 736c 6174 6520 6e6f 6869 6768 6c69  anslate nohighli
+00001f30: 6768 7422 3e3c 6d6a 782d 636f 6e74 6169  ght"><mjx-contai
+00001f40: 6e65 7220 636c 6173 733d 224d 6174 684a  ner class="MathJ
+00001f50: 6178 2043 7478 744d 656e 755f 4174 7461  ax CtxtMenu_Atta
+00001f60: 6368 6564 5f30 2220 6a61 783d 2243 4854  ched_0" jax="CHT
+00001f70: 4d4c 2220 7461 6269 6e64 6578 3d22 3022  ML" tabindex="0"
+00001f80: 2063 7478 746d 656e 755f 636f 756e 7465   ctxtmenu_counte
+00001f90: 723d 2230 2220 7374 796c 653d 2266 6f6e  r="0" style="fon
+00001fa0: 742d 7369 7a65 3a20 3131 382e 3925 3b20  t-size: 118.9%; 
+00001fb0: 706f 7369 7469 6f6e 3a20 7265 6c61 7469  position: relati
+00001fc0: 7665 3b22 3e3c 6d6a 782d 6d61 7468 2063  ve;"><mjx-math c
+00001fd0: 6c61 7373 3d22 4d4a 582d 5445 5822 2061  lass="MJX-TEX" a
+00001fe0: 7269 612d 6869 6464 656e 3d22 7472 7565  ria-hidden="true
+00001ff0: 223e 3c6d 6a78 2d6d 6920 636c 6173 733d  "><mjx-mi class=
+00002000: 226d 6a78 2d69 223e 3c6d 6a78 2d63 2063  "mjx-i"><mjx-c c
+00002010: 6c61 7373 3d22 6d6a 782d 6331 4434 3435  lass="mjx-c1D445
+00002020: 2054 4558 2d49 223e 3c2f 6d6a 782d 633e   TEX-I"></mjx-c>
+00002030: 3c2f 6d6a 782d 6d69 3e3c 2f6d 6a78 2d6d  </mjx-mi></mjx-m
+00002040: 6174 683e 3c6d 6a78 2d61 7373 6973 7469  ath><mjx-assisti
+00002050: 7665 2d6d 6d6c 2075 6e73 656c 6563 7461  ve-mml unselecta
+00002060: 626c 653d 226f 6e22 2064 6973 706c 6179  ble="on" display
+00002070: 3d22 696e 6c69 6e65 223e 3c6d 6174 6820  ="inline"><math 
+00002080: 786d 6c6e 733d 2268 7474 703a 2f2f 7777  xmlns="http://ww
+00002090: 772e 7733 2e6f 7267 2f31 3939 382f 4d61  w.w3.org/1998/Ma
+000020a0: 7468 2f4d 6174 684d 4c22 3e3c 6d69 3e52  th/MathML"><mi>R
+000020b0: 3c2f 6d69 3e3c 2f6d 6174 683e 3c2f 6d6a  </mi></math></mj
+000020c0: 782d 6173 7369 7374 6976 652d 6d6d 6c3e  x-assistive-mml>
+000020d0: 3c2f 6d6a 782d 636f 6e74 6169 6e65 723e  </mjx-container>
+000020e0: 3c2f 7370 616e 3e2c 2061 6e20 3c73 7472  </span>, an <str
+000020f0: 6f6e 673e 416e 6e6f 7461 7469 6f6e 3c2f  ong>Annotation</
+00002100: 7374 726f 6e67 3e20 3c73 7061 6e20 636c  strong> <span cl
+00002110: 6173 733d 226d 6174 6820 6e6f 7472 616e  ass="math notran
+00002120: 736c 6174 6520 6e6f 6869 6768 6c69 6768  slate nohighligh
+00002130: 7422 3e3c 6d6a 782d 636f 6e74 6169 6e65  t"><mjx-containe
+00002140: 7220 636c 6173 733d 224d 6174 684a 6178  r class="MathJax
+00002150: 2043 7478 744d 656e 755f 4174 7461 6368   CtxtMenu_Attach
+00002160: 6564 5f30 2220 6a61 783d 2243 4854 4d4c  ed_0" jax="CHTML
+00002170: 2220 7461 6269 6e64 6578 3d22 3022 2063  " tabindex="0" c
+00002180: 7478 746d 656e 755f 636f 756e 7465 723d  txtmenu_counter=
+00002190: 2231 2220 7374 796c 653d 2266 6f6e 742d  "1" style="font-
+000021a0: 7369 7a65 3a20 3131 382e 3925 3b20 706f  size: 118.9%; po
+000021b0: 7369 7469 6f6e 3a20 7265 6c61 7469 7665  sition: relative
+000021c0: 3b22 3e3c 6d6a 782d 6d61 7468 2063 6c61  ;"><mjx-math cla
+000021d0: 7373 3d22 4d4a 582d 5445 5822 2061 7269  ss="MJX-TEX" ari
+000021e0: 612d 6869 6464 656e 3d22 7472 7565 223e  a-hidden="true">
+000021f0: 3c6d 6a78 2d6d 7375 623e 3c6d 6a78 2d6d  <mjx-msub><mjx-m
+00002200: 6920 636c 6173 733d 226d 6a78 2d69 223e  i class="mjx-i">
+00002210: 3c6d 6a78 2d63 2063 6c61 7373 3d22 6d6a  <mjx-c class="mj
+00002220: 782d 6331 4434 3435 2054 4558 2d49 223e  x-c1D445 TEX-I">
+00002230: 3c2f 6d6a 782d 633e 3c2f 6d6a 782d 6d69  </mjx-c></mjx-mi
+00002240: 3e3c 6d6a 782d 7363 7269 7074 2073 7479  ><mjx-script sty
+00002250: 6c65 3d22 7665 7274 6963 616c 2d61 6c69  le="vertical-ali
+00002260: 676e 3a20 2d30 2e31 3533 656d 3b22 3e3c  gn: -0.153em;"><
+00002270: 6d6a 782d 6d69 2063 6c61 7373 3d22 6d6a  mjx-mi class="mj
+00002280: 782d 6922 2073 697a 653d 2273 223e 3c6d  x-i" size="s"><m
+00002290: 6a78 2d63 2063 6c61 7373 3d22 6d6a 782d  jx-c class="mjx-
+000022a0: 6331 4434 3334 2054 4558 2d49 223e 3c2f  c1D434 TEX-I"></
+000022b0: 6d6a 782d 633e 3c2f 6d6a 782d 6d69 3e3c  mjx-c></mjx-mi><
+000022c0: 2f6d 6a78 2d73 6372 6970 743e 3c2f 6d6a  /mjx-script></mj
+000022d0: 782d 6d73 7562 3e3c 2f6d 6a78 2d6d 6174  x-msub></mjx-mat
+000022e0: 683e 3c6d 6a78 2d61 7373 6973 7469 7665  h><mjx-assistive
+000022f0: 2d6d 6d6c 2075 6e73 656c 6563 7461 626c  -mml unselectabl
+00002300: 653d 226f 6e22 2064 6973 706c 6179 3d22  e="on" display="
+00002310: 696e 6c69 6e65 223e 3c6d 6174 6820 786d  inline"><math xm
+00002320: 6c6e 733d 2268 7474 703a 2f2f 7777 772e  lns="http://www.
+00002330: 7733 2e6f 7267 2f31 3939 382f 4d61 7468  w3.org/1998/Math
+00002340: 2f4d 6174 684d 4c22 3e3c 6d73 7562 3e3c  /MathML"><msub><
+00002350: 6d69 3e52 3c2f 6d69 3e3c 6d69 3e41 3c2f  mi>R</mi><mi>A</
+00002360: 6d69 3e3c 2f6d 7375 623e 3c2f 6d61 7468  mi></msub></math
+00002370: 3e3c 2f6d 6a78 2d61 7373 6973 7469 7665  ></mjx-assistive
+00002380: 2d6d 6d6c 3e3c 2f6d 6a78 2d63 6f6e 7461  -mml></mjx-conta
+00002390: 696e 6572 3e3c 2f73 7061 6e3e 2c20 616e  iner></span>, an
+000023a0: 6420 6120 7461 7267 6574 203c 7374 726f  d a target <stro
+000023b0: 6e67 3e47 656e 6f6d 653c 2f73 7472 6f6e  ng>Genome</stron
+000023c0: 673e 203c 7370 616e 2063 6c61 7373 3d22  g> <span class="
+000023d0: 6d61 7468 206e 6f74 7261 6e73 6c61 7465  math notranslate
+000023e0: 206e 6f68 6967 686c 6967 6874 223e 3c6d   nohighlight"><m
+000023f0: 6a78 2d63 6f6e 7461 696e 6572 2063 6c61  jx-container cla
+00002400: 7373 3d22 4d61 7468 4a61 7820 4374 7874  ss="MathJax Ctxt
+00002410: 4d65 6e75 5f41 7474 6163 6865 645f 3022  Menu_Attached_0"
+00002420: 206a 6178 3d22 4348 544d 4c22 2074 6162   jax="CHTML" tab
+00002430: 696e 6465 783d 2230 2220 6374 7874 6d65  index="0" ctxtme
+00002440: 6e75 5f63 6f75 6e74 6572 3d22 3222 2073  nu_counter="2" s
+00002450: 7479 6c65 3d22 666f 6e74 2d73 697a 653a  tyle="font-size:
+00002460: 2031 3138 2e39 253b 2070 6f73 6974 696f   118.9%; positio
+00002470: 6e3a 2072 656c 6174 6976 653b 223e 3c6d  n: relative;"><m
+00002480: 6a78 2d6d 6174 6820 636c 6173 733d 224d  jx-math class="M
+00002490: 4a58 2d54 4558 2220 6172 6961 2d68 6964  JX-TEX" aria-hid
+000024a0: 6465 6e3d 2274 7275 6522 3e3c 6d6a 782d  den="true"><mjx-
+000024b0: 6d69 2063 6c61 7373 3d22 6d6a 782d 6922  mi class="mjx-i"
+000024c0: 3e3c 6d6a 782d 6320 636c 6173 733d 226d  ><mjx-c class="m
+000024d0: 6a78 2d63 3144 3434 3720 5445 582d 4922  jx-c1D447 TEX-I"
+000024e0: 3e3c 2f6d 6a78 2d63 3e3c 2f6d 6a78 2d6d  ></mjx-c></mjx-m
+000024f0: 693e 3c2f 6d6a 782d 6d61 7468 3e3c 6d6a  i></mjx-math><mj
+00002500: 782d 6173 7369 7374 6976 652d 6d6d 6c20  x-assistive-mml 
+00002510: 756e 7365 6c65 6374 6162 6c65 3d22 6f6e  unselectable="on
+00002520: 2220 6469 7370 6c61 793d 2269 6e6c 696e  " display="inlin
+00002530: 6522 3e3c 6d61 7468 2078 6d6c 6e73 3d22  e"><math xmlns="
+00002540: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
+00002550: 672f 3139 3938 2f4d 6174 682f 4d61 7468  g/1998/Math/Math
+00002560: 4d4c 223e 3c6d 693e 543c 2f6d 693e 3c2f  ML"><mi>T</mi></
+00002570: 6d61 7468 3e3c 2f6d 6a78 2d61 7373 6973  math></mjx-assis
+00002580: 7469 7665 2d6d 6d6c 3e3c 2f6d 6a78 2d63  tive-mml></mjx-c
+00002590: 6f6e 7461 696e 6572 3e3c 2f73 7061 6e3e  ontainer></span>
+000025a0: 2e20 5468 6520 6c69 6674 2d6f 7665 7220  . The lift-over 
+000025b0: 7072 6f62 6c65 6d20 6973 2064 6566 696e  problem is defin
+000025c0: 6564 2061 7320 7468 6520 7072 6f63 6573  ed as the proces
+000025d0: 7320 6f66 2063 6861 6e67 696e 6720 7468  s of changing th
+000025e0: 6520 636f 6f72 6469 6e61 7465 7320 6f66  e coordinates of
+000025f0: 203c 7374 726f 6e67 3e41 6e6e 6f74 6174   <strong>Annotat
+00002600: 696f 6e3c 2f73 7472 6f6e 673e 203c 7370  ion</strong> <sp
+00002610: 616e 2063 6c61 7373 3d22 6d61 7468 206e  an class="math n
+00002620: 6f74 7261 6e73 6c61 7465 206e 6f68 6967  otranslate nohig
+00002630: 686c 6967 6874 223e 3c6d 6a78 2d63 6f6e  hlight"><mjx-con
+00002640: 7461 696e 6572 2063 6c61 7373 3d22 4d61  tainer class="Ma
+00002650: 7468 4a61 7820 4374 7874 4d65 6e75 5f41  thJax CtxtMenu_A
+00002660: 7474 6163 6865 645f 3022 206a 6178 3d22  ttached_0" jax="
+00002670: 4348 544d 4c22 2074 6162 696e 6465 783d  CHTML" tabindex=
+00002680: 2230 2220 6374 7874 6d65 6e75 5f63 6f75  "0" ctxtmenu_cou
+00002690: 6e74 6572 3d22 3322 2073 7479 6c65 3d22  nter="3" style="
+000026a0: 666f 6e74 2d73 697a 653a 2031 3138 2e39  font-size: 118.9
+000026b0: 253b 2070 6f73 6974 696f 6e3a 2072 656c  %; position: rel
+000026c0: 6174 6976 653b 223e 3c6d 6a78 2d6d 6174  ative;"><mjx-mat
+000026d0: 6820 636c 6173 733d 224d 4a58 2d54 4558  h class="MJX-TEX
+000026e0: 2220 6172 6961 2d68 6964 6465 6e3d 2274  " aria-hidden="t
+000026f0: 7275 6522 3e3c 6d6a 782d 6d73 7562 3e3c  rue"><mjx-msub><
+00002700: 6d6a 782d 6d69 2063 6c61 7373 3d22 6d6a  mjx-mi class="mj
+00002710: 782d 6922 3e3c 6d6a 782d 6320 636c 6173  x-i"><mjx-c clas
+00002720: 733d 226d 6a78 2d63 3144 3434 3520 5445  s="mjx-c1D445 TE
+00002730: 582d 4922 3e3c 2f6d 6a78 2d63 3e3c 2f6d  X-I"></mjx-c></m
+00002740: 6a78 2d6d 693e 3c6d 6a78 2d73 6372 6970  jx-mi><mjx-scrip
+00002750: 7420 7374 796c 653d 2276 6572 7469 6361  t style="vertica
+00002760: 6c2d 616c 6967 6e3a 202d 302e 3135 3365  l-align: -0.153e
+00002770: 6d3b 223e 3c6d 6a78 2d6d 6920 636c 6173  m;"><mjx-mi clas
+00002780: 733d 226d 6a78 2d69 2220 7369 7a65 3d22  s="mjx-i" size="
+00002790: 7322 3e3c 6d6a 782d 6320 636c 6173 733d  s"><mjx-c class=
+000027a0: 226d 6a78 2d63 3144 3433 3420 5445 582d  "mjx-c1D434 TEX-
+000027b0: 4922 3e3c 2f6d 6a78 2d63 3e3c 2f6d 6a78  I"></mjx-c></mjx
+000027c0: 2d6d 693e 3c2f 6d6a 782d 7363 7269 7074  -mi></mjx-script
+000027d0: 3e3c 2f6d 6a78 2d6d 7375 623e 3c2f 6d6a  ></mjx-msub></mj
+000027e0: 782d 6d61 7468 3e3c 6d6a 782d 6173 7369  x-math><mjx-assi
+000027f0: 7374 6976 652d 6d6d 6c20 756e 7365 6c65  stive-mml unsele
+00002800: 6374 6162 6c65 3d22 6f6e 2220 6469 7370  ctable="on" disp
+00002810: 6c61 793d 2269 6e6c 696e 6522 3e3c 6d61  lay="inline"><ma
+00002820: 7468 2078 6d6c 6e73 3d22 6874 7470 3a2f  th xmlns="http:/
+00002830: 2f77 7777 2e77 332e 6f72 672f 3139 3938  /www.w3.org/1998
+00002840: 2f4d 6174 682f 4d61 7468 4d4c 223e 3c6d  /Math/MathML"><m
+00002850: 7375 623e 3c6d 693e 523c 2f6d 693e 3c6d  sub><mi>R</mi><m
+00002860: 693e 413c 2f6d 693e 3c2f 6d73 7562 3e3c  i>A</mi></msub><
+00002870: 2f6d 6174 683e 3c2f 6d6a 782d 6173 7369  /math></mjx-assi
+00002880: 7374 6976 652d 6d6d 6c3e 3c2f 6d6a 782d  stive-mml></mjx-
+00002890: 636f 6e74 6169 6e65 723e 3c2f 7370 616e  container></span
+000028a0: 3e20 6672 6f6d 203c 7374 726f 6e67 3e47  > from <strong>G
+000028b0: 656e 6f6d 653c 2f73 7472 6f6e 673e 203c  enome</strong> <
+000028c0: 7370 616e 2063 6c61 7373 3d22 6d61 7468  span class="math
+000028d0: 206e 6f74 7261 6e73 6c61 7465 206e 6f68   notranslate noh
+000028e0: 6967 686c 6967 6874 223e 3c6d 6a78 2d63  ighlight"><mjx-c
+000028f0: 6f6e 7461 696e 6572 2063 6c61 7373 3d22  ontainer class="
+00002900: 4d61 7468 4a61 7820 4374 7874 4d65 6e75  MathJax CtxtMenu
+00002910: 5f41 7474 6163 6865 645f 3022 206a 6178  _Attached_0" jax
+00002920: 3d22 4348 544d 4c22 2074 6162 696e 6465  ="CHTML" tabinde
+00002930: 783d 2230 2220 6374 7874 6d65 6e75 5f63  x="0" ctxtmenu_c
+00002940: 6f75 6e74 6572 3d22 3422 2073 7479 6c65  ounter="4" style
+00002950: 3d22 666f 6e74 2d73 697a 653a 2031 3138  ="font-size: 118
+00002960: 2e39 253b 2070 6f73 6974 696f 6e3a 2072  .9%; position: r
+00002970: 656c 6174 6976 653b 223e 3c6d 6a78 2d6d  elative;"><mjx-m
+00002980: 6174 6820 636c 6173 733d 224d 4a58 2d54  ath class="MJX-T
+00002990: 4558 2220 6172 6961 2d68 6964 6465 6e3d  EX" aria-hidden=
+000029a0: 2274 7275 6522 3e3c 6d6a 782d 6d69 2063  "true"><mjx-mi c
+000029b0: 6c61 7373 3d22 6d6a 782d 6922 3e3c 6d6a  lass="mjx-i"><mj
+000029c0: 782d 6320 636c 6173 733d 226d 6a78 2d63  x-c class="mjx-c
+000029d0: 3144 3434 3520 5445 582d 4922 3e3c 2f6d  1D445 TEX-I"></m
+000029e0: 6a78 2d63 3e3c 2f6d 6a78 2d6d 693e 3c2f  jx-c></mjx-mi></
+000029f0: 6d6a 782d 6d61 7468 3e3c 6d6a 782d 6173  mjx-math><mjx-as
+00002a00: 7369 7374 6976 652d 6d6d 6c20 756e 7365  sistive-mml unse
+00002a10: 6c65 6374 6162 6c65 3d22 6f6e 2220 6469  lectable="on" di
+00002a20: 7370 6c61 793d 2269 6e6c 696e 6522 3e3c  splay="inline"><
+00002a30: 6d61 7468 2078 6d6c 6e73 3d22 6874 7470  math xmlns="http
+00002a40: 3a2f 2f77 7777 2e77 332e 6f72 672f 3139  ://www.w3.org/19
+00002a50: 3938 2f4d 6174 682f 4d61 7468 4d4c 223e  98/Math/MathML">
+00002a60: 3c6d 693e 523c 2f6d 693e 3c2f 6d61 7468  <mi>R</mi></math
+00002a70: 3e3c 2f6d 6a78 2d61 7373 6973 7469 7665  ></mjx-assistive
+00002a80: 2d6d 6d6c 3e3c 2f6d 6a78 2d63 6f6e 7461  -mml></mjx-conta
+00002a90: 696e 6572 3e3c 2f73 7061 6e3e 2074 6f20  iner></span> to 
+00002aa0: 3c73 7472 6f6e 673e 4765 6e6f 6d65 3c2f  <strong>Genome</
+00002ab0: 7374 726f 6e67 3e20 3c73 7061 6e20 636c  strong> <span cl
+00002ac0: 6173 733d 226d 6174 6820 6e6f 7472 616e  ass="math notran
+00002ad0: 736c 6174 6520 6e6f 6869 6768 6c69 6768  slate nohighligh
+00002ae0: 7422 3e3c 6d6a 782d 636f 6e74 6169 6e65  t"><mjx-containe
+00002af0: 7220 636c 6173 733d 224d 6174 684a 6178  r class="MathJax
+00002b00: 2043 7478 744d 656e 755f 4174 7461 6368   CtxtMenu_Attach
+00002b10: 6564 5f30 2220 6a61 783d 2243 4854 4d4c  ed_0" jax="CHTML
+00002b20: 2220 7461 6269 6e64 6578 3d22 3022 2063  " tabindex="0" c
+00002b30: 7478 746d 656e 755f 636f 756e 7465 723d  txtmenu_counter=
+00002b40: 2235 2220 7374 796c 653d 2266 6f6e 742d  "5" style="font-
+00002b50: 7369 7a65 3a20 3131 382e 3925 3b20 706f  size: 118.9%; po
+00002b60: 7369 7469 6f6e 3a20 7265 6c61 7469 7665  sition: relative
+00002b70: 3b22 3e3c 6d6a 782d 6d61 7468 2063 6c61  ;"><mjx-math cla
+00002b80: 7373 3d22 4d4a 582d 5445 5822 2061 7269  ss="MJX-TEX" ari
+00002b90: 612d 6869 6464 656e 3d22 7472 7565 223e  a-hidden="true">
+00002ba0: 3c6d 6a78 2d6d 6920 636c 6173 733d 226d  <mjx-mi class="m
+00002bb0: 6a78 2d69 223e 3c6d 6a78 2d63 2063 6c61  jx-i"><mjx-c cla
+00002bc0: 7373 3d22 6d6a 782d 6331 4434 3437 2054  ss="mjx-c1D447 T
+00002bd0: 4558 2d49 223e 3c2f 6d6a 782d 633e 3c2f  EX-I"></mjx-c></
+00002be0: 6d6a 782d 6d69 3e3c 2f6d 6a78 2d6d 6174  mjx-mi></mjx-mat
+00002bf0: 683e 3c6d 6a78 2d61 7373 6973 7469 7665  h><mjx-assistive
+00002c00: 2d6d 6d6c 2075 6e73 656c 6563 7461 626c  -mml unselectabl
+00002c10: 653d 226f 6e22 2064 6973 706c 6179 3d22  e="on" display="
+00002c20: 696e 6c69 6e65 223e 3c6d 6174 6820 786d  inline"><math xm
+00002c30: 6c6e 733d 2268 7474 703a 2f2f 7777 772e  lns="http://www.
+00002c40: 7733 2e6f 7267 2f31 3939 382f 4d61 7468  w3.org/1998/Math
+00002c50: 2f4d 6174 684d 4c22 3e3c 6d69 3e54 3c2f  /MathML"><mi>T</
+00002c60: 6d69 3e3c 2f6d 6174 683e 3c2f 6d6a 782d  mi></math></mjx-
+00002c70: 6173 7369 7374 6976 652d 6d6d 6c3e 3c2f  assistive-mml></
+00002c80: 6d6a 782d 636f 6e74 6169 6e65 723e 3c2f  mjx-container></
+00002c90: 7370 616e 3e2c 2061 6e64 2067 656e 6572  span>, and gener
+00002ca0: 6174 6520 6120 6e65 7720 616e 6e6f 7461  ate a new annota
+00002cb0: 7469 6f6e 2066 696c 6520 3c73 7472 6f6e  tion file <stron
+00002cc0: 673e 416e 6e6f 7461 7469 6f6e 3c2f 7374  g>Annotation</st
+00002cd0: 726f 6e67 3e20 3c73 7061 6e20 636c 6173  rong> <span clas
+00002ce0: 733d 226d 6174 6820 6e6f 7472 616e 736c  s="math notransl
+00002cf0: 6174 6520 6e6f 6869 6768 6c69 6768 7422  ate nohighlight"
+00002d00: 3e3c 6d6a 782d 636f 6e74 6169 6e65 7220  ><mjx-container 
+00002d10: 636c 6173 733d 224d 6174 684a 6178 2043  class="MathJax C
+00002d20: 7478 744d 656e 755f 4174 7461 6368 6564  txtMenu_Attached
+00002d30: 5f30 2220 6a61 783d 2243 4854 4d4c 2220  _0" jax="CHTML" 
+00002d40: 7461 6269 6e64 6578 3d22 3022 2063 7478  tabindex="0" ctx
+00002d50: 746d 656e 755f 636f 756e 7465 723d 2236  tmenu_counter="6
+00002d60: 2220 7374 796c 653d 2266 6f6e 742d 7369  " style="font-si
+00002d70: 7a65 3a20 3131 382e 3925 3b20 706f 7369  ze: 118.9%; posi
+00002d80: 7469 6f6e 3a20 7265 6c61 7469 7665 3b22  tion: relative;"
+00002d90: 3e3c 6d6a 782d 6d61 7468 2063 6c61 7373  ><mjx-math class
+00002da0: 3d22 4d4a 582d 5445 5822 2061 7269 612d  ="MJX-TEX" aria-
+00002db0: 6869 6464 656e 3d22 7472 7565 223e 3c6d  hidden="true"><m
+00002dc0: 6a78 2d6d 7375 623e 3c6d 6a78 2d6d 6920  jx-msub><mjx-mi 
+00002dd0: 636c 6173 733d 226d 6a78 2d69 223e 3c6d  class="mjx-i"><m
+00002de0: 6a78 2d63 2063 6c61 7373 3d22 6d6a 782d  jx-c class="mjx-
+00002df0: 6331 4434 3437 2054 4558 2d49 223e 3c2f  c1D447 TEX-I"></
+00002e00: 6d6a 782d 633e 3c2f 6d6a 782d 6d69 3e3c  mjx-c></mjx-mi><
+00002e10: 6d6a 782d 7363 7269 7074 2073 7479 6c65  mjx-script style
+00002e20: 3d22 7665 7274 6963 616c 2d61 6c69 676e  ="vertical-align
+00002e30: 3a20 2d30 2e31 3533 656d 3b20 6d61 7267  : -0.153em; marg
+00002e40: 696e 2d6c 6566 743a 202d 302e 3132 656d  in-left: -0.12em
+00002e50: 3b22 3e3c 6d6a 782d 6d69 2063 6c61 7373  ;"><mjx-mi class
+00002e60: 3d22 6d6a 782d 6922 2073 697a 653d 2273  ="mjx-i" size="s
+00002e70: 223e 3c6d 6a78 2d63 2063 6c61 7373 3d22  "><mjx-c class="
+00002e80: 6d6a 782d 6331 4434 3334 2054 4558 2d49  mjx-c1D434 TEX-I
+00002e90: 223e 3c2f 6d6a 782d 633e 3c2f 6d6a 782d  "></mjx-c></mjx-
+00002ea0: 6d69 3e3c 2f6d 6a78 2d73 6372 6970 743e  mi></mjx-script>
+00002eb0: 3c2f 6d6a 782d 6d73 7562 3e3c 2f6d 6a78  </mjx-msub></mjx
+00002ec0: 2d6d 6174 683e 3c6d 6a78 2d61 7373 6973  -math><mjx-assis
+00002ed0: 7469 7665 2d6d 6d6c 2075 6e73 656c 6563  tive-mml unselec
+00002ee0: 7461 626c 653d 226f 6e22 2064 6973 706c  table="on" displ
+00002ef0: 6179 3d22 696e 6c69 6e65 223e 3c6d 6174  ay="inline"><mat
+00002f00: 6820 786d 6c6e 733d 2268 7474 703a 2f2f  h xmlns="http://
+00002f10: 7777 772e 7733 2e6f 7267 2f31 3939 382f  www.w3.org/1998/
+00002f20: 4d61 7468 2f4d 6174 684d 4c22 3e3c 6d73  Math/MathML"><ms
+00002f30: 7562 3e3c 6d69 3e54 3c2f 6d69 3e3c 6d69  ub><mi>T</mi><mi
+00002f40: 3e41 3c2f 6d69 3e3c 2f6d 7375 623e 3c2f  >A</mi></msub></
+00002f50: 6d61 7468 3e3c 2f6d 6a78 2d61 7373 6973  math></mjx-assis
+00002f60: 7469 7665 2d6d 6d6c 3e3c 2f6d 6a78 2d63  tive-mml></mjx-c
+00002f70: 6f6e 7461 696e 6572 3e3c 2f73 7061 6e3e  ontainer></span>
+00002f80: 2e20 4120 7369 6d70 6c65 2069 6c6c 7573  . A simple illus
+00002f90: 7472 6174 696f 6e20 6f66 2074 6865 206c  tration of the l
+00002fa0: 6966 742d 6f76 6572 2070 726f 626c 656d  ift-over problem
+00002fb0: 2069 7320 7368 6f77 6e20 696e 203c 6120   is shown in <a 
+00002fc0: 636c 6173 733d 2272 6566 6572 656e 6365  class="reference
+00002fd0: 2069 6e74 6572 6e61 6c22 2068 7265 663d   internal" href=
+00002fe0: 2223 6c69 6674 6f76 6572 2d69 6c6c 7573  "#liftover-illus
+00002ff0: 7472 6174 696f 6e22 3e3c 7370 616e 2063  tration"><span c
+00003000: 6c61 7373 3d22 7374 6420 7374 642d 6e75  lass="std std-nu
+00003010: 6d72 6566 223e 4669 6775 7265 2031 3c2f  mref">Figure 1</
+00003020: 7370 616e 3e3c 2f61 3e2e 3c2f 703e 0a3c  span></a>.</p>.<
+00003030: 6669 6775 7265 2063 6c61 7373 3d22 616c  figure class="al
+00003040: 6967 6e2d 6365 6e74 6572 2220 6964 3d22  ign-center" id="
+00003050: 6964 3422 3e0a 3c66 6967 6361 7074 696f  id4">.<figcaptio
+00003060: 6e3e 0a3c 7370 616e 2069 643d 226c 6966  n>.<span id="lif
+00003070: 746f 7665 722d 696c 6c75 7374 7261 7469  tover-illustrati
+00003080: 6f6e 223e 3c2f 7370 616e 3e3c 6120 636c  on"></span><a cl
+00003090: 6173 733d 2272 6566 6572 656e 6365 2069  ass="reference i
+000030a0: 6e74 6572 6e61 6c20 696d 6167 652d 7265  nternal image-re
+000030b0: 6665 7265 6e63 6522 2068 7265 663d 2268  ference" href="h
+000030c0: 7474 7073 3a2f 2f73 746f 7261 6765 2e67  ttps://storage.g
+000030d0: 6f6f 676c 6561 7069 732e 636f 6d2f 7374  oogleapis.com/st
+000030e0: 6f72 6167 652e 6b68 6368 616f 2e63 6f6d  orage.khchao.com
+000030f0: 2f66 6967 7572 6573 2f4c 6966 744f 6e2f  /figures/LiftOn/
+00003100: 6c69 6674 6f76 6572 5f69 6c6c 7573 7472  liftover_illustr
+00003110: 6174 696f 6e2e 6769 6622 3e3c 696d 6720  ation.gif"><img 
+00003120: 616c 743d 2267 7261 7068 6963 732f 6c69  alt="graphics/li
+00003130: 6674 6f76 6572 5f69 6c6c 7573 7472 6174  ftover_illustrat
+00003140: 696f 6e2e 6769 6622 2073 7263 3d22 6874  ion.gif" src="ht
+00003150: 7470 733a 2f2f 7374 6f72 6167 652e 676f  tps://storage.go
+00003160: 6f67 6c65 6170 6973 2e63 6f6d 2f73 746f  ogleapis.com/sto
+00003170: 7261 6765 2e6b 6863 6861 6f2e 636f 6d2f  rage.khchao.com/
+00003180: 6669 6775 7265 732f 4c69 6674 4f6e 2f6c  figures/LiftOn/l
+00003190: 6966 746f 7665 725f 696c 6c75 7374 7261  iftover_illustra
+000031a0: 7469 6f6e 2e67 6966 2220 7374 796c 653d  tion.gif" style=
+000031b0: 2277 6964 7468 3a20 3637 322e 3570 783b  "width: 672.5px;
+000031c0: 2068 6569 6768 743a 2032 3730 2e30 7078   height: 270.0px
+000031d0: 3b22 3e3c 2f61 3e0a 3c2f 6669 6763 6170  ;"></a>.</figcap
+000031e0: 7469 6f6e 3e0a 3c2f 6669 6775 7265 3e0a  tion>.</figure>.
+000031f0: 3c64 6976 2063 6c61 7373 3d22 6c69 6e65  <div class="line
+00003200: 2d62 6c6f 636b 223e 0a3c 6469 7620 636c  -block">.<div cl
+00003210: 6173 733d 226c 696e 6522 3e3c 6272 3e3c  ass="line"><br><
+00003220: 2f64 6976 3e0a 3c2f 6469 763e 0a3c 703e  /div>.</div>.<p>
+00003230: 4c69 6674 4f6e 2069 7320 7468 6520 6265  LiftOn is the be
+00003240: 7374 2074 6f6f 6c20 746f 2068 656c 7020  st tool to help 
+00003250: 796f 7520 736f 6c76 6520 7468 6973 2070  you solve this p
+00003260: 726f 626c 656d 2120 4c69 6674 4f6e 2065  roblem! LiftOn e
+00003270: 6d70 6c6f 7973 2061 2074 776f 2d73 7465  mploys a two-ste
+00003280: 7020 3c61 2063 6c61 7373 3d22 7265 6665  p <a class="refe
+00003290: 7265 6e63 6520 696e 7465 726e 616c 2220  rence internal" 
+000032a0: 6872 6566 3d22 6874 7470 733a 2f2f 6363  href="https://cc
+000032b0: 622e 6a68 752e 6564 752f 6c69 6674 6f6e  b.jhu.edu/lifton
+000032c0: 2f63 6f6e 7465 6e74 2f62 6568 696e 645f  /content/behind_
+000032d0: 7363 656e 6573 2e68 746d 6c23 7072 6f74  scenes.html#prot
+000032e0: 6569 6e2d 6d61 7869 6d69 7a61 7469 6f6e  ein-maximization
+000032f0: 2d61 6c67 6f72 6974 686d 223e 3c73 7061  -algorithm"><spa
+00003300: 6e20 636c 6173 733d 2273 7464 2073 7464  n class="std std
+00003310: 2d72 6566 223e 7072 6f74 6569 6e20 6d61  -ref">protein ma
+00003320: 7869 6d69 7a61 7469 6f6e 2061 6c67 6f72  ximization algor
+00003330: 6974 686d 3c2f 7370 616e 3e3c 2f61 3e20  ithm</span></a> 
+00003340: 2850 4d20 616c 676f 7269 7468 6d29 2e3c  (PM algorithm).<
+00003350: 2f70 3e0a 3c6f 6c20 636c 6173 733d 2261  /p>.<ol class="a
+00003360: 7261 6269 6320 7369 6d70 6c65 223e 0a3c  rabic simple">.<
+00003370: 6c69 3e3c 703e 5468 6520 6669 7273 7420  li><p>The first 
+00003380: 6d6f 6475 6c65 2069 7320 7468 6520 3c65  module is the <e
+00003390: 6d3e 6368 6169 6e69 6e67 2061 6c67 6f72  m>chaining algor
+000033a0: 6974 686d 3c2f 656d 3e2e 2049 7420 7374  ithm</em>. It st
+000033b0: 6172 7473 2062 7920 6578 7472 6163 7469  arts by extracti
+000033c0: 6e67 2070 726f 7465 696e 2073 6571 7565  ng protein seque
+000033d0: 6e63 6573 2061 6e6e 6f74 6174 6564 2062  nces annotated b
+000033e0: 7920 4c69 6674 6f66 6620 616e 6420 6d69  y Liftoff and mi
+000033f0: 6e69 7072 6f74 2e20 4c69 6674 4f6e 2074  niprot. LiftOn t
+00003400: 6865 6e20 616c 6967 6e73 2074 6865 7365  hen aligns these
+00003410: 2073 6571 7565 6e63 6573 2074 6f20 6675   sequences to fu
+00003420: 6c6c 2d6c 656e 6774 6820 7265 6665 7265  ll-length refere
+00003430: 6e63 6520 7072 6f74 6569 6e73 2e20 466f  nce proteins. Fo
+00003440: 7220 6561 6368 2067 656e 6520 6c6f 6375  r each gene locu
+00003450: 732c 204c 6966 744f 6e20 636f 6d70 6172  s, LiftOn compar
+00003460: 6573 2065 6163 6820 7365 6374 696f 6e20  es each section 
+00003470: 6f66 2074 6865 2070 726f 7465 696e 2061  of the protein a
+00003480: 6c69 676e 6d65 6e74 7320 6672 6f6d 204c  lignments from L
+00003490: 6966 746f 6666 2061 6e64 206d 696e 6970  iftoff and minip
+000034a0: 726f 742c 2063 6861 696e 696e 6720 746f  rot, chaining to
+000034b0: 6765 7468 6572 2074 6865 2062 6573 7420  gether the best 
+000034c0: 636f 6d62 696e 6174 696f 6e73 2e3c 2f70  combinations.</p
+000034d0: 3e3c 2f6c 693e 0a3c 6c69 3e3c 703e 5468  ></li>.<li><p>Th
+000034e0: 6520 7365 636f 6e64 206d 6f64 756c 6520  e second module 
+000034f0: 6973 2074 6865 203c 656d 3e6f 7065 6e2d  is the <em>open-
+00003500: 7265 6164 696e 6720 6672 616d 6520 7365  reading frame se
+00003510: 6172 6368 2028 4f52 4620 7365 6172 6368  arch (ORF search
+00003520: 2920 616c 676f 7269 7468 6d3c 2f65 6d3e  ) algorithm</em>
+00003530: 2e20 496e 2074 6865 2063 6173 6520 6f66  . In the case of
+00003540: 2074 7275 6e63 6174 6564 2070 726f 7465   truncated prote
+00003550: 696e 2d63 6f64 696e 6720 7472 616e 7363  in-coding transc
+00003560: 7269 7074 732c 2074 6869 7320 616c 676f  ripts, this algo
+00003570: 7269 7468 6d20 6578 616d 696e 6573 2061  rithm examines a
+00003580: 6c74 6572 6e61 7469 7665 2066 7261 6d65  lternative frame
+00003590: 7320 746f 2069 6465 6e74 6966 7920 7468  s to identify th
+000035a0: 6520 4f52 4620 7468 6174 2070 726f 6475  e ORF that produ
+000035b0: 6365 7320 7468 6520 6c6f 6e67 6573 7420  ces the longest 
+000035c0: 6d61 7463 6820 7769 7468 2074 6865 2072  match with the r
+000035d0: 6566 6572 656e 6365 2070 726f 7465 696e  eference protein
+000035e0: 2e3c 2f70 3e3c 2f6c 693e 0a3c 2f6f 6c3e  .</p></li>.</ol>
+000035f0: 0a3c 6469 7620 636c 6173 733d 226c 696e  .<div class="lin
+00003600: 652d 626c 6f63 6b22 3e0a 3c64 6976 2063  e-block">.<div c
+00003610: 6c61 7373 3d22 6c69 6e65 223e 3c62 723e  lass="line"><br>
+00003620: 3c2f 6469 763e 0a3c 2f64 6976 3e0a 3c2f  </div>.</div>.</
+00003630: 7365 6374 696f 6e3e 0a3c 7365 6374 696f  section>.<sectio
+00003640: 6e20 6964 3d22 696e 7075 7473 2d6f 7574  n id="inputs-out
+00003650: 7075 7473 2220 636c 6173 733d 2222 3e0a  puts" class="">.
+00003660: 3c68 323e 496e 7075 7473 2026 616d 703b  <h2>Inputs &amp;
+00003670: 206f 7574 7075 7473 3c61 2063 6c61 7373   outputs<a class
+00003680: 3d22 6865 6164 6572 6c69 6e6b 2220 6872  ="headerlink" hr
+00003690: 6566 3d22 2369 6e70 7574 732d 6f75 7470  ef="#inputs-outp
+000036a0: 7574 7322 2074 6974 6c65 3d22 5065 726d  uts" title="Perm
+000036b0: 616c 696e 6b20 746f 2074 6869 7320 6865  alink to this he
+000036c0: 6164 696e 6722 3e23 3c2f 613e 3c2f 6832  ading">#</a></h2
+000036d0: 3e0a 3c75 6c20 636c 6173 733d 2273 696d  >.<ul class="sim
+000036e0: 706c 6522 3e0a 3c6c 693e 3c64 6c20 636c  ple">.<li><dl cl
+000036f0: 6173 733d 2273 696d 706c 6522 3e0a 3c64  ass="simple">.<d
+00003700: 743e 3c73 7472 6f6e 673e 496e 7075 743c  t><strong>Input<
+00003710: 2f73 7472 6f6e 673e 3a3c 2f64 743e 3c64  /strong>:</dt><d
+00003720: 643e 3c6f 6c20 636c 6173 733d 2261 7261  d><ol class="ara
+00003730: 6269 6320 7369 6d70 6c65 223e 0a3c 6c69  bic simple">.<li
+00003740: 3e3c 703e 7461 7267 6574 203c 7374 726f  ><p>target <stro
+00003750: 6e67 3e47 656e 6f6d 653c 2f73 7472 6f6e  ng>Genome</stron
+00003760: 673e 203c 7370 616e 2063 6c61 7373 3d22  g> <span class="
+00003770: 6d61 7468 206e 6f74 7261 6e73 6c61 7465  math notranslate
+00003780: 206e 6f68 6967 686c 6967 6874 223e 3c6d   nohighlight"><m
+00003790: 6a78 2d63 6f6e 7461 696e 6572 2063 6c61  jx-container cla
+000037a0: 7373 3d22 4d61 7468 4a61 7820 4374 7874  ss="MathJax Ctxt
+000037b0: 4d65 6e75 5f41 7474 6163 6865 645f 3022  Menu_Attached_0"
+000037c0: 206a 6178 3d22 4348 544d 4c22 2074 6162   jax="CHTML" tab
+000037d0: 696e 6465 783d 2230 2220 6374 7874 6d65  index="0" ctxtme
+000037e0: 6e75 5f63 6f75 6e74 6572 3d22 3722 2073  nu_counter="7" s
+000037f0: 7479 6c65 3d22 666f 6e74 2d73 697a 653a  tyle="font-size:
+00003800: 2031 3138 2e39 253b 2070 6f73 6974 696f   118.9%; positio
+00003810: 6e3a 2072 656c 6174 6976 653b 223e 3c6d  n: relative;"><m
+00003820: 6a78 2d6d 6174 6820 636c 6173 733d 224d  jx-math class="M
+00003830: 4a58 2d54 4558 2220 6172 6961 2d68 6964  JX-TEX" aria-hid
+00003840: 6465 6e3d 2274 7275 6522 3e3c 6d6a 782d  den="true"><mjx-
+00003850: 6d69 2063 6c61 7373 3d22 6d6a 782d 6922  mi class="mjx-i"
+00003860: 3e3c 6d6a 782d 6320 636c 6173 733d 226d  ><mjx-c class="m
+00003870: 6a78 2d63 3144 3434 3720 5445 582d 4922  jx-c1D447 TEX-I"
+00003880: 3e3c 2f6d 6a78 2d63 3e3c 2f6d 6a78 2d6d  ></mjx-c></mjx-m
+00003890: 693e 3c2f 6d6a 782d 6d61 7468 3e3c 6d6a  i></mjx-math><mj
+000038a0: 782d 6173 7369 7374 6976 652d 6d6d 6c20  x-assistive-mml 
+000038b0: 756e 7365 6c65 6374 6162 6c65 3d22 6f6e  unselectable="on
+000038c0: 2220 6469 7370 6c61 793d 2269 6e6c 696e  " display="inlin
+000038d0: 6522 3e3c 6d61 7468 2078 6d6c 6e73 3d22  e"><math xmlns="
+000038e0: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
+000038f0: 672f 3139 3938 2f4d 6174 682f 4d61 7468  g/1998/Math/Math
+00003900: 4d4c 223e 3c6d 693e 543c 2f6d 693e 3c2f  ML"><mi>T</mi></
+00003910: 6d61 7468 3e3c 2f6d 6a78 2d61 7373 6973  math></mjx-assis
+00003920: 7469 7665 2d6d 6d6c 3e3c 2f6d 6a78 2d63  tive-mml></mjx-c
+00003930: 6f6e 7461 696e 6572 3e3c 2f73 7061 6e3e  ontainer></span>
+00003940: 2069 6e20 4641 5354 4120 666f 726d 6174   in FASTA format
+00003950: 2e3c 2f70 3e3c 2f6c 693e 0a3c 6c69 3e3c  .</p></li>.<li><
+00003960: 703e 7265 6665 7265 6e63 6520 3c73 7472  p>reference <str
+00003970: 6f6e 673e 4765 6e6f 6d65 3c2f 7374 726f  ong>Genome</stro
+00003980: 6e67 3e20 3c73 7061 6e20 636c 6173 733d  ng> <span class=
+00003990: 226d 6174 6820 6e6f 7472 616e 736c 6174  "math notranslat
+000039a0: 6520 6e6f 6869 6768 6c69 6768 7422 3e3c  e nohighlight"><
+000039b0: 6d6a 782d 636f 6e74 6169 6e65 7220 636c  mjx-container cl
+000039c0: 6173 733d 224d 6174 684a 6178 2043 7478  ass="MathJax Ctx
+000039d0: 744d 656e 755f 4174 7461 6368 6564 5f30  tMenu_Attached_0
+000039e0: 2220 6a61 783d 2243 4854 4d4c 2220 7461  " jax="CHTML" ta
+000039f0: 6269 6e64 6578 3d22 3022 2063 7478 746d  bindex="0" ctxtm
+00003a00: 656e 755f 636f 756e 7465 723d 2238 2220  enu_counter="8" 
+00003a10: 7374 796c 653d 2266 6f6e 742d 7369 7a65  style="font-size
+00003a20: 3a20 3131 382e 3925 3b20 706f 7369 7469  : 118.9%; positi
+00003a30: 6f6e 3a20 7265 6c61 7469 7665 3b22 3e3c  on: relative;"><
+00003a40: 6d6a 782d 6d61 7468 2063 6c61 7373 3d22  mjx-math class="
+00003a50: 4d4a 582d 5445 5822 2061 7269 612d 6869  MJX-TEX" aria-hi
+00003a60: 6464 656e 3d22 7472 7565 223e 3c6d 6a78  dden="true"><mjx
+00003a70: 2d6d 6920 636c 6173 733d 226d 6a78 2d69  -mi class="mjx-i
+00003a80: 223e 3c6d 6a78 2d63 2063 6c61 7373 3d22  "><mjx-c class="
+00003a90: 6d6a 782d 6331 4434 3435 2054 4558 2d49  mjx-c1D445 TEX-I
+00003aa0: 223e 3c2f 6d6a 782d 633e 3c2f 6d6a 782d  "></mjx-c></mjx-
+00003ab0: 6d69 3e3c 2f6d 6a78 2d6d 6174 683e 3c6d  mi></mjx-math><m
+00003ac0: 6a78 2d61 7373 6973 7469 7665 2d6d 6d6c  jx-assistive-mml
+00003ad0: 2075 6e73 656c 6563 7461 626c 653d 226f   unselectable="o
+00003ae0: 6e22 2064 6973 706c 6179 3d22 696e 6c69  n" display="inli
+00003af0: 6e65 223e 3c6d 6174 6820 786d 6c6e 733d  ne"><math xmlns=
+00003b00: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
+00003b10: 7267 2f31 3939 382f 4d61 7468 2f4d 6174  rg/1998/Math/Mat
+00003b20: 684d 4c22 3e3c 6d69 3e52 3c2f 6d69 3e3c  hML"><mi>R</mi><
+00003b30: 2f6d 6174 683e 3c2f 6d6a 782d 6173 7369  /math></mjx-assi
+00003b40: 7374 6976 652d 6d6d 6c3e 3c2f 6d6a 782d  stive-mml></mjx-
+00003b50: 636f 6e74 6169 6e65 723e 3c2f 7370 616e  container></span
+00003b60: 3e20 696e 2046 4153 5441 2066 6f72 6d61  > in FASTA forma
+00003b70: 742e 3c2f 703e 3c2f 6c69 3e0a 3c6c 693e  t.</p></li>.<li>
+00003b80: 3c70 3e72 6566 6572 656e 6365 203c 7374  <p>reference <st
+00003b90: 726f 6e67 3e41 6e6e 6f74 6174 696f 6e3c  rong>Annotation<
+00003ba0: 2f73 7472 6f6e 673e 203c 7370 616e 2063  /strong> <span c
+00003bb0: 6c61 7373 3d22 6d61 7468 206e 6f74 7261  lass="math notra
+00003bc0: 6e73 6c61 7465 206e 6f68 6967 686c 6967  nslate nohighlig
+00003bd0: 6874 223e 3c6d 6a78 2d63 6f6e 7461 696e  ht"><mjx-contain
+00003be0: 6572 2063 6c61 7373 3d22 4d61 7468 4a61  er class="MathJa
+00003bf0: 7820 4374 7874 4d65 6e75 5f41 7474 6163  x CtxtMenu_Attac
+00003c00: 6865 645f 3022 206a 6178 3d22 4348 544d  hed_0" jax="CHTM
+00003c10: 4c22 2074 6162 696e 6465 783d 2230 2220  L" tabindex="0" 
+00003c20: 6374 7874 6d65 6e75 5f63 6f75 6e74 6572  ctxtmenu_counter
+00003c30: 3d22 3922 2073 7479 6c65 3d22 666f 6e74  ="9" style="font
+00003c40: 2d73 697a 653a 2031 3138 2e39 253b 2070  -size: 118.9%; p
+00003c50: 6f73 6974 696f 6e3a 2072 656c 6174 6976  osition: relativ
+00003c60: 653b 223e 3c6d 6a78 2d6d 6174 6820 636c  e;"><mjx-math cl
+00003c70: 6173 733d 224d 4a58 2d54 4558 2220 6172  ass="MJX-TEX" ar
+00003c80: 6961 2d68 6964 6465 6e3d 2274 7275 6522  ia-hidden="true"
+00003c90: 3e3c 6d6a 782d 6d73 7562 3e3c 6d6a 782d  ><mjx-msub><mjx-
+00003ca0: 6d69 2063 6c61 7373 3d22 6d6a 782d 6922  mi class="mjx-i"
+00003cb0: 3e3c 6d6a 782d 6320 636c 6173 733d 226d  ><mjx-c class="m
+00003cc0: 6a78 2d63 3144 3434 3520 5445 582d 4922  jx-c1D445 TEX-I"
+00003cd0: 3e3c 2f6d 6a78 2d63 3e3c 2f6d 6a78 2d6d  ></mjx-c></mjx-m
+00003ce0: 693e 3c6d 6a78 2d73 6372 6970 7420 7374  i><mjx-script st
+00003cf0: 796c 653d 2276 6572 7469 6361 6c2d 616c  yle="vertical-al
+00003d00: 6967 6e3a 202d 302e 3135 3365 6d3b 223e  ign: -0.153em;">
+00003d10: 3c6d 6a78 2d6d 6920 636c 6173 733d 226d  <mjx-mi class="m
+00003d20: 6a78 2d69 2220 7369 7a65 3d22 7322 3e3c  jx-i" size="s"><
+00003d30: 6d6a 782d 6320 636c 6173 733d 226d 6a78  mjx-c class="mjx
+00003d40: 2d63 3144 3433 3420 5445 582d 4922 3e3c  -c1D434 TEX-I"><
+00003d50: 2f6d 6a78 2d63 3e3c 2f6d 6a78 2d6d 693e  /mjx-c></mjx-mi>
+00003d60: 3c2f 6d6a 782d 7363 7269 7074 3e3c 2f6d  </mjx-script></m
+00003d70: 6a78 2d6d 7375 623e 3c2f 6d6a 782d 6d61  jx-msub></mjx-ma
+00003d80: 7468 3e3c 6d6a 782d 6173 7369 7374 6976  th><mjx-assistiv
+00003d90: 652d 6d6d 6c20 756e 7365 6c65 6374 6162  e-mml unselectab
+00003da0: 6c65 3d22 6f6e 2220 6469 7370 6c61 793d  le="on" display=
+00003db0: 2269 6e6c 696e 6522 3e3c 6d61 7468 2078  "inline"><math x
+00003dc0: 6d6c 6e73 3d22 6874 7470 3a2f 2f77 7777  mlns="http://www
+00003dd0: 2e77 332e 6f72 672f 3139 3938 2f4d 6174  .w3.org/1998/Mat
+00003de0: 682f 4d61 7468 4d4c 223e 3c6d 7375 623e  h/MathML"><msub>
+00003df0: 3c6d 693e 523c 2f6d 693e 3c6d 693e 413c  <mi>R</mi><mi>A<
+00003e00: 2f6d 693e 3c2f 6d73 7562 3e3c 2f6d 6174  /mi></msub></mat
+00003e10: 683e 3c2f 6d6a 782d 6173 7369 7374 6976  h></mjx-assistiv
+00003e20: 652d 6d6d 6c3e 3c2f 6d6a 782d 636f 6e74  e-mml></mjx-cont
+00003e30: 6169 6e65 723e 3c2f 7370 616e 3e20 696e  ainer></span> in
+00003e40: 2047 4646 3320 666f 726d 6174 2e3c 2f70   GFF3 format.</p
+00003e50: 3e3c 2f6c 693e 0a3c 2f6f 6c3e 0a3c 2f64  ></li>.</ol>.</d
+00003e60: 643e 0a3c 2f64 6c3e 0a3c 2f6c 693e 0a3c  d>.</dl>.</li>.<
+00003e70: 6c69 3e3c 646c 2063 6c61 7373 3d22 7369  li><dl class="si
+00003e80: 6d70 6c65 223e 0a3c 6474 3e3c 7374 726f  mple">.<dt><stro
+00003e90: 6e67 3e4f 7574 7075 743c 2f73 7472 6f6e  ng>Output</stron
+00003ea0: 673e 3a3c 2f64 743e 3c64 643e 3c6f 6c20  g>:</dt><dd><ol 
+00003eb0: 636c 6173 733d 2261 7261 6269 6320 7369  class="arabic si
+00003ec0: 6d70 6c65 223e 0a3c 6c69 3e3c 703e 4c69  mple">.<li><p>Li
+00003ed0: 6674 4f6e 2061 6e6e 6f74 6174 696f 6e20  ftOn annotation 
+00003ee0: 6669 6c65 2c20 3c73 7472 6f6e 673e 416e  file, <strong>An
+00003ef0: 6e6f 7461 7469 6f6e 3c2f 7374 726f 6e67  notation</strong
+00003f00: 3e20 3c73 7061 6e20 636c 6173 733d 226d  > <span class="m
+00003f10: 6174 6820 6e6f 7472 616e 736c 6174 6520  ath notranslate 
+00003f20: 6e6f 6869 6768 6c69 6768 7422 3e3c 6d6a  nohighlight"><mj
+00003f30: 782d 636f 6e74 6169 6e65 7220 636c 6173  x-container clas
+00003f40: 733d 224d 6174 684a 6178 2043 7478 744d  s="MathJax CtxtM
+00003f50: 656e 755f 4174 7461 6368 6564 5f30 2220  enu_Attached_0" 
+00003f60: 6a61 783d 2243 4854 4d4c 2220 7461 6269  jax="CHTML" tabi
+00003f70: 6e64 6578 3d22 3022 2063 7478 746d 656e  ndex="0" ctxtmen
+00003f80: 755f 636f 756e 7465 723d 2231 3022 2073  u_counter="10" s
+00003f90: 7479 6c65 3d22 666f 6e74 2d73 697a 653a  tyle="font-size:
+00003fa0: 2031 3138 2e39 253b 2070 6f73 6974 696f   118.9%; positio
+00003fb0: 6e3a 2072 656c 6174 6976 653b 223e 3c6d  n: relative;"><m
+00003fc0: 6a78 2d6d 6174 6820 636c 6173 733d 224d  jx-math class="M
+00003fd0: 4a58 2d54 4558 2220 6172 6961 2d68 6964  JX-TEX" aria-hid
+00003fe0: 6465 6e3d 2274 7275 6522 3e3c 6d6a 782d  den="true"><mjx-
+00003ff0: 6d73 7562 3e3c 6d6a 782d 6d69 2063 6c61  msub><mjx-mi cla
+00004000: 7373 3d22 6d6a 782d 6922 3e3c 6d6a 782d  ss="mjx-i"><mjx-
+00004010: 6320 636c 6173 733d 226d 6a78 2d63 3144  c class="mjx-c1D
+00004020: 3434 3720 5445 582d 4922 3e3c 2f6d 6a78  447 TEX-I"></mjx
+00004030: 2d63 3e3c 2f6d 6a78 2d6d 693e 3c6d 6a78  -c></mjx-mi><mjx
+00004040: 2d73 6372 6970 7420 7374 796c 653d 2276  -script style="v
+00004050: 6572 7469 6361 6c2d 616c 6967 6e3a 202d  ertical-align: -
+00004060: 302e 3135 3365 6d3b 206d 6172 6769 6e2d  0.153em; margin-
+00004070: 6c65 6674 3a20 2d30 2e31 3265 6d3b 223e  left: -0.12em;">
+00004080: 3c6d 6a78 2d6d 6920 636c 6173 733d 226d  <mjx-mi class="m
+00004090: 6a78 2d69 2220 7369 7a65 3d22 7322 3e3c  jx-i" size="s"><
+000040a0: 6d6a 782d 6320 636c 6173 733d 226d 6a78  mjx-c class="mjx
+000040b0: 2d63 3144 3433 3420 5445 582d 4922 3e3c  -c1D434 TEX-I"><
+000040c0: 2f6d 6a78 2d63 3e3c 2f6d 6a78 2d6d 693e  /mjx-c></mjx-mi>
+000040d0: 3c2f 6d6a 782d 7363 7269 7074 3e3c 2f6d  </mjx-script></m
+000040e0: 6a78 2d6d 7375 623e 3c2f 6d6a 782d 6d61  jx-msub></mjx-ma
+000040f0: 7468 3e3c 6d6a 782d 6173 7369 7374 6976  th><mjx-assistiv
+00004100: 652d 6d6d 6c20 756e 7365 6c65 6374 6162  e-mml unselectab
+00004110: 6c65 3d22 6f6e 2220 6469 7370 6c61 793d  le="on" display=
+00004120: 2269 6e6c 696e 6522 3e3c 6d61 7468 2078  "inline"><math x
+00004130: 6d6c 6e73 3d22 6874 7470 3a2f 2f77 7777  mlns="http://www
+00004140: 2e77 332e 6f72 672f 3139 3938 2f4d 6174  .w3.org/1998/Mat
+00004150: 682f 4d61 7468 4d4c 223e 3c6d 7375 623e  h/MathML"><msub>
+00004160: 3c6d 693e 543c 2f6d 693e 3c6d 693e 413c  <mi>T</mi><mi>A<
+00004170: 2f6d 693e 3c2f 6d73 7562 3e3c 2f6d 6174  /mi></msub></mat
+00004180: 683e 3c2f 6d6a 782d 6173 7369 7374 6976  h></mjx-assistiv
+00004190: 652d 6d6d 6c3e 3c2f 6d6a 782d 636f 6e74  e-mml></mjx-cont
+000041a0: 6169 6e65 723e 3c2f 7370 616e 3e2c 2069  ainer></span>, i
+000041b0: 6e20 4746 4633 2066 6f72 6d61 742e 3c2f  n GFF3 format.</
+000041c0: 703e 3c2f 6c69 3e0a 3c6c 693e 3c70 3e50  p></li>.<li><p>P
+000041d0: 726f 7465 696e 2073 6571 7565 6e63 6520  rotein sequence 
+000041e0: 6964 656e 7469 7469 6573 2026 616d 703b  identities &amp;
+000041f0: 206d 7574 6174 696f 6e20 7479 7065 733c   mutation types<
+00004200: 2f70 3e3c 2f6c 693e 0a3c 6c69 3e3c 703e  /p></li>.<li><p>
+00004210: 4665 6174 7572 6573 2077 6974 6820 6578  Features with ex
+00004220: 7472 6120 636f 7069 6573 3c2f 703e 3c2f  tra copies</p></
+00004230: 6c69 3e0a 3c6c 693e 3c70 3e55 6e6d 6170  li>.<li><p>Unmap
+00004240: 7065 6420 6665 6174 7572 6573 3c2f 703e  ped features</p>
+00004250: 3c2f 6c69 3e0a 3c2f 6f6c 3e0a 3c2f 6464  </li>.</ol>.</dd
+00004260: 3e0a 3c2f 646c 3e0a 3c2f 6c69 3e0a 3c2f  >.</dl>.</li>.</
+00004270: 756c 3e0a 3c64 6976 2063 6c61 7373 3d22  ul>.<div class="
+00004280: 6c69 6e65 2d62 6c6f 636b 223e 0a3c 6469  line-block">.<di
+00004290: 7620 636c 6173 733d 226c 696e 6522 3e3c  v class="line"><
+000042a0: 6272 3e3c 2f64 6976 3e0a 3c2f 6469 763e  br></div>.</div>
+000042b0: 0a3c 2f73 6563 7469 6f6e 3e0a 3c73 6563  .</section>.<sec
+000042c0: 7469 6f6e 2069 643d 2263 6974 652d 7573  tion id="cite-us
+000042d0: 2220 636c 6173 733d 2222 3e0a 3c68 323e  " class="">.<h2>
+000042e0: 4369 7465 2075 733c 6120 636c 6173 733d  Cite us<a class=
+000042f0: 2268 6561 6465 726c 696e 6b22 2068 7265  "headerlink" hre
+00004300: 663d 2223 6369 7465 2d75 7322 2074 6974  f="#cite-us" tit
+00004310: 6c65 3d22 5065 726d 616c 696e 6b20 746f  le="Permalink to
+00004320: 2074 6869 7320 6865 6164 696e 6722 3e23   this heading">#
+00004330: 3c2f 613e 3c2f 6832 3e0a 3c70 3e4b 7561  </a></h2>.<p>Kua
+00004340: 2d48 616f 2043 6861 6f2c 204a 616b 6f62  -Hao Chao, Jakob
+00004350: 204d 2e20 4865 696e 7a2c 2043 656c 696e   M. Heinz, Celin
+00004360: 6520 486f 682c 2041 6c61 6e20 4d61 6f2c  e Hoh, Alan Mao,
+00004370: 2041 6c61 696e 6120 5368 756d 6174 652c   Alaina Shumate,
+00004380: 204d 6968 6165 6c61 2050 6572 7465 612c   Mihaela Pertea,
+00004390: 2061 6e64 2053 7465 7665 6e20 4c2e 2053   and Steven L. S
+000043a0: 616c 7a62 6572 672e 203c 693e 2243 6f6d  alzberg. <i>"Com
+000043b0: 6269 6e69 6e67 2044 4e41 2061 6e64 2070  bining DNA and p
+000043c0: 726f 7465 696e 2061 6c69 676e 6d65 6e74  rotein alignment
+000043d0: 7320 746f 2069 6d70 726f 7665 2067 656e  s to improve gen
+000043e0: 6f6d 6520 616e 6e6f 7461 7469 6f6e 2077  ome annotation w
+000043f0: 6974 6820 4c69 6674 4f6e 2e22 3c2f 693e  ith LiftOn."</i>
+00004400: 203c 623e 6269 6f52 7869 7620 636f 6d69   <b>bioRxiv comi
+00004410: 6e67 2073 6f6f 6e3c 2f62 3e2e 0a3c 6120  ng soon</b>..<a 
+00004420: 6872 6566 3d22 6874 7470 733a 2f2f 646f  href="https://do
+00004430: 692e 6f72 672f 3130 2e31 3039 332f 6269  i.org/10.1093/bi
+00004440: 6f69 6e66 6f72 6d61 7469 6373 2f62 7461  oinformatics/bta
+00004450: 6131 3031 3622 2074 6172 6765 743d 225f  a1016" target="_
+00004460: 626c 616e 6b22 3e20 3c73 7667 2078 6d6c  blank"> <svg xml
+00004470: 6e73 3d22 6874 7470 3a2f 2f77 7777 2e77  ns="http://www.w
+00004480: 332e 6f72 672f 3230 3030 2f73 7667 2220  3.org/2000/svg" 
+00004490: 6172 6961 2d68 6964 6465 6e3d 2274 7275  aria-hidden="tru
+000044a0: 6522 2078 3d22 3070 7822 2079 3d22 3070  e" x="0px" y="0p
+000044b0: 7822 2076 6965 7742 6f78 3d22 3020 3020  x" viewBox="0 0 
+000044c0: 3130 3020 3130 3022 2077 6964 7468 3d22  100 100" width="
+000044d0: 3135 2220 6865 6967 6874 3d22 3135 2220  15" height="15" 
+000044e0: 636c 6173 733d 2269 636f 6e20 6f75 7462  class="icon outb
+000044f0: 6f75 6e64 223e 3c70 6174 6820 6669 6c6c  ound"><path fill
+00004500: 3d22 6375 7272 656e 7443 6f6c 6f72 2220  ="currentColor" 
+00004510: 643d 224d 3138 2e38 2c38 352e 3168 3536  d="M18.8,85.1h56
+00004520: 6c30 2c30 6332 2e32 2c30 2c34 2d31 2e38  l0,0c2.2,0,4-1.8
+00004530: 2c34 2d34 762d 3332 682d 3876 3238 682d  ,4-4v-32h-8v28h-
+00004540: 3438 762d 3438 6832 3876 2d38 682d 3332  48v-48h28v-8h-32
+00004550: 6c30 2c30 632d 322e 322c 302d 342c 312e  l0,0c-2.2,0-4,1.
+00004560: 382d 342c 3476 3536 4331 342e 382c 3833  8-4,4v56C14.8,83
+00004570: 2e33 2c31 362e 362c 3835 2e31 2c31 382e  .3,16.6,85.1,18.
+00004580: 382c 3835 2e31 7a22 3e3c 2f70 6174 683e  8,85.1z"></path>
+00004590: 203c 706f 6c79 676f 6e20 6669 6c6c 3d22   <polygon fill="
+000045a0: 6375 7272 656e 7443 6f6c 6f72 2220 706f  currentColor" po
+000045b0: 696e 7473 3d22 3435 2e37 2c34 382e 3720  ints="45.7,48.7 
+000045c0: 3531 2e33 2c35 342e 3320 3737 2e32 2c32  51.3,54.3 77.2,2
+000045d0: 382e 3520 3737 2e32 2c33 372e 3220 3835  8.5 77.2,37.2 85
+000045e0: 2e32 2c33 372e 3220 3835 2e32 2c31 342e  .2,37.2 85.2,14.
+000045f0: 3920 3632 2e38 2c31 342e 3920 3632 2e38  9 62.8,14.9 62.8
+00004600: 2c32 322e 3920 3731 2e35 2c32 322e 3922  ,22.9 71.5,22.9"
+00004610: 3e3c 2f70 6f6c 7967 6f6e 3e3c 2f73 7667  ></polygon></svg
+00004620: 3e20 3c2f 613e 203c 2f70 3e0a 0a3c 703e  > </a> </p>..<p>
+00004630: 416c 6169 6e61 2053 6875 6d61 7465 2c20  Alaina Shumate, 
+00004640: 616e 6420 5374 6576 656e 204c 2e20 5361  and Steven L. Sa
+00004650: 6c7a 6265 7267 2e20 3c69 3e22 4c69 6674  lzberg. <i>"Lift
+00004660: 6f66 663a 2061 6363 7572 6174 6520 6d61  off: accurate ma
+00004670: 7070 696e 6720 6f66 2067 656e 6520 616e  pping of gene an
+00004680: 6e6f 7461 7469 6f6e 732e 223c 2f69 3e20  notations."</i> 
+00004690: 3c62 3e42 696f 696e 666f 726d 6174 6963  <b>Bioinformatic
+000046a0: 733c 2f62 3e20 3337 2e31 3220 2832 3032  s</b> 37.12 (202
+000046b0: 3129 3a20 3136 3339 2d31 3634 332e 0a0a  1): 1639-1643...
+000046c0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000046d0: 2f64 6f69 2e6f 7267 2f31 302e 3130 3933  /doi.org/10.1093
+000046e0: 2f62 696f 696e 666f 726d 6174 6963 732f  /bioinformatics/
+000046f0: 6274 6161 3130 3136 2220 7461 7267 6574  btaa1016" target
+00004700: 3d22 5f62 6c61 6e6b 223e 203c 7376 6720  ="_blank"> <svg 
+00004710: 786d 6c6e 733d 2268 7474 703a 2f2f 7777  xmlns="http://ww
+00004720: 772e 7733 2e6f 7267 2f32 3030 302f 7376  w.w3.org/2000/sv
+00004730: 6722 2061 7269 612d 6869 6464 656e 3d22  g" aria-hidden="
+00004740: 7472 7565 2220 783d 2230 7078 2220 793d  true" x="0px" y=
+00004750: 2230 7078 2220 7669 6577 426f 783d 2230  "0px" viewBox="0
+00004760: 2030 2031 3030 2031 3030 2220 7769 6474   0 100 100" widt
+00004770: 683d 2231 3522 2068 6569 6768 743d 2231  h="15" height="1
+00004780: 3522 2063 6c61 7373 3d22 6963 6f6e 206f  5" class="icon o
+00004790: 7574 626f 756e 6422 3e3c 7061 7468 2066  utbound"><path f
+000047a0: 696c 6c3d 2263 7572 7265 6e74 436f 6c6f  ill="currentColo
+000047b0: 7222 2064 3d22 4d31 382e 382c 3835 2e31  r" d="M18.8,85.1
+000047c0: 6835 366c 302c 3063 322e 322c 302c 342d  h56l0,0c2.2,0,4-
+000047d0: 312e 382c 342d 3476 2d33 3268 2d38 7632  1.8,4-4v-32h-8v2
+000047e0: 3868 2d34 3876 2d34 3868 3238 762d 3868  8h-48v-48h28v-8h
+000047f0: 2d33 326c 302c 3063 2d32 2e32 2c30 2d34  -32l0,0c-2.2,0-4
+00004800: 2c31 2e38 2d34 2c34 7635 3643 3134 2e38  ,1.8-4,4v56C14.8
+00004810: 2c38 332e 332c 3136 2e36 2c38 352e 312c  ,83.3,16.6,85.1,
+00004820: 3138 2e38 2c38 352e 317a 223e 3c2f 7061  18.8,85.1z"></pa
+00004830: 7468 3e20 3c70 6f6c 7967 6f6e 2066 696c  th> <polygon fil
+00004840: 6c3d 2263 7572 7265 6e74 436f 6c6f 7222  l="currentColor"
+00004850: 2070 6f69 6e74 733d 2234 352e 372c 3438   points="45.7,48
+00004860: 2e37 2035 312e 332c 3534 2e33 2037 372e  .7 51.3,54.3 77.
+00004870: 322c 3238 2e35 2037 372e 322c 3337 2e32  2,28.5 77.2,37.2
+00004880: 2038 352e 322c 3337 2e32 2038 352e 322c   85.2,37.2 85.2,
+00004890: 3134 2e39 2036 322e 382c 3134 2e39 2036  14.9 62.8,14.9 6
+000048a0: 322e 382c 3232 2e39 2037 312e 352c 3232  2.8,22.9 71.5,22
+000048b0: 2e39 223e 3c2f 706f 6c79 676f 6e3e 3c2f  .9"></polygon></
+000048c0: 7376 673e 0a3c 2f61 3e0a 3c2f 703e 3c64  svg>.</a>.</p><d
+000048d0: 6976 2063 6c61 7373 3d22 6c69 6e65 2d62  iv class="line-b
+000048e0: 6c6f 636b 223e 0a3c 6469 7620 636c 6173  lock">.<div clas
+000048f0: 733d 226c 696e 6522 3e3c 6272 3e3c 2f64  s="line"><br></d
+00004900: 6976 3e0a 3c2f 6469 763e 0a3c 2f73 6563  iv>.</div>.</sec
+00004910: 7469 6f6e 3e0a 3c73 6563 7469 6f6e 2069  tion>.<section i
+00004920: 643d 2275 7365 722d 7375 7070 6f72 7422  d="user-support"
+00004930: 2063 6c61 7373 3d22 223e 0a3c 6832 3e55   class="">.<h2>U
+00004940: 7365 7220 7375 7070 6f72 743c 6120 636c  ser support<a cl
+00004950: 6173 733d 2268 6561 6465 726c 696e 6b22  ass="headerlink"
+00004960: 2068 7265 663d 2223 7573 6572 2d73 7570   href="#user-sup
+00004970: 706f 7274 2220 7469 746c 653d 2250 6572  port" title="Per
+00004980: 6d61 6c69 6e6b 2074 6f20 7468 6973 2068  malink to this h
+00004990: 6561 6469 6e67 223e 233c 2f61 3e3c 2f68  eading">#</a></h
+000049a0: 323e 0a3c 703e 506c 6561 7365 2067 6f20  2>.<p>Please go 
+000049b0: 7468 726f 7567 6820 7468 6520 3c61 2063  through the <a c
+000049c0: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
+000049d0: 696e 7465 726e 616c 2220 6872 6566 3d22  internal" href="
+000049e0: 2374 6162 6c65 2d6f 662d 636f 6e74 656e  #table-of-conten
+000049f0: 7473 223e 3c73 7061 6e20 636c 6173 733d  ts"><span class=
+00004a00: 2273 7464 2073 7464 2d72 6566 223e 646f  "std std-ref">do
+00004a10: 6375 6d65 6e74 6174 696f 6e3c 2f73 7061  cumentation</spa
+00004a20: 6e3e 3c2f 613e 2062 656c 6f77 2066 6972  n></a> below fir
+00004a30: 7374 2e20 4966 2079 6f75 2068 6176 6520  st. If you have 
+00004a40: 7175 6573 7469 6f6e 7320 6162 6f75 7420  questions about 
+00004a50: 7573 696e 6720 7468 6520 7061 636b 6167  using the packag
+00004a60: 652c 2061 2062 7567 2072 6570 6f72 742c  e, a bug report,
+00004a70: 206f 7220 6120 6665 6174 7572 6520 7265   or a feature re
+00004a80: 7175 6573 742c 2070 6c65 6173 6520 7573  quest, please us
+00004a90: 6520 7468 6520 4769 7448 7562 2069 7373  e the GitHub iss
+00004aa0: 7565 2074 7261 636b 6572 2068 6572 653a  ue tracker here:
+00004ab0: 3c2f 703e 0a3c 703e 3c61 2063 6c61 7373  </p>.<p><a class
+00004ac0: 3d22 7265 6665 7265 6e63 6520 6578 7465  ="reference exte
+00004ad0: 726e 616c 2220 6872 6566 3d22 6874 7470  rnal" href="http
+00004ae0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4b  s://github.com/K
+00004af0: 7561 6e68 616f 2d43 6861 6f2f 4c69 6674  uanhao-Chao/Lift
+00004b00: 4f6e 2f69 7373 7565 7322 3e68 7474 7073  On/issues">https
+00004b10: 3a2f 2f67 6974 6875 622e 636f 6d2f 4b75  ://github.com/Ku
+00004b20: 616e 6861 6f2d 4368 616f 2f4c 6966 744f  anhao-Chao/LiftO
+00004b30: 6e2f 6973 7375 6573 3c2f 613e 3c2f 703e  n/issues</a></p>
+00004b40: 0a3c 6469 7620 636c 6173 733d 226c 696e  .<div class="lin
+00004b50: 652d 626c 6f63 6b22 3e0a 3c64 6976 2063  e-block">.<div c
+00004b60: 6c61 7373 3d22 6c69 6e65 223e 3c62 723e  lass="line"><br>
+00004b70: 3c2f 6469 763e 0a3c 2f64 6976 3e0a 3c2f  </div>.</div>.</
+00004b80: 7365 6374 696f 6e3e 0a3c 7365 6374 696f  section>.<sectio
+00004b90: 6e20 6964 3d22 6b65 792d 636f 6e74 7269  n id="key-contri
+00004ba0: 6275 746f 7273 2220 636c 6173 733d 2222  butors" class=""
+00004bb0: 3e0a 3c68 323e 4b65 7920 636f 6e74 7269  >.<h2>Key contri
+00004bc0: 6275 746f 7273 3c61 2063 6c61 7373 3d22  butors<a class="
+00004bd0: 6865 6164 6572 6c69 6e6b 2220 6872 6566  headerlink" href
+00004be0: 3d22 236b 6579 2d63 6f6e 7472 6962 7574  ="#key-contribut
+00004bf0: 6f72 7322 2074 6974 6c65 3d22 5065 726d  ors" title="Perm
+00004c00: 616c 696e 6b20 746f 2074 6869 7320 6865  alink to this he
+00004c10: 6164 696e 6722 3e23 3c2f 613e 3c2f 6832  ading">#</a></h2
+00004c20: 3e0a 3c70 3e4c 6966 744f 6e20 7761 7320  >.<p>LiftOn was 
+00004c30: 6465 7369 676e 6564 2061 6e64 2064 6576  designed and dev
+00004c40: 656c 6f70 6564 2062 7920 3c61 2063 6c61  eloped by <a cla
+00004c50: 7373 3d22 7265 6665 7265 6e63 6520 6578  ss="reference ex
+00004c60: 7465 726e 616c 2220 6872 6566 3d22 6874  ternal" href="ht
+00004c70: 7470 733a 2f2f 6b68 6368 616f 2e63 6f6d  tps://khchao.com
+00004c80: 2f22 3e4b 7561 6e2d 4861 6f20 4368 616f  /">Kuan-Hao Chao
+00004c90: 3c2f 613e 2e20 2054 6869 7320 646f 6375  </a>.  This docu
+00004ca0: 6d65 6e74 6174 696f 6e20 7761 7320 7772  mentation was wr
+00004cb0: 6974 7465 6e20 6279 203c 6120 636c 6173  itten by <a clas
+00004cc0: 733d 2272 6566 6572 656e 6365 2065 7874  s="reference ext
+00004cd0: 6572 6e61 6c22 2068 7265 663d 2268 7474  ernal" href="htt
+00004ce0: 7073 3a2f 2f6b 6863 6861 6f2e 636f 6d2f  ps://khchao.com/
+00004cf0: 223e 4b75 616e 2d48 616f 2043 6861 6f3c  ">Kuan-Hao Chao<
+00004d00: 2f61 3e20 616e 6420 3c61 2063 6c61 7373  /a> and <a class
+00004d10: 3d22 7265 6665 7265 6e63 6520 6578 7465  ="reference exte
+00004d20: 726e 616c 2220 6872 6566 3d22 6874 7470  rnal" href="http
+00004d30: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+00004d40: 6d31 3222 3e41 6c61 6e20 4d61 6e3c 2f61  m12">Alan Man</a
+00004d50: 3e2e 2054 6865 204c 6966 744f 6e20 6c6f  >. The LiftOn lo
+00004d60: 676f 2077 6173 2064 6573 6967 6e65 6420  go was designed 
+00004d70: 6279 203c 6120 636c 6173 733d 2272 6566  by <a class="ref
+00004d80: 6572 656e 6365 2065 7874 6572 6e61 6c22  erence external"
+00004d90: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00004da0: 6974 6875 622e 636f 6d2f 616d 3132 223e  ithub.com/am12">
+00004db0: 416c 616e 204d 616e 3c2f 613e 2e3c 2f70  Alan Man</a>.</p
+00004dc0: 3e0a 3c64 6976 2063 6c61 7373 3d22 6c69  >.<div class="li
+00004dd0: 6e65 2d62 6c6f 636b 223e 0a3c 6469 7620  ne-block">.<div 
+00004de0: 636c 6173 733d 226c 696e 6522 3e3c 6272  class="line"><br
+00004df0: 3e3c 2f64 6976 3e0a 3c2f 6469 763e 0a3c  ></div>.</div>.<
+00004e00: 2f73 6563 7469 6f6e 3e0a 3c73 6563 7469  /section>.<secti
+00004e10: 6f6e 2069 643d 2274 6162 6c65 2d6f 662d  on id="table-of-
+00004e20: 636f 6e74 656e 7473 2220 636c 6173 733d  contents" class=
+00004e30: 2222 3e0a 3c73 7061 6e20 6964 3d22 6964  "">.<span id="id
+00004e40: 3322 3e3c 2f73 7061 6e3e 3c68 323e 5461  3"></span><h2>Ta
+00004e50: 626c 6520 6f66 2063 6f6e 7465 6e74 733c  ble of contents<
+00004e60: 6120 636c 6173 733d 2268 6561 6465 726c  a class="headerl
+00004e70: 696e 6b22 2068 7265 663d 2223 7461 626c  ink" href="#tabl
+00004e80: 652d 6f66 2d63 6f6e 7465 6e74 7322 2074  e-of-contents" t
+00004e90: 6974 6c65 3d22 5065 726d 616c 696e 6b20  itle="Permalink 
+00004ea0: 746f 2074 6869 7320 6865 6164 696e 6722  to this heading"
+00004eb0: 3e23 3c2f 613e 3c2f 6832 3e0a 3c64 6976  >#</a></h2>.<div
+00004ec0: 2063 6c61 7373 3d22 746f 6374 7265 652d   class="toctree-
+00004ed0: 7772 6170 7065 7220 636f 6d70 6f75 6e64  wrapper compound
+00004ee0: 223e 0a3c 756c 3e0a 3c6c 6920 636c 6173  ">.<ul>.<li clas
+00004ef0: 733d 2274 6f63 7472 6565 2d6c 3122 3e3c  s="toctree-l1"><
+00004f00: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
+00004f10: 6365 2069 6e74 6572 6e61 6c22 2068 7265  ce internal" hre
+00004f20: 663d 2268 7474 7073 3a2f 2f63 6362 2e6a  f="https://ccb.j
+00004f30: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
+00004f40: 6e74 656e 742f 696e 7374 616c 6c61 7469  ntent/installati
+00004f50: 6f6e 2e68 746d 6c22 3e49 6e73 7461 6c6c  on.html">Install
+00004f60: 6174 696f 6e3c 2f61 3e3c 756c 3e0a 3c6c  ation</a><ul>.<l
+00004f70: 6920 636c 6173 733d 2274 6f63 7472 6565  i class="toctree
+00004f80: 2d6c 3222 3e3c 6120 636c 6173 733d 2272  -l2"><a class="r
+00004f90: 6566 6572 656e 6365 2069 6e74 6572 6e61  eference interna
+00004fa0: 6c22 2068 7265 663d 2268 7474 7073 3a2f  l" href="https:/
+00004fb0: 2f63 6362 2e6a 6875 2e65 6475 2f6c 6966  /ccb.jhu.edu/lif
+00004fc0: 746f 6e2f 636f 6e74 656e 742f 696e 7374  ton/content/inst
+00004fd0: 616c 6c61 7469 6f6e 2e68 746d 6c23 7379  allation.html#sy
+00004fe0: 7374 656d 2d72 6571 7569 7265 6d65 6e74  stem-requirement
+00004ff0: 7322 3e53 7973 7465 6d20 7265 7175 6972  s">System requir
+00005000: 656d 656e 7473 3c2f 613e 3c2f 6c69 3e0a  ements</a></li>.
+00005010: 3c6c 6920 636c 6173 733d 2274 6f63 7472  <li class="toctr
+00005020: 6565 2d6c 3222 3e3c 6120 636c 6173 733d  ee-l2"><a class=
+00005030: 2272 6566 6572 656e 6365 2069 6e74 6572  "reference inter
+00005040: 6e61 6c22 2068 7265 663d 2268 7474 7073  nal" href="https
+00005050: 3a2f 2f63 6362 2e6a 6875 2e65 6475 2f6c  ://ccb.jhu.edu/l
+00005060: 6966 746f 6e2f 636f 6e74 656e 742f 696e  ifton/content/in
+00005070: 7374 616c 6c61 7469 6f6e 2e68 746d 6c23  stallation.html#
+00005080: 696e 7374 616c 6c2d 7468 726f 7567 682d  install-through-
+00005090: 7069 7022 3e49 6e73 7461 6c6c 2074 6872  pip">Install thr
+000050a0: 6f75 6768 2070 6970 3c2f 613e 3c2f 6c69  ough pip</a></li
+000050b0: 3e0a 3c6c 6920 636c 6173 733d 2274 6f63  >.<li class="toc
+000050c0: 7472 6565 2d6c 3222 3e3c 6120 636c 6173  tree-l2"><a clas
+000050d0: 733d 2272 6566 6572 656e 6365 2069 6e74  s="reference int
+000050e0: 6572 6e61 6c22 2068 7265 663d 2268 7474  ernal" href="htt
+000050f0: 7073 3a2f 2f63 6362 2e6a 6875 2e65 6475  ps://ccb.jhu.edu
+00005100: 2f6c 6966 746f 6e2f 636f 6e74 656e 742f  /lifton/content/
+00005110: 696e 7374 616c 6c61 7469 6f6e 2e68 746d  installation.htm
+00005120: 6c23 696e 7374 616c 6c2d 7468 726f 7567  l#install-throug
+00005130: 682d 636f 6e64 6122 3e49 6e73 7461 6c6c  h-conda">Install
+00005140: 2074 6872 6f75 6768 2063 6f6e 6461 3c2f   through conda</
+00005150: 613e 3c2f 6c69 3e0a 3c6c 6920 636c 6173  a></li>.<li clas
+00005160: 733d 2274 6f63 7472 6565 2d6c 3222 3e3c  s="toctree-l2"><
+00005170: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
+00005180: 6365 2069 6e74 6572 6e61 6c22 2068 7265  ce internal" hre
+00005190: 663d 2268 7474 7073 3a2f 2f63 6362 2e6a  f="https://ccb.j
+000051a0: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
+000051b0: 6e74 656e 742f 696e 7374 616c 6c61 7469  ntent/installati
+000051c0: 6f6e 2e68 746d 6c23 696e 7374 616c 6c2d  on.html#install-
+000051d0: 6672 6f6d 2d73 6f75 7263 6522 3e49 6e73  from-source">Ins
+000051e0: 7461 6c6c 2066 726f 6d20 736f 7572 6365  tall from source
+000051f0: 3c2f 613e 3c2f 6c69 3e0a 3c6c 6920 636c  </a></li>.<li cl
+00005200: 6173 733d 2274 6f63 7472 6565 2d6c 3222  ass="toctree-l2"
+00005210: 3e3c 6120 636c 6173 733d 2272 6566 6572  ><a class="refer
+00005220: 656e 6365 2069 6e74 6572 6e61 6c22 2068  ence internal" h
+00005230: 7265 663d 2268 7474 7073 3a2f 2f63 6362  ref="https://ccb
+00005240: 2e6a 6875 2e65 6475 2f6c 6966 746f 6e2f  .jhu.edu/lifton/
+00005250: 636f 6e74 656e 742f 696e 7374 616c 6c61  content/installa
+00005260: 7469 6f6e 2e68 746d 6c23 6368 6563 6b2d  tion.html#check-
+00005270: 6c69 6674 6f6e 2d69 6e73 7461 6c6c 6174  lifton-installat
+00005280: 696f 6e22 3e43 6865 636b 204c 6966 744f  ion">Check LiftO
+00005290: 6e20 696e 7374 616c 6c61 7469 6f6e 3c2f  n installation</
+000052a0: 613e 3c2f 6c69 3e0a 3c6c 6920 636c 6173  a></li>.<li clas
+000052b0: 733d 2274 6f63 7472 6565 2d6c 3222 3e3c  s="toctree-l2"><
+000052c0: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
+000052d0: 6365 2069 6e74 6572 6e61 6c22 2068 7265  ce internal" hre
+000052e0: 663d 2268 7474 7073 3a2f 2f63 6362 2e6a  f="https://ccb.j
+000052f0: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
+00005300: 6e74 656e 742f 696e 7374 616c 6c61 7469  ntent/installati
+00005310: 6f6e 2e68 746d 6c23 6e6f 772d 796f 752d  on.html#now-you-
+00005320: 6172 652d 7265 6164 792d 746f 2d67 6f22  are-ready-to-go"
+00005330: 3e4e 6f77 2c20 796f 7520 6172 6520 7265  >Now, you are re
+00005340: 6164 7920 746f 2067 6f20 213c 2f61 3e3c  ady to go !</a><
+00005350: 2f6c 693e 0a3c 2f75 6c3e 0a3c 2f6c 693e  /li>.</ul>.</li>
+00005360: 0a3c 6c69 2063 6c61 7373 3d22 746f 6374  .<li class="toct
+00005370: 7265 652d 6c31 223e 3c61 2063 6c61 7373  ree-l1"><a class
+00005380: 3d22 7265 6665 7265 6e63 6520 696e 7465  ="reference inte
+00005390: 726e 616c 2220 6872 6566 3d22 6874 7470  rnal" href="http
+000053a0: 733a 2f2f 6363 622e 6a68 752e 6564 752f  s://ccb.jhu.edu/
+000053b0: 6c69 6674 6f6e 2f63 6f6e 7465 6e74 2f71  lifton/content/q
+000053c0: 7569 636b 7374 6172 742e 6874 6d6c 223e  uickstart.html">
+000053d0: 5175 6963 6b20 5374 6172 7420 4775 6964  Quick Start Guid
+000053e0: 653c 2f61 3e3c 756c 3e0a 3c6c 6920 636c  e</a><ul>.<li cl
+000053f0: 6173 733d 2274 6f63 7472 6565 2d6c 3222  ass="toctree-l2"
+00005400: 3e3c 6120 636c 6173 733d 2272 6566 6572  ><a class="refer
+00005410: 656e 6365 2069 6e74 6572 6e61 6c22 2068  ence internal" h
+00005420: 7265 663d 2268 7474 7073 3a2f 2f63 6362  ref="https://ccb
+00005430: 2e6a 6875 2e65 6475 2f6c 6966 746f 6e2f  .jhu.edu/lifton/
+00005440: 636f 6e74 656e 742f 7175 6963 6b73 7461  content/quicksta
+00005450: 7274 2e68 746d 6c23 7375 7065 722d 7175  rt.html#super-qu
+00005460: 6963 6b2d 7374 6172 742d 6f6e 652d 6c69  ick-start-one-li
+00005470: 6e65 7222 3e53 7570 6572 2d51 7569 636b  ner">Super-Quick
+00005480: 2053 7461 7274 2028 6f6e 652d 6c69 6e65   Start (one-line
+00005490: 7229 3c2f 613e 3c2f 6c69 3e0a 3c6c 6920  r)</a></li>.<li 
+000054a0: 636c 6173 733d 2274 6f63 7472 6565 2d6c  class="toctree-l
+000054b0: 3222 3e3c 6120 636c 6173 733d 2272 6566  2"><a class="ref
+000054c0: 6572 656e 6365 2069 6e74 6572 6e61 6c22  erence internal"
+000054d0: 2068 7265 663d 2268 7474 7073 3a2f 2f63   href="https://c
+000054e0: 6362 2e6a 6875 2e65 6475 2f6c 6966 746f  cb.jhu.edu/lifto
+000054f0: 6e2f 636f 6e74 656e 742f 7175 6963 6b73  n/content/quicks
+00005500: 7461 7274 2e68 746d 6c23 696e 7465 7270  tart.html#interp
+00005510: 7265 7469 6e67 2d6f 7574 7075 7473 2d6f  reting-outputs-o
+00005520: 6e2d 7468 652d 7465 726d 696e 616c 223e  n-the-terminal">
+00005530: 496e 7465 7270 7265 7469 6e67 206f 7574  Interpreting out
+00005540: 7075 7473 206f 6e20 7468 6520 7465 726d  puts on the term
+00005550: 696e 616c 3c2f 613e 3c2f 6c69 3e0a 3c6c  inal</a></li>.<l
+00005560: 6920 636c 6173 733d 2274 6f63 7472 6565  i class="toctree
+00005570: 2d6c 3222 3e3c 6120 636c 6173 733d 2272  -l2"><a class="r
+00005580: 6566 6572 656e 6365 2069 6e74 6572 6e61  eference interna
+00005590: 6c22 2068 7265 663d 2268 7474 7073 3a2f  l" href="https:/
+000055a0: 2f63 6362 2e6a 6875 2e65 6475 2f6c 6966  /ccb.jhu.edu/lif
+000055b0: 746f 6e2f 636f 6e74 656e 742f 7175 6963  ton/content/quic
+000055c0: 6b73 7461 7274 2e68 746d 6c23 7472 792d  kstart.html#try-
+000055d0: 6c69 6674 6f6e 2d6f 6e2d 676f 6f67 6c65  lifton-on-google
+000055e0: 2d63 6f6c 6162 223e 5472 7920 4c69 6674  -colab">Try Lift
+000055f0: 4f6e 206f 6e20 476f 6f67 6c65 2043 6f6c  On on Google Col
+00005600: 6162 3c2f 613e 3c2f 6c69 3e0a 3c2f 756c  ab</a></li>.</ul
+00005610: 3e0a 3c2f 6c69 3e0a 3c2f 756c 3e0a 3c2f  >.</li>.</ul>.</
+00005620: 6469 763e 0a3c 6469 7620 636c 6173 733d  div>.<div class=
+00005630: 2274 6f63 7472 6565 2d77 7261 7070 6572  "toctree-wrapper
+00005640: 2063 6f6d 706f 756e 6422 3e0a 3c70 2063   compound">.<p c
+00005650: 6c61 7373 3d22 6361 7074 696f 6e22 2072  lass="caption" r
+00005660: 6f6c 653d 2268 6561 6469 6e67 223e 3c73  ole="heading"><s
+00005670: 7061 6e20 636c 6173 733d 2263 6170 7469  pan class="capti
+00005680: 6f6e 2d74 6578 7422 3e45 7861 6d70 6c65  on-text">Example
+00005690: 733c 2f73 7061 6e3e 3c2f 703e 0a3c 756c  s</span></p>.<ul
+000056a0: 3e0a 3c6c 6920 636c 6173 733d 2274 6f63  >.<li class="toc
+000056b0: 7472 6565 2d6c 3122 3e3c 6120 636c 6173  tree-l1"><a clas
+000056c0: 733d 2272 6566 6572 656e 6365 2069 6e74  s="reference int
+000056d0: 6572 6e61 6c22 2068 7265 663d 2268 7474  ernal" href="htt
+000056e0: 7073 3a2f 2f63 6362 2e6a 6875 2e65 6475  ps://ccb.jhu.edu
+000056f0: 2f6c 6966 746f 6e2f 636f 6e74 656e 742f  /lifton/content/
+00005700: 7361 6d65 5f73 7065 6369 6573 5f6c 6966  same_species_lif
+00005710: 746f 7665 722f 696e 6465 782e 6874 6d6c  tover/index.html
+00005720: 223e 5361 6d65 2073 7065 6369 6573 206c  ">Same species l
+00005730: 6966 742d 6f76 6572 3c2f 613e 3c2f 6c69  ift-over</a></li
+00005740: 3e0a 3c6c 6920 636c 6173 733d 2274 6f63  >.<li class="toc
+00005750: 7472 6565 2d6c 3122 3e3c 6120 636c 6173  tree-l1"><a clas
+00005760: 733d 2272 6566 6572 656e 6365 2069 6e74  s="reference int
+00005770: 6572 6e61 6c22 2068 7265 663d 2268 7474  ernal" href="htt
+00005780: 7073 3a2f 2f63 6362 2e6a 6875 2e65 6475  ps://ccb.jhu.edu
+00005790: 2f6c 6966 746f 6e2f 636f 6e74 656e 742f  /lifton/content/
+000057a0: 636c 6f73 655f 7370 6563 6965 735f 6c69  close_species_li
+000057b0: 6674 6f76 6572 2f69 6e64 6578 2e68 746d  ftover/index.htm
+000057c0: 6c22 3e43 6c6f 7365 6c79 2072 656c 6174  l">Closely relat
+000057d0: 6564 2073 7065 6369 6573 206c 6966 742d  ed species lift-
+000057e0: 6f76 6572 3c2f 613e 3c2f 6c69 3e0a 3c6c  over</a></li>.<l
+000057f0: 6920 636c 6173 733d 2274 6f63 7472 6565  i class="toctree
+00005800: 2d6c 3122 3e3c 6120 636c 6173 733d 2272  -l1"><a class="r
+00005810: 6566 6572 656e 6365 2069 6e74 6572 6e61  eference interna
+00005820: 6c22 2068 7265 663d 2268 7474 7073 3a2f  l" href="https:/
+00005830: 2f63 6362 2e6a 6875 2e65 6475 2f6c 6966  /ccb.jhu.edu/lif
+00005840: 746f 6e2f 636f 6e74 656e 742f 6469 7374  ton/content/dist
+00005850: 616e 745f 7370 6563 6965 735f 6c69 6674  ant_species_lift
+00005860: 6f76 6572 2f69 6e64 6578 2e68 746d 6c22  over/index.html"
+00005870: 3e44 6973 7461 6e74 6c79 2072 656c 6174  >Distantly relat
+00005880: 6564 2073 7065 6369 6573 206c 6966 742d  ed species lift-
+00005890: 6f76 6572 3c2f 613e 3c2f 6c69 3e0a 3c2f  over</a></li>.</
+000058a0: 756c 3e0a 3c2f 6469 763e 0a3c 6469 7620  ul>.</div>.<div 
+000058b0: 636c 6173 733d 2274 6f63 7472 6565 2d77  class="toctree-w
+000058c0: 7261 7070 6572 2063 6f6d 706f 756e 6422  rapper compound"
+000058d0: 3e0a 3c70 2063 6c61 7373 3d22 6361 7074  >.<p class="capt
+000058e0: 696f 6e22 2072 6f6c 653d 2268 6561 6469  ion" role="headi
+000058f0: 6e67 223e 3c73 7061 6e20 636c 6173 733d  ng"><span class=
+00005900: 2263 6170 7469 6f6e 2d74 6578 7422 3e49  "caption-text">I
+00005910: 6e66 6f3c 2f73 7061 6e3e 3c2f 703e 0a3c  nfo</span></p>.<
+00005920: 756c 3e0a 3c6c 6920 636c 6173 733d 2274  ul>.<li class="t
+00005930: 6f63 7472 6565 2d6c 3122 3e3c 6120 636c  octree-l1"><a cl
+00005940: 6173 733d 2272 6566 6572 656e 6365 2069  ass="reference i
+00005950: 6e74 6572 6e61 6c22 2068 7265 663d 2268  nternal" href="h
+00005960: 7474 7073 3a2f 2f63 6362 2e6a 6875 2e65  ttps://ccb.jhu.e
+00005970: 6475 2f6c 6966 746f 6e2f 636f 6e74 656e  du/lifton/conten
+00005980: 742f 6f75 7470 7574 5f65 7870 6c61 6e61  t/output_explana
+00005990: 7469 6f6e 2e68 746d 6c22 3e4f 7574 7075  tion.html">Outpu
+000059a0: 7420 6669 6c65 733c 2f61 3e3c 756c 3e0a  t files</a><ul>.
+000059b0: 3c6c 6920 636c 6173 733d 2274 6f63 7472  <li class="toctr
+000059c0: 6565 2d6c 3222 3e3c 6120 636c 6173 733d  ee-l2"><a class=
+000059d0: 2272 6566 6572 656e 6365 2069 6e74 6572  "reference inter
+000059e0: 6e61 6c22 2068 7265 663d 2268 7474 7073  nal" href="https
+000059f0: 3a2f 2f63 6362 2e6a 6875 2e65 6475 2f6c  ://ccb.jhu.edu/l
+00005a00: 6966 746f 6e2f 636f 6e74 656e 742f 6f75  ifton/content/ou
+00005a10: 7470 7574 5f65 7870 6c61 6e61 7469 6f6e  tput_explanation
+00005a20: 2e68 746d 6c23 6c69 6674 6f6e 2d67 6666  .html#lifton-gff
+00005a30: 3322 3e6c 6966 746f 6e2e 6766 6633 3c2f  3">lifton.gff3</
+00005a40: 613e 3c2f 6c69 3e0a 3c6c 6920 636c 6173  a></li>.<li clas
+00005a50: 733d 2274 6f63 7472 6565 2d6c 3222 3e3c  s="toctree-l2"><
+00005a60: 6120 636c 6173 733d 2272 6566 6572 656e  a class="referen
+00005a70: 6365 2069 6e74 6572 6e61 6c22 2068 7265  ce internal" hre
+00005a80: 663d 2268 7474 7073 3a2f 2f63 6362 2e6a  f="https://ccb.j
+00005a90: 6875 2e65 6475 2f6c 6966 746f 6e2f 636f  hu.edu/lifton/co
+00005aa0: 6e74 656e 742f 6f75 7470 7574 5f65 7870  ntent/output_exp
+00005ab0: 6c61 6e61 7469 6f6e 2e68 746d 6c23 6c69  lanation.html#li
+00005ac0: 6674 6f6e 2d6f 7574 7075 7422 3e6c 6966  fton-output">lif
+00005ad0: 746f 6e5f 6f75 7470 7574 2f3c 2f61 3e3c  ton_output/</a><
+00005ae0: 2f6c 693e 0a3c 2f75 6c3e 0a3c 2f6c 693e  /li>.</ul>.</li>
+00005af0: 0a3c 6c69 2063 6c61 7373 3d22 746f 6374  .<li class="toct
+00005b00: 7265 652d 6c31 223e 3c61 2063 6c61 7373  ree-l1"><a class
+00005b10: 3d22 7265 6665 7265 6e63 6520 696e 7465  ="reference inte
+00005b20: 726e 616c 2220 6872 6566 3d22 6874 7470  rnal" href="http
+00005b30: 733a 2f2f 6363 622e 6a68 752e 6564 752f  s://ccb.jhu.edu/
+00005b40: 6c69 6674 6f6e 2f63 6f6e 7465 6e74 2f66  lifton/content/f
+00005b50: 6561 7475 7265 5f63 6f75 6e74 696e 672e  eature_counting.
+00005b60: 6874 6d6c 223e 4765 6e65 202f 2054 7261  html">Gene / Tra
+00005b70: 6e73 6372 6970 7420 636f 756e 7469 6e67  nscript counting
+00005b80: 3c2f 613e 3c75 6c3e 0a3c 6c69 2063 6c61  </a><ul>.<li cla
+00005b90: 7373 3d22 746f 6374 7265 652d 6c32 223e  ss="toctree-l2">
+00005ba0: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
+00005bb0: 6e63 6520 696e 7465 726e 616c 2220 6872  nce internal" hr
+00005bc0: 6566 3d22 6874 7470 733a 2f2f 6363 622e  ef="https://ccb.
+00005bd0: 6a68 752e 6564 752f 6c69 6674 6f6e 2f63  jhu.edu/lifton/c
+00005be0: 6f6e 7465 6e74 2f66 6561 7475 7265 5f63  ontent/feature_c
+00005bf0: 6f75 6e74 696e 672e 6874 6d6c 2367 656e  ounting.html#gen
+00005c00: 652d 636f 756e 7469 6e67 223e 4765 6e65  e-counting">Gene
+00005c10: 2063 6f75 6e74 696e 673c 2f61 3e3c 2f6c   counting</a></l
+00005c20: 693e 0a3c 6c69 2063 6c61 7373 3d22 746f  i>.<li class="to
+00005c30: 6374 7265 652d 6c32 223e 3c61 2063 6c61  ctree-l2"><a cla
+00005c40: 7373 3d22 7265 6665 7265 6e63 6520 696e  ss="reference in
+00005c50: 7465 726e 616c 2220 6872 6566 3d22 6874  ternal" href="ht
+00005c60: 7470 733a 2f2f 6363 622e 6a68 752e 6564  tps://ccb.jhu.ed
+00005c70: 752f 6c69 6674 6f6e 2f63 6f6e 7465 6e74  u/lifton/content
+00005c80: 2f66 6561 7475 7265 5f63 6f75 6e74 696e  /feature_countin
+00005c90: 672e 6874 6d6c 2374 7261 6e73 6372 6970  g.html#transcrip
+00005ca0: 742d 636f 756e 7469 6e67 223e 5472 616e  t-counting">Tran
+00005cb0: 7363 7269 7074 2063 6f75 6e74 696e 673c  script counting<
+00005cc0: 2f61 3e3c 2f6c 693e 0a3c 2f75 6c3e 0a3c  /a></li>.</ul>.<
+00005cd0: 2f6c 693e 0a3c 6c69 2063 6c61 7373 3d22  /li>.<li class="
+00005ce0: 746f 6374 7265 652d 6c31 223e 3c61 2063  toctree-l1"><a c
+00005cf0: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
+00005d00: 696e 7465 726e 616c 2220 6872 6566 3d22  internal" href="
+00005d10: 6874 7470 733a 2f2f 6363 622e 6a68 752e  https://ccb.jhu.
+00005d20: 6564 752f 6c69 6674 6f6e 2f63 6f6e 7465  edu/lifton/conte
+00005d30: 6e74 2f65 7661 6c75 6174 696f 6e5f 6d65  nt/evaluation_me
+00005d40: 7472 6963 732e 6874 6d6c 223e 4576 616c  trics.html">Eval
+00005d50: 7561 7469 6f6e 206d 6574 7269 6373 202d  uation metrics -
+00005d60: 2073 6571 7565 6e63 6520 6964 656e 7469   sequence identi
+00005d70: 7479 3c2f 613e 3c75 6c3e 0a3c 6c69 2063  ty</a><ul>.<li c
+00005d80: 6c61 7373 3d22 746f 6374 7265 652d 6c32  lass="toctree-l2
+00005d90: 223e 3c61 2063 6c61 7373 3d22 7265 6665  "><a class="refe
+00005da0: 7265 6e63 6520 696e 7465 726e 616c 2220  rence internal" 
+00005db0: 6872 6566 3d22 6874 7470 733a 2f2f 6363  href="https://cc
+00005dc0: 622e 6a68 752e 6564 752f 6c69 6674 6f6e  b.jhu.edu/lifton
+00005dd0: 2f63 6f6e 7465 6e74 2f65 7661 6c75 6174  /content/evaluat
+00005de0: 696f 6e5f 6d65 7472 6963 732e 6874 6d6c  ion_metrics.html
+00005df0: 2364 6e61 2d73 6571 7565 6e63 652d 6964  #dna-sequence-id
+00005e00: 656e 7469 7479 2d73 636f 7265 223e 444e  entity-score">DN
+00005e10: 4120 7365 7175 656e 6365 2069 6465 6e74  A sequence ident
+00005e20: 6974 7920 7363 6f72 653c 2f61 3e3c 2f6c  ity score</a></l
+00005e30: 693e 0a3c 6c69 2063 6c61 7373 3d22 746f  i>.<li class="to
+00005e40: 6374 7265 652d 6c32 223e 3c61 2063 6c61  ctree-l2"><a cla
+00005e50: 7373 3d22 7265 6665 7265 6e63 6520 696e  ss="reference in
+00005e60: 7465 726e 616c 2220 6872 6566 3d22 6874  ternal" href="ht
+00005e70: 7470 733a 2f2f 6363 622e 6a68 752e 6564  tps://ccb.jhu.ed
+00005e80: 752f 6c69 6674 6f6e 2f63 6f6e 7465 6e74  u/lifton/content
+00005e90: 2f65 7661 6c75 6174 696f 6e5f 6d65 7472  /evaluation_metr
+00005ea0: 6963 732e 6874 6d6c 2370 726f 7465 696e  ics.html#protein
+00005eb0: 2d73 6571 7565 6e63 652d 6964 656e 7469  -sequence-identi
+00005ec0: 7479 2d73 636f 7265 223e 5072 6f74 6569  ty-score">Protei
+00005ed0: 6e20 7365 7175 656e 6365 2069 6465 6e74  n sequence ident
+00005ee0: 6974 7920 7363 6f72 653c 2f61 3e3c 2f6c  ity score</a></l
+00005ef0: 693e 0a3c 2f75 6c3e 0a3c 2f6c 693e 0a3c  i>.</ul>.</li>.<
+00005f00: 6c69 2063 6c61 7373 3d22 746f 6374 7265  li class="toctre
+00005f10: 652d 6c31 223e 3c61 2063 6c61 7373 3d22  e-l1"><a class="
+00005f20: 7265 6665 7265 6e63 6520 696e 7465 726e  reference intern
+00005f30: 616c 2220 6872 6566 3d22 6874 7470 733a  al" href="https:
+00005f40: 2f2f 6363 622e 6a68 752e 6564 752f 6c69  //ccb.jhu.edu/li
+00005f50: 6674 6f6e 2f63 6f6e 7465 6e74 2f62 6568  fton/content/beh
+00005f60: 696e 645f 7363 656e 6573 2e68 746d 6c22  ind_scenes.html"
+00005f70: 3e42 6568 696e 6420 7468 6520 7363 656e  >Behind the scen
+00005f80: 6573 3c2f 613e 3c75 6c3e 0a3c 6c69 2063  es</a><ul>.<li c
+00005f90: 6c61 7373 3d22 746f 6374 7265 652d 6c32  lass="toctree-l2
+00005fa0: 223e 3c61 2063 6c61 7373 3d22 7265 6665  "><a class="refe
+00005fb0: 7265 6e63 6520 696e 7465 726e 616c 2220  rence internal" 
+00005fc0: 6872 6566 3d22 6874 7470 733a 2f2f 6363  href="https://cc
+00005fd0: 622e 6a68 752e 6564 752f 6c69 6674 6f6e  b.jhu.edu/lifton
+00005fe0: 2f63 6f6e 7465 6e74 2f62 6568 696e 645f  /content/behind_
+00005ff0: 7363 656e 6573 2e68 746d 6c23 6465 6369  scenes.html#deci
+00006000: 6469 6e67 2d63 6872 6f6d 6f73 6f6d 6573  ding-chromosomes
+00006010: 2d61 6e64 2d66 6561 7475 7265 732d 666f  -and-features-fo
+00006020: 722d 616e 6e6f 7461 7469 6f6e 2d6c 6966  r-annotation-lif
+00006030: 742d 6f76 6572 223e 4465 6369 6469 6e67  t-over">Deciding
+00006040: 2063 6872 6f6d 6f73 6f6d 6573 2061 6e64   chromosomes and
+00006050: 2066 6561 7475 7265 7320 666f 7220 616e   features for an
+00006060: 6e6f 7461 7469 6f6e 206c 6966 742d 6f76  notation lift-ov
+00006070: 6572 3c2f 613e 3c2f 6c69 3e0a 3c6c 6920  er</a></li>.<li 
+00006080: 636c 6173 733d 2274 6f63 7472 6565 2d6c  class="toctree-l
+00006090: 3222 3e3c 6120 636c 6173 733d 2272 6566  2"><a class="ref
+000060a0: 6572 656e 6365 2069 6e74 6572 6e61 6c22  erence internal"
+000060b0: 2068 7265 663d 2268 7474 7073 3a2f 2f63   href="https://c
+000060c0: 6362 2e6a 6875 2e65 6475 2f6c 6966 746f  cb.jhu.edu/lifto
+000060d0: 6e2f 636f 6e74 656e 742f 6265 6869 6e64  n/content/behind
+000060e0: 5f73 6365 6e65 732e 6874 6d6c 236d 6174  _scenes.html#mat
+000060f0: 6368 696e 672d 6d69 6e69 7072 6f74 2d6c  ching-miniprot-l
+00006100: 6966 746f 6666 2d67 656e 6f6d 652d 616e  iftoff-genome-an
+00006110: 6e6f 7461 7469 6f6e 223e 4d61 7463 6869  notation">Matchi
+00006120: 6e67 206d 696e 6970 726f 7420 2661 6d70  ng miniprot &amp
+00006130: 3b20 4c69 6674 6f66 6620 6765 6e6f 6d65  ; Liftoff genome
+00006140: 2061 6e6e 6f74 6174 696f 6e3c 2f61 3e3c   annotation</a><
+00006150: 2f6c 693e 0a3c 6c69 2063 6c61 7373 3d22  /li>.<li class="
+00006160: 746f 6374 7265 652d 6c32 223e 3c61 2063  toctree-l2"><a c
+00006170: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
+00006180: 696e 7465 726e 616c 2220 6872 6566 3d22  internal" href="
+00006190: 6874 7470 733a 2f2f 6363 622e 6a68 752e  https://ccb.jhu.
+000061a0: 6564 752f 6c69 6674 6f6e 2f63 6f6e 7465  edu/lifton/conte
+000061b0: 6e74 2f62 6568 696e 645f 7363 656e 6573  nt/behind_scenes
+000061c0: 2e68 746d 6c23 7072 6f74 6569 6e2d 6d61  .html#protein-ma
+000061d0: 7869 6d69 7a61 7469 6f6e 2d61 6c67 6f72  ximization-algor
+000061e0: 6974 686d 223e 5072 6f74 6569 6e2d 6d61  ithm">Protein-ma
+000061f0: 7869 6d69 7a61 7469 6f6e 2061 6c67 6f72  ximization algor
+00006200: 6974 686d 3c2f 613e 3c2f 6c69 3e0a 3c6c  ithm</a></li>.<l
+00006210: 6920 636c 6173 733d 2274 6f63 7472 6565  i class="toctree
+00006220: 2d6c 3222 3e3c 6120 636c 6173 733d 2272  -l2"><a class="r
+00006230: 6566 6572 656e 6365 2069 6e74 6572 6e61  eference interna
+00006240: 6c22 2068 7265 663d 2268 7474 7073 3a2f  l" href="https:/
+00006250: 2f63 6362 2e6a 6875 2e65 6475 2f6c 6966  /ccb.jhu.edu/lif
+00006260: 746f 6e2f 636f 6e74 656e 742f 6265 6869  ton/content/behi
+00006270: 6e64 5f73 6365 6e65 732e 6874 6d6c 236d  nd_scenes.html#m
+00006280: 7574 6174 696f 6e2d 7265 706f 7274 223e  utation-report">
+00006290: 4d75 7461 7469 6f6e 2072 6570 6f72 743c  Mutation report<
+000062a0: 2f61 3e3c 2f6c 693e 0a3c 6c69 2063 6c61  /a></li>.<li cla
+000062b0: 7373 3d22 746f 6374 7265 652d 6c32 223e  ss="toctree-l2">
+000062c0: 3c61 2063 6c61 7373 3d22 7265 6665 7265  <a class="refere
+000062d0: 6e63 6520 696e 7465 726e 616c 2220 6872  nce internal" hr
+000062e0: 6566 3d22 6874 7470 733a 2f2f 6363 622e  ef="https://ccb.
+000062f0: 6a68 752e 6564 752f 6c69 6674 6f6e 2f63  jhu.edu/lifton/c
+00006300: 6f6e 7465 6e74 2f62 6568 696e 645f 7363  ontent/behind_sc
+00006310: 656e 6573 2e68 746d 6c23 7265 6665 7265  enes.html#refere
+00006320: 6e63 6522 3e52 6566 6572 656e 6365 3c2f  nce">Reference</
+00006330: 613e 3c2f 6c69 3e0a 3c2f 756c 3e0a 3c2f  a></li>.</ul>.</
+00006340: 6c69 3e0a 3c6c 6920 636c 6173 733d 2274  li>.<li class="t
+00006350: 6f63 7472 6565 2d6c 3122 3e3c 6120 636c  octree-l1"><a cl
+00006360: 6173 733d 2272 6566 6572 656e 6365 2069  ass="reference i
+00006370: 6e74 6572 6e61 6c22 2068 7265 663d 2268  nternal" href="h
+00006380: 7474 7073 3a2f 2f63 6362 2e6a 6875 2e65  ttps://ccb.jhu.e
+00006390: 6475 2f6c 6966 746f 6e2f 636f 6e74 656e  du/lifton/conten
+000063a0: 742f 686f 775f 746f 5f70 6167 652e 6874  t/how_to_page.ht
+000063b0: 6d6c 223e 4641 5120 2e2e 2e3c 2f61 3e3c  ml">FAQ ...</a><
+000063c0: 2f6c 693e 0a3c 6c69 2063 6c61 7373 3d22  /li>.<li class="
+000063d0: 746f 6374 7265 652d 6c31 223e 3c61 2063  toctree-l1"><a c
+000063e0: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
+000063f0: 696e 7465 726e 616c 2220 6872 6566 3d22  internal" href="
+00006400: 6874 7470 733a 2f2f 6363 622e 6a68 752e  https://ccb.jhu.
+00006410: 6564 752f 6c69 6674 6f6e 2f63 6f6e 7465  edu/lifton/conte
+00006420: 6e74 2f66 756e 6374 696f 6e5f 6d61 6e75  nt/function_manu
+00006430: 616c 2e68 746d 6c22 3e55 7365 7220 4d61  al.html">User Ma
+00006440: 6e75 616c 3c2f 613e 3c75 6c3e 0a3c 6c69  nual</a><ul>.<li
+00006450: 2063 6c61 7373 3d22 746f 6374 7265 652d   class="toctree-
+00006460: 6c32 223e 3c61 2063 6c61 7373 3d22 7265  l2"><a class="re
+00006470: 6665 7265 6e63 6520 696e 7465 726e 616c  ference internal
+00006480: 2220 6872 6566 3d22 6874 7470 733a 2f2f  " href="https://
+00006490: 6363 622e 6a68 752e 6564 752f 6c69 6674  ccb.jhu.edu/lift
+000064a0: 6f6e 2f63 6f6e 7465 6e74 2f66 756e 6374  on/content/funct
+000064b0: 696f 6e5f 6d61 6e75 616c 2e68 746d 6c23  ion_manual.html#
+000064c0: 6c69 6674 6f6e 223e 4c69 6674 4f6e 3c2f  lifton">LiftOn</
+000064d0: 613e 3c2f 6c69 3e0a 3c2f 756c 3e0a 3c2f  a></li>.</ul>.</
+000064e0: 6c69 3e0a 3c6c 6920 636c 6173 733d 2274  li>.<li class="t
+000064f0: 6f63 7472 6565 2d6c 3122 3e3c 6120 636c  octree-l1"><a cl
+00006500: 6173 733d 2272 6566 6572 656e 6365 2069  ass="reference i
+00006510: 6e74 6572 6e61 6c22 2068 7265 663d 2268  nternal" href="h
+00006520: 7474 7073 3a2f 2f63 6362 2e6a 6875 2e65  ttps://ccb.jhu.e
+00006530: 6475 2f6c 6966 746f 6e2f 636f 6e74 656e  du/lifton/conten
+00006540: 742f 6368 616e 6765 6c6f 672e 6874 6d6c  t/changelog.html
+00006550: 223e 4368 616e 6765 6c6f 673c 2f61 3e3c  ">Changelog</a><
+00006560: 756c 3e0a 3c6c 6920 636c 6173 733d 2274  ul>.<li class="t
+00006570: 6f63 7472 6565 2d6c 3222 3e3c 6120 636c  octree-l2"><a cl
+00006580: 6173 733d 2272 6566 6572 656e 6365 2069  ass="reference i
+00006590: 6e74 6572 6e61 6c22 2068 7265 663d 2268  nternal" href="h
+000065a0: 7474 7073 3a2f 2f63 6362 2e6a 6875 2e65  ttps://ccb.jhu.e
+000065b0: 6475 2f6c 6966 746f 6e2f 636f 6e74 656e  du/lifton/conten
+000065c0: 742f 6368 616e 6765 6c6f 672e 6874 6d6c  t/changelog.html
+000065d0: 2376 312d 302d 3022 3e76 312e 302e 303c  #v1-0-0">v1.0.0<
+000065e0: 2f61 3e3c 2f6c 693e 0a3c 2f75 6c3e 0a3c  /a></li>.</ul>.<
+000065f0: 2f6c 693e 0a3c 6c69 2063 6c61 7373 3d22  /li>.<li class="
+00006600: 746f 6374 7265 652d 6c31 223e 3c61 2063  toctree-l1"><a c
+00006610: 6c61 7373 3d22 7265 6665 7265 6e63 6520  lass="reference 
+00006620: 696e 7465 726e 616c 2220 6872 6566 3d22  internal" href="
+00006630: 6874 7470 733a 2f2f 6363 622e 6a68 752e  https://ccb.jhu.
+00006640: 6564 752f 6c69 6674 6f6e 2f63 6f6e 7465  edu/lifton/conte
+00006650: 6e74 2f6c 6963 656e 7365 2e68 746d 6c22  nt/license.html"
+00006660: 3e4c 6963 656e 7365 3c2f 613e 3c2f 6c69  >License</a></li
+00006670: 3e0a 3c6c 6920 636c 6173 733d 2274 6f63  >.<li class="toc
+00006680: 7472 6565 2d6c 3122 3e3c 6120 636c 6173  tree-l1"><a clas
+00006690: 733d 2272 6566 6572 656e 6365 2069 6e74  s="reference int
+000066a0: 6572 6e61 6c22 2068 7265 663d 2268 7474  ernal" href="htt
+000066b0: 7073 3a2f 2f63 6362 2e6a 6875 2e65 6475  ps://ccb.jhu.edu
+000066c0: 2f6c 6966 746f 6e2f 636f 6e74 656e 742f  /lifton/content/
+000066d0: 636f 6e74 6163 742e 6874 6d6c 223e 436f  contact.html">Co
+000066e0: 6e74 6163 743c 2f61 3e3c 2f6c 693e 0a3c  ntact</a></li>.<
+000066f0: 2f75 6c3e 0a3c 2f64 6976 3e0a 3c64 6976  /ul>.</div>.<div
+00006700: 2063 6c61 7373 3d22 6c69 6e65 2d62 6c6f   class="line-blo
+00006710: 636b 223e 0a3c 6469 7620 636c 6173 733d  ck">.<div class=
+00006720: 226c 696e 6522 3e3c 6272 3e3c 2f64 6976  "line"><br></div
+00006730: 3e0a 3c2f 6469 763e 0a3c 2f73 6563 7469  >.</div>.</secti
+00006740: 6f6e 3e0a 3c73 6563 7469 6f6e 2069 643d  on>.<section id=
+00006750: 226c 6966 746f 6e2d 732d 6c69 6d69 7461  "lifton-s-limita
+00006760: 7469 6f6e 223e 0a3c 6832 3e4c 6966 744f  tion">.<h2>LiftO
+00006770: 6e27 7320 6c69 6d69 7461 7469 6f6e 3c61  n's limitation<a
+00006780: 2063 6c61 7373 3d22 6865 6164 6572 6c69   class="headerli
+00006790: 6e6b 2220 6872 6566 3d22 236c 6966 746f  nk" href="#lifto
+000067a0: 6e2d 732d 6c69 6d69 7461 7469 6f6e 2220  n-s-limitation" 
+000067b0: 7469 746c 653d 2250 6572 6d61 6c69 6e6b  title="Permalink
+000067c0: 2074 6f20 7468 6973 2068 6561 6469 6e67   to this heading
+000067d0: 223e 233c 2f61 3e3c 2f68 323e 0a3c 703e  ">#</a></h2>.<p>
+000067e0: 4c69 6674 4f6e 2773 203c 656d 3e63 6861  LiftOn's <em>cha
+000067f0: 696e 696e 6720 616c 676f 7269 7468 6d3c  ining algorithm<
+00006800: 2f65 6d3e 2063 7572 7265 6e74 6c79 206f  /em> currently o
+00006810: 6e6c 7920 7574 696c 697a 6573 206d 696e  nly utilizes min
+00006820: 6970 726f 7420 616c 6967 6e6d 656e 7420  iprot alignment 
+00006830: 7265 7375 6c74 7320 746f 2066 6978 2074  results to fix t
+00006840: 6865 204c 6966 746f 6666 2061 6e6e 6f74  he Liftoff annot
+00006850: 6174 696f 6e2e 2048 6f77 6576 6572 2c20  ation. However, 
+00006860: 6974 2063 616e 2062 6520 6578 7465 6e64  it can be extend
+00006870: 6564 2074 6f20 6368 6169 6e20 746f 6765  ed to chain toge
+00006880: 7468 6572 206d 756c 7469 706c 6520 444e  ther multiple DN
+00006890: 412d 2061 6e64 2070 726f 7465 696e 2d62  A- and protein-b
+000068a0: 6173 6564 2061 6e6e 6f74 6174 696f 6e20  ased annotation 
+000068b0: 6669 6c65 7320 6f72 2061 6173 656d 626c  files or aasembl
+000068c0: 6564 2052 4e41 2d53 6571 2074 7261 6e73  ed RNA-Seq trans
+000068d0: 6372 6970 7473 2e3c 2f70 3e0a 3c70 3e44  cripts.</p>.<p>D
+000068e0: 4e41 2d20 616e 6420 7072 6f74 6569 6e2d  NA- and protein-
+000068f0: 6261 7365 6420 6d65 7468 6f64 7320 7374  based methods st
+00006900: 696c 6c20 6861 7665 2073 6f6d 6520 6c69  ill have some li
+00006910: 6d69 7461 7469 6f6e 732e 2057 6520 6172  mitations. We ar
+00006920: 6520 6465 7665 6c6f 7069 6e67 2061 206d  e developing a m
+00006930: 6f64 756c 6520 746f 206d 6572 6765 2074  odule to merge t
+00006940: 6865 204c 6966 744f 6e20 616e 6e6f 7461  he LiftOn annota
+00006950: 7469 6f6e 2077 6974 6820 7468 6520 7265  tion with the re
+00006960: 6c65 6173 6564 2063 7572 6174 6564 2061  leased curated a
+00006970: 6e6e 6f74 6174 696f 6e73 2074 6f20 6765  nnotations to ge
+00006980: 6e65 7261 7465 2062 6574 7465 7220 616e  nerate better an
+00006990: 6e6f 7461 7469 6f6e 732e 3c2f 703e 0a3c  notations.</p>.<
+000069a0: 703e 5468 6520 4c69 6674 4f6e 203c 656d  p>The LiftOn <em
+000069b0: 3e63 6861 696e 696e 6720 616c 676f 7269  >chaining algori
+000069c0: 7468 6d3c 2f65 6d3e 206e 6f77 2064 6f65  thm</em> now doe
+000069d0: 7320 6e6f 7420 7375 7070 6f72 7420 6d75  s not support mu
+000069e0: 6c74 692d 7468 7265 6164 696e 672e 2054  lti-threading. T
+000069f0: 6869 7320 6675 6e63 7469 6f6e 616c 6974  his functionalit
+00006a00: 7920 7374 616e 6473 2061 7320 6f75 7220  y stands as our 
+00006a10: 6e65 7874 2074 6172 6765 7465 6420 6665  next targeted fe
+00006a20: 6174 7572 6520 6f6e 2074 6865 2064 6576  ature on the dev
+00006a30: 656c 6f70 6d65 6e74 2068 6f72 697a 6f6e  elopment horizon
+00006a40: 213c 2f70 3e0a 3c64 6976 2063 6c61 7373  !</p>.<div class
+00006a50: 3d22 6c69 6e65 2d62 6c6f 636b 223e 0a3c  ="line-block">.<
+00006a60: 6469 7620 636c 6173 733d 226c 696e 6522  div class="line"
+00006a70: 3e3c 6272 3e3c 2f64 6976 3e0a 3c2f 6469  ><br></div>.</di
+00006a80: 763e 0a3c 2f73 6563 7469 6f6e 3e0a 3c2f  v>.</section>.</
+00006a90: 7365 6374 696f 6e3e 0a0a 2020 2020 2020  section>..      
+00006aa0: 2020 0a0a 2323 203c 6120 6e61 6d65 3d22    ..## <a name="
+00006ab0: 6369 7461 7469 6f6e 223e 3c2f 613e 4369  citation"></a>Ci
+00006ac0: 7461 7469 6f6e 3c61 2063 6c61 7373 3d22  tation<a class="
+00006ad0: 6865 6164 6572 6c69 6e6b 2220 6872 6566  headerlink" href
+00006ae0: 3d22 2363 6974 6174 696f 6e22 2074 6974  ="#citation" tit
+00006af0: 6c65 3d22 5065 726d 616c 696e 6b20 746f  le="Permalink to
+00006b00: 2074 6869 7320 6865 6164 696e 6722 3e23   this heading">#
+00006b10: 3c2f 613e 0a0a 0a4b 7561 6e2d 4861 6f20  </a>...Kuan-Hao 
+00006b20: 4368 616f 2a2c 204d 6968 6165 6c61 2050  Chao*, Mihaela P
+00006b30: 6572 7465 612c 2053 7465 7665 6e20 4c20  ertea, Steven L 
+00006b40: 5361 6c7a 6265 7267 2a2c 2022 4c69 6674  Salzberg*, "Lift
+00006b50: 4f6e 3a20 6120 746f 6f6c 2074 6f20 696d  On: a tool to im
+00006b60: 7072 6f76 6520 616e 6e6f 7461 7469 6f6e  prove annotation
+00006b70: 7320 666f 7220 7072 6f74 6569 6e2d 636f  s for protein-co
+00006b80: 6469 6e67 2067 656e 6573 2064 7572 696e  ding genes durin
+00006b90: 6720 7468 6520 6c69 6674 2d6f 7665 7220  g the lift-over 
+00006ba0: 7072 6f63 6573 732e 222c 203c 693e 6269  process.", <i>bi
+00006bb0: 6f52 7869 763c 2f69 3e20 3c62 3e32 3032  oRxiv</i> <b>202
+00006bc0: 332e 3037 2e32 372e 3535 3037 3534 3c2f  3.07.27.550754</
+00006bd0: 623e 2c20 646f 693a 205b 6874 7470 733a  b>, doi: [https:
+00006be0: 2f2f 646f 692e 6f72 672f 3130 2e31 3130  //doi.org/10.110
+00006bf0: 312f 3230 3233 2e30 372e 3237 2e35 3530  1/2023.07.27.550
+00006c00: 3735 345d 2868 7474 7073 3a2f 2f64 6f69  754](https://doi
+00006c10: 2e6f 7267 2f31 302e 3131 3031 2f32 3032  .org/10.1101/202
+00006c20: 332e 3037 2e32 372e 3535 3037 3534 292c  3.07.27.550754),
+00006c30: 2032 3032 330a 0a3c 6272 3e0a 3c62 723e   2023..<br>.<br>
+00006c40: 0a3c 6272 3e0a 0a3c 696d 6720 616c 743d  .<br>..<img alt=
+00006c50: 224d 7920 4c6f 676f 2220 636c 6173 733d  "My Logo" class=
+00006c60: 226c 6f67 6f20 6865 6164 6572 2d69 6d61  "logo header-ima
+00006c70: 6765 206f 6e6c 792d 6c69 6768 7420 616c  ge only-light al
+00006c80: 6967 6e2d 6365 6e74 6572 2220 7372 633d  ign-center" src=
+00006c90: 2268 7474 7073 3a2f 2f73 746f 7261 6765  "https://storage
+00006ca0: 2e67 6f6f 676c 6561 7069 732e 636f 6d2f  .googleapis.com/
+00006cb0: 7374 6f72 6167 652e 6b68 6368 616f 2e63  storage.khchao.c
+00006cc0: 6f6d 2f66 6967 7572 6573 2f6a 6875 2d6c  om/figures/jhu-l
+00006cd0: 6f67 6f2d 6461 726b 2e70 6e67 223e 0a    ogo-dark.png">.
```

### Comparing `lifton-0.0.3/lifton.egg-info/SOURCES.txt` & `lifton-1.0.0/lifton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lifton-0.0.3/setup.py` & `lifton-1.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 from pathlib import Path
 
 this_directory = Path(__file__).resolve().parent
 long_description = (this_directory / "./README.md").read_text()
 setuptools.setup(
 	name="lifton",
-	version="0.0.3",
+	version="1.0.0",
 	author="Kuan-Hao Chao",
 	author_email="kh.chao@cs.jhu.edu",
-	description="A protein-coding gene annotation fixing tool",
+	description="Combining DNA and protein alignments to improve genome annotation with LiftOn",
 	url="https://github.com/Kuanhao-Chao/Lifton",
 	install_requires=['numpy>= 1.22.0', "biopython>=1.76", "cigar>=0.1.3", "parasail>=1.2.4", 'intervaltree>=3.1.0', 'interlap>=0.2.6', 'networkx>=2.4', 'pyfaidx>=0.5.8', 'pysam>=0.19.1', 'gffutils>=0.10.1', 'ujson>=3.2.0'],
 	python_requires='>=3.6',
 	packages=setuptools.find_packages(),
 	entry_points={'console_scripts': ['lifton = lifton.lifton:main'], },
         long_description=long_description,
         long_description_content_type='text/markdown'
-)
+)
```


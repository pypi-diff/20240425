# Comparing `tmp/exafs_neo-2.0.4.tar.gz` & `tmp/exafs_neo-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exafs_neo-2.0.4.tar", last modified: Sat Apr 20 17:35:44 2024, max compression
+gzip compressed data, was "exafs_neo-2.0.5.tar", last modified: Wed Apr 24 22:07:05 2024, max compression
```

## Comparing `exafs_neo-2.0.4.tar` & `exafs_neo-2.0.5.tar`

### file list

```diff
@@ -1,66 +1,68 @@
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-20 17:35:44.953078 exafs_neo-2.0.4/
--rw-r--r--   0 andy       (501) staff       (20)    35198 2021-08-14 12:28:51.000000 exafs_neo-2.0.4/LICENSE
--rw-r--r--   0 andy       (501) staff       (20)     5897 2024-04-20 17:35:44.953001 exafs_neo-2.0.4/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)     5337 2024-04-20 17:35:07.000000 exafs_neo-2.0.4/README.md
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-20 17:35:44.942760 exafs_neo-2.0.4/exafs_neo/
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-02-03 07:16:06.000000 exafs_neo-2.0.4/exafs_neo/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)      152 2024-04-20 17:34:57.000000 exafs_neo-2.0.4/exafs_neo/_version.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-20 17:35:44.945072 exafs_neo-2.0.4/exafs_neo/analysis/
--rw-r--r--   0 andy       (501) staff       (20)    28217 2024-04-02 02:45:54.000000 exafs_neo-2.0.4/exafs_neo/analysis/EXAFS_Analysis.py
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-19 04:33:48.000000 exafs_neo-2.0.4/exafs_neo/analysis/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)    20093 2024-03-19 06:15:52.000000 exafs_neo-2.0.4/exafs_neo/analysis/larch_score.py
--rw-r--r--   0 andy       (501) staff       (20)     4189 2024-04-02 00:35:24.000000 exafs_neo-2.0.4/exafs_neo/exafs.py
--rw-r--r--   0 andy       (501) staff       (20)     5812 2024-04-02 02:57:21.000000 exafs_neo-2.0.4/exafs_neo/exafs_pop.py
--rw-r--r--   0 andy       (501) staff       (20)     5263 2024-04-02 02:59:48.000000 exafs_neo-2.0.4/exafs_neo/exafsfileobj.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-20 17:35:44.948035 exafs_neo-2.0.4/exafs_neo/gui/
--rw-r--r--   0 andy       (501) staff       (20)     3079 2024-03-19 04:34:51.000000 exafs_neo-2.0.4/exafs_neo/gui/Analysis_plot.py
--rw-r--r--   0 andy       (501) staff       (20)     5721 2024-03-18 17:12:48.000000 exafs_neo-2.0.4/exafs_neo/gui/Background_plot.py
--rw-r--r--   0 andy       (501) staff       (20)     2124 2024-03-18 17:11:48.000000 exafs_neo-2.0.4/exafs_neo/gui/Console.py
--rw-r--r--   0 andy       (501) staff       (20)     1575 2024-04-20 17:28:50.000000 exafs_neo-2.0.4/exafs_neo/gui/Misc_Function.py
--rw-r--r--   0 andy       (501) staff       (20)    55561 2024-04-02 19:11:16.000000 exafs_neo-2.0.4/exafs_neo/gui/XAFS_GUI.py
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-18 05:23:32.000000 exafs_neo-2.0.4/exafs_neo/gui/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     3268 2024-03-18 17:10:18.000000 exafs_neo-2.0.4/exafs_neo/gui/feff_folder_larch.py
--rw-r--r--   0 andy       (501) staff       (20)      265 2023-05-16 01:15:35.000000 exafs_neo-2.0.4/exafs_neo/gui/first_shell_fits.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-20 17:35:44.949039 exafs_neo-2.0.4/exafs_neo/gui/media/
--rw-r--r--   0 andy       (501) staff       (20)      539 2023-07-01 21:09:31.000000 exafs_neo-2.0.4/exafs_neo/gui/media/Citation
--rw-r--r--   0 andy       (501) staff       (20)    35198 2024-04-02 19:10:46.000000 exafs_neo-2.0.4/exafs_neo/gui/media/LICENSE
--rw-r--r--   0 andy       (501) staff       (20)     3848 2021-08-14 12:28:51.000000 exafs_neo-2.0.4/exafs_neo/gui/media/icon.png
--rw-r--r--   0 andy       (501) staff       (20)      983 2024-04-02 03:00:16.000000 exafs_neo-2.0.4/exafs_neo/helper.py
--rw-r--r--   0 andy       (501) staff       (20)     3909 2024-04-02 03:07:35.000000 exafs_neo-2.0.4/exafs_neo/individual.py
--rw-r--r--   0 andy       (501) staff       (20)     6206 2024-04-02 03:12:20.000000 exafs_neo-2.0.4/exafs_neo/ini_parser.py
--rwxr-xr-x   0 andy       (501) staff       (20)     1317 2024-04-02 03:13:29.000000 exafs_neo-2.0.4/exafs_neo/input_arg.py
--rw-r--r--   0 andy       (501) staff       (20)     9228 2024-03-23 23:40:18.000000 exafs_neo-2.0.4/exafs_neo/neoCrossOver.py
--rw-r--r--   0 andy       (501) staff       (20)     3364 2024-04-02 03:14:48.000000 exafs_neo-2.0.4/exafs_neo/neoFilePars.py
--rw-r--r--   0 andy       (501) staff       (20)     9223 2024-04-02 03:15:32.000000 exafs_neo-2.0.4/exafs_neo/neoMutator.py
--rw-r--r--   0 andy       (501) staff       (20)    13651 2024-04-17 06:16:45.000000 exafs_neo-2.0.4/exafs_neo/neoPars.py
--rw-r--r--   0 andy       (501) staff       (20)     3122 2024-04-02 03:23:54.000000 exafs_neo-2.0.4/exafs_neo/neoResult.py
--rw-r--r--   0 andy       (501) staff       (20)     3920 2024-04-02 03:27:20.000000 exafs_neo-2.0.4/exafs_neo/neoSelector.py
--rwxr-xr-x   0 andy       (501) staff       (20)     5748 2024-04-02 05:25:47.000000 exafs_neo-2.0.4/exafs_neo/parser.py
--rw-r--r--   0 andy       (501) staff       (20)     2953 2024-04-02 05:26:13.000000 exafs_neo-2.0.4/exafs_neo/pathObj.py
--rw-r--r--   0 andy       (501) staff       (20)     5121 2024-04-02 03:36:53.000000 exafs_neo-2.0.4/exafs_neo/pathrange.py
--rw-r--r--   0 andy       (501) staff       (20)     1321 2024-04-02 03:39:27.000000 exafs_neo-2.0.4/exafs_neo/pathrange_file.py
--rw-r--r--   0 andy       (501) staff       (20)    19175 2024-04-02 05:26:30.000000 exafs_neo-2.0.4/exafs_neo/utils.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-20 17:35:44.952709 exafs_neo-2.0.4/exafs_neo.egg-info/
--rw-r--r--   0 andy       (501) staff       (20)     5897 2024-04-20 17:35:44.000000 exafs_neo-2.0.4/exafs_neo.egg-info/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)     1482 2024-04-20 17:35:44.000000 exafs_neo-2.0.4/exafs_neo.egg-info/SOURCES.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2024-04-20 17:35:44.000000 exafs_neo-2.0.4/exafs_neo.egg-info/dependency_links.txt
--rw-r--r--   0 andy       (501) staff       (20)       99 2024-04-20 17:35:44.000000 exafs_neo-2.0.4/exafs_neo.egg-info/entry_points.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2024-02-18 07:51:41.000000 exafs_neo-2.0.4/exafs_neo.egg-info/not-zip-safe
--rw-r--r--   0 andy       (501) staff       (20)       40 2024-04-20 17:35:44.000000 exafs_neo-2.0.4/exafs_neo.egg-info/requires.txt
--rw-r--r--   0 andy       (501) staff       (20)       16 2024-04-20 17:35:44.000000 exafs_neo-2.0.4/exafs_neo.egg-info/top_level.txt
--rw-r--r--   0 andy       (501) staff       (20)       79 2024-04-20 17:35:44.953330 exafs_neo-2.0.4/setup.cfg
--rw-r--r--   0 andy       (501) staff       (20)     1240 2024-04-19 05:22:39.000000 exafs_neo-2.0.4/setup.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-20 17:35:44.952399 exafs_neo-2.0.4/tests/
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-17 22:01:17.000000 exafs_neo-2.0.4/tests/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     4089 2024-03-23 20:03:07.000000 exafs_neo-2.0.4/tests/test_EXAFS_analysis.py
--rw-r--r--   0 andy       (501) staff       (20)     1607 2024-03-23 19:26:46.000000 exafs_neo-2.0.4/tests/test_exafs_fileobj.py
--rw-r--r--   0 andy       (501) staff       (20)     3857 2024-03-23 20:01:49.000000 exafs_neo-2.0.4/tests/test_exafs_pars.py
--rw-r--r--   0 andy       (501) staff       (20)     2280 2024-03-20 02:02:00.000000 exafs_neo-2.0.4/tests/test_exafs_pathObj.py
--rw-r--r--   0 andy       (501) staff       (20)     1573 2024-02-03 07:05:06.000000 exafs_neo-2.0.4/tests/test_exafs_pathrange.py
--rw-r--r--   0 andy       (501) staff       (20)     1053 2024-03-20 03:41:05.000000 exafs_neo-2.0.4/tests/test_individual.py
--rw-r--r--   0 andy       (501) staff       (20)      514 2024-03-17 20:09:18.000000 exafs_neo-2.0.4/tests/test_ini_parser.py
--rw-r--r--   0 andy       (501) staff       (20)     3385 2024-03-23 20:03:36.000000 exafs_neo-2.0.4/tests/test_larchscore.py
--rw-r--r--   0 andy       (501) staff       (20)      976 2024-03-23 23:13:20.000000 exafs_neo-2.0.4/tests/test_neo_pop.py
--rw-r--r--   0 andy       (501) staff       (20)     5754 2024-03-31 00:14:43.000000 exafs_neo-2.0.4/tests/test_neocrossover.py
--rw-r--r--   0 andy       (501) staff       (20)     3771 2024-04-03 00:18:39.000000 exafs_neo-2.0.4/tests/test_neomutator.py
--rw-r--r--   0 andy       (501) staff       (20)      338 2024-02-18 20:02:49.000000 exafs_neo-2.0.4/tests/test_utils.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-24 22:07:05.113795 exafs_neo-2.0.5/
+-rw-r--r--   0 andy       (501) staff       (20)    35198 2021-08-14 12:28:51.000000 exafs_neo-2.0.5/LICENSE
+-rw-r--r--   0 andy       (501) staff       (20)     5782 2024-04-24 22:07:05.113930 exafs_neo-2.0.5/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)     5337 2024-04-24 22:02:46.000000 exafs_neo-2.0.5/README.md
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-24 22:07:05.102360 exafs_neo-2.0.5/exafs_neo/
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-02-03 07:16:06.000000 exafs_neo-2.0.5/exafs_neo/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)      152 2024-04-24 22:02:53.000000 exafs_neo-2.0.5/exafs_neo/_version.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-24 22:07:05.104782 exafs_neo-2.0.5/exafs_neo/analysis/
+-rw-r--r--   0 andy       (501) staff       (20)    28217 2024-04-02 02:45:54.000000 exafs_neo-2.0.5/exafs_neo/analysis/EXAFS_Analysis.py
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-19 04:33:48.000000 exafs_neo-2.0.5/exafs_neo/analysis/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)    20093 2024-03-19 06:15:52.000000 exafs_neo-2.0.5/exafs_neo/analysis/larch_score.py
+-rw-r--r--   0 andy       (501) staff       (20)     4325 2024-04-24 02:36:38.000000 exafs_neo-2.0.5/exafs_neo/exafs.py
+-rw-r--r--   0 andy       (501) staff       (20)     5812 2024-04-02 02:57:21.000000 exafs_neo-2.0.5/exafs_neo/exafs_pop.py
+-rw-r--r--   0 andy       (501) staff       (20)     5263 2024-04-02 02:59:48.000000 exafs_neo-2.0.5/exafs_neo/exafsfileobj.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-24 22:07:05.107544 exafs_neo-2.0.5/exafs_neo/gui/
+-rw-r--r--   0 andy       (501) staff       (20)     3079 2024-03-19 04:34:51.000000 exafs_neo-2.0.5/exafs_neo/gui/Analysis_plot.py
+-rw-r--r--   0 andy       (501) staff       (20)     5721 2024-03-18 17:12:48.000000 exafs_neo-2.0.5/exafs_neo/gui/Background_plot.py
+-rw-r--r--   0 andy       (501) staff       (20)     2124 2024-03-18 17:11:48.000000 exafs_neo-2.0.5/exafs_neo/gui/Console.py
+-rw-r--r--   0 andy       (501) staff       (20)     1575 2024-04-20 17:28:50.000000 exafs_neo-2.0.5/exafs_neo/gui/Misc_Function.py
+-rw-r--r--   0 andy       (501) staff       (20)    54782 2024-04-24 22:01:45.000000 exafs_neo-2.0.5/exafs_neo/gui/XAFS_GUI.py
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-18 05:23:32.000000 exafs_neo-2.0.5/exafs_neo/gui/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     3268 2024-03-18 17:10:18.000000 exafs_neo-2.0.5/exafs_neo/gui/feff_folder_larch.py
+-rw-r--r--   0 andy       (501) staff       (20)      265 2023-05-16 01:15:35.000000 exafs_neo-2.0.5/exafs_neo/gui/first_shell_fits.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-24 22:07:05.109075 exafs_neo-2.0.5/exafs_neo/gui/media/
+-rw-r--r--   0 andy       (501) staff       (20)      539 2023-07-01 21:09:31.000000 exafs_neo-2.0.5/exafs_neo/gui/media/Citation
+-rw-r--r--   0 andy       (501) staff       (20)    35198 2024-04-02 19:10:46.000000 exafs_neo-2.0.5/exafs_neo/gui/media/LICENSE
+-rw-r--r--   0 andy       (501) staff       (20)     3848 2021-08-14 12:28:51.000000 exafs_neo-2.0.5/exafs_neo/gui/media/icon.png
+-rw-r--r--   0 andy       (501) staff       (20)      983 2024-04-02 03:00:16.000000 exafs_neo-2.0.5/exafs_neo/helper.py
+-rw-r--r--   0 andy       (501) staff       (20)     3909 2024-04-02 03:07:35.000000 exafs_neo-2.0.5/exafs_neo/individual.py
+-rw-r--r--   0 andy       (501) staff       (20)     6206 2024-04-02 03:12:20.000000 exafs_neo-2.0.5/exafs_neo/ini_parser.py
+-rwxr-xr-x   0 andy       (501) staff       (20)     1317 2024-04-02 03:13:29.000000 exafs_neo-2.0.5/exafs_neo/input_arg.py
+-rw-r--r--   0 andy       (501) staff       (20)     9228 2024-03-23 23:40:18.000000 exafs_neo-2.0.5/exafs_neo/neoCrossOver.py
+-rw-r--r--   0 andy       (501) staff       (20)     3364 2024-04-02 03:14:48.000000 exafs_neo-2.0.5/exafs_neo/neoFilePars.py
+-rw-r--r--   0 andy       (501) staff       (20)     9223 2024-04-02 03:15:32.000000 exafs_neo-2.0.5/exafs_neo/neoMutator.py
+-rw-r--r--   0 andy       (501) staff       (20)    13873 2024-04-24 02:27:00.000000 exafs_neo-2.0.5/exafs_neo/neoPars.py
+-rw-r--r--   0 andy       (501) staff       (20)     3122 2024-04-02 03:23:54.000000 exafs_neo-2.0.5/exafs_neo/neoResult.py
+-rw-r--r--   0 andy       (501) staff       (20)     3904 2024-04-24 02:04:22.000000 exafs_neo-2.0.5/exafs_neo/neoSelector.py
+-rw-r--r--   0 andy       (501) staff       (20)     3419 2024-04-24 02:27:04.000000 exafs_neo-2.0.5/exafs_neo/neoSolver.py
+-rwxr-xr-x   0 andy       (501) staff       (20)     5748 2024-04-02 05:25:47.000000 exafs_neo-2.0.5/exafs_neo/parser.py
+-rw-r--r--   0 andy       (501) staff       (20)     2953 2024-04-02 05:26:13.000000 exafs_neo-2.0.5/exafs_neo/pathObj.py
+-rw-r--r--   0 andy       (501) staff       (20)     5121 2024-04-02 03:36:53.000000 exafs_neo-2.0.5/exafs_neo/pathrange.py
+-rw-r--r--   0 andy       (501) staff       (20)     1321 2024-04-02 03:39:27.000000 exafs_neo-2.0.5/exafs_neo/pathrange_file.py
+-rw-r--r--   0 andy       (501) staff       (20)    19175 2024-04-02 05:26:30.000000 exafs_neo-2.0.5/exafs_neo/utils.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-24 22:07:05.103770 exafs_neo-2.0.5/exafs_neo.egg-info/
+-rw-r--r--   0 andy       (501) staff       (20)     5782 2024-04-24 22:07:05.000000 exafs_neo-2.0.5/exafs_neo.egg-info/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)     1529 2024-04-24 22:07:05.000000 exafs_neo-2.0.5/exafs_neo.egg-info/SOURCES.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2024-04-24 22:07:05.000000 exafs_neo-2.0.5/exafs_neo.egg-info/dependency_links.txt
+-rw-r--r--   0 andy       (501) staff       (20)       99 2024-04-24 22:07:05.000000 exafs_neo-2.0.5/exafs_neo.egg-info/entry_points.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2024-02-18 07:51:41.000000 exafs_neo-2.0.5/exafs_neo.egg-info/not-zip-safe
+-rw-r--r--   0 andy       (501) staff       (20)       40 2024-04-24 22:07:05.000000 exafs_neo-2.0.5/exafs_neo.egg-info/requires.txt
+-rw-r--r--   0 andy       (501) staff       (20)       16 2024-04-24 22:07:05.000000 exafs_neo-2.0.5/exafs_neo.egg-info/top_level.txt
+-rw-r--r--   0 andy       (501) staff       (20)       79 2024-04-24 22:07:05.114247 exafs_neo-2.0.5/setup.cfg
+-rw-r--r--   0 andy       (501) staff       (20)     1240 2024-04-19 05:22:39.000000 exafs_neo-2.0.5/setup.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-24 22:07:05.113445 exafs_neo-2.0.5/tests/
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-17 22:01:17.000000 exafs_neo-2.0.5/tests/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     4089 2024-03-23 20:03:07.000000 exafs_neo-2.0.5/tests/test_EXAFS_analysis.py
+-rw-r--r--   0 andy       (501) staff       (20)     1607 2024-03-23 19:26:46.000000 exafs_neo-2.0.5/tests/test_exafs_fileobj.py
+-rw-r--r--   0 andy       (501) staff       (20)     3857 2024-03-23 20:01:49.000000 exafs_neo-2.0.5/tests/test_exafs_pars.py
+-rw-r--r--   0 andy       (501) staff       (20)     2280 2024-03-20 02:02:00.000000 exafs_neo-2.0.5/tests/test_exafs_pathObj.py
+-rw-r--r--   0 andy       (501) staff       (20)     1573 2024-02-03 07:05:06.000000 exafs_neo-2.0.5/tests/test_exafs_pathrange.py
+-rw-r--r--   0 andy       (501) staff       (20)     1053 2024-03-20 03:41:05.000000 exafs_neo-2.0.5/tests/test_individual.py
+-rw-r--r--   0 andy       (501) staff       (20)      514 2024-03-17 20:09:18.000000 exafs_neo-2.0.5/tests/test_ini_parser.py
+-rw-r--r--   0 andy       (501) staff       (20)     3385 2024-03-23 20:03:36.000000 exafs_neo-2.0.5/tests/test_larchscore.py
+-rw-r--r--   0 andy       (501) staff       (20)      976 2024-03-23 23:13:20.000000 exafs_neo-2.0.5/tests/test_neo_pop.py
+-rw-r--r--   0 andy       (501) staff       (20)     5754 2024-03-31 00:14:43.000000 exafs_neo-2.0.5/tests/test_neocrossover.py
+-rw-r--r--   0 andy       (501) staff       (20)     3771 2024-04-03 00:18:39.000000 exafs_neo-2.0.5/tests/test_neomutator.py
+-rw-r--r--   0 andy       (501) staff       (20)     3725 2024-04-24 06:01:42.000000 exafs_neo-2.0.5/tests/test_neosolver.py
+-rw-r--r--   0 andy       (501) staff       (20)      338 2024-02-18 20:02:49.000000 exafs_neo-2.0.5/tests/test_utils.py
```

### Comparing `exafs_neo-2.0.4/LICENSE` & `exafs_neo-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/PKG-INFO` & `exafs_neo-2.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 Metadata-Version: 2.1
 Name: exafs_neo
-Version: 2.0.4
+Version: 2.0.5
 Summary: exafs_neo AI analysis using GA
 Home-page: https://github.com/laumiulun/EXAFS_Neo
 Download-URL: https://github.com/laumiulun/EXAFS_Neo/tarball/master
 Author: Miu Lun Lau, Jeff Terry, Min Long
 Author-email: andylau@u.boisestate.edu, jterry98@iit.edu, minlong@boisestate.edu
 License: GPLv3
 Keywords: exafs_neo,AI,analysis
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: xraylarch
-Requires-Dist: attrs
-Requires-Dist: matplotlib
-Requires-Dist: psutil
 
 # EXAFS Neo
 
-#### Versions: 2.0.4
+#### Versions: 2.0.5
 
-#### Last update: Apr 20, 2024
+#### Last update: Apr 24, 2024
 
 <!-- ![example workflow](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/<WORKFLOW_FILE>/badge.svg) -->
 
 [![Test with Ubuntu, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml)[![Test with Windows, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml)
 
 
 EXAFS Neo utilize Genetic algorithm in fitting Extended X-ray absorption fine structure(EXAFS).
```

### Comparing `exafs_neo-2.0.4/README.md` & `exafs_neo-2.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # EXAFS Neo
 
-#### Versions: 2.0.4
+#### Versions: 2.0.5
 
-#### Last update: Apr 20, 2024
+#### Last update: Apr 24, 2024
 
 <!-- ![example workflow](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/<WORKFLOW_FILE>/badge.svg) -->
 
 [![Test with Ubuntu, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml)[![Test with Windows, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml)
 
 
 EXAFS Neo utilize Genetic algorithm in fitting Extended X-ray absorption fine structure(EXAFS).
```

### Comparing `exafs_neo-2.0.4/exafs_neo/analysis/EXAFS_Analysis.py` & `exafs_neo-2.0.5/exafs_neo/analysis/EXAFS_Analysis.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/analysis/larch_score.py` & `exafs_neo-2.0.5/exafs_neo/analysis/larch_score.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/exafs.py` & `exafs_neo-2.0.5/exafs_neo/exafs.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from exafs_neo.helper import banner
 from exafs_neo.utils import NeoLogger, STRColors
 from exafs_neo.neoCrossOver import NeoCrossover
 from exafs_neo.neoSelector import NeoSelector
 from exafs_neo.neoResult import NeoResult
 from exafs_neo.ini_parser import validate_input_file
 from exafs_neo.parser import InputParamsParser
+from neoSolver import NeoSolver
 
 
 class ExafsNeo:
 
     def __init__(self, verbose_lvl=5):
         """
         Initialize Params:
@@ -22,14 +23,15 @@
 
         print(banner())
         self.logger = NeoLogger()
         self.exafs_neo_pars = NeoPars()
         self.mutator = NeoMutator(logger=self.logger)
         self.selector = NeoSelector(logger=self.logger)
         self.crossOver = NeoCrossover(logger=self.logger)
+        self.solver = NeoSolver(logger=self.logger)
         self.neo_population = None
         self.verbose_lvl = verbose_lvl
         self.result = NeoResult(logger=self.logger)
         self.input_parameters = None
 
     def exafs_read(self, filepath=None, input_parameters=None):
         """
@@ -63,14 +65,15 @@
         self.neo_population = NeoPopulations(self.exafs_neo_pars)
         self.neo_population.initialize_populations()
         self.result.initialize(self.exafs_neo_pars)
         # Initialize all the operators
         self.selector.initialize(self.exafs_neo_pars)
         self.crossOver.initialize(self.exafs_neo_pars)
         self.mutator.initialize(self.exafs_neo_pars)
+        self.solver.initialize(self.exafs_neo_pars)
 
     def run(self):
         """
         Initialize a EXAFS Run
         :return: result class 
         """
         STRColors.run_verbose_start(self.logger, self.exafs_neo_pars, verbose_lvl=self.verbose_lvl)
```

### Comparing `exafs_neo-2.0.4/exafs_neo/exafs_pop.py` & `exafs_neo-2.0.5/exafs_neo/exafs_pop.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/exafsfileobj.py` & `exafs_neo-2.0.5/exafs_neo/exafsfileobj.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/gui/Analysis_plot.py` & `exafs_neo-2.0.5/exafs_neo/gui/Analysis_plot.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/gui/Background_plot.py` & `exafs_neo-2.0.5/exafs_neo/gui/Background_plot.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/gui/Console.py` & `exafs_neo-2.0.5/exafs_neo/gui/Console.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/gui/Misc_Function.py` & `exafs_neo-2.0.5/exafs_neo/gui/Misc_Function.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/gui/XAFS_GUI.py` & `exafs_neo-2.0.5/exafs_neo/gui/XAFS_GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 Please start the program within the "gui" directory, or "select file" buttons won't start the user in EXAFS.
 "Select Directory" button starts the user in EXAFS/path_files/Cu
 """
 
 # Import Basic libraries
 import os, subprocess, glob
+import pathlib
 # import queue
 from pathlib import Path
 import numpy as np
 
 # Import Tkiner
 import tkinter as tk
 from tkinter import ttk, Tk, N, W, E, S, StringVar, IntVar, DoubleVar, BooleanVar, filedialog, messagebox, PhotoImage, \
@@ -260,27 +261,25 @@
             writer.write(str(populations))
             writer.write(str(mutations))
             writer.write(str(paths))
             writer.write(str(larch_paths))
             writer.write(str(outputs))
 
     def Generate_ini(self):
-        os.chdir("../..")  # change the working directory from gui to EXAFS
         # while proceed ==  False:
         ini_file = filedialog.asksaveasfilename(initialdir=os.getcwd(),
                                                 title="Choose output ini file",
                                                 filetypes=[("ini files", "*.ini")])
         if ini_file is None:
             return
         if not isinstance(ini_file, tuple):
             if len(ini_file) != 0:
                 self.Write_ini(ini_file)
                 messagebox.showinfo('', 'Ini file written to {fileloc}'.format(fileloc=ini_file))
 
-        os.chdir("gui")
 
     def stop_term(self):
         if hasattr(self, 'proc'):
             # print("Stopped EXAFS")
             self.proc.kill()
 
     def run_term(self, file='test_temp.i'):
@@ -308,15 +307,15 @@
             print(self.data_file.get())
 
             sabcor.call_executable(execut_path, self.data_file.get())
             sabcor.edited_final_header(self.data_file.get())
             post_sabcor_file = os.path.splitext(self.data_file.get())
             self.data_file.set(post_sabcor_file[0] + "_sac" + post_sabcor_file[1])
 
-        self.Write_ini('test_temp.i')
+        self.Write_ini(str(pathlib.Path.cwd() / 'test_temp.i'))
 
         command = ['exafs_neo', '-i', file]
         if self.os == 'Windows':
             print(' '.join(command))
             self.proc = subprocess.Popen(' '.join(command), shell=True)
         else:
             self.proc = subprocess.Popen("exec " + ' '.join(command), shell=True)
@@ -427,45 +426,39 @@
 
         comp_list = list(range(1, 6))
         entry_ncomp = ttk.Combobox(self.tab_Inputs, width=7, values=comp_list, textvariable=self.ncomp,
                                    font=self.entryFont)
         entry_ncomp.grid(column=1, row=3, sticky=(W, E), padx=self.padx)
 
         def select_data_file():
-            os.chdir("../..")  # change the working directory from gui to EXAFS
 
             file_name = filedialog.askopenfilenames(initialdir=os.getcwd(), title="Choose xmu/csv", filetypes=(
                 ("xmu files", "*.xmu"), ("csv files", "*.csv"), ("all files", "*.*")))
             if not file_name:
                 self.data_file.set('Please choose file/s')
                 self.temp_data_file.set('Please choose file/s')
-                os.chdir("gui")
             else:
                 if isinstance(file_name, tuple):
                     if len(file_name) == 1:
                         self.data_file.set(str(file_name[0]))
                         self.temp_data_file.set(str(file_name[0]))
                     else:
                         file_list = list(self.root.splitlist(file_name))
                         separator = ' '
                         self.data_file.set(separator.join(file_list))
                         entry_data_file['value'] = file_list
                         self.series.set(True)
-                os.chdir("gui")
 
         def select_output_file():
-            os.chdir("../..")  # change the working directory from gui to EXAFS
             file_name = filedialog.asksaveasfilename(initialdir=os.getcwd(), title="Choose data_file",
                                                      filetypes=(("csv files", "*.csv"), ("all files", "*.*")))
             if not file_name:
                 self.output_file.set('Please choose a file')
-                os.chdir("gui")
             else:
                 self.output_file.set(file_name)
-                os.chdir("gui")
 
         def feff_trace(var, indx, mode):
             # Todo: Need to add assertion to make sure every folder is not normal
             raw_str = []
             for i in range(len(self.feff_file_list)):
                 raw_str.append(self.feff_file_list[i].get())
             raw_feff = ','.join(raw_str)
@@ -542,27 +535,24 @@
             else:
                 # self.txtbox.insert('No feff.inp in folder')
                 self.txtbox.insert(tk.END, "No feff.inp in folder\n")
 
                 # return False
 
         def select_feff_folder(var):
-            os.chdir("../..")  # change the working directory from gui to EXAFS
             # select folder name
             folder_name = filedialog.askdirectory(initialdir=os.getcwd(), title="Select folder")
 
             if not folder_name:
                 var.set('Please choose a directory')
-                os.chdir("gui")
             else:
                 check_feff_folder(folder_name)
                 folder_name = os.path.join(folder_name, 'feff')
                 var.set(folder_name)
 
-                os.chdir("gui")
 
         # add trace back
         self.ncomp.trace_add('write', gen_feff_folder)
         self.ncomp.set(1)
 
         button_data_file = ttk.Button(self.tab_Inputs, text="Choose",
                                       command=select_data_file, style='my.TButton')
@@ -1027,24 +1017,21 @@
         button_run_nini = tk.Button(self.tab_Output, text="Run Multiple Input Files", command=run_multi_ini)
         button_run_nini.grid(column=0, row=10, columnspan=3, sticky=W + E, padx=self.padx, pady=self.pady)
         button_run_nini.config(state='disabled')
 
     def Build_analysis_tab(self):
 
         def select_analysis_folder():
-            os.chdir("../..")  # change the working directory from gui to EXAFS
             folder_name = filedialog.askdirectory(initialdir=os.getcwd(), title="Select folder")
             if not folder_name:
                 analysis_folder.set('Please choose a directory')
-                os.chdir("gui")
             else:
                 # folder_name = os.path.join(folder_name,'feff')
                 analysis_folder.set(folder_name)
                 # print(self.feff_file.get())
-                os.chdir("gui")
 
         def run_analysis():
             params = {}
             # params['base'] = Path(os.getcwd()).parent
             params['base'] = ''
             params['Kmin'] = self.kmin.get()
             params['Kmax'] = self.kmax.get()
@@ -1127,23 +1114,20 @@
         button_plot_occurances = ttk.Button(self.tab_Analysis, text='Plot Occurances',
                                             command=plot_occurances, style='my.TButton')
         button_plot_occurances.grid(column=3, row=3, columnspan=1, sticky=W + E, padx=self.padx, pady=self.pady)
 
     def Build_expert_tab(self):
 
         def select_sabcor_file():
-            os.chdir("../..")  # change the working directory from gui to EXAFS
             file_name = filedialog.askopenfilename(initialdir=os.getcwd(), title="Choose Sabcor Input File",
                                                    filetypes=(("inp file", "*.inp"), ("all files", "*.*")))
             if not file_name:
                 self.sabcor_input_file.set('Please choose a file')
-                os.chdir("gui")
             else:
                 self.sabcor_input_file.set(file_name)
-                os.chdir("gui")
 
         def checkbox_sabcor():
             if self.sabcor_toggle.get() == True:
                 sabcor_input_file.config(state='normal')
                 button_sabcor_input_file.config(state='normal')
                 # allow only single entry
                 self.ncomp.set(1)
```

### Comparing `exafs_neo-2.0.4/exafs_neo/gui/feff_folder_larch.py` & `exafs_neo-2.0.5/exafs_neo/gui/feff_folder_larch.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/gui/media/Citation` & `exafs_neo-2.0.5/exafs_neo/gui/media/Citation`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/gui/media/LICENSE` & `exafs_neo-2.0.5/exafs_neo/gui/media/LICENSE`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/gui/media/icon.png` & `exafs_neo-2.0.5/exafs_neo/gui/media/icon.png`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/helper.py` & `exafs_neo-2.0.5/exafs_neo/helper.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/individual.py` & `exafs_neo-2.0.5/exafs_neo/individual.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/ini_parser.py` & `exafs_neo-2.0.5/exafs_neo/ini_parser.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/input_arg.py` & `exafs_neo-2.0.5/exafs_neo/input_arg.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/neoCrossOver.py` & `exafs_neo-2.0.5/exafs_neo/neoCrossOver.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/neoFilePars.py` & `exafs_neo-2.0.5/exafs_neo/neoFilePars.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/neoMutator.py` & `exafs_neo-2.0.5/exafs_neo/neoMutator.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/neoPars.py` & `exafs_neo-2.0.5/exafs_neo/neoPars.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,14 +166,20 @@
         self.nBestSample = checkKey('nBestSample', input_dicts, 0.3)
         self.nLuckSample = checkKey('nLuckSample', input_dicts, 0.2)
         self.__nPop = checkKey('nPops', input_dicts, 100)
         self.nBest = int(self.__nPop * self.nBestSample)
         self.nLuck = int(self.__nPop * self.nLuckSample)
         self.nCross = self.__nPop - self.nBest - self.nLuck
 
+@define
+class NeoSol:
+    solOpt: int = 0
+    def read_inputs(self, input_dicts):
+        self.solOpt = checkKey('solver_type', input_dicts, 0)
+
 
 class NeoPars:
     def __init__(self, verbose_lvl=5):
         """
         Wrapped all paras together
         """
 
@@ -184,22 +190,23 @@
         self.crossPars = NeoCrossPars()
         self.selPars = NeoSelPars()
         self.exafsPars = EXAFSStaticPars()
         self.bestFitPars = NeoBestFit()
         self.neoFilePars = NeoFilePars()
         self.exafsRangePars = EXAFSPathRange()
         self.exafsPathPars = EXAFSPath()
-
+        self.solPars = NeoSol()
     def read_inputs(self, input_dicts):
         self.fixedPars.read_inputs(input_dicts)
         self.runPars.read_inputs(input_dicts)
         self.exafsPars.read_inputs(input_dicts)
         self.neoFilePars.read_inputs(input_dicts)
         self.mutPars.read_inputs(input_dicts)
         self.selPars.read_inputs(input_dicts)
+        self.solPars.read_inputs(input_dicts)
         self.crossPars.read_inputs(input_dicts)
         self.neoFilePars.initialize_filepath(cycles=0)
 
         self.exafsRangePars.read_inputs(input_dicts, self.exafsPars)
         self.exafsPathPars.read_inputs(self.neoFilePars, self.exafsPars)
 
         self.exafsPathPars.initialize()
```

### Comparing `exafs_neo-2.0.4/exafs_neo/neoResult.py` & `exafs_neo-2.0.5/exafs_neo/neoResult.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/neoSelector.py` & `exafs_neo-2.0.5/exafs_neo/neoSelector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from exafs_neo.exafs_pop import NeoPopulations
 from exafs_neo.neoPars import NeoPars
 
 
-class ExafsSelectorBase:
+class NeoSelectorBase:
     def __init__(self, exafs_pars, logger):
         """
         Initialize the selector base class
         :param exafs_pars:
         :param logger:
         """
         self.logger = logger
@@ -24,15 +24,15 @@
     def select(self, pops):
         pass
 
     def __str__(self):
         return f"Top Percentage: {100 * self.nBest_Percent}%, Lucky: {100 * self.nLucky_Percent}%"
 
 
-class ExafsSelector_RouletteWheel(ExafsSelectorBase):
+class NeoSelector_RouletteWheel(NeoSelectorBase):
     def __init__(self, exafs_pars, logger):
         super().__init__(exafs_pars, logger)
         self.selector_type = 0
         self.selector_operator = "Roulette Wheel"
 
     def select(self, pops):
         # Create parents
@@ -43,15 +43,15 @@
         # Create lucky
         for i in range(self.nLucky):
             next_population.append(pops.generate_individual())
 
         pops.next_population = next_population
 
 
-class ExafsSelector_Tournament(ExafsSelectorBase):
+class NeoSelector_Tournament(NeoSelectorBase):
     def __init__(self, exafs_pars, logger):
         super().__init__(exafs_pars, logger)
         self.selector_type = 1
         self.selector_operator = "Tournament"
 
     def select(self, pops):
         pass
@@ -74,19 +74,19 @@
         Initialize the Selector
         :param exafs_pars:
         :return:
         """
         self.exafs_pars = exafs_pars
         self.selector_type = exafs_pars.selPars.selOpt
         if self.selector_type == 0:
-            self.selector_operator = ExafsSelector_RouletteWheel(exafs_pars, logger=self.logger)
+            self.selector_operator = NeoSelector_RouletteWheel(exafs_pars, logger=self.logger)
         elif self.selector_type == 1:
-            self.selector_operator = ExafsSelector_Tournament(exafs_pars, logger=self.logger)
+            self.selector_operator = NeoSelector_Tournament(exafs_pars, logger=self.logger)
         else:
-            self.selector_operator = ExafsSelectorBase(exafs_pars, logger=self.logger)
+            self.selector_operator = NeoSelectorBase(exafs_pars, logger=self.logger)
             raise ValueError("Invalid selector type, returning standard selector type.")
 
     def select(self, pops):
         """
         Perform the actual selection
         :param NeoPopulation pops:  
         :return:
```

### Comparing `exafs_neo-2.0.4/exafs_neo/parser.py` & `exafs_neo-2.0.5/exafs_neo/parser.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/pathObj.py` & `exafs_neo-2.0.5/exafs_neo/pathObj.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/pathrange.py` & `exafs_neo-2.0.5/exafs_neo/pathrange.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/pathrange_file.py` & `exafs_neo-2.0.5/exafs_neo/pathrange_file.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo/utils.py` & `exafs_neo-2.0.5/exafs_neo/utils.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/exafs_neo.egg-info/PKG-INFO` & `exafs_neo-2.0.5/exafs_neo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 Metadata-Version: 2.1
-Name: exafs_neo
-Version: 2.0.4
+Name: exafs-neo
+Version: 2.0.5
 Summary: exafs_neo AI analysis using GA
 Home-page: https://github.com/laumiulun/EXAFS_Neo
 Download-URL: https://github.com/laumiulun/EXAFS_Neo/tarball/master
 Author: Miu Lun Lau, Jeff Terry, Min Long
 Author-email: andylau@u.boisestate.edu, jterry98@iit.edu, minlong@boisestate.edu
 License: GPLv3
 Keywords: exafs_neo,AI,analysis
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: xraylarch
-Requires-Dist: attrs
-Requires-Dist: matplotlib
-Requires-Dist: psutil
 
 # EXAFS Neo
 
-#### Versions: 2.0.4
+#### Versions: 2.0.5
 
-#### Last update: Apr 20, 2024
+#### Last update: Apr 24, 2024
 
 <!-- ![example workflow](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/<WORKFLOW_FILE>/badge.svg) -->
 
 [![Test with Ubuntu, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml)[![Test with Windows, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml)
 
 
 EXAFS Neo utilize Genetic algorithm in fitting Extended X-ray absorption fine structure(EXAFS).
```

### Comparing `exafs_neo-2.0.4/exafs_neo.egg-info/SOURCES.txt` & `exafs_neo-2.0.5/exafs_neo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 exafs_neo/input_arg.py
 exafs_neo/neoCrossOver.py
 exafs_neo/neoFilePars.py
 exafs_neo/neoMutator.py
 exafs_neo/neoPars.py
 exafs_neo/neoResult.py
 exafs_neo/neoSelector.py
+exafs_neo/neoSolver.py
 exafs_neo/parser.py
 exafs_neo/pathObj.py
 exafs_neo/pathrange.py
 exafs_neo/pathrange_file.py
 exafs_neo/utils.py
 exafs_neo.egg-info/PKG-INFO
 exafs_neo.egg-info/SOURCES.txt
@@ -51,8 +52,9 @@
 tests/test_exafs_pathrange.py
 tests/test_individual.py
 tests/test_ini_parser.py
 tests/test_larchscore.py
 tests/test_neo_pop.py
 tests/test_neocrossover.py
 tests/test_neomutator.py
+tests/test_neosolver.py
 tests/test_utils.py
```

### Comparing `exafs_neo-2.0.4/setup.py` & `exafs_neo-2.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/tests/test_EXAFS_analysis.py` & `exafs_neo-2.0.5/tests/test_EXAFS_analysis.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/tests/test_exafs_fileobj.py` & `exafs_neo-2.0.5/tests/test_exafs_fileobj.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/tests/test_exafs_pars.py` & `exafs_neo-2.0.5/tests/test_exafs_pars.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/tests/test_exafs_pathObj.py` & `exafs_neo-2.0.5/tests/test_exafs_pathObj.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/tests/test_exafs_pathrange.py` & `exafs_neo-2.0.5/tests/test_exafs_pathrange.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/tests/test_individual.py` & `exafs_neo-2.0.5/tests/test_individual.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/tests/test_ini_parser.py` & `exafs_neo-2.0.5/tests/test_ini_parser.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/tests/test_larchscore.py` & `exafs_neo-2.0.5/tests/test_larchscore.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/tests/test_neo_pop.py` & `exafs_neo-2.0.5/tests/test_neo_pop.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/tests/test_neocrossover.py` & `exafs_neo-2.0.5/tests/test_neocrossover.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.4/tests/test_neomutator.py` & `exafs_neo-2.0.5/tests/test_neomutator.py`

 * *Files identical despite different names*


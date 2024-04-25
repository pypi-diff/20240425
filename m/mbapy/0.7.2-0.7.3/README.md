# Comparing `tmp/mbapy-0.7.2.tar.gz` & `tmp/mbapy-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbapy-0.7.2.tar", last modified: Sun Apr 21 13:12:32 2024, max compression
+gzip compressed data, was "mbapy-0.7.3.tar", last modified: Thu Apr 25 15:18:07 2024, max compression
```

## Comparing `mbapy-0.7.2.tar` & `mbapy-0.7.3.tar`

### file list

```diff
@@ -1,104 +1,109 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.198437 mbapy-0.7.2/
--rw-rw-rw-   0        0        0     1085 2023-09-30 06:15:47.000000 mbapy-0.7.2/LICENSE
--rw-rw-rw-   0        0        0      214 2024-04-21 10:41:48.000000 mbapy-0.7.2/MANIFEST.in
--rw-rw-rw-   0        0        0     7500 2024-04-21 13:12:32.197438 mbapy-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     5549 2024-04-04 11:37:22.000000 mbapy-0.7.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.059190 mbapy-0.7.2/mbapy/
--rw-rw-rw-   0        0        0     1203 2024-01-04 08:03:01.000000 mbapy-0.7.2/mbapy/__init__.py
--rw-rw-rw-   0        0        0      402 2024-04-21 13:06:56.000000 mbapy-0.7.2/mbapy/__version__.py
--rw-rw-rw-   0        0        0    26515 2024-03-01 02:09:58.000000 mbapy-0.7.2/mbapy/base.py
-drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.075514 mbapy-0.7.2/mbapy/bio/
--rw-rw-rw-   0        0        0      133 2024-01-08 14:19:44.000000 mbapy-0.7.2/mbapy/bio/__init__.py
--rw-rw-rw-   0        0        0    21232 2024-03-12 14:00:39.000000 mbapy-0.7.2/mbapy/bio/peptide.py
-drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.088507 mbapy-0.7.2/mbapy/dl_torch/
--rw-rw-rw-   0        0        0      361 2024-01-11 01:58:53.000000 mbapy-0.7.2/mbapy/dl_torch/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.090507 mbapy-0.7.2/mbapy/dl_torch/arch/
-drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.094686 mbapy-0.7.2/mbapy/dl_torch/arch/CL/
--rw-rw-rw-   0        0        0       34 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/arch/CL/__init__.py
--rw-rw-rw-   0        0        0    16559 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/arch/CL/builder.py
--rw-rw-rw-   0        0        0     2423 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/arch/CL/trainer.py
-drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.098682 mbapy-0.7.2/mbapy/dl_torch/arch/CLIP/
--rw-rw-rw-   0        0        0       32 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/arch/CLIP/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-10 08:31:51.000000 mbapy-0.7.2/mbapy/dl_torch/arch/CLIP/builder.py
--rw-rw-rw-   0        0        0        0 2023-07-10 08:31:51.000000 mbapy-0.7.2/mbapy/dl_torch/arch/CLIP/trainer.py
--rw-rw-rw-   0        0        0      203 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/arch/__init__.py
--rw-rw-rw-   0        0        0    26096 2024-01-05 08:43:17.000000 mbapy-0.7.2/mbapy/dl_torch/bb.py
--rw-rw-rw-   0        0        0     6352 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/data.py
--rw-rw-rw-   0        0        0     1063 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/hyper_search.py
--rw-rw-rw-   0        0        0     4113 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/loss.py
--rw-rw-rw-   0        0        0    13191 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/m.py
--rw-rw-rw-   0        0        0     4661 2023-12-11 09:26:16.000000 mbapy-0.7.2/mbapy/dl_torch/optim.py
-drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.101844 mbapy-0.7.2/mbapy/dl_torch/paper/
--rw-rw-rw-   0        0        0       18 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/paper/__init__.py
--rw-rw-rw-   0        0        0     2917 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/dl_torch/paper/bb.py
--rw-rw-rw-   0        0        0    17600 2024-01-11 07:34:28.000000 mbapy-0.7.2/mbapy/dl_torch/utils.py
--rw-rw-rw-   0        0        0    22088 2024-04-21 10:54:51.000000 mbapy-0.7.2/mbapy/file.py
-drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.105842 mbapy-0.7.2/mbapy/file_utils/
--rw-rw-rw-   0        0        0        0 2023-07-20 02:35:49.000000 mbapy-0.7.2/mbapy/file_utils/__init__.py
--rw-rw-rw-   0        0        0     7095 2023-12-18 14:29:23.000000 mbapy-0.7.2/mbapy/file_utils/image.py
--rw-rw-rw-   0        0        0    11531 2024-03-10 02:50:26.000000 mbapy-0.7.2/mbapy/file_utils/video.py
--rw-rw-rw-   0        0        0    25377 2024-02-23 13:27:31.000000 mbapy-0.7.2/mbapy/game.py
--rw-rw-rw-   0        0        0     3364 2023-12-18 14:29:23.000000 mbapy-0.7.2/mbapy/paper.py
--rw-rw-rw-   0        0        0    22809 2024-04-18 04:48:16.000000 mbapy-0.7.2/mbapy/plot.py
-drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.110839 mbapy-0.7.2/mbapy/sci_utils/
--rw-rw-rw-   0        0        0        0 2023-07-20 02:35:49.000000 mbapy-0.7.2/mbapy/sci_utils/__init__.py
--rw-rw-rw-   0        0        0    10594 2024-01-20 12:03:17.000000 mbapy-0.7.2/mbapy/sci_utils/paper_download.py
--rw-rw-rw-   0        0        0    23045 2023-12-11 09:26:16.000000 mbapy-0.7.2/mbapy/sci_utils/paper_parse.py
--rw-rw-rw-   0        0        0    16559 2024-01-20 12:03:17.000000 mbapy-0.7.2/mbapy/sci_utils/paper_search.py
-drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.147013 mbapy-0.7.2/mbapy/scripts/
--rw-rw-rw-   0        0        0      153 2024-01-08 13:31:52.000000 mbapy-0.7.2/mbapy/scripts/__init__.py
--rw-rw-rw-   0        0        0       68 2024-01-08 13:31:52.000000 mbapy-0.7.2/mbapy/scripts/__main__.py
--rw-rw-rw-   0        0        0     2821 2024-04-21 10:45:32.000000 mbapy-0.7.2/mbapy/scripts/_main_.py
--rw-rw-rw-   0        0        0      522 2024-04-10 06:02:44.000000 mbapy-0.7.2/mbapy/scripts/_script_utils_.py
--rw-rw-rw-   0        0        0     5549 2024-02-23 13:27:31.000000 mbapy-0.7.2/mbapy/scripts/avif.py
--rw-rw-rw-   0        0        0     1947 2024-01-22 08:25:16.000000 mbapy-0.7.2/mbapy/scripts/cluster.py
--rw-rw-rw-   0        0        0    13566 2024-01-08 13:31:52.000000 mbapy-0.7.2/mbapy/scripts/cnipa.py
--rw-rw-rw-   0        0        0     2741 2024-02-23 13:27:31.000000 mbapy-0.7.2/mbapy/scripts/cp.py
--rw-rw-rw-   0        0        0     4821 2024-02-23 13:27:31.000000 mbapy-0.7.2/mbapy/scripts/duitang.py
--rw-rw-rw-   0        0        0     2651 2024-02-23 13:27:31.000000 mbapy-0.7.2/mbapy/scripts/extract-dir.py
--rw-rw-rw-   0        0        0     2637 2024-01-08 13:31:52.000000 mbapy-0.7.2/mbapy/scripts/extract_paper.py
--rw-rw-rw-   0        0        0     3781 2024-04-15 15:02:22.000000 mbapy-0.7.2/mbapy/scripts/file-size.py
--rw-rw-rw-   0        0        0     9123 2024-04-21 10:31:57.000000 mbapy-0.7.2/mbapy/scripts/hplc.py
--rw-rw-rw-   0        0        0    14739 2024-04-21 13:10:16.000000 mbapy-0.7.2/mbapy/scripts/mass.py
--rw-rw-rw-   0        0        0     2614 2024-02-23 13:27:31.000000 mbapy-0.7.2/mbapy/scripts/mv.py
--rw-rw-rw-   0        0        0    26028 2024-04-10 09:30:41.000000 mbapy-0.7.2/mbapy/scripts/peptide.py
--rw-rw-rw-   0        0        0     1679 2024-01-12 08:11:59.000000 mbapy-0.7.2/mbapy/scripts/reviz.py
--rw-rw-rw-   0        0        0     2101 2024-02-23 13:27:31.000000 mbapy-0.7.2/mbapy/scripts/rm.py
--rw-rw-rw-   0        0        0     5392 2024-01-08 13:31:52.000000 mbapy-0.7.2/mbapy/scripts/scihub.py
--rw-rw-rw-   0        0        0     8636 2024-01-08 13:31:52.000000 mbapy-0.7.2/mbapy/scripts/scihub_selenium.py
--rw-rw-rw-   0        0        0     5633 2024-02-23 13:27:31.000000 mbapy-0.7.2/mbapy/scripts/splash_img.py
--rw-rw-rw-   0        0        0     9128 2024-03-14 08:21:47.000000 mbapy-0.7.2/mbapy/scripts/video.py
-drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.169338 mbapy-0.7.2/mbapy/stats/
--rw-rw-rw-   0        0        0     2839 2023-10-04 07:59:59.000000 mbapy-0.7.2/mbapy/stats/__init__.py
--rw-rw-rw-   0        0        0    30529 2023-10-06 03:00:11.000000 mbapy-0.7.2/mbapy/stats/cluster.py
--rw-rw-rw-   0        0        0    15779 2024-04-09 06:03:49.000000 mbapy-0.7.2/mbapy/stats/df.py
--rw-rw-rw-   0        0        0    19333 2023-09-30 06:15:47.000000 mbapy-0.7.2/mbapy/stats/geography.py
--rw-rw-rw-   0        0        0     3784 2024-04-02 03:46:14.000000 mbapy-0.7.2/mbapy/stats/reg.py
--rw-rw-rw-   0        0        0    16955 2024-04-05 10:19:56.000000 mbapy-0.7.2/mbapy/stats/test.py
-drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.183329 mbapy-0.7.2/mbapy/storage/
--rw-rw-rw-   0        0        0    69698 2024-01-11 01:58:53.000000 mbapy-0.7.2/mbapy/storage/libsci.dll
--rw-rw-rw-   0        0        0    15864 2024-01-11 01:58:53.000000 mbapy-0.7.2/mbapy/storage/libsci.so
--rw-rw-rw-   0        0        0    40252 2024-01-11 01:58:53.000000 mbapy-0.7.2/mbapy/storage/libstats.dll
--rw-rw-rw-   0        0        0    16752 2024-01-11 01:58:53.000000 mbapy-0.7.2/mbapy/storage/libstats.so
--rw-rw-rw-   0        0        0     3546 2024-04-21 10:41:06.000000 mbapy-0.7.2/mbapy/storage/mbapy-cli-scripts-list.json
--rw-rw-rw-   0        0        0     1565 2023-12-18 14:29:23.000000 mbapy-0.7.2/mbapy/web.py
-drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.191324 mbapy-0.7.2/mbapy/web_utils/
--rw-rw-rw-   0        0        0        0 2023-07-27 10:19:54.000000 mbapy-0.7.2/mbapy/web_utils/__init__.py
--rw-rw-rw-   0        0        0     4133 2023-11-06 08:06:25.000000 mbapy-0.7.2/mbapy/web_utils/parse.py
--rw-rw-rw-   0        0        0    35766 2024-02-23 13:27:31.000000 mbapy-0.7.2/mbapy/web_utils/request.py
--rw-rw-rw-   0        0        0    28907 2024-02-23 13:27:31.000000 mbapy-0.7.2/mbapy/web_utils/spider.py
--rw-rw-rw-   0        0        0    11644 2024-02-23 13:30:29.000000 mbapy-0.7.2/mbapy/web_utils/task.py
-drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.073607 mbapy-0.7.2/mbapy.egg-info/
--rw-rw-rw-   0        0        0     7500 2024-04-21 13:12:31.000000 mbapy-0.7.2/mbapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2107 2024-04-21 13:12:31.000000 mbapy-0.7.2/mbapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 13:12:31.000000 mbapy-0.7.2/mbapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-21 13:12:31.000000 mbapy-0.7.2/mbapy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      961 2024-04-21 13:12:31.000000 mbapy-0.7.2/mbapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-21 13:12:31.000000 mbapy-0.7.2/mbapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      899 2024-04-09 04:33:27.000000 mbapy-0.7.2/requirements.json
--rw-rw-rw-   0        0        0       42 2024-04-21 13:12:32.198437 mbapy-0.7.2/setup.cfg
--rw-rw-rw-   0        0        0     3400 2024-04-21 13:07:12.000000 mbapy-0.7.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 13:12:32.196439 mbapy-0.7.2/test/
--rw-rw-rw-   0        0        0     2028 2024-01-11 01:58:53.000000 mbapy-0.7.2/test/test_base.py
--rw-rw-rw-   0        0        0     1575 2023-10-20 09:14:56.000000 mbapy-0.7.2/test/test_game.py
--rw-rw-rw-   0        0        0     1742 2024-01-11 01:58:53.000000 mbapy-0.7.2/test/test_web.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.150521 mbapy-0.7.3/
+-rw-rw-rw-   0        0        0     1085 2023-09-30 06:15:47.000000 mbapy-0.7.3/LICENSE
+-rw-rw-rw-   0        0        0      214 2024-04-21 10:41:48.000000 mbapy-0.7.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     7500 2024-04-25 15:18:07.149519 mbapy-0.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5549 2024-04-04 11:37:22.000000 mbapy-0.7.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 15:18:06.993658 mbapy-0.7.3/mbapy/
+-rw-rw-rw-   0        0        0     1203 2024-01-04 08:03:01.000000 mbapy-0.7.3/mbapy/__init__.py
+-rw-rw-rw-   0        0        0      402 2024-04-25 15:17:56.000000 mbapy-0.7.3/mbapy/__version__.py
+-rw-rw-rw-   0        0        0    27309 2024-04-25 14:59:13.000000 mbapy-0.7.3/mbapy/base.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.031911 mbapy-0.7.3/mbapy/bio/
+-rw-rw-rw-   0        0        0      133 2024-01-08 14:19:44.000000 mbapy-0.7.3/mbapy/bio/__init__.py
+-rw-rw-rw-   0        0        0    21232 2024-03-12 14:00:39.000000 mbapy-0.7.3/mbapy/bio/peptide.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.044903 mbapy-0.7.3/mbapy/dl_torch/
+-rw-rw-rw-   0        0        0      361 2024-01-11 01:58:53.000000 mbapy-0.7.3/mbapy/dl_torch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.045902 mbapy-0.7.3/mbapy/dl_torch/arch/
+drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.049999 mbapy-0.7.3/mbapy/dl_torch/arch/CL/
+-rw-rw-rw-   0        0        0       34 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/arch/CL/__init__.py
+-rw-rw-rw-   0        0        0    16559 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/arch/CL/builder.py
+-rw-rw-rw-   0        0        0     2423 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/arch/CL/trainer.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.055026 mbapy-0.7.3/mbapy/dl_torch/arch/CLIP/
+-rw-rw-rw-   0        0        0       32 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/arch/CLIP/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-10 08:31:51.000000 mbapy-0.7.3/mbapy/dl_torch/arch/CLIP/builder.py
+-rw-rw-rw-   0        0        0        0 2023-07-10 08:31:51.000000 mbapy-0.7.3/mbapy/dl_torch/arch/CLIP/trainer.py
+-rw-rw-rw-   0        0        0      203 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/arch/__init__.py
+-rw-rw-rw-   0        0        0    26096 2024-01-05 08:43:17.000000 mbapy-0.7.3/mbapy/dl_torch/bb.py
+-rw-rw-rw-   0        0        0     6352 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/data.py
+-rw-rw-rw-   0        0        0     1063 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/hyper_search.py
+-rw-rw-rw-   0        0        0     4113 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/loss.py
+-rw-rw-rw-   0        0        0    13191 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/m.py
+-rw-rw-rw-   0        0        0     4661 2023-12-11 09:26:16.000000 mbapy-0.7.3/mbapy/dl_torch/optim.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.057996 mbapy-0.7.3/mbapy/dl_torch/paper/
+-rw-rw-rw-   0        0        0       18 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/paper/__init__.py
+-rw-rw-rw-   0        0        0     2917 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/dl_torch/paper/bb.py
+-rw-rw-rw-   0        0        0    17600 2024-01-11 07:34:28.000000 mbapy-0.7.3/mbapy/dl_torch/utils.py
+-rw-rw-rw-   0        0        0    22088 2024-04-21 10:54:51.000000 mbapy-0.7.3/mbapy/file.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.062168 mbapy-0.7.3/mbapy/file_utils/
+-rw-rw-rw-   0        0        0        0 2023-07-20 02:35:49.000000 mbapy-0.7.3/mbapy/file_utils/__init__.py
+-rw-rw-rw-   0        0        0     7095 2023-12-18 14:29:23.000000 mbapy-0.7.3/mbapy/file_utils/image.py
+-rw-rw-rw-   0        0        0    11531 2024-03-10 02:50:26.000000 mbapy-0.7.3/mbapy/file_utils/video.py
+-rw-rw-rw-   0        0        0    25377 2024-02-23 13:27:31.000000 mbapy-0.7.3/mbapy/game.py
+-rw-rw-rw-   0        0        0     3364 2023-12-18 14:29:23.000000 mbapy-0.7.3/mbapy/paper.py
+-rw-rw-rw-   0        0        0    11093 2024-04-23 13:37:47.000000 mbapy-0.7.3/mbapy/plot.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.074159 mbapy-0.7.3/mbapy/plot_utils/
+-rw-rw-rw-   0        0        0        0 2024-04-21 13:25:30.000000 mbapy-0.7.3/mbapy/plot_utils/__init__.py
+-rw-rw-rw-   0        0        0    15028 2024-04-24 01:25:33.000000 mbapy-0.7.3/mbapy/plot_utils/bar_utils.py
+-rw-rw-rw-   0        0        0        0 2024-04-21 13:26:21.000000 mbapy-0.7.3/mbapy/plot_utils/line_utils.py
+-rw-rw-rw-   0        0        0    11533 2024-04-23 03:04:53.000000 mbapy-0.7.3/mbapy/plot_utils/scatter_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.081195 mbapy-0.7.3/mbapy/sci_utils/
+-rw-rw-rw-   0        0        0        0 2023-07-20 02:35:49.000000 mbapy-0.7.3/mbapy/sci_utils/__init__.py
+-rw-rw-rw-   0        0        0    10594 2024-01-20 12:03:17.000000 mbapy-0.7.3/mbapy/sci_utils/paper_download.py
+-rw-rw-rw-   0        0        0    23045 2023-12-11 09:26:16.000000 mbapy-0.7.3/mbapy/sci_utils/paper_parse.py
+-rw-rw-rw-   0        0        0    16559 2024-04-25 15:14:19.000000 mbapy-0.7.3/mbapy/sci_utils/paper_search.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.116393 mbapy-0.7.3/mbapy/scripts/
+-rw-rw-rw-   0        0        0      153 2024-01-08 13:31:52.000000 mbapy-0.7.3/mbapy/scripts/__init__.py
+-rw-rw-rw-   0        0        0       68 2024-01-08 13:31:52.000000 mbapy-0.7.3/mbapy/scripts/__main__.py
+-rw-rw-rw-   0        0        0     2821 2024-04-21 10:45:32.000000 mbapy-0.7.3/mbapy/scripts/_main_.py
+-rw-rw-rw-   0        0        0      522 2024-04-10 06:02:44.000000 mbapy-0.7.3/mbapy/scripts/_script_utils_.py
+-rw-rw-rw-   0        0        0     5549 2024-02-23 13:27:31.000000 mbapy-0.7.3/mbapy/scripts/avif.py
+-rw-rw-rw-   0        0        0     1947 2024-01-22 08:25:16.000000 mbapy-0.7.3/mbapy/scripts/cluster.py
+-rw-rw-rw-   0        0        0    13566 2024-01-08 13:31:52.000000 mbapy-0.7.3/mbapy/scripts/cnipa.py
+-rw-rw-rw-   0        0        0     2741 2024-02-23 13:27:31.000000 mbapy-0.7.3/mbapy/scripts/cp.py
+-rw-rw-rw-   0        0        0     4806 2024-04-24 02:05:38.000000 mbapy-0.7.3/mbapy/scripts/duitang.py
+-rw-rw-rw-   0        0        0     2651 2024-02-23 13:27:31.000000 mbapy-0.7.3/mbapy/scripts/extract-dir.py
+-rw-rw-rw-   0        0        0     2637 2024-01-08 13:31:52.000000 mbapy-0.7.3/mbapy/scripts/extract_paper.py
+-rw-rw-rw-   0        0        0     3781 2024-04-15 15:02:22.000000 mbapy-0.7.3/mbapy/scripts/file-size.py
+-rw-rw-rw-   0        0        0     9141 2024-04-23 02:49:34.000000 mbapy-0.7.3/mbapy/scripts/hplc.py
+-rw-rw-rw-   0        0        0    14775 2024-04-23 02:48:49.000000 mbapy-0.7.3/mbapy/scripts/mass.py
+-rw-rw-rw-   0        0        0     2614 2024-02-23 13:27:31.000000 mbapy-0.7.3/mbapy/scripts/mv.py
+-rw-rw-rw-   0        0        0    26028 2024-04-10 09:30:41.000000 mbapy-0.7.3/mbapy/scripts/peptide.py
+-rw-rw-rw-   0        0        0     1679 2024-01-12 08:11:59.000000 mbapy-0.7.3/mbapy/scripts/reviz.py
+-rw-rw-rw-   0        0        0     2101 2024-02-23 13:27:31.000000 mbapy-0.7.3/mbapy/scripts/rm.py
+-rw-rw-rw-   0        0        0     5392 2024-01-08 13:31:52.000000 mbapy-0.7.3/mbapy/scripts/scihub.py
+-rw-rw-rw-   0        0        0     8636 2024-01-08 13:31:52.000000 mbapy-0.7.3/mbapy/scripts/scihub_selenium.py
+-rw-rw-rw-   0        0        0     5633 2024-02-23 13:27:31.000000 mbapy-0.7.3/mbapy/scripts/splash_img.py
+-rw-rw-rw-   0        0        0     9128 2024-03-14 08:21:47.000000 mbapy-0.7.3/mbapy/scripts/video.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.125388 mbapy-0.7.3/mbapy/stats/
+-rw-rw-rw-   0        0        0     2839 2023-10-04 07:59:59.000000 mbapy-0.7.3/mbapy/stats/__init__.py
+-rw-rw-rw-   0        0        0    30529 2023-10-06 03:00:11.000000 mbapy-0.7.3/mbapy/stats/cluster.py
+-rw-rw-rw-   0        0        0    15779 2024-04-09 06:03:49.000000 mbapy-0.7.3/mbapy/stats/df.py
+-rw-rw-rw-   0        0        0    19333 2023-09-30 06:15:47.000000 mbapy-0.7.3/mbapy/stats/geography.py
+-rw-rw-rw-   0        0        0     4009 2024-04-23 02:29:03.000000 mbapy-0.7.3/mbapy/stats/reg.py
+-rw-rw-rw-   0        0        0    16955 2024-04-05 10:19:56.000000 mbapy-0.7.3/mbapy/stats/test.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.134394 mbapy-0.7.3/mbapy/storage/
+-rw-rw-rw-   0        0        0    69698 2024-01-11 01:58:53.000000 mbapy-0.7.3/mbapy/storage/libsci.dll
+-rw-rw-rw-   0        0        0    15864 2024-01-11 01:58:53.000000 mbapy-0.7.3/mbapy/storage/libsci.so
+-rw-rw-rw-   0        0        0    40252 2024-01-11 01:58:53.000000 mbapy-0.7.3/mbapy/storage/libstats.dll
+-rw-rw-rw-   0        0        0    16752 2024-01-11 01:58:53.000000 mbapy-0.7.3/mbapy/storage/libstats.so
+-rw-rw-rw-   0        0        0     3546 2024-04-21 10:41:06.000000 mbapy-0.7.3/mbapy/storage/mbapy-cli-scripts-list.json
+-rw-rw-rw-   0        0        0     1565 2023-12-18 14:29:23.000000 mbapy-0.7.3/mbapy/web.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.143379 mbapy-0.7.3/mbapy/web_utils/
+-rw-rw-rw-   0        0        0        0 2023-07-27 10:19:54.000000 mbapy-0.7.3/mbapy/web_utils/__init__.py
+-rw-rw-rw-   0        0        0     4133 2023-11-06 08:06:25.000000 mbapy-0.7.3/mbapy/web_utils/parse.py
+-rw-rw-rw-   0        0        0    35800 2024-04-25 03:11:33.000000 mbapy-0.7.3/mbapy/web_utils/request.py
+-rw-rw-rw-   0        0        0    31544 2024-04-25 01:49:36.000000 mbapy-0.7.3/mbapy/web_utils/spider.py
+-rw-rw-rw-   0        0        0    16389 2024-04-25 13:20:01.000000 mbapy-0.7.3/mbapy/web_utils/task.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.028787 mbapy-0.7.3/mbapy.egg-info/
+-rw-rw-rw-   0        0        0     7500 2024-04-25 15:18:06.000000 mbapy-0.7.3/mbapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2231 2024-04-25 15:18:06.000000 mbapy-0.7.3/mbapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 15:18:06.000000 mbapy-0.7.3/mbapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-25 15:18:06.000000 mbapy-0.7.3/mbapy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      961 2024-04-25 15:18:06.000000 mbapy-0.7.3/mbapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-25 15:18:06.000000 mbapy-0.7.3/mbapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      899 2024-04-09 04:33:27.000000 mbapy-0.7.3/requirements.json
+-rw-rw-rw-   0        0        0       42 2024-04-25 15:18:07.150521 mbapy-0.7.3/setup.cfg
+-rw-rw-rw-   0        0        0     3400 2024-04-25 15:18:02.000000 mbapy-0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:18:07.148385 mbapy-0.7.3/test/
+-rw-rw-rw-   0        0        0     2028 2024-01-11 01:58:53.000000 mbapy-0.7.3/test/test_base.py
+-rw-rw-rw-   0        0        0     1575 2023-10-20 09:14:56.000000 mbapy-0.7.3/test/test_game.py
+-rw-rw-rw-   0        0        0     1742 2024-01-11 01:58:53.000000 mbapy-0.7.3/test/test_web.py
```

### Comparing `mbapy-0.7.2/LICENSE` & `mbapy-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/PKG-INFO` & `mbapy-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbapy
-Version: 0.7.2
+Version: 0.7.3
 Summary: MyBA in Python
 Home-page: https://github.com/BHM-Bob/BA_PY
 Author: BHM-Bob G
 Author-email: bhmfly@foxmail.com
 License: MIT Licence
 Description: <!--
          * @Author: BHM-Bob 2262029386@qq.com
```

### Comparing `mbapy-0.7.2/README.md` & `mbapy-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/__init__.py` & `mbapy-0.7.3/mbapy/__init__.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/base.py` & `mbapy-0.7.3/mbapy/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2022-10-19 22:46:30
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2024-03-01 10:09:58
+LastEditTime: 2024-04-25 22:58:26
 Description: 
 '''
 import ctypes
 import inspect
 import json
 import math
 import os
@@ -352,50 +352,61 @@
     Args:
         *arg_checkers: Variable number of functions that check the validity of positional arguments.
         raise_err (bool): Flag indicating whether to raise a ValueError when an invalid argument is encountered. Defaults to True.
         **kwarg_checkers: Variable number of functions that check the validity of keyword arguments.
 
     Returns:
         A decorated function that performs argument validity checks before executing the original function.
+        
+    Notes:
+        - If all checkers get passed, the original function is executed.
+        - If any checker fails, the function returns None or raises a ValueError, depending on the value of `raise_err`.
 
     Example usage:
     >>> @check_arguments(path = check_parameters_path, head = check_parameters_len)
     >>> def my_function(path, len, head):
     >>>     # Function body
     >>>     pass
     """
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
-            # info string
             info_string = f"Parameter checker for {func.__code__.co_name} : Invalid value for argument "
+            def check_arg(checker, arg_name: str, arg_value):
+                if not checker(arg_value):
+                    if raise_err:
+                        raise ValueError(info_string+arg_name)
+                    else:
+                        return put_err(info_string+arg_name, False)
+                return True
+            # args_name will exclude *args and **kwargs with name of args and kwargs
+            args_name = list(func.__code__.co_varnames)[:func.__code__.co_argcount+
+                                                 func.__code__.co_kwonlyargcount]
             # check positional arguments
-            for i, arg_check in enumerate(arg_checkers):
+            for i, arg_checker in enumerate(arg_checkers):
                 if i < len(args):
-                    arg = args[i]
-                    if not arg_check(arg):
-                        arg_name = func.__code__.co_varnames[i]
-                        if raise_err:
-                            raise ValueError(info_string+arg_name)
-                        else:
-                            # directly return a none value, skip the err pop
-                            return put_err(info_string+arg_name, None)
+                    if not check_arg(arg_checker, args_name[i], args[i]):
+                        return None
             # check keyword arguments
             for arg_name, kwarg_checker in kwarg_checkers.items():
-                # pass the rigth arg name
-                if arg_name in func.__code__.co_varnames:
+                # if passed the rigth arg name
+                if arg_name in args_name:
                     # get the index of the argument
-                    idx = func.__code__.co_varnames.index(arg_name)
-                    # get the argument through the index if passed positionally
-                    arg = args[idx] if idx < len(args) else kwargs[arg_name]
-                    if not kwarg_checker(arg):
-                        if raise_err:
-                            raise ValueError(info_string+arg_name)
-                        else:
-                            return put_err(info_string+arg_name, None)
+                    idx = args_name.index(arg_name)
+                    # get arg value
+                    if idx < len(args):
+                        arg_value = args[idx]
+                    elif arg_name in kwargs:
+                        arg_value = kwargs[arg_name]
+                    elif func.__defaults__ and idx-len(args) < len(func.__defaults__):
+                        arg_value = func.__defaults__[idx-len(args)]
+                    else:
+                        raise TypeError(f'{func.__code__.co_name}() minssing required argument')
+                    if not check_arg(kwarg_checker, arg_name, arg_value):
+                        return None
             return func(*args, **kwargs)
         return wrapper
     return decorator
 
 def rand_choose_times(choices_range:Tuple[int, int] = (0,10), times:int = 100):
     """
     Generates a random sequence of integers within a given range and 
@@ -677,9 +688,15 @@
     'get_dll_path_for_sys',
     'CDLL',
     'run_cmd',    
 ]
 
 if __name__ == '__main__':
     # dev code
-    # set_default_kwargs
-    d = set_default_kwargs({'a':1}, discard_extra=True, eps = 0.5, min_samples = 3)
+    class Test:
+        @parameter_checker(b = lambda b: b in ['b', 'B'], raise_err=False)
+        def __init__(self, a, b: str = 'b', *args, **kwargs) -> None:
+            print(a, b)
+            
+    Test('A')
+    Test('A', 'A', e = 'E')
+    Test('A', 'B', 10)
```

### Comparing `mbapy-0.7.2/mbapy/bio/peptide.py` & `mbapy-0.7.3/mbapy/bio/peptide.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/dl_torch/arch/CL/builder.py` & `mbapy-0.7.3/mbapy/dl_torch/arch/CL/builder.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/dl_torch/arch/CL/trainer.py` & `mbapy-0.7.3/mbapy/dl_torch/arch/CL/trainer.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/dl_torch/bb.py` & `mbapy-0.7.3/mbapy/dl_torch/bb.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/dl_torch/data.py` & `mbapy-0.7.3/mbapy/dl_torch/data.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/dl_torch/hyper_search.py` & `mbapy-0.7.3/mbapy/dl_torch/hyper_search.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/dl_torch/loss.py` & `mbapy-0.7.3/mbapy/dl_torch/loss.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/dl_torch/m.py` & `mbapy-0.7.3/mbapy/dl_torch/m.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/dl_torch/optim.py` & `mbapy-0.7.3/mbapy/dl_torch/optim.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/dl_torch/paper/bb.py` & `mbapy-0.7.3/mbapy/dl_torch/paper/bb.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/dl_torch/utils.py` & `mbapy-0.7.3/mbapy/dl_torch/utils.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/file.py` & `mbapy-0.7.3/mbapy/file.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/file_utils/image.py` & `mbapy-0.7.3/mbapy/file_utils/image.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/file_utils/video.py` & `mbapy-0.7.3/mbapy/file_utils/video.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/game.py` & `mbapy-0.7.3/mbapy/game.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/paper.py` & `mbapy-0.7.3/mbapy/paper.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/plot.py` & `mbapy-0.7.3/mbapy/plot_utils/bar_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,69 +4,28 @@
 
 import matplotlib.patches as patches
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
 import numpy as np
 import pandas as pd
 import seaborn as sns
-import statsmodels.api as sm
 from mpl_toolkits import axisartist
 from mpl_toolkits.axes_grid1 import host_subplot
 
-import mbapy.stats.test as mst
-from mbapy.base import get_wanted_args
-from mbapy.stats.df import (get_df_data, pro_bar_data, pro_bar_data_R,
-                            sort_df_factors)
-from mbapy.stats.test import p_value_to_stars
-
-# plt.rcParams['font.sans-serif'] = ['SimHei'] #用来正常显示中文
-plt.rcParams["font.family"] = 'Times New Roman'
-plt.rcParams['axes.unicode_minus'] = False #用来正常显示负号
-colors = plt.rcParams['axes.prop_cycle'].by_key()['color']
-
-def rgb2hex(r, g, b):
-  return '#'+('{:02X}' * 3).format(r, g, b)
-def hex2rgb(hex:str):
-  return [int(hex[i:i+2], 16) for i in (1, 3, 5)]
-def rgbs2hexs(rgbs:List[Tuple[float]]):
-    """
-    Takes a list of RGB tuples and converts them to a list of hexadecimal color codes. 
-    Each RGB tuple must contain three floats between 0 and 1 representing the red, green, and blue 
-    components of the color. Returns a list of hexadecimal color codes as strings.
-    """
-    return list(map(lambda x : rgb2hex(*[int(x[i]*255) for i in range(3)]),
-                    rgbs))
-    
-def get_palette(n:int = 10, mode:Union[None, str] = None, return_n = True) -> List[str]:
-    """get a seq of hex colors    
-    Parameters
-    ----------
-    n: how many colors required
-    mode: kind of colors
-        - hls : [default] sns.color_palette('hls', n)
-        - green : sum 5 grenns
-        - pair : plt.get_cmap('tab20')
-        - None : plt.get_cmap('Set1') for n<=9 or plt.get_cmap('Set3') for n<= 12
-    """
-    assert n >= 1, 'n < 1'
-    ret = None
-    if mode == 'hls':
-        ret = rgbs2hexs(sns.color_palette('hls', n))
-    elif n <= 5 and mode == 'green':
-        ret = ['#80ab1c', '#405535', '#99b69b', '#92e4ce', '#72cb87'][0:n]
-    elif n <= 9:
-        ret = rgbs2hexs(plt.get_cmap('Set1').colors)
-    elif n <= 12:
-        ret = rgbs2hexs(plt.get_cmap('Set3').colors)
-    elif n <= 20 and mode == 'pair':
-        ret = rgbs2hexs(plt.get_cmap('tab20').colors)
-    if return_n and ret is not None:
-        ret = ret[:n]
-    return ret
-    
+if __name__ == '__main__':
+    # dev mode
+    from mbapy.base import get_wanted_args, get_default_for_None
+    from mbapy.stats.df import (get_df_data, pro_bar_data, pro_bar_data_R,
+                                sort_df_factors)
+else:
+    # release mode
+    from ..base import get_wanted_args, get_default_for_None
+    from ..stats.df import (get_df_data, pro_bar_data, pro_bar_data_R,
+                           sort_df_factors)
+
 class AxisLable():
     def __init__(self, name:str, hold_space:int = 1) -> None:
         self.name = name
         self.hold_space = hold_space
         self.father = None
         self.child = set()
         self._hash = id(self) # 固定hash值
@@ -137,65 +96,75 @@
     Stack bar plot with hue style
 
     Args:
         - factors (List[str]): A list of factors. [low_lever_factor, medium_lever_factor, ...] or just one.
         - tags (List[str]): A list of tags. [stack_low_y, stack_medium_y, ...] or just one.
         - df (pd.DataFrame): A pandas DataFrame. From `pro_bar_data` or `sort_df_factors`.
         - kwargs: Additional keyword arguments.
-            - fig = None
+            - figsize = (8, 6)
             - jitter = Flase, IF True, pass the original df, the func will call `pro_bar_data` internally.
             - jitter_kwargs = {'size': 10, 'alpha': 0.5, 'color': None}
             - width = 0.4
             - bar_space = 0.05
             - hue_space = 0.2
             - xrotations = [0]*len(factors)
             - colors = plt.rcParams['axes.prop_cycle'].by_key()['color']
-            - hatchs:['-', '+', 'x', '\\', '*', 'o', 'O', '.'],
+            - hatchs:None, could be [['-', '+', 'x', '\\'], ['*', 'o', 'O', '.']],
             - font_size:None,
             - labels:None,
+            - ylabel: None, default is the first tag, fontsize will be set same as TOP level's x-axis' fontsize.
             - offset = [None] + [(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors)-1)], x-axis offset
             - xticks_pad: [5 for _ in range(len(factors)+1)], x-axis label pad from x-axis
             - edgecolor:['white'] * len(tags),
             - linewidth: 0,
             - err: (str|np.array), if str, will use df[err] as yerr. if np.array, will use it directly. will multiply 1.96 to yerr.
-            - err_kwargs = {'capsize':5, 'capthick':2, 'elinewidth':2, 'fmt':' k', 'ecolor':'black'}
+            - err_kwargs = 
+                - 'capsize':5, # error bar cap size
+                - 'capthick':2, # error bar cap thickness
+                - 'elinewidth':2, # error bar line width
+                - 'fmt':' k', # error bar format. 'k' means black.
+                - 'ecolor':'black', # error bar color. support list of hex color.
 
     Returns:
         - np.array: An array of positions.
         - ax1: An axis object.
         - df: If `jitter` is True, return the processed df.
         
     Notes:
         - the `FIRST factor` will be the `LOWEST level x-axis`.
         - y-axis tick labels' fontsize will be set same as first level's x-axis tick labels' fontsize.
     """
     # process args
     if len(tags) == 0:
         # TODO: 可能存在'Unbond: 0'等其他情况
         tags = list(df.columns)[len(factors):]
-    args = get_wanted_args({'fig': None,
+    args = get_wanted_args({'figsize': (8, 6),
+                            'dpi': 100,
                             'jitter':False,
                             'jitter_kwargs': {'size': 10, 'alpha': 0.5, 'color': None},
                             'width':0.4, 'hue_space':0.2, 'bar_space':0.05,
                             'xrotations':[0]*len(factors),
                             'colors':plt.rcParams['axes.prop_cycle'].by_key()['color'],
-                            'hatchs':['-', '+', 'x', '\\', '*', 'o', 'O', '.'],
+                            'hatchs': None,
                             'font_size':None,
                             'labels':None,
+                            'ylabel': None,
                             'offset':[None] + [(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors))],
                             'xticks_pad':[5 for _ in range(len(factors)+1)],
                             'edgecolor':['white'] * len(tags),
                             'linewidth': 0,
                             'log': False,
                             'err':None,
                             'err_kwargs':{'capsize':5, 'capthick':2, 'elinewidth':2, 'fmt':' k', 'ecolor':'black'}},
                             kwargs)
     args.xrotations.append(0)
     # make first level axis
-    ax1 = host_subplot(111, axes_class=axisartist.Axes, figure=args.fig)
+    ax1 = host_subplot(111, axes_class=axisartist.Axes)
+    ax1.figure.set_size_inches(args.figsize)
+    ax1.figure.set_dpi(args.dpi)
     # plot jitter using seaborn
     if args.jitter:
         jittor_color = args.jitter_kwargs['color']
         del args.jitter_kwargs['color']
         @pro_bar_data_R(factors[::-1], tags, df, ['', '_SE', '_N', '_V'])
         def pro_bar_jitter_data(v):
             if v.shape[0] > 1:
@@ -215,38 +184,40 @@
         if args.jitter:
             for i, (n, y) in enumerate(zip(df[yName+'_N'], df[yName+'_V'])):
                 x = [pos[0][i]] * n
                 color = jittor_color[yIdx][i] if jittor_color is not None else 'black'
                 sns.stripplot(x=x, y=y.reshape(-1), ax=ax1, jitter=True, native_scale=True,
                               color=color, zorder = 1, legend = False, **args.jitter_kwargs)
         # plot bar
+        hatch = args.hatchs[yIdx] if (args.hatchs and args.hatchs[yIdx] is not None) else None
         ax1.bar(pos[0], df[yName], width = args.width, bottom = bottom, label=label,
-                edgecolor=args.edgecolor[yIdx], linewidth = args.linewidth,
+                edgecolor=args.edgecolor[yIdx], linewidth = args.linewidth, hatch = hatch,
                 color=args.colors[yIdx], log = args.log, zorder = 0)
         bottom += df[yName]
     ax1.set_xlim(0, pos[0][-1]+args.hue_space+args.width/2)
     ax1.set_xticks(pos[0], [l.name for l in xlabels[0]])
     plt.setp(ax1.axis["bottom"].major_ticklabels, rotation=args.xrotations[0], pad = args.xticks_pad[0])
     if args.font_size is not None:
         plt.setp(ax1.axis["bottom"].major_ticklabels, fontsize=args.font_size[0])
         plt.setp(ax1.axis["left"].major_ticklabels, fontsize=args.font_size[0])
+        ax1.axis['left'].set_label(get_default_for_None(args.ylabel, tags[0]))
+        ax1.axis['left'].label.set_fontsize(args.font_size[-1])
     
     axs = []
     for idx, sub_pos in enumerate(pos[1:]):
         axs.append(ax1.twiny())
         axs[-1].set_xticks(sub_pos, [l.name for l in xlabels[idx+1]])
         new_axisline = axs[-1].get_grid_helper().new_fixed_axis
         axs[-1].axis["bottom"] = new_axisline(loc="bottom", axes=axs[-1], offset=(0, -args.offset[idx+1]))
         plt.setp(axs[-1].axis["bottom"].major_ticklabels, rotation=args.xrotations[idx+1], pad = args.xticks_pad[idx+1])
         if args.font_size is not None:
             plt.setp(axs[-1].axis["bottom"].major_ticklabels, fontsize=args.font_size[idx+1])
         axs[-1].axis["top"].major_ticks.set_ticksize(0)
         # TODO : do not work
         axs[-1].axis["right"].major_ticks.set_ticksize(0)
-        
     # err bar, put here because errorbar will change ax obj and occur errs
     if args.err is not None:
         if isinstance(args.err, str):
             args.err = df[args.err]
         if 'ecolor' in args.err_kwargs and isinstance(args.err_kwargs['ecolor'], list):
             err_cols = args.err_kwargs['ecolor']
             del args.err_kwargs['ecolor']
@@ -300,169 +271,30 @@
                 axs[-1].axis["top"].major_ticks.set_ticksize(0)
                 # TODO : do not work
                 axs[-1].axis["right"].major_ticks.set_ticksize(0)            
             return np.array(pos[0]), ax1
         return core_wrapper
     return ret_wrapper
 
-def calcu_swarm_pos(x: float, y: np.ndarray, width: float, d: Optional[float] = None):
-    """
-   This function calculates the x-coordinates for the data points in a swarm plot.
-   The x-coordinates are calculated based on the given x-coordinate, y-coordinates,
-   and width of the swarm. If d is not None, it will be used as the distance between
-   the data points. Otherwise, it will be calculated based on the number of data points.
-   
-    Parameters:
-        - x: the x-coordinate of the center of the swarm.
-        - y: the y-coordinates of the data points.
-        - width: the width of the swarm.
-        - d: the distance between the data points. If None, it will be calculated based on the number of data points.
-        
-    Returns:
-        - A numpy array of x-coordinates for the data points.
-    """
-    def _calcu_arithmetic(x, n, w, d):
-        if isinstance(d, float) or isinstance(d, int):
-            a0 = x - (n-1)*d/2
-            return np.linspace(a0, a0+d*(n-1), n)
-        if n == 1:
-            return x
-        else:
-            a0, d = x-w/2, w/(n-1)
-            return np.linspace(a0, a0+d*(n-1), n)
-    ret = np.zeros(len(y))
-    for y_u in np.unique(y):
-        y_idx = np.where(y == y_u)[0]
-        ret[y_idx] = _calcu_arithmetic(x, len(y_idx), width, d)
-    return ret
-
-def qqplot(tags:List[str], df:pd.DataFrame, figsize = (12, 6), nrows = 1, ncols = 1, **kwargs):
-    """
-    Generate a QQ-plot for each column in the given DataFrame.
-
-    Parameters:
-        tags (List[str]): A list of column names to generate QQ-plots for.
-        df (pd.DataFrame): The DataFrame containing the data.
-        figsize (tuple, optional): The size of the figure. Defaults to (12, 6).
-        nrows (int, optional): The number of rows in the figure grid. Defaults to 1.
-        ncols (int, optional): The number of columns in the figure grid. Defaults to 1.
-        **kwargs: Additional keyword arguments including xlim, ylim, title, tick_size, and label_size.
-
-    Returns:
-        None
-    """
-    axs = []
-    fig = plt.figure(figsize = (12, 6))
-    for fig_idx in range(1, ncols*nrows+1):
-        axs.append(fig.add_subplot(nrows, ncols, fig_idx))
-        if 'xlim' in kwargs:
-            axs[-1].set_xlim(kwargs['xlim'])
-        if 'ylim' in kwargs:
-            axs[-1].set_ylim(kwargs['ylim'])            
-        sm.qqplot(np.array(df[tags[fig_idx-1]]), fit=True, line="45", ax=axs[-1])
-        axs[-1].set_title(tags[fig_idx-1]+' - QQPlot', fontdict={'fontsize':15})
-        if 'title' in kwargs:
-            axs[-1].set_ylim(kwargs['title'][fig_idx-1])
-        if 'tick_size' in kwargs:
-            axs[-1].tick_params(labelsize = kwargs['tick_size'])
-        if 'label_size' in kwargs:
-            axs[-1].set_xlabel('Theoretical Quantiles', fontsize = kwargs['label_size'])
-            axs[-1].set_ylabel('Sample Quantiles', fontsize = kwargs['label_size'])
-    return axs
-            
-def save_show(path:str, dpi = 300, bbox_inches = 'tight'):
-    """
-    Saves the current matplotlib figure to a file at the specified path and displays the figure.
-
-    Parameters:
-        path (str): The path where the figure will be saved.
-        dpi (int, optional): The resolution of the saved figure in dots per inch. Default is 300.
-        bbox_inches (str or Bbox, optional): The portion of the figure to save. Default is 'tight'.
 
-    Returns:
-        None
-    """
-    plt.tight_layout()
-    plt.gcf().savefig(path, dpi=dpi, bbox_inches = bbox_inches)
-    plt.show()
-    
-def plot_stats_star(x1: float, x2: float, h: float, endpoint: float, p_value: float,
-                    ax = plt, p2star: Callable[[float], str] = p_value_to_stars):
-    """
-    Params
-        - x1: The x-coordinate of the left endpoint.
-        - x2: The x-coordinate of the right endpoint.
-        - h: The y-coordinate of the horizontal line.
-        - endpoint: The height of the endpoint.
-        - p_value: The p-value of the difference.
-        - ax: The `Axes` instance to plot on. Default is `plt`.
-        - p2star: A function that converts a p-value to a string of stars. Default is `p_value_to_stars`.
-
-    Returns:
-        None
-    """
-    ax.plot([x1, x2], [h, h], color='black')
-    ax.plot([x1, x1], [h, h-endpoint], color='black')
-    ax.plot([x2, x2], [h, h-endpoint], color='black')
-    ax.text((x1+x2)/2, h, p2star(p_value), ha='center')    
-    
-def plot_turkey(means, std_errs, tukey_results, min_star = 1):
-    """
-    Plot a bar chart showing the means of different groups along with the standard errors.
+__all__ = [
+    'AxisLabel'
+    'pro_hue_pos',
+    'plot_bar'
+    'plot_positional_hue',
+    ]
 
-    Parameters:
-        - means: A list of mean values for each group.
-        - std_errs: A list of standard errors for each group.
-        - tukey_results: The Tukey's test results object.
-
-    Returns:
-        The current `Axes` instance.
-
-    This function plots a bar chart using the given mean values and standard errors. It also marks the groups with significant differences based on the Tukey's test results.
-    For each combination of groups, the function checks if the corresponding Tukey's test result indicates a significant difference. If so, it plots a horizontal line at the maximum height, vertical lines at the endpoints, and places a text label with stars indicating the p-value of the difference.
-    """
-    x = np.arange(len(means))
-    plt.bar(x, means, yerr=std_errs, capsize=5)
-
-    combins = np.array(list(combinations(range(len(means)), 2)))
-    height = max(means) + max(std_errs)
-    min_height = 0.05 * height
-    endpoint_height = [height - 0.05 * min_height, height + 0.05 * min_height]
-    for i, combination in enumerate(combins):
-        if tukey_results.reject[i] \
-                and len(p_value_to_stars(tukey_results.pvalues[i])) >= min_star:
-            plt.plot(combination, [height, height], color='black')
-            plt.plot([combination[0], combination[0]], endpoint_height, color='black')
-            plt.plot([combination[1], combination[1]], endpoint_height, color='black')
-            plt.text(np.mean(combination), height,
-                     p_value_to_stars(tukey_results.pvalues[i]), ha='center')
-            height += min_height
-
-    plt.xticks(x, tukey_results.groupsunique)
-    return plt.gca()
 
 if __name__ == '__main__':
     # dev code
+    from mbapy.plot import get_palette
     df = pd.read_excel('./data/plot.xlsx', sheet_name='MWM')
-    df['Animal Type'] = df['Animal Type'].astype('str')
-    model = mst.multicomp_turkeyHSD({'Animal Type':[]}, 'Duration', df)
-    result = mst.turkey_to_table(model)
-    print(result)
-    # sub_df = get_df_data({'Animal Type':[]}, ['Duration'], df)
-    sub_df = pro_bar_data(['Animal Type'], ['Duration'], df)
-    # test err
     cols = get_palette(n = 4, mode = 'hls')
-    plot_bar(['Animal Type'], ['Duration'], df, err = sub_df['Duration_SE'], jitter = True,
-             edgecolor = [cols], linewidth = 5, colors = ['white'], jitter_kwargs = {'size': 10, 'alpha': 1, 'color': [cols]})
-    plt.show()
-    plot_turkey(sub_df['Duration'], sub_df['Duration_SE'], model)
-    plt.show()
-    
-    df = pd.DataFrame({'Month': [5, 5, 6, 6, 7, 7, 8, 8, 9, 9],
-                       'Ozone': [23.61538, 22.22445, 29.44444, 18.20790, 59.11538, 31.63584, 59.96154, 39.68121, 31.44828, 24.14182]})
-    model = mst.multicomp_turkeyHSD({'Month':[]}, 'Ozone', df)
-    result = mst.turkey_to_table(model)
-    print(result)
-    sub_df = pro_bar_data(['Month'], ['Ozone'], df)
-    plot_turkey(sub_df['Ozone'], sub_df['Ozone_SE'], model)
+    plot_bar(['Animal Type'], ['Duration'], df,
+             err = 'Duration_SE', err_kwargs = {'capsize':5, 'capthick':2, 'elinewidth':2, 'fmt':' k', 'ecolor':cols},
+             figsize = (8, 6),
+             edgecolor = [cols], linewidth = 5, colors = ['white'],
+             font_size = [10, 20],
+             jitter = True, jitter_kwargs = {'size': 10, 'alpha': 0.6, 'color': [cols]})
     plt.show()
+
```

### Comparing `mbapy-0.7.2/mbapy/sci_utils/paper_download.py` & `mbapy-0.7.3/mbapy/sci_utils/paper_download.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/sci_utils/paper_parse.py` & `mbapy-0.7.3/mbapy/sci_utils/paper_parse.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/sci_utils/paper_search.py` & `mbapy-0.7.3/mbapy/sci_utils/paper_search.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/scripts/_main_.py` & `mbapy-0.7.3/mbapy/scripts/_main_.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/scripts/_script_utils_.py` & `mbapy-0.7.3/mbapy/scripts/_script_utils_.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/scripts/avif.py` & `mbapy-0.7.3/mbapy/scripts/avif.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/scripts/cluster.py` & `mbapy-0.7.3/mbapy/scripts/cluster.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/scripts/cnipa.py` & `mbapy-0.7.3/mbapy/scripts/cnipa.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/scripts/cp.py` & `mbapy-0.7.3/mbapy/scripts/cp.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/scripts/duitang.py` & `mbapy-0.7.3/mbapy/scripts/duitang.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 from tqdm import tqdm
 from selenium.webdriver.common.keys import Keys
 
 if __name__ == '__main__':
     from mbapy.base import put_err, Configs, get_fmt_time
     from mbapy.file import read_json, save_json
     from mbapy.scripts._script_utils_ import clean_path, show_args
-    from mbapy.web import Browser, CoroutinePool, get_url_page_s, random_sleep
+    from mbapy.web import Browser, TaskPool, get_url_page_s, random_sleep
     from mbapy.web_utils.spider import retrieve_file_async
 else:
     from ..base import put_err, Configs, get_fmt_time
     from ..file import read_json, save_json
     from ._script_utils_ import clean_path, show_args
-    from ..web import Browser, CoroutinePool, get_url_page_s, random_sleep
+    from ..web import Browser, TaskPool, get_url_page_s, random_sleep
     from ..web_utils.spider import retrieve_file_async
     
 
 def main(sys_args: List[str] = None):
     args_paser = argparse.ArgumentParser(description = 'download images from duitang.com')
     args_paser.add_argument('-q', '--query', type=str,
                             help="search query string, warp with '' if contains space. Default is %(default)s.")
@@ -55,15 +55,15 @@
     # setup selenium
     # NOTE: use header to enable PC browser mode
     b_options = ['--no-sandbox', f"--user-agent={Configs.web.request_header}"]
     b = Browser(options=b_options + ([] if args.gui else ['--headless']),
                 use_undetected=args.undetected_chromedriver)
     
     # setup coroutine pool
-    pool = CoroutinePool().run()
+    pool = TaskPool().run()
     
     # get base page and search
     base_url = 'https://www.duitang.com/'
     b.get(base_url)
     b.send_key(key = args.query, element='//*[@id="kw"]')
     b.click(element='//*[@id="dt-search"]/form/button')
     b.click(element='/html/body/div[9]/div/div[1]/a', sleep_before=(10, 5))
```

### Comparing `mbapy-0.7.2/mbapy/scripts/extract-dir.py` & `mbapy-0.7.3/mbapy/scripts/extract-dir.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/scripts/extract_paper.py` & `mbapy-0.7.3/mbapy/scripts/extract_paper.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/scripts/file-size.py` & `mbapy-0.7.3/mbapy/scripts/file-size.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/scripts/hplc.py` & `mbapy-0.7.3/mbapy/scripts/hplc.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             xlim_max = max(xlim_max, data_df_i['Time'].max())
         xlim = [float(xlim[0]), xlim_max if xlim[1] == 'None' else float(xlim[1])]
     plt.xticks(size = 20)
     plt.yticks(size = 20)
     ax.set_xlabel('Time (min)', fontsize=25)
     ax.set_ylabel(f'Absorbance ({au_units})', fontsize=25)
     ax.set_xlim(xlim[0], xlim[1])
-    plt.legend(fontsize=15, loc = args.legend_pos, bbox_to_anchor = (args.legend_pos_bbox1, args.legend_pos_bbox2))
+    plt.legend(fontsize=15, loc = args.legend_pos, bbox_to_anchor = (args.legend_pos_bbox1, args.legend_pos_bbox2), draggable = True)
     save_show(os.path.join(args.output, f'{file_name} absorbance.png'), dpi = 600)
     
 def plot_hplc(args):           
     # process args
     args.input = clean_path(args.input)
     args.output = clean_path(args.output) if args.output else args.input
     if not os.path.isdir(args.output):
```

### Comparing `mbapy-0.7.2/mbapy/scripts/mass.py` & `mbapy-0.7.3/mbapy/scripts/mass.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     plt.yscale('log')
     axis_lim = (1-args.expand, 1+args.expand)
     plt.xlim(df['mass_data'].min() * axis_lim[0], df['mass_data'].max() * axis_lim[1])
     plt.ylim(df['Height'].min() * axis_lim[0], df['Height'].max() * axis_lim[1])
     ax.set_title(f'{name} (Peak List of TOF MS)', fontsize=25)
     ax.set_xlabel(f'Mass{"" if args.mass else "/charge"}', fontsize=25)
     ax.set_ylabel('Intensity (cps)', fontsize=25)
-    plt.legend(fontsize=15, loc = args.legend_pos, bbox_to_anchor = (args.legend_pos_bbox1, args.legend_pos_bbox2))
+    plt.legend(fontsize=15, loc = args.legend_pos, bbox_to_anchor = (args.legend_pos_bbox1, args.legend_pos_bbox2), draggable = True)
     save_show(os.path.join(args.output, f'{name} peak list.png'), dpi = 600)
     
 def plot_mass_plot_masscharge(name: str, df: pd.DataFrame, args):
     # find peaks
     peaks_cache_path = os.path.join(args.output, f'{name} peaks.cache.npy')
     if args.use_peaks_cache and os.path.exists(peaks_cache_path):
         peaks = np.load(peaks_cache_path)
@@ -141,15 +141,15 @@
     plt.yscale('log')
     axis_lim = (1-args.expand, 1+args.expand)
     plt.xlim(df['Mass/Charge'].min() * axis_lim[0], df['Mass/Charge'].max() * axis_lim[1])
     plt.ylim(df['Intensity'].min() * axis_lim[0], df['Intensity'].max() * axis_lim[1])
     ax.set_title(f'{name} (Mass/Charge of TOF MS)', fontsize=25)
     ax.set_xlabel(f'Mass/Charge', fontsize=25)
     ax.set_ylabel('Intensity (cps)', fontsize=25)
-    plt.legend(fontsize=15, loc = args.legend_pos, bbox_to_anchor = (args.legend_pos_bbox1, args.legend_pos_bbox2))
+    plt.legend(fontsize=15, loc = args.legend_pos, bbox_to_anchor = (args.legend_pos_bbox1, args.legend_pos_bbox2), draggable = True)
     save_show(os.path.join(args.output, f'{name} Mass-Charge.png'), dpi = 600)
     
 def plot_mass(args):           
     # process input and output args
     # after process, output whether be str or be None if recursive
     args.dir = clean_path(args.dir)
     if args.output is None:
```

### Comparing `mbapy-0.7.2/mbapy/scripts/mv.py` & `mbapy-0.7.3/mbapy/scripts/mv.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/scripts/peptide.py` & `mbapy-0.7.3/mbapy/scripts/peptide.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/scripts/reviz.py` & `mbapy-0.7.3/mbapy/scripts/reviz.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/scripts/rm.py` & `mbapy-0.7.3/mbapy/scripts/rm.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/scripts/scihub.py` & `mbapy-0.7.3/mbapy/scripts/scihub.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/scripts/scihub_selenium.py` & `mbapy-0.7.3/mbapy/scripts/scihub_selenium.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/scripts/splash_img.py` & `mbapy-0.7.3/mbapy/scripts/splash_img.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/scripts/video.py` & `mbapy-0.7.3/mbapy/scripts/video.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/stats/__init__.py` & `mbapy-0.7.3/mbapy/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/stats/cluster.py` & `mbapy-0.7.3/mbapy/stats/cluster.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/stats/df.py` & `mbapy-0.7.3/mbapy/stats/df.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/stats/geography.py` & `mbapy-0.7.3/mbapy/stats/geography.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/stats/reg.py` & `mbapy-0.7.3/mbapy/stats/reg.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2023-04-06 20:44:44
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2024-04-02 11:46:14
+LastEditTime: 2024-04-23 10:28:57
 Description: 
 '''
 from typing import Dict, List
 
 import numpy as np
 import pandas as pd
 import scipy
@@ -22,36 +22,38 @@
     from .cluster import KBayesian, KMeans, cluster, cluster_support_methods
 
 def linear_reg(x:str, y:str, df:pd.DataFrame):
     """
     Perform linear regression on the given DataFrame.
 
     Parameters:
-        x (str): The column name for the independent variable.
-        y (str): The column name for the dependent variable.
-        df (pd.DataFrame): The DataFrame containing the data.
+        - x (str): The column name for the independent variable.
+        - y (str): The column name for the dependent variable.
+        - df (pd.DataFrame): The DataFrame containing the data.
 
     Returns:
-        dict: A dictionary containing the regression model, slope, intercept, and R-squared value.
+        - dict: A dictionary containing the regression model, slope, intercept, and R-squared value.
             - 'regressor' (LinearRegression): The fitted regression model.
             - 'a' (float): The slope of the regression line.
             - 'b' (float): The intercept of the regression line.
             - 'r2' (float): The R-squared value of the regression.
     """
     x = np.array(df[x]).reshape(-1, 1)
     y = np.array(df[y]).reshape(-1, 1)
     regressor = LinearRegression()
     regressor = regressor.fit(x, y)
-    equation_a, equation_b = regressor.coef_.item(), regressor.intercept_.item()
-    equation_r2 = regressor.score(x, y)
+    a, b = regressor.coef_.item(), regressor.intercept_.item()
+    r2 = regressor.score(x, y)
     return {
         'regressor':regressor,
-        'a':equation_a,
-        'b':equation_b,
-        'r2':equation_r2,
+        'a':a,
+        'b':b,
+        'r2':r2,
+        'equation': f"y = {a:.2f}x {'+' if b>=0 else '-'} {abs(b):.2f}",
+        'r2_equation': f'R^2 = {r2:.2f}'
     }
     
 def quadratic_reg(x_str: str, y_str: str, df: pd.DataFrame):
     """
     Perform quadratic regression on the given DataFrame.
 
     Parameters:
@@ -92,13 +94,15 @@
     return {
         'regressor': regressor,
         'polynomial_features': poly_features,
         'a': a,
         'b': b,
         'c': c,
         'r2': r2,
+        'equation': f"y = {a:.2f}x^2 {'+' if b>=0 else '-'} {abs(b):.2f}x {'+' if c>=0 else '-'} {abs(c):.2f}",
+        'r2_equation': f'R^2 = {r2:.2f}'
     }
 
 
 if __name__ == '__main__':
     # dev code
     pass
```

### Comparing `mbapy-0.7.2/mbapy/stats/test.py` & `mbapy-0.7.3/mbapy/stats/test.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/storage/libsci.dll` & `mbapy-0.7.3/mbapy/storage/libsci.dll`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/storage/libsci.so` & `mbapy-0.7.3/mbapy/storage/libsci.so`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/storage/libstats.dll` & `mbapy-0.7.3/mbapy/storage/libstats.dll`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/storage/libstats.so` & `mbapy-0.7.3/mbapy/storage/libstats.so`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/storage/mbapy-cli-scripts-list.json` & `mbapy-0.7.3/mbapy/storage/mbapy-cli-scripts-list.json`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/web.py` & `mbapy-0.7.3/mbapy/web.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/web_utils/parse.py` & `mbapy-0.7.3/mbapy/web_utils/parse.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/mbapy/web_utils/request.py` & `mbapy-0.7.3/mbapy/web_utils/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -533,15 +533,16 @@
         else:
             return by
         
     @BrowserActionWarpper
     def get(self, url: str,
             sleep_before: Union[None, int, float, Tuple[int, int]] = None,
             sleep_after: Union[None, int, float, Tuple[int, int]] = (10, 5)):
-        return self.browser.get(url)
+        self.browser.get(url)
+        return self.browser.page_source
     
     def find_elements(self, element: str, by: str = 'xpath'):
         by = self._get_by(by)
         return self.browser.find_elements(by, element)
         
     def execute_script(self, script: str, *args):
         return self.browser.execute_script(script, *args)
```

### Comparing `mbapy-0.7.2/mbapy/web_utils/spider.py` & `mbapy-0.7.3/mbapy/web_utils/spider.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 import aiohttp
 from bs4 import BeautifulSoup
 from lxml import etree
 from tqdm import tqdm
 
 
 if __name__ == '__main__':
-    from mbapy.base import Configs, put_err
+    from mbapy.base import Configs, put_err, get_default_for_None
     from mbapy.file import get_valid_file_path
     from mbapy.game import BaseInfo # NOTE, for record
-    from mbapy.web_utils.request import random_sleep
-    from mbapy.web_utils.task import CoroutinePool, TaskStatus, Key2Action, launch_sub_thread, statues_que_opts, statuesQue
+    from mbapy.web_utils.request import random_sleep, Browser, get_url_page_se
+    from mbapy.web_utils.task import TaskPool, TaskStatus, Key2Action, launch_sub_thread, statues_que_opts, statuesQue
 else:
-    from ..base import Configs, put_err
+    from ..base import Configs, put_err, get_default_for_None
     from ..file import get_valid_file_path
     from ..game import BaseInfo # NOTE, for record
-    from .request import random_sleep
-    from .task import CoroutinePool, TaskStatus, Key2Action, launch_sub_thread, statues_que_opts, statuesQue
+    from .request import random_sleep, Browser, get_url_page_se
+    from .task import TaskPool, TaskStatus, Key2Action, launch_sub_thread, statues_que_opts, statuesQue
     
     
 def install_headers(agent: str = None):
     opener = urllib.request.build_opener()
     agent = agent or 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/101.0.4951.67 Safari/537.36'
     opener.addheaders = [('User-agent', agent)]
     urllib.request.install_opener(opener)
@@ -42,15 +42,14 @@
         async with aiohttp.request('GET', url, headers=headers, timeout=timeout) as response:
             if response.status != 200:
                 return (TaskStatus.NOT_SUCCEED, f'Web error: {response.status}')
             return await response.text(encoding=encoding)
     except Exception as e:
         return (TaskStatus.NOT_SUCCEED, f'Error occurred: {e}')
 
-
 async def retrieve_file_async(url: str, file_path: str, headers: Dict[str, str] = None):
     """async version of download_file"""
     timeout = aiohttp.ClientTimeout(total=30, connect=9999)
     try:
         async with aiohttp.request('GET', url, headers=headers, timeout=timeout) as response:
             if response.status != 200:
                 return (TaskStatus.NOT_SUCCEED, f'Web error: {response.status}')
@@ -61,26 +60,26 @@
             return file_path
     except Exception as e:
         return (TaskStatus.NOT_SUCCEED, f'Error occurred: {e}')
 
 
 @dataclass
 class AsyncResult:
-    async_pool: CoroutinePool
+    task_pool: TaskPool
     name: str
     result: Any = TaskStatus.NOT_RETURNED
     def get(self):
         """block to get result"""
         # short cut to get result
         if self.result is not TaskStatus.NOT_RETURNED:
             return self.result
         # wait for result
-        self.result = self.async_pool.query_task(self.name)
+        self.result = self.task_pool.query_task(self.name)
         while self.result == TaskStatus.NOT_FINISHED:
-            self.result = self.async_pool.query_task(self.name)
+            self.result = self.task_pool.query_task(self.name)
             time.sleep(0.1)
         # will also return TaskStatus.NOT_SUCCEED
         return self.result
         
         
 def only_sleep(seconds: float = 1, rand = True, max: float = 5):
     """sleep for seconds, with random sleep up to max seconds, return True."""
@@ -120,15 +119,15 @@
                  findall_fn: Callable = None, ignore_records: bool = False,
                  *args, **kwargs):
         """page container, store each web-page and its parsed data."""
         super().__init__(*args, **kwargs)
         self.name: str = name # name of this page, could be empty
         self.xpath: Union[str, List[str]] = xpath # xpath expression to extract data, if it is a list, will treat as alternative xpath expressions.
         self.findall_fn: Callable = findall_fn # alternative function to extract data via bs4.find_all, if it is not None, will use it instead of xpath.
-        self._async_task_pool: CoroutinePool = None # async task pool to execute async tasks
+        self._task_pool: TaskPool = None # async task pool to execute async tasks
         self._headers: Dict[str, str] = {} # headers for web-page request
         # result generally is a list of result, top-level list is for each web-page, and it ONLY store one kind item.
         self.result: List[Any] = [] # parsed result
         self.result_page_html: List[str] = [] # web-page html of parsed result
         self.result_page_xpath: List[etree._Element] = [] # web-page xpath object of parsed result
         self.result_page_bs4: List[BeautifulSoup] = [] # web-page bs4 object of parsed result
         self.father_page: 'BasePage' = None # father page of this page
@@ -142,37 +141,44 @@
     def add_next_page(self, name:str, page: 'BasePage') -> None:
         if isinstance(name, str):
             self.next_pages[name] = page
             return True
         else:
             return put_err('name should be str, skip and return False', False)
         
-    def parse(self, results: List[List[Union[str, etree._Element]]] = None) -> None:
+    def parse(self, *args, results: List[List[Union[str, etree._Element]]] = None,
+              clear_history: bool = True, **kwargs) -> None:
         """
         parse data from results, override by subclass.
-        In BasePage.perform, it will call this function to parse data and store in self.result..
+        In BasePage.perform, it will call this function to parse data and store in self.result.
+        
+        Parameters:
+            - results: List[List[Union[str, etree._Element]]], results from previous pages, could be None.
+            - clear_history[SHOULD IMPLEMENT BY SUBCLASS]: bool, if clear_history is True, will clear history results before parsing, default is True.
         """
         
     def _process_parsed_data(self, *args, **kwargs):
         """
         process parsed data, could be override by subclass
         """
         
-    def perform(self, *args, results: List[List[Union[str, etree._Element]]] = None, **kwargs):
+    def perform(self, *args, results: List[List[Union[str, etree._Element]]] = None,
+                clear_history: bool = True, **kwargs) -> List[Any]:
         self.result =  self.parse(results)
         self._process_parsed_data(*args, **kwargs)
         return self.result
     
     
 class PagePage(BasePage):
     """
     Only START and store a new web page or a list of web pages.
     """
     def __init__(self, url: List[Union[str, List[str]]] = None, ignore_records: bool = False,
-                 web_get_fn: Callable[[Any], str] = None, *args, **kwargs) -> None:
+                 web_get_fn: Callable[[Any], str] = None, *args,
+                 each_delay: float = 0.5, max_each_delay: float = 1, **kwargs) -> None:
         """
         Parameters:
             - url: List[str | List[str]], url to get web page, could be empty if get from father_page.result.
             - ignore_records: bool, if ignore_records is True, will not record this url to avoid duplicate request.
             - web_get_fn: Callable[[Any], str], function to get web page, default is None(get_web_html_async).
                 Note: the function should accept url as first argument and return web page html.
             - args: any, args for web_get_fn
@@ -180,33 +186,36 @@
                 - each_delay: float, delay seconds between each request, default is 1.
         
         Note:
             - item of url could be str of list of str.
         """
         super().__init__(ignore_records=ignore_records)
         self.url = url
-        self.each_delay = kwargs.get('each_delay', 0.5)
-        self.max_each_delay = kwargs.get('max_each_delay', 1)
-        self.web_get_fn = web_get_fn
+        self.each_delay = each_delay
+        self.max_each_delay = max_each_delay
+        self.web_get_fn = web_get_fn # set in self.parse, default is get_web_html_async
         self.args = args
         self.kwargs = kwargs
         
     def _process_url(self, results: List[List[Union[str, etree._Element]]] = None):
         # Note: result always be list(page) for list(items)
         # get url from results or father_page.result_page_xpath
         if self.url is None:
             if results is None:
                 results = self.father_page.result
+        elif isinstance(self.url, str):
+            results = [[self.url]] # => list of list of urls
         elif isinstance(self.url, list) and len(self.url) > 0 and isinstance(self.url[0], str):
             results = [self.url] # => list of list of urls
         else:
             results = self.url
         return results
     
-    def parse(self, results: List[List[Union[str, etree._Element]]] = None):
+    def parse(self, results: List[List[Union[str, etree._Element]]] = None,
+              clear_history: bool = True, **kwargs):
         """
         get new web-page(s) from self.url, results(as links) or self.father_page.result_page_xpath(as links)
         Note: a page store one kind item, the content of this item could be url or list of urls.
         """
         results = self._process_url(results)
         # set web_get_fn and args, kwargs
         if self.web_get_fn is None:
@@ -219,16 +228,16 @@
             self.result_page_xpath.append([])
             for url in tqdm(page, leave=False, desc=f'{self.name} get Item'):
                 # listen to keybord input to stop
                 if self.use_thread_listen and statues_que_opts(statuesQue, '__is_quit__', 'getValue'):
                     return self.result
                 # qurey url and get web page
                 if url not in self._records or self.ignore_records:
-                    task_name = self._async_task_pool.add_task(None, self.web_get_fn, url, *self.args, **self.kwargs)
-                    self.result[-1].append(AsyncResult(self._async_task_pool, task_name))
+                    task_name = self._task_pool.add_task(None, self.web_get_fn, url, *self.args, **self.kwargs)
+                    self.result[-1].append(AsyncResult(self._task_pool, task_name))
                     self.result_page_html[-1].append(self.result[-1][-1])
                     # NOTE: do not append xpath object because html is async.
                     random_sleep(self.max_each_delay, self.each_delay)
                     self._records[url] = True # record this url to avoid duplicate request.
         return self.result
     
     
@@ -239,23 +248,30 @@
     
     Note:
         - url_fn should return '' if no more url to get.
         - This class also represents a page container, 
             so the result also be list(page) for list(items) for links(result).
         - ignore_records is True by default. Because the url is idx type.
     """
-    def __init__(self, base_url: str = '', url_fn: Callable[[str, int], str] = None,
+    def __init__(self, base_url: str, url_fn: Callable[[str, int], str],
                  ignore_records: bool = True,
                  web_get_fn: Callable[[Any], str] = None,
                  *args, **kwargs) -> None:
+        """
+        Parameters:
+            - base_url: str, base url to get page url.
+            - url_fn: Callable[[str, int], str], function to get page url, default is None.
+                Note: the function should accept base_url and idx as arguments and return page url.
+        """
         super().__init__([], ignore_records=ignore_records, web_get_fn=web_get_fn, *args, **kwargs)
         self.base_url = base_url
         self.url_fn = url_fn
         
-    def parse(self, results: List[List[Union[str, etree._Element]]]):
+    def parse(self, results: List[List[Union[str, etree._Element]]],
+              clear_history: bool = True, **kwargs):
         is_valid, idx = True, 0
         while is_valid:
             url = self.url_fn(self.base_url, idx)
             idx += 1
             if url == '' or url is None:
                 is_valid = False
             else:
@@ -280,15 +296,16 @@
         super().__init__(url, ignore_records=ignore_records, web_get_fn=web_get_fn, *args, **kwargs)
         self.folder = folder
         self.wait_all = wait_all
         self.skip_downloaded = skip_downloaded
         self.page_folder_name: List[str] = None # folder name of each page, could be empty
         self.item_file_name: List[List[str]] = None # file name of each item, could be empty
         
-    def parse(self, results: List[List[Union[str, etree._Element]]] = None):
+    def parse(self, results: List[List[Union[str, etree._Element]]] = None,
+              clear_history: bool = True, **kwargs):
         """
         download file from self.url, results(as links) or self.father_page.result_page_xpath(as links)
         Note: a page store one kind item, the content of this item could be url or list of urls.
         """
         results = self._process_url(results)
         # set web_get_fn and args, kwargs
         if self.web_get_fn is None:
@@ -319,28 +336,28 @@
                 if os.path.exists(file_path) and self.skip_downloaded:
                     self._records[url] = False
                     continue
                 # qurey if this url is already in records
                 if url in self._records and self.ignore_records:
                     continue
                 # create download task
-                task_name = self._async_task_pool.add_task(None, self.web_get_fn, url, file_path, *self.args, **self.kwargs)
-                self.result[-1].append(AsyncResult(self._async_task_pool, task_name))
+                task_name = self._task_pool.add_task(None, self.web_get_fn, url, file_path, *self.args, **self.kwargs)
+                self.result[-1].append(AsyncResult(self._task_pool, task_name))
                 self._records[url] = False # record this url to avoid duplicate request.
                 random_sleep(self.max_each_delay, self.each_delay)
         # wait all tasks finished
         if self.wait_all:
             sum_tasks = sum([len(i) for i in self.result])
             not_finished, last_not_finished = sum_tasks, sum_tasks
             with tqdm(total=sum_tasks, leave=False, desc=f'{self.name} wait all') as pbar:
                 while not_finished > 0:
                     not_finished = 0
                     for page in self.result:
                         for i in page:
-                            if self._async_task_pool.query_task(i.name) == TaskStatus.NOT_FINISHED:
+                            if self._task_pool.query_task(i.name) == TaskStatus.NOT_FINISHED:
                                 not_finished += 1
                     pbar.update(last_not_finished - not_finished)
                     last_not_finished = not_finished
                     time.sleep(0.1)
         return self.result
     
     
@@ -361,29 +378,31 @@
         if self.findall_fn is None and self.alternative_bs4:
             raise ValueError('findall_fn should not be None if alternative_bs4 is True')
         
     def parse_xpath(self, xpath_r: etree._Element):
         if isinstance(xpath_r, etree._Element):
             self.result_page_xpath[-1].append(xpath_r) # Only store xpath object, not html
             if isinstance(self.xpath, str):
-                xpath_r = xpath_r.xpath(self.xpath)
-                if xpath_r:
-                    self.result[-1].extend(xpath_r)
+                xpath_result = xpath_r.xpath(self.xpath)
+                if xpath_result:
+                    self.result[-1].extend(xpath_result)
                     return True
             elif isinstance(self.xpath, list) and len(self.xpath) >= 1:
                 xpath_result, xpath_idx = xpath_r.xpath(self.xpath[0]), 1
                 while not xpath_result and xpath_idx < len(self.xpath):
                     xpath_result = xpath_r.xpath(self.xpath[xpath_idx])
                     xpath_idx += 1
                 if xpath_result:
                     self.result[-1].extend(xpath_result)
                     return True
+            put_err(f'{self.name} ItemsPage parse_xpath failed, xpath_r: {xpath_r}, xpath: {self.xpath}')
         return False
         
-    def parse(self, results: List[List[Union[str, etree._Element]]] = None):
+    def parse(self, results: List[List[Union[str, etree._Element]]] = None,
+              clear_history: bool = True, **kwargs):
         """
         parse data from results, override by subclass.
         """
         if results is None:
             results = self.father_page.result
         # detect available result and transfer to xpath object
         for page in tqdm(results, leave=False, desc=f'{self.name} parse Page'): # page is a result container of one kind item
@@ -449,34 +468,37 @@
         - perform(*args, **kwargs) -> Dict:
             perform all pages to get results.
         - close() -> None:
             close async task pool.
     """
     def __init__(self, pages = {},
                  headers: str = {'User-Agent': Configs.web.request_header},
+                 browser: Browser = None,
+                 task_pool_mode: str = 'async',
                  use_thread_listen: bool = True,
-                 k2a: List[Tuple[str, Key2Action]] = [
-                     ('save', Key2Action('running', statues_que_opts, [statuesQue, "__signal__", "setValue", 'save'], {}))],
+                 k2a: List[Tuple[str, Key2Action]] = None,
                  from_json_path: str = None) -> None:
         """
         Parameters:
             - pages: a dict of pages, key is page name, value is page object.
             - headers: a dict of headers to send request.
             - use_thread_control: if True, use a single thread to listening keybord input and control to save.
             - k2a: a list of tuple, key is key to listen, value is action to perform.
-                - default key2action: 'e': exit single thread and set statuesQue's __is_quit__ to True.
+                - default key2action 1: 'e': exit single thread and set statuesQue's __is_quit__ to True.
+                - default key2action 2: 'save': set statuesQue's __signal__ to 'save'.
         """
         super().__init__()
         self.pages: Dict[str, BasePage] = pages
         self.results: Dict = None
+        self.browser = browser
         self.use_thread_listen = use_thread_listen
-        self.k2a = k2a
+        self.k2a = get_default_for_None(k2a, [('save', Key2Action('running', statues_que_opts, [statuesQue, "__signal__", "setValue", 'save'], {}))])
         self.json_path = from_json_path
         self._headers: str = headers
-        self._async_task_pool: CoroutinePool = CoroutinePool() # call run in perform() to start async task pool
+        self._task_pool: TaskPool = TaskPool(task_pool_mode) # call run in perform() to start async task pool
         # recover from json file if exists
         if self.json_path is not None and os.path.exists(self.json_path):
             self.from_json(self.json_path)
     
     @staticmethod
     def get_page(name: str, father_pages: Dict[str, BasePage] = None,
                  father_page: BasePage = None) -> BasePage:
@@ -529,30 +551,31 @@
         if father != '':
             father = self.get_page(father, self.pages)
         # add before_func and after_func
         page.before_func = before_func
         page.after_func = after_func
         # add page to pages
         page.name = name
-        page._async_task_pool = self._async_task_pool
+        page._task_pool = self._task_pool
         page._headers = self._headers
         page.use_thread_listen = self.use_thread_listen
         if father is None or father == '':
             self.pages[name] = page
         else:
             father.add_next_page(name, page)
             page.father_page = father
         return self
     
     def del_page(self, name: str) -> None:
         raise NotImplementedError()
     
-    def perform(self, *args, **kwargs):
+    def perform(self, *args, clear_history: bool = True, **kwargs):
         """
         Parameters:
+            - clear_history: if True, clear all history before perform.
             - args, kwargs: parameters to pass to each page's perform method.
             
         Returns:
             - results: a dict of all results, key is page name, value is page's result.
             
         Notes:
             - This method will start a single thread to listen keybord input and control to save.
@@ -561,31 +584,49 @@
             - if a page has next_pages, it will perform each next_page recursively.
         """
         def _perform(page: Dict[str, BasePage], results: Dict, *args, **kwargs):
             for n, p in page.items():
                 # check before_func
                 if p.before_func is None or p.before_func(self, p):
                     # perform this page to make it's own result
-                    result = p.perform(*args, **kwargs)
+                    result = p.perform(*args, clear_history=clear_history, **kwargs)
                     # execute after_func if exists
                     if p.after_func is not None:
                         p.after_func(self, p)
                     # perform each next_page recursively
                     if p.next_pages is not None and len(p.next_pages) > 0:
                         results[n] = {f'__{n}__': result}
                         results[n].update(_perform(p.next_pages, results[n], *args, **kwargs))
                     else: # or perform itself if no next_page
                         results[n] = result
             return results
         # prepare listner
         if self.use_thread_listen:
             launch_sub_thread(key2action=self.k2a)
         # prepare async task pool
-        self._async_task_pool.run()
+        self._task_pool.run()
         self.results = {}
         self.results = _perform(self.pages, self.results, *args, **kwargs)
         return self.results
     
     def close(self):
         """close async task pool"""
-        self._async_task_pool.close()
+        self._task_pool.close()
 
+
+if __name__ == '__main__':
+    b = Browser()
+    main_page = UrlIdxPagesPage(base_url='https://www.kuaidaili.com/free/inha/',
+                                url_fn=lambda url, i: f'{url}{i+1}' if i < 10 else '',
+                                web_get_fn=lambda url: b.get(url))
+    ip_items = ItemsPage("//*[@id='table__free-proxy']/div[1]/table[1]/tbody[1]//td[1]/text()")
+    port_items = ItemsPage("//*[@id='table__free-proxy']/div[1]/table[1]/tbody[1]//td[2]/text()")
+    timeout_items = ItemsPage("//*[@id='table__free-proxy']/div[1]/table[1]/tbody[1]//td[6]/text()")
+    verify_items = ItemsPage("//*[@id='table__free-proxy']/div[1]/table[1]/tbody[1]//td[7]/text()")
+    action = Actions(browser = b, task_pool_mode='thread')
+    action.add_page(main_page, '', 'main-page')
+    action.add_page(ip_items, 'main-page', 'ip')
+    action.add_page(port_items, 'main-page', 'port')
+    action.add_page(timeout_items, 'main-page', 'timeout')
+    action.add_page(verify_items, 'main-page', 'verify')
+    action.perform()
+    print(action.results)
```

### Comparing `mbapy-0.7.2/mbapy/web_utils/task.py` & `mbapy-0.7.3/mbapy/web_utils/task.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 import time
 import threading
 from collections import namedtuple
 from enum import Enum
 from queue import Queue
 from typing import Any, Callable, Dict, List, Tuple, Union
 
-from mbapy.base import put_err, put_log
+if __name__ == '__main__':
+    # dev mode
+    from mbapy.base import put_err, put_log, parameter_checker
+else:
+    from ..base import put_err, put_log, parameter_checker
 
 statuesQue = Queue()
 Key2Action = namedtuple('Key2Action', ['statue', 'func', 'args', 'kwgs',
                                        'is_reg', 'lock'],
                         defaults=[False, None])
 
 def _wait_for_quit(statuesQue, key2action: Dict[str, List[Key2Action]]):
@@ -94,15 +98,15 @@
 def launch_sub_thread(statuesQue = statuesQue,
                       key2action: List[Tuple[str, Key2Action]] = []):
     """
     Launches a sub-thread to run a separate task concurrently with the main thread.
     
     Note:
         - statuesQue has two keys for mbapy inner usage: __is_quit__ and __inputs__.
-        - key2action iwill add a ket 'e' first, and then add other key-to-action.
+        - key2action will add a key 'e' first, and then add other key-to-action.
             The 'e' key will trigle the 'exit' signal to _wait_for_quit func.
         - NOLY IF get no match without reg, then try to match with reg.
     
     Parameters:
         - statuesQue: ...
         - key2action(List[Tuple[str, Key2Action]]): key-to-action
             - key(str): keyboard inputs to trigle this action, such as 'save'.
@@ -212,103 +216,189 @@
                 return retList            
         for que in self.getDataQues:
             while not que.empty():
                 retList.append(que.get())
         return retList
     
 class TaskStatus(Enum):
+    SUCCEED = 0
     NOT_FOUND = 1
     NOT_FINISHED = 2
     NOT_SUCCEEDED = 3
     NOT_RETURNED = 4
 
-class CoroutinePool:
+class TaskPool:
     """
-    co-routine pool, use asyncio to run co-routines in a separate thread.
+    task pool, use asyncio to run co-routines in a separate thread OR just run normal tasks in a separate thread.
+    
+    Attributes:
+        - mode (str, default='async'): 'async' or 'thread', use asyncio or threading to run a pool.
+        - loop (asyncio.loop): asyncio event loop.
+        - thread (threading.Thread): threading thread.
+        - tasks (Dict[str, asyncio.Future]): task name to future.
+        - TASK_NOT_FOUND (TaskStatus): signal FLAG, task not found.
+        - TASK_NOT_FINISHED (TaskStatus): signal FLAG, task not finished.
+        - TASK_NOT_SUCCEEDED (TaskStatus): signal FLAG, task not succeeded.
+        
+    Methods:
     """
-    def __init__(self):
-        self.loop = None
-        self.thread = None
+    @parameter_checker(mode = lambda mode: mode in ['async', 'thread', 'threads'])
+    def __init__(self, mode: str = 'async', n_worker: int = None):
+        """
+        Parameters:
+            - mode (str, default='async'): 'async' or 'thread', use asyncio or threading to run a pool.
+                - If it's IO heavy and has suitable coroutine function, use 'async'
+                - If it's IO heavy and only has normal function, and wants run ONE task at ONCE, use 'thread'. Use Queue to cache tasks and run ONE task at ONCE.
+                - If it's IO heavy and only has normal function, and wants run MULTI tasks at ONCE, use 'threads'. Use Queue to cache tasks and run MULTI tasks at ONCE.
+        """
+        if mode in ['async', 'thread'] and n_worker is not None:
+            put_err(f'n_worker should be None when mode is {mode}, skip')
+        self.MODE = mode
+        self.N_WORKER = n_worker
+        self._async_loop: asyncio.AbstractEventLoop = None
+        self._thread_task_queue: Queue = Queue()
+        self._thread_result_queue: Queue = Queue()
+        self._thread_quit_event: threading.Event = threading.Event()
+        self.thread: threading.Thread = None
         self.tasks = {}
         self.TASK_NOT_FOUND = TaskStatus.NOT_FOUND        
         self.TASK_NOT_FINISHED = TaskStatus.NOT_FINISHED
         self.TASK_NOT_SUCCEEDED = TaskStatus.NOT_SUCCEEDED
 
-    def _run_loop(self):
-        asyncio.set_event_loop(self.loop)
-        self.loop.run_forever()
+    def _run_async_loop(self):
+        asyncio.set_event_loop(self._async_loop)
+        self._async_loop.run_forever()
+        
+    def _run_thread_loop(self):
+        while not self._thread_quit_event.is_set():
+            if not self._thread_task_queue.empty():
+                task_name, task_func, task_args, task_kwargs = self._thread_task_queue.get()
+                try:
+                    result = task_func(*task_args, **task_kwargs)
+                    self._thread_result_queue.put((task_name, result, TaskStatus.SUCCEED))
+                except Exception as e:
+                    self._thread_result_queue.put((task_name, e, TaskStatus.NOT_SUCCEEDED))
+            time.sleep(0.1)
 
+    def _add_task_async(self, name: str, coro_func, *args, **kwargs):
+        future = asyncio.run_coroutine_threadsafe(coro_func(*args, **kwargs), self._async_loop)
+        self.tasks[name] = future
+        return name
+    
+    def _add_task_thread(self, name: str, func, *args, **kwargs):
+        self._thread_task_queue.put((name, func, args, kwargs))
+        self.tasks[name] = TaskStatus.NOT_RETURNED
+        return name
+    
+    def _add_task_threads(self, name: str, func, *args, **kwargs):
+        return self._add_task_thread(name, func, *args, **kwargs)
+    
     def add_task(self, name: str, coro_func, *args, **kwargs):
         if name == '' or name is None:
             name = f'{coro_func.__name__}-{time.time():.2f}'
-        future = asyncio.run_coroutine_threadsafe(coro_func(*args, **kwargs), self.loop)
-        self.tasks[name] = future
-        return name
+        if name in self.tasks:
+            put_err(f'Task {name} already exists, replace it with the new one')
+        return getattr(self, f'_add_task_{self.MODE}')(name, coro_func, *args, **kwargs)
 
-    def query_task(self, name):
+    def _query_async_task(self, name, block: bool = True, timeout: int = 3):
         if name in self.tasks:
             future = self.tasks[name]
             if future.done():
                 try:
                     result = future.result()
                     del self.tasks[name]
                     return result
                 except Exception as e:
                     del self.tasks[name]
                     return self.TASK_NOT_SUCCEEDED, e
             else:
                 return self.TASK_NOT_FINISHED
         else:
             return self.TASK_NOT_FOUND
+        
+    def _query_thread_task(self, name, block: bool = True, timeout: int = 3):
+        # short-cut for not found
+        if name not in self.tasks:
+            return self.TASK_NOT_FOUND
+        # retrive finished results
+        while not self._thread_result_queue.empty():
+            try:
+                _name, result, statue = self._thread_result_queue.get(block, timeout)
+                self.tasks[_name] = (_name, result, statue)
+            except:
+                pass
+        # check if not return, succeed, or not succeed
+        if self.tasks[name] == TaskStatus.NOT_RETURNED:
+            return self.TASK_NOT_FINISHED
+        else:
+            _name, result, statue = self.tasks[name]
+            del self.tasks[name]
+            if statue == TaskStatus.NOT_SUCCEEDED:
+                put_err(f'Task {name} failed with {result}, return {result}')
+            return result
+        
+    def _query_threads_task(self, name, block: bool = True, timeout: int = 3):
+        return self._query_thread_task(name, block, timeout)
+        
+    def query_task(self, name: str, block: bool = False):
+        return getattr(self, f'_query_{self.MODE}_task')(name, block)
 
     def run(self):
-        self.loop = asyncio.new_event_loop()      
-        self.thread = threading.Thread(target=self._run_loop, daemon=True)
-        self.thread.start()
+        if self.MODE == 'async':
+            self._async_loop = asyncio.new_event_loop()
+        if self.MODE == 'threads':
+            self.thread = []
+            for _ in range(self.N_WORKER):
+                self.thread.append(threading.Thread(target=self._run_thread_loop, daemon=True))
+                self.thread[-1].start()
+        else:
+            self.thread = threading.Thread(target=getattr(self, f'_run_{self.MODE}_loop'), daemon=True)
+            self.thread.start()
         return self
     
     def check_empty(self):
-        for task in self.tasks.values():
-            if not task.done():
-                return False
-        return True
+        if self.MODE == 'async':
+            for task in self.tasks.values():
+                if not task.done():
+                    return False
+            return True
+        elif self.MODE in ['thread', 'threads']:
+            return self._thread_task_queue.empty()
     
     def close(self):
-        self.loop.close()
+        if self.MODE == 'async':
+            self._async_loop.close()
+            self.thread.join()
+        elif self.MODE == 'thread':
+            self._thread_quit_event.set()
+            self.thread.join()
+        elif self.MODE == 'threads':
+            self._thread_quit_event.set()
+            [t.join() for t in self.thread]
 
 
 __all__ = [
     'Key2Action',
     'statuesQue',
     '_wait_for_quit',
     'statues_que_opts',
     'get_input',
     'launch_sub_thread',
     'show_prog_info',
     'Timer',
     'ThreadsPool',
     'TaskStatus',
-    'CoroutinePool'
+    'TaskPool'
 ]
 
 
 if __name__ == '__main__':
     # dev code
     async def example_coroutine(name, seconds):
         print(f"Coroutine {name} started")
         await asyncio.sleep(seconds)
         print(f"Coroutine {name} finished after {seconds} seconds")
         return f"Coroutine {name} result"
 
-    pool = CoroutinePool().run()
-    pool.add_task("task1", example_coroutine, "task1", 3)
-    pool.add_task("task2", example_coroutine, "task2", 5)
-
-    print(pool.query_task("task1"))  # Output: TaskStatus.NOT_FINISHED
-    print(pool.query_task("task2"))  # Output: TaskStatus.NOT_FINISHED
-
-    # wait for tasks to finish
-    import time
-    time.sleep(6)
-
-    print(pool.query_task("task1"))  # Output: Coroutine task1 finished after 3 seconds
-    print(pool.query_task("task2"))  # Output: Coroutine task2 finished after 5 seconds
+    pool = TaskPool().run()
+    pool.add_task("task1", example_coroutine, "task1", 2)
+    pool.add_task("task2", example_coroutine, "task2", 4)
```

### Comparing `mbapy-0.7.2/mbapy.egg-info/PKG-INFO` & `mbapy-0.7.3/mbapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbapy
-Version: 0.7.2
+Version: 0.7.3
 Summary: MyBA in Python
 Home-page: https://github.com/BHM-Bob/BA_PY
 Author: BHM-Bob G
 Author-email: bhmfly@foxmail.com
 License: MIT Licence
 Description: <!--
          * @Author: BHM-Bob 2262029386@qq.com
```

### Comparing `mbapy-0.7.2/mbapy.egg-info/SOURCES.txt` & `mbapy-0.7.3/mbapy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,18 @@
 mbapy/dl_torch/arch/CLIP/builder.py
 mbapy/dl_torch/arch/CLIP/trainer.py
 mbapy/dl_torch/paper/__init__.py
 mbapy/dl_torch/paper/bb.py
 mbapy/file_utils/__init__.py
 mbapy/file_utils/image.py
 mbapy/file_utils/video.py
+mbapy/plot_utils/__init__.py
+mbapy/plot_utils/bar_utils.py
+mbapy/plot_utils/line_utils.py
+mbapy/plot_utils/scatter_utils.py
 mbapy/sci_utils/__init__.py
 mbapy/sci_utils/paper_download.py
 mbapy/sci_utils/paper_parse.py
 mbapy/sci_utils/paper_search.py
 mbapy/scripts/__init__.py
 mbapy/scripts/__main__.py
 mbapy/scripts/_main_.py
```

### Comparing `mbapy-0.7.2/mbapy.egg-info/requires.txt` & `mbapy-0.7.3/mbapy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/requirements.json` & `mbapy-0.7.3/requirements.json`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/setup.py` & `mbapy-0.7.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2022-11-01 18:30:01
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2024-04-21 21:07:12
+LastEditTime: 2024-04-25 23:18:02
 Description: 
 '''
 """
 something is from https://github.com/pypa/sampleproject
 thanks to https://zetcode.com/python/package/
 thanks to https://github.com/gaogaotiantian/viztracer/blob/master/setup.py
 """
@@ -104,8 +104,8 @@
         'full': requirements['std'] + requirements['full'],
         },
 )
 
 # pip install .
 
 # python setup.py sdist
-# twine upload dist/mbapy-0.7.2.tar.gz
+# twine upload dist/mbapy-0.7.3.tar.gz
```

### Comparing `mbapy-0.7.2/test/test_base.py` & `mbapy-0.7.3/test/test_base.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/test/test_game.py` & `mbapy-0.7.3/test/test_game.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.2/test/test_web.py` & `mbapy-0.7.3/test/test_web.py`

 * *Files identical despite different names*


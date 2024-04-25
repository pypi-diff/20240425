# Comparing `tmp/pyDecision-4.4.3.tar.gz` & `tmp/pyDecision-4.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyDecision-4.4.3.tar", last modified: Wed Apr 24 15:12:50 2024, max compression
+gzip compressed data, was "dist\pyDecision-4.4.5.tar", last modified: Thu Apr 25 16:02:21 2024, max compression
```

## Comparing `pyDecision-4.4.3.tar` & `pyDecision-4.4.5.tar`

### file list

```diff
@@ -1,91 +1,93 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 15:12:50.000000 pyDecision-4.4.3/
--rw-rw-rw-   0        0        0      656 2023-10-24 20:28:27.000000 pyDecision-4.4.3/LICENSE
--rw-rw-rw-   0        0        0    18281 2024-04-24 15:12:50.000000 pyDecision-4.4.3/PKG-INFO
--rw-rw-rw-   0        0        0    17788 2024-04-24 15:11:29.000000 pyDecision-4.4.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 15:12:49.000000 pyDecision-4.4.3/pyDecision/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-4.4.3/pyDecision/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 15:12:49.000000 pyDecision-4.4.3/pyDecision/algorithm/
--rw-rw-rw-   0        0        0     2856 2024-04-24 13:00:49.000000 pyDecision-4.4.3/pyDecision/algorithm/__init__.py
--rw-rw-rw-   0        0        0     1638 2023-08-15 11:11:40.000000 pyDecision-4.4.3/pyDecision/algorithm/ahp.py
--rw-rw-rw-   0        0        0     2591 2023-07-21 17:32:54.000000 pyDecision-4.4.3/pyDecision/algorithm/aras.py
--rw-rw-rw-   0        0        0     2147 2023-07-21 20:21:53.000000 pyDecision-4.4.3/pyDecision/algorithm/borda.py
--rw-rw-rw-   0        0        0     2553 2023-11-10 15:52:16.000000 pyDecision-4.4.3/pyDecision/algorithm/bwm.py
--rw-rw-rw-   0        0        0     1006 2023-11-12 15:54:44.000000 pyDecision-4.4.3/pyDecision/algorithm/bwm_s.py
--rw-rw-rw-   0        0        0     1221 2024-04-24 14:49:40.000000 pyDecision-4.4.3/pyDecision/algorithm/cilos.py
--rw-rw-rw-   0        0        0     2762 2023-07-22 02:44:56.000000 pyDecision-4.4.3/pyDecision/algorithm/cocoso.py
--rw-rw-rw-   0        0        0     2754 2023-07-21 17:33:49.000000 pyDecision-4.4.3/pyDecision/algorithm/codas.py
--rw-rw-rw-   0        0        0     2870 2023-07-23 17:00:58.000000 pyDecision-4.4.3/pyDecision/algorithm/copeland.py
--rw-rw-rw-   0        0        0     2471 2023-07-21 17:34:03.000000 pyDecision-4.4.3/pyDecision/algorithm/copras.py
--rw-rw-rw-   0        0        0     2347 2023-07-23 16:38:01.000000 pyDecision-4.4.3/pyDecision/algorithm/cradis.py
--rw-rw-rw-   0        0        0     1125 2023-10-24 20:07:49.000000 pyDecision-4.4.3/pyDecision/algorithm/critic.py
--rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-4.4.3/pyDecision/algorithm/dematel.py
--rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-4.4.3/pyDecision/algorithm/e_i.py
--rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-4.4.3/pyDecision/algorithm/e_i_s.py
--rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-4.4.3/pyDecision/algorithm/e_i_v.py
--rw-rw-rw-   0        0        0    16907 2023-07-21 20:38:15.000000 pyDecision-4.4.3/pyDecision/algorithm/e_ii.py
--rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-4.4.3/pyDecision/algorithm/e_iii.py
--rw-rw-rw-   0        0        0    14298 2023-07-21 19:41:40.000000 pyDecision-4.4.3/pyDecision/algorithm/e_iv.py
--rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-4.4.3/pyDecision/algorithm/e_tri_b.py
--rw-rw-rw-   0        0        0     2711 2023-07-21 20:33:16.000000 pyDecision-4.4.3/pyDecision/algorithm/edas.py
--rw-rw-rw-   0        0        0      925 2023-07-19 01:09:53.000000 pyDecision-4.4.3/pyDecision/algorithm/entropy.py
--rw-rw-rw-   0        0        0     2166 2024-04-24 15:10:36.000000 pyDecision-4.4.3/pyDecision/algorithm/fucom.py
--rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-4.4.3/pyDecision/algorithm/fuzzy_ahp.py
--rw-rw-rw-   0        0        0     3321 2023-07-25 15:17:23.000000 pyDecision-4.4.3/pyDecision/algorithm/fuzzy_aras.py
--rw-rw-rw-   0        0        0     4635 2023-11-12 11:24:00.000000 pyDecision-4.4.3/pyDecision/algorithm/fuzzy_bwm.py
--rw-rw-rw-   0        0        0     4545 2023-07-21 17:31:44.000000 pyDecision-4.4.3/pyDecision/algorithm/fuzzy_copras.py
--rw-rw-rw-   0        0        0     4100 2023-08-01 01:06:41.000000 pyDecision-4.4.3/pyDecision/algorithm/fuzzy_dematel.py
--rw-rw-rw-   0        0        0     5042 2023-07-21 18:03:22.000000 pyDecision-4.4.3/pyDecision/algorithm/fuzzy_edas.py
--rw-rw-rw-   0        0        0     3706 2023-07-21 18:11:21.000000 pyDecision-4.4.3/pyDecision/algorithm/fuzzy_moora.py
--rw-rw-rw-   0        0        0     4098 2023-07-21 18:13:14.000000 pyDecision-4.4.3/pyDecision/algorithm/fuzzy_ocra.py
--rw-rw-rw-   0        0        0     4086 2023-07-21 18:17:14.000000 pyDecision-4.4.3/pyDecision/algorithm/fuzzy_topsis.py
--rw-rw-rw-   0        0        0     5994 2023-07-21 18:18:25.000000 pyDecision-4.4.3/pyDecision/algorithm/fuzzy_vikor.py
--rw-rw-rw-   0        0        0     5399 2023-09-09 01:09:43.000000 pyDecision-4.4.3/pyDecision/algorithm/fuzzy_waspas.py
--rw-rw-rw-   0        0        0     2553 2023-07-22 02:46:58.000000 pyDecision-4.4.3/pyDecision/algorithm/gra.py
--rw-rw-rw-   0        0        0     2300 2023-10-26 23:42:55.000000 pyDecision-4.4.3/pyDecision/algorithm/idocriw.py
--rw-rw-rw-   0        0        0     2585 2023-07-21 18:06:06.000000 pyDecision-4.4.3/pyDecision/algorithm/mabac.py
--rw-rw-rw-   0        0        0     2388 2023-07-28 22:31:36.000000 pyDecision-4.4.3/pyDecision/algorithm/macbeth.py
--rw-rw-rw-   0        0        0     2575 2023-07-23 16:39:11.000000 pyDecision-4.4.3/pyDecision/algorithm/mairca.py
--rw-rw-rw-   0        0        0     3048 2023-07-21 18:09:18.000000 pyDecision-4.4.3/pyDecision/algorithm/marcos.py
--rw-rw-rw-   0        0        0     3766 2023-07-22 02:46:58.000000 pyDecision-4.4.3/pyDecision/algorithm/maut.py
--rw-rw-rw-   0        0        0     1175 2023-10-26 23:47:00.000000 pyDecision-4.4.3/pyDecision/algorithm/merec.py
--rw-rw-rw-   0        0        0     2541 2023-07-21 18:10:51.000000 pyDecision-4.4.3/pyDecision/algorithm/moora.py
--rw-rw-rw-   0        0        0     2549 2023-07-21 18:12:07.000000 pyDecision-4.4.3/pyDecision/algorithm/moosra.py
--rw-rw-rw-   0        0        0     4968 2023-07-22 01:50:19.000000 pyDecision-4.4.3/pyDecision/algorithm/multimoora.py
--rw-rw-rw-   0        0        0     2477 2023-07-21 23:26:24.000000 pyDecision-4.4.3/pyDecision/algorithm/ocra.py
--rw-rw-rw-   0        0        0     2563 2023-09-09 00:46:31.000000 pyDecision-4.4.3/pyDecision/algorithm/oreste.py
--rw-rw-rw-   0        0        0    13836 2023-10-30 12:17:12.000000 pyDecision-4.4.3/pyDecision/algorithm/p_ec.py
--rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-4.4.3/pyDecision/algorithm/p_i.py
--rw-rw-rw-   0        0        0     5891 2023-07-21 19:40:41.000000 pyDecision-4.4.3/pyDecision/algorithm/p_ii.py
--rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-4.4.3/pyDecision/algorithm/p_iii.py
--rw-rw-rw-   0        0        0     8547 2023-07-21 19:39:42.000000 pyDecision-4.4.3/pyDecision/algorithm/p_iv.py
--rw-rw-rw-   0        0        0     6622 2023-08-02 21:49:15.000000 pyDecision-4.4.3/pyDecision/algorithm/p_v.py
--rw-rw-rw-   0        0        0     9380 2023-07-21 19:37:53.000000 pyDecision-4.4.3/pyDecision/algorithm/p_vi.py
--rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-4.4.3/pyDecision/algorithm/p_xgaia.py
--rw-rw-rw-   0        0        0     2139 2023-07-23 16:40:26.000000 pyDecision-4.4.3/pyDecision/algorithm/piv.py
--rw-rw-rw-   0        0        0     2184 2023-07-21 18:14:04.000000 pyDecision-4.4.3/pyDecision/algorithm/psi.py
--rw-rw-rw-   0        0        0     5228 2023-07-29 11:05:11.000000 pyDecision-4.4.3/pyDecision/algorithm/regime.py
--rw-rw-rw-   0        0        0     2434 2023-07-22 02:08:59.000000 pyDecision-4.4.3/pyDecision/algorithm/rov.py
--rw-rw-rw-   0        0        0     2130 2023-07-21 18:14:55.000000 pyDecision-4.4.3/pyDecision/algorithm/saw.py
--rw-rw-rw-   0        0        0     2344 2023-07-21 18:15:17.000000 pyDecision-4.4.3/pyDecision/algorithm/smart.py
--rw-rw-rw-   0        0        0     2185 2023-08-02 00:35:27.000000 pyDecision-4.4.3/pyDecision/algorithm/spotis.py
--rw-rw-rw-   0        0        0     2867 2023-07-21 18:15:39.000000 pyDecision-4.4.3/pyDecision/algorithm/todim.py
--rw-rw-rw-   0        0        0     2600 2023-07-21 18:16:04.000000 pyDecision-4.4.3/pyDecision/algorithm/topsis.py
--rw-rw-rw-   0        0        0     3703 2023-07-22 03:11:26.000000 pyDecision-4.4.3/pyDecision/algorithm/vikor.py
--rw-rw-rw-   0        0        0     4278 2023-09-08 23:55:42.000000 pyDecision-4.4.3/pyDecision/algorithm/waspas.py
--rw-rw-rw-   0        0        0     2643 2023-07-21 18:23:36.000000 pyDecision-4.4.3/pyDecision/algorithm/wings.py
--rw-rw-rw-   0        0        0     3188 2024-04-24 01:11:01.000000 pyDecision-4.4.3/pyDecision/algorithm/wisp.py
-drwxrwxrwx   0        0        0        0 2024-04-24 15:12:50.000000 pyDecision-4.4.3/pyDecision/compare/
--rw-rw-rw-   0        0        0      104 2023-08-02 19:39:50.000000 pyDecision-4.4.3/pyDecision/compare/__init__.py
--rw-rw-rw-   0        0        0    23637 2024-04-24 15:08:34.000000 pyDecision-4.4.3/pyDecision/compare/compare.py
-drwxrwxrwx   0        0        0        0 2024-04-24 15:12:50.000000 pyDecision-4.4.3/pyDecision/util/
--rw-rw-rw-   0        0        0     8733 2023-12-03 18:26:24.000000 pyDecision-4.4.3/pyDecision/util/LLM.py
--rw-rw-rw-   0        0        0      109 2023-08-02 19:44:51.000000 pyDecision-4.4.3/pyDecision/util/__init__.py
--rw-rw-rw-   0        0        0     6266 2023-08-02 19:44:27.000000 pyDecision-4.4.3/pyDecision/util/ga.py
-drwxrwxrwx   0        0        0        0 2024-04-24 15:12:49.000000 pyDecision-4.4.3/pyDecision.egg-info/
--rw-rw-rw-   0        0        0    18281 2024-04-24 15:12:48.000000 pyDecision-4.4.3/pyDecision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2490 2024-04-24 15:12:48.000000 pyDecision-4.4.3/pyDecision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 15:12:48.000000 pyDecision-4.4.3/pyDecision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-24 15:12:48.000000 pyDecision-4.4.3/pyDecision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-24 15:12:48.000000 pyDecision-4.4.3/pyDecision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 15:12:50.000000 pyDecision-4.4.3/setup.cfg
--rw-rw-rw-   0        0        0      744 2024-04-24 15:10:50.000000 pyDecision-4.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:02:21.000000 pyDecision-4.4.5/
+-rw-rw-rw-   0        0        0      656 2023-10-24 20:28:27.000000 pyDecision-4.4.5/LICENSE
+-rw-rw-rw-   0        0        0    18765 2024-04-25 16:02:21.000000 pyDecision-4.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0    18270 2024-04-25 15:42:00.000000 pyDecision-4.4.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 16:02:20.000000 pyDecision-4.4.5/pyDecision/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-4.4.5/pyDecision/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:02:21.000000 pyDecision-4.4.5/pyDecision/algorithm/
+-rw-rw-rw-   0        0        0     2934 2024-04-25 15:49:24.000000 pyDecision-4.4.5/pyDecision/algorithm/__init__.py
+-rw-rw-rw-   0        0        0     1638 2023-08-15 11:11:40.000000 pyDecision-4.4.5/pyDecision/algorithm/ahp.py
+-rw-rw-rw-   0        0        0     2591 2023-07-21 17:32:54.000000 pyDecision-4.4.5/pyDecision/algorithm/aras.py
+-rw-rw-rw-   0        0        0     2147 2023-07-21 20:21:53.000000 pyDecision-4.4.5/pyDecision/algorithm/borda.py
+-rw-rw-rw-   0        0        0     2553 2023-11-10 15:52:16.000000 pyDecision-4.4.5/pyDecision/algorithm/bwm.py
+-rw-rw-rw-   0        0        0     1006 2023-11-12 15:54:44.000000 pyDecision-4.4.5/pyDecision/algorithm/bwm_s.py
+-rw-rw-rw-   0        0        0     1221 2024-04-24 14:49:40.000000 pyDecision-4.4.5/pyDecision/algorithm/cilos.py
+-rw-rw-rw-   0        0        0     2762 2023-07-22 02:44:56.000000 pyDecision-4.4.5/pyDecision/algorithm/cocoso.py
+-rw-rw-rw-   0        0        0     2754 2023-07-21 17:33:49.000000 pyDecision-4.4.5/pyDecision/algorithm/codas.py
+-rw-rw-rw-   0        0        0     2870 2023-07-23 17:00:58.000000 pyDecision-4.4.5/pyDecision/algorithm/copeland.py
+-rw-rw-rw-   0        0        0     2471 2023-07-21 17:34:03.000000 pyDecision-4.4.5/pyDecision/algorithm/copras.py
+-rw-rw-rw-   0        0        0     2347 2023-07-23 16:38:01.000000 pyDecision-4.4.5/pyDecision/algorithm/cradis.py
+-rw-rw-rw-   0        0        0     1125 2023-10-24 20:07:49.000000 pyDecision-4.4.5/pyDecision/algorithm/critic.py
+-rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-4.4.5/pyDecision/algorithm/dematel.py
+-rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-4.4.5/pyDecision/algorithm/e_i.py
+-rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-4.4.5/pyDecision/algorithm/e_i_s.py
+-rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-4.4.5/pyDecision/algorithm/e_i_v.py
+-rw-rw-rw-   0        0        0    16907 2023-07-21 20:38:15.000000 pyDecision-4.4.5/pyDecision/algorithm/e_ii.py
+-rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-4.4.5/pyDecision/algorithm/e_iii.py
+-rw-rw-rw-   0        0        0    14298 2023-07-21 19:41:40.000000 pyDecision-4.4.5/pyDecision/algorithm/e_iv.py
+-rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-4.4.5/pyDecision/algorithm/e_tri_b.py
+-rw-rw-rw-   0        0        0     2711 2023-07-21 20:33:16.000000 pyDecision-4.4.5/pyDecision/algorithm/edas.py
+-rw-rw-rw-   0        0        0      925 2023-07-19 01:09:53.000000 pyDecision-4.4.5/pyDecision/algorithm/entropy.py
+-rw-rw-rw-   0        0        0     2289 2024-04-24 15:29:47.000000 pyDecision-4.4.5/pyDecision/algorithm/fucom.py
+-rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-4.4.5/pyDecision/algorithm/fuzzy_ahp.py
+-rw-rw-rw-   0        0        0     3321 2023-07-25 15:17:23.000000 pyDecision-4.4.5/pyDecision/algorithm/fuzzy_aras.py
+-rw-rw-rw-   0        0        0     4635 2023-11-12 11:24:00.000000 pyDecision-4.4.5/pyDecision/algorithm/fuzzy_bwm.py
+-rw-rw-rw-   0        0        0     4545 2023-07-21 17:31:44.000000 pyDecision-4.4.5/pyDecision/algorithm/fuzzy_copras.py
+-rw-rw-rw-   0        0        0     4100 2023-08-01 01:06:41.000000 pyDecision-4.4.5/pyDecision/algorithm/fuzzy_dematel.py
+-rw-rw-rw-   0        0        0     5042 2023-07-21 18:03:22.000000 pyDecision-4.4.5/pyDecision/algorithm/fuzzy_edas.py
+-rw-rw-rw-   0        0        0     3706 2023-07-21 18:11:21.000000 pyDecision-4.4.5/pyDecision/algorithm/fuzzy_moora.py
+-rw-rw-rw-   0        0        0     4098 2023-07-21 18:13:14.000000 pyDecision-4.4.5/pyDecision/algorithm/fuzzy_ocra.py
+-rw-rw-rw-   0        0        0     4086 2023-07-21 18:17:14.000000 pyDecision-4.4.5/pyDecision/algorithm/fuzzy_topsis.py
+-rw-rw-rw-   0        0        0     5994 2023-07-21 18:18:25.000000 pyDecision-4.4.5/pyDecision/algorithm/fuzzy_vikor.py
+-rw-rw-rw-   0        0        0     5399 2023-09-09 01:09:43.000000 pyDecision-4.4.5/pyDecision/algorithm/fuzzy_waspas.py
+-rw-rw-rw-   0        0        0     2553 2023-07-22 02:46:58.000000 pyDecision-4.4.5/pyDecision/algorithm/gra.py
+-rw-rw-rw-   0        0        0     2300 2023-10-26 23:42:55.000000 pyDecision-4.4.5/pyDecision/algorithm/idocriw.py
+-rw-rw-rw-   0        0        0     2585 2023-07-21 18:06:06.000000 pyDecision-4.4.5/pyDecision/algorithm/mabac.py
+-rw-rw-rw-   0        0        0     2388 2023-07-28 22:31:36.000000 pyDecision-4.4.5/pyDecision/algorithm/macbeth.py
+-rw-rw-rw-   0        0        0     2575 2023-07-23 16:39:11.000000 pyDecision-4.4.5/pyDecision/algorithm/mairca.py
+-rw-rw-rw-   0        0        0     2598 2024-04-25 15:20:07.000000 pyDecision-4.4.5/pyDecision/algorithm/mara.py
+-rw-rw-rw-   0        0        0     3048 2023-07-21 18:09:18.000000 pyDecision-4.4.5/pyDecision/algorithm/marcos.py
+-rw-rw-rw-   0        0        0     3766 2023-07-22 02:46:58.000000 pyDecision-4.4.5/pyDecision/algorithm/maut.py
+-rw-rw-rw-   0        0        0     1175 2023-10-26 23:47:00.000000 pyDecision-4.4.5/pyDecision/algorithm/merec.py
+-rw-rw-rw-   0        0        0     2541 2023-07-21 18:10:51.000000 pyDecision-4.4.5/pyDecision/algorithm/moora.py
+-rw-rw-rw-   0        0        0     2549 2023-07-21 18:12:07.000000 pyDecision-4.4.5/pyDecision/algorithm/moosra.py
+-rw-rw-rw-   0        0        0     4968 2023-07-22 01:50:19.000000 pyDecision-4.4.5/pyDecision/algorithm/multimoora.py
+-rw-rw-rw-   0        0        0     2477 2023-07-21 23:26:24.000000 pyDecision-4.4.5/pyDecision/algorithm/ocra.py
+-rw-rw-rw-   0        0        0     2563 2023-09-09 00:46:31.000000 pyDecision-4.4.5/pyDecision/algorithm/oreste.py
+-rw-rw-rw-   0        0        0    13836 2023-10-30 12:17:12.000000 pyDecision-4.4.5/pyDecision/algorithm/p_ec.py
+-rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-4.4.5/pyDecision/algorithm/p_i.py
+-rw-rw-rw-   0        0        0     5891 2023-07-21 19:40:41.000000 pyDecision-4.4.5/pyDecision/algorithm/p_ii.py
+-rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-4.4.5/pyDecision/algorithm/p_iii.py
+-rw-rw-rw-   0        0        0     8547 2023-07-21 19:39:42.000000 pyDecision-4.4.5/pyDecision/algorithm/p_iv.py
+-rw-rw-rw-   0        0        0     6622 2023-08-02 21:49:15.000000 pyDecision-4.4.5/pyDecision/algorithm/p_v.py
+-rw-rw-rw-   0        0        0     9380 2023-07-21 19:37:53.000000 pyDecision-4.4.5/pyDecision/algorithm/p_vi.py
+-rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-4.4.5/pyDecision/algorithm/p_xgaia.py
+-rw-rw-rw-   0        0        0     2139 2023-07-23 16:40:26.000000 pyDecision-4.4.5/pyDecision/algorithm/piv.py
+-rw-rw-rw-   0        0        0     2184 2023-07-21 18:14:04.000000 pyDecision-4.4.5/pyDecision/algorithm/psi.py
+-rw-rw-rw-   0        0        0      688 2024-04-25 15:23:46.000000 pyDecision-4.4.5/pyDecision/algorithm/psi_m.py
+-rw-rw-rw-   0        0        0     5265 2024-04-25 14:52:15.000000 pyDecision-4.4.5/pyDecision/algorithm/regime.py
+-rw-rw-rw-   0        0        0     2434 2023-07-22 02:08:59.000000 pyDecision-4.4.5/pyDecision/algorithm/rov.py
+-rw-rw-rw-   0        0        0     2130 2023-07-21 18:14:55.000000 pyDecision-4.4.5/pyDecision/algorithm/saw.py
+-rw-rw-rw-   0        0        0     2344 2023-07-21 18:15:17.000000 pyDecision-4.4.5/pyDecision/algorithm/smart.py
+-rw-rw-rw-   0        0        0     2185 2023-08-02 00:35:27.000000 pyDecision-4.4.5/pyDecision/algorithm/spotis.py
+-rw-rw-rw-   0        0        0     2867 2023-07-21 18:15:39.000000 pyDecision-4.4.5/pyDecision/algorithm/todim.py
+-rw-rw-rw-   0        0        0     2600 2023-07-21 18:16:04.000000 pyDecision-4.4.5/pyDecision/algorithm/topsis.py
+-rw-rw-rw-   0        0        0     3703 2023-07-22 03:11:26.000000 pyDecision-4.4.5/pyDecision/algorithm/vikor.py
+-rw-rw-rw-   0        0        0     4278 2023-09-08 23:55:42.000000 pyDecision-4.4.5/pyDecision/algorithm/waspas.py
+-rw-rw-rw-   0        0        0     2643 2023-07-21 18:23:36.000000 pyDecision-4.4.5/pyDecision/algorithm/wings.py
+-rw-rw-rw-   0        0        0     3188 2024-04-24 01:11:01.000000 pyDecision-4.4.5/pyDecision/algorithm/wisp.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:02:21.000000 pyDecision-4.4.5/pyDecision/compare/
+-rw-rw-rw-   0        0        0      104 2024-04-25 14:56:00.000000 pyDecision-4.4.5/pyDecision/compare/__init__.py
+-rw-rw-rw-   0        0        0    24199 2024-04-25 16:00:45.000000 pyDecision-4.4.5/pyDecision/compare/compare.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:02:21.000000 pyDecision-4.4.5/pyDecision/util/
+-rw-rw-rw-   0        0        0     8733 2023-12-03 18:26:24.000000 pyDecision-4.4.5/pyDecision/util/LLM.py
+-rw-rw-rw-   0        0        0      109 2023-08-02 19:44:51.000000 pyDecision-4.4.5/pyDecision/util/__init__.py
+-rw-rw-rw-   0        0        0     6266 2023-08-02 19:44:27.000000 pyDecision-4.4.5/pyDecision/util/ga.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:02:20.000000 pyDecision-4.4.5/pyDecision.egg-info/
+-rw-rw-rw-   0        0        0    18765 2024-04-25 16:02:19.000000 pyDecision-4.4.5/pyDecision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2549 2024-04-25 16:02:20.000000 pyDecision-4.4.5/pyDecision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 16:02:19.000000 pyDecision-4.4.5/pyDecision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-25 16:02:19.000000 pyDecision-4.4.5/pyDecision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-25 16:02:19.000000 pyDecision-4.4.5/pyDecision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 16:02:21.000000 pyDecision-4.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      744 2024-04-25 16:01:20.000000 pyDecision-4.4.5/setup.py
```

### Comparing `pyDecision-4.4.3/LICENSE` & `pyDecision-4.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/PKG-INFO` & `pyDecision-4.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 4.4.3
+Version: 4.4.5
 Summary: A MCDA Library Incorporating a Large Language Model to Enhance Decision Analysis
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **Regime**; **ROV** (Range Of Value); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **Fuzzy WASPAS**. 
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **Regime** (REGIonal Multicriteria Elimination); **ROV** (Range Of Value); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **Fuzzy WASPAS**. 
 
 pyDecision offers an array of features, including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
 
 ## Citation
 
 PEREIRA, V.; BASILIO, M.P.; SANTOS, C.H.T (2024). Enhancing Decision Analysis with a Large Language Model: pyDecision a Comprehensive Library of MCDA Methods in Python. arXiv. https://arxiv.org/abs/2404.06370
 
@@ -98,14 +98,15 @@
 - ELECTRE Tri-B ([ Colab Demo ](https://colab.research.google.com/drive/1hu0fJcxdBAiEDrVngmKQfpINpjTF-osE?usp=sharing)) ( [ Paper ](https://drive.google.com/file/d/1oWOI_sX3EEYdRbavoBTT7vUmPII1yPgE/view?usp=sharing))
 - FUCOM ([ Colab Demo ](https://colab.research.google.com/drive/1eWP3xf3-9iLLW_l_9JuAe6BEeoMsqzcL?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/sym10090393))
 - GRA ([ Colab Demo ](https://colab.research.google.com/drive/1aMMI0Cuo5kpzTDefqEwJhf0wWpBOP_JL?usp=sharing)) ( [ Paper ](https://uranos.ch/research/references/Julong_1989/10.1.1.678.3477.pdf))
 - IDOCRIW ([ Colab Demo ](https://colab.research.google.com/drive/1zt8uPFZGcHaSnpiT7tDnrDjvs0pK_7vS?usp=sharing)) ( [ Paper ](https://doi.org/10.1142/S0219622016500036))
 - MABAC ([ Colab Demo ](https://colab.research.google.com/drive/1BMqO-HnBXdcOZfZoULpx1H4MLPoUGucJ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2014.11.057))
 - MACBETH ([ Colab Demo ](https://colab.research.google.com/drive/1GqM9uPgbaWCGyj4l-XjkoifY2JJoVyf2?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0969-6016(94)90010-8))
 - MAIRCA ([ Colab Demo ](https://colab.research.google.com/drive/1gfqgrBAFGVygwm1j3lTjfy5wTsLgT_j5?usp=sharing)) ( [ Paper ](https://doi.org/10.1080/1331677X.2018.1506706))
+- MARA ([ Colab Demo ](https://colab.research.google.com/drive/1Ggg5e7TKVF_JN4yZRq9zThJO-PRBSI-N?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/systems10060248))
 - MARCOS ([ Colab Demo ](https://colab.research.google.com/drive/13MI2Qrakm5VzHN3r5O2RqggCzQwRxCs-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.cie.2019.106231))
 - MAUT ([ Colab Demo ](https://colab.research.google.com/drive/1qm3ARgQm68GUK2irGiCB-B49vnVHazB7?usp=sharing)) ( [ Paper ](https://doi.org/10.1017/CBO9781139174084))
 - MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1XE3AIzS84w-gw_1MEtV7xvkU1Gj_tRPd?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/sym13040525))
 - MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1FpKl0QAdwGgCVvLYsRHvMWhz7yOp17B5?usp=sharing)) ( [ Paper ](http://matwbn.icm.edu.pl/ksiazki/cc/cc35/cc35213.pdf))
 - Fuzzy MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1ydHzGeA8WBVY5Gyu8K7Oq6kofQ5XbK3P?usp=sharing)) ( [ Paper ](https://pdfs.semanticscholar.org/6d33/ca3f14c9ed44d23742fd4e9cf94cebcaf148.pdf))
 - MOOSRA ([ Colab Demo ](https://colab.research.google.com/drive/1KYyA4f3OsipPA5e63Ja4A0OGmHvNY6dj?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.15623/ijret.2014.0315105))
 - MULTIMOORA ([ Colab Demo ](https://colab.research.google.com/drive/1JAT8qqHPNoFfMV6a-CzF6BgRwtcUF3-e?usp=sharing)) ( [ Paper ](https://journals.vilniustech.lt/index.php/TEDE/article/view/5832/5078))
@@ -119,14 +120,15 @@
 ))
 - PROMETHEE IV   ([ Colab Demo ](https://colab.research.google.com/drive/1X2evE6pIf4F7qiKjt1fSU2PqT-NaA5sJ?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-319-11949-6_14))
 - PROMETHEE V    ([ Colab Demo ](https://colab.research.google.com/drive/1IaZCCtq5m8vBBxrBLMCp6xB5U2j8ZNRc?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE VI   ([ Colab Demo ](https://colab.research.google.com/drive/14QdhifGitj4GK-QijRr1vj_dmGU2Pfh4?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - EC PROMETHEE ([ Colab Demo ](https://colab.research.google.com/drive/1YxXXuc2urj7_sUreZAROFldAhE0o6gio?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/math11214432))
 - PSI ([ Colab Demo ](https://colab.research.google.com/drive/1u9tN8cYl2mx6KK6yLW2oz6fuVoy8xcCI?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.matdes.2009.11.020))
+- MPSI ([ Colab Demo ](https://colab.research.google.com/drive/1zj2AS6W_VWmG5mYgY4b-dnCK0q3AG1-K?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/systems10060248))
 - Regime ([ Colab Demo ](https://colab.research.google.com/drive/1jcAcjAS92rxvE2urhc6HPixvzJ60HqEg?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/BF00221383))
 - ROV ([ Colab Demo ](https://colab.research.google.com/drive/1sQAPCem0pcS29uf6-n4TpncXMXNx9JDh?usp=sharing)) ( [ Paper ](https://doi.org/10.5267/j.dsl.2015.12.001))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
 - SPOTIS ([ Colab Demo ](https://colab.research.google.com/drive/1TyjDn-xwut3w6Rf0zMiugdwytwmGY_NE?usp=sharing)) ( [ Paper ](https://doi.org/10.23919/FUSION45008.2020.9190347))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2007.10.046))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
@@ -137,15 +139,15 @@
 - WSM, WPM, WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1HbLwXI4HkrmI-lsNzDtBOlCiwxfJltHi?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.acme.2013.07.006))
 - WISP, Simple WISP ([ Colab Demo ](https://colab.research.google.com/drive/1xyJf3aydLdVPqhWpNyVXXD8T4PsrX0du?usp=sharing)) ( [ Paper ](https://doi.org/10.1109/TEM.2021.3075783))
 - Fuzzy WSM, Fuzzy WPM, Fuzzy WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1PcN_PaXwPHawzCU05UiHE504SkgF6vQ2?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.15837/ijccc.2015.6.2078))
 
 4. Compare Methods:
 - Compare Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1RfLNEJjaHjtn3Lb2cfEDqS-iblaC4GQZ?usp=sharing))
 - Compare Fuzzy Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1pRO-E9xnk6DYEj_0DaEHUrUiCeIjmnXx?usp=sharing))
-- Compare Weigths & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/169hTJxP2APHrDA1h0fD1YEeu9s29wu0T?usp=sharing))
+- Compare Weights & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/169hTJxP2APHrDA1h0fD1YEeu9s29wu0T?usp=sharing))
 
 5. Advanced MCDA Methods:
 
 - [3MOAHP](https://github.com/Valdecy/Method_3MOAHP) - Inconsistency Reduction Technique for AHP and Fuzzy-AHP Methods
 - [pyMissingAHP](https://github.com/Valdecy/pyMissingAHP) - A Method to Infer AHP Missing Pairwise Comparisons
 - [ELECTRE-Tree](https://github.com/Valdecy/ELECTRE-Tree) - Algorithm to infer the ELECTRE Tri-B method parameters
 - [Ranking-Trees](https://github.com/Valdecy/Ranking-Trees) - Algorithm to infer the ELECTRE II, III, IV, and PROMETHEE I, II, III, IV method parameters
```

### Comparing `pyDecision-4.4.3/README.md` & `pyDecision-4.4.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **Regime**; **ROV** (Range Of Value); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **Fuzzy WASPAS**. 
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **Regime** (REGIonal Multicriteria Elimination); **ROV** (Range Of Value); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **Fuzzy WASPAS**. 
 
 pyDecision offers an array of features, including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
 
 ## Citation
 
 PEREIRA, V.; BASILIO, M.P.; SANTOS, C.H.T (2024). Enhancing Decision Analysis with a Large Language Model: pyDecision a Comprehensive Library of MCDA Methods in Python. arXiv. https://arxiv.org/abs/2404.06370
 
@@ -87,14 +87,15 @@
 - ELECTRE Tri-B ([ Colab Demo ](https://colab.research.google.com/drive/1hu0fJcxdBAiEDrVngmKQfpINpjTF-osE?usp=sharing)) ( [ Paper ](https://drive.google.com/file/d/1oWOI_sX3EEYdRbavoBTT7vUmPII1yPgE/view?usp=sharing))
 - FUCOM ([ Colab Demo ](https://colab.research.google.com/drive/1eWP3xf3-9iLLW_l_9JuAe6BEeoMsqzcL?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/sym10090393))
 - GRA ([ Colab Demo ](https://colab.research.google.com/drive/1aMMI0Cuo5kpzTDefqEwJhf0wWpBOP_JL?usp=sharing)) ( [ Paper ](https://uranos.ch/research/references/Julong_1989/10.1.1.678.3477.pdf))
 - IDOCRIW ([ Colab Demo ](https://colab.research.google.com/drive/1zt8uPFZGcHaSnpiT7tDnrDjvs0pK_7vS?usp=sharing)) ( [ Paper ](https://doi.org/10.1142/S0219622016500036))
 - MABAC ([ Colab Demo ](https://colab.research.google.com/drive/1BMqO-HnBXdcOZfZoULpx1H4MLPoUGucJ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2014.11.057))
 - MACBETH ([ Colab Demo ](https://colab.research.google.com/drive/1GqM9uPgbaWCGyj4l-XjkoifY2JJoVyf2?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0969-6016(94)90010-8))
 - MAIRCA ([ Colab Demo ](https://colab.research.google.com/drive/1gfqgrBAFGVygwm1j3lTjfy5wTsLgT_j5?usp=sharing)) ( [ Paper ](https://doi.org/10.1080/1331677X.2018.1506706))
+- MARA ([ Colab Demo ](https://colab.research.google.com/drive/1Ggg5e7TKVF_JN4yZRq9zThJO-PRBSI-N?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/systems10060248))
 - MARCOS ([ Colab Demo ](https://colab.research.google.com/drive/13MI2Qrakm5VzHN3r5O2RqggCzQwRxCs-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.cie.2019.106231))
 - MAUT ([ Colab Demo ](https://colab.research.google.com/drive/1qm3ARgQm68GUK2irGiCB-B49vnVHazB7?usp=sharing)) ( [ Paper ](https://doi.org/10.1017/CBO9781139174084))
 - MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1XE3AIzS84w-gw_1MEtV7xvkU1Gj_tRPd?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/sym13040525))
 - MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1FpKl0QAdwGgCVvLYsRHvMWhz7yOp17B5?usp=sharing)) ( [ Paper ](http://matwbn.icm.edu.pl/ksiazki/cc/cc35/cc35213.pdf))
 - Fuzzy MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1ydHzGeA8WBVY5Gyu8K7Oq6kofQ5XbK3P?usp=sharing)) ( [ Paper ](https://pdfs.semanticscholar.org/6d33/ca3f14c9ed44d23742fd4e9cf94cebcaf148.pdf))
 - MOOSRA ([ Colab Demo ](https://colab.research.google.com/drive/1KYyA4f3OsipPA5e63Ja4A0OGmHvNY6dj?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.15623/ijret.2014.0315105))
 - MULTIMOORA ([ Colab Demo ](https://colab.research.google.com/drive/1JAT8qqHPNoFfMV6a-CzF6BgRwtcUF3-e?usp=sharing)) ( [ Paper ](https://journals.vilniustech.lt/index.php/TEDE/article/view/5832/5078))
@@ -108,14 +109,15 @@
 ))
 - PROMETHEE IV   ([ Colab Demo ](https://colab.research.google.com/drive/1X2evE6pIf4F7qiKjt1fSU2PqT-NaA5sJ?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-319-11949-6_14))
 - PROMETHEE V    ([ Colab Demo ](https://colab.research.google.com/drive/1IaZCCtq5m8vBBxrBLMCp6xB5U2j8ZNRc?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE VI   ([ Colab Demo ](https://colab.research.google.com/drive/14QdhifGitj4GK-QijRr1vj_dmGU2Pfh4?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - EC PROMETHEE ([ Colab Demo ](https://colab.research.google.com/drive/1YxXXuc2urj7_sUreZAROFldAhE0o6gio?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/math11214432))
 - PSI ([ Colab Demo ](https://colab.research.google.com/drive/1u9tN8cYl2mx6KK6yLW2oz6fuVoy8xcCI?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.matdes.2009.11.020))
+- MPSI ([ Colab Demo ](https://colab.research.google.com/drive/1zj2AS6W_VWmG5mYgY4b-dnCK0q3AG1-K?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/systems10060248))
 - Regime ([ Colab Demo ](https://colab.research.google.com/drive/1jcAcjAS92rxvE2urhc6HPixvzJ60HqEg?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/BF00221383))
 - ROV ([ Colab Demo ](https://colab.research.google.com/drive/1sQAPCem0pcS29uf6-n4TpncXMXNx9JDh?usp=sharing)) ( [ Paper ](https://doi.org/10.5267/j.dsl.2015.12.001))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
 - SPOTIS ([ Colab Demo ](https://colab.research.google.com/drive/1TyjDn-xwut3w6Rf0zMiugdwytwmGY_NE?usp=sharing)) ( [ Paper ](https://doi.org/10.23919/FUSION45008.2020.9190347))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2007.10.046))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
@@ -126,15 +128,15 @@
 - WSM, WPM, WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1HbLwXI4HkrmI-lsNzDtBOlCiwxfJltHi?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.acme.2013.07.006))
 - WISP, Simple WISP ([ Colab Demo ](https://colab.research.google.com/drive/1xyJf3aydLdVPqhWpNyVXXD8T4PsrX0du?usp=sharing)) ( [ Paper ](https://doi.org/10.1109/TEM.2021.3075783))
 - Fuzzy WSM, Fuzzy WPM, Fuzzy WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1PcN_PaXwPHawzCU05UiHE504SkgF6vQ2?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.15837/ijccc.2015.6.2078))
 
 4. Compare Methods:
 - Compare Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1RfLNEJjaHjtn3Lb2cfEDqS-iblaC4GQZ?usp=sharing))
 - Compare Fuzzy Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1pRO-E9xnk6DYEj_0DaEHUrUiCeIjmnXx?usp=sharing))
-- Compare Weigths & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/169hTJxP2APHrDA1h0fD1YEeu9s29wu0T?usp=sharing))
+- Compare Weights & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/169hTJxP2APHrDA1h0fD1YEeu9s29wu0T?usp=sharing))
 
 5. Advanced MCDA Methods:
 
 - [3MOAHP](https://github.com/Valdecy/Method_3MOAHP) - Inconsistency Reduction Technique for AHP and Fuzzy-AHP Methods
 - [pyMissingAHP](https://github.com/Valdecy/pyMissingAHP) - A Method to Infer AHP Missing Pairwise Comparisons
 - [ELECTRE-Tree](https://github.com/Valdecy/ELECTRE-Tree) - Algorithm to infer the ELECTRE Tri-B method parameters
 - [Ranking-Trees](https://github.com/Valdecy/Ranking-Trees) - Algorithm to infer the ELECTRE II, III, IV, and PROMETHEE I, II, III, IV method parameters
```

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/__init__.py` & `pyDecision-4.4.5/pyDecision/algorithm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from .fuzzy_vikor   import fuzzy_vikor_method
 from .fuzzy_waspas  import fuzzy_waspas_method
 from .gra           import gra_method
 from .idocriw       import idocriw_method
 from .mabac         import mabac_method
 from .macbeth       import macbeth_method
 from .mairca        import mairca_method
+from .mara          import mara_method
 from .marcos        import marcos_method
 from .maut          import maut_method
 from .merec         import merec_method
 from .moora         import moora_method
 from .moosra        import moosra_method
 from .multimoora    import multimoora_method  
 from .ocra          import ocra_method
@@ -51,14 +52,15 @@
 from .p_iii         import promethee_iii
 from .p_iv          import promethee_iv
 from .p_v           import promethee_v
 from .p_vi          import promethee_vi
 from .p_xgaia       import promethee_gaia
 from .piv           import piv_method
 from .psi           import psi_method
+from .psi_m         import mpsi_method
 from .regime        import regime_method
 from .rov           import rov_method
 from .saw           import saw_method
 from .smart         import smart_method
 from .spotis        import spotis_method
 from .todim         import todim_method
 from .topsis        import topsis_method
```

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/ahp.py` & `pyDecision-4.4.5/pyDecision/algorithm/ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/aras.py` & `pyDecision-4.4.5/pyDecision/algorithm/aras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/borda.py` & `pyDecision-4.4.5/pyDecision/algorithm/borda.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/bwm.py` & `pyDecision-4.4.5/pyDecision/algorithm/bwm.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/bwm_s.py` & `pyDecision-4.4.5/pyDecision/algorithm/bwm_s.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/cilos.py` & `pyDecision-4.4.5/pyDecision/algorithm/cilos.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/cocoso.py` & `pyDecision-4.4.5/pyDecision/algorithm/cocoso.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/codas.py` & `pyDecision-4.4.5/pyDecision/algorithm/codas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/copeland.py` & `pyDecision-4.4.5/pyDecision/algorithm/copeland.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/copras.py` & `pyDecision-4.4.5/pyDecision/algorithm/copras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/cradis.py` & `pyDecision-4.4.5/pyDecision/algorithm/cradis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/critic.py` & `pyDecision-4.4.5/pyDecision/algorithm/critic.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/dematel.py` & `pyDecision-4.4.5/pyDecision/algorithm/dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/e_i.py` & `pyDecision-4.4.5/pyDecision/algorithm/e_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/e_i_s.py` & `pyDecision-4.4.5/pyDecision/algorithm/e_i_s.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/e_i_v.py` & `pyDecision-4.4.5/pyDecision/algorithm/e_i_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/e_ii.py` & `pyDecision-4.4.5/pyDecision/algorithm/e_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/e_iii.py` & `pyDecision-4.4.5/pyDecision/algorithm/e_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/e_iv.py` & `pyDecision-4.4.5/pyDecision/algorithm/e_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/e_tri_b.py` & `pyDecision-4.4.5/pyDecision/algorithm/e_tri_b.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/edas.py` & `pyDecision-4.4.5/pyDecision/algorithm/edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/entropy.py` & `pyDecision-4.4.5/pyDecision/algorithm/entropy.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/fucom.py` & `pyDecision-4.4.5/pyDecision/algorithm/fucom.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ###############################################################################
 
 # Required Libraries
 import numpy as np
 import re
 import warnings
 warnings.filterwarnings('ignore', message = 'delta_grad == 0.0. Check if the approximated')
+warnings.filterwarnings('ignore', message = 'Values in x were outside bounds during a minimize step, clipping to bounds')
 
 from scipy.optimize import minimize, Bounds, LinearConstraint
 
 ###############################################################################
 
 # Function: FUCOM (Full Consistency Method)
 def fucom_method(criteria_rank, criteria_priority, sort_criteria = True, verbose = True):
```

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/fuzzy_ahp.py` & `pyDecision-4.4.5/pyDecision/algorithm/fuzzy_ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/fuzzy_aras.py` & `pyDecision-4.4.5/pyDecision/algorithm/fuzzy_aras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/fuzzy_bwm.py` & `pyDecision-4.4.5/pyDecision/algorithm/fuzzy_bwm.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/fuzzy_copras.py` & `pyDecision-4.4.5/pyDecision/algorithm/fuzzy_copras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/fuzzy_dematel.py` & `pyDecision-4.4.5/pyDecision/algorithm/fuzzy_dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/fuzzy_edas.py` & `pyDecision-4.4.5/pyDecision/algorithm/fuzzy_edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/fuzzy_moora.py` & `pyDecision-4.4.5/pyDecision/algorithm/fuzzy_moora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/fuzzy_ocra.py` & `pyDecision-4.4.5/pyDecision/algorithm/fuzzy_ocra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/fuzzy_topsis.py` & `pyDecision-4.4.5/pyDecision/algorithm/fuzzy_topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/fuzzy_vikor.py` & `pyDecision-4.4.5/pyDecision/algorithm/fuzzy_vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/fuzzy_waspas.py` & `pyDecision-4.4.5/pyDecision/algorithm/fuzzy_waspas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/gra.py` & `pyDecision-4.4.5/pyDecision/algorithm/gra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/idocriw.py` & `pyDecision-4.4.5/pyDecision/algorithm/idocriw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/mabac.py` & `pyDecision-4.4.5/pyDecision/algorithm/mabac.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/macbeth.py` & `pyDecision-4.4.5/pyDecision/algorithm/macbeth.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/mairca.py` & `pyDecision-4.4.5/pyDecision/algorithm/mairca.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/marcos.py` & `pyDecision-4.4.5/pyDecision/algorithm/marcos.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/maut.py` & `pyDecision-4.4.5/pyDecision/algorithm/maut.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/merec.py` & `pyDecision-4.4.5/pyDecision/algorithm/merec.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/moora.py` & `pyDecision-4.4.5/pyDecision/algorithm/moora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/moosra.py` & `pyDecision-4.4.5/pyDecision/algorithm/moosra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/multimoora.py` & `pyDecision-4.4.5/pyDecision/algorithm/multimoora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/ocra.py` & `pyDecision-4.4.5/pyDecision/algorithm/ocra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/oreste.py` & `pyDecision-4.4.5/pyDecision/algorithm/oreste.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/p_ec.py` & `pyDecision-4.4.5/pyDecision/algorithm/p_ec.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/p_i.py` & `pyDecision-4.4.5/pyDecision/algorithm/p_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/p_ii.py` & `pyDecision-4.4.5/pyDecision/algorithm/p_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/p_iii.py` & `pyDecision-4.4.5/pyDecision/algorithm/p_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/p_iv.py` & `pyDecision-4.4.5/pyDecision/algorithm/p_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/p_v.py` & `pyDecision-4.4.5/pyDecision/algorithm/p_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/p_vi.py` & `pyDecision-4.4.5/pyDecision/algorithm/p_vi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/p_xgaia.py` & `pyDecision-4.4.5/pyDecision/algorithm/p_xgaia.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/piv.py` & `pyDecision-4.4.5/pyDecision/algorithm/piv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/psi.py` & `pyDecision-4.4.5/pyDecision/algorithm/psi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/regime.py` & `pyDecision-4.4.5/pyDecision/algorithm/regime.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         axes.set_ylim([ymin, ymax])
     else:
         axes.set_ylim([ymin-1, ymax+1])
     plt.axis('off')
     plt.show() 
     return
 
-# Function: Regime
+# Function: Regime (REGIonal Multicriteria Elimination)
 def regime_method(dataset, weights, criterion_type):
     X       = np.copy(dataset)/1.0
     weights = weights/np.sum(weights)
     g_ind   = np.zeros((X.shape[0], X.shape[0]))
     for i in range(0, g_ind.shape[0]):
         for k in range(0, g_ind.shape[0]):
             for j in range(0, X.shape[1]):
```

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/rov.py` & `pyDecision-4.4.5/pyDecision/algorithm/rov.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/saw.py` & `pyDecision-4.4.5/pyDecision/algorithm/saw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/smart.py` & `pyDecision-4.4.5/pyDecision/algorithm/smart.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/spotis.py` & `pyDecision-4.4.5/pyDecision/algorithm/spotis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/todim.py` & `pyDecision-4.4.5/pyDecision/algorithm/todim.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/topsis.py` & `pyDecision-4.4.5/pyDecision/algorithm/topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/vikor.py` & `pyDecision-4.4.5/pyDecision/algorithm/vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/waspas.py` & `pyDecision-4.4.5/pyDecision/algorithm/waspas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/wings.py` & `pyDecision-4.4.5/pyDecision/algorithm/wings.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/algorithm/wisp.py` & `pyDecision-4.4.5/pyDecision/algorithm/wisp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/compare/compare.py` & `pyDecision-4.4.5/pyDecision/compare/compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from pyDecision.algorithm.bwm_s        import simplified_bw_method
 from pyDecision.algorithm.cilos        import cilos_method
 from pyDecision.algorithm.critic       import critic_method
 from pyDecision.algorithm.entropy      import entropy_method
 from pyDecision.algorithm.fucom        import fucom_method
 from pyDecision.algorithm.idocriw      import idocriw_method
 from pyDecision.algorithm.merec        import merec_method
+from pyDecision.algorithm.psi_m        import mpsi_method
 
 #from pyDecision.algorithm.fuzzy_bwm    import fuzzy_bw_method
 
 from pyDecision.algorithm.aras         import aras_method
 from pyDecision.algorithm.borda        import borda_method
 from pyDecision.algorithm.cocoso       import cocoso_method
 from pyDecision.algorithm.codas        import codas_method
@@ -29,14 +30,15 @@
 from pyDecision.algorithm.copras       import copras_method
 from pyDecision.algorithm.cradis       import cradis_method
 from pyDecision.algorithm.edas         import edas_method
 from pyDecision.algorithm.gra          import gra_method
 from pyDecision.algorithm.mabac        import mabac_method
 from pyDecision.algorithm.macbeth      import macbeth_method
 from pyDecision.algorithm.mairca       import mairca_method
+from pyDecision.algorithm.mara         import mara_method
 from pyDecision.algorithm.marcos       import marcos_method
 from pyDecision.algorithm.maut         import maut_method
 from pyDecision.algorithm.moora        import moora_method
 from pyDecision.algorithm.moosra       import moosra_method
 from pyDecision.algorithm.multimoora   import multimoora_method
 from pyDecision.algorithm.ocra         import ocra_method
 from pyDecision.algorithm.oreste       import oreste_method
@@ -116,17 +118,17 @@
         for (i, j), z in np.ndenumerate(corr_df):
             plt.text(j, i, '{:0.2f}'.format(z), ha = 'center', va = 'center', fontsize = font_size, bbox = dict(boxstyle = 'round', facecolor = 'white', edgecolor = '0.1'))
     return corr_df
 
 ###############################################################################
 
 # Function: Compare Weights Crisp
-def compare_weigths(dataset, criterion_type, custom_methods = [], custom_weigths = [], methods_list = [], mic = [], lic = [], criteria_priority = [], criteria_rank = [], alpha = 0.5):
+def compare_weights(dataset, criterion_type, custom_methods = [], custom_weigths = [], methods_list = [], mic = [], lic = [], criteria_priority = [], criteria_rank = [], alpha = 0.5):
     if ('all' in methods_list):
-        methods_list = ['bwm', 'bwm_s', 'cilos', 'critic', 'entropy', 'fucom', 'idocriw', 'merec']
+        methods_list = ['bwm', 'bwm_s', 'cilos', 'critic', 'entropy', 'fucom', 'idocriw', 'merec', 'mpsi']
     if (len(custom_methods) > 0):
         methods_list = custom_methods + methods_list 
     X       = np.zeros((dataset.shape[1], len(methods_list)))
     j       = 0
     for i in range(0, len(custom_weigths)):
         X[:,j] = custom_weigths[i]
         j      = j + 1 
@@ -168,19 +170,24 @@
             j      = j + 1
             print('IDOCRIW: Done!')
         if (method == 'merec' or method == 'all'):
             w      = merec_method(dataset, criterion_type)
             X[:,j] = w
             j      = j + 1
             print('MEREC: Done!')
+        if (method == 'mpsi' or method == 'all'):
+            w      = mpsi_method(dataset, criterion_type)
+            X[:,j] = w
+            j      = j + 1
+            print('MPSI: Done!')
     X = pd.DataFrame(X, index = ['g'+str(i+1) for i in range(0, X.shape[0])], columns = methods_list)    
     return X
 
 # Function: Compare Weights Fuzzy
-#def compare_weigths_fuzzy(dataset, criterion_type, custom_methods = [], custom_weigths = [], methods_list = [], mic = [], lic = [], eps_penalty = 1):
+#def compare_weights_fuzzy(dataset, criterion_type, custom_methods = [], custom_weigths = [], methods_list = [], mic = [], lic = [], eps_penalty = 1):
     #if ('all' in methods_list):
         #methods_list = ['fuzzy_bwm']
     #if (len(custom_methods) > 0):
         #methods_list = custom_methods + methods_list 
     #for i in range(0, len(custom_weigths)):
         #X[:,j] = custom_weigths[i]
         #j      = j + 1 
@@ -192,15 +199,15 @@
             #j          = j + 1
             #print('Fuzzy BWM: Done!')
     #return
     
 # Function: Compare Ranks Crisp
 def compare_ranks_crisp(dataset, weights, criterion_type, utility_functions = [], custom_methods = [], custom_ranks = [], methods_list = [], L = 0.5, lmbd = 0.02, epsilon = 0.5, step_size = 1, teta = 1, strategy_coefficient = 0.5, Q = [], S = [], P = [], F = [], custom_sets = [], iterations = 1000, lambda_value = 0.5, alpha = 0.4, s_min = [], s_max = []):
     if ('all' in methods_list):
-        methods_list = ['aras', 'borda', 'cocoso', 'codas', 'copeland', 'copras', 'cradis', 'edas', 'gra', 'mabac', 'macbeth', 'mairca', 'marcos', 'maut', 'moora', 'moosra', 'multimoora', 'ocra', 'oreste', 'piv', 'promethee_ii', 'promethee_iv', 'ec_promethee', 'psi', 'rov', 'saw', 'spotis', 'todim', 'topsis', 'vikor', 'wsm', 'wpm', 'waspas', 'wisp', 'simple wisp']
+        methods_list = ['aras', 'borda', 'cocoso', 'codas', 'copeland', 'copras', 'cradis', 'edas', 'gra', 'mabac', 'macbeth', 'mairca', 'mara', 'marcos', 'maut', 'moora', 'moosra', 'multimoora', 'ocra', 'oreste', 'piv', 'promethee_ii', 'promethee_iv', 'ec_promethee', 'psi', 'rov', 'saw', 'spotis', 'todim', 'topsis', 'vikor', 'wsm', 'wpm', 'waspas', 'wisp', 'simple wisp']
     if (len(custom_methods) > 0):
         methods_list = custom_methods + methods_list 
     graph   = False
     verbose = False
     X       = np.zeros((dataset.shape[0], len(methods_list)))
     j       = 0
     for i in range(0, len(custom_ranks)):
@@ -264,14 +271,19 @@
             j      = j + 1
             print('MACBETH: Done!')
         if (method == 'mairca' or method == 'all'):
             rank   = mairca_method(dataset, weights, criterion_type, graph, verbose)
             X[:,j] = rank
             j      = j + 1
             print('MAIRCA: Done!')
+        if (method == 'mara' or method == 'all'):
+            rank   = mara_method(dataset, weights, criterion_type, graph, verbose)
+            X[:,j] = rank
+            j      = j + 1
+            print('MARA: Done!')
         if (method == 'marcos' or method == 'all'):
             rank   = marcos_method(dataset, weights, criterion_type, graph, verbose)
             X[:,j] = rank
             j      = j + 1
             print('MARCOS: Done!')
         if (method == 'maut' or method == 'all'):
             rank   = maut_method(dataset, weights, criterion_type, utility_functions, step_size, graph, verbose)
@@ -389,15 +401,15 @@
         if (method == 'simple wisp' or method == 'all'):
             w      = wisp_method(dataset, criterion_type, weights, simplified = True)
             X[:,j] = w
             j      = j + 1
             print('Simple WISP: Done!')
     ranked = np.zeros_like(X)
     for i in range(0, len(methods_list)):
-        if (methods_list[i] in ['borda', 'cradis', 'mairca', 'oreste', 'piv', 'spotis']):
+        if (methods_list[i] in ['borda', 'cradis', 'mairca', 'mara', 'oreste', 'piv', 'spotis']):
             ranked[:, i] = X.shape[0] + 1 - rankdata(-X[:, i], method = 'max')
         else:
             ranked[:, i] = X.shape[0] + 1 - rankdata(X[:, i], method = 'max')
     X      = pd.DataFrame(X, index = ['a'+str(i+1) for i in range(0, X.shape[0])], columns = methods_list)    
     ranked = pd.DataFrame(ranked, index = ['a'+str(i+1) for i in range(0, X.shape[0])], columns = methods_list)
     return X, ranked
```

### Comparing `pyDecision-4.4.3/pyDecision/util/LLM.py` & `pyDecision-4.4.5/pyDecision/util/LLM.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision/util/ga.py` & `pyDecision-4.4.5/pyDecision/util/ga.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.4.3/pyDecision.egg-info/PKG-INFO` & `pyDecision-4.4.5/pyDecision.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 4.4.3
+Version: 4.4.5
 Summary: A MCDA Library Incorporating a Large Language Model to Enhance Decision Analysis
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **Regime**; **ROV** (Range Of Value); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **Fuzzy WASPAS**. 
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **Simplified BWM**; **Fuzzy BWM**; **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **FUCOM** (Full Consistency Method); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARA** (Magnitude of the Area for the Ranking of Alternatives) ; **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PIV** (Proximity Indexed Value); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **EC PROMETHEE**; **Regime** (REGIonal Multicriteria Elimination); **ROV** (Range Of Value); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PSI** (Preference Selection Index); **MPSI** (Modified Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **Fuzzy WSM**; **WPM** (Weighted Product Model); **Fuzzy WPM**; **WASPAS** (Weighted Aggregates Sum Product Assessment); **WISP** (Integrated Simple Weighted Sum Product); **Simple WISP**; **Fuzzy WASPAS**. 
 
 pyDecision offers an array of features, including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
 
 ## Citation
 
 PEREIRA, V.; BASILIO, M.P.; SANTOS, C.H.T (2024). Enhancing Decision Analysis with a Large Language Model: pyDecision a Comprehensive Library of MCDA Methods in Python. arXiv. https://arxiv.org/abs/2404.06370
 
@@ -98,14 +98,15 @@
 - ELECTRE Tri-B ([ Colab Demo ](https://colab.research.google.com/drive/1hu0fJcxdBAiEDrVngmKQfpINpjTF-osE?usp=sharing)) ( [ Paper ](https://drive.google.com/file/d/1oWOI_sX3EEYdRbavoBTT7vUmPII1yPgE/view?usp=sharing))
 - FUCOM ([ Colab Demo ](https://colab.research.google.com/drive/1eWP3xf3-9iLLW_l_9JuAe6BEeoMsqzcL?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/sym10090393))
 - GRA ([ Colab Demo ](https://colab.research.google.com/drive/1aMMI0Cuo5kpzTDefqEwJhf0wWpBOP_JL?usp=sharing)) ( [ Paper ](https://uranos.ch/research/references/Julong_1989/10.1.1.678.3477.pdf))
 - IDOCRIW ([ Colab Demo ](https://colab.research.google.com/drive/1zt8uPFZGcHaSnpiT7tDnrDjvs0pK_7vS?usp=sharing)) ( [ Paper ](https://doi.org/10.1142/S0219622016500036))
 - MABAC ([ Colab Demo ](https://colab.research.google.com/drive/1BMqO-HnBXdcOZfZoULpx1H4MLPoUGucJ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2014.11.057))
 - MACBETH ([ Colab Demo ](https://colab.research.google.com/drive/1GqM9uPgbaWCGyj4l-XjkoifY2JJoVyf2?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0969-6016(94)90010-8))
 - MAIRCA ([ Colab Demo ](https://colab.research.google.com/drive/1gfqgrBAFGVygwm1j3lTjfy5wTsLgT_j5?usp=sharing)) ( [ Paper ](https://doi.org/10.1080/1331677X.2018.1506706))
+- MARA ([ Colab Demo ](https://colab.research.google.com/drive/1Ggg5e7TKVF_JN4yZRq9zThJO-PRBSI-N?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/systems10060248))
 - MARCOS ([ Colab Demo ](https://colab.research.google.com/drive/13MI2Qrakm5VzHN3r5O2RqggCzQwRxCs-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.cie.2019.106231))
 - MAUT ([ Colab Demo ](https://colab.research.google.com/drive/1qm3ARgQm68GUK2irGiCB-B49vnVHazB7?usp=sharing)) ( [ Paper ](https://doi.org/10.1017/CBO9781139174084))
 - MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1XE3AIzS84w-gw_1MEtV7xvkU1Gj_tRPd?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/sym13040525))
 - MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1FpKl0QAdwGgCVvLYsRHvMWhz7yOp17B5?usp=sharing)) ( [ Paper ](http://matwbn.icm.edu.pl/ksiazki/cc/cc35/cc35213.pdf))
 - Fuzzy MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1ydHzGeA8WBVY5Gyu8K7Oq6kofQ5XbK3P?usp=sharing)) ( [ Paper ](https://pdfs.semanticscholar.org/6d33/ca3f14c9ed44d23742fd4e9cf94cebcaf148.pdf))
 - MOOSRA ([ Colab Demo ](https://colab.research.google.com/drive/1KYyA4f3OsipPA5e63Ja4A0OGmHvNY6dj?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.15623/ijret.2014.0315105))
 - MULTIMOORA ([ Colab Demo ](https://colab.research.google.com/drive/1JAT8qqHPNoFfMV6a-CzF6BgRwtcUF3-e?usp=sharing)) ( [ Paper ](https://journals.vilniustech.lt/index.php/TEDE/article/view/5832/5078))
@@ -119,14 +120,15 @@
 ))
 - PROMETHEE IV   ([ Colab Demo ](https://colab.research.google.com/drive/1X2evE6pIf4F7qiKjt1fSU2PqT-NaA5sJ?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-319-11949-6_14))
 - PROMETHEE V    ([ Colab Demo ](https://colab.research.google.com/drive/1IaZCCtq5m8vBBxrBLMCp6xB5U2j8ZNRc?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE VI   ([ Colab Demo ](https://colab.research.google.com/drive/14QdhifGitj4GK-QijRr1vj_dmGU2Pfh4?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - EC PROMETHEE ([ Colab Demo ](https://colab.research.google.com/drive/1YxXXuc2urj7_sUreZAROFldAhE0o6gio?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/math11214432))
 - PSI ([ Colab Demo ](https://colab.research.google.com/drive/1u9tN8cYl2mx6KK6yLW2oz6fuVoy8xcCI?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.matdes.2009.11.020))
+- MPSI ([ Colab Demo ](https://colab.research.google.com/drive/1zj2AS6W_VWmG5mYgY4b-dnCK0q3AG1-K?usp=sharing)) ( [ Paper ](https://doi.org/10.3390/systems10060248))
 - Regime ([ Colab Demo ](https://colab.research.google.com/drive/1jcAcjAS92rxvE2urhc6HPixvzJ60HqEg?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/BF00221383))
 - ROV ([ Colab Demo ](https://colab.research.google.com/drive/1sQAPCem0pcS29uf6-n4TpncXMXNx9JDh?usp=sharing)) ( [ Paper ](https://doi.org/10.5267/j.dsl.2015.12.001))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
 - SPOTIS ([ Colab Demo ](https://colab.research.google.com/drive/1TyjDn-xwut3w6Rf0zMiugdwytwmGY_NE?usp=sharing)) ( [ Paper ](https://doi.org/10.23919/FUSION45008.2020.9190347))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2007.10.046))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
@@ -137,15 +139,15 @@
 - WSM, WPM, WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1HbLwXI4HkrmI-lsNzDtBOlCiwxfJltHi?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.acme.2013.07.006))
 - WISP, Simple WISP ([ Colab Demo ](https://colab.research.google.com/drive/1xyJf3aydLdVPqhWpNyVXXD8T4PsrX0du?usp=sharing)) ( [ Paper ](https://doi.org/10.1109/TEM.2021.3075783))
 - Fuzzy WSM, Fuzzy WPM, Fuzzy WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1PcN_PaXwPHawzCU05UiHE504SkgF6vQ2?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.15837/ijccc.2015.6.2078))
 
 4. Compare Methods:
 - Compare Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1RfLNEJjaHjtn3Lb2cfEDqS-iblaC4GQZ?usp=sharing))
 - Compare Fuzzy Ranks & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/1pRO-E9xnk6DYEj_0DaEHUrUiCeIjmnXx?usp=sharing))
-- Compare Weigths & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/169hTJxP2APHrDA1h0fD1YEeu9s29wu0T?usp=sharing))
+- Compare Weights & Ask chatGPT ([ Colab Demo ](https://colab.research.google.com/drive/169hTJxP2APHrDA1h0fD1YEeu9s29wu0T?usp=sharing))
 
 5. Advanced MCDA Methods:
 
 - [3MOAHP](https://github.com/Valdecy/Method_3MOAHP) - Inconsistency Reduction Technique for AHP and Fuzzy-AHP Methods
 - [pyMissingAHP](https://github.com/Valdecy/pyMissingAHP) - A Method to Infer AHP Missing Pairwise Comparisons
 - [ELECTRE-Tree](https://github.com/Valdecy/ELECTRE-Tree) - Algorithm to infer the ELECTRE Tri-B method parameters
 - [Ranking-Trees](https://github.com/Valdecy/Ranking-Trees) - Algorithm to infer the ELECTRE II, III, IV, and PROMETHEE I, II, III, IV method parameters
```

### Comparing `pyDecision-4.4.3/pyDecision.egg-info/SOURCES.txt` & `pyDecision-4.4.5/pyDecision.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 pyDecision/algorithm/fuzzy_vikor.py
 pyDecision/algorithm/fuzzy_waspas.py
 pyDecision/algorithm/gra.py
 pyDecision/algorithm/idocriw.py
 pyDecision/algorithm/mabac.py
 pyDecision/algorithm/macbeth.py
 pyDecision/algorithm/mairca.py
+pyDecision/algorithm/mara.py
 pyDecision/algorithm/marcos.py
 pyDecision/algorithm/maut.py
 pyDecision/algorithm/merec.py
 pyDecision/algorithm/moora.py
 pyDecision/algorithm/moosra.py
 pyDecision/algorithm/multimoora.py
 pyDecision/algorithm/ocra.py
@@ -61,14 +62,15 @@
 pyDecision/algorithm/p_iii.py
 pyDecision/algorithm/p_iv.py
 pyDecision/algorithm/p_v.py
 pyDecision/algorithm/p_vi.py
 pyDecision/algorithm/p_xgaia.py
 pyDecision/algorithm/piv.py
 pyDecision/algorithm/psi.py
+pyDecision/algorithm/psi_m.py
 pyDecision/algorithm/regime.py
 pyDecision/algorithm/rov.py
 pyDecision/algorithm/saw.py
 pyDecision/algorithm/smart.py
 pyDecision/algorithm/spotis.py
 pyDecision/algorithm/todim.py
 pyDecision/algorithm/topsis.py
```

### Comparing `pyDecision-4.4.3/setup.py` & `pyDecision-4.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyDecision',
-    version='4.4.3',
+    version='4.4.5',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyDecisions',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
```


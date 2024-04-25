# Comparing `tmp/buildz-0.5.1.tar.gz` & `tmp/buildz-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildz-0.5.1.tar", last modified: Tue Apr 23 20:20:42 2024, max compression
+gzip compressed data, was "buildz-0.5.2.tar", last modified: Thu Apr 25 17:53:28 2024, max compression
```

## Comparing `buildz-0.5.1.tar` & `buildz-0.5.2.tar`

### file list

```diff
@@ -1,159 +1,160 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.875188 buildz-0.5.1/
--rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.5.1/LICENSE
--rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2705 2024-04-23 20:20:42.875188 buildz-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     2290 2024-04-16 14:12:21.000000 buildz-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.417045 buildz-0.5.1/buildz/
--rw-rw-rw-   0        0        0      153 2024-04-16 14:04:54.000000 buildz-0.5.1/buildz/__init__.py
--rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.5.1/buildz/__main__.py
--rw-rw-rw-   0        0        0     2944 2024-04-13 11:54:47.000000 buildz-0.5.1/buildz/argx.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.432049 buildz-0.5.1/buildz/demo/
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.463809 buildz-0.5.1/buildz/demo/ioc/
--rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.5.1/buildz/demo/ioc/deal.py
--rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.5.1/buildz/demo/ioc/help.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.471001 buildz-0.5.1/buildz/demo/myers/
--rw-rw-rw-   0        0        0     2060 2024-04-07 18:54:16.000000 buildz-0.5.1/buildz/demo/myers/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.1/buildz/demo/myers/help.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.479509 buildz-0.5.1/buildz/demo/res/
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.486432 buildz-0.5.1/buildz/demo/res/conf/
--rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.5.1/buildz/demo/res/conf/ioc.js
--rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.5.1/buildz/demo/res/conf/main.js
--rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.5.1/buildz/demo/res/conf/myers.js
--rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.5.1/buildz/demo/res/conf/search.js
--rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.5.1/buildz/demo/res/conf/xf.js
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.486432 buildz-0.5.1/buildz/demo/res/help/
--rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.5.1/buildz/demo/res/help/default.js
--rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.5.1/buildz/demo/res/help/ioc.js
--rw-rw-rw-   0        0        0     1234 2024-04-07 18:48:53.000000 buildz-0.5.1/buildz/demo/res/help/myers.js
--rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.5.1/buildz/demo/res/help/search.js
--rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.5.1/buildz/demo/res/help/xf.js
--rw-rw-rw-   0        0        0      572 2024-04-16 13:25:08.000000 buildz-0.5.1/buildz/demo/res/test.js
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.495437 buildz-0.5.1/buildz/demo/search/
--rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.5.1/buildz/demo/search/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.1/buildz/demo/search/help.py
--rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.5.1/buildz/demo/test.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.495437 buildz-0.5.1/buildz/demo/xf/
--rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.5.1/buildz/demo/xf/deal.py
--rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.5.1/buildz/demo/xf/help.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.542601 buildz-0.5.1/buildz/fz/
--rw-rw-rw-   0        0        0      233 2024-04-05 04:01:25.000000 buildz-0.5.1/buildz/fz/__init__.py
--rw-rw-rw-   0        0        0     1387 2024-04-01 14:39:23.000000 buildz-0.5.1/buildz/fz/dirz.py
--rw-rw-rw-   0        0        0      629 2024-04-05 10:37:31.000000 buildz-0.5.1/buildz/fz/fio.py
--rw-rw-rw-   0        0        0     1729 2024-04-02 16:31:56.000000 buildz-0.5.1/buildz/fz/lsf.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.542601 buildz-0.5.1/buildz/ioc/
--rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.5.1/buildz/ioc/__init__.py
--rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.5.1/buildz/ioc/init.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.542601 buildz-0.5.1/buildz/ioc/ioc/
--rw-rw-rw-   0        0        0     2230 2024-04-23 14:05:55.000000 buildz-0.5.1/buildz/ioc/ioc/base.py
--rw-rw-rw-   0        0        0     6624 2024-04-23 19:13:22.000000 buildz-0.5.1/buildz/ioc/ioc/conf.py
--rw-rw-rw-   0        0        0    13056 2024-04-23 19:19:25.000000 buildz-0.5.1/buildz/ioc/ioc/confs.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.558233 buildz-0.5.1/buildz/ioc/ioc_deal/
--rw-rw-rw-   0        0        0     4828 2024-04-23 18:50:39.000000 buildz-0.5.1/buildz/ioc/ioc_deal/base.py
--rw-rw-rw-   0        0        0     1461 2024-04-02 15:35:04.000000 buildz-0.5.1/buildz/ioc/ioc_deal/call.py
--rw-rw-rw-   0        0        0     1239 2024-04-02 15:36:13.000000 buildz-0.5.1/buildz/ioc/ioc_deal/calls.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.570451 buildz-0.5.1/buildz/ioc/ioc_deal/conf/
--rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/call_defaults.js
--rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/call_lists.js
--rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/calls_defaults.js
--rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/calls_lists.js
--rw-rw-rw-   0        0        0      412 2024-04-23 19:15:09.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/deal_lists.js
--rw-rw-rw-   0        0        0     2197 2024-04-23 19:17:12.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/deals.js
--rw-rw-rw-   0        0        0      307 2024-04-01 14:20:24.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/env_lists.js
--rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/ioc_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/join_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/list_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/map_lists.js
--rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/mcall_defaults.js
--rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/mcall_lists.js
--rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
--rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/obj_defaults.js
--rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/obj_lists.js
--rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/obj_set_lists.js
--rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/ovar_lists.js
--rw-rw-rw-   0        0        0      488 2024-04-02 15:09:57.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/ref_lists.js
--rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/var_lists.js
--rw-rw-rw-   0        0        0        4 2024-04-23 10:50:44.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/xfile_defaults.js
--rw-rw-rw-   0        0        0      410 2024-04-23 10:50:04.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/xfile_lists.js
--rw-rw-rw-   0        0        0     1356 2024-04-23 19:35:52.000000 buildz-0.5.1/buildz/ioc/ioc_deal/deal.py
--rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.5.1/buildz/ioc/ioc_deal/demo.py
--rw-rw-rw-   0        0        0      824 2024-04-02 15:07:38.000000 buildz-0.5.1/buildz/ioc/ioc_deal/env.py
--rw-rw-rw-   0        0        0      950 2024-04-02 15:27:47.000000 buildz-0.5.1/buildz/ioc/ioc_deal/ioc.py
--rw-rw-rw-   0        0        0      928 2024-04-02 15:33:45.000000 buildz-0.5.1/buildz/ioc/ioc_deal/join.py
--rw-rw-rw-   0        0        0     1086 2024-04-02 17:38:51.000000 buildz-0.5.1/buildz/ioc/ioc_deal/list.py
--rw-rw-rw-   0        0        0     1017 2024-04-02 15:31:18.000000 buildz-0.5.1/buildz/ioc/ioc_deal/map.py
--rw-rw-rw-   0        0        0     1972 2024-04-02 15:18:24.000000 buildz-0.5.1/buildz/ioc/ioc_deal/mcall.py
--rw-rw-rw-   0        0        0     6130 2024-04-23 14:07:16.000000 buildz-0.5.1/buildz/ioc/ioc_deal/obj.py
--rw-rw-rw-   0        0        0     1558 2024-04-02 15:23:58.000000 buildz-0.5.1/buildz/ioc/ioc_deal/ovar.py
--rw-rw-rw-   0        0        0     1083 2024-04-02 15:10:34.000000 buildz-0.5.1/buildz/ioc/ioc_deal/ref.py
--rw-rw-rw-   0        0        0      702 2024-04-02 15:08:11.000000 buildz-0.5.1/buildz/ioc/ioc_deal/val.py
--rw-rw-rw-   0        0        0     1000 2024-04-02 15:26:02.000000 buildz-0.5.1/buildz/ioc/ioc_deal/var.py
--rw-rw-rw-   0        0        0     1078 2024-04-23 10:55:49.000000 buildz-0.5.1/buildz/ioc/ioc_deal/xfile.py
--rw-rw-rw-   0        0        0     1958 2024-04-23 08:58:52.000000 buildz-0.5.1/buildz/pyz.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.589591 buildz-0.5.1/buildz/tz/
--rw-rw-rw-   0        0        0      324 2024-04-16 14:03:17.000000 buildz-0.5.1/buildz/tz/__init__.py
--rw-rw-rw-   0        0        0     7543 2024-04-07 19:00:58.000000 buildz-0.5.1/buildz/tz/myers_diff.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.643635 buildz-0.5.1/buildz/xf/
--rw-rw-rw-   0        0        0      210 2024-04-16 13:29:45.000000 buildz-0.5.1/buildz/xf/__init__.py
--rw-rw-rw-   0        0        0       86 2024-04-13 11:53:05.000000 buildz-0.5.1/buildz/xf/__main__.py
--rw-rw-rw-   0        0        0      841 2024-04-01 17:49:56.000000 buildz-0.5.1/buildz/xf/file.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.668493 buildz-0.5.1/buildz/xf/loader/
--rw-rw-rw-   0        0        0     1782 2024-04-14 12:14:09.000000 buildz-0.5.1/buildz/xf/loader/base.py
--rw-rw-rw-   0        0        0     3647 2024-04-14 14:34:15.000000 buildz-0.5.1/buildz/xf/loader/buffer.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.719803 buildz-0.5.1/buildz/xf/loader/deal/
--rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.5.1/buildz/xf/loader/deal/listz.py
--rw-rw-rw-   0        0        0     2647 2024-04-14 14:34:45.000000 buildz-0.5.1/buildz/xf/loader/deal/lr.py
--rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.5.1/buildz/xf/loader/deal/lrval.py
--rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.5.1/buildz/xf/loader/deal/mapz.py
--rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.5.1/buildz/xf/loader/deal/nextz.py
--rw-rw-rw-   0        0        0     1242 2024-04-14 12:03:17.000000 buildz-0.5.1/buildz/xf/loader/deal/reval.py
--rw-rw-rw-   0        0        0     1134 2024-04-14 12:09:59.000000 buildz-0.5.1/buildz/xf/loader/deal/setz.py
--rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.5.1/buildz/xf/loader/deal/spc.py
--rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.5.1/buildz/xf/loader/deal/spt.py
--rw-rw-rw-   0        0        0     3180 2024-04-14 14:16:55.000000 buildz-0.5.1/buildz/xf/loader/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.1/buildz/xf/loader/exp.py
--rw-rw-rw-   0        0        0     1490 2024-04-12 12:01:04.000000 buildz-0.5.1/buildz/xf/loader/item.py
--rw-rw-rw-   0        0        0     2502 2024-04-16 13:18:40.000000 buildz-0.5.1/buildz/xf/loader/mg.py
--rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.1/buildz/xf/loader/pos.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.747437 buildz-0.5.1/buildz/xf/loaderz/
--rw-rw-rw-   0        0        0      746 2024-04-16 13:01:38.000000 buildz-0.5.1/buildz/xf/loaderz/base.py
--rw-rw-rw-   0        0        0     3126 2024-04-16 13:11:00.000000 buildz-0.5.1/buildz/xf/loaderz/buffer.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.811401 buildz-0.5.1/buildz/xf/loaderz/deal/
--rw-rw-rw-   0        0        0      533 2024-04-16 10:23:04.000000 buildz-0.5.1/buildz/xf/loaderz/deal/listz.py
--rw-rw-rw-   0        0        0     1787 2024-04-16 12:27:38.000000 buildz-0.5.1/buildz/xf/loaderz/deal/lr.py
--rw-rw-rw-   0        0        0     1094 2024-04-16 13:26:19.000000 buildz-0.5.1/buildz/xf/loaderz/deal/lrval.py
--rw-rw-rw-   0        0        0      699 2024-04-16 10:17:43.000000 buildz-0.5.1/buildz/xf/loaderz/deal/mapz.py
--rw-rw-rw-   0        0        0      452 2024-04-16 12:57:03.000000 buildz-0.5.1/buildz/xf/loaderz/deal/nextz.py
--rw-rw-rw-   0        0        0      691 2024-04-16 13:02:05.000000 buildz-0.5.1/buildz/xf/loaderz/deal/reval.py
--rw-rw-rw-   0        0        0      287 2024-04-16 10:07:28.000000 buildz-0.5.1/buildz/xf/loaderz/deal/setz.py
--rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.5.1/buildz/xf/loaderz/deal/spc.py
--rw-rw-rw-   0        0        0     1147 2024-04-16 12:27:46.000000 buildz-0.5.1/buildz/xf/loaderz/deal/spt.py
--rw-rw-rw-   0        0        0     3234 2024-04-16 13:34:36.000000 buildz-0.5.1/buildz/xf/loaderz/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.1/buildz/xf/loaderz/exp.py
--rw-rw-rw-   0        0        0     1911 2024-04-16 10:34:17.000000 buildz-0.5.1/buildz/xf/loaderz/item.py
--rw-rw-rw-   0        0        0     2838 2024-04-16 10:04:19.000000 buildz-0.5.1/buildz/xf/loaderz/mg.py
--rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.1/buildz/xf/loaderz/pos.py
--rw-rw-rw-   0        0        0     1687 2024-04-16 14:12:03.000000 buildz-0.5.1/buildz/xf/loaderz/test.py
--rw-rw-rw-   0        0        0     2009 2024-04-23 09:07:57.000000 buildz-0.5.1/buildz/xf/mapz.py
--rw-rw-rw-   0        0        0     2587 2024-04-16 13:17:27.000000 buildz-0.5.1/buildz/xf/read.py
--rw-rw-rw-   0        0        0     2587 2024-04-22 07:14:54.000000 buildz-0.5.1/buildz/xf/readz.py
--rw-rw-rw-   0        0        0     1999 2024-04-15 04:06:48.000000 buildz-0.5.1/buildz/xf/stack.py
--rw-rw-rw-   0        0        0     1230 2024-04-07 17:26:44.000000 buildz-0.5.1/buildz/xf/write.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.844079 buildz-0.5.1/buildz/xf/writer/
--rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.5.1/buildz/xf/writer/base.py
--rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.5.1/buildz/xf/writer/conf.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.875188 buildz-0.5.1/buildz/xf/writer/deal/
--rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.5.1/buildz/xf/writer/deal/jsonval.py
--rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.5.1/buildz/xf/writer/deal/listz.py
--rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.5.1/buildz/xf/writer/deal/mapz.py
--rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.5.1/buildz/xf/writer/deal/reval.py
--rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.5.1/buildz/xf/writer/deal/strz.py
--rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.5.1/buildz/xf/writer/itemz.py
--rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.5.1/buildz/xf/writer/mg.py
--rw-rw-rw-   0        0        0      597 2024-04-13 11:53:25.000000 buildz-0.5.1/buildz/xf/xargs.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.432049 buildz-0.5.1/buildz.egg-info/
--rw-rw-rw-   0        0        0     2705 2024-04-23 20:20:42.000000 buildz-0.5.1/buildz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3705 2024-04-23 20:20:42.000000 buildz-0.5.1/buildz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 20:20:42.000000 buildz-0.5.1/buildz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 20:20:42.000000 buildz-0.5.1/buildz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 20:20:42.875188 buildz-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      770 2024-04-23 20:17:27.000000 buildz-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:28.043943 buildz-0.5.2/
+-rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2705 2024-04-25 17:53:28.043943 buildz-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2290 2024-04-16 14:12:21.000000 buildz-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.968517 buildz-0.5.2/buildz/
+-rw-rw-rw-   0        0        0      153 2024-04-16 14:04:54.000000 buildz-0.5.2/buildz/__init__.py
+-rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.5.2/buildz/__main__.py
+-rw-rw-rw-   0        0        0     2944 2024-04-13 11:54:47.000000 buildz-0.5.2/buildz/argx.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.971522 buildz-0.5.2/buildz/demo/
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.972522 buildz-0.5.2/buildz/demo/ioc/
+-rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.5.2/buildz/demo/ioc/deal.py
+-rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.5.2/buildz/demo/ioc/help.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.973522 buildz-0.5.2/buildz/demo/myers/
+-rw-rw-rw-   0        0        0     2060 2024-04-07 18:54:16.000000 buildz-0.5.2/buildz/demo/myers/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.2/buildz/demo/myers/help.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.974522 buildz-0.5.2/buildz/demo/res/
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.976521 buildz-0.5.2/buildz/demo/res/conf/
+-rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.5.2/buildz/demo/res/conf/ioc.js
+-rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.5.2/buildz/demo/res/conf/main.js
+-rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.5.2/buildz/demo/res/conf/myers.js
+-rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.5.2/buildz/demo/res/conf/search.js
+-rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.5.2/buildz/demo/res/conf/xf.js
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.979522 buildz-0.5.2/buildz/demo/res/help/
+-rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.5.2/buildz/demo/res/help/default.js
+-rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.5.2/buildz/demo/res/help/ioc.js
+-rw-rw-rw-   0        0        0     1234 2024-04-07 18:48:53.000000 buildz-0.5.2/buildz/demo/res/help/myers.js
+-rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.5.2/buildz/demo/res/help/search.js
+-rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.5.2/buildz/demo/res/help/xf.js
+-rw-rw-rw-   0        0        0      572 2024-04-16 13:25:08.000000 buildz-0.5.2/buildz/demo/res/test.js
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.980522 buildz-0.5.2/buildz/demo/search/
+-rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.5.2/buildz/demo/search/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.2/buildz/demo/search/help.py
+-rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.5.2/buildz/demo/test.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.981521 buildz-0.5.2/buildz/demo/xf/
+-rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.5.2/buildz/demo/xf/deal.py
+-rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.5.2/buildz/demo/xf/help.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.984522 buildz-0.5.2/buildz/fz/
+-rw-rw-rw-   0        0        0      233 2024-04-05 04:01:25.000000 buildz-0.5.2/buildz/fz/__init__.py
+-rw-rw-rw-   0        0        0     1387 2024-04-01 14:39:23.000000 buildz-0.5.2/buildz/fz/dirz.py
+-rw-rw-rw-   0        0        0      629 2024-04-05 10:37:31.000000 buildz-0.5.2/buildz/fz/fio.py
+-rw-rw-rw-   0        0        0     1729 2024-04-02 16:31:56.000000 buildz-0.5.2/buildz/fz/lsf.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.986538 buildz-0.5.2/buildz/ioc/
+-rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.5.2/buildz/ioc/__init__.py
+-rw-rw-rw-   0        0        0       89 2024-04-25 13:59:49.000000 buildz-0.5.2/buildz/ioc/base.py
+-rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.5.2/buildz/ioc/init.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.988521 buildz-0.5.2/buildz/ioc/ioc/
+-rw-rw-rw-   0        0        0     2390 2024-04-25 13:41:08.000000 buildz-0.5.2/buildz/ioc/ioc/base.py
+-rw-rw-rw-   0        0        0     6918 2024-04-25 16:44:39.000000 buildz-0.5.2/buildz/ioc/ioc/conf.py
+-rw-rw-rw-   0        0        0    13518 2024-04-25 16:45:58.000000 buildz-0.5.2/buildz/ioc/ioc/confs.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.998942 buildz-0.5.2/buildz/ioc/ioc_deal/
+-rw-rw-rw-   0        0        0     5966 2024-04-25 13:56:41.000000 buildz-0.5.2/buildz/ioc/ioc_deal/base.py
+-rw-rw-rw-   0        0        0     1465 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/call.py
+-rw-rw-rw-   0        0        0     1243 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/calls.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:28.010942 buildz-0.5.2/buildz/ioc/ioc_deal/conf/
+-rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/call_defaults.js
+-rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/call_lists.js
+-rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/calls_defaults.js
+-rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/calls_lists.js
+-rw-rw-rw-   0        0        0      412 2024-04-23 19:15:09.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/deal_lists.js
+-rw-rw-rw-   0        0        0     2197 2024-04-23 19:17:12.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/deals.js
+-rw-rw-rw-   0        0        0      307 2024-04-01 14:20:24.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/env_lists.js
+-rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/ioc_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/join_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/list_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/map_lists.js
+-rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/mcall_defaults.js
+-rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/mcall_lists.js
+-rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
+-rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/obj_defaults.js
+-rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/obj_lists.js
+-rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/obj_set_lists.js
+-rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/ovar_lists.js
+-rw-rw-rw-   0        0        0      488 2024-04-02 15:09:57.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/ref_lists.js
+-rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/var_lists.js
+-rw-rw-rw-   0        0        0        4 2024-04-23 10:50:44.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/xfile_defaults.js
+-rw-rw-rw-   0        0        0      410 2024-04-23 10:50:04.000000 buildz-0.5.2/buildz/ioc/ioc_deal/conf/xfile_lists.js
+-rw-rw-rw-   0        0        0     2713 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/deal.py
+-rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.5.2/buildz/ioc/ioc_deal/demo.py
+-rw-rw-rw-   0        0        0      828 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/env.py
+-rw-rw-rw-   0        0        0      954 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/ioc.py
+-rw-rw-rw-   0        0        0      932 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/join.py
+-rw-rw-rw-   0        0        0     1090 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/list.py
+-rw-rw-rw-   0        0        0     1021 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/map.py
+-rw-rw-rw-   0        0        0     1976 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/mcall.py
+-rw-rw-rw-   0        0        0     6134 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/obj.py
+-rw-rw-rw-   0        0        0     1562 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/ovar.py
+-rw-rw-rw-   0        0        0     1087 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/ref.py
+-rw-rw-rw-   0        0        0      702 2024-04-02 15:08:11.000000 buildz-0.5.2/buildz/ioc/ioc_deal/val.py
+-rw-rw-rw-   0        0        0     1004 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/var.py
+-rw-rw-rw-   0        0        0     1082 2024-04-25 13:54:58.000000 buildz-0.5.2/buildz/ioc/ioc_deal/xfile.py
+-rw-rw-rw-   0        0        0     1958 2024-04-23 08:58:52.000000 buildz-0.5.2/buildz/pyz.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:28.011942 buildz-0.5.2/buildz/tz/
+-rw-rw-rw-   0        0        0      324 2024-04-16 14:03:17.000000 buildz-0.5.2/buildz/tz/__init__.py
+-rw-rw-rw-   0        0        0     7543 2024-04-07 19:00:58.000000 buildz-0.5.2/buildz/tz/myers_diff.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:28.017943 buildz-0.5.2/buildz/xf/
+-rw-rw-rw-   0        0        0      224 2024-04-25 14:33:04.000000 buildz-0.5.2/buildz/xf/__init__.py
+-rw-rw-rw-   0        0        0       86 2024-04-13 11:53:05.000000 buildz-0.5.2/buildz/xf/__main__.py
+-rw-rw-rw-   0        0        0      960 2024-04-25 14:34:17.000000 buildz-0.5.2/buildz/xf/file.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:28.020942 buildz-0.5.2/buildz/xf/loader/
+-rw-rw-rw-   0        0        0     1782 2024-04-14 12:14:09.000000 buildz-0.5.2/buildz/xf/loader/base.py
+-rw-rw-rw-   0        0        0     3647 2024-04-14 14:34:15.000000 buildz-0.5.2/buildz/xf/loader/buffer.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:28.026943 buildz-0.5.2/buildz/xf/loader/deal/
+-rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.5.2/buildz/xf/loader/deal/listz.py
+-rw-rw-rw-   0        0        0     2647 2024-04-14 14:34:45.000000 buildz-0.5.2/buildz/xf/loader/deal/lr.py
+-rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.5.2/buildz/xf/loader/deal/lrval.py
+-rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.5.2/buildz/xf/loader/deal/mapz.py
+-rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.5.2/buildz/xf/loader/deal/nextz.py
+-rw-rw-rw-   0        0        0     1242 2024-04-14 12:03:17.000000 buildz-0.5.2/buildz/xf/loader/deal/reval.py
+-rw-rw-rw-   0        0        0     1134 2024-04-14 12:09:59.000000 buildz-0.5.2/buildz/xf/loader/deal/setz.py
+-rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.5.2/buildz/xf/loader/deal/spc.py
+-rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.5.2/buildz/xf/loader/deal/spt.py
+-rw-rw-rw-   0        0        0     3180 2024-04-14 14:16:55.000000 buildz-0.5.2/buildz/xf/loader/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.2/buildz/xf/loader/exp.py
+-rw-rw-rw-   0        0        0     1490 2024-04-12 12:01:04.000000 buildz-0.5.2/buildz/xf/loader/item.py
+-rw-rw-rw-   0        0        0     2502 2024-04-16 13:18:40.000000 buildz-0.5.2/buildz/xf/loader/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.2/buildz/xf/loader/pos.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:28.030942 buildz-0.5.2/buildz/xf/loaderz/
+-rw-rw-rw-   0        0        0      746 2024-04-16 13:01:38.000000 buildz-0.5.2/buildz/xf/loaderz/base.py
+-rw-rw-rw-   0        0        0     3126 2024-04-16 13:11:00.000000 buildz-0.5.2/buildz/xf/loaderz/buffer.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:28.035943 buildz-0.5.2/buildz/xf/loaderz/deal/
+-rw-rw-rw-   0        0        0      533 2024-04-16 10:23:04.000000 buildz-0.5.2/buildz/xf/loaderz/deal/listz.py
+-rw-rw-rw-   0        0        0     1787 2024-04-16 12:27:38.000000 buildz-0.5.2/buildz/xf/loaderz/deal/lr.py
+-rw-rw-rw-   0        0        0     1094 2024-04-16 13:26:19.000000 buildz-0.5.2/buildz/xf/loaderz/deal/lrval.py
+-rw-rw-rw-   0        0        0      699 2024-04-16 10:17:43.000000 buildz-0.5.2/buildz/xf/loaderz/deal/mapz.py
+-rw-rw-rw-   0        0        0      452 2024-04-16 12:57:03.000000 buildz-0.5.2/buildz/xf/loaderz/deal/nextz.py
+-rw-rw-rw-   0        0        0      691 2024-04-16 13:02:05.000000 buildz-0.5.2/buildz/xf/loaderz/deal/reval.py
+-rw-rw-rw-   0        0        0      287 2024-04-16 10:07:28.000000 buildz-0.5.2/buildz/xf/loaderz/deal/setz.py
+-rw-rw-rw-   0        0        0      418 2024-04-25 17:42:03.000000 buildz-0.5.2/buildz/xf/loaderz/deal/spc.py
+-rw-rw-rw-   0        0        0     1147 2024-04-16 12:27:46.000000 buildz-0.5.2/buildz/xf/loaderz/deal/spt.py
+-rw-rw-rw-   0        0        0     3234 2024-04-16 13:34:36.000000 buildz-0.5.2/buildz/xf/loaderz/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.2/buildz/xf/loaderz/exp.py
+-rw-rw-rw-   0        0        0     1911 2024-04-16 10:34:17.000000 buildz-0.5.2/buildz/xf/loaderz/item.py
+-rw-rw-rw-   0        0        0     3032 2024-04-25 17:50:27.000000 buildz-0.5.2/buildz/xf/loaderz/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.2/buildz/xf/loaderz/pos.py
+-rw-rw-rw-   0        0        0     1751 2024-04-25 17:51:42.000000 buildz-0.5.2/buildz/xf/loaderz/test.py
+-rw-rw-rw-   0        0        0     2009 2024-04-23 09:07:57.000000 buildz-0.5.2/buildz/xf/mapz.py
+-rw-rw-rw-   0        0        0     2587 2024-04-16 13:17:27.000000 buildz-0.5.2/buildz/xf/read.py
+-rw-rw-rw-   0        0        0     2746 2024-04-25 17:36:02.000000 buildz-0.5.2/buildz/xf/readz.py
+-rw-rw-rw-   0        0        0     1999 2024-04-15 04:06:48.000000 buildz-0.5.2/buildz/xf/stack.py
+-rw-rw-rw-   0        0        0     1477 2024-04-25 14:36:40.000000 buildz-0.5.2/buildz/xf/write.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:28.039943 buildz-0.5.2/buildz/xf/writer/
+-rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.5.2/buildz/xf/writer/base.py
+-rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.5.2/buildz/xf/writer/conf.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:28.042942 buildz-0.5.2/buildz/xf/writer/deal/
+-rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.5.2/buildz/xf/writer/deal/jsonval.py
+-rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.5.2/buildz/xf/writer/deal/listz.py
+-rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.5.2/buildz/xf/writer/deal/mapz.py
+-rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.5.2/buildz/xf/writer/deal/reval.py
+-rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.5.2/buildz/xf/writer/deal/strz.py
+-rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.5.2/buildz/xf/writer/itemz.py
+-rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.5.2/buildz/xf/writer/mg.py
+-rw-rw-rw-   0        0        0      597 2024-04-13 11:53:25.000000 buildz-0.5.2/buildz/xf/xargs.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:53:27.970522 buildz-0.5.2/buildz.egg-info/
+-rw-rw-rw-   0        0        0     2705 2024-04-25 17:53:27.000000 buildz-0.5.2/buildz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3724 2024-04-25 17:53:27.000000 buildz-0.5.2/buildz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 17:53:27.000000 buildz-0.5.2/buildz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-25 17:53:27.000000 buildz-0.5.2/buildz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 17:53:28.043943 buildz-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      770 2024-04-25 17:52:05.000000 buildz-0.5.2/setup.py
```

### Comparing `buildz-0.5.1/LICENSE` & `buildz-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/PKG-INFO` & `buildz-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.5.1
+Version: 0.5.2
 Summary: a json-base file format's read and write code by python, and codes to read and product object from configure file in such format
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.5.1/README.md` & `buildz-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/argx.py` & `buildz-0.5.2/buildz/argx.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/demo/ioc/deal.py` & `buildz-0.5.2/buildz/demo/ioc/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/demo/ioc/help.py` & `buildz-0.5.2/buildz/demo/ioc/help.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/demo/myers/deal.py` & `buildz-0.5.2/buildz/demo/myers/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/demo/res/conf/main.js` & `buildz-0.5.2/buildz/demo/res/conf/main.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/demo/res/help/ioc.js` & `buildz-0.5.2/buildz/demo/res/help/ioc.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/demo/res/help/myers.js` & `buildz-0.5.2/buildz/demo/res/help/myers.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/demo/res/help/search.js` & `buildz-0.5.2/buildz/demo/res/help/search.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/demo/res/help/xf.js` & `buildz-0.5.2/buildz/demo/res/help/xf.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/demo/res/test.js` & `buildz-0.5.2/buildz/demo/res/test.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/demo/search/deal.py` & `buildz-0.5.2/buildz/demo/search/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/demo/test.py` & `buildz-0.5.2/buildz/demo/test.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/fz/dirz.py` & `buildz-0.5.2/buildz/fz/dirz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/fz/fio.py` & `buildz-0.5.2/buildz/fz/fio.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/fz/lsf.py` & `buildz-0.5.2/buildz/fz/lsf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/ioc/ioc/base.py` & `buildz-0.5.2/buildz/ioc/ioc/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,19 +43,23 @@
                 if pedt is None:
                     raise IOCError("unfind parend: "+pid)
                 pdt = pedt.data
                 if typez(pdt)!=dict:
                     raise IOCError("only dict can be a parent: "+pid)
                 data = dict(data)
                 self.update_maps(data, pdt, replace=0)
+                del data['parent']
         self.data = data
         self.sid = conf.id
         self.src = src
         self.conf = conf
         self.confs = conf.confs
         self.local = local
         if type is None:
             type = conf.confs.get_data_type(data, 0, conf.default_type())
         self.type = type
         self.info = info
+    def deal(self, remove = False):
+        return self.conf.get(self, src = self.src, info=self.info, remove = remove)
+
 
 pass
```

### Comparing `buildz-0.5.1/buildz/ioc/ioc/conf.py` & `buildz-0.5.2/buildz/ioc/ioc/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #coding=utf-8
 from buildz import xf, pyz
 from buildz.xf import g as xg
 import json
 from .base import Base, EncapeData,IOCError
+from builtins import id as _id
 class Conf(Base):
     """
         配置文件格式：
             {
                 id: 配置文件id，默认null
                 //在配置文件配置的环境变量
                 envs: {
@@ -80,14 +81,15 @@
         self.locals = self.map(xf.g(conf, locals=[]), self.confs.get_data_id)
         self.datas = self.map(xf.g(conf, datas=[]), self.confs.get_data_id)
         self.deals = self.map(xf.g(conf, deals = []), self.confs.get_deal_type)
         self.inits = xf.g(conf, inits = [])
         self._default_type = xf.g(conf, default_type = None)
         self.envs = xf.g(conf, envs = {})
         self.confs.flush_env(self.envs)
+        self.confs.update_env(self.envs)
         for _type in list(self.deals.keys()):
             conf = self.deals[_type]
             if type(conf) in [list, tuple]:
                 maps = {}
                 maps['type'] = conf[0]
                 maps['build'] = conf[1]
                 arr = conf[2:]
@@ -110,25 +112,15 @@
             return
         self.mark_init = True
         for id in self.inits:
             self.get(id)
     def get_env(self, id, search_confs = True):
         if self.confs.global_env and search_confs:
             return self.confs.get_env(id, self.id)
-        ids = self.confs.env_ids(id)
-        envs = self.envs
-        find = None
-        for id in ids:
-            if type(envs)!=dict:
-                envs = None
-                break
-            if id not in envs:
-                envs = None
-                break
-            envs = envs[id]
+        envs = self.confs.get_env_maps(id, self.envs)
         if envs is not None:
             return envs
         if not search_confs:
             return None
         return self.confs.get_env(id, self.id)
     def set_deal(self, type, fc):
         self.deals[type] = fc
@@ -141,34 +133,46 @@
         if not search_confs:
             return None
         return self.confs.get_deal(type, self.id)
     def get_data(self, id, local = True, search_confs = True, src = None, info = None):
         self.do_init()
         if id in self.datas:
             obj = self.datas[id]
-            return EncapeData(obj, self, local = False, src=src, info = info)
+            edata = EncapeData(obj, self, local = False, src=src, info = info)
+            if _id(obj) != _id(edata.data):
+                # 有parent，做了填充，用填充后的替换
+                self.datas[id] = edata.data
+            return edata
         if not local:
             return None
         if id in self.locals:
             obj = self.locals[id]
-            return EncapeData(obj, self, local = True, src=src, info = info)
+            edata = EncapeData(obj, self, local = True, src=src, info = info)
+            if _id(obj) != _id(edata.data):
+                # 有parent，做了填充，用填充后的替换
+                self.locals[id] = edata.data
+            return edata
         if not search_confs:
             return None
         return self.confs.get_data(id, self.id, src=src, info = info)
     def get(self, *args, **maps):
         return self.get_obj(*args, **maps)
     def default_type(self):
         if self._default_type is None:
             return self.confs.default_type
         return self._default_type
     def get_obj(self, id, src = None, info=None, remove = False):
         """
             根据data id获取data对象，处理逻辑：根据data id查配置，根据配置的type查deal，返回deal处理过的配置
         """
-        conf = self.get_data(id, src = src, info = info)
+        self.do_init()
+        if type(id) == EncapeData:
+            conf = id
+        else:
+            conf = self.get_data(id, src = src, info = info)
         if conf is None:
             raise IOCError(f"can't find conf of {id}")
             return None
         deal = self.get_deal(conf.type)
         if deal is None:
             raise IOCError(f"can't find deal of {id}, type = {conf.type}")
             return None
```

### Comparing `buildz-0.5.1/buildz/ioc/ioc/confs.py` & `buildz-0.5.2/buildz/ioc/ioc/confs.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,47 +51,53 @@
     def get_env_sys(self, id, sid=None):
         sysdt = os.getenv(id)
         return sysdt
     def build_env_args_xf(self):
         data = xf.args()
         env = data['env']
         self.envs_args = env
+        self.flush_env(self.envs_args)
     def build_env_args_buildz(self):
         args, maps = argx.fetch()
         e = xf.get(maps, e = [])
         env = xf.get(maps, env=[])
         env += e
         env = [k.split("=") for k in env]
         env = {k[0]:"=".join(k[1:]) for k in env}
         self.envs_args = env
+        self.flush_env(self.envs_args)
+    def build_env_args(self):
+        if self.args_type == "xf":
+            self.build_env_args_xf()
+        else:
+            self.build_env_args_buildz()
     def get_env_args(self, id, sid=None):
-        if self.envs_args is not None:
-            if self.args_type == "xf":
-                self.build_env_args_xf()
-            else:
-                self.build_env_args_buildz()
-        return xf.get(self.envs_args, id)
+        if self.envs_args is None:
+            self.build_env_args()
+        return self.get_env_maps(id, self.envs_args)
     def get_env_local(self, id, sid=None):
         if sid is not None and not self.global_env:
             val = self.confs[sid].get_env(id, False)
             if val is not None:
                 return val
         return None
-    def get_env_conf(self, id, sid=None):
+    def get_env_maps(self, id, maps):
         ids = self.env_ids(id)
-        envs = self.envs
+        envs = maps
         for id in ids:
             if type(envs)!=dict:
                 envs = None
                 break
             if id not in envs:
                 envs = None
                 break 
             envs = envs[id]
         return envs
+    def get_env_conf(self, id, sid=None):
+        return self.get_env_maps(id, self.envs)
     def get_env(self, id, sid=None):
         for key in self.env_orders:
             fc = self.env_fcs[key]
             obj = fc(id, sid)
             if obj is not None:
                 return obj
         return None
@@ -113,14 +119,16 @@
                 break 
             envs = envs[id]
         return envs
     def set_env(self, id, val):
         obj = {id:val}
         self.flush_env(obj)
         self.update_maps(self.envs, obj)
+    def update_env(self, obj):
+        self.update_maps(self.envs, obj)
     def set_deal(self, type, fc):
         self.deals[type] = fc
     def init_fp(self, fp):
         conf = self.loads(xf.fread(fp))
         self.init(conf, self.loads)
     def by_json(self):
         self.by('json')
@@ -201,15 +209,15 @@
         self.global_deal = xf.g(conf, global_deal = True)
         self.data_key_id = xf.g(conf, data_key_id = 'id')
         self.data_key_type = xf.g(conf, data_key_type = 'type')
         self.data_index_id = xf.g(conf, data_index_id = [0,0])
         self.data_index_type = xf.g(conf, data_index_type = [0,1])
         self.deal_key_type = xf.g(conf, deal_key_type = 'type')
         self.deal_index_type = xf.g(conf, deal_index_type = 0)
-        self.env_orders = xf.g(conf, env_orders = ['args', 'sys', 'local', 'conf'])
+        self.env_orders = xf.g(conf, env_orders = ['sys', 'local', 'conf'])
         self.env_fcs = {
             'args': self.get_env_args,
             'sys': self.get_env_sys,
             'local': self.get_env_local,
             'conf': self.get_env_conf
         }
         self.args_type = xf.g(conf, args_type = "xf")
@@ -217,14 +225,16 @@
         self.conf = conf
         self.node = ConfsNode()
         self.confs = {}
         self.deals = {}
         self.envs = {}
         self.envs_args = None
         self.mark_init = False
+        if 'args' in self.env_orders:
+            self.build_env_args()
     def do_init(self):
         if self.mark_init:
             return
         self.mark_init = True
         for id in self.confs:
             self.confs[id].do_init()
     def get_deal_type(self, obj):
@@ -235,14 +245,15 @@
         if type(obj)==dict:
             return obj[self.data_key_id]
         obj = obj[self.data_index_id[0]]
         if type(obj) in [list, tuple]:
             obj = obj[self.data_index_id[1]]
         return obj
     def get_data_type(self, obj, type_first = 1, default = None):
+        self.do_init()
         if type(obj)==dict:
             if self.data_key_type not in obj:
                 return default
             return obj[self.data_key_type]
         obj = obj[self.data_index_type[0]]
         if type(obj) in [list, tuple]:
             return obj[self.data_index_type[1]]
@@ -310,15 +321,18 @@
     def remove(self, *a,**b):
         return self.get_obj(*a, **b, remove=True)
     def get_obj(self, id, sid = None, src = None, info = None, remove = False):
         """
             根据data id获取data对象，处理逻辑：根据data id查配置，根据配置的type查deal，返回deal处理过的配置
         """
         self.do_init()
-        conf = self.get_data(id, sid, src=src, info = info)
+        if type(id) == EncapeData:
+            conf = id
+        else:
+            conf = self.get_data(id, sid, src=src, info = info)
         if conf is None:
             raise IOCError(f"confs: can't find conf of {id}")
             return None
         deal = self.get_deal(conf.type, sid)
         if deal is None:
             raise IOCError(f"confs: can't find deal of {id}, type = {conf.type}")
             return None
```

### Comparing `buildz-0.5.1/buildz/ioc/ioc_deal/base.py` & `buildz-0.5.2/buildz/ioc/ioc_deal/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -113,19 +113,46 @@
             else:
                 maps[key] = _maps
             cnt +=1
         return maps
 
 pass
 
-
 class BaseDeal(Base):
-    def init(self, name = "BaseDeal", fp_lists = None, fp_defaults = None, df_fp_lists=None, df_fp_defaults=None):
-        self.singles = {}
-        self.sources = {}
+    """
+        基础处理类，加了一些方便处理的方法，自己写的处理可以不用继承这个
+        自己实现的处理类，要实现两个方法：__call__(self, edata:EncapeData)和remove(self, edata:EncapeData)
+        其中remove可以只写个空方法
+    """
+    def get_obj(self, data, conf, src = None, info = None):
+        if type(data) not in [list, dict, tuple]:
+            i = conf.confs.data_index_type[0]
+            data = [conf.default_type(), data]
+            if i != 0:
+                data.reverse()
+        _type = conf.confs.get_data_type(data, 1, conf.default_type())
+        edata = EncapeData(data, conf, local=True, type=_type, src = src, info = info)
+        return edata()
+        deal = conf.get_deal(edata.type)
+        if deal is None:
+            return None
+        return deal(edata)
+    def deal(self, edata:EncapeData):
+        """
+        """
+        return None
+    def remove(self, edata:EncapeData):
+        return None
+
+pass
+class FormatDeal(BaseDeal):
+    """
+        格式化处理类，加了自动装填，但感觉不太好用（一方面忘记写注释，写的时间久了，不知道要怎么用了，另一方面不好扩展，再一方面自动填充要消耗时间））
+    """
+    def init(self, name = "FormatDeal", fp_lists = None, fp_defaults = None, df_fp_lists=None, df_fp_defaults=None):
         if fp_lists is None:
             fp_lists = df_fp_lists
         if fp_defaults is None:
             fp_defaults = df_fp_defaults
         lists = []
         defaults = {}
         if fp_lists  is not None:
@@ -141,17 +168,14 @@
         if type(data) not in [list, dict, tuple]:
             i = conf.confs.data_index_type[0]
             data = [conf.default_type(), data]
             if i != 0:
                 data.reverse()
         _type = conf.confs.get_data_type(data, 1, conf.default_type())
         edata = EncapeData(data, conf, local=True, type=_type, src = src, info = info)
+        return edata()
         deal = conf.get_deal(edata.type)
         if deal is None:
             return None
         return deal(edata)
-    def deal(self, edata:EncapeData):
-        return None
-    def remove(self, edata:EncapeData):
-        return None
 
 pass
```

### Comparing `buildz-0.5.1/buildz/ioc/ioc_deal/call.py` & `buildz-0.5.2/buildz/ioc/ioc_deal/call.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 from ..ioc.base import Base, EncapeData
-from .base import FormatData,BaseDeal
+from .base import FormatData,FormatDeal
 from buildz import xf, pyz
 import os
 dp = os.path.dirname(__file__)
 join = os.path.join
-class CallDeal(BaseDeal):
+class CallDeal(FormatDeal):
     """
     函数调用call:
         {
             id:id
             type:call
             method: import路径+"."+方法名
             args: [item_conf, ...]
```

### Comparing `buildz-0.5.1/buildz/ioc/ioc_deal/calls.py` & `buildz-0.5.2/buildz/ioc/ioc_deal/calls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 from ..ioc.base import Base, EncapeData
-from .base import FormatData,BaseDeal
+from .base import FormatData,FormatDeal
 from buildz import xf, pyz
 import os
 dp = os.path.dirname(__file__)
 join = os.path.join
-class CallsDeal(BaseDeal):
+class CallsDeal(FormatDeal):
     """
     函数调用序列calls:
         {
             id:id
             type:calls
             calls: [
                 item_conf,
```

### Comparing `buildz-0.5.1/buildz/ioc/ioc_deal/conf/deals.js` & `buildz-0.5.2/buildz/ioc/ioc_deal/conf/deals.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/ioc/ioc_deal/conf/obj_lists.js` & `buildz-0.5.2/buildz/ioc/ioc_deal/conf/obj_lists.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/ioc/ioc_deal/deal.py` & `buildz-0.5.2/buildz/ioc/ioc_deal/xfile.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-#coding=utf-8
-from ..ioc.base import Base, EncapeData,IOCError
-from .base import FormatData,BaseDeal
+#
+from ..ioc.base import Base, EncapeData
+from .base import FormatData,FormatDeal
 from buildz import xf, pyz
 import os
 dp = os.path.dirname(__file__)
 join = os.path.join
-class DealDeal(BaseDeal):
+class XfileDeal(FormatDeal):
     """
-        // 调用后会注册到conf的deal上，用于扩展deals配置
-        deal字段deal:
-            {
-                id:id
-                type: deal
-                target: type
-                source: id # 要求source实现了方法__call__(self, edata:EncapeData)
-            }
-        简写:
-            [[id, deal], target, source]
-            [deal, target, source]
-        例:
-            [deal, target, source] //
+    配置文件载入xfile/xf:
+        {
+            id:id
+            type:xfile
+            filepath: fp 
+            # or fp: fp
+        }
+    简写:
+        [[id, xfile], fp]
+        [xfile, fp]
+        [xf, fp]
+    例:
+        [xfile, test.js]
     """
-    def init(self, fp_lists=None, fp_defaults=None):
-        super().init("DealDeal", fp_lists, fp_defaults, join(dp, "conf", "deal_lists.js"), None)
+    def init(self, fp_lists = None, fp_defaults = None):
+        self.singles = {}
+        self.sources = {}
+        super().init("XfileDeal", fp_lists, fp_defaults, 
+            join(dp, "conf", "xfile_lists.js"),
+            join(dp, "conf", "xfile_defaults.js"))
     def deal(self, edata:EncapeData):
+        sid = edata.sid
         data = edata.data
-        source = xf.g(data, source=None)
-        if source is None:
-            raise IOCError("not source in dealdeal")
-        target = xf.g(data, target=None)
-        if target is None:
-            raise IOCError("not target in dealdeal")
-        obj = edata.conf.get(source)
-        if obj is None:
-            raise IOCError("source object not found in dealdeal")
-        edata.conf.set_deal(target, obj)
-        return None
+        conf = edata.conf
+        data = self.format(data)
+        fp = xf.g(data, filepath=None)
+        if fp is None:
+            fp = xf.g(data, fp = fp)
+        rst = xf.loads(xf.fread(fp))
+        return rst
 
 pass
```

### Comparing `buildz-0.5.1/buildz/ioc/ioc_deal/env.py` & `buildz-0.5.2/buildz/ioc/ioc_deal/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 from ..ioc.base import Base, EncapeData
-from .base import FormatData,BaseDeal
+from .base import FormatData,FormatDeal
 from buildz import xf, pyz
 import os
 dp = os.path.dirname(__file__)
 join = os.path.join
-class EnvDeal(BaseDeal):
+class EnvDeal(FormatDeal):
     """
         环境变量env:
             {
                 id: id
                 type: env
                 key: 环境变量key
             }
```

### Comparing `buildz-0.5.1/buildz/ioc/ioc_deal/ioc.py` & `buildz-0.5.2/buildz/ioc/ioc_deal/ioc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #coding=utf-8
 from ..ioc.base import Base, EncapeData
-from .base import FormatData,BaseDeal
+from .base import FormatData,FormatDeal
 from buildz import xf, pyz
 import os
 dp = os.path.dirname(__file__)
 join = os.path.join
-class IOCObjectDeal(BaseDeal):
+class IOCObjectDeal(FormatDeal):
     """
         ioc字段ioc:
             {
                 id:id
                 type: ioc
                 //default conf
                 key: string = conf, confs, sid
```

### Comparing `buildz-0.5.1/buildz/ioc/ioc_deal/join.py` & `buildz-0.5.2/buildz/ioc/ioc_deal/join.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #coding=utf-8
 from ..ioc.base import Base, EncapeData
-from .base import FormatData,BaseDeal
+from .base import FormatData,FormatDeal
 from buildz import xf, pyz
 import os
 dp = os.path.dirname(__file__)
 join = os.path.join
-class JoinDeal(BaseDeal):
+class JoinDeal(FormatDeal):
     """
     文件路径合并join:
         {
             id:id
             type: join
             data: [...]
         }
```

### Comparing `buildz-0.5.1/buildz/ioc/ioc_deal/list.py` & `buildz-0.5.2/buildz/ioc/ioc_deal/list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #coding=utf-8
 from ..ioc.base import Base, EncapeData
-from .base import FormatData,BaseDeal
+from .base import FormatData,FormatDeal
 from buildz import xf, pyz
 import os
 dp = os.path.dirname(__file__)
 join = os.path.join
-class ListDeal(BaseDeal):
+class ListDeal(FormatDeal):
     """
         list:
             {
                 id: id
                 type: list
                 data: [
                     item_conf,
```

### Comparing `buildz-0.5.1/buildz/ioc/ioc_deal/map.py` & `buildz-0.5.2/buildz/ioc/ioc_deal/map.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #coding=utf-8
 from ..ioc.base import Base, EncapeData
-from .base import FormatData,BaseDeal
+from .base import FormatData,FormatDeal
 from buildz import xf, pyz
 import os
 dp = os.path.dirname(__file__)
 join = os.path.join
-class MapDeal(BaseDeal):
+class MapDeal(FormatDeal):
     """
     map:
         {
             id:id
             type:map
             data: {
                 key1: item_conf,
```

### Comparing `buildz-0.5.1/buildz/ioc/ioc_deal/mcall.py` & `buildz-0.5.2/buildz/ioc/ioc_deal/mcall.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 from ..ioc.base import Base, EncapeData
-from .base import FormatData,BaseDeal
+from .base import FormatData,FormatDeal
 from buildz import xf, pyz
 import os
 dp = os.path.dirname(__file__)
 join = os.path.join
-class MethodCallDeal(BaseDeal):
+class MethodCallDeal(FormatDeal):
     """
     对象方法调用:
         {
             id: id
             type: mcall
             source: 对象id
             method: 调用方法
```

### Comparing `buildz-0.5.1/buildz/ioc/ioc_deal/obj.py` & `buildz-0.5.2/buildz/ioc/ioc_deal/obj.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 from ..ioc.base import Base, EncapeData,IOCError
-from .base import FormatData,BaseDeal
+from .base import FormatData,FormatDeal
 from buildz import xf, pyz
 import os
 dp = os.path.dirname(__file__)
 join = os.path.join
-class ObjectDeal(BaseDeal):
+class ObjectDeal(FormatDeal):
     """
         对象object:
             {
                 id: id
                 type: object
                 source: 导入路径+调用方法/类
                 single: 1 //是否单例，默认是，
```

### Comparing `buildz-0.5.1/buildz/ioc/ioc_deal/ovar.py` & `buildz-0.5.2/buildz/ioc/ioc_deal/ovar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 from ..ioc.base import Base, EncapeData
-from .base import FormatData,BaseDeal
+from .base import FormatData,FormatDeal
 from buildz import xf, pyz
 import os
 dp = os.path.dirname(__file__)
 join = os.path.join
-class ObjectVarDeal(BaseDeal):
+class ObjectVarDeal(FormatDeal):
     """
         对象变量ovar:
             {
                 id:id
                 type: ovar
                 source: string
                 key: string
```

### Comparing `buildz-0.5.1/buildz/ioc/ioc_deal/ref.py` & `buildz-0.5.2/buildz/ioc/ioc_deal/ref.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #coding=utf-8
 from ..ioc.base import Base, EncapeData
-from .base import FormatData,BaseDeal
+from .base import FormatData,FormatDeal
 from buildz import xf, pyz
 import os
 dp = os.path.dirname(__file__)
 join = os.path.join
-class RefDeal(BaseDeal):
+class RefDeal(FormatDeal):
     """
         引用ref:
             {
                 id: id
                 type: ref
                 key: 引导数据id
                 info: item_conf, 额外的引用信息, 默认null
```

### Comparing `buildz-0.5.1/buildz/ioc/ioc_deal/val.py` & `buildz-0.5.2/buildz/ioc/ioc_deal/val.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/ioc/ioc_deal/var.py` & `buildz-0.5.2/buildz/ioc/ioc_deal/var.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 from ..ioc.base import Base, EncapeData
-from .base import FormatData,BaseDeal
+from .base import FormatData,FormatDeal
 from buildz import xf, pyz
 import os
 dp = os.path.dirname(__file__)
 join = os.path.join
-class VarDeal(BaseDeal):
+class VarDeal(FormatDeal):
     """
         代码变量var:
             {
                 id:id
                 type: var
                 key: string
             }
```

### Comparing `buildz-0.5.1/buildz/pyz.py` & `buildz-0.5.2/buildz/pyz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/tz/myers_diff.py` & `buildz-0.5.2/buildz/tz/myers_diff.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/file.py` & `buildz-0.5.2/buildz/xf/file.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,8 +34,14 @@
     return decode(s, coding)
 
 pass
 def fread_c(filepath, coding = 'utf-8'):
     s = bread(filepath)
     return decode_c(s, coding)
 
-pass
+pass
+
+def fwrite(filepath, content, mode = 'w'):
+    with open(filepath, mode) as f:
+        f.write(content)
+
+pass
```

### Comparing `buildz-0.5.1/buildz/xf/loader/base.py` & `buildz-0.5.2/buildz/xf/loader/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loader/buffer.py` & `buildz-0.5.2/buildz/xf/loader/buffer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loader/deal/listz.py` & `buildz-0.5.2/buildz/xf/loader/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loader/deal/lr.py` & `buildz-0.5.2/buildz/xf/loader/deal/lr.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loader/deal/lrval.py` & `buildz-0.5.2/buildz/xf/loader/deal/lrval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loader/deal/mapz.py` & `buildz-0.5.2/buildz/xf/loader/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loader/deal/nextz.py` & `buildz-0.5.2/buildz/xf/loader/deal/nextz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loader/deal/reval.py` & `buildz-0.5.2/buildz/xf/loader/deal/reval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loader/deal/setz.py` & `buildz-0.5.2/buildz/xf/loader/deal/setz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loader/deal/spt.py` & `buildz-0.5.2/buildz/xf/loader/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loader/deal/strz.py` & `buildz-0.5.2/buildz/xf/loader/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loader/item.py` & `buildz-0.5.2/buildz/xf/loader/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loader/mg.py` & `buildz-0.5.2/buildz/xf/loader/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loader/pos.py` & `buildz-0.5.2/buildz/xf/loader/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loaderz/base.py` & `buildz-0.5.2/buildz/xf/loaderz/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loaderz/buffer.py` & `buildz-0.5.2/buildz/xf/loaderz/buffer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loaderz/deal/listz.py` & `buildz-0.5.2/buildz/xf/loaderz/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loaderz/deal/lr.py` & `buildz-0.5.2/buildz/xf/loaderz/deal/lr.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loaderz/deal/lrval.py` & `buildz-0.5.2/buildz/xf/loaderz/deal/lrval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loaderz/deal/mapz.py` & `buildz-0.5.2/buildz/xf/loaderz/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loaderz/deal/reval.py` & `buildz-0.5.2/buildz/xf/loaderz/deal/reval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loaderz/deal/spt.py` & `buildz-0.5.2/buildz/xf/loaderz/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loaderz/deal/strz.py` & `buildz-0.5.2/buildz/xf/loaderz/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loaderz/item.py` & `buildz-0.5.2/buildz/xf/loaderz/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loaderz/mg.py` & `buildz-0.5.2/buildz/xf/loaderz/mg.py`

 * *Files 12% similar despite different names*

```diff
@@ -151,28 +151,40 @@
 00000960: 2020 2020 2020 6172 7220 3d20 5b5d 0d0a        arr = []..
 00000970: 2020 2020 2020 2020 7768 696c 6520 7365          while se
 00000980: 6c66 2e64 6561 6c28 6275 6666 6572 2c20  lf.deal(buffer, 
 00000990: 6172 7229 3a0d 0a20 2020 2020 2020 2020  arr):..         
 000009a0: 2020 2070 6173 730d 0a20 2020 2020 2020     pass..       
 000009b0: 2061 7272 203d 205b 6b2e 7661 6c20 666f   arr = [k.val fo
 000009c0: 7220 6b20 696e 2061 7272 5d0d 0a20 2020  r k in arr]..   
-000009d0: 2020 2020 2069 6620 6c65 6e28 6172 7229       if len(arr)
-000009e0: 3d3d 313a 0d0a 2020 2020 2020 2020 2020  ==1:..          
-000009f0: 2020 6172 7220 3d20 6172 725b 305d 0d0a    arr = arr[0]..
-00000a00: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-00000a10: 7272 0d0a 2020 2020 6465 6620 6c6f 6164  rr..    def load
-00000a20: 7328 7365 6c66 2c20 7265 6164 6572 293a  s(self, reader):
-00000a30: 0d0a 2020 2020 2020 2020 6966 2074 7970  ..        if typ
-00000a40: 6528 7265 6164 6572 2920 3d3d 2073 656c  e(reader) == sel
-00000a50: 662e 7479 7065 3a0d 0a20 2020 2020 2020  f.type:..       
-00000a60: 2020 2020 2023 7072 696e 7428 6622 7472       #print(f"tr
-00000a70: 7920 7374 722c 207b 6c65 6e28 7265 6164  y str, {len(read
-00000a80: 6572 297d 2229 0d0a 2020 2020 2020 2020  er)}")..        
-00000a90: 2020 2020 6275 6666 203d 2062 7566 6665      buff = buffe
-00000aa0: 722e 5374 7242 7566 6665 7228 7265 6164  r.StrBuffer(read
-00000ab0: 6572 290d 0a20 2020 2020 2020 2065 6c73  er)..        els
-00000ac0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00000ad0: 6275 6666 203d 2062 7566 6665 722e 4275  buff = buffer.Bu
-00000ae0: 6666 6572 2872 6561 6465 7229 0d0a 2020  ffer(reader)..  
-00000af0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00000b00: 662e 6c6f 6164 2862 7566 6629 0d0a 0d0a  f.load(buff)....
-00000b10: 7061 7373 0d0a                           pass..
+000009d0: 2020 2020 2072 7374 203d 205b 5d0d 0a20       rst = [].. 
+000009e0: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
+000009f0: 6172 723a 0d0a 2020 2020 2020 2020 2020  arr:..          
+00000a00: 2020 6966 2074 7970 6528 6b29 203d 3d20    if type(k) == 
+00000a10: 7365 6c66 2e74 7970 653a 0d0a 2020 2020  self.type:..    
+00000a20: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00000a30: 656e 286b 2e73 7472 6970 2829 293d 3d30  en(k.strip())==0
+00000a40: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000a50: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
+00000a60: 0a20 2020 2020 2020 2020 2020 2072 7374  .            rst
+00000a70: 2e61 7070 656e 6428 6b29 0d0a 2020 2020  .append(k)..    
+00000a80: 2020 2020 6172 7220 3d20 7273 740d 0a20      arr = rst.. 
+00000a90: 2020 2020 2020 2069 6620 6c65 6e28 6172         if len(ar
+00000aa0: 7229 3d3d 313a 0d0a 2020 2020 2020 2020  r)==1:..        
+00000ab0: 2020 2020 6172 7220 3d20 6172 725b 305d      arr = arr[0]
+00000ac0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000ad0: 2061 7272 0d0a 2020 2020 6465 6620 6c6f   arr..    def lo
+00000ae0: 6164 7328 7365 6c66 2c20 7265 6164 6572  ads(self, reader
+00000af0: 293a 0d0a 2020 2020 2020 2020 6966 2074  ):..        if t
+00000b00: 7970 6528 7265 6164 6572 2920 3d3d 2073  ype(reader) == s
+00000b10: 656c 662e 7479 7065 3a0d 0a20 2020 2020  elf.type:..     
+00000b20: 2020 2020 2020 2023 7072 696e 7428 6622         #print(f"
+00000b30: 7472 7920 7374 722c 207b 6c65 6e28 7265  try str, {len(re
+00000b40: 6164 6572 297d 2229 0d0a 2020 2020 2020  ader)}")..      
+00000b50: 2020 2020 2020 6275 6666 203d 2062 7566        buff = buf
+00000b60: 6665 722e 5374 7242 7566 6665 7228 7265  fer.StrBuffer(re
+00000b70: 6164 6572 290d 0a20 2020 2020 2020 2065  ader)..        e
+00000b80: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00000b90: 2020 6275 6666 203d 2062 7566 6665 722e    buff = buffer.
+00000ba0: 4275 6666 6572 2872 6561 6465 7229 0d0a  Buffer(reader)..
+00000bb0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00000bc0: 656c 662e 6c6f 6164 2862 7566 6629 0d0a  elf.load(buff)..
+00000bd0: 0d0a 7061 7373 0d0a                      ..pass..
```

### Comparing `buildz-0.5.1/buildz/xf/loaderz/pos.py` & `buildz-0.5.2/buildz/xf/loaderz/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/loaderz/test.py` & `buildz-0.5.2/buildz/xf/loaderz/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 """
 from buildz.xf import readz as rz
 from buildz.xf import read as rd
 from buildz import xf
 import json
 import time
 
-def cost(f,*a,**b):
+def cost(n, f,*a,**b):
     c = time.time()
     r = f(*a,**b)
     d = time.time()-c
-    print(f"time cost in {f}: {d}")
+    print(f"time cost in {n}-{f}: {d}")
     return r
 
 pass
 
 n = 100
 m = 12
 l = 11
@@ -51,25 +51,26 @@
 pass
 print("test D")
 json.dumps(_arr)
 print("test E")
 json.dumps(_map)
 print("test F")
 js = json.dumps(rst)
+js = "\n\n"+js+"\n"
 #js = xf.dumps(rst, json_format=1)
 # js = r"""
 # [
 #     1,2,3,{"4":5,"6":7,"8":9,"10":11,"4":6}
 # ]
 # """
 print("start")
-jv = cost(json.loads,js)
-xv = cost(rz.loads,js)
+jv = cost("json.loads", json.loads,js)
+xv = cost("rz.loads",rz.loads,js)
 print(f"judge: {jv==xv}")
-_xv = cost(rd.loads, js)
+_xv = cost("rd.loads",rd.loads, js)
 #with open("test.json", 'w') as f:
 #    f.write(js)
 if n>3 or m>3 or l > 3:
     exit()
 print(json.dumps(jv))
 print(json.dumps(xv))
```

### Comparing `buildz-0.5.1/buildz/xf/mapz.py` & `buildz-0.5.2/buildz/xf/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/read.py` & `buildz-0.5.2/buildz/xf/read.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/readz.py` & `buildz-0.5.2/buildz/xf/readz.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from .loaderz import mg, buffer, base
-
+from . import file
 from .loaderz.deal import nextz, spt, strz, listz, spc, setz, mapz, reval, lrval
 class BoolFc:
     def __init__(self, mg):
         trues = [mg.like(k) for k in ["true", "True", "1"]]   
         trues += [1,True] 
         falses = [mg.like(k) for k in ["false", "False", "0"]]
         falses += [0,False]
@@ -72,11 +72,20 @@
 
 pass
 def load(read, as_bytes = False):
     mgs = build(as_bytes)
     return msg.loads(read)
 def loads(s):
     mgs = build(type(s)==bytes)
-    input = buffer.BufferInput(s)
+    #input = buffer.BufferInput(s)
     return mgs.loads(s)
 
 pass
+
+def loadf(fp, bts = False):
+    if bts:
+        s = file.bread(fp)
+    else:
+        s = file.fread(fp)
+    return loads(s)
+
+pass
```

### Comparing `buildz-0.5.1/buildz/xf/stack.py` & `buildz-0.5.2/buildz/xf/stack.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/write.py` & `buildz-0.5.2/buildz/xf/write.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 from .writer import mg, itemz, base, conf
 from .writer.deal import listz, mapz, strz, reval, jsonval
+from . import file
 pts = [
     "[\+\-]?\d+",
     "[\+\-]?\d+\.\d+",
     "[\+\-]?\d+e[\+\-]?\d+",
     "null",
     "true",
     "false",
@@ -33,12 +34,18 @@
     else:
         cf.set(set=1, prev=1)
     mgs = build(json_format)
     return mgs.dump(obj, cf)
 
 pass
 
+def dumpf(filepath, obj, bytes = 0, format = 0, deep = 0, json_format= 0, mode = 'w'):
+    s = dumps(obj, bytes = bytes, format = format, deep = deep, json_format= json_format)
+    file.fwrite(filepath, s, mode)
+
+pass
+
 def dump(output, obj, *argv, **maps):
     rs = dumps(obj, *argv, **maps)
     output(rs)
 
-pass
+pass
```

### Comparing `buildz-0.5.1/buildz/xf/writer/base.py` & `buildz-0.5.2/buildz/xf/writer/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/writer/conf.py` & `buildz-0.5.2/buildz/xf/writer/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/writer/deal/listz.py` & `buildz-0.5.2/buildz/xf/writer/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/writer/deal/mapz.py` & `buildz-0.5.2/buildz/xf/writer/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/writer/deal/strz.py` & `buildz-0.5.2/buildz/xf/writer/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/writer/itemz.py` & `buildz-0.5.2/buildz/xf/writer/itemz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/writer/mg.py` & `buildz-0.5.2/buildz/xf/writer/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz/xf/xargs.py` & `buildz-0.5.2/buildz/xf/xargs.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.1/buildz.egg-info/PKG-INFO` & `buildz-0.5.2/buildz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.5.1
+Version: 0.5.2
 Summary: a json-base file format's read and write code by python, and codes to read and product object from configure file in such format
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.5.1/buildz.egg-info/SOURCES.txt` & `buildz-0.5.2/buildz.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 buildz/demo/xf/deal.py
 buildz/demo/xf/help.py
 buildz/fz/__init__.py
 buildz/fz/dirz.py
 buildz/fz/fio.py
 buildz/fz/lsf.py
 buildz/ioc/__init__.py
+buildz/ioc/base.py
 buildz/ioc/init.py
 buildz/ioc/ioc/base.py
 buildz/ioc/ioc/conf.py
 buildz/ioc/ioc/confs.py
 buildz/ioc/ioc_deal/base.py
 buildz/ioc/ioc_deal/call.py
 buildz/ioc/ioc_deal/calls.py
```

### Comparing `buildz-0.5.1/setup.py` & `buildz-0.5.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Author: Zzz(1309458652@qq.com)
 # Description:
 
 from setuptools import setup, find_packages
 
 setup(
     name = 'buildz',
-    version = '0.5.1',
+    version = '0.5.2',
     keywords='buildz',
     long_description=open('README.md', 'r', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     description = "a json-base file format's read and write code by python, and codes to read and product object from configure file in such format",
     license = 'Apache License 2.0',
     url = 'https://github.com/buildCodeZ/buildz',
     author = 'Zzz',
```


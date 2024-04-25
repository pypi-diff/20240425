# Comparing `tmp/maptasker-2.6.3.tar.gz` & `tmp/maptasker-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maptasker-2.6.3.tar", max compression
+gzip compressed data, was "maptasker-3.2.2.tar", max compression
```

## Comparing `maptasker-2.6.3.tar` & `maptasker-3.2.2.tar`

### file list

```diff
@@ -1,69 +1,71 @@
--rw-r--r--   0        0        0    35149 2023-08-09 15:05:35.777000 maptasker-2.6.3/LICENSE.txt
--rw-r--r--   0        0        0      296 2023-08-09 15:05:35.778000 maptasker-2.6.3/README_PyPl.md
--rw-r--r--   0        0        0        0 2023-08-09 15:05:35.789000 maptasker-2.6.3/maptasker/__init__.py
--rw-r--r--   0        0        0   905912 2023-12-04 16:07:45.835000 maptasker-2.6.3/maptasker/assets/bg_gradient.jpg
--rw-r--r--   0        0        0   104984 2023-11-21 17:46:03.716000 maptasker-2.6.3/maptasker/assets/maptasker_logo_dark.png
--rw-r--r--   0        0        0   104904 2023-11-21 17:46:03.717000 maptasker-2.6.3/maptasker/assets/maptasker_logo_light.png
--rw-r--r--   0        0        0     1782 2024-01-08 16:34:35.226894 maptasker-2.6.3/maptasker/main.py
--rw-r--r--   0        0        0        0 2023-08-09 15:05:35.790000 maptasker-2.6.3/maptasker/src/__init__.py
--rw-r--r--   0        0        0    12381 2023-12-04 16:08:07.114000 maptasker-2.6.3/maptasker/src/actargs.py
--rw-r--r--   0        0        0    22444 2023-12-14 15:57:12.789000 maptasker-2.6.3/maptasker/src/action.py
--rw-r--r--   0        0        0   114452 2024-01-08 16:34:35.227682 maptasker-2.6.3/maptasker/src/actionc.py
--rw-r--r--   0        0        0     9294 2023-12-04 16:08:02.917000 maptasker-2.6.3/maptasker/src/actiond.py
--rw-r--r--   0        0        0    10932 2023-12-04 16:08:03.872000 maptasker-2.6.3/maptasker/src/actione.py
--rw-r--r--   0        0        0    13010 2023-12-10 16:27:17.486000 maptasker-2.6.3/maptasker/src/actionr.py
--rw-r--r--   0        0        0    15219 2024-01-12 20:24:12.771792 maptasker-2.6.3/maptasker/src/actiont.py
--rw-r--r--   0        0        0     2661 2023-12-04 16:08:02.782000 maptasker-2.6.3/maptasker/src/addcss.py
--rw-r--r--   0        0        0     3707 2023-12-14 15:57:12.762000 maptasker-2.6.3/maptasker/src/caveats.py
--rw-r--r--   0        0        0    11678 2023-11-15 16:38:54.566000 maptasker-2.6.3/maptasker/src/clip.py
--rw-r--r--   0        0        0     8660 2023-12-04 16:08:02.839000 maptasker-2.6.3/maptasker/src/colors.py
--rw-r--r--   0        0        0     3382 2023-11-08 17:54:50.532000 maptasker-2.6.3/maptasker/src/colrmode.py
--rw-r--r--   0        0        0    11500 2023-12-04 16:08:07.371000 maptasker-2.6.3/maptasker/src/condition.py
--rw-r--r--   0        0        0     2739 2024-01-11 16:49:08.085538 maptasker-2.6.3/maptasker/src/config.py
--rw-r--r--   0        0        0     6555 2023-12-14 15:57:12.728000 maptasker-2.6.3/maptasker/src/debug.py
--rw-r--r--   0        0        0      417 2023-12-04 16:07:45.842000 maptasker-2.6.3/maptasker/src/deprecate.py
--rw-r--r--   0        0        0    30403 2024-01-08 16:34:35.228240 maptasker-2.6.3/maptasker/src/diagram.py
--rw-r--r--   0        0        0    26445 2023-12-28 18:49:26.181000 maptasker-2.6.3/maptasker/src/diagutil.py
--rw-r--r--   0        0        0    20368 2023-12-28 18:49:27.078000 maptasker-2.6.3/maptasker/src/dirout.py
--rw-r--r--   0        0        0     2520 2024-01-08 16:34:35.228839 maptasker-2.6.3/maptasker/src/error.py
--rw-r--r--   0        0        0     2441 2023-12-28 18:49:26.993000 maptasker-2.6.3/maptasker/src/fonts.py
--rw-r--r--   0        0        0     5491 2023-12-10 16:27:14.906000 maptasker-2.6.3/maptasker/src/format.py
--rw-r--r--   0        0        0     5476 2024-01-11 16:52:41.474045 maptasker-2.6.3/maptasker/src/frontmtr.py
--rw-r--r--   0        0        0     6950 2024-01-11 18:21:05.836974 maptasker-2.6.3/maptasker/src/getbakup.py
--rw-r--r--   0        0        0     2543 2023-11-15 16:38:53.473000 maptasker-2.6.3/maptasker/src/getids.py
--rw-r--r--   0        0        0     5414 2024-01-11 18:42:30.648155 maptasker-2.6.3/maptasker/src/getputer.py
--rw-r--r--   0        0        0     8319 2023-12-04 16:08:08.829000 maptasker-2.6.3/maptasker/src/globalvr.py
--rw-r--r--   0        0        0     8791 2024-01-15 16:27:00.307046 maptasker-2.6.3/maptasker/src/guiutils.py
--rw-r--r--   0        0        0     3657 2024-01-11 18:54:10.878938 maptasker-2.6.3/maptasker/src/initparg.py
--rw-r--r--   0        0        0     2368 2023-11-15 16:38:53.257000 maptasker-2.6.3/maptasker/src/kidapp.py
--rw-r--r--   0        0        0    18441 2023-12-10 16:27:15.005000 maptasker-2.6.3/maptasker/src/lineout.py
--rw-r--r--   0        0        0    29184 2024-01-08 16:34:35.229752 maptasker-2.6.3/maptasker/src/mapit.py
--rw-r--r--   0        0        0     2519 2024-01-11 20:18:18.244235 maptasker-2.6.3/maptasker/src/maputils.py
--rw-r--r--   0        0        0     2788 2023-12-28 18:49:26.174000 maptasker-2.6.3/maptasker/src/nameattr.py
--rw-r--r--   0        0        0    20847 2023-12-28 18:49:28.675000 maptasker-2.6.3/maptasker/src/outline.py
--rw-r--r--   0        0        0    18226 2024-01-14 20:14:54.776517 maptasker-2.6.3/maptasker/src/parsearg.py
--rw-r--r--   0        0        0     8598 2023-12-04 16:08:07.441000 maptasker-2.6.3/maptasker/src/prefers.py
--rw-r--r--   0        0        0     6828 2023-12-28 18:49:28.526000 maptasker-2.6.3/maptasker/src/primitem.py
--rw-r--r--   0        0        0    11378 2024-01-11 20:20:41.403034 maptasker-2.6.3/maptasker/src/proclist.py
--rw-r--r--   0        0        0    12527 2023-12-10 16:27:17.489000 maptasker-2.6.3/maptasker/src/profiles.py
--rw-r--r--   0        0        0     2279 2024-01-08 16:34:35.231061 maptasker-2.6.3/maptasker/src/progargs.py
--rw-r--r--   0        0        0    12888 2024-01-14 16:27:42.436473 maptasker-2.6.3/maptasker/src/proginit.py
--rw-r--r--   0        0        0    25042 2024-01-08 16:34:35.232342 maptasker-2.6.3/maptasker/src/projects.py
--rw-r--r--   0        0        0     4895 2024-01-12 20:27:52.811152 maptasker-2.6.3/maptasker/src/property.py
--rw-r--r--   0        0        0    19366 2024-01-14 20:09:27.727795 maptasker-2.6.3/maptasker/src/runcli.py
--rw-r--r--   0        0        0     5685 2024-01-14 15:50:03.818038 maptasker-2.6.3/maptasker/src/rungui.py
--rw-r--r--   0        0        0    10544 2023-12-04 16:08:09.887000 maptasker-2.6.3/maptasker/src/scenes.py
--rw-r--r--   0        0        0    16184 2023-11-02 17:52:05.892000 maptasker-2.6.3/maptasker/src/servicec.py
--rw-r--r--   0        0        0     5610 2023-12-04 16:08:11.829000 maptasker-2.6.3/maptasker/src/share.py
--rw-r--r--   0        0        0     3235 2023-12-28 18:49:27.012000 maptasker-2.6.3/maptasker/src/shelsort.py
--rw-r--r--   0        0        0     6895 2024-01-11 17:27:45.193550 maptasker-2.6.3/maptasker/src/sysconst.py
--rw-r--r--   0        0        0     5519 2023-12-04 16:08:07.429000 maptasker-2.6.3/maptasker/src/taskactn.py
--rw-r--r--   0        0        0     4458 2023-12-04 16:08:07.300000 maptasker-2.6.3/maptasker/src/taskerd.py
--rw-r--r--   0        0        0     2695 2023-11-08 17:54:50.622000 maptasker-2.6.3/maptasker/src/taskflag.py
--rw-r--r--   0        0        0    19245 2023-12-14 15:57:14.741000 maptasker-2.6.3/maptasker/src/tasks.py
--rw-r--r--   0        0        0     9877 2023-12-10 16:27:14.905000 maptasker-2.6.3/maptasker/src/taskuniq.py
--rw-r--r--   0        0        0     2577 2023-12-04 16:08:10.113000 maptasker-2.6.3/maptasker/src/twisty.py
--rw-r--r--   0        0        0    92693 2024-01-14 18:22:43.440467 maptasker-2.6.3/maptasker/src/userintr.py
--rw-r--r--   0        0        0     9094 2023-12-28 18:49:28.572000 maptasker-2.6.3/maptasker/src/xmldata.py
--rw-r--r--   0        0        0     4414 2024-01-11 17:24:48.841356 maptasker-2.6.3/pyproject.toml
--rw-r--r--   0        0        0     1427 1970-01-01 00:00:00.000000 maptasker-2.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-02-16 16:36:22.405000 maptasker-3.2.2/LICENSE.txt
+-rw-r--r--   0        0        0      536 2024-03-04 15:40:38.700000 maptasker-3.2.2/README_PyPl.md
+-rw-r--r--   0        0        0        0 2024-03-10 15:08:20.218081 maptasker-3.2.2/maptasker/__init__.py
+-rw-r--r--   0        0        0     6148 2024-04-01 19:20:50.516566 maptasker-3.2.2/maptasker/assets/.DS_Store
+-rw-r--r--   0        0        0     9216 2024-02-22 20:13:00.839000 maptasker-3.2.2/maptasker/assets/Thumbs.db
+-rw-r--r--   0        0        0      390 2024-03-25 17:21:31.285000 maptasker-3.2.2/maptasker/assets/icons/arrow.png
+-rw-r--r--   0        0        0   104984 2023-11-21 17:46:03.716000 maptasker-3.2.2/maptasker/assets/maptasker_logo_dark.png
+-rw-r--r--   0        0        0   104904 2023-11-21 17:46:03.717000 maptasker-3.2.2/maptasker/assets/maptasker_logo_light.png
+-rw-r--r--   0        0        0     1782 2024-01-08 16:34:50.197000 maptasker-3.2.2/maptasker/main.py
+-rw-r--r--   0        0        0       17 2024-02-02 20:14:04.969000 maptasker-3.2.2/maptasker/src/__init__.py
+-rw-r--r--   0        0        0    13403 2024-04-22 18:46:54.550133 maptasker-3.2.2/maptasker/src/actargs.py
+-rw-r--r--   0        0        0    22348 2024-04-23 15:59:50.762210 maptasker-3.2.2/maptasker/src/action.py
+-rw-r--r--   0        0        0   124439 2024-04-22 17:26:35.331982 maptasker-3.2.2/maptasker/src/actionc.py
+-rw-r--r--   0        0        0     8377 2024-02-22 20:13:10.380000 maptasker-3.2.2/maptasker/src/actiond.py
+-rw-r--r--   0        0        0    15288 2024-04-24 15:53:27.526860 maptasker-3.2.2/maptasker/src/actione.py
+-rw-r--r--   0        0        0     9824 2024-04-22 17:26:35.332913 maptasker-3.2.2/maptasker/src/actionr.py
+-rw-r--r--   0        0        0    17204 2024-04-22 17:49:35.161773 maptasker-3.2.2/maptasker/src/actiont.py
+-rw-r--r--   0        0        0     3376 2024-02-22 20:13:12.356000 maptasker-3.2.2/maptasker/src/addcss.py
+-rw-r--r--   0        0        0     3783 2024-04-03 14:57:05.818846 maptasker-3.2.2/maptasker/src/caveats.py
+-rw-r--r--   0        0        0    11837 2024-04-08 18:48:52.139846 maptasker-3.2.2/maptasker/src/clip.py
+-rw-r--r--   0        0        0     8660 2023-12-04 16:08:02.839000 maptasker-3.2.2/maptasker/src/colors.py
+-rw-r--r--   0        0        0     3186 2024-03-08 20:16:24.477154 maptasker-3.2.2/maptasker/src/colrmode.py
+-rw-r--r--   0        0        0    11594 2024-04-22 19:20:55.481502 maptasker-3.2.2/maptasker/src/condition.py
+-rw-r--r--   0        0        0     2964 2024-04-22 18:09:44.736049 maptasker-3.2.2/maptasker/src/config.py
+-rw-r--r--   0        0        0     6541 2024-02-02 20:14:15.316000 maptasker-3.2.2/maptasker/src/debug.py
+-rw-r--r--   0        0        0      417 2023-12-04 16:07:45.842000 maptasker-3.2.2/maptasker/src/deprecate.py
+-rw-r--r--   0        0        0    30601 2024-03-25 17:21:29.641646 maptasker-3.2.2/maptasker/src/diagram.py
+-rw-r--r--   0        0        0    27007 2024-02-16 16:36:21.774000 maptasker-3.2.2/maptasker/src/diagutil.py
+-rw-r--r--   0        0        0    19996 2024-02-09 18:52:35.434000 maptasker-3.2.2/maptasker/src/dirout.py
+-rw-r--r--   0        0        0     2567 2024-03-25 17:21:29.642197 maptasker-3.2.2/maptasker/src/error.py
+-rw-r--r--   0        0        0     2399 2024-02-02 20:14:19.267000 maptasker-3.2.2/maptasker/src/fonts.py
+-rw-r--r--   0        0        0     4456 2024-04-22 17:26:35.333800 maptasker-3.2.2/maptasker/src/format.py
+-rw-r--r--   0        0        0     5667 2024-04-24 17:08:54.572965 maptasker-3.2.2/maptasker/src/frontmtr.py
+-rw-r--r--   0        0        0     5353 2024-04-22 17:26:35.334483 maptasker-3.2.2/maptasker/src/getbakup.py
+-rw-r--r--   0        0        0     2311 2024-03-28 13:52:59.398409 maptasker-3.2.2/maptasker/src/getids.py
+-rw-r--r--   0        0        0     9022 2024-04-22 17:26:35.334798 maptasker-3.2.2/maptasker/src/getputer.py
+-rw-r--r--   0        0        0     9754 2024-02-22 20:13:15.666000 maptasker-3.2.2/maptasker/src/globalvr.py
+-rw-r--r--   0        0        0    57599 2024-04-25 14:09:33.914038 maptasker-3.2.2/maptasker/src/guiutils.py
+-rw-r--r--   0        0        0     3622 2024-04-22 17:26:35.335618 maptasker-3.2.2/maptasker/src/initparg.py
+-rw-r--r--   0        0        0     2660 2024-04-23 19:17:24.453323 maptasker-3.2.2/maptasker/src/kidapp.py
+-rw-r--r--   0        0        0    25168 2024-04-22 17:49:35.083904 maptasker-3.2.2/maptasker/src/lineout.py
+-rw-r--r--   0        0        0    30569 2024-04-22 17:26:35.336412 maptasker-3.2.2/maptasker/src/mapit.py
+-rw-r--r--   0        0        0    11473 2024-04-22 17:26:35.336848 maptasker-3.2.2/maptasker/src/maputils.py
+-rw-r--r--   0        0        0     2788 2023-12-28 18:49:26.174000 maptasker-3.2.2/maptasker/src/nameattr.py
+-rw-r--r--   0        0        0    20711 2024-02-16 16:36:22.869000 maptasker-3.2.2/maptasker/src/outline.py
+-rw-r--r--   0        0        0    19389 2024-04-22 17:26:35.337190 maptasker-3.2.2/maptasker/src/parsearg.py
+-rw-r--r--   0        0        0     8606 2024-02-02 20:14:19.240000 maptasker-3.2.2/maptasker/src/prefers.py
+-rw-r--r--   0        0        0     6557 2024-04-22 17:26:35.337522 maptasker-3.2.2/maptasker/src/primitem.py
+-rw-r--r--   0        0        0    11458 2024-04-22 17:26:35.337860 maptasker-3.2.2/maptasker/src/proclist.py
+-rw-r--r--   0        0        0    14911 2024-04-23 17:25:10.170331 maptasker-3.2.2/maptasker/src/profiles.py
+-rw-r--r--   0        0        0     2280 2024-02-02 20:14:19.331000 maptasker-3.2.2/maptasker/src/progargs.py
+-rw-r--r--   0        0        0    14895 2024-04-22 17:49:35.097099 maptasker-3.2.2/maptasker/src/proginit.py
+-rw-r--r--   0        0        0    29741 2024-04-22 17:26:35.338911 maptasker-3.2.2/maptasker/src/projects.py
+-rw-r--r--   0        0        0     6427 2024-04-24 16:19:29.129511 maptasker-3.2.2/maptasker/src/property.py
+-rw-r--r--   0        0        0    23015 2024-04-22 18:30:56.778950 maptasker-3.2.2/maptasker/src/runcli.py
+-rw-r--r--   0        0        0     7007 2024-04-22 17:26:35.340024 maptasker-3.2.2/maptasker/src/rungui.py
+-rw-r--r--   0        0        0    23118 2024-04-23 17:36:37.169021 maptasker-3.2.2/maptasker/src/scenes.py
+-rw-r--r--   0        0        0    16315 2024-02-02 20:14:14.236000 maptasker-3.2.2/maptasker/src/servicec.py
+-rw-r--r--   0        0        0     6193 2024-02-22 20:13:15.794000 maptasker-3.2.2/maptasker/src/share.py
+-rw-r--r--   0        0        0     3658 2024-02-16 16:36:21.861000 maptasker-3.2.2/maptasker/src/shelsort.py
+-rw-r--r--   0        0        0     7592 2024-04-23 16:41:51.648697 maptasker-3.2.2/maptasker/src/sysconst.py
+-rw-r--r--   0        0        0     6351 2024-04-22 17:26:35.341001 maptasker-3.2.2/maptasker/src/taskactn.py
+-rw-r--r--   0        0        0     6835 2024-03-25 17:21:29.645740 maptasker-3.2.2/maptasker/src/taskerd.py
+-rw-r--r--   0        0        0     2673 2024-04-22 17:26:35.341286 maptasker-3.2.2/maptasker/src/taskflag.py
+-rw-r--r--   0        0        0    23237 2024-04-24 13:57:13.525905 maptasker-3.2.2/maptasker/src/tasks.py
+-rw-r--r--   0        0        0     9999 2024-04-22 18:40:19.709942 maptasker-3.2.2/maptasker/src/taskuniq.py
+-rw-r--r--   0        0        0     2100 2024-02-20 15:01:50.903000 maptasker-3.2.2/maptasker/src/twisty.py
+-rw-r--r--   0        0        0   106559 2024-04-25 14:30:36.887208 maptasker-3.2.2/maptasker/src/userintr.py
+-rw-r--r--   0        0        0    10663 2024-04-22 17:49:35.056082 maptasker-3.2.2/maptasker/src/xmldata.py
+-rw-r--r--   0        0        0     4998 2024-04-22 17:31:25.198247 maptasker-3.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 maptasker-3.2.2/PKG-INFO
```

### Comparing `maptasker-2.6.3/maptasker/assets/maptasker_logo_dark.png` & `maptasker-3.2.2/maptasker/assets/maptasker_logo_dark.png`

 * *Files identical despite different names*

### Comparing `maptasker-2.6.3/maptasker/assets/maptasker_logo_light.png` & `maptasker-3.2.2/maptasker/assets/maptasker_logo_light.png`

 * *Files identical despite different names*

### Comparing `maptasker-2.6.3/maptasker/main.py` & `maptasker-3.2.2/maptasker/main.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.6.3/maptasker/src/actargs.py` & `maptasker-3.2.2/maptasker/src/actargs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing action runner logic."""
+
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
 # actargs: process Task "Action" arguments                                             #
 #                                                                                      #
 # GNU General Public License v3.0                                                      #
@@ -16,140 +17,159 @@
 import defusedxml.ElementTree  # Need for type hints
 
 import maptasker.src.action as get_action
 from maptasker.src.actiond import process_condition_list
 from maptasker.src.format import format_html
 from maptasker.src.primitem import PrimeItems
 from maptasker.src.sysconst import FormatLine, logger
+from maptasker.src.xmldata import extract_integer, extract_string
 
 
 # ##################################################################################
 # We have a <bundle>.   Process it
 # ##################################################################################
-def get_bundle(code_action: defusedxml.ElementTree.XML, evaluated_results: dict) -> dict:
+def get_bundle(code_action: defusedxml.ElementTree.XML, evaluated_results: dict, arg: str) -> dict:
     """
-    Get the details regarding the <bundle> action argument type
-        Args:
-            code_action (defusedxml.ElementTree.XML): XML element of the action code <code>
-            evaluated_results (dict): We stuff the findings in here for passing to the caller
-
-        Returns:
-            dict: The results from the <bundle> argument
+    Gets a bundle from an XML code action.
+    Args:
+        code_action: ElementTree.XML: The XML code action
+        evaluated_results: dict: The dictionary to store results
+        arg: str: The argument name
+    Returns:
+        dict: The evaluated results dictionary with the bundle value
+    Processing Logic:
+    - Finds the "Bundle" child in the code action
+    - Finds the "Vals" child of "Bundle"
+    - Finds either the "com.twofortyfouram.locale.intent.extra.BLURB" or "Configcommand" child of "Vals"
+    - If either is found, gets the text and stores in the results dict
+    - Else, sets a flag and empty string in results
     """
+
     child1 = code_action.find("Bundle")
     child2 = child1.find("Vals")
-    child3 = child2.find("com.twofortyfouram.locale.intent.extra.BLURB")  # 2:40 am...funny!
-    if child3 is not None and child3.text is not None:
-        # Get rid of extraneous html in Action's label
-        # clean_string = child3.text.replace("</font><br><br>", "<br><br>")
-        # clean_string = clean_string.replace("&lt;", "<")
-        # clean_string = clean_string.replace("&gt;", ">")
-        clean_string = child3.text
-        evaluated_results["result_bun"].append(clean_string)
+    child3 = child2.find("com.twofortyfouram.locale.intent.extra.BLURB")
+    child4 = child2.find("Configcommand")
+    if (child3 is not None or child4 is not None) or (child4 is not None and child4.text is not None):
+        clean_string = child3.text if child3 is not None else child4.text
+
+        # Make pretty
+        if PrimeItems.program_arguments["pretty"] and clean_string is not None:
+            clean_string = clean_string.replace("\n\n", "\n")
+            clean_string = clean_string.replace("\n", ",")
+        evaluated_results[f"arg{arg}"]["value"] = f"Configuration Parameter(s):\n{clean_string}\n"
     else:
         evaluated_results["returning_something"] = False
+        evaluated_results[f"arg{arg}"]["value"] = ""
     return evaluated_results
 
 
 # ##################################################################################
 # Given an <argn> element, evaluate it's contents based on our Action code dictionary
 # ##################################################################################
 def get_action_arguments(
     evaluated_results: dict,
     arg: object,
     argeval: list,
     argtype: list,
     code_action: defusedxml.ElementTree.XML,
 ) -> dict:
     """
-    Given an <argn> element, evaluate it's contents based on our Action code dictionary
-    (actionc.py)
-
-        :param evaluated_results: all the Action argument "types" and "arguments" as
-            a dictionary
-        :param arg: the incoming argument location/number (e.g. "0" for <arg0>)
-        :param argeval: the evaluation argument from our action code table (actionc.py)
-            e.g. "Timeout:" in "evalargs": ["", "Timeout:", ["", "e", ",
-            Structure Output (JSON, etc)"]],
-        :param argtype: the argument "type"- Str, Int, App, ConditionList, Bundle, Img
-        :param code_action: xml element of the Action code (<code>nnn</code>)
-        :return:  of results
+    Gets action arguments from XML code action
+    Args:
+        evaluated_results: dict - Stores evaluation results
+        arg: object - Argument object
+        argeval: list - Argument evaluation
+        argtype: list - Argument type
+        code_action: defusedxml.ElementTree.XML - XML code action
+    Returns:
+        dict - Updated evaluated results dictionary
+    Processing Logic:
+        - Sets flags for returning value and parsing XML
+        - Extracts argument value based on type by calling extraction functions
+        - Handles special types like App, ConditionList, Image, Bundle
+        - Returns updated evaluated results
     """
 
     # Assume we are returing something and that we have a <str> or <int> argument to get
     evaluated_results["returning_something"] = True
-    evaluated_results["get_xml_flag"] = True
 
     # Evaluate the argument based on its type.
+    the_arg = f"arg{arg}"
     match argtype:
         case "Int":
-            evaluated_results["intargs"].append(f"arg{arg}")
-            evaluated_results["inteval"].append(argeval)
+            evaluated_results[the_arg]["value"] = extract_integer(code_action, the_arg, argeval)
 
         case "Str":
-            evaluated_results["strargs"].append(f"arg{arg}")
-            evaluated_results["streval"].append(argeval)
+            if argeval == "Label":
+                for child in code_action:
+                    if child.tag == "label":
+                        evaluated_results[the_arg]["value"] = child.text
+                        break
+            else:
+                evaluated_results[the_arg]["value"] = extract_string(code_action, the_arg, argeval)
 
         case "App":
             extract_argument(evaluated_results, arg, argeval)
             app_class, app_pkg, app = get_action.get_app_details(code_action)
-            evaluated_results["result_app"].append(f"{app_class}, {app_pkg}, {app}")
+            evaluated_results[the_arg]["value"] = f"{app_class}, {app_pkg}, {app}"
 
         case "ConditionList":
             extract_condition(evaluated_results, arg, argeval, code_action)
 
         case "Img":
-            extract_image(evaluated_results, code_action, argeval)
+            extract_image(evaluated_results, code_action, argeval, arg)
         case "Bundle":  # It's a plugin
-            evaluated_results["get_xml_flag"] = False
-            evaluated_results = get_bundle(code_action, evaluated_results)
+            evaluated_results = get_bundle(code_action, evaluated_results, arg)
 
         case _:
-            evaluated_results["get_xml_flag"] = False
             logger.debug(f"actargs get_action_results error unknown argtype:{argtype}!!!!!")
             evaluated_results["returning_something"] = False
     return evaluated_results
 
 
 # ##################################################################################
 # Get image details from <img> sub-elements.
 # ##################################################################################
 # Get image related details from action xml
-def extract_image(evaluated_results: dict, code_action: defusedxml, argeval: str) -> None:
+def extract_image(evaluated_results: dict, code_action: defusedxml, argeval: str, arg: str) -> None:
     """
     Extract image from evaluated results
     Args:
         evaluated_results: dict - The dictionary containing the evaluation results
         code_action: defusedxml - The parsed defusedxml object
         argeval: str - The argument evaluation string
+        arg: str - The argument number
     Returns:
         None - No return value
     Processing Logic:
         - Find the <Img> tag in the code_action
         - Extract the image name and package if present
         - Append the image details to the result_img list in evaluated_results dictionary
         - Set returning_something to False if no image is found
     """
-    evaluated_results["get_xml_flag"] = False
     image, package = "", ""
     child = code_action.find("Img")
     # Image name
     with contextlib.suppress(Exception):
         image = child.find("nme").text
     if child.find("pkg") is not None:
         package = f'", Package:"{child.find("pkg").text}'
     elif child.find("var") is not None:  # There is a variable name?
         image = child.find("var").text
     if image:
-        evaluated_results["result_img"].append(f"{argeval}{image}{package}")
+        evaluated_results[f"arg{arg}"]["value"] = f"{argeval}{image}{package}"
+
     else:
-        evaluated_results["result_img"].append(" ")
-        evaluated_results["returning_something"] = False
+        evaluated_results[f"arg{arg}"]["value"] = " "
+        # evaluated_results["returning_something"] = False  # NOTE: This caused errors with Scene ButtonElement
 
 
+# ##################################################################################
+# Get condition releated details from action xml
+# ##################################################################################
 # Get condition releated details from action xml
 def extract_condition(evaluated_results: dict, arg: str, argeval: str, code_action: str) -> None:
     # Get argument
     """
     Extracts the condition from the code action.
     Args:
         evaluated_results: dict - The dictionary containing the evaluated results
@@ -174,33 +194,35 @@
     for numx, condition in enumerate(condition_list):
         # Add the condition 0 1 2: a = x
         conditions.append(f" {condition[0]}{condition[1]}{condition[2]}")
         # Add the boolean operator if it exists
         if boolean_list and len(boolean_list) > numx:
             conditions.append(f" {boolean_list[numx]}")
     seperator = ""
-    evaluated_results["result_con"].append(seperator.join(conditions))
 
+    evaluated_results[f"arg{arg}"]["value"] = seperator.join(conditions)
 
+
+# ##################################################################################
+# Get the argument details from action xml
+# ##################################################################################
 # Get the argument details from action xml
 def extract_argument(evaluated_results: dict, arg: str, argeval: str) -> None:
     """
     Extracts an argument from evaluated results
     Args:
         evaluated_results: Dictionary containing evaluated results
         arg: Argument name
         argeval: Argument evaluation
     Returns:
         None: Function does not return anything
     - Appends argument name to strargs list in evaluated_results
     - Appends argument evaluation to streval list in evaluated_results
     - Sets get_xml_flag to False"""
-    evaluated_results["get_xml_flag"] = False
-    evaluated_results["strargs"].append(f"arg{arg!s}")
-    evaluated_results["streval"].append(argeval)
+    evaluated_results[f"arg{arg}"]["value"] = argeval
 
 
 # ##################################################################################
 # Action code not found...let user know
 # ##################################################################################
 def handle_missing_code(the_action_code_plus: str, index: int) -> str:
     """
@@ -264,25 +286,26 @@
         index = num if arg == "if" else our_action_args.index(arg)
 
         # Get the arg name and type
         try:
             argeval = evaluate_list[num]
         except IndexError:
             evaluated_results["returning_something"] = False
-            evaluated_results[
-                "error"
-            ] = "MapTasker mapped IndexError error in action_args...action details not displayed"
+            evaluated_results["error"] = (
+                "MapTasker mapped IndexError error in action_args...action details not displayed"
+            )
             return evaluated_results
         try:
             argtype = our_action_code.types[index]
         except IndexError:
             argtype = handle_missing_code(the_action_code_plus, index)
 
         # Get the Action arguments
-        evaluated_results["position_arg_type"].append(argtype)
+        evaluated_results[f"arg{arg}"] = {}
+        evaluated_results[f"arg{arg}"]["type"] = argtype
         evaluated_results = get_action_arguments(
             evaluated_results,
             arg,
             argeval,
             argtype,
             code_action,
         )
```

### Comparing `maptasker-2.6.3/maptasker/src/action.py` & `maptasker-3.2.2/maptasker/src/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing action runner logic."""
+
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
 # action: Find Task's Action arguments (<argn>) and return as sorted list              #
 #                                                                                      #
 # Permissions of this strong copyleft license are conditioned on making available      #
@@ -21,15 +22,15 @@
     import defusedxml.ElementTree
 
 from maptasker.src.actiont import lookup_values
 from maptasker.src.error import error_handler
 from maptasker.src.format import format_html
 from maptasker.src.primitem import PrimeItems
 from maptasker.src.shelsort import shell_sort
-from maptasker.src.sysconst import FONT_FAMILY, RE_FONT, DISPLAY_DETAIL_LEVEL_all_tasks
+from maptasker.src.sysconst import DISABLED, FONT_FAMILY, RE_FONT, DISPLAY_DETAIL_LEVEL_all_tasks
 from maptasker.src.xmldata import remove_html_tags
 
 
 # ##################################################################################
 # Given a Task's Action, find all 'arg(n)' xml elements and return as a sorted list
 #  This is only called if the action code is not already in our master dictionary
 #   actionc.py
@@ -69,29 +70,14 @@
             str(ind) for ind, x in enumerate(arguments)
         ]  # Build list of arg position only (numeric part of argn)
 
     return arguments, argument_types, arg_nums
 
 
 # ##################################################################################
-# Check a value for '0' and return the appropriate string if it is/isn't
-# ##################################################################################
-def if_zero_else(the_value: str, if_zero_string: str, if_not_zero_string: str) -> str:
-    """
-    Returns string #1 if the value is 0, otherwise return string #2
-        :param the_value: the value to evaluate
-        :param if_zero_string: the string to return if the value to evaluate is zero
-        :param if_not_zero_string: the string to return if the value to evaluate
-                is not zero
-        :return: the value set by the above evaluation
-    """
-    return if_zero_string if the_value == "0" else if_not_zero_string
-
-
-# ##################################################################################
 # Evaluate the If statement and return the operation
 # ##################################################################################
 def evaluate_condition(child: defusedxml.ElementTree) -> tuple[str, str, str]:
     """
     Evaluate the If statement and return the operation
         :param child: xml head element containing the <lhs xml element to be evaluated
         :return: the evaluated result based on the <lhs elemental number
@@ -200,16 +186,15 @@
     [
             ["Test:", "l", "235"],
             ", Name:",
             ", Value:",
             ["", "e", "Use Root"],
             ", Read Setting To:",
         ]
-    arg_locvation points to the specific item in the agbove list that we are to
-    process here.
+    arg_location points to the specific item in the above list that we are to process here.
     # code_flag identifies the type of xml data to go after based on the specific code
     #   in <code>xxx</code>
     # *args is an undetermined number of lists, each consisting of 3 pairs:
     #   1: True=it is a string, False it is an integer,
     #   2: the value to test
     #   3: the value to plug in if it meets the test
         :param names: list of entries to substitute the argn value against from actionc.
@@ -232,15 +217,23 @@
         idx = (idx + 1) % len_of_list  # Get next element = first element in pair
         this_element = the_list[idx]
 
         # Are we to just evaluate for 0 or 1?
         if this_element in ["e", "if"]:
             idx = (idx + 1) % len_of_list
             next_element = the_list[idx]  # Second element in pair
-            evaluated_value = evaluate_action_setting([False, the_int_value, next_element])
+            # Determine whether we are to include the negative value.
+            # This will equate to True or False, depending on 1 or 0.
+            # The next line equates to the followinbg commented-out lines.
+            include_negative = the_list[0] == "1" if this_element == "e" else False
+            # if this_element == "e":
+            #    include_negative = the_list[0] == "1"  # This will equate to True or False, depending on 1 or 0.
+            # else:
+            #    include_negative = False  # The default
+            evaluated_value = evaluate_action_setting([include_negative, the_int_value, next_element])
             evaluated_value = f"{evaluated_value[0]}, "
             match_results.append(evaluated_value)
             break
 
         # Are we to do a table lookup for the value?
         if this_element == "l":
             idx = (idx + 1) % len_of_list  # Point to the lookup key
@@ -254,15 +247,14 @@
                         f"MapTasker 'mapped' error in action: int {the_int_value} not"
                         f" in lookup_values (actiont) for item {the_list[idx]} which is"
                         f" {[lookup_values[the_list[idx]]]}",
                     )
                 break
 
             # Error: the element is not in the lookup table.
-            # Handle the error and exit.
             match_results.append(
                 f"MapTasker 'mapped' error in action: {the_list[idx]} is not in"
                 f" actiont (lookup table) for name:{names}",
             )
             # Get out of loop
             break
 
@@ -284,26 +276,32 @@
     """
     Get Task's label, disabled flag and any conditions
         :param child: head Action xml element
         :return: the string containing any found label, disabled flag and conditions
     """
     task_label = ""
     task_conditions = ""
-    the_action_code = child.find("code").text
+
+    # If no code found, bail.
+    if child.find("code") is not None:
+        the_action_code = child.find("code").text
+    else:
+        return ""
+
     # Get the label, if any
     if child.find("label") is not None:
         lbl = child.find("label").text
         # Make sure the label doesn't have any HTML crap in it
         task_label = clean_label(lbl)
     # See if Action is disabled
     action_disabled = (
         format_html(
             "disabled_action_color",
             "",
-            " [DISABLED]",
+            DISABLED,
             True,
         )
         if child.find("on") is not None
         else ""
     )
     # Look for any conditions:  <ConditionList sr="if">
     if child.find("ConditionList") is not None:  # If condition on Action?
@@ -426,28 +424,35 @@
 - The function formats the output using the 'format_html' function.
 - The function removes any empty '<span>' elements from the output.
 - The function only retrieves extra details if the code represents a Task Action and
     the display detail level is set to 3.
 """
 
 
+# ##################################################################################
+# Chase after relevant data after <code> Task action
+# ##################################################################################
 def get_extra_stuff(
     code_action: defusedxml.ElementTree,
     action_type: bool,
 ) -> str:
     """
     # Chase after relevant data after <code> Task action
     # code_flag identifies the type of xml data to go after based on the specific code in <code>xxx</code>
     # Get the: label, whether to continue Task after error, etc.
 
         :param code_action: action code (e.g. "543") xml element
         :param action_type: True if this is a Task Action, otherwise False
         :return: formatted line of extra details about Task Action
     """
 
+    # If no code, just bail out.add
+    if code_action.find("code") is None:
+        return ""
+
     program_arguments = PrimeItems.program_arguments
     colors_to_use = PrimeItems.colors_to_use
 
     # Only get extras if this is a Task action (vs. a Profile condition)
     if action_type and program_arguments["display_detail_level"] > DISPLAY_DETAIL_LEVEL_all_tasks:
         # Look for extra Task stuff: label, disabled, conditions
         extra_stuff = get_label_disabled_condition(code_action)
@@ -456,20 +461,14 @@
         extra_stuff = (
             RE_FONT.sub("", extra_stuff)
             # extra_stuff.replace("</font>", "")
             if "<font" in extra_stuff and "</font>" not in extra_stuff
             else extra_stuff
         )
         extra_stuff = (
-            RE_FONT.sub("", extra_stuff)
-            # extra_stuff.replace("</font>", "")
-            if "&lt;font" in extra_stuff and "&lt;/font&gt;" not in extra_stuff
-            else extra_stuff
-        )
-        extra_stuff = (
             extra_stuff.replace("</b>", "") if "<b>" in extra_stuff and "</b>" not in extra_stuff else extra_stuff
         )
 
     else:
         extra_stuff = ""
 
     if program_arguments["debug"] and action_type:  # Add the code if this is an Action and in debug mode
```

### Comparing `maptasker-2.6.3/maptasker/src/actionc.py` & `maptasker-3.2.2/maptasker/src/actionc.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,77 +26,78 @@
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 # #################################################################################### #
 from collections import namedtuple
 
 # from typing import List
 
-ActionCode = namedtuple(
+ActionCode = namedtuple(  # noqa: PYI024
     "ActionCode",
     ["numargs", "redirect", "args", "types", "display", "reqargs", "evalargs"],
 )
 
 action_codes = {
-    "1000e": ActionCode(0, "", ["0"], ["Int"], "Display Unlocked", ["0"], [["Priority:", "l", "4s"]]),
+    "1000e": ActionCode(0, "", ["0"], ["Int"], "Display Unlocked", ["0"], [["Priority=", "l", "4s"]]),
     "1000s": ActionCode(0, "", [], [], "Plugin", [], []),
     "1000t": ActionCode(0, "", [], [], "Plugin", [], []),
     "100s": ActionCode(0, "", [], [], "Airplane Mode", [], []),
     "100t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Int", "ConditionList"],
         "Search",
         ["0", "1"],
-        ["Number:", ["", "e", "Info"]],
+        ["Number=", ["", "e", "Info"]],
     ),
     "101t": ActionCode(0, "", [], [], "Take Photo", [], []),
     "102t": ActionCode(0, "", [], [], "Open File", [], []),
     "103s": ActionCode(0, "", [], [], "Light Level", ["0"], []),
     "104s": ActionCode(0, "", [], [], "Pressure", [], []),
     "104t": ActionCode(0, "", [], [], "Browse URL", [], []),
     "1040876951t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Bundle", "Str", "Str", "Int", "Int"],
         "AutoInput UI Query",
         ["0", "3", "4"],
-        ["", "Timeout:", ["", "e", ", Structure Output (JSON, etc)"]],
+        ["", "Timeout=", ["", "e", ", Structure Output (JSON, etc)"]],
     ),
     "105s": ActionCode(0, "", [], [], "Media Button", [], []),
     "105t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Int", "Str"],
         "Set Clipboard",
         ["0", "1", "2"],
-        ["Text:", ["", "e", ", Add"], "Image:"],
+        ["Text=", ["", "e", ", Add"], "Image="],
     ),
     "106s": ActionCode(0, "", [], [], "Magnetic Field", [], []),
     "107s": ActionCode(0, "", [], [], "Missed Call", [], []),
     "107361459t": ActionCode(0, "1040876951t", [], [], "AutoInput Actions V2", [], []),
     "109t": ActionCode(0, "", [], [], "Set Wallpaper", [], []),
     "1099157652t": ActionCode(0, "1040876951t", [], [], "AutoTools Json Write", [], []),
-    "10s": ActionCode(1, "", ["0"], ["Int"], "Power", ["0"], [["Set:", "l", "10s"]]),
+    "1094115366t": ActionCode(0, "1040876951t", [], [], "AutoCast Device Settings", [], []),
+    "10s": ActionCode(1, "", ["0"], ["Int"], "Power", ["0"], [["Set=", "l", "10s"]]),
     "110s": ActionCode(
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["Int", "Int", "Int", "Int", "Int", "Int"],
         "Mobile Network",
         ["0", "1", "2", "3", "4", "5"],
         [
             ["", "e", "2G"],
             ["", "e", "3G"],
             ["", "e", "3G-HSPA"],
             ["", "e", "4G"],
             ["", "e", "5G"],
-            [", Active:", "l", "160"],
+            [", Active=", "l", "160"],
         ],
     ),
     "111t": ActionCode(0, "", [], [], "Compose MMS", [], []),
     "112t": ActionCode(0, "", [], [], "Run SL4A Script", [], []),
     "1120274117t": ActionCode(0, "1040876951t", [], [], "Locus Map", [], []),
     "1132319851t": ActionCode(0, "1040876951t", [], [], "AutoSheets Add Sheet", [], []),
     "1133159835e": ActionCode(
@@ -131,19 +132,19 @@
     "119t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Int", "Str", "Str", "Int", "Str"],
         "Open Map",
         ["0", "1", "2", "3", "4"],
-        [["Mode:", "l", "119"], ", Address:", ", Lat, Long:", ", Zoom:", ", Label:"],
+        [["Mode=", "l", "119"], ", Address=", ", Lat, Long=", ", Zoom=", ", Label="],
     ),
-    "120s": ActionCode(1, "", ["0"], ["Int"], "Orientation", ["0"], [["Is:", "l", "120s"]]),
+    "120s": ActionCode(1, "", ["0"], ["Int"], "Orientation", ["0"], [["Is=", "l", "120s"]]),
     "122375409t": ActionCode(0, "1040876951t", [], [], "AutoWeb Web Services", [], []),
-    "122s": ActionCode(1, "", ["0"], ["Int"], "Display Orientation", ["0"], [["Is:", "l", "122s"]]),
+    "122s": ActionCode(1, "", ["0"], ["Int"], "Display Orientation", ["0"], [["Is=", "l", "122s"]]),
     "123s": ActionCode(
         8,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7"],
         ["Str", "Int", "Int", "Str", "Str", "Str", "Int", "Int"],
         "Display State",
         ["0"],
@@ -153,20 +154,20 @@
         8,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7"],
         ["Str", "Int", "Int", "Str", "Str", "Str", "Int", "Int"],
         "Run Shell",
         ["0", "1", "2", "3", "4", "5"],
         [
-            "Command:",
-            ", Timeout:",
+            "Command=",
+            ", Timeout=",
             ["", "e", ", Use Root"],
-            ", Store Output In:",
-            ", Store Errors In:",
-            ", Timeout:",
+            ", Store Output In=",
+            ", Store Errors In=",
+            ", Timeout=",
             ["", "e", ", Use Task Set0tings"],
         ],
     ),
     "1246578872t": ActionCode(0, "1040876951t", [], [], "AutoWear Notification", [], []),
     "124t": ActionCode(0, "", [], [], "Remount", [], []),
     "1250249549t": ActionCode(0, "1040876951t", [], [], "AutoInput Screen Off/On", [], []),
     "1256900802t": ActionCode(0, "1040876951t", [], [], "Termux", [], []),
@@ -174,39 +175,39 @@
     "125t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Str", "Str"],
         "Compose Email",
         ["0", "1", "2"],
-        ["Recipient(s):", ", Subject:", ", Message:"],
+        ["Recipient(s)=", ", Subject=", ", Message="],
     ),
     "126t": ActionCode(
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["Str", "Int", "Int", "Int", "Str", "ConditionList"],
         "Return",
         ["0", "1", "2", "3", "4"],
         [
-            "Value:",
+            "Value=",
             ["", "e", ", Stop"],
             ["", "e", ", Local Variable Passthrough"],
             ["", "e", ", Replace On Passthrough"],
-            ", Limit Passthrough To:",
+            ", Limit Passthrough To=",
         ],
     ),
     "129t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Str", "Str", "Int", "Int", "ConditionList"],
         "JavaScriptLet",
         ["0", "1", "2", "3"],
-        ["Code:", ", Libraries:", ["", "e", ", Auto Exit"], ", Timeout:"],
+        ["Code=", ", Libraries=", ["", "e", ", Auto Exit"], ", Timeout="],
     ),
     "12s": ActionCode(0, "", [], [], "HDMI Plugged", [], []),
     "1304982781t": ActionCode(0, "1040876951t", [], [], "AutoTools Dialog", [], []),
     "130t": ActionCode(
         12,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11"],
@@ -223,143 +224,143 @@
             "Int",
             "Int",
             "ConditionList",
         ],
         "Perform Task",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "10"],
         [
-            "Name:",
-            ", Priority:",
-            ", Parameter 1:",
-            ", Parameter 2:",
-            ", Return Value Variable:",
+            "Name=",
+            ", Priority=",
+            ", Parameter 1=",
+            ", Parameter 2=",
+            ", Return Value Variable=",
             ["", "e", ", Stop"],
             ["", "e", ", Local Variable Passthrough"],
-            ", Limit Passthrough To:",
+            ", Limit Passthrough To=",
             ["", "e", ", Reset Return Variable"],
             ["", "e", ", Allow Overwrite Variables"],
             ["", "e", ", Structure Output (JSON, etc)"],
         ],
     ),
     "131t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Str", "Int", "Int"],
         "JavaScript",
         ["0", "1", "2"],
-        ["Path:", ", Libraries:", ["", "e", ", Auto Exit"], ", Timeout:"],
+        ["Path=", ", Libraries=", ["", "e", ", Auto Exit"], ", Timeout="],
     ),
     "1339942270t": ActionCode(0, "1040876951t", [], [], "SharpTools Thing", [], []),
     "133t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Int", "Int"],
         "Set Tasker Pref",
         ["0", "1"],
-        [["Set:", "l", "133"], ", Value:"],
+        [["Set=", "l", "133"], ", Value="],
     ),
     "1339291165t": ActionCode(0, "1040876951t", [], [], "AutoWeb Download", [], []),
     "1344888481e": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Bundle", "Str", "Str", "Int"],
         "Notification Listener",
         ["0", "3"],
         ["", ["", "e", ", Structure Output (JSON, etc)"]],
     ),
     "134e": ActionCode(0, "", [], [], "Card Mounted", [], []),
-    "134t": ActionCode(1, "", ["0"], ["Str"], "Query Action", ["0"], ["Action:"]),
+    "134t": ActionCode(1, "", ["0"], ["Str"], "Query Action", ["0"], ["Action="]),
     "135e": ActionCode(0, "", [], [], "Card Unmounted", [], []),
     "135s": ActionCode(0, "", [], [], "Auto-Sync", [], []),
     "135t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Int", "Int", "Str", "ConditionList"],
         "Go To",
         ["0", "1", "2"],
-        [["Set:", "l", "135"], ", Number:", ", Label:"],
+        [["Set=", "l", "135"], ", Number=", ", Label="],
     ),
     "136e": ActionCode(0, "", [], [], "Card Removed", [], []),
     "136s": ActionCode(0, "", [], [], "VPN Connected", [], []),
-    "136t": ActionCode(1, "", ["0"], ["Int"], "Sound Effects", ["0"], [["Set:", "l", "switch_set"]]),
+    "136t": ActionCode(1, "", ["0"], ["Int"], "Sound Effects", ["0"], [["Set=", "l", "switch_set"]]),
     "137t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Str", "ConditionList"],
         "Stop",
         ["0", "1"],
-        [["", "e", "Stop"], ", Task:"],
+        [["", "e", "Stop"], " Task="],
     ),
-    "138t": ActionCode(1, "", ["0"], ["Img"], "Set Tasker Icon", ["0"], ["Icon:"]),
+    "138t": ActionCode(1, "", ["0"], ["Img"], "Set Tasker Icon", ["0"], ["Icon="]),
     "139t": ActionCode(0, "", [], [], "Disable (Tasker)", [], []),
     "140618776t": ActionCode(0, "1040876951t", [], [], "AutoWear Toast", [], []),
     "140s": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "Int"],
         "Battery Level",
         ["0", "1"],
-        ["From:", ", To:"],
+        ["From=", ", To="],
     ),
     "140t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Str"],
         "Change Icon Set",
         ["0", "1"],
-        ["Old:", ", New:"],
+        ["Old=", ", New="],
     ),
     "1410790256t": ActionCode(0, "1040876951t", [], [], "AutoWear Floating Icon", [], []),
     "141s": ActionCode(0, "", [], [], "Battery Temperature", [], []),
     "1411074191t": ActionCode(0, "1040876951t", [], [], "AutoSheets Add Rows", [], []),
-    "142s": ActionCode(2, "", ["0", "1"], ["Str", "Str"], "Profile Active", ["0"], ["Name:"]),
+    "142s": ActionCode(2, "", ["0", "1"], ["Str", "Str"], "Profile Active", ["0"], ["Name="]),
     "142t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Str"],
         "Edit Task",
         ["0", "1"],
-        ["Task:", ", Action:"],
+        ["Task=", ", Action="],
     ),
-    "143s": ActionCode(2, "", ["0", "1"], ["Str", "Str"], "Task Running", ["0"], ["Name:"]),
+    "143s": ActionCode(2, "", ["0", "1"], ["Str", "Str"], "Task Running", ["0"], ["Name="]),
     "143t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Str"],
         "Edit Scene",
         ["0", "1"],
-        ["Scene Name:", ", Element:"],
+        ["Scene Name=", ", Element="],
     ),
     "144741820t": ActionCode(0, "1040876951t", [], [], "AutoNotification Hide Notification Icons", [], []),
     "1446679033t": ActionCode(0, "1040876951t", [], [], "AutoTools Time", [], []),
     "1446874931t": ActionCode(0, "1040876951t", [], [], "AutoTools Json Read", [], []),
     "1447159672t": ActionCode(0, "1040876951t", [], [], "AutoTools Text", [], []),
     "1447244736t": ActionCode(0, "1040876951t", [], [], "AutoTools Action Wait", [], []),
     "1446697909t": ActionCode(0, "1040876951t", [], [], "AutoWear Dialog", [], []),
     "145s": ActionCode(0, "", [], [], "Signal Strength", [], []),
     "1452528931t": ActionCode(0, "1040876951t", [], [], "AutoContacts Query 2.0", [], []),
     "1461810131t": ActionCode(0, "1040876951t", [], [], "AutoSheets Update Cells", [], []),
     "147s": ActionCode(0, "", [], [], "Unread Text", [], []),
-    "147t": ActionCode(1, "", ["0"], ["Int"], "Show Prefs", ["0"], [["Section:", "l", "147"]]),
+    "147t": ActionCode(1, "", ["0"], ["Int"], "Show Prefs", ["0"], [["Section=", "l", "147"]]),
     "148s": ActionCode(0, "", [], [], "Pen Out", [], []),
     "148t": ActionCode(0, "", [], [], "Show Runlog", [], []),
     "1482108003t": ActionCode(0, "1040876951t", [], [], "AutoSpotify Player State", [], []),
     "149s": ActionCode(0, "", [], [], "Pen Menu", [], []),
     "14s": ActionCode(0, "", [], [], "Power Save Mode", [], []),
     "1508929357t": ActionCode(0, "1040876951t", [], [], "AutoTools Array", [], []),
-    "150s": ActionCode(1, "", ["0"], ["Int"], "USB Connected", ["0"], [["Is:", "l", "150s"]]),
+    "150s": ActionCode(1, "", ["0"], ["Int"], "USB Connected", ["0"], [["Is=", "l", "150s"]]),
     "150t": ActionCode(0, "", [], [], "Keyguard", [], []),
     "1520257414e": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Bundle", "Str", "Str", "Int"],
         "AutoNotification Intercept",
@@ -369,96 +370,96 @@
     "152t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Img"],
         "Set Widget Icon",
         ["0", "1"],
-        ["Name:", ", Icon:"],
+        ["Name=", ", Icon="],
     ),
     "153t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Int", "Str"],
         "Import Data",
         ["0", "1", "2"],
-        [["Type:", "l", "153"], ["Source:", "l", "153a"], ", Variable:"],
+        [["Type=", "l", "153"], ["Source=", "l", "153a"], ", Variable="],
     ),
     "154s": ActionCode(0, "", [], [], "Active User", [], []),
     "155t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Str"],
         "Set Widget Label",
         ["0", "1"],
-        ["Name:", ", Label:"],
+        ["Name=", ", Label="],
     ),
     "1563355455t": ActionCode(0, "1040876951t", [], [], "AutoNotification Buttons Notification", [], []),
     "1563799945t": ActionCode(0, "1040876951t", [], [], "Secure Settings", [], []),
     "156t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Int", "Int", "Int", "Str"],
         "MIDI Play",
         ["0", "1", "2", "3"],
         [
-            ["Format:", "l", "156"],
-            ["Locality:", "l", "156a"],
-            ", Best Timing:",
-            ", Score:",
+            ["Format=", "l", "156"],
+            ["Locality=", "l", "156a"],
+            ", Best Timing=",
+            ", Score=",
         ],
     ),
     "157t": ActionCode(0, "", [], [], "Quick Setting Add", [], []),
     "158t": ActionCode(0, "", [], [], "Quick Setting Remove", [], []),
     "159t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Int", "ConditionList"],
         "Profile Status",
         ["0", "1"],
-        ["Name:", ["Set:", "l", "switch_set"]],
+        ["Name=", ["Set=", "l", "switch_set"]],
     ),
     "15t": ActionCode(
         7,
         "",
         ["0", "1", "2", "3", "4", "5", "6"],
         ["Str", "Str", "Int", "Int", "Int", "Str", "Str"],
         "Lock",
         ["2", "3", "4", "5", "6"],
         [
             ["", "e", "Allow Cancel"],
             ["", "e", "Remember Till Off"],
             ["", "e", "Full Screen"],
-            ", Background Image:",
-            ", Layout:",
+            ", Background Image=",
+            ", Layout=",
         ],
     ),
     "160s": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Str", "Str", "Int"],
         "Wifi Connected",
         ["0", "1", "2", "3"],
-        ["SSID:", ", MAC:", ", IP", ["Active:", "l", "160"]],
+        ["SSID=", ", MAC=", ", IP", ["Active=", "l", "160"]],
     ),
     "1600958131t": ActionCode(0, "1040876951t", [], [], "AutoBubbles Create Bubble", [], []),
     "161s": ActionCode(0, "", [], [], "Ethernet Connect", [], []),
     "161t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Str", "Str", "Str"],
         "Setup App Shortcuts",
         ["0", "1", "2", "3"],
-        ["Task:", ", Task:", ", Task:", ", Task:"],
+        ["Task=", ", Task=", ", Task=", ", Task="],
     ),
     "1620773086t": ActionCode(0, "1040876951t", [], [], "SharpTools A Thing", [], []),
     "162t": ActionCode(
         13,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11", "12"],
         [
@@ -475,41 +476,41 @@
             "Str",
             "Str",
             "Str",
         ],
         "Setup Quick Setting Tile",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11", "12"],
         [
-            ["Number:", "l", "162"],
-            ", Task:",
-            [", Status:", "l", "162a"],
+            ["Number=", "l", "162"],
+            ", Task=",
+            [", Status=", "l", "162a"],
             ["", "e", ", Can Use On Locked Device"],
-            ", Long Click Task:",
-            ", Double Click Task:",
-            ", Subtitle:",
-            ", Icon:",
-            ", Label:",
-            ", Command:",
-            ", Long Click Command:",
-            ", Double Click Command:",
-            ", Command Prefix:",
+            ", Long Click Task=",
+            ", Double Click Task=",
+            ", Subtitle=",
+            ", Icon=",
+            ", Label=",
+            ", Command=",
+            ", Long Click Command=",
+            ", Double Click Command=",
+            ", Command Prefix=",
         ],
     ),
     "1643249237t": ActionCode(0, "1040876951t", [], [], "Tools & AmazFit", [], []),
     "1644316156t": ActionCode(0, "1040876951t", [], [], "AutoNotification Reply", [], []),
     "1646792910t": ActionCode(0, "1040876951t", [], [], "AutoTools Secure Settings", [], []),
     "165s": ActionCode(1, "", ["0"], ["ConditionList"], "Variable Value", [], []),
     "165t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Int", "Int", "Int", "Str"],
         "Cancel Alarm",
         ["0", "1"],
-        [["Mode:", "l", "165"], ", Minutes:"],
+        [["Mode=", "l", "165"], ", Minutes="],
     ),
     "166160670t": ActionCode(0, "1040876951t", [], [], "AutoVoice Natural Language", [], []),
     "1664218170e": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Bundle", "Str", "Str", "Int"],
@@ -553,54 +554,55 @@
     "171t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Int", "Int", "Int", "Int", "ConditionList"],
         "Beep",
         ["0", "1", "2", "3"],
-        ["Frequency:", ", Duration:", ", Amplitude", ["Stream:", "l", "171"]],
+        ["Frequency=", ", Duration=", ", Amplitude", ["Stream=", "l", "171"]],
     ),
     "172t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Str", "Int", "Int", "Int", "Int"],
         "Morse",
         ["0", "1", "2", "3", "4"],
         [
-            "Text:",
-            ", Frequency:",
-            ", Speed:",
-            ", Amplitude:",
-            [", Stream:", "l", "171"],
+            "Text=",
+            ", Frequency=",
+            ", Speed=",
+            ", Amplitude=",
+            [", Stream=", "l", "171"],
         ],
     ),
     "1732635924t": ActionCode(0, "1040876951t", [], [], "AutoInput Action", [], []),
     "173t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "App"],
         "Network Access",
         ["0"],
-        [["Mode:", "l", "173"]],
+        [["Mode=", "l", "173"]],
     ),
     "175s": ActionCode(0, "", [], [], "Dreaming", [], []),
-    "175t": ActionCode(1, "", ["0"], ["Int"], "Power Mode", ["0"], [["Mode:", "l", "175"]]),
+    "175t": ActionCode(1, "", ["0"], ["Int"], "Power Mode", ["0"], [["Mode=", "l", "175"]]),
     "1754437993t": ActionCode(0, "1040876951t", [], [], "AutoVoice Recognition", [], []),
     "176t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Int"],
         "Take Screenshot",
         ["0", "1"],
-        ["File:", ["", "e", ", Insert In Gallery"]],
+        ["File=", ["", "e", ", Insert In Gallery"]],
     ),
-    "177t": ActionCode(1, "", ["0"], ["Int"], "Haptic Feedback", ["0"], [["Set:", "l", "switch_set"]]),
+    "1764880755t": ActionCode(0, "1040876951t", [], [], "AutoCast Best Guess", [], []),
+    "177t": ActionCode(1, "", ["0"], ["Int"], "Haptic Feedback", ["0"], [["Set=", "l", "switch_set"]]),
     "1788518030e": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Bundle", "Str", "Str", "Int"],
         "AutoInput Key",
         ["0", "3"],
@@ -617,25 +619,27 @@
         ["0", "1", "2", "3"],
         ["Bundle", "Str", "Str", "Int"],
         "AutoNotification",
         ["0", "3"],
         ["", ["", "e", ", Structure Output (JSON, etc)"]],
     ),
     "182s": ActionCode(0, "", [], [], "Heart Rate", [], []),
+    "1828597236t": ActionCode(0, "1040876951t", [], [], "AutoCast App", [], []),
+    "1831781712t": ActionCode(0, "1040876951t", [], [], "AutoCast Settings", [], []),
     "1830656901t": ActionCode(0, "1040876951t", [], [], "AutoWear List Screens", [], []),
     "1830829821t": ActionCode(0, "1040876951t", [], [], "AutoWear 4 Screen", [], []),
     "185s": ActionCode(0, "", [], [], "Humidity", [], []),
     "185t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "Int"],
         "Filter Image",
         ["0", "1"],
-        [["Mode:", "l", "185"], ", Threshold:"],
+        [["Mode=", "l", "185"], ", Threshold="],
     ),
     "1861978578e": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Bundle", "Str", "Str", "Int"],
         "AutoWear Command/Command Filter",
@@ -646,41 +650,40 @@
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["Int", "Str", "Str", "Int", "Str", "ConditionList"],
         "Custom Setting",
         ["0", "1", "2", "3", "4"],
         [
-            ["Test:", "l", "235"],
-            ", Name:",
-            ", Value:",
+            ["Test=", "l", "235"],
+            ", Name=",
+            ", Value=",
             ["", "e", "Use Root"],
-            ", Read Setting To:",
+            ", Read Setting To=",
         ],
     ),
     "187t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Int", "Int"],
         "Save Image",
         ["0", "1", "2"],
-        ["File:", ", Image Quality:", ["", "e", ", Delete From Memory After"]],
+        ["File=", ", Image Quality=", ["", "e", ", Delete From Memory After"]],
     ),
     "1879487834t": ActionCode(0, "1040876951t", [], [], "AutoLocation Geofences", [], []),
-    "1957670352t": ActionCode(0, "1040876951t", [], [], "AutoLocation", [], []),
     "188s": ActionCode(3, "", ["0", "1", "2"], ["Img", "Int", "Int"], "Dark Mode", [], []),
     "188t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Img", "Int", "Int"],
         "Load Image",
         ["0", "1", "2"],
-        ["Source:", ", Max Width or Height:", ["", "e", ", Respect EXIF Orientation"]],
+        ["Source=", ", Max Width or Height=", ["", "e", ", Respect EXIF Orientation"]],
     ),
     "18927444e": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Bundle", "Str", "Str", "Int"],
         "AutoApps Command",
@@ -691,31 +694,31 @@
         4,
         "",
         ["0", "1", "2", "3"],
         ["Int", "Int", "Int", "Int"],
         "Crop Image",
         ["0", "1", "2", "3"],
         [
-            "From Left (%):",
-            ", From Right (%):",
-            ", From Top (%):",
-            ", From Bottom (%):",
+            "From Left (%)=",
+            ", From Right (%)=",
+            ", From Top (%)=",
+            ", From Bottom (%)=",
         ],
     ),
     "18t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["App", "Int"],
         "Kill App",
         ["0", "1"],
-        [["a", "", "App:"], ["", "e", "Use Root"]],
+        [["a", "", "App="], ["", "e", "Use Root"]],
     ),
     "190s": ActionCode(0, "", [], [], "Any Sensor", [], []),
-    "190t": ActionCode(1, "", ["0"], ["Int"], "Flip Image", ["0"], [["Direction:", "l", "190"]]),
+    "190t": ActionCode(1, "", ["0"], ["Int"], "Flip Image", ["0"], [["Direction=", "l", "190"]]),
     "1910383148t": ActionCode(0, "1040876951t", [], [], "AutoTools Regex", [], []),
     "1912522764t": ActionCode(0, "1040876951t", [], [], "AutoTools Toast", [], []),
     "191971507t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Bundle", "Str", "Str", "Int", "Int"],
@@ -726,52 +729,53 @@
     "191t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "Int"],
         "Rotate Image",
         ["0", "1"],
-        [["Direction:", "l", "191"], [", Degrees:", "l", "191a"]],
+        [["Direction=", "l", "191"], [", Degrees=", "l", "191a"]],
     ),
     "192s": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Bundle", "Str"],
         "Matter Light",
         ["1"],
-        ["Device IDs/Names:"],
+        ["Device IDs/Names="],
     ),
     "192t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Str", "Int"],
         "Play Ringtone",
         ["0", "1", "2"],
-        [["Direction:", "l", "192"], ", Sound:", [", Stream:", "l", "171"]],
+        [["Direction=", "l", "192"], ", Sound=", [", Stream=", "l", "171"]],
     ),
+    "1928381944t": ActionCode(0, "1040876951t", [], [], "AutoCast Control Media", [], []),
     "193t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "Int"],
         "Resize Image",
         ["0", "1"],
-        ["Width:", ", Height:"],
+        ["Width=", ", Height="],
     ),
     "194s": ActionCode(0, "", [], [], "Work Profile", [], []),
     "194t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Int", "Str"],
         "Test Scene",
         ["0", "1", "2"],
-        ["Name:", [", Test:", "l", "194"], ", Store Result In:"],
+        ["Name=", [", Test=", "l", "194"], ", Store Result In="],
     ),
     "1957670352t": ActionCode(0, "1040876951t", [], [], "AutoWear App", [], []),
     "1957681000e": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Bundle", "Str", "Str", "Int"],
@@ -783,47 +787,47 @@
     "195t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Str", "Int", "Str"],
         "Test Element",
         ["0", "1", "2", "3"],
-        ["Scene Name:", ", Element:", [", Test:", "l", "195"], ", Store Result In:"],
+        ["Scene Name=", ", Element=", [", Test=", "l", "195"], ", Store Result In="],
     ),
     "197t": ActionCode(0, "", [], [], "Developer Settings", [], []),
     "198t": ActionCode(0, "", [], [], "Device Info Settings", [], []),
     "199t": ActionCode(0, "", [], [], "Add Account Settings", [], []),
     "199558826t": ActionCode(0, "1040876951t", [], [], "TouchTask Gestures", [], []),
     "2000e": ActionCode(
         2,
         "",
         ["0", "1"],
         ["App", "Str"],
         "Notification Click",
         ["0", "1"],
-        ["Owner Application:", ", Title:"],
+        ["Owner Application=", ", Title="],
     ),
     "2003e": ActionCode(0, "", [], [], "Missed Call", [], []),
     "2005e": ActionCode(0, "", [], [], "SMS Success", [], []),
     "200t": ActionCode(0, "", [], [], "All Settings", [], []),
     "2010e": ActionCode(0, "", [], [], "SMS Failure", [], []),
     "201e": ActionCode(
         4,
         "",
         ["0", "1", "2", "3", "4"],
         ["App", "Str", "Str", "Str"],
         "Assistance Request",
         ["0", "1", "2", "3"],
-        ["App:", ", URL:", ", Texts:", ", Extras:", [", Priority:", "4s"]],
+        ["App=", ", URL=", ", Texts=", ", Extras=", [", Priority=", "4s"]],
     ),
     "201t": ActionCode(0, "", [], [], "Airplane Mode Settings", [], []),
     "2010186613t": ActionCode(0, "1040876951t", [], [], "AutoSheets Delete Cell Content", [], []),
     "202t": ActionCode(0, "", [], [], "APN Settings", [], []),
     "2022280279t": ActionCode(0, "1040876951t", [], [], "AutoNotification Media", [], []),
-    "203e": ActionCode(0, "", [], [], "Battery Changed", ["0"], [["Priority:", "l", "4s"]]),
+    "203e": ActionCode(0, "", [], [], "Battery Changed", ["0"], [["Priority=", "l", "4s"]]),
     "203t": ActionCode(0, "", [], [], "Date Settings", [], []),
     "2046367074t": ActionCode(0, "1040876951t", [], [], "AutoNotification Cancel", [], []),
     "2041559229t": ActionCode(0, "1040876951t", [], [], "AutoSpotify Playlists", [], []),
     "204t": ActionCode(0, "", [], [], "Internal Storage Settings", [], []),
     "2050e": ActionCode(0, "", [], [], "Quick Setting Clicked", [], []),
     "205e": ActionCode(0, "", [], [], "Battery Full", [], []),
     "2051074546t": ActionCode(0, "1040876951t", [], [], "AutoSpotify Control Media", [], []),
@@ -832,115 +836,115 @@
     "2075e": ActionCode(
         2,
         "",
         ["0", "1", "2"],
         ["Int", "Str", "Str"],
         "Custom Setting",
         ["0", "1", "2"],
-        [["Type:", "l", "235"], ", Name:", ", Value:"],
+        [["Type=", "l", "235"], ", Name=", ", Value="],
     ),
-    "2076e": ActionCode(2, "", ["0", "1"], ["Str", "Str"], "NFC Tag", ["0", "1"], ["ID:", ", Content:"]),
+    "2076e": ActionCode(2, "", ["0", "1"], ["Str", "Str"], "NFC Tag", ["0", "1"], ["ID=", ", Content="]),
     "2077e": ActionCode(1, "", ["0"], ["Bundle"], "Secondary App Opened", [], []),
-    "2078e": ActionCode(2, "", ["0", "1"], ["Bundle", "Str"], "App Changed", ["1"], ["Package:"]),
+    "2078e": ActionCode(2, "", ["0", "1"], ["Bundle", "Str"], "App Changed", ["1"], ["Package="]),
     "2079e": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "Str"],
         "Volume Long Press",
         ["0", "1"],
-        [["Type:", "l", "2079e"], ", Additional Time:"],
+        [["Type=", "l", "2079e"], ", Additional Time="],
     ),
     "2080e": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Bundle", "Str", "Str", "ConditionList"],
         "BT Connected",
         ["1", "2"],
-        ["Name:", ", Address:"],
+        ["Name=", ", Address="],
     ),
     "2081e": ActionCode(
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["Bundle", "Str", "Str", "Str", "Str", "Int"],
         "Music Track Changed",
         ["1", "2", "3", "4", "5"],
-        ["Track:", ", Album:", ", Artist", ", Package:", [", Type:", "l", "2081e"]],
+        ["Track=", ", Album=", ", Artist", ", Package=", [", Type=", "l", "2081e"]],
     ),
     "2083e": ActionCode(0, "", [], [], "Significant Motion", [], []),
     "2084e": ActionCode(0, "", [], [], "Alarm Changed", [], []),
     "2085e": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Bundle", "Str", "Str", "Int"],
         "Logcat Entry",
         ["1", "2", "3"],
-        ["Component:", ", Filter:", ["", "e", ", Grep Filter"]],
+        ["Component=", ", Filter=", ["", "e", ", Grep Filter"]],
     ),
     "2088e": ActionCode(0, "", [], [], "Any Sensor", [], []),
     "2089e": ActionCode(
         8,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7"],
         ["Bundle", "Int", "Str", "Str", "Str", "Int", "Int", "Str"],
         "HTTP Request",
         ["1", "2", "3", "4", "5", "6", "7"],
         [
-            "Port:",
-            ", Method:",
-            ", Path:",
+            "Port=",
+            ", Method=",
+            ", Path=",
             ", Quick Response",
-            ", Timeout:",
+            ", Timeout=",
             ["", "e", ", Only On Wifi"],
-            ", Network Name/MAC Address:",
+            ", Network Name/MAC Address=",
         ],
     ),
-    "208e": ActionCode(0, "", 0, [], "Display On", ["0"], [["Priority:", "l", "4s"]]),
+    "208e": ActionCode(0, "", 0, [], "Display On", ["0"], [["Priority=", "l", "4s"]]),
     "208t": ActionCode(0, "", [], [], "Location Settings", [], []),
     "2091e": ActionCode(
         6,
         "",
         ["0", "1", "2", "3"],
         ["Bundle", "Str", "Str", "Int"],
         "Logcat Entry",
         ["1", "2", "3"],
-        ["Component:", ", Filter:", ["", "e", ", Grep Filter"]],
+        ["Component=", ", Filter=", ["", "e", ", Grep Filter"]],
     ),
     "2092e": ActionCode(0, "", [], [], "Power Menu Shown", [], []),
-    "2093e": ActionCode(1, "", ["0"], ["App", "Str"], "Assistant Action", ["0"], ["Command:"]),
+    "2093e": ActionCode(1, "", ["0"], ["App", "Str"], "Assistant Action", ["0"], ["Command="]),
     "2094e": ActionCode(0, "", [], [], "Call Screened", [], []),
-    "2095e": ActionCode(2, "", ["0", "1"], ["Bundle", "Str"], "Tick", ["1"], ["Interval (ms):"]),
+    "2095e": ActionCode(2, "", ["0", "1"], ["Bundle", "Str"], "Tick", ["1"], ["Interval (ms)="]),
     "2096e": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Bundle", "Int", "Int", "Int"],
         "Sleeping",
         ["1", "2", "3"],
-        ["Minimum Confidence:", ", Maximum Light:", ", Maximum Motion:"],
+        ["Minimum Confidence=", ", Maximum Light=", ", Maximum Motion="],
     ),
     "20t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["App", "Str", "Int", "Int", "ConditionList"],
         "Launch App",
         ["0", "1", "2", "3"],
         [
-            ["a", "", "App:"],
-            ", Data:",
+            ["a", "", "App="],
+            ", Data=",
             ["", "e", "Exclude From Recent Apps"],
             ["", "e", "Always Start New Copy"],
             ["if"],
         ],
     ),
-    "210e": ActionCode(0, "", 0, [], "Display Off", ["0"], [["Priority:", "l", "4s"]]),
+    "210e": ActionCode(0, "", 0, [], "Display Off", ["0"], [["Priority=", "l", "4s"]]),
     "210t": ActionCode(0, "", [], [], "Input Method Settings", [], []),
     "211t": ActionCode(0, "", [], [], "Sync Settings", [], []),
     "211707263t": ActionCode(0, "1040876951t", [], [], "Global Actions", [], []),
     "211905330t": ActionCode(0, "1040876951t", [], [], "AutoContacts", [], []),
     "2114100406t": ActionCode(0, "1040876951t", [], [], "AutoLaunch Query", [], []),
     "212t": ActionCode(0, "", [], [], "WiFi IP Settings", [], []),
     "2132875086t": ActionCode(0, "1040876951t", [], [], "AutoSheets Delete Rows/Columns", [], []),
@@ -949,15 +953,15 @@
     "215e": ActionCode(0, "", [], [], "Button: Camera", [], []),
     "216e": ActionCode(0, "", [], [], "Button: Long Search", [], []),
     "216t": ActionCode(2, "", ["0", "1"], ["Str", "ConditionList"], "App Settings", ["0"], ["App"]),
     "218t": ActionCode(0, "", [], [], "Bluetooth Settings", [], []),
     "219t": ActionCode(0, "", [], [], "Quick Settings", [], []),
     "220e": ActionCode(0, "", [], [], "File Moved", [], []),
     "220t": ActionCode(0, "", [], [], "Mobile Data Settings", [], []),
-    "222e": ActionCode(0, "", 0, [], "File Modified", ["0", "1"], ["File:", ", Event:"]),
+    "222e": ActionCode(0, "", 0, [], "File Modified", ["0", "1"], ["File=", ", Event="]),
     "222t": ActionCode(0, "", [], [], "Display Settings", [], []),
     "224e": ActionCode(0, "", [], [], "File Closed", [], []),
     "224t": ActionCode(0, "", [], [], "Locale Settings", [], []),
     "226e": ActionCode(0, "", [], [], "File Opened", [], []),
     "226t": ActionCode(0, "", [], [], "App Manager Settings", [], []),
     "227t": ActionCode(0, "", [], [], "Memory Card Settings", [], []),
     "228e": ActionCode(0, "", [], [], "File Deleted", [], []),
@@ -974,19 +978,19 @@
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["Int", "Str", "Str", "Int", "Str", "ConditionList"],
         "Custom Settings",
         ["0", "1", "2", "3", "4"],
         [
-            ["Test:", "l", "235"],
-            ", Name:",
-            ", Value:",
+            ["Test=", "l", "235"],
+            ", Name=",
+            ", Value=",
             ["", "e", "Use Root"],
-            ", Read Setting To:",
+            ", Read Setting To=",
         ],
     ),
     "236t": ActionCode(0, "", [], [], "Accessibility Settings", [], []),
     "237t": ActionCode(0, "", [], [], "Notification Listener Settings", [], []),
     "238t": ActionCode(0, "", [], [], "Privacy Settings", [], []),
     "239t": ActionCode(0, "", [], [], "Print Settings", [], []),
     "24081025t": ActionCode(0, "1040876951t", [], [], "AutoNotification Snooze", [], []),
@@ -997,292 +1001,292 @@
     "248t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "Int"],
         "Turn Off",
         ["0", "1"],
-        ["File:", ["", "e", "Dim"], ["", "e", ", Lock"]],
+        ["File=", ["", "e", "Dim"], ["", "e", ", Lock"]],
     ),
     "249t": ActionCode(0, "", [], [], "System Screenshot", [], []),
     "250t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Str"],
         "Compose SMS",
         ["0", "1"],
-        ["Recipient(s):", "Message:"],
+        ["Recipient(s)=", "Message="],
     ),
     "251t": ActionCode(0, "", [], [], "Battery Settings", [], []),
-    "252t": ActionCode(1, "", ["0"], ["App"], "Set SMS App", ["0"], ["App:"]),
-    "254t": ActionCode(1, "", ["0"], ["Int"], "Speakerphone", ["0"], [["Set:", "l", "switch_set"]]),
-    "256t": ActionCode(1, "", ["0"], ["Int"], "Vibrate On Ringer", ["0"], [["Set:", "l", "switch_set"]]),
+    "252t": ActionCode(1, "", ["0"], ["App"], "Set SMS App", ["0"], ["App="]),
+    "254t": ActionCode(1, "", ["0"], ["Int"], "Speakerphone", ["0"], [["Set=", "l", "switch_set"]]),
+    "256t": ActionCode(1, "", ["0"], ["Int"], "Vibrate On Ringer", ["0"], [["Set=", "l", "switch_set"]]),
     "257t": ActionCode(0, "", [], [], "Power Usage Settings", [], []),
     "258t": ActionCode(0, "", [], [], "Vibrate On Notify", [], []),
     "259t": ActionCode(
         1,
         "",
         ["0"],
         ["Int"],
         "Notification Pulse",
         ["0"],
-        [["Set:", "l", "switch_set"]],
+        [["Set=", "l", "switch_set"]],
     ),
     "25t": ActionCode(0, "", [], [], "Go Home", [], []),
     "260559060t": ActionCode(0, "1040876951t", [], [], "AutoNotification Block", [], []),
     "263029931t": ActionCode(0, "1040876951t", [], [], "AutoInput Unlock Screen", [], []),
     "268157305t": ActionCode(0, "1040876951t", [], [], "AutoNotification Tiles", [], []),
     "294t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "ConditionList"],
         "Bluetooth",
         ["0"],
-        [["Set:", "l", "switch_set"]],
+        [["Set=", "l", "switch_set"]],
     ),
-    "295t": ActionCode(1, "", ["0"], ["Str"], "Bluetooth ID", ["0"], ["Name:"]),
-    "296t": ActionCode(1, "", ["0"], ["Int"], "Bluetooth Voice", ["0"], [["Set:", "l", "switch_set"]]),
+    "295t": ActionCode(1, "", ["0"], ["Str"], "Bluetooth ID", ["0"], ["Name="]),
+    "296t": ActionCode(1, "", ["0"], ["Int"], "Bluetooth Voice", ["0"], [["Set=", "l", "switch_set"]]),
     "2e": ActionCode(0, "", [], [], "Phone Offhook", [], []),
     "2s": ActionCode(
         1,
         "",
         ["0"],
         ["Int"],
         "Mobile Data Settings",
         ["0"],
-        [["Set:", "l", "switch_set"]],
+        [["Set=", "l", "switch_set"]],
     ),
     "3000e": ActionCode(0, "", [], [], "Gesture", [], []),
     "3001e": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Int", "Int"],
         "Shake",
         ["0", "1", "2"],
         [
-            ["Axis:", "l", "3001e"],
-            ["Sensitivity:", "l", "3001ea"],
-            ["Duration:", "l", "3001eb"],
+            ["Axis=", "l", "3001e"],
+            ["Sensitivity=", "l", "3001ea"],
+            ["Duration=", "l", "3001eb"],
         ],
     ),
     "300e": ActionCode(0, "", [], [], "Date Set", [], []),
-    "300t": ActionCode(1, "", ["0"], ["Int"], "Anchor", ["0"], ["Label"]),
+    "300t": ActionCode(1, "", ["0"], ["Str"], "Anchor", ["0"], ["Label"]),
     "301t": ActionCode(0, "", [], [], "Mic Mute", [], []),
     "302e": ActionCode(0, "", [], [], "Time/Date Set", [], []),
     "303e": ActionCode(0, "", [], [], "Timer Change", [], []),
     "303t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Int", "Int"],
         "Alarm Volume",
         ["0", "1", "2"],
-        ["Level:", ["", "e", ", Display"], ["", "e", ", Sound"]],
+        ["Level=", ["", "e", ", Display"], ["", "e", ", Sound"]],
     ),
     "304e": ActionCode(0, "", [], [], "Timezone Set", [], []),
     "304t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Int", "Int"],
         "Ringer Volume",
         ["0", "1", "2"],
-        ["Level:", ["", "e", ", Display"], ["", "e", ", Sound"]],
+        ["Level=", ["", "e", ", Display"], ["", "e", ", Sound"]],
     ),
     "3050e": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Str", "Int"],
         "Variable Set",
         ["0", "1", "2"],
-        ["Variable:", ", Value:", ["", "e", ", User Variables Only"]],
+        ["Variable=", ", Value=", ["", "e", ", User Variables Only"]],
     ),
     "305e": ActionCode(0, "", [], [], "Alarm Clock", [], []),
     "305t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Int", "Int", "Int", "ConditionList"],
         "Notification Volume",
         ["0", "1", "2"],
-        ["Level:", ["", "e", ", Display"], ["", "e", ", Sound"]],
+        ["Level=", ["", "e", ", Display"], ["", "e", ", Sound"]],
     ),
     "3060e": ActionCode(0, "", [], [], "Variable Cleared", [], []),
     "306e": ActionCode(0, "", [], [], "Alarm Done", [], []),
     "306t": ActionCode(0, "", [], [], "In-Call Volume", [], []),
     "3071e": ActionCode(0, "", [], [], "Zoom Click", [], []),
     "307e": ActionCode(0, "", [], [], "Monitor Start", [], []),
     "307t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Int", "Int", "Int", "ConditionList"],
         "Media Volume",
         ["0", "1", "2"],
-        ["Level:", ["", "e", ", Display"], ["", "e", ", Sound"]],
+        ["Level=", ["", "e", ", Display"], ["", "e", ", Sound"]],
     ),
     "308t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Int", "Int"],
         "System Volume",
         ["0", "1", "2"],
-        ["Level:", ["", "e", ", Display"], ["", "e", ", Sound"]],
+        ["Level=", ["", "e", ", Display"], ["", "e", ", Sound"]],
     ),
     "309e": ActionCode(0, "", [], [], "Steps Taken", [], []),
     "309t": ActionCode(0, "", [], [], "DTMF Volume", [], []),
     "30s": ActionCode(
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["Int", "Int", "Int", "Int", "Int", "ConditionList"],
         "Headset Plugged",
         ["0"],
-        [["Type:", "l", "30s"]],
+        [["Type=", "l", "30s"]],
     ),
     "30t": ActionCode(
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["Int", "Int", "Int", "Int", "Int", "ConditionList"],
         "Wait",
         ["0", "1", "2", "3", "4"],
-        ["MS:", ", Seconds:", ", Minutes:", ", Hours:", ", Days:"],
+        ["MS=", ", Seconds=", ", Minutes=", ", Hours=", ", Days="],
     ),
-    "310t": ActionCode(1, "", ["0"], ["Int"], "Vibrate Mode", ["0"], [["Mode:", "l", "310"]]),
+    "310t": ActionCode(1, "", ["0"], ["Int"], "Vibrate Mode", ["0"], [["Mode=", "l", "310"]]),
     "311t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Int", "Int"],
         "BT Voice Volume",
         ["0", "1", "2"],
-        ["Level:", ["", "e", ", Display"], ["", "e", ", Sound"]],
+        ["Level=", ["", "e", ", Display"], ["", "e", ", Sound"]],
     ),
     "312t": ActionCode(
         8,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7"],
         ["Int", "Int", "Int", "Int", "Str", "Str", "Bundle", "ConditionList"],
         "Do Not Disturb",
         ["0"],
-        [["Mode:", "l", "312"]],
+        [["Mode=", "l", "312"]],
     ),
     "313t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Int", "ConditionList"],
         "Sound Mode",
         ["0", "1"],
-        [["Mode:", "l", "313"], ["", "e", ", Ignore DND"]],
+        [["Mode=", "l", "313"], ["", "e", ", Ignore DND"]],
     ),
     "314t": ActionCode(
         10,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"],
         ["Int", "Str", "Str", "Str", "Str", "Int", "Str", "Int", "Int", "Int"],
         "Authentication Dialog",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"],
         [
-            ["Type:", "l", "314"],
-            ", Title:",
-            ", Subtitle:",
-            ", Description:",
-            ", Cancel Button Text:",
-            ", Number of Attempts:",
-            ", Read Result Into:",
-            ", Timeout (Seconds):",
+            ["Type=", "l", "314"],
+            ", Title=",
+            ", Subtitle=",
+            ", Description=",
+            ", Cancel Button Text=",
+            ", Number of Attempts=",
+            ", Read Result Into=",
+            ", Timeout (Seconds)=",
             ["", "e", ", Confirmation Required"],
             ["", "e", ", Device Credentials Allowed"],
         ],
     ),
     "316t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "Str"],
         "Display Size",
         ["0", "1"],
-        [["Size:", "l", "316"], ", Manual:"],
+        [["Size=", "l", "316"], ", Manual="],
     ),
     "317t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "Bundle"],
         "NFC",
         ["0"],
-        [["Set:", "l", "switch_set"]],
+        [["Set=", "l", "switch_set"]],
     ),
     "318t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "Int"],
         "Force Rotation",
         ["0", "1"],
-        [["Mode:", "l", "318"], ["", "e", ", Alternative Method (Check Help)"]],
+        [["Mode=", "l", "318"], ["", "e", ", Alternative Method (Check Help)"]],
     ),
     "319692633t": ActionCode(0, "1040876951t", [], [], "AutoShare Process Text", [], []),
     "319t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Str"],
         "Ask Permissions",
         ["0", "1"],
-        ["Required Permissions:", ", Prompt If Not Granted:"],
+        ["Required Permissions=", ", Prompt If Not Granted="],
     ),
     "320t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Str", "Int", "Str", "Str", "Str"],
         "Ping",
         ["0", "1", "2", "3", "4"],
         [
-            ", Host:",
-            ", Number:",
-            ", Average Result Variable:",
-            ", Min Result Variable:",
-            ", Max Result Variable:",
+            ", Host=",
+            ", Number=",
+            ", Average Result Variable=",
+            ", Min Result Variable=",
+            ", Max Result Variable=",
         ],
     ),
     "321t": ActionCode(
         9,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8"],
         ["Bundle", "Str", "Str", "Str", "Str", "Str", "Int", "Int", "Str"],
         "GD Upload",
         ["1", "2", "3", "4", "5", "6", "7", "8"],
         [
-            "Google Drive/Account:",
-            ", Data/File:",
-            ", Remote File Name:",
-            ", Remote Folder:",
-            ", Content Description:",
+            "Google Drive/Account=",
+            ", Data/File=",
+            ", Remote File Name=",
+            ", Remote Folder=",
+            ", Content Description=",
             ["", "e", ", Overwrite If Exists"],
             ["", "e", ", Publicly Share File"],
-            ", Mime Type:",
+            ", Mime Type=",
         ],
     ),
     "322t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Str", "Int"],
         "Data Backup",
         ["0", "1", "2"],
-        ["Path:", ", Google Drive Account:", ["", "e", ", Include User Vars/Prefs"]],
+        ["Path=", ", Google Drive Account=", ["", "e", ", Include User Vars/Prefs"]],
     ),
     "323t": ActionCode(
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["Int", "Int", "Int", "Int", "Int", "ConditionList"],
         "Airplane Radios",
@@ -1299,149 +1303,149 @@
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["Bundle", "Str", "Int", "Int", "Str", "Str"],
         "GD List",
         ["1", "2", "3", "5"],
         [
-            "Google Drive Account:",
-            [", Type:", "l", "324"],
-            [", Files or Folders:", "l", "324a"],
-            ", Query:",
+            "Google Drive Account=",
+            [", Type=", "l", "324"],
+            [", Files or Folders=", "l", "324a"],
+            ", Query=",
         ],
     ),
     "325t": ActionCode(
         8,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7"],
         ["Bundle", "Str", "Int", "Int", "Str", "Str", "Str", "Str"],
         "GD Trash",
         ["1", "2", "3", "4", "5", "6"],
         [
-            "Google Drive Account:",
-            [", Trash Value:", "l", "325"],
-            [", Type:", "l", "325a"],
-            ", File ID:",
-            ", Path:",
-            ", Remote File Name:",
+            "Google Drive Account=",
+            [", Trash Value=", "l", "325"],
+            [", Type=", "l", "325a"],
+            ", File ID=",
+            ", Path=",
+            ", Remote File Name=",
         ],
     ),
     "326t": ActionCode(
         7,
         "",
         ["0", "1", "2", "3", "4", "5", "6"],
         ["Bundle", "Str", "Int", "Str", "Str", "Str", "Str"],
         "GD Download",
         ["1", "2", "3", "4", "5", "6"],
         [
-            "Google Drive Account:",
-            [", Type:", "l", "325a"],
-            ", File ID:",
-            ", Remote Folder:",
-            ", Remote File Name:",
-            ", Local Path:",
+            "Google Drive Account=",
+            [", Type=", "l", "325a"],
+            ", File ID=",
+            ", Remote Folder=",
+            ", Remote File Name=",
+            ", Local Path=",
         ],
     ),
     "327t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Bundle", "Str", "Int"],
         "GD Sign In",
         ["1", "2"],
-        ["Google Drive Account:", ["", "e", ", Full Access"]],
+        ["Google Drive Account=", ["", "e", ", Full Access"]],
     ),
     "328t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Bundle", "Str", "Int", "Int"],
         "Keyboard",
         ["1", "2", "3"],
-        ["Input", ", Time Between Inputs:", ["", "e", ", Don't Restore Keyboard"]],
+        ["Input", ", Time Between Inputs=", ["", "e", ", Don't Restore Keyboard"]],
     ),
     "329t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Str", "Str"],
         "Navigation Bar",
         ["0", "1", "2"],
-        ["Left:", "Center:", "Right:"],
+        ["Left=", "Center=", "Right="],
     ),
     "330t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Bundle", "Str", "Str"],
         "NFC Tag",
         ["1", "2"],
-        ["Payload To Write:", ", Payload Type:"],
+        ["Payload To Write=", ", Payload Type="],
     ),
-    "331t": ActionCode(1, "", ["0"], ["Int"], "Auto-Sync", ["0"], [["Set:", "l", "switch_set"]]),
+    "331t": ActionCode(1, "", ["0"], ["Int"], "Auto-Sync", ["0"], [["Set=", "l", "switch_set"]]),
     "332t": ActionCode(0, "", [], [], "GPS", [], []),
     "333t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "Bundle"],
         "Airplane Mode",
         ["0"],
-        [["Set:", "l", "switch_set"]],
+        [["Set=", "l", "switch_set"]],
     ),
     "334t": ActionCode(
         9,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8"],
         ["Str", "Str", "Int", "Int", "Int", "Int", "Str", "Str", "Int"],
         "Say WaveNet",
         ["0", "1", "2", "3", "4", "5", "6", "7"],
         [
-            "Test/SSML:",
-            ", Voice:",
-            [", Type:", "l", "171"],
-            ", Pitch:",
-            ", Speed:",
+            "Test/SSML=",
+            ", Voice=",
+            [", Type=", "l", "171"],
+            ", Pitch=",
+            ", Speed=",
             ["", "e", ", Continue Task Immediately"],
-            ", File:",
-            ", Override API Key:",
+            ", File=",
+            ", Override API Key=",
             ["", "e", ", Respect Audio Focus"],
         ],
     ),
     "335t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Bundle", "Str", "Str", "Int", "Int"],
         "App Info",
         ["1", "2", "3", "4"],
         [
-            "Package/App Name:",
-            ", Ignore Packages:",
+            "Package/App Name=",
+            ", Ignore Packages=",
             ["", "e", ", Ignore Unlaunchable Apps"],
             ["", "e", ", Get All Details"],
         ],
     ),
     "337t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Str"],
         "Notification Settings",
         ["0", "1"],
-        ["Package:", ", Category:"],
+        ["Package=", ", Category="],
     ),
     "338t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Bundle", "Str"],
         "Notification Category Info",
         ["1"],
-        ["Category:"],
+        ["Category="],
     ),
     "339t": ActionCode(
         14,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11", "12", "13"],
         [
             "Bundle",
@@ -1458,105 +1462,105 @@
             "Int",
             "Int",
             "ConditionList",
         ],
         "HTTP Request",
         ["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11", "12"],
         [
-            ["Method:", "l", "339"],
-            ", URL:",
-            ", Headers:",
-            ", Query Parameters:",
-            ", Body:",
-            ", File To Send:",
-            ", File/Directory To Save With Output:",
-            ", Timeout:",
+            ["Method=", "l", "339"],
+            ", URL=",
+            ", Headers=",
+            ", Query Parameters=",
+            ", Body=",
+            ", File To Send=",
+            ", File/Directory To Save With Output=",
+            ", Timeout=",
             ["", "e", ", Trust Any Certificate"],
             ["", "e", ", Automatically Follow Redirects"],
             ["", "e", ", Use Cookies"],
             ["", "e", ", Structure Output (JSON, etc)"],
         ],
     ),
     "340t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Bundle", "Int", "Str", "Int"],
         "Bluetooth Connection",
         ["1", "2", "3"],
-        [["Action:", "l", "340"], ", Device:", ", Timeout:"],
+        [["Action=", "l", "340"], ", Device=", ", Timeout="],
     ),
     "341t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Str", "Str"],
         "Test Net",
         ["0", "2"],
-        [["Type:", "l", "341"], ", Store Result In:"],
+        [["Type=", "l", "341"], ", Store Result In="],
     ),
     "342t": ActionCode(
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["Int", "Str", "Str", "Int", "Int", "ConditionList"],
         "Test File",
         ["0", "1", "2", "3"],
         [
-            ["Type:", "l", "342"],
-            ", Data:",
-            ", Store Result In:",
+            ["Type=", "l", "342"],
+            ", Data=",
+            ", Store Result In=",
             ["", "e", ", Use Root"],
         ],
     ),
     "343t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Str", "Str"],
         "Test Media",
         ["0", "1", "2"],
-        [["Type:", "l", "343"], ", Data:", ", Store Result In:"],
+        [["Type=", "l", "343"], ", Data=", ", Store Result In="],
     ),
     "344636446t": ActionCode(0, "1040876951t", [], [], "AutoVoice Trigger Alexa Routine", [], []),
     "344t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Str", "Str"],
         "Test App",
         ["0", "1", "2"],
-        [["Type:", "l", "344"], ", Data:", ", Store Result In:"],
+        [["Type=", "l", "344"], ", Data=", ", Store Result In="],
     ),
     "345t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Str", "Str"],
         "Test Variable",
         ["0", "1", "2"],
-        [["Type:", "l", "345"], ", Data:", ", Store Results In:"],
+        [["Type=", "l", "345"], ", Data=", ", Store Results In="],
     ),
     "346t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Str", "Str"],
         "Test Phone",
         ["0", "1", "2"],
-        [["Type:", "l", "346"], ", Data:", ", Store Result In:"],
+        [["Type=", "l", "346"], ", Data=", ", Store Result In="],
     ),
     "347t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Int", "Str", "Str", "ConditionList"],
         "Test Tasker",
         ["0", "1", "2"],
-        [["Type:", "l", "347"], ", Data:", ", Store Result In:"],
+        [["Type=", "l", "347"], ", Data=", ", Store Result In="],
     ),
     "34829087e": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Bundle", "Str", "Str", "Int"],
         "Tools & AmazFit",
@@ -1566,24 +1570,24 @@
     "348t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Str", "Str"],
         "Test Display",
         ["0", "1"],
-        [["Type:", "l", "348"], ", Store Result In:"],
+        [["Type=", "l", "348"], ", Store Result In="],
     ),
     "349t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Str", "Str"],
         "Test System",
         ["0", "1"],
-        [["Type:", "l", "349"], ", Store Result In:"],
+        [["Type=", "l", "349"], ", Store Result In="],
     ),
     "351t": ActionCode(
         11,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "10"],
         [
             "Bundle",
@@ -1597,218 +1601,239 @@
             "Int",
             "Str",
             "Str",
         ],
         "HTTP Auth",
         ["1", "2", "3", "4", "5", "6", "7", "8", "9", "10"],
         [
-            ["Method:", "l", "351"],
-            ", Client ID:",
-            ", Client Secret:",
-            ", Endpoint To Get Code:",
-            ", Endpoint To Get Refresh Token:",
-            ", Scopes:",
+            ["Method=", "l", "351"],
+            ", Client ID=",
+            ", Client Secret=",
+            ", Endpoint To Get Code=",
+            ", Endpoint To Get Refresh Token=",
+            ", Scopes=",
             ["", "e", "Force Re-Authentication"],
-            ", Timeout:",
-            ", Username:",
-            ", Password:",
+            ", Timeout=",
+            ", Username=",
+            ", Password=",
+        ],
+    ),
+    "352t": ActionCode(
+        6,
+        "",
+        ["0", "1", "2", "3", "4", "5"],
+        [
+            "Bundle",
+            "Int",
+            "Str",
+            "Str",
+            "Str",
+            "Str",
+        ],
+        "Get Network Data Usage",
+        ["1", "2", "3", "4"],
+        [
+            ["Network Type=", "l", "352"],
+            ", From=",
+            ", To=",
+            ", Package=",
         ],
     ),
     "354t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Str", "Str", "ConditionList"],
         "Array Set",
         ["0", "1", "2"],
-        ["Variable Array:", ", Values:", ", Splitter:"],
+        ["Variable Array=", ", Values=", ", Splitter="],
     ),
     "355t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Str", "Int", "Str", "Int", "ConditionList"],
         "Array Push",
         ["0", "1", "2", "3"],
-        ["Variable Array:", ", Position:", ", Value:", ["", "e", ", Fill Spaces"]],
+        ["Variable Array=", ", Position=", ", Value=", ["", "e", ", Fill Spaces"]],
     ),
     "356t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Int", "Str", "ConditionList"],
         "Array Pop",
         ["0", "1", "2"],
-        ["Variable Array:", ", Position:", ", To Var:"],
+        ["Variable Array=", ", Position=", ", To Var="],
     ),
-    "357t": ActionCode(1, "", ["0"], ["Str"], "Array Clear", ["0"], ["Variable Array:"]),
+    "357t": ActionCode(1, "", ["0"], ["Str"], "Array Clear", ["0"], ["Variable Array="]),
     "358t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Bundle", "Int", "Str", "Int"],
         "Bluetooth Info",
         ["1", "2", "3"],
-        [["Type:", "l", "358"], ", Device:", ", Timeout:"],
+        [["Type=", "l", "358"], ", Device=", ", Timeout="],
     ),
     "35t": ActionCode(
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["Int", "Int", "Int", "Int", "Int", "ConditionList"],
         "Wait Until",
         ["0", "1", "2", "3", "4"],
-        [["if"], "MS:", ", Seconds:", ", Minutes:", ", Hours:", ", Days:"],
+        [["if"], "MS=", ", Seconds=", ", Minutes=", ", Hours=", ", Days="],
     ),
     "360t": ActionCode(
         8,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7"],
         ["Bundle", "Str", "Str", "Str", "Int", "Str", "Int", "Int"],
         "Input Dialog",
         ["1", "2", "3", "4", "5", "6", "7"],
         [
-            "Title:",
-            ", Text:",
-            ", Default Input:",
-            ", Close After (Seconds):",
-            ", Input Type:",
+            "Title=",
+            ", Text=",
+            ", Default Input=",
+            ", Close After (Seconds)=",
+            ", Input Type=",
             ["", "e", ", Use HTML"],
             ["", "e", ", Pre-Select Input"],
         ],
     ),
     "361t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "Bundle"],
         "Dark Mode",
         ["0"],
-        [["Set:", "l", "switch_set"]],
+        [["Set=", "l", "switch_set"]],
     ),
-    "362t": ActionCode(1, "", ["0"], ["Str"], "Set Assistant", ["0"], ["Assistant:"]),
+    "362t": ActionCode(1, "", ["0"], ["Str"], "Set Assistant", ["0"], ["Assistant="]),
     "363t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "Str"],
         "Mobile Network Type",
         ["0"],
-        [["Set:", "l", "switch_set"]],
+        [["Set=", "l", "switch_set"]],
     ),
     "364t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Bundle", "Int"],
         "Text Next Alarm",
         ["1"],
-        ["Minutes Difference:"],
+        ["Minutes Difference="],
     ),
     "365t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Bundle", "Str", "ConditionList"],
         "Tasker Function",
         ["1"],
-        ["Function:"],
+        ["Function="],
     ),
     "366t": ActionCode(
         10,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"],
         ["Bundle", "Int", "Str", "Str", "Str", "Str", "Int", "Int", "Str", "Int"],
         "Get Location V2",
         ["1", "2", "3", "4", "5", "6", "7", "8", "9"],
         [
-            "Timeout (Seconds):",
-            ", Minimum Accuracy (meters):",
-            ", Speed (meters/second):",
-            ", Altitude (meters):",
-            ", Near Location:",
+            "Timeout (Seconds)=",
+            ", Minimum Accuracy (meters)=",
+            ", Speed (meters/second)=",
+            ", Altitude (meters)=",
+            ", Near Location=",
             ["", "e", ", Enable Location If Needed"],
             ["", "e", ", Last Location If Timeout"],
-            ", Min Speed Accuracy (m/s):",
+            ", Min Speed Accuracy (m/s)=",
             ["", "e", ", Force High Accuracy"],
         ],
     ),
     "367t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "Bundle"],
         "Camera",
         ["0"],
-        [["Set:", "l", "switch_set"]],
+        [["Set=", "l", "switch_set"]],
     ),
     "368t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Bundle", "Str", "Int", "Str", "Int"],
         "Pick Location",
         ["1", "2", "3", "4"],
         [
-            "Title:",
+            "Title=",
             ["", "e", ", Select Radius"],
-            ", Initial Location:",
-            [", Set:", "l", "368"],
+            ", Initial Location=",
+            [", Set=", "l", "368"],
         ],
     ),
     "369t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Int", "ConditionList"],
         "Array Process",
         ["0", "1"],
-        ["Variable Array:", [", Type:", "l", "369"]],
+        ["Variable Array=", [", Type=", "l", "369"]],
     ),
-    "370t": ActionCode(2, "", ["0", "1"], ["Bundle", "Str"], "Shortcut", ["0"], ["Shortcut:"]),
+    "370t": ActionCode(2, "", ["0", "1"], ["Bundle", "Str"], "Shortcut", ["0"], ["Shortcut="]),
     "371t": ActionCode(0, "", [], [], "Astrid", [], []),
-    "372t": ActionCode(2, "", ["0", "1"], ["Bundle", "Str"], "Sensor Info", ["1"], ["Type:"]),
+    "372t": ActionCode(2, "", ["0", "1"], ["Bundle", "Str"], "Sensor Info", ["1"], ["Type="]),
     "373t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Bundle", "Str", "Int", "Int"],
         "Test Sensor",
         ["1", "2", "3"],
-        ["Type:", ", Timeout (Seconds):", ["", "e", ", Convert Orientation"]],
+        ["Type=", ", Timeout (Seconds)=", ["", "e", ", Convert Orientation"]],
     ),
     "374t": ActionCode(
         8,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7"],
         ["Bundle", "Int", "Str", "Int", "Str", "Str", "Str", "Str"],
         "Screen Capture",
         ["1", "2", "3", "4", "5", "6"],
         [
-            ["Type:", "l", "374"],
-            ", Output File:",
+            ["Type=", "l", "374"],
+            ", Output File=",
             ["", "e", ", Sound"],
-            ", Video Encoder:",
-            ", Resolution:",
-            ", Video Bitrate:",
+            ", Video Encoder=",
+            ", Resolution=",
+            ", Video Bitrate=",
         ],
     ),
     "375t": ActionCode(0, "", [], [], "ADB Wifi", [], []),
     "376t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Str", "Int", "Str"],
         "Share File",
         ["0", "1", "2", "3"],
         [
-            "File:",
-            ", Mime Type:",
+            "File=",
+            ", Mime Type=",
             ["", "e", ", Show Chooser Dialog"],
-            ", Chooser Dialog Title:",
+            ", Chooser Dialog Title=",
         ],
     ),
     "377t": ActionCode(
         11,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "10"],
         [
@@ -1823,23 +1848,23 @@
             "Str",
             "Str",
             "ConditionList",
         ],
         "Text/Image Dialog",
         ["1", "2", "3", "4", "5", "6", "7", "8", "9"],
         [
-            "Title:",
-            ", Text:",
-            ", Button 1:",
-            ", Button 2:",
-            ", Button 3:",
-            ", Close After (Seconds):",
+            "Title=",
+            ", Text=",
+            ", Button 1=",
+            ", Button 2=",
+            ", Button 3=",
+            ", Close After (Seconds)=",
             ["", "e", ", Use HTML"],
-            ", Image:",
-            ", Max Width or Height:",
+            ", Image=",
+            ", Max Width or Height=",
         ],
     ),
     "378t": ActionCode(
         15,
         "",
         [
             "0",
@@ -1874,65 +1899,87 @@
             "Int",
             "Str",
             "ConditionList",
         ],
         "List Dialog",
         ["1", "2", "3", "4", "6", "7", "8", "9", "10", "11", "12", "13"],
         [
-            ["Mode:", "l", "378"],
-            ", Title:",
-            ", Items:",
-            ", Long Click Task:",
-            ", Button 1:",
-            ", Button 2:",
-            ", Button 3:",
-            ", Close After (Seconds):",
+            ["Mode=", "l", "378"],
+            ", Title=",
+            ", Items=",
+            ", Long Click Task=",
+            ", Button 1=",
+            ", Button 2=",
+            ", Button 3=",
+            ", Close After (Seconds)=",
             ["", "e", ", Use HTML"],
-            ", First Visible Index:",
+            ", First Visible Index=",
             ["", "e", ", Hide Filter"],
-            ", Text:",
+            ", Text=",
+        ],
+    ),
+    "379t": ActionCode(
+        6,
+        "",
+        ["0", "1", "2", "3", "4", "5"],
+        [
+            "Bundle",
+            "Int",
+            "App",
+            "Str",
+            "Int",
+            "Str",
+        ],
+        "Device Admin/Owner",
+        ["1", "2", "3", "4", "5"],
+        [
+            ["Action=", "l", "379"],
+            ", App=",
+            ", Function=",
+            ["", "e", ", Enable"],
+            ", Restrictions=",
         ],
     ),
     "37s": ActionCode(1, "", ["0"], ["ConditionList"], "Variable Set", [], []),
     "37t": ActionCode(1, "", ["0"], ["ConditionList"], "If", ["if"], [""]),
     "380t": ActionCode(
         10,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"],
         ["Bundle", "Str", "Str", "Str", "Int", "Str", "Str", "Str", "Int", "Str"],
         "HTTP Response",
         ["1", "2", "3", "4", "5", "6", "7", "8"],
         [
-            "Request ID:",
-            ", Status Code:",
-            ", Headers:",
-            ["Type:", "l", "380"],
+            "Request ID=",
+            ", Status Code=",
+            ", Headers=",
+            ["Type=", "l", "380"],
             "",
-            ", File:",
-            ", Mime Type:",
+            ", File=",
+            ", Mime Type=",
             ["", "e", ", File Inline"],
         ],
     ),
     "381t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Bundle", "Str", "Str", "Str", "Int"],
         "Contact Via App",
         ["0", "1"],
-        ["Contact:", ", App:"],
+        ["Contact=", ", App="],
     ),
     "383t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "Int"],
         "Settings Panel",
         ["0"],
-        [["Contact:", "l", "383"]],
+        [["Contact=", "l", "383"]],
     ),
     "384t": ActionCode(
         15,
         "",
         [
             "0",
             "1",
@@ -1966,52 +2013,52 @@
             "Str",
             "Str",
             "Int",
         ],
         "Device Control (Power Menu Action)",
         ["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11", "12", "13", "14"],
         [
-            "ID:",
-            [", Action:", "l", "384"],
-            [", Type:", "l", "384a"],
-            ", Title:",
-            ", Subtitle:",
-            ", Icon:",
-            ", Command:",
-            ", Active:",
-            ", Range Min:",
-            ", Range Max:",
-            ", Range Current:",
-            "Range Step:",
-            ", Range Format:",
+            "ID=",
+            [", Action=", "l", "384"],
+            [", Type=", "l", "384a"],
+            ", Title=",
+            ", Subtitle=",
+            ", Icon=",
+            ", Command=",
+            ", Active=",
+            ", Range Min=",
+            ", Range Max=",
+            ", Range Current=",
+            "Range Step=",
+            ", Range Format=",
             ["", "e", ", Can Use On Locked Device"],
         ],
     ),
-    "385t": ActionCode(1, "", ["0"], ["Str"], "Command", ["0"], ["Command:"]),
+    "385t": ActionCode(1, "", ["0"], ["Str"], "Command", ["0"], ["Command="]),
     "386t": ActionCode(
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["Bundle", "Int", "Int", "Int", "Int", "Int"],
         "Call Screening",
         ["0", "1", "2"],
         [
-            ["ID:", "l", "386"],
+            ["ID=", "l", "386"],
             ["", "e", ", Skip Call Log"],
             ["", "e", ", Skip Notification"],
         ],
     ),
     "387t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Int", "Int"],
         "Accessibility Volume",
         ["0", "1", "2"],
-        ["Level:", ["", "e", ", Display"], ["", "e", ", Sound"]],
+        ["Level=", ["", "e", ", Display"], ["", "e", ", Sound"]],
     ),
     "388543774t": ActionCode(0, "1040876951t", [], [], "AutoSheets Insert Empty Rows/Columns", [], []),
     "389t": ActionCode(
         10,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"],
         [
@@ -2025,37 +2072,37 @@
             "Int",
             "Int",
             "ConditionList",
         ],
         "Multiple Variables Set",
         ["1", "2", "3", "4", "5", "6", "7"],
         [
-            "Names:",
-            ", Variable Name Splitter:",
-            ", Values:",
-            ", Values Splitter:",
+            "Names=",
+            ", Variable Name Splitter=",
+            ", Values=",
+            ", Values Splitter=",
             ["", "e", ", Do Maths"],
             ["", "e", ", Keep Existing"],
             ["", "e", ", Structure Output (JSON, etc)"],
         ],
     ),
     "38t": ActionCode(0, "", [], [], "End If", [], []),
     "390t": ActionCode(
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["Bundle", "Str", "Str", "Str", "Str", "Int"],
         "Pick Input Dialog",
         ["1", "2", "3", "4", "5"],
         [
-            "Type:",
-            ", Title:",
-            ", Text:",
-            ", Default Input:",
-            ", Close After (Seconds):",
+            "Type=",
+            ", Title=",
+            ", Text=",
+            ", Default Input=",
+            ", Close After (Seconds)=",
         ],
     ),
     "391t": ActionCode(
         12,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11"],
         [
@@ -2071,48 +2118,48 @@
             "Int",
             "Int",
             "ConditionList",
         ],
         "Progress Dialog",
         ["1", "2", "3", "4", "5", "6", "7", "8", "9"],
         [
-            ["Action:", "l", "391"],
-            ", Title:",
-            ", Text:",
-            [", Type:", "l", "391a"],
-            ", Animation Images:",
-            ", Animation Tint:",
-            ", Frame Duration:",
-            ", Progress:",
-            ", Max:",
+            ["Action=", "l", "391"],
+            ", Title=",
+            ", Text=",
+            [", Type=", "l", "391a"],
+            ", Animation Images=",
+            ", Animation Tint=",
+            ", Frame Duration=",
+            ", Progress=",
+            ", Max=",
         ],
     ),
     "392t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Bundle", "Str", "Str"],
         "Set Variable Structure",
         ["1", "2"],
-        ["Name:", ", Structure Type:"],
+        ["Name=", ", Structure Type="],
     ),
     "393t": ActionCode(
         7,
         "",
         ["0", "1", "2", "3", "4", "5", "6"],
         ["Bundle", "Str", "Int", "Str", "Str", "Str", "Str"],
         "Array Merge",
         ["1", "2", "3", "4", "5", "6"],
         [
-            "Names:",
-            [", Title:", "l", "393"],
-            ", Joiner:",
-            ", Format:",
-            ", Output:",
-            ", Join Output:",
+            "Names=",
+            [", Title=", "l", "393"],
+            ", Joiner=",
+            ", Format=",
+            ", Output=",
+            ", Join Output=",
         ],
     ),
     "394t": ActionCode(
         13,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11", "12"],
         [
@@ -2124,203 +2171,205 @@
             "Str",
             "Str",
             "Str",
             "Int",
             "Int",
             "Int",
             "Str",
-            "ConditionList",
+            "Str",
         ],
         "Parse/Format DateTime",
-        ["1", "2", "3", "4", "5", "7", "8", "9", "10", "11"],
+        ["1", "2", "3", "4", "5", "7", "8", "9", "10", "11", "12"],
         [
-            ["Input Type:", "l", "394"],
-            ", Input:",
-            ", Input Format:",
-            ", Input Separator:",
-            ", Output Format:",
-            ", Formatted Value Names:",
+            ["Input Type=", "l", "394"],
+            ", Input=",
+            ", Input Format=",
+            ", Input Separator=",
+            ", Output Format=",
+            ", Formatted Value Names=",
             ["", "e", ", Get All Details"],
             ["", "e", ", Do Maths"],
-            [", Output Offset Type:", "l", "394a"],
-            ", Output Offset:",
+            [", Output Offset Type=", "l", "394a"],
+            ", Output Offset=",
+            ", Time Zone=",
         ],
     ),
     "395t": ActionCode(0, "", [], [], "JD Status", [], []),
     "396t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Bundle", "Int", "Str", "Str", "Str"],
         "Simple Match/Regex",
         ["1", "2", "3"],
-        [["Type:", "l", "396"], ", Text:", ", Match Pattern/Regex:"],
+        [["Type=", "l", "396"], ", Text=", ", Match Pattern/Regex="],
     ),
     "397t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Bundle", "Int"],
         "Get Material You Colors",
         ["1"],
         [["", "e", "Output Hashtags"]],
     ),
-    "398t": ActionCode(1, "", ["0"], ["Str"], "Connect To WiFi", ["0"], ["SSID:"]),
+    "398t": ActionCode(1, "", ["0"], ["Str"], "Connect To WiFi", ["0"], ["SSID="]),
     "399t": ActionCode(
         10,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"],
         ["Bundle", "Str", "Str", "Str", "Str", "Str", "Int", "Int", "Int", "Str"],
         "Variable Map",
         ["1", "2", "3", "4", "5", "7", "8", "9"],
         [
-            "Input:",
-            ", Input Minimum:",
-            ", Input Maximum:",
-            ", Output Minimum:",
-            ", Output Maximum:",
+            "Input=",
+            ", Input Minimum=",
+            ", Input Maximum=",
+            ", Output Minimum=",
+            ", Output Maximum=",
             ["", "e", ", Invert"],
             ["", "e", ", Restrict Range"],
-            ", Max Rounding Digits:",
-            ", Output Variable Name:",
+            ", Max Rounding Digits=",
+            ", Output Variable Name=",
         ],
     ),
     "39t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Str", "Int", "ConditionList"],
         "For",
         ["0", "1", "2"],
         [
-            "Variable:",
-            ", Items:",
+            "Variable=",
+            ", Items=",
             ["", "e", ", Structure Output (JSON, etc)"],
             ["if"],
             [""],
         ],
     ),
     "3s": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Str"],
         "BT Connected",
         ["0", "1"],
-        ["Name:", ", Address:"],
+        ["Name=", ", Address="],
     ),
     "400t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Str", "Int", "Int"],
         "Move",
         ["0", "1", "2"],
-        ["From:", ", To:", ["", "e", ", Use Root"]],
+        ["From=", ", To=", ["", "e", ", Use Root"]],
     ),
     "402t": ActionCode(0, "", ["0"], ["Bundle"], "Get Clipboard", [], []),
     "404t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Str", "Int", "Int"],
         "Copy File",
         ["0", "1", "2"],
-        ["From:", ", To:", ["", "e", ", Use Root"]],
+        ["From=", ", To=", ["", "e", ", Use Root"]],
     ),
     "405t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Str", "Int", "Int"],
         "Copy Dir",
         ["0", "1", "2"],
-        ["From:", ", To:", ["", "e", ", Use Root"]],
+        ["From=", ", To=", ["", "e", ", Use Root"]],
     ),
     "406t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Str", "Int", "Int", "Int", "ConditionList"],
         "Delete File",
         ["0", "1"],
-        ["File:", ["", "e", ", Use Root"]],
+        ["File=", ["", "e", ", Use Root"]],
     ),
     "407t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Bundle", "Str", "Str", "Int"],
         "Pick Photos",
         ["1", "2", "3"],
-        [",Max Number:", ", Mime Type:", ["", "e", ", Copy To Cache"]],
+        [",Max Number=", ", Mime Type=", ["", "e", ", Copy To Cache"]],
     ),
     "40830242s": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Bundle", "Str", "Str", "Int"],
         "AutoNotification Intercept",
         ["0", "3"],
-        ["Configuration:", ["", "e", ", Structure Output (JSON (etc)"]],
+        ["Configuration=", ["", "e", ", Structure Output (JSON (etc)"]],
     ),
     "408t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Int", "Int", "Int"],
         "Delete Directory",
         ["0", "1", "2"],
-        ["Directory:", ["", "e", ", Recurse"], ["", "e", ", Use Root"]],
+        ["Directory=", ["", "e", ", Recurse"], ["", "e", ", Use Root"]],
     ),
     "409t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Str", "Int", "Int", "Int", "ConditionList"],
         "Create Directory",
         ["0", "1", "2"],
-        ["Directory:", ["", "e", ", Create All"], ["", "e", ", Use Root"]],
+        ["Directory=", ["", "e", ", Create All"], ["", "e", ", Use Root"]],
     ),
-    "40s": ActionCode(0, "", 0, [], "Call", ["0", "1"], ["Type:", ", Number:"]),
+    "40966172t": ActionCode(0, "1040876951t", [], [], "AutoCast", [], []),
+    "40s": ActionCode(0, "", 0, [], "Call", ["0", "1"], ["Type=", ", Number="]),
     "40t": ActionCode(0, "", [], [], "End For", [], []),
     "410t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Str", "Str", "Int", "Int", "ConditionList"],
         "Write File",
         ["0", "1", "2", "3"],
-        ["File:", ", Text:", ["", "e", ", Append"], ["", "e", ", Add New Line"]],
+        ["File=", ", Text=", ["", "e", ", Append"], ["", "e", ", Add New Line"]],
     ),
     "411e": ActionCode(0, "", [], [], "Device Boot", [], []),
     "412t": ActionCode(
         7,
         "",
         ["0", "1", "2", "3", "4", "5", "6"],
         ["Str", "Str", "Int", "Int", "Int", "Str", "Int"],
         "List Files",
         ["0", "1", "2", "3", "4", "5"],
         [
-            "Directory:",
-            ", Match:",
+            "Directory=",
+            ", Match=",
             ["", "e", ", Include Hidden Files"],
             ["", "e", ", Use Root"],
-            [", Sort Selection:", "l", "412"],
-            ", Variable Array:",
+            [", Sort Selection=", "l", "412"],
+            ", Variable Array=",
         ],
     ),
     "413t": ActionCode(
         3,
         "",
         ["1", "2", "3"],
         ["Str", "Str", "Str"],
         "Request Add Tile",
         ["1", "2", "3"],
-        ["Tile To Add:", "Title:", "Icon:"],
+        ["Tile To Add=", "Title=", "Icon="],
     ),
     "413e": ActionCode(0, "", [], [], "Device Shutdown", [], []),
     "414549629t": ActionCode(0, "1040876951t", [], [], "AutoSpotify Search", [], []),
     "415t": ActionCode(0, "", [], [], "Read Line", [], []),
     "41628340e": ActionCode(
         4,
         "",
@@ -2333,84 +2382,84 @@
     "416t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Str", "Str"],
         "Read Paragraph",
         ["0", "1", "2"],
-        ["File:", ", Para:", ", To Var:"],
+        ["File=", ", Para=", ", To Var="],
     ),
     "417t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Str", "Int"],
         "Read File",
         ["0", "1", "2"],
-        ["File:", ", To Var:", ["", "e", ", Structure Output (JSON, etc)"]],
+        ["File=", ", To Var=", ["", "e", ", Structure Output (JSON, etc)"]],
     ),
     "41t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Str", "Str", "Int", "Str", "Int"],
         "Send SMS",
         ["0", "1", "3", "4"],
-        ["Number:", ", Message:", ", SIM Card:", ["", "e", ", Wait For Result"]],
+        ["Number=", ", Message=", ", SIM Card=", ["", "e", ", Wait For Result"]],
     ),
     "420t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Int", "Int", "Str"],
         "Zip",
         ["0", "1", "2", "3"],
-        ["File:", ["", "e", ", Delete Dialog"], ", Level:", ", Output File:"],
+        ["File=", ["", "e", ", Delete Dialog"], ", Level=", ", Output File="],
     ),
     "421t": ActionCode(0, "", ["0"], ["Bundle"], "Get Screen Info", [], []),
     "422e": ActionCode(0, "", [], [], "Device Storage Low", [], []),
     "422t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Int"],
         "UnZip",
         ["0", "1"],
-        ["File:", ["", "e", ", Delete Zip"]],
+        ["File=", ["", "e", ", Delete Zip"]],
     ),
     "424e": ActionCode(0, "", [], [], "Screebl / TSC", [], []),
     "424t": ActionCode(0, "", ["0"], ["Bundle"], "Get Battery Info", [], []),
     "424867932t": ActionCode(0, "1040876951t", [], [], "AutoBubbles Manage Bubble", [], []),
     "425e": ActionCode(0, "", [], [], "K9 Email Received", [], []),
-    "425t": ActionCode(1, "", ["0"], ["Int"], "Wifi", ["0"], [["Set:", "l", "switch_set"]]),
+    "425t": ActionCode(1, "", ["0"], ["Int"], "Wifi", ["0"], [["Set=", "l", "switch_set"]]),
     "426e": ActionCode(0, "", [], [], "Widget Locker", [], []),
     "426t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Int", "Int"],
         "Wifi Net",
         ["0", "1", "2"],
-        [["Action:", "l", "426"], ["", "e", ", Force"], ["", "e", ", Report Failure"]],
+        [["Action=", "l", "426"], ["", "e", ", Force"], ["", "e", ", Report Failure"]],
     ),
     "427e": ActionCode(0, "", [], [], "OpenWatch", [], []),
-    "427t": ActionCode(1, "", ["0"], ["Int"], "Wifi Sleep", ["0"], [["Policy:", "l", "427"]]),
+    "427t": ActionCode(1, "", ["0"], ["Int"], "Wifi Sleep", ["0"], [["Policy=", "l", "427"]]),
     "427019141t": ActionCode(0, "1040876951t", [], [], "AutoNotification Replace Gmail Notifications", [], []),
     "428e": ActionCode(0, "", [], [], "Kaloer Clock", [], []),
     "42924197t": ActionCode(0, "1040876951t", [], [], "Notification Listener", [], []),
     "429032033t": ActionCode(0, "1040876951t", [], [], "AutoContacts Details", [], []),
     "429e": ActionCode(0, "", [], [], "Locale Changed", [], []),
     "42t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Int", "Str"],
         "Send Data SMS",
         ["0", "1", "2"],
-        ["Number:", ", Port:", ", Data:", ["if", ""]],
+        ["Number=", ", Port=", ", Data=", ["if", ""]],
     ),
     "430t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Bundle", "Int", "ConditionList"],
         "Restart Tasker",
@@ -2420,208 +2469,218 @@
     "431t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Bundle", "Int", "Str", "Str", "ConditionList"],
         "Accessibility Services",
         ["1", "2"],
-        [["Action:", "l", "431"], ", Services"],
+        [["Action=", "l", "431"], ", Services"],
     ),
     "433t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "Bundle"],
         "Mobile Data",
         ["0"],
-        [["Set:", "l", "switch_set"]],
+        [["Set=", "l", "switch_set"]],
     ),
     "438t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Bundle", "Str", "Str", "Str", "Str"],
         "Matter Light",
         ["1", "2", "3", "4"],
-        ["Device IDs/Name:", ", Set:", ", Color:", ", Brightness:"],
+        ["Device IDs/Name=", ", Set=", ", Color=", ", Brightness="],
     ),
     "439t": ActionCode(0, "", [], [], "WiMax", [], []),
     "43t": ActionCode(1, "", ["0"], ["ConditionList"], "Else/Else If", ["if"], [""]),
     "432t": ActionCode(0, "", [], [], "Get Network Info", [], []),
     "440t": ActionCode(0, "", [], [], "Set Timezone", [], []),
     "441t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "Bundle"],
         "Work Profile",
         ["0"],
-        [["Set:", "l", "switch_set"]],
+        [["Set=", "l", "switch_set"]],
     ),
     "442t": ActionCode(0, "", [], [], "SleepBot", [], []),
     "443t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Int", "Int", "App", "Int"],
         "Media Control",
         ["0", "1", "2", "3"],
         [
-            ["Cmd:", "l", "443"],
+            ["Cmd=", "l", "443"],
             ["", "e", ", Simulate Media Button"],
-            ", Package/App Name:",
+            ", Package/App Name=",
             ["", "e", ", Use Notification If Available"],
         ],
     ),
     "444e": ActionCode(0, "", [], [], "Pomodroido", [], []),
     "444t": ActionCode(0, "", [], [], "TeslaLED", [], []),
     "445e": ActionCode(0, "", [], [], "Radardroid", [], []),
     "445t": ActionCode(
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["Str", "Int", "Int", "Int", "Int", "ConditionList"],
         "Music Play",
         ["0", "1", "2", "3", "4"],
         [
-            "File:",
-            ", Start:",
+            "File=",
+            ", Start=",
             ["", "e", ", Loop"],
-            ["Cmd:", "l", "171"],
+            ["Cmd=", "l", "171"],
             ["", "e", ", Continue Task Immediately"],
         ],
     ),
     "446e": ActionCode(0, "", [], [], "Gentle Alarm", [], []),
+    "446t": ActionCode(
+        6,
+        "",
+        ["0", "1", "2", "3", "4", "5"],
+        ["Bundle", "Str", "Str", "Str", "Str", "Int"],
+        "Get File/Folder Properties",
+        ["1", "2", "3", "4", "5"],
+        ["Path=", ", Type=", ", Name/Path Filter=", ", Other Filters=", ["", "e", ", Recurse"]],
+    ),
     "447e": ActionCode(0, "", [], [], "Reddit Notify", [], []),
     "447t": ActionCode(
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["Str", "Int", "Int", "Int", "Int", "Int"],
         "Music Play Dir",
         ["0", "1", "2", "3", "4", "5"],
         [
-            "Directory:",
+            "Directory=",
             ["", "e", ", Subdirs"],
             ["", "e", ", Audio Only"],
             ["", "e", ", Random"],
             ["", "e", ", Flash"],
-            ", Maximum Tracks:",
+            ", Maximum Tracks=",
         ],
     ),
     "448e": ActionCode(0, "", [], [], "Notify My Android", [], []),
+    "448t": ActionCode(2, "", ["0", "1"], ["Bundle", "Str"], "Array Compare", ["1"], ["Names="]),
     "449t": ActionCode(1, "", ["0"], ["Int"], "Music Stop", ["0"], [["", "e", ", Clear Dir"]]),
     "450e": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Str"],
         "New Package",
         ["0", "1"],
-        ["Name:", ", Package:"],
+        [",Name=", ", Package="],
     ),
     "450t": ActionCode(0, "", [], [], "APN Droid", [], []),
-    "451e": ActionCode(1, "", ["0"], ["Str"], "Package Removed", ["0"], ["Package:"]),
-    "451t": ActionCode(1, "", ["0"], ["Int"], "Music Skip", ["0"], ["Jump:"]),
+    "451e": ActionCode(1, "", ["0"], ["Str"], "Package Removed", ["0"], ["Package="]),
+    "451t": ActionCode(1, "", ["0"], ["Int"], "Music Skip", ["0"], ["Jump="]),
     "453e": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Str"],
         "Package Updated",
         ["0", "1"],
-        ["Name:", ", Package:"],
+        ["Name=", ", Package="],
     ),
-    "453t": ActionCode(1, "", ["0"], ["Int"], "Music Back", ["0"], ["Jump:"]),
+    "453t": ActionCode(1, "", ["0"], ["Int"], "Music Back", ["0"], ["Jump="]),
     "455t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Str", "Int", "Int", "Int", "Int"],
         "Record Audio",
         ["0", "1", "2", "3"],
-        ["File:", [", Source:", "l", "455"], ", MaxSize:", [", Format:", "l", "455a"]],
+        ["File=", [", Source=", "l", "455"], ", MaxSize=", [", Format=", "l", "455a"]],
     ),
     "456t": ActionCode(0, "", [], [], "JD APN", [], []),
     "457t": ActionCode(0, "", [], [], "Default Ringtone", [], []),
     "458t": ActionCode(0, "", [], [], "WidgetLocker", [], []),
-    "459t": ActionCode(1, "", ["0"], ["Str"], "Scan Media", ["0"], ["File:"]),
+    "459t": ActionCode(1, "", ["0"], ["Str"], "Scan Media", ["0"], ["File="]),
     "460e": ActionCode(0, "", [], [], "Wallpaper Changed", [], []),
     "461e": ActionCode(
         8,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7"],
         ["App", "Str", "Str", "Str", "Str", "Str", "Str", "Int"],
         "Notification",
         ["0", "1", "2", "3", "4", "5", "6", "7"],
         [
-            "Owner Application:",
-            ", Title:",
-            ", Text:",
-            ", Subtext:",
-            ", Messages:",
-            ", Other Text:",
-            ", Cat:",
+            "Owner Application=",
+            ", Title=",
+            ", Text=",
+            ", Subtext=",
+            ", Messages=",
+            ", Other Text=",
+            ", Cat=",
             ["", "e", ", New Only"],
         ],
     ),
     "461t": ActionCode(
         0,
         "",
         [],
         [],
         "Scan Media",
         ["0", "1", "2", "3", "4", "5", "6", "7"],
         [
-            "Owner Application:",
-            ", Title:",
-            ", Text:",
-            ", Subtext:",
-            ", Messages:",
-            ", Other Text:",
-            ", Cat:",
+            "Owner Application=",
+            ", Title=",
+            ", Text=",
+            ", Subtext=",
+            ", Messages=",
+            ", Other Text=",
+            ", Cat=",
             ["", "e", ", New Only"],
         ],
     ),
     "462e": ActionCode(0, "", [], [], "Button Widget Clicked", [], []),
     "463e": ActionCode(0, "", [], [], "New Window", [], []),
     "464e": ActionCode(
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["App", "Str", "Str", "Str", "Str", "Str"],
         "Notification Removal",
         ["0", "1", "2", "3", "4", "5"],
         [
-            "Owner Application:",
-            ", Title:",
-            ", Text:",
-            ", Subtext:",
-            ", Messages:",
-            ", Other Text:",
+            "Owner Application=",
+            ", Title=",
+            ", Text=",
+            ", Subtext=",
+            ", Messages=",
+            ", Other Text=",
         ],
     ),
-    "46t": ActionCode(1, "", ["0"], ["Str"], "Create Scene", ["0"], ["Name:"]),
+    "46t": ActionCode(1, "", ["0"], ["Str"], "Create Scene", ["0"], ["Name="]),
     "475t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Int"],
         "GZip",
         ["0", "1"],
-        ["File:", ["", "e", ", Delete Orig"]],
+        ["File=", ["", "e", ", Delete Orig"]],
     ),
     "476t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Int"],
         "GUnzip",
         ["0", "1"],
-        ["File:", ["", "e", ", Delete Zip"]],
+        ["File=", ["", "e", ", Delete Zip"]],
     ),
     "47t": ActionCode(
         12,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11"],
         [
             "Str",
@@ -2636,88 +2695,88 @@
             "Int",
             "Int",
             "ConditionList",
         ],
         "Show Scene",
         ["0", "1", "6", "7", "8", "9", "if"],
         [
-            "Name:",
-            ["Display As:", "l", "47"],
-            ["", "e", "Show Exit Button"],
-            ["", "e", "Continue Task Immediately"],
-            ["", "e", "Allow Outside Boundaries"],
-            ["", "e", "Blocking Overlay +"],
+            "Name=",
+            [", Display As=", "l", "47"],
+            ["", "e", ", Show Exit Button"],
+            ["", "e", ", Continue Task Immediately"],
+            ["", "e", ", Allow Outside Boundaries"],
+            ["", "e", ", Blocking Overlay +"],
             [""],
         ],
     ),
     "48t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Int", "ConditionList"],
         "Hide Scene",
         ["0", "1"],
-        ["Name:", ["Animation:", "l", "48"]],
+        ["Name=", ["Animation=", "l", "48"]],
     ),
     "490t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "Int"],
         "Media Button Events",
         ["0", "1"],
-        [["File:", "l", "490"], ["", "e", ", Use New API"]],
+        [["File=", "l", "490"], ["", "e", ", Use New API"]],
     ),
-    "49t": ActionCode(2, "", ["0", "1"], ["Str", "ConditionList"], "Destroy Scene", ["0"], ["Name:"]),
+    "49t": ActionCode(2, "", ["0", "1"], ["Str", "ConditionList"], "Destroy Scene", ["0"], ["Name="]),
     "4e": ActionCode(0, "", [], [], "Phone Idle", [], []),
     "502102143t": ActionCode(0, "1040876951t", [], [], "AutoSheets Get Spreadsheet", [], []),
-    "4s": ActionCode(0, "", [], [], "Phone Idle", ["0"], [["Priority:", "l", "4s"]]),
+    "4s": ActionCode(0, "", [], [], "Phone Idle", ["0"], [["Priority=", "l", "4s"]]),
     "502807688t": ActionCode(0, "1040876951t", [], [], "AutoAppsHub SendCommand", [], []),
     "50s": ActionCode(0, "", [], [], "Keyboard Out", [], []),
     "50t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Str", "Int", "ConditionList"],
         "Element Value",
         ["0", "1", "2"],
-        ["Scene Name:", ", Element:", ", Value:"],
+        ["Scene Name=", ", Element=", ", Value="],
     ),
     "511t": ActionCode(
-        1,
+        2,
         "",
         ["0", "1"],
         ["Int", "Str"],
         "Torch",
         ["0"],
-        [["File:", "l", "switch_set"]],
+        [[", File=", "l", "switch_set"]],
     ),
     "512t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "ConditionList"],
         "Status Bar",
         ["0"],
-        [["File:", "l", "512"]],
+        [[", File=", "l", "512"]],
     ),
     "513t": ActionCode(0, "", [], [], "Close System Dialogs", [], []),
     "51t": ActionCode(
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["Str", "Str", "Int", "Str", "Str", "ConditionList"],
         "Element Text",
         ["0", "1", "2", "3", "4"],
         [
-            "Scene Name:",
-            ", Element:",
-            [", Position:", "l", "51"],
-            ", Text:",
-            ", Selection:",
+            "Scene Name=",
+            ", Element=",
+            [", Position=", "l", "51"],
+            ", Text=",
+            ", Selection=",
         ],
     ),
     "523t": ActionCode(
         13,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11", "12"],
         [
@@ -2734,123 +2793,123 @@
             "Str",
             "Str",
             "ConditionList",
         ],
         "Notify",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11"],
         [
-            "Title:",
-            ", Text:",
-            ", Icon:",
+            "Title=",
+            ", Text=",
+            ", Icon=",
             "",
             ["", "e", ", Permanent"],
-            ", Priority:",
+            ", Priority=",
             ["", "e", ", Repeat Alert"],
-            [", LED Color:", "l", "523"],
-            ", LED Rate:",
-            ", Sound File:",
-            ", Vibration Pattern:",
-            ", Cat:",
-            "Actions:",
+            [", LED Color=", "l", "523"],
+            ", LED Rate=",
+            ", Sound File=",
+            ", Vibration Pattern=",
+            ", Cat=",
+            "Actions=",
         ],
     ),
     "525t": ActionCode(
         8,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7"],
         ["Str", "Str", "Img", "Int", "Int", "Int", "Int", "Int"],
         "Notify LED",
         ["0", "1", "2", "3", "4", "5", "6", "7"],
         [
-            ":Title:",
-            ", Text:",
-            ", Icon:",
+            ":Title=",
+            ", Text=",
+            ", Icon=",
             "",
-            [", LED Color:", "l", "523"],
-            ", Rate:",
-            ", Priority:",
+            [", LED Color=", "l", "523"],
+            ", Rate=",
+            ", Priority=",
             ["", "e", ", Repeat Alert"],
         ],
     ),
     "536t": ActionCode(
         7,
         "",
         ["0", "1", "2", "3", "4", "5", "6"],
         ["Str", "Str", "Img", "Int", "Str", "Int", "Int"],
         "Notify Vibrate",
         ["0", "1", "2", "4", "5", "6"],
         [
-            "Title:",
-            ", Text:",
-            ", Icon:",
-            ", Pattern:",
-            ", Priority:",
+            "Title=",
+            ", Text=",
+            ", Icon=",
+            ", Pattern=",
+            ", Priority=",
             ["", "e", ", Repeat Alert"],
         ],
     ),
     "538t": ActionCode(
         7,
         "",
         ["0", "1", "2", "3", "4", "5", "6"],
         ["Str", "Str", "Img", "Int", "Str", "Int", "Int"],
         "Notification Sound",
         ["0", "1", "2", "4", "5"],
         [
-            "Title:",
-            ", Text:",
-            ", Icon:",
-            ", Sound File:",
-            ", Priority:",
+            "Title=",
+            ", Text=",
+            ", Icon=",
+            ", Sound File=",
+            ", Priority=",
             ["", "e", ", Repeat Alert"],
         ],
     ),
     "53t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Str", "Int", "Str"],
         "Element Web Control",
         ["0", "1", "2"],
-        ["Scene Name:", ", Element:", [", Mode:", "l", "53"]],
+        ["Scene Name=", ", Element=", [", Mode=", "l", "53"]],
     ),
     "543t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Str", "Int"],
         "Start System Timer",
         ["0", "1", "2"],
-        ["Seconds:", ", Message:", ["", "e", ", Show UI"]],
+        ["Seconds=", ", Message=", ["", "e", ", Show UI"]],
     ),
     "544t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Int"],
         "Timer Widget Control",
         ["0", "1"],
-        ["Name:", [", Type:", "l", "544"]],
+        ["Name=", [", Type=", "l", "544"]],
     ),
     "545t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Int", "Int"],
         "Variable Randomize",
         ["0", "1", "2"],
-        ["Name:", ", Min:", ", Max:"],
+        ["Name=", ", Min=", ", Max="],
     ),
     "546t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Str", "Int", "Int", "Int", "Int"],
         "Timer Widget Set",
         ["0", "1", "2", "3", "4"],
-        ["Name:", ", Seconds:", ", Minutes:", ", Hours:", ", Days:"],
+        ["Name=", ", Seconds=", ", Minutes=", ", Hours=", ", Days="],
     ),
     "547e": ActionCode(
         8,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7"],
         ["Str", "Str", "Int", "Int", "Int", "Int", "Int", "ConditionList"],
         "unmapped",
@@ -2861,20 +2920,20 @@
         8,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7"],
         ["Str", "Str", "Int", "Int", "Int", "Int", "Int", "ConditionList"],
         "Variable Set",
         ["0", "1", "2", "4", "5", "6"],
         [
-            "Name:",
-            ", To:",
+            "Name=",
+            ", To=",
             ["", "e", ", Recursive Variables"],
             ["", "e", ", Do Maths"],
             ["", "e", ", Append"],
-            ", Max Rounding Digits:",
+            ", Max Rounding Digits=",
             ["", "e", ", Structure Output (JSON, etc)"],
         ],
     ),
     "548t": ActionCode(
         16,
         "",
         [
@@ -2928,82 +2987,82 @@
             "10",
             "11",
             "12",
             "13",
             "14",
         ],
         [
-            "Text:",
+            "Text=",
             ["", "e", ", Long"],
             ["", "e", ", Tasker Layout"],
-            ", Title:",
-            ", Icon:",
-            " Icon Size:",
-            ", Background Color:",
-            ", Task:",
-            ", Timeout:",
+            ", Title=",
+            ", Icon=",
+            " Icon Size=",
+            ", Background Color=",
+            ", Task=",
+            ", Timeout=",
             ["", "e", ", Continue Task Immediately"],
-            ", Text Color:",
+            ", Text Color=",
             ["", "e", ", Dismiss On Click"],
             ["", "e", ", Show Over Everything"],
-            ", Position:",
+            ", Position=",
             ["", "e", ", Use HTML"],
         ],
     ),
     "549t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Str", "Int", "Int", "Int", "ConditionList"],
         "Variable Clear",
         ["0", "1", "2"],
-        ["Name:", ["", "e", ", Pattern Matching"], ["", "e", ", Clear All Variables"]],
+        ["Name=", ["", "e", ", Pattern Matching"], ["", "e", ", Clear All Variables"]],
     ),
     "54t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Str", "Str"],
         "Element Text Color",
         ["0", "1", "2"],
-        ["Scene Name:", ", Element:", " Colour:"],
+        ["Scene Name=", ", Element=", " Colour="],
     ),
     "550t": ActionCode(
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["Str", "Str", "Str", "Str", "Int", "Int"],
         "Popup",
         ["0", "1", "2", "4", "5"],
         [
-            "Title:",
-            ", Text:",
-            ", Background Image:",
-            ", Layout:",
-            ", Timeout (Seconds):",
+            "Title=",
+            ", Text=",
+            ", Background Image=",
+            ", Layout=",
+            ", Timeout (Seconds)=",
             ["", "e", ", Show Over Keyguard"],
         ],
     ),
     "551t": ActionCode(0, "", [], [], "Menu", [], []),
     "552t": ActionCode(
         9,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8"],
         ["Str", "Int", "Str", "Str", "Str", "Str", "Str", "Int", "Int"],
         "Popup Task Buttons",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8"],
         [
-            "Text:",
-            [", Mode:", "l", "552"],
-            ", Task:",
-            ", Task:",
-            ", Task:",
-            ", Background Image:",
-            ", Layout:",
-            ", Timeout (Seconds):",
+            "Text=",
+            [", Mode=", "l", "552"],
+            ", Task=",
+            ", Task=",
+            ", Task=",
+            ", Background Image=",
+            ", Layout=",
+            ", Timeout (Seconds)=",
             ["", "e", ", Show Over Keyguard"],
         ],
     ),
     "553t": ActionCode(0, "", [], [], "SMS Backup+", [], []),
     "555t": ActionCode(0, "", [], [], "BeyondPod", [], []),
     "556t": ActionCode(0, "", [], [], "GrazeRSS", [], []),
     "557649458t": ActionCode(0, "1040876951t", [], [], "AutoWear Time", [], []),
@@ -3012,64 +3071,64 @@
         9,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8"],
         ["Str", "Str", "Int", "Int", "Int", "Int", "Int", "Int", "ConditionList"],
         "Say",
         ["0", "1", "2", "3", "4", "5", "6", "7"],
         [
-            "Text:",
-            ", Engine Voice:",
-            [", Stream:", "l", "171"],
-            ", Pitch:",
-            ", Speed:",
+            "Text=",
+            ", Engine Voice=",
+            [", Stream=", "l", "171"],
+            ", Pitch=",
+            ", Speed=",
             ["", "e", ", Respect Audio Focus"],
             ["", "e", ", Network"],
             ["", "e", ", Continue Task Immediately"],
         ],
     ),
     "55t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Str", "Str", "Str", "Str", "ConditionList"],
         "Element Back Color",
         ["0", "1", "2", "3"],
-        ["Scene Name:", ", Element:", " Colour:", " End Colour:"],
+        ["Scene Name=", ", Element=", " Colour=", " End Colour="],
     ),
     "563213414t": ActionCode(0, "1040876951t", [], [], "AutoNotification Table", [], []),
     "565385068t": ActionCode(0, "1040876951t", [], [], "AutoNotification Query", [], []),
     "566t": ActionCode(
         7,
         "",
         ["0", "1", "2", "3", "4", "5", "6"],
         ["Int", "Int", "Str", "Str", "Int", "Int", "ConditionList"],
         "Set Alarm",
         ["0", "1", "2", "3", "4", "5"],
         [
-            "Hours:",
-            ", Minutes:",
-            ", Label:",
-            ", Sound:",
-            [", Vibrate:", "l", "566"],
+            "Hours=",
+            ", Minutes=",
+            ", Label=",
+            ", Sound=",
+            [", Vibrate=", "l", "566"],
             ["", "e", ", Confirm"],
         ],
     ),
     "567t": ActionCode(
         8,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7"],
         ["Str", "Str", "Str", "Str", "Str", "Int", "Int", "ConditionList"],
         "Calendar Insert",
         ["0", "1", "2", "3", "4", "5", "6"],
         [
-            "In/For Minutes:",
-            ", Calendar:",
-            ", Title:",
-            ", Description:",
-            ", Location:",
+            "In/For Minutes=",
+            ", Calendar=",
+            ", Title=",
+            ", Description=",
+            ", Location=",
             ["", "e", ", Available"],
             ["", "e", ", All Day"],
         ],
     ),
     "568t": ActionCode(0, "", [], [], "DailyRoads Voyager", [], []),
     "5683503e": ActionCode(
         4,
@@ -3083,30 +3142,30 @@
     "56t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Str", "Int", "Str"],
         "Element Border",
         ["0", "1", "2", "3"],
-        ["Scene Name:", ", Element:", ", Width:", ", Colour:"],
+        ["Scene Name=", ", Element=", ", Width=", ", Colour="],
     ),
     "57t": ActionCode(
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["Str", "Str", "Int", "Int", "Int", "Int"],
         "Element Size",
         ["0", "1", "2", "3", "4", "5"],
         [
-            "Scene Name:",
-            ", Element:",
-            [", Orientation:", "l", "57"],
-            ", X:",
-            ", Y:",
-            ", Animation Time (MS):",
+            "Scene Name=",
+            ", Element=",
+            [", Orientation=", "l", "57"],
+            ", X=",
+            ", Y=",
+            ", Animation Time (MS)=",
         ],
     ),
     "570237327t": ActionCode(0, "1040876951t", [], [], "AutoSheets Format Cells", [], []),
     "580953799e": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
@@ -3119,461 +3178,463 @@
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["Str", "Str", "Int", "Int", "Int", "Int"],
         "Element Size",
         ["0", "1", "2", "3", "4", "5"],
         [
-            "Scene Name:",
-            ", Element:",
-            [", Orientation:", "l", "57"],
-            ", Width:",
-            ", Height:",
-            ", Animation Time (MS):",
+            "Scene Name=",
+            ", Element=",
+            [", Orientation=", "l", "57"],
+            ", Width=",
+            ", Height=",
+            ", Animation Time (MS)=",
         ],
     ),
     "590t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Str", "Str", "Int", "Int", "ConditionList"],
         "Variable Split",
         ["0", "1", "2", "3"],
-        ["Name:", ", Splitter:", ["", "e", ", Delete Base"], ["", "e", ", Regex"]],
+        ["Name=", ", Splitter=", ["", "e", ", Delete Base"], ["", "e", ", Regex"]],
     ),
     "592t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Str", "Int"],
         "Variable Join",
         ["0", "1", "2"],
-        ["Name:", ", Joiner:", ["", "e", ", Delete Parts"]],
+        ["Name=", ", Joiner=", ["", "e", ", Delete Parts"]],
     ),
     "595t": ActionCode(
         8,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7"],
         ["Str", "Str", "Int", "Str", "Str", "Str", "Int", "Int"],
         "Variable Query",
         ["0", "1", "2", "3", "4", "5", "6", "7"],
         [
-            "Title:",
-            ", Variable:",
-            [", Input Type:", "l", "595"],
-            ", Default:",
-            ", Background Image:",
-            ", Layout:",
-            ", Timeout (Seconds):",
+            "Title=",
+            ", Variable=",
+            [", Input Type=", "l", "595"],
+            ", Default=",
+            ", Background Image=",
+            ", Layout=",
+            ", Timeout (Seconds)=",
             ["", "e", ", Show Over Keyguard"],
         ],
     ),
     "596t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Int", "Str", "Int"],
         "Variable Convert",
         ["0", "1", "2"],
-        ["Name:", [", Function:", "l", "596"], ", Store Result In:"],
+        ["Name=", [", Function=", "l", "596"], ", Store Result In="],
     ),
     "597t": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Str", "Int", "Int", "Int", "Str"],
         "Variable Section",
         ["0", "1", "2", "3", "4"],
         [
-            "Name:",
-            ", From:",
-            ", Length:",
+            "Name=",
+            ", From=",
+            ", Length=",
             ["", "e", ", Adopt To Fit"],
-            ", Store Result In:",
+            ", Store Result In=",
         ],
     ),
     "598t": ActionCode(
         9,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8"],
         ["Str", "Str", "Int", "Int", "Int", "Str", "Int", "Str", "ConditionList"],
         "Variable Search Replace",
         ["0", "1", "2", "3", "4", "5", "6"],
         [
-            "Variable:",
-            ", Search:",
+            "Variable=",
+            ", Search=",
             ["", "e", ", Ignore Case"],
             ["", "e", ", Multi-Line"],
             ["", "e", ", One Match Only"],
-            ", Show Matches In Array:",
+            ", Show Matches In Array=",
             ["", "e", ", Replace Matches"],
         ],
     ),
     "599e": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Str", "Int", "Int", "Str", "Str"],
         "Intent Received",
         ["1", "2", "3", "4"],
         [
-            "Action:",
-            [", Cat:", "l", "877"],
-            [", Cat:", "l", "877"],
-            ", Schema:",
-            ", Mime Type:",
-            ", Priority:",
+            "Action=",
+            [", Cat=", "l", "877"],
+            [", Cat=", "l", "877"],
+            ", Schema=",
+            ", Mime Type=",
+            ", Priority=",
             ["", "e", ", Stop Event"],
         ],
     ),
     "599t": ActionCode(0, "", [], [], "Due Today", [], []),
     "59t": ActionCode(0, "", [], [], "Reboot", [], []),
     "5s": ActionCode(0, "", [], [], "Calendar Entry", [], []),
     "60t": ActionCode(
         9,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8"],
         ["Str", "Str", "Str", "Str", "Str", "Int", "Int", "Str", "Img"],
         "Element Add GeoMarker",
         ["0", "1", "2", "3", "4", "5"],
         [
-            "Scene Name:",
-            ", Element:",
-            ", Lat,Long:",
-            ", Label:",
-            ", Spot Radius (Meters):",
-            ", Spot Color:",
+            "Scene Name=",
+            ", Element=",
+            ", Lat,Long=",
+            ", Label=",
+            ", Spot Radius (Meters)=",
+            ", Spot Color=",
         ],
     ),
+    "610246503t": ActionCode(0, "1040876951t", [], [], "AutoCast Query", [], []),
     "612t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Str", "Int", "Str"],
         "Element Video Control",
         ["0", "1", "2", "3"],
-        ["Scene Name:", ", Element:", [", Mode:", "l", "612"], ", MilliSeconds:"],
+        ["Scene Name=", ", Element=", [", Mode=", "l", "612"], ", MilliSeconds="],
     ),
-    "61t": ActionCode(2, "", ["0", "1"], ["Int", "ConditionList"], "Vibrate", ["0"], ["Time:"]),
+    "61t": ActionCode(2, "", ["0", "1"], ["Int", "ConditionList"], "Vibrate", ["0"], ["Time="]),
+    "611944049t": ActionCode(0, "1040876951t", [], [], "AutoCast Speak", [], []),
     "62t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "ConditionList"],
         "Vibrate Pattern",
         ["0"],
-        ["Pattern:"],
+        ["Pattern="],
     ),
     "63t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Str", "Str", "Str"],
         "Element Delete GeoMarker",
         ["0", "1", "2", "3"],
-        ["Scene Name:", ", Element:", " Lat,Long:", " Label:"],
+        ["Scene Name=", ", Element=", " Lat,Long=", " Label="],
     ),
     "643t": ActionCode(0, "", [], [], "OfficeTalk", [], []),
     "64t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Str", "Int", "Str"],
         "Element Map Control",
         ["0", "1", "2"],
-        ["Scene Name:", ", Element:", [", Mode:", "l", "64"]],
+        ["Scene Name=", ", Element=", [", Mode=", "l", "64"]],
     ),
     "657t": ActionCode(0, "", [], [], "Record Audio Stop", [], []),
     "65t": ActionCode(
         6,
         "",
         ["0", "1", "2", "3", "4", "5"],
         ["Str", "Str", "Int", "Int", "Int", "ConditionList"],
         "Element Visibility",
         ["0", "1", "2", "3", "4"],
         [
-            "Scene Name:",
-            ", Element Match:",
-            [", Set:", "l", "65"],
-            "Animation Time (MS):",
+            "Scene Name=",
+            ", Element Match=",
+            [", Set=", "l", "65"],
+            "Animation Time (MS)=",
             ["", "e", ", Continue Task Immediately"],
         ],
     ),
     "658527372t": ActionCode(0, "1040876951t", [], [], "AutoTools HTML Read", [], []),
     "664t": ActionCode(
         10,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"],
         ["Str", "Str", "Str", "Str", "Str", "Str", "Str", "Str", "Str", "Str"],
         "Java Function",
         ["0", "1"],
-        ["Class or Object:", ", Function:"],
+        ["Class or Object=", ", Function="],
     ),
     "665t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "Str"],
         "Java Object",
         ["0", "1"],
-        [["Mode:", "l", "665"], ", Name:"],
+        [["Mode=", "l", "665"], ", Name="],
     ),
     "667t": ActionCode(0, "", [], [], "SQL Query", [], []),
     "66t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Str", "Img", "ConditionList"],
         "Element Image",
         ["0", "1", "2"],
-        ["Scene Name:", ", Element:", ", Image:"],
+        ["Scene Name=", ", Element=", ", Image="],
     ),
     "67t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Str", "Int"],
         "Element Depth",
         ["0", "1", "2"],
-        ["Scene Name:", ", Element:", ", Set Depth:"],
+        ["Scene Name=", ", Element=", ", Set Depth="],
     ),
     "68t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Str", "Int"],
         "Element Focus",
         ["0", "1", "2"],
-        ["Scene Name:", ", Element:", ["", "e", ", Set"]],
+        ["Scene Name=", ", Element=", ["", "e", ", Set"]],
     ),
     "697t": ActionCode(0, "", [], [], "Shut Up", [], []),
     "699t": ActionCode(
         7,
         "",
         ["0", "1", "2", "3", "4", "5", "6"],
         ["Str", "Str", "Str", "Int", "Int", "Int", "Int"],
         "Say To File",
         ["0", "1", "2", "3", "4", "5", "6"],
         [
-            "Text:",
-            ", Engine/Voice:",
-            ", File:",
-            ", Pitch:",
-            ", Speed:",
+            "Text=",
+            ", Engine/Voice=",
+            ", File=",
+            ", Pitch=",
+            ", Speed=",
             ["", "e", ", Network"],
             ["", "e", ", Continue Task Immediately"],
         ],
     ),
     "69t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Int", "Int", "Str"],
         "Element Create",
         ["0", "1", "2", "3"],
-        ["Scene Name:", [", Set:", "l", "69"], ["", "e", ", Visible"], ", Content:"],
+        ["Scene Name=", [", Set=", "l", "69"], ["", "e", ", Visible"], ", Content="],
     ),
     "6e": ActionCode(0, "", [], [], "Phone Ringing", [], []),
-    "6s": ActionCode(1, "", ["0"], ["Str"], "Phone Ringing", ["0"], ["Contact:"]),
+    "6s": ActionCode(1, "", ["0"], ["Str"], "Phone Ringing", ["0"], ["Contact="]),
     "701t": ActionCode(0, "", [], [], "Dpad", [], []),
     "702t": ActionCode(0, "", [], [], "Type", [], []),
     "703953103t": ActionCode(0, "1040876951t", [], [], "KLWP Live Wallpaper", [], []),
     "703t": ActionCode(0, "", [], [], "Button", [], []),
     "71t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Str", "Int"],
         "Element Text Size",
         ["0", "1", "2"],
-        ["Scene Name:", ", Element:", ", Text Size:"],
+        ["Scene Name=", ", Element=", ", Text Size="],
     ),
     "721t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Int"],
         "Zoom Visibility",
         ["0", "1"],
-        ["Element:", ["", "e", ", Set"]],
+        ["Element=", ["", "e", ", Set"]],
     ),
     "731t": ActionCode(0, "", [], [], "Take Call", [], []),
     "732t": ActionCode(0, "", [], [], "Radio", [], []),
     "733t": ActionCode(0, "", ["0"], ["Bundle"], "End Call", [], []),
     "734t": ActionCode(0, "", [], [], "Silence Ringer", [], []),
     "735t": ActionCode(0, "", [], [], "Mobile Data 2G/3G", [], []),
     "73t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Str"],
         "Element Destroy",
         ["0", "1"],
-        ["Scene Name:", ", Element:"],
+        ["Scene Name=", ", Element="],
     ),
     "740t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Str"],
         "Zoom Text",
         ["0", "1"],
-        ["Element:", ", Text:"],
+        ["Element=", ", Text="],
     ),
     "741t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Int"],
         "Zoom Text Size",
         ["0", "1"],
-        ["Element:", ", Text Size:"],
+        ["Element=", ", Text Size="],
     ),
     "742t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Str"],
         "Zoom Text Color",
         ["0", "1"],
-        ["Element:", ", Text Color:"],
+        ["Element=", ", Text Color="],
     ),
     "760t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Int"],
         "Zoom Alpha",
         ["0", "1"],
-        ["Element:", ", Set:"],
+        ["Element=", ", Set="],
     ),
     "761t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Str"],
         "Zoom Image",
         ["0", "1"],
-        ["Element:", ", URL:"],
+        ["Element=", ", URL="],
     ),
     "762t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Str", "Str"],
         "Zoom Color",
         ["0", "1", "2"],
-        ["Element:", ", Color:", ", End Color:"],
+        ["Element=", ", Color=", ", End Color="],
     ),
     "774351906t": ActionCode(0, "1040876951t", [], [], "Join Action", [], []),
     "775t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Str"],
         "Write Binary",
         ["0", "1"],
-        ["Variable:", ", File:"],
+        ["Variable=", ", File="],
     ),
     "776t": ActionCode(0, "", [], [], "Read Binary", [], []),
     "778682267t": ActionCode(0, "1040876951t", [], [], "AutoInput Gestures", [], []),
     "779t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Int", "ConditionList"],
         "Notify Cancel",
         ["0"],
-        ["Title:"],
+        ["Title="],
     ),
     "794294329t": ActionCode(0, "1040876951t", [], [], "AutoSheets Add Sheet", [], []),
     "793t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Int"],
         "Zoom State",
         ["0", "1"],
-        ["Element:", ", State:"],
+        ["Element=", ", State="],
     ),
     "794t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Int", "Int", "Int"],
         "Zoom Position",
         ["0", "1", "2", "3"],
-        ["Element:", [", Orientation:", "l", "57"], ", X:", ", Y:"],
+        ["Element=", [", Orientation=", "l", "57"], ", X=", ", Y="],
     ),
     "795t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Int", "Int", "Int"],
         "Zoom Size",
         ["0", "1", "2", "3"],
-        ["Element:", [", Orientation:", "l", "57"], ", Width:", ", Height:"],
+        ["Element=", [", Orientation=", "l", "57"], ", Width=", ", Height="],
     ),
     "7e": ActionCode(
         5,
         "",
         ["0", "1", "2", "3", "4"],
         ["Int", "Str", "Str", "Str", "Str"],
         "Received Text",
         ["0", "1", "2", "3", "4"],
-        [["Type:", "l", "7e"], ", Sender:", ", Content:", ", SIM Card:", ", MMS Body:"],
+        [["Type=", "l", "7e"], ", Sender=", ", Content=", ", SIM Card=", ", MMS Body="],
     ),
     "7s": ActionCode(0, "", [], [], "Cell Near", [], []),
     "801498676t": ActionCode(0, "1040876951t", [], [], "AutoSpotify Albums", [], []),
     "804t": ActionCode(0, "", [], [], "Input Method Select", [], []),
-    "806t": ActionCode(1, "", ["0"], ["Int"], "Turn On", ["0"], ["Block Time:"]),
-    "808t": ActionCode(1, "", ["0"], ["Int"], "Auto Brightness", ["0"], [["Set:", "l", "switch_set"]]),
+    "806t": ActionCode(1, "", ["0"], ["Int"], "Turn On", ["0"], ["Block Time="]),
+    "808t": ActionCode(1, "", ["0"], ["Int"], "Auto Brightness", ["0"], [["Set=", "l", "switch_set"]]),
     "80s": ActionCode(0, "", [], [], "Docked", [], []),
     "810t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Int", "Int", "Int", "Int"],
         "Display Brightness",
         ["0", "1", "2"],
         [
-            "Level:",
+            "Level=",
             ["", "e", ", Disable Safeguard"],
             ["", "e", ", Ignore Current Level"],
         ],
     ),
     "811079103t": ActionCode(0, "1040876951t", [], [], "AutoInput Global Action", [], []),
     "812t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Int", "Int"],
         "Display Timeout",
         ["0", "1", "2"],
-        ["Secs:", ", Mins:", ", Hours:"],
+        ["Secs=", ", Mins=", ", Hours="],
     ),
     "815t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Int", "Str", "Str"],
         "List Apps",
         ["0", "1", "2"],
-        [["Type:", "l", "815"], ", Match:", ", Store Result In:"],
+        [["Type=", "l", "815"], ", Match=", ", Store Result In="],
     ),
     "819222800t": ActionCode(0, "1040876951t", [], [], "AutoSpotify Tracks", [], []),
-    "820t": ActionCode(1, "", ["0"], ["Int"], "Stay On", ["0"], [["Mode:", "l", "820"]]),
+    "820t": ActionCode(1, "", ["0"], ["Int"], "Stay On", ["0"], [["Mode=", "l", "820"]]),
     "822t": ActionCode(
         1,
         "",
         ["0"],
         ["Int"],
         "Display Autorotate",
         ["0"],
-        [["Set:", "l", "switch_set"]],
+        [["Set=", "l", "switch_set"]],
     ),
     "864692752t": ActionCode(0, "1040876951t", [], [], "Join", [], []),
     "8618362t": ActionCode(0, "1040876951t", [], [], "AutoSpotify Notification", [], []),
     "877t": ActionCode(
         11,
         "",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "10"],
@@ -3589,119 +3650,119 @@
             "Str",
             "Int",
             "ConditionList",
         ],
         "Send Intent",
         ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"],
         [
-            "Action:",
-            [", Mode:", "l", "877"],
-            ", Mime Type:",
-            ", Data:",
-            ", Extra:",
-            ", Extra:",
-            ", Extra:",
-            ", Package:",
-            ", Class:",
-            [", Target:", "l", "877a"],
+            "Action=",
+            [", Mode=", "l", "877"],
+            ", Mime Type=",
+            ", Data=",
+            ", Extra=",
+            ", Extra=",
+            ", Extra=",
+            ", Package=",
+            ", Class=",
+            [", Target=", "l", "877a"],
         ],
     ),
     "888t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Int", "Int"],
         "Variable Add",
         ["0", "1", "2"],
-        ["Name:", ", Value:", ", Wrap Around:"],
+        ["Name=", ", Value=", ", Wrap Around="],
     ),
     "890t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Int", "Int"],
         "Variable Subtract",
         ["0", "1", "2"],
-        ["Name:", ", Value:", ", Wrap Around:"],
+        ["Name=", ", Value=", ", Wrap Around="],
     ),
     "8e": ActionCode(0, "", [], [], "Received Data SMS", [], []),
     "900t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Str", "Int"],
         "Browse Files",
         ["0", "1", "2"],
-        ["Directory:", ", Match:", ["", "e", ", Include Hidden Files"]],
+        ["Directory=", ", Match=", ["", "e", ", Include Hidden Files"]],
     ),
-    "901t": ActionCode(1, "", ["0"], ["Int"], "Stop Location", ["0"], [["Set:", "l", "901"]]),
+    "901t": ActionCode(1, "", ["0"], ["Int"], "Stop Location", ["0"], [["Set=", "l", "901"]]),
     "902t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Int", "Int", "Int", "Int"],
         "Get Location",
         ["0", "1", "2", "3"],
         [
-            ["Set:", "l", "901"],
-            ", Timeout (Seconds):",
+            ["Set=", "l", "901"],
+            ", Timeout (Seconds)=",
             ["", "e", ", Continue Task Immediately"],
             ["", "e", ", Keep Tracking"],
         ],
     ),
     "903t": ActionCode(
         7,
         "",
         ["0", "1", "2", "3", "4", "5", "6"],
         ["Str", "Int", "Str", "Int", "Int", "Int", "Bundle"],
         "Get Voice",
         ["0", "1", "2", "3", "4", "5"],
         [
-            "Title:",
-            [", Mode:", "l", "903"],
-            ", Language:",
-            ", Maximum Results:",
-            ", Timeout:",
+            "Title=",
+            [", Mode=", "l", "903"],
+            ", Language=",
+            ", Maximum Results=",
+            ", Timeout=",
             ["", "e", ", Hide Dialog"],
         ],
     ),
     "904t": ActionCode(0, "", [], [], "Voice Command", [], []),
-    "905t": ActionCode(1, "", ["0"], ["Int"], "Location Mode", ["0"], [["Mode:", "l", "905"]]),
+    "905t": ActionCode(1, "", ["0"], ["Int"], "Location Mode", ["0"], [["Mode=", "l", "905"]]),
     "906355163t": ActionCode(0, "1040876951t", [], [], "AutoWear Voice Screen", [], []),
-    "906t": ActionCode(1, "", ["0"], ["Int"], "Immersive Mode", ["0"], [["Mode:", "l", "906"]]),
+    "906t": ActionCode(1, "", ["0"], ["Int"], "Immersive Mode", ["0"], [["Mode=", "l", "906"]]),
     "906686306e": ActionCode(0, "1040876951t", [], [], "AutoLocation Geofences", [], []),
-    "907t": ActionCode(1, "", ["0"], ["Str"], "Status Bar Icons", ["0"], ["Icons To Hide:"]),
+    "907t": ActionCode(1, "", ["0"], ["Str"], "Status Bar Icons", ["0"], ["Icons To Hide="]),
     "907418897t": ActionCode(0, "1040876951t", [], [], "AutoTools Action Report", [], []),
-    "909t": ActionCode(1, "", ["0"], ["Int"], "Contacts", ["0"], [["Mode:", "l", "909"]]),
+    "909t": ActionCode(1, "", ["0"], ["Int"], "Contacts", ["0"], [["Mode=", "l", "909"]]),
     "90t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Int", "Str"],
         "Call",
         ["0", "1", "2"],
-        ["Number:", ["", "e", ", Auto Dial"], ", Sim Card:"],
+        ["Number=", ["", "e", ", Auto Dial"], ", Sim Card="],
     ),
-    "910t": ActionCode(1, "", ["0"], ["Int"], "Call Log", ["0"], [["Mode:", "l", "910"]]),
+    "910t": ActionCode(1, "", ["0"], ["Int"], "Call Log", ["0"], [["Mode=", "l", "910"]]),
     "911t": ActionCode(0, "", [], [], "Gentle Alarm", [], []),
     "915t": ActionCode(0, "", [], [], "CPU", [], []),
     "917310686t": ActionCode(0, "1040876951t", [], [], "AutoSpotify Artists", [], []),
     "918403287t": ActionCode(0, "1040876951t", [], [], "AutoNotification Categories", [], []),
     "921575593t": ActionCode(0, "1040876951t", [], [], "AutoInput Keyguard", [], []),
     "940160580t": ActionCode(0, "1040876951t", [], [], "AutoShare", [], []),
     "941t": ActionCode(
         4,
         "",
         ["0", "1", "2", "3"],
         ["Str", "Str", "Int", "Int"],
         "HTML Popup",
         ["0", "1", "2", "3"],
         [
-            "Code:",
-            ", Layout:",
+            "Code=",
+            ", Layout=",
             ", Timeout (Seconds)",
             ["", "e", ", Show Over Keyguard"],
         ],
     ),
     "956t": ActionCode(0, "", [], [], "NFC Settings", [], []),
     "957t": ActionCode(0, "", [], [], "Android Beam Settings", [], []),
     "958t": ActionCode(0, "", [], [], "NFC Payment Settings", [], []),
@@ -3709,43 +3770,341 @@
     "95t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Int"],
         "Call Block",
         ["0", "1"],
-        ["Number Match:", ["", "e", "Info"]],
+        ["Number Match=", ["", "e", "Info"]],
     ),
     "96135575t": ActionCode(0, "1040876951t", [], [], "AutoLocation Info", [], []),
     "96585332t": ActionCode(0, "1040876951t", [], [], "AutoWear Settings", [], []),
     "97t": ActionCode(
         3,
         "",
         ["0", "1", "2"],
         ["Str", "Str", "Int"],
         "Call Divert",
         ["0", "1", "2"],
-        ["From Match:", ", To:", ["", "e", ", Info"]],
+        ["From Match=", ", To=", ["", "e", ", Info"]],
     ),
     "985050481t": ActionCode(0, "1040876951t", [], [], "Actions", [], []),
     "987t": ActionCode(0, "", [], [], "Soft Keyboard", [], []),
     "988t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Int", "Int"],
         "Car Mode",
         ["0", "1"],
-        [["Set:", "l", "switch_set"], ["", "e", ", Go Home"]],
+        [["Set=", "l", "switch_set"], ["", "e", ", Go Home"]],
     ),
     "989t": ActionCode(0, "", [], [], "Night Mode", [], []),
     "999t": ActionCode(0, "", [], [], "Set Light", [], []),
     "99t": ActionCode(
         2,
         "",
         ["0", "1"],
         ["Str", "Int"],
         "Call Revert",
         ["0", "1"],
-        ["Number:", ["", "e", "Info"]],
+        ["Number=", ["", "e", "Info"]],
+    ),
+    # Scene Element type definitions
+    #     ["numargs", "redirect", "args", "types", "display", "reqargs", "evalargs"],
+    "TextElement": ActionCode(
+        9,
+        "",
+        ["0", "1", "2", "3", "4", "5", "6", "7", "8"],
+        ["Str", "Str", "Int", "Int", "Str", "Str", "Int", "Int", "Int"],
+        "",
+        ["0", "1", "2", "3", "4", "5", "6", "7", "8"],
+        [
+            "Name=",
+            ", Text=",
+            ", Text Size=",
+            ", Text Width Scale Percent (100=0%)=",
+            ", Text Color=",
+            ", Font=",
+            [", Position=", "l", "TextElement1"],
+            [", Vertical Fit Mode=", "l", "TextElement2"],
+            [", Text Format=", "l", "TextElement3"],
+        ],
+    ),
+    "EditTextElement": ActionCode(
+        9,
+        "",
+        ["0", "1", "2", "3", "4", "5", "6", "7", "8"],
+        ["Str", "Str", "Int", "Int", "Str", "Str", "Int", "Int", "Int"],
+        "",
+        ["0", "1", "2", "3", "4", "5", "6", "7", "8"],
+        [
+            "Name=",
+            ", Text=",
+            ", Text Size=",
+            ", Text Width Scale Percent=",
+            ", Text Color=",
+            ", Font=",
+            [", Position=", "l", "TextElement1"],
+            [", Input Type=", "l", "EditTextElement"],
+            ", Maximum Characters=",
+        ],
+    ),
+    "RectElement": ActionCode(
+        8,
+        "",
+        ["0", "1", "2", "3", "4", "5", "6", "7"],
+        ["Str", "Int", "Str", "Str", "Int", "Str", "Int", "Int"],
+        "",
+        ["0", "1", "2", "3", "4", "5", "6", "7"],
+        [
+            "Name=",
+            [", Shader=", "l", "RectElement1"],
+            ", Color=",
+            ", End Color=",
+            ", Border Width=",
+            ", Border XColor=",
+            ", Corner Radius=",
+            [", Rounded Corners=", "l", "RectElement2"],
+        ],
+    ),
+    "ImageElement": ActionCode(
+        3,
+        "",
+        ["0", "1", "2"],
+        ["Str", "Img", "Int"],
+        "",
+        ["0", "1", "2"],
+        [
+            "Name=",
+            ", Image=",
+            ", Alpha=",
+        ],
+    ),
+    "WebElement": ActionCode(
+        8,
+        "",
+        ["0", "1", "2", "3", "4", "5", "6", "7"],
+        ["Str", "Int", "Str", "Int", "Str", "Str", "Str", "Int"],
+        "",
+        ["0", "1", "2", "3", "4", "5", "6", "7"],
+        [
+            "Name=",
+            [", Mode=", "l", "WebElement"],
+            ", Source=",
+            ["", "e", ", Allow Phone Access"],
+            ["", "e", ", Self Handle Links"],
+            ["", "e", ", DB API"],
+            ["", "e", ", Support Popups"],
+            ", User Agent=",
+        ],
+    ),
+    "ListElement": ActionCode(
+        7,
+        "",
+        ["0", "1", "2", "3", "4", "5", "6"],
+        ["Str", "Int", "Str", "Int", "Int", "Int", "Int"],
+        "",
+        ["0", "1", "2", "3", "5", "6"],
+        [
+            "Name=",
+            [", Source=", "l", "ListElement1"],
+            [", Selection Mode=", "l", "ListElement2"],
+            [", Selection Mode=", "l", "ListElement2"],
+            ", Horizontal Space=",
+            ", Vertical Space=",
+        ],
+    ),
+    "ButtonElement": ActionCode(
+        8,
+        "",
+        ["0", "1", "2", "3", "4", "5", "6", "7"],
+        ["Str", "Str", "Int", "Int", "Str", "Str", "Int", "Img"],
+        "",
+        ["0", "1", "2", "3", "4", "5", "6", "7"],
+        [
+            "Name=",
+            ", Label=",
+            ", Label Size=",
+            ", Label Width Scale %=",
+            ", Label Color=",
+            ", Font=",
+            [", Position=", "l", "TextElement1"],
+            ", Icon=",
+        ],
+    ),
+    "OvalElement": ActionCode(
+        6,
+        "",
+        ["0", "1", "2", "3", "4", "5"],
+        ["Str", "Int", "Str", "Str", "Int", "Str"],
+        "",
+        ["0", "1", "2", "3", "4", "5"],
+        [
+            "Name=",
+            [", Shader=", "l", "RectElement1"],
+            ", Color=",
+            ", End Color=",
+            ", Border Width=",
+            ", Border Color=",
+        ],
+    ),
+    "CheckBoxElement": ActionCode(
+        2,
+        "",
+        ["0", "1"],
+        ["Str", "Int"],
+        "",
+        ["0", "1"],
+        [
+            "Name=",
+            ["1", "e", ", Checked"],
+        ],
+    ),
+    "SpinnerElement": ActionCode(
+        5,
+        "",
+        ["0", "1", "2", "3", "4"],
+        ["Str", "Int", "Str", "", "Str"],
+        "",
+        ["0", "1", "2", "4"],
+        [
+            "Name=",
+            [", Source=", "l", "ListElement1"],
+            ", Variable=",
+            ", Popup Background Color=",
+        ],
+    ),
+    "DoodleElement": ActionCode(
+        3,
+        "",
+        ["0", "1", "2"],
+        ["Str", "Int", "Int"],
+        "",
+        ["0", "1", "2"],
+        [
+            "Name=",
+            ", Doodle=",
+            ", Alpha=",
+        ],
+    ),
+    "SceneElement": ActionCode(  # MapElement is called SceneElement for some reason
+        6,
+        "Map",
+        ["0", "1", "2", "3", "4", "5"],
+        ["Str", "Str", "Int", "Int", "Int", "Int"],
+        "Map",
+        ["0", "1", "2", "3", "4", "5"],
+        [
+            "Name=",
+            ", Lat/Long=",
+            ", Zoom=",
+            ["", "e", ", Show Traffic"],
+            ["", "e", ", Show Satellite"],
+            ["", "e", ", Show Roads"],
+        ],
+    ),
+    "MenuElement": ActionCode(
+        5,
+        "",
+        ["0", "1", "2", "3", "4"],
+        ["Str", "Int", "Int", "Int", "Int"],
+        "",
+        ["0", "1", "2", "3", "4"],
+        [
+            "Name=",
+            [", Source=", "l", "ListElement1"],
+            [", Selection Mode=", "l", "ListElement2"],
+            ", Horizontal Space=",
+            ", Vertical Space=",
+        ],
+    ),
+    "PickerElement": ActionCode(
+        6,
+        "",
+        ["0", "1", "2", "3", "4", "5"],
+        ["Str", "Str", "Str", "Str", "Int", "Int"],
+        "",
+        ["0", "1", "2", "3", "4", "5"],
+        [
+            "Name=",
+            ", Min=",
+            ", Max=",
+            ", Default=",
+            ["", "e", ", Wrap Around"],
+            [", Format=", "l", "NumberPickerElement"],
+        ],
+    ),
+    "PropertiesElement": ActionCode(
+        8,
+        "",
+        ["0", "1", "2", "3", "4", "5", "6", "7"],
+        ["Int", "Int", "Str", "Int", "Str", "Str", "Img", "Str"],
+        "",
+        ["0", "1", "2", "3", "4", "5", "6", "7"],
+        [
+            [", Property Type=", "l", "PropertyElement1"],
+            [", Orientation=", "l", "PropertyElement2"],
+            ", Background_Color=",
+            [", Property Type=", "l", "PropertyElement3"],
+            ", Title=",
+            ", Subtitle=",
+            ", Icon=",
+            ", Tab Labels=",
+        ],
+    ),
+    "ListElementItem": ActionCode(
+        0,
+        "",
+        [],
+        [],
+        "",
+        [],
+        [],
+    ),
+    "SliderElement": ActionCode(
+        7,
+        "",
+        ["0", "1", "2", "3", "4", "5", "6"],
+        ["Str", "Int", "Int", "Int", "Int", "Int", "Img"],
+        "",
+        ["0", "1", "2", "3", "4", "5", "6"],
+        [
+            "Name=",
+            [", Orientation=", "l", "SliderElement1"],
+            ", Min=",
+            ", Max=",
+            ", Default=",
+            [", Show Indicators=", "l", "SliderElement2"],
+            ", Icon=",
+        ],
+    ),
+    "SwitchElement": ActionCode(
+        2,
+        "",
+        ["0", "1"],
+        ["Str", "Int"],
+        "",
+        ["0", "1"],
+        [
+            "Name=",
+            ["", "e", ", Checked"],
+        ],
+    ),
+    "ToggleElement": ActionCode(
+        7,
+        "",
+        ["0", "1", "2", "3", "4", "5", "6"],
+        ["Str", "Int", "Str", "Str", "Int", "Int", "Str"],
+        "",
+        ["0", "1", "2", "3", "4", "5", "6"],
+        [
+            "Name=",
+            ["", "e", ", On"],
+            ", Off Label=",
+            ", On Label=",
+            ", Label Size=",
+            ", Label Width Width Scale Percent (100=0%)=",
+            ", Label Color=",
+        ],
     ),
 }
```

### Comparing `maptasker-2.6.3/maptasker/src/actiond.py` & `maptasker-3.2.2/maptasker/src/actiond.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,34 @@
+"""Action dictionary functions."""
+
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
 # actiond: Task Action dictionary functions for MapTasker                              #
 #                                                                                      #
 # GNU General Public License v3.0                                                      #
 # Permissions of this strong copyleft license are conditioned on making available      #
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
-import contextlib
-from typing import Any
+from __future__ import annotations
 
-import defusedxml.ElementTree  # Need for type hints
+import contextlib
+from typing import TYPE_CHECKING, Any
 
 import maptasker.src.action as get_action
 from maptasker.src.actionc import action_codes
 from maptasker.src.sysconst import logger
 
+if TYPE_CHECKING:
+    import defusedxml.ElementTree
+
 IGNORE_ITEMS = ["code", "label", "se", "on", "ListElementItem", "pri", "pin"]
 
 
 # ##################################################################################
 # Provide the Action dictionary to the caller
 # ##################################################################################
 # def get_dict() -> defusedxml.ElementTree:
@@ -32,15 +37,16 @@
 
 # ##################################################################################
 # Update the dictionary for the Action code
 #  This is only called if the action code is already in our master
 #  dictionary of codes.
 # ##################################################################################
 def update_action_codes(
-    action: defusedxml.ElementTree.XML, the_action_code_plus: defusedxml.ElementTree
+    action: defusedxml.ElementTree.XML,
+    the_action_code_plus: defusedxml.ElementTree,
 ) -> defusedxml.ElementTree:
     """
     Update the dictionary for the Action code
         :param action: <Action> xml element
         :param the_action_code_plus: the Action code with "action type"
                 (e.g. 861t, t=Task, e=Event, s=State)
         :return: nothing
@@ -59,25 +65,26 @@
         with contextlib.suppress(Exception):
             action_codes[the_action_code_plus].numargs = arg_count
             action_codes[the_action_code_plus].args = arg_nums
             action_codes[the_action_code_plus].types = type_list
 
         logger.debug(
             "update_action_codes:"
-            f" {the_action_code_plus} {str(action_codes[the_action_code_plus])} numargs of {action_codes[the_action_code_plus].numargs} update to {arg_count}:  needs to be updated in actionc.py!"
+            f" {the_action_code_plus} {action_codes[the_action_code_plus]!s} numargs of {action_codes[the_action_code_plus].numargs} update to {arg_count}:  needs to be updated in actionc.py!",
         )
     return
 
 
 # ##################################################################################
 # Build the dictionary for the Action code.  Only called if the action code is not
 #   in our master dictionary of codes.
 # ##################################################################################
 def build_new_action_codes(
-    action: defusedxml.ElementTree.XML, the_action_code_plus: defusedxml.ElementTree
+    action: defusedxml.ElementTree.XML,
+    the_action_code_plus: defusedxml.ElementTree,
 ) -> defusedxml.ElementTree:
     """
     Build the dictionary for the Action code
         :param action: <Action> xml element
         :param the_action_code_plus: the Action code with "action type" (e.g. 861t, t=Task, e=Event, s=State)
         :return: nothing
     """
@@ -126,40 +133,21 @@
     else:
         build_new_action_codes(action, the_action_code_plus)
 
     return
 
 
 # ##################################################################################
-# See if the display name is already in our Action dictionary.  If not, add it.
-# ##################################################################################
-def add_name_to_action_codes(
-    the_action_code_plus: defusedxml.ElementTree.XML,
-    display_name: defusedxml.ElementTree,
-) -> defusedxml.ElementTree:
-    """
-    See if the display name is already in our Action dictionary.  If not, add it.
-        :param the_action_code_plus: the Action code with "action type"
-                (e.g. 861t, t=Task, e=Event, s=State)
-        :param display_name: the name to appear in the output for this action
-        :return: nothing
-    """
-    if the_action_code_plus not in action_codes:
-        build_new_action_codes("", the_action_code_plus)
-    if display_name not in action_codes[the_action_code_plus]:
-        action_codes[the_action_code_plus].display = display_name
-    return
-
-
-# ##################################################################################
 # Given a child xml element, determine if it is a boolean of condtion
 # add return if in a list
 # ##################################################################################
 def get_boolean_or_condition(
-    child: defusedxml.ElementTree, condition_list: list, boolean_list: list
+    child: defusedxml.ElementTree,
+    condition_list: list,
+    boolean_list: list,
 ) -> tuple[list, list]:
     """
     Evaluates the condition/boolean and updates the condition_list and boolean_list.
 
     Args:
         child (Element): The XML element to evaluate.
         condition_list (list): The list of conditions.
@@ -195,8 +183,7 @@
     """
     condition_list, boolean_list = [], []
     condition_list_str = code_action.find("ConditionList")
     if condition_list_str is not None:
         for child in condition_list_str:
             condition_list, boolean_list = get_boolean_or_condition(child, condition_list, boolean_list)
     return condition_list, boolean_list
-    return condition_list, boolean_list
```

### Comparing `maptasker-2.6.3/maptasker/src/actiont.py` & `maptasker-3.2.2/maptasker/src/actiont.py`

 * *Files 6% similar despite different names*

```diff
@@ -302,14 +302,15 @@
         "Global",
         "Local",
         "Profiles",
         "Scenes",
         "Tasks",
         "Timer Widget Remaining",
         "Current Task Name",
+        "Used Memory",
     ],
     "348": [
         "AutoRotate",
         "Orientation",
         "DPI",
         "Available Resolution",
         "Hardware Resolution",
@@ -319,14 +320,15 @@
         "Navigation Bar Height",
         "Navigation Bar Top Offset",
         "Navigation Bar Top Offset",
         "Status Bar Offset",
     ],
     "349": ["Android ID", "User ID"],
     "351": ["OAuth 2.0", "Username and Password"],
+    "352": ["Mobile", "Wifi", "Bluetooth", "Ethernet", "VPN", "MMS"],
     "358": ["Single Device", "Paired Devices", "Scan Devices"],
     "363": [
         "Auto",
         "2G",
         "3G",
         "4G",
         "2G and 3G",
@@ -351,14 +353,24 @@
         "Sort Numeric, Integer",
         "Sort Numeric",
         "Floating-Point",
         "Squash",
     ],
     "374": ["Start", "Stop", "Query"],
     "378": ["Select Single Item", "Multiple Choices"],
+    "379": [
+        "Custom",
+        "Freeze App",
+        "Suspend App",
+        "Kill App",
+        "Clear App Data",
+        "Reboot",
+        "User Restrictions",
+        "Backup Service",
+    ],
     "380": ["Text", "File", "Redirect"],
     "383": ["Connectivity", "NFC", "Volume", "WiFi", "Media Output"],
     "384": ["Add/Edit", "Delete"],
     "384a": ["Button", "Toggle", "Range", "Toggle Range", "No Action"],
     "386": ["Disallow", "Allow"],
     "391": ["Show/Update", "Dismiss"],
     "391a": ["Animation", "Progress Bar"],
@@ -405,14 +417,15 @@
         "Stop",
         "Play [Simulated Only]",
         "Rewind",
         "Fast Forward",
     ],
     "455": ["Default", "Microphone", "Call Outgoing", "Call Incoming", "Call"],
     "455a": ["MP4", "3GPP", "AMR Narrowband", "AMR Wideband"],
+    "446": ["Directories", "Files"],
     "490": ["Grab", "Release"],
     "512": ["Expanded", "Collapsed"],
     "523": [
         "Red",
         "Green",
         "Blue",
         "Yellow",
@@ -532,8 +545,76 @@
     ],
     "2079e": ["Volume Up", "Volume Down", "Volume Up Or Down"],
     "2081e": ["Playing or Not Playing", "Playing", "Not Playing"],
     "3001e": ["Left-Right", "Up-Down", "Backwards-Forwards"],
     "3001ea": ["Very Low", "Low", "Medium", "High", "Very High"],
     "3001eb": ["Very Short", "Short", "Medium", "Long", "Very Long"],
     "switch_set": ["Off", "On", "Toggle"],
+    # Scene elements
+    "TextElement1": [
+        "Center",
+        "Top",
+        "Bottom",
+        "Left",
+        "Right",
+        "Top Left",
+        "Top Right",
+        "Bottom Left",
+        "Bottom Right",
+    ],
+    "TextElement2": [
+        "None",
+        "Reduce Text Size",
+        "Allow Scrolling",
+    ],
+    "TextElement3": [
+        "Plain Text",
+        "Text With Links",
+        "HTML",
+    ],
+    "EditTextElement": [
+        "Caps / Word",
+        "Caps / All",
+        "Numeric / Decimal",
+        "Numeic / Integer",
+        "Password",
+        "Phone Number",
+        "Passcode",
+    ],
+    "RectElement1": [
+        "None",
+        "Horizontal",
+        "Vertical",
+        "Diagonal, Top Left",
+        "Diagonal, Bottom Left",
+        "Radial",
+    ],
+    "RectElement2": [
+        "All",
+        "Top",
+        "Bottom",
+        "Left",
+        "Right",
+    ],
+    "WebElement": ["URL", "File", "Direct"],
+    "ListElement1": ["Manual", "Variable Array", "Variable"],
+    "ListElement2": ["None", "Single", "Multiple"],
+    "NumberPickerElement": ["Normal", "Prefixed Zeroes"],
+    "PropertyElement1": ["Overlay", "Dialog", "Activity"],
+    "PropertyElement2": [
+        "System",
+        "Landscape",
+        "Portrait",
+        "User",
+        "Behind",
+        "Sensor",
+        "No Sensor",
+        "Sensor Landscape",
+        "Sensor Portrait",
+        "Reverse Landscape",
+        "Reverse Portrait",
+        "Full Sensor",
+    ],
+    "PropertyElement3": ["System", "Dark", "Light"],
+    "SliderElement1": ["Horizontal", "Rotated Left", "rotated Right"],
+    "SliderElement2": ["Never", "While Changing", "Always"],
 }
```

### Comparing `maptasker-2.6.3/maptasker/src/addcss.py` & `maptasker-3.2.2/maptasker/src/addcss.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+"""Add required formatting CSS to HTML output"""
+
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
 # addcss: Add formatting CSS to output HTML for the colors and font to use             #
 #                                                                                      #
 # Permissions of this strong copyleft license are conditioned on making available      #
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
+import contextlib
 
-from maptasker.src.sysconst import FONT_FAMILY, FormatLine
 from maptasker.src.primitem import PrimeItems
+from maptasker.src.sysconst import FONT_FAMILY, FormatLine
 
 
 def add_css() -> None:
     """
     Add formatting CSS to output HTML for the colors and font to use.
     We must re-add the font each time in case a Tasker element overrides the font.
         Args:
@@ -31,35 +34,46 @@
     )
 
     # Go through all colors
 
     # First, get the liost of colors and reverse the dictionary
     if PrimeItems.colors_to_use:
         for color_argument_name in PrimeItems.colors_to_use:
-            try:
+            with contextlib.suppress(KeyError):
                 if PrimeItems.colors_to_use[color_argument_name]:
                     our_html = f'color: {PrimeItems.colors_to_use[color_argument_name]}{FONT_FAMILY}{PrimeItems.program_arguments["font"]}'
                     PrimeItems.output_lines.add_line_to_output(
                         5,
                         f".{color_argument_name} {{{our_html}}}",
                         FormatLine.dont_format_line,
                     )
-            except KeyError:
-                continue
 
-    # Add CSS for Bullet color
-    bullet_color = PrimeItems.colors_to_use["bullet_color"]
-    bullet_css = """ul {list-style: none;}
-
-ul li::before {
-    content: "\\2756";
-    color: red;
-    font-weight: bold;
-    display: inline-block;
-    width: 1em;
-    margin-left: -1em;
-}"""
-    bullet_css = bullet_css.replace("red", bullet_color)
-    PrimeItems.output_lines.add_line_to_output(5, bullet_css, FormatLine.dont_format_line)
+    #     # Add CSS for Bullet color
+    #     bullet_color = PrimeItems.colors_to_use["bullet_color"]
+    #     bullet_css = """ul {list-style: none;}
+
+    # ul li::before {
+    #     content: "\\2756";
+    #     color: red;
+    #     font-weight: bold;
+    #     display: inline-block;
+    #     width: 1em;
+    #     margin-left: -1em;
+    # }"""
+    #     bullet_css = bullet_css.replace("red", bullet_color)
+    #     PrimeItems.output_lines.add_line_to_output(5, bullet_css, FormatLine.dont_format_line)
+
+    # Add css for Tasker Project/Profile/Task/Scene/SceneTask tabs
+    tabs = """
+.resettab {display: inline-block; margin-left: 0;}
+.normtab {display: inline-block; margin-left: 20;}
+.projtab {display: inline-block; margin-left: 20;}
+.proftab {display: inline-block; margin-left: 40;}
+.tasktab {display: inline-block; margin-left: 70;}
+.actiontab {display: inline-block; margin-left: 80;}
+.scenetab {display: inline-block; margin-left: 20;}
+.scenetasktab {display: inline-block; margin-left: 30;}
+    """
+    PrimeItems.output_lines.add_line_to_output(5, tabs, FormatLine.dont_format_line)
 
     # End the style css
     PrimeItems.output_lines.add_line_to_output(5, "</style>\n", FormatLine.dont_format_line)
```

### Comparing `maptasker-2.6.3/maptasker/src/caveats.py` & `maptasker-3.2.2/maptasker/src/caveats.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
 
 from maptasker.src.format import format_html
-from maptasker.src.sysconst import FormatLine
 from maptasker.src.primitem import PrimeItems
+from maptasker.src.sysconst import FormatLine
 
 
 def display_caveats() -> None:
     """
     Output the program caveats at the very end
     Inputs:
     - None
@@ -77,8 +77,12 @@
             ),
         )
     # Start the output
     PrimeItems.output_lines.add_line_to_output(0, "<hr>", FormatLine.dont_format_line)
 
     # Output all caveats
     for caveat in caveats:
-        PrimeItems.output_lines.add_line_to_output(0, caveat, FormatLine.dont_format_line)
+        PrimeItems.output_lines.add_line_to_output(
+            0,
+            caveat,
+            ["", "trailing_comments_color", FormatLine.add_end_span],
+        )
```

### Comparing `maptasker-2.6.3/maptasker/src/clip.py` & `maptasker-3.2.2/maptasker/src/clip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""
+# ruff: noqa
+r"""
 DO NOT DELETE THE AUTHOR COPYRIGHT
 ©Connor Talbot 2021 - https://github.com/con-dog/clippy
 
 clip.py - Animate and color a given directory of .txt files.
 
 The text in PIC should be 'frames' in a sequence
 to give the impression of animation. For steps to make your own, visit the
@@ -60,14 +61,15 @@
 author if copying
 """
 
 import os
 import re
 import sys
 import time
+from maptasker.src.primitem import PrimeItems
 
 # COLORS: FOREGROUND = F, BACKGROUND = B, Value = ANSI value
 COLORS = {
     "F_BLK": "\033[30m",
     "B_BLK": "\033[40m",  # BLACK
     "F_RED": "\033[31m",
     "B_RED": "\033[41m",  # RED
@@ -122,58 +124,58 @@
 CURSOR_ON = "\033[?25h"  # makes cursor visible
 CURSOR_SAVE_POS = "\033[s"  # saves cursor position
 CURSOR_RESTORE_POS = "\033[u"  # returns cursor to last saved position
 
 PIC = (
     [
         ".......|~......",
-        "....../.\......",
-        ")..|~/___\.|~..",
-        "../_\|::.|/_\..",
-        "..|$||/^\||$|..",
+        r"....../.\......",
+        r")..|~/___\.|~..",
+        r"../_\|::.|/_\..",
+        r"..|$||/^\||$|..",
         "..|nnn|I|nnn|..",
     ],
     [
         "......~|.......",
-        "(x).../.\......",
-        "..~|./___\.|~..",
-        "../_\|::.|/_\..",
-        "..|$||/^\||$|..",
+        r"(x).../.\......",
+        r"..~|./___\.|~..",
+        r"../_\|::.|/_\..",
+        r"..|$||/^\||$|..",
         "..|nnn|I|nnn|..",
     ],
     [
         "...(X).|~......",
-        "....../.\......",
-        "..~|./___\~|...",
-        "../_\|::.|/_\..",
-        "..|$||/^\||$|..",
+        r"....../.\......",
+        r"..~|./___\~|...",
+        r"../_\|::.|/_\..",
+        r"..|$||/^\||$|..",
         "..|nnn|I|nnn|..",
     ],
     [
         "......~|.(X)...",
-        "....../.\......",
-        "...|~/___\.|~..",
-        "../_\|::.|/_\..",
-        "..|$||/^\||$|..",
+        r"....../.\......",
+        r"...|~/___\.|~..",
+        r"../_\|::.|/_\..",
+        r"..|$||/^\||$|..",
         "..|nnn|I|nnn|..",
     ],
     [
         ".*....~|..*....",
-        "...*../.\....(o",
-        "..~|./___\.|~..",
-        "../_\|::.|/_\..",
-        "..|$||/^\||$|..",
+        r"...*../.\....(o",
+        r"..~|./___\.|~..",
+        r"../_\|::.|/_\..",
+        r"..|$||/^\||$|..",
         "..|nnn|I|nnn|..",
     ],
     [
         "...*...|~....*.",
-        ".*..*./.\.*...*",
-        "...|~/___\~|..(",
-        "../_\|::.|/_\..",
-        "..|$||/^\||$|..",
+        r".*..*./.\.*...*",
+        r"...|~/___\~|..(",
+        r"../_\|::.|/_\..",
+        r"..|$||/^\||$|..",
         "..|nnn|I|nnn|..",
     ],
 )
 
 PIC_COLORS = [
     "[0][7] = F_WHT, B_BLU",
     "[0][7] = F_WHT, B_BLU",
@@ -212,15 +214,15 @@
 
     pass
 
 
 class Clip:
     """A class to manage all aspects of a clip."""
 
-    def __init__(self, source_folder, play_speed, play_cycles, color=False):
+    def __init__(self, source_folder, play_speed, play_cycles, color=False) -> None:
         """Initialize instance of Tile"""
         sys.stdout.write(CURSOR_OFF)
         self._source_folder = source_folder
         self.play_speed = 5.1 - (play_speed / 20)
         self.play_cycles = play_cycles
         self._color = color
 
@@ -357,9 +359,10 @@
     # dance = "/clip/dance"  # Colors = False
     colored = False
     if not figure:
         figure = "/clip/castles"  # Colors = False
 
     colored = True
 
-    my_output_dir = f"{os.getcwd()}/clip/{figure}"
+    my_output_dir = f"{os.getcwd()}{PrimeItems.slash}clip{PrimeItems.slash}{figure}"
     clippy(my_output_dir, 100, 3, colored)
+    print("\a")  # Bell/alert
```

### Comparing `maptasker-2.6.3/maptasker/src/colors.py` & `maptasker-3.2.2/maptasker/src/colors.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.6.3/maptasker/src/colrmode.py` & `maptasker-3.2.2/maptasker/src/colrmode.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,59 +17,54 @@
 def set_color_mode(appearance_mode: str) -> dict:
     """
     Given the color mode to use (dark or light), set the colors appropriately
        :param appearance_mode: color mode: dark or light
        :return new colormap of colors to use in the output
     """
     # Deal with "System" color mode
-    if appearance_mode == "system":
-        mode = "dark" if darkdetect.isDark() else "light"
-    else:
-        mode = appearance_mode
+    mode = ("dark" if darkdetect.isDark() else "light") if appearance_mode == "system" else appearance_mode
 
     # Now set the colors to use based on the appearance mode
     if mode == "dark":
         return {
             "project_color": "White",
             "profile_color": "Aqua",
             "disabled_profile_color": "Red",
             "launcher_task_color": "GreenYellow",
             "task_color": "Yellow",
             "unknown_task_color": "Red",
             "scene_color": "Lime",
-            "bullet_color": "White",
             "action_name_color": "Gold",
             "action_color": "DarkOrange",
             "action_label_color": "Magenta",
             "action_condition_color": "PapayaWhip",
             "disabled_action_color": "Crimson",
             "profile_condition_color": "Lavender",
-            "background_color": "DarkBlue",
+            "background_color": "222623",
             "trailing_comments_color": "PeachPuff",
             "taskernet_color": "LightPink",
             "preferences_color": "PeachPuff",
             "highlight_color": "DarkTurquoise",
             "heading_color": "LimeGreen",
         }
-    else:
-        return {
-            "project_color": "Black",
-            "profile_color": "DarkBlue",
-            "disabled_profile_color": "DarkRed",
-            "launcher_task_color": "LawnGreen",
-            "task_color": "DarkGreen",
-            "unknown_task_color": "MediumVioletRed",
-            "scene_color": "Purple",
-            "bullet_color": "Black",
-            "action_color": "DarkSlateGray",
-            "action_name_color": "Indigo",
-            "action_label_color": "MediumOrchid",
-            "action_condition_color": "Brown",
-            "disabled_action_color": "IndianRed",
-            "profile_condition_color": "DarkSlateGray",
-            "background_color": "Lavender",
-            "trailing_comments_color": "Tomato",
-            "taskernet_color": "RoyalBlue",
-            "preferences_color": "DodgerBlue",
-            "highlight_color": "Yellow",
-            "heading_color": "DarkSlateGray",
-        }
+
+    return {
+        "project_color": "Black",
+        "profile_color": "DarkBlue",
+        "disabled_profile_color": "DarkRed",
+        "launcher_task_color": "LawnGreen",
+        "task_color": "DarkGreen",
+        "unknown_task_color": "MediumVioletRed",
+        "scene_color": "Purple",
+        "action_color": "DarkSlateGray",
+        "action_name_color": "Indigo",
+        "action_label_color": "MediumOrchid",
+        "action_condition_color": "Brown",
+        "disabled_action_color": "IndianRed",
+        "profile_condition_color": "DarkSlateGray",
+        "background_color": "Lavender",
+        "trailing_comments_color": "Tomato",
+        "taskernet_color": "RoyalBlue",
+        "preferences_color": "DodgerBlue",
+        "highlight_color": "Yellow",
+        "heading_color": "DarkSlateGray",
+    }
```

### Comparing `maptasker-2.6.3/maptasker/src/condition.py` & `maptasker-3.2.2/maptasker/src/condition.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Process profile condition: time, date, state, event, location, app"""
+
 #! /usr/bin/env python3
 # #################################################################################### #
 #                                                                                      #
 # condition: Process profile condition: time, date, state, event, location, app        #
 #                                                                                      #
 # GNU General Public License v3.0                                                      #
 # Permissions of this strong copyleft license are conditioned on making available      #
@@ -197,18 +199,15 @@
             be formatted
         :return: the formatted condition's output string
     """
     the_event_code = the_item.find("code")
 
     # Determine what the Event code is and return the actual Event text
     logger.debug(f"code:{the_event_code.text}")
-    if "e" not in the_event_code.text:
-        event_code = f"{the_event_code.text}e"
-    else:
-        event_code = the_event_code.text
+    event_code = f"{the_event_code.text}e" if "e" not in the_event_code.text else the_event_code.text
     if event_code not in action_codes:
         # Build new (template_ action code if not in our dictionary of codes yet
         process_action_codes.build_action_codes(the_event_code, the_item)  # Add it to our action dictionary
     # the_event_code.text = event_code
     event = action_evaluate.get_action_code(
         the_event_code,
         the_item,
@@ -253,15 +252,15 @@
             be formatted
         :return: the formatted condition's output string
     """
     lat = item.find("lat").text
     lon = item.find("long").text
     rad = item.find("rad").text
     if lat:
-        return f"{condition}Location with latitude {lat} longitude" f" {lon} radius {rad}"
+        return f"{condition}Location with latitude {lat} longitude {lon} radius {rad}"
     return ""
 
 
 # ##################################################################################
 # Given a Profile, return its list of conditions
 # ##################################################################################
 def parse_profile_condition(the_profile: defusedxml.ElementTree) -> str:
@@ -277,14 +276,16 @@
         "State": condition_state,
         "Event": condition_event,
         "App": condition_app,
         "Loc": condition_loc,
     }
     ignore_items = ["cdate", "edate", "flags", "id", "ProfileVariable"]
     condition = ""  # Assume no condition
+
+    # Go through Profile'x sub-XML looking for conditions
     for item in the_profile:
         if item.tag in ignore_items or "mid" in item.tag:  # Bypass junk we don't care about
             continue
         if condition:  # If we already have a condition, add 'and' (italicized)
             condition = f"{condition} <em>AND</em> "
 
         # Find out what the condition is and handle it.
```

### Comparing `maptasker-2.6.3/maptasker/src/config.py` & `maptasker-3.2.2/maptasker/src/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""User Modifiable Configutration File"""
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
 # config: Configuration file for MapTasker                                             #
 #                                                                                      #
 # GNU General Public License v3.0                                                      #
@@ -48,10 +49,14 @@
 ANDROID_PORT = ""
 
 # This is the location on the Android device from which to pull the backup file
 # Example: ANDROID_FILE = "/Tasker/configs/user/backup.xml"
 
 ANDROID_FILE = ""
 
+# This is used as the default display detail level.  It does not override the runtime option.
+# This value is used if the runtime option is not set.
+DEFAULT_DISPLAY_DETAIL_LEVEL = 5
+
 # ##################################################################################
 #  END User-modifiable global constants
 # ##################################################################################
```

### Comparing `maptasker-2.6.3/maptasker/src/debug.py` & `maptasker-3.2.2/maptasker/src/debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,8 +162,8 @@
         Args:
             condition_type (str): name of condition: Action, State, Event
             code (str): the xml code"""
     logger.debug(
         f"Error action code {code} not in the dictionary!",
     )
     if PrimeItems.program_arguments["debug"]:
-        print(f"{condition_type} code {code} not found in actionc!")  # noqa: T201
+        print(f"{condition_type} code {code} not found in actionc!")
```

### Comparing `maptasker-2.6.3/maptasker/src/diagram.py` & `maptasker-3.2.2/maptasker/src/diagram.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     print_3_lines,
     print_all,
     print_box,
     remove_icon,
 )
 from maptasker.src.getids import get_ids
 from maptasker.src.primitem import PrimeItems
-from maptasker.src.sysconst import MY_VERSION, FormatLine
+from maptasker.src.sysconst import MY_VERSION, NOW_TIME, FormatLine
 
 if TYPE_CHECKING:
     import defusedxml.ElementTree
 
 box_line = "═"
 blank = " "
 straight_line = "─"
@@ -55,15 +55,14 @@
 right_arrow_corner_down = "↘"
 right_arrow_corner_up = "↗"
 left_arrow_corner_down = "↙"
 left_arrow_corner_up = "↖"
 
 arrows = f"{down_arrow}{up_arrow}{left_arrow}{right_arrow}{right_arrow_corner_down}{right_arrow_corner_up}{left_arrow_corner_down}{left_arrow_corner_up}"
 directional_arrows = f"{right_arrow_corner_down}{right_arrow_corner_up}{left_arrow_corner_down}{left_arrow_corner_up}{up_arrow}{down_arrow}"
-all_special_characters = f"{arrows}│└"
 bar = "│"
 
 
 # ##################################################################################
 # Print the specific Task.
 # ##################################################################################
 def output_the_task(
@@ -466,14 +465,17 @@
         called_line_num,
         output_lines,
     )
 
     # If indice coming back is blank, then it wasn't found since it is named "Anonymous"
     if caller_line_index == "":
         return
+    # If called_line_index comes back as not found, we have a problem.
+    if called_line_index == "":
+        called_line_index = 1
 
     # Add up and down arrows to the connection points.
     add_down_and_up_arrows(
         caller_line_index,
         caller_line_num,
         caller_task_position,
         called_line_index,
@@ -790,19 +792,24 @@
 
     # Start with a ruler line
     PrimeItems.output_lines.add_line_to_output(1, "<hr>", FormatLine.dont_format_line)
 
     PrimeItems.netmap_output = []
 
     # Print a heading
+
     # datetime object containing current date and time
     now = datetime.now()  # noqa: DTZ005
 
     # dd/mm/YY H:M:S
     dt_string = now.strftime("%B %d, %Y  %H:%M:%S")
+
+    # dd/mm/YY H:M:S
+    dt_string = NOW_TIME.strftime("%B %d, %Y  %H:%M:%S")
+
     add_output_line(
         f"{MY_VERSION}{blank*5}Configuration Map{blank*5}{dt_string}",
     )
     add_output_line(" ")
     add_output_line(
         "Display with a monospaced font (e.g. Courier New) for accurate column alignment. And turn off line wrap.\nIcons in names can cause minor mis-alignment.",
     )
@@ -810,13 +817,13 @@
     add_output_line(" ")
 
     # Print the configuration
     build_network_map(network)
 
     # Print it all out.
     # Redirect print to a file
-    output_dir = f"{os.getcwd()}/MapTasker_Map.txt"  # Get the directory from which we are running.
+    output_dir = f"{os.getcwd()}{PrimeItems.slash}MapTasker_Map.txt"  # Get the directory from which we are running.
     with open(str(output_dir), "w", encoding="utf-8") as mapfile:
         # PrimeItems.printfile = mapfile
         for line in PrimeItems.netmap_output:
             # print(line, file=mapfile)
             mapfile.write(f"{line}\n")
```

### Comparing `maptasker-2.6.3/maptasker/src/diagutil.py` & `maptasker-3.2.2/maptasker/src/diagutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities used by diagram.py."""
+
 #! /usr/bin/env python3
 # #################################################################################### #
 #                                                                                      #
 # diagutil: Utilities used by diagram.py.                                              #
 #                                                                                      #
 # Traverse our network map and print out everything in connected boxes.                #
 #                                                                                      #
@@ -199,15 +200,15 @@
     - Return an empty string or a blank string trailer depending on if the icon is wider or taller
     """
     # We have at least one character that is probably an icon.
     for char in name:
         if char.strip() and set(char).difference(printable):
             # tkframe = PrimeItems.tkroot.frame()  # Initialize Tkinter
             # We have the icon.
-            char_dimension = width_and_height_calculator_in_pixel(char, "Courier New", 12)
+            char_dimension = width_and_height_calculator_in_pixel(char, "Courier", 12)
             trailer = "" if char_dimension[0] > char_dimension[1] else blank
             break
     return trailer
 
 
 # ##################################################################################
 # Remove a character from a string at a specific location and return the modified
@@ -348,17 +349,17 @@
     while check_line:
         with contextlib.suppress(IndexError):
             # Only insert bar if previous line character is a right arrow or two blanks.
             if output_lines[line_num][called_task_position] == right_arrow or (
                 output_lines[line_num][called_task_position] == " "
                 and output_lines[line_num][called_task_position - 1] == " "
             ):
-                output_lines[
-                    line_num
-                ] = f"{output_lines[line_num][:called_task_position]}{bar}{output_lines[line_num][called_task_position + 1:]}"
+                output_lines[line_num] = (
+                    f"{output_lines[line_num][:called_task_position]}{bar}{output_lines[line_num][called_task_position + 1:]}"
+                )
                 line_num -= 1
             else:
                 check_line = False
 
 
 # ##################################################################################
 # Go through output and delete all occurances of hanging bars |
@@ -381,17 +382,17 @@
 
     while line_num > 0:
         indices = [i.start() for i in re.finditer(bar, output_lines[line_num])]
 
         # Go through list of bar positions in line.
         for position_bar in indices:
             if len(output_lines[line_num + 1]) < position_bar or output_lines[line_num + 1][position_bar] == " ":
-                output_lines[
-                    line_num
-                ] = f"{output_lines[line_num][:position_bar]} {output_lines[line_num][position_bar + 1:]}"
+                output_lines[line_num] = (
+                    f"{output_lines[line_num][:position_bar]} {output_lines[line_num][position_bar + 1:]}"
+                )
 
         # Now let's make sure there is a bar connecting right down arrow to Task.
         # Add bar(s) (|) above right-down arrow as necessary.
         arrow_position = output_lines[line_num].find(right_arrow_corner_down)
         if arrow_position != -1:
             add_bar_above_lines(output_lines, line_num, arrow_position)
 
@@ -623,15 +624,23 @@
 
         #  Find the "Called" Task line for the caller Task.
         search_name = f"└─ {called_task_name}"
 
         # Make sure the called Task exists.
         found_called_task = False
         for called_line_num, check_line in enumerate(output_lines):
+            # See if the task name is in the line
             if search_name in check_line:
+                # Make certain that this is the exact string we want and not a substr match.
+                # If search_name as a substr of the task name we are looking for, then erroneously gets a match and we
+                # must continue the search!
+                str_pos = check_line.find(search_name)
+                bracket = check_line[str_pos + len(search_name) + 1]
+                if bracket != "[":  # If not a bracket, then it is a substring of a larger task name.
+                    continue
                 found_called_task = True
                 # Find the position of the "Calls -->" task name on the called line
                 caller_task_position = output_lines[called_line_num].index(called_task_name) + (
                     len(called_task_name) // 2
                 )
                 # Find the position of the "Called by" task name on the caller by line
                 called_task_position = output_lines[caller_line_num].index(called_task_name) + (
```

### Comparing `maptasker-2.6.3/maptasker/src/dirout.py` & `maptasker-3.2.2/maptasker/src/dirout.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #                                                                                      #
 # #################################################################################### #
 import math
 
 import darkdetect
 
 from maptasker.src.primitem import PrimeItems
-from maptasker.src.sysconst import NO_PROFILE, FormatLine
+from maptasker.src.sysconst import NO_PROFILE, NORMAL_TAB, TABLE_BACKGROUND_COLOR, TABLE_BORDER, FormatLine
 from maptasker.src.xmldata import find_task_by_name
 
 period = "."
 
 
 # ##################################################################################
 # Search a list of lists for a given string.  Return True if found.
@@ -144,45 +144,25 @@
     Returns:
         str: The generated HTML table.
 
     Example:
         ```python
         data = {
             "header": ["Name", "Age", "City"],
-            "rows": [
-                ["John Doe", 25, "New York"],
-                ["Jane Smith", 30, "Los Angeles"],
-                ["Mike Johnson", 35, "Chicago"]
-            ]
+            "rows": [["John Doe", 25, "New York"], ["Jane Smith", 30, "Los Angeles"], ["Mike Johnson", 35, "Chicago"]],
         }
 
         html_table = generate_html_table(data)
         print(html_table)
         ```
     """
-    # Set up background color
-    color_to_use = "LightSteelBlue" if darkdetect.isDark() else "DarkTurquoise"
-    border = (
-        "\n"
-        "<style> \
-            table, \
-            td, \
-            th { \
-            padding: 5px; \
-            border: 2px solid #1c87c9; \
-            border-radius: 3px; \
-            background-color: #128198; \
-            text-align: center; \
-            } \
-        </style>"
-    )
 
     # Set up the variables
-    html = f'{border}<table style="width:100%;text-align:left;background-color:\
-    {color_to_use};">\n'
+    html = f'{TABLE_BORDER}<table style="width:100%;margin-left: 20;text-align:left;background-color:\
+    {TABLE_BACKGROUND_COLOR};">\n'
     index = 0
     data.sort()  # Sort the directory by name
 
     # Build our table
     for _ in range(rows):
         html += "  <tr> \n"
         for _ in range(columns):
@@ -209,15 +189,15 @@
 
     Returns:
         None
     """
     trailing_matter = []
     PrimeItems.output_lines.add_line_to_output(
         5,
-        f"<br><br>Trailing Information{period*50}<br><br>",
+        f"<br><br>{NORMAL_TAB}Trailing Information{period*50}<br><br>",
         ["", "project_color", FormatLine.add_end_span],
     )
 
     # Do the Configuration Variables
     if PrimeItems.program_arguments["display_detail_level"] == 4:
         trailing_matter.append("<a href=#unreferenced_variables>Unreferenced Global Variables</a>")
 
@@ -264,15 +244,15 @@
 # ##################################################################################
 def check_scene(item: str) -> bool:
     """
     Check to make sure this Scene should be included in the output
         Args:
             item (str): directory hyperlink item we are processing
 
-        Returns:
+        Returns:20.
             bool: True if we should output this hperlink, False if it is to be ingored.
     """
     # Single Project?
     if PrimeItems.program_arguments["single_project_name"]:
         found, project = find_task_in_project("", item[1], "scenes")
         return found
 
@@ -449,15 +429,15 @@
                 # Append our hyperlink to this Project to the list
                 directory_hyperlinks.append(f"<a href=#{name}_{hyperlink_name}>{display_name}</a>")
 
         if directory_hyperlinks:
             # Output the name title: Project, Profile, Task, Scene
             PrimeItems.output_lines.add_line_to_output(
                 5,
-                f"{name.capitalize()}{period*60}<br><br>",
+                f"{NORMAL_TAB}{name.capitalize()}{period*60}<br><br>",
                 ["<br><br>", "project_color", FormatLine.add_end_span],
             )
             # 6 columns for projects, 5 columns for tasks
             number_of_columns = 5 if name == "tasks" else 6
             output_table(directory_hyperlinks, number_of_columns)
 
 
@@ -474,15 +454,15 @@
     Returns:
         None
     """
 
     # Add heading
     PrimeItems.output_lines.add_line_to_output(
         5,
-        "<h2>Directory</h2><br><br>",
+        f"<h2>{NORMAL_TAB}Directory</h2><br><br>",
         ["<br><br>", "profile_color", FormatLine.add_end_span],
     )
     # Ok, run through the Tasker key elements and output the directory for each
     # Only do Projects and Profiles if not looking for a single Project or Profile
     if not (PrimeItems.program_arguments["single_profile_name"] or PrimeItems.program_arguments["single_task_name"]):
         do_tasker_element("projects")
     do_tasker_element("profiles")
```

### Comparing `maptasker-2.6.3/maptasker/src/error.py` & `maptasker-3.2.2/maptasker/src/error.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,25 +31,29 @@
     elif exit_code > 100:
         final_error_message = f"{Colors.Yellow}{error_message}"
     else:
         final_error_message = f"{Colors.Red}MapTasker error: {error_message}"
 
     # Process an error?
     if exit_code > 0:
-        logger.critical(final_error_message)
-        if PrimeItems.program_arguments and PrimeItems.program_arguments["debug"]:
-            print(final_error_message)  # noqa: T201
+        logger.debug(final_error_message)
+        if (
+            PrimeItems.program_arguments
+            and PrimeItems.program_arguments["debug"]
+            and not PrimeItems.program_arguments["gui"]
+        ):
+            print(final_error_message)
 
         # If coming from GUI, set error info. and return to GUI.
         if PrimeItems.program_arguments and PrimeItems.program_arguments["gui"]:
             PrimeItems.error_code = exit_code
             PrimeItems.error_msg = error_message
             return
         # Not coming from GUI...just print error.
-        print(final_error_message)  # noqa: T201
+        print(final_error_message)
         sys.exit(exit_code)
 
     # return code 0
     else:
-        print(final_error_message)  # noqa: T201
+        print(final_error_message)
         logger.info(final_error_message)
         return
```

### Comparing `maptasker-2.6.3/maptasker/src/fonts.py` & `maptasker-3.2.2/maptasker/src/fonts.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,24 +34,24 @@
     our_font = PrimeItems.program_arguments["font"]
 
     # Set up our list of fonts, including Courier
     mono_fonts = ["Courier"]
 
     # If the font requested is 'help', then just display the fonts and exit
     if our_font == "help":
-        print("Valid monospace fonts...")  # noqa: T201
-        print('  "Courier" is the default')  # noqa: T201
+        print("Valid monospace fonts...")
+        print('  "Courier" is the default')
 
     # Go thru list of fonts from tkinter
     PrimeItems.mono_fonts = {}
     for f in fonts:
         # Monospace only
         if f.metrics("fixed") and "Wingding" not in f.actual("family"):
             if our_font == "help":
-                print(f'  "{f.actual("family")}"')  # noqa: T201
+                print(f'  "{f.actual("family")}"')
             elif save_fonts:
                 PrimeItems.mono_fonts[f.name] = f.actual("family")
             mono_fonts.append(f.actual("family"))
     if our_font == "help":
         sys.exit(0)
 
     del fonts
```

### Comparing `maptasker-2.6.3/maptasker/src/frontmtr.py` & `maptasker-3.2.2/maptasker/src/frontmtr.py`

 * *Files 13% similar despite different names*

```diff
@@ -55,289 +55,301 @@
 00000360: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000370: 2020 2020 2020 2020 230a 2320 2323 2323          #.# ####
 00000380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00000390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000003a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000003b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000003c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000003d0: 2023 0a66 726f 6d20 6461 7465 7469 6d65   #.from datetime
-000003e0: 2069 6d70 6f72 7420 6461 7465 7469 6d65   import datetime
-000003f0: 0a0a 6672 6f6d 206d 6170 7461 736b 6572  ..from maptasker
-00000400: 2e73 7263 2e61 6464 6373 7320 696d 706f  .src.addcss impo
-00000410: 7274 2061 6464 5f63 7373 0a66 726f 6d20  rt add_css.from 
-00000420: 6d61 7074 6173 6b65 722e 7372 632e 6465  maptasker.src.de
-00000430: 6275 6720 696d 706f 7274 2064 6973 706c  bug import displ
-00000440: 6179 5f64 6562 7567 5f69 6e66 6f0a 6672  ay_debug_info.fr
-00000450: 6f6d 206d 6170 7461 736b 6572 2e73 7263  om maptasker.src
-00000460: 2e66 6f72 6d61 7420 696d 706f 7274 2066  .format import f
-00000470: 6f72 6d61 745f 6874 6d6c 0a66 726f 6d20  ormat_html.from 
-00000480: 6d61 7074 6173 6b65 722e 7372 632e 7072  maptasker.src.pr
-00000490: 6566 6572 7320 696d 706f 7274 2067 6574  efers import get
-000004a0: 5f70 7265 6665 7265 6e63 6573 0a66 726f  _preferences.fro
-000004b0: 6d20 6d61 7074 6173 6b65 722e 7372 632e  m maptasker.src.
-000004c0: 7072 696d 6974 656d 2069 6d70 6f72 7420  primitem import 
-000004d0: 5072 696d 6549 7465 6d73 0a66 726f 6d20  PrimeItems.from 
-000004e0: 6d61 7074 6173 6b65 722e 7372 632e 7379  maptasker.src.sy
-000004f0: 7363 6f6e 7374 2069 6d70 6f72 7420 4d59  sconst import MY
-00000500: 5f56 4552 5349 4f4e 2c20 466f 726d 6174  _VERSION, Format
-00000510: 4c69 6e65 0a0a 0a23 2023 2323 2323 2323  Line...# #######
+000003d0: 2023 0a0a 6672 6f6d 206d 6170 7461 736b   #..from maptask
+000003e0: 6572 2e73 7263 2e61 6464 6373 7320 696d  er.src.addcss im
+000003f0: 706f 7274 2061 6464 5f63 7373 0a66 726f  port add_css.fro
+00000400: 6d20 6d61 7074 6173 6b65 722e 7372 632e  m maptasker.src.
+00000410: 6465 6275 6720 696d 706f 7274 2064 6973  debug import dis
+00000420: 706c 6179 5f64 6562 7567 5f69 6e66 6f0a  play_debug_info.
+00000430: 6672 6f6d 206d 6170 7461 736b 6572 2e73  from maptasker.s
+00000440: 7263 2e66 6f72 6d61 7420 696d 706f 7274  rc.format import
+00000450: 2066 6f72 6d61 745f 6874 6d6c 0a66 726f   format_html.fro
+00000460: 6d20 6d61 7074 6173 6b65 722e 7372 632e  m maptasker.src.
+00000470: 7072 6566 6572 7320 696d 706f 7274 2067  prefers import g
+00000480: 6574 5f70 7265 6665 7265 6e63 6573 0a66  et_preferences.f
+00000490: 726f 6d20 6d61 7074 6173 6b65 722e 7372  rom maptasker.sr
+000004a0: 632e 7072 696d 6974 656d 2069 6d70 6f72  c.primitem impor
+000004b0: 7420 5072 696d 6549 7465 6d73 0a66 726f  t PrimeItems.fro
+000004c0: 6d20 6d61 7074 6173 6b65 722e 7372 632e  m maptasker.src.
+000004d0: 7379 7363 6f6e 7374 2069 6d70 6f72 7420  sysconst import 
+000004e0: 4d59 5f56 4552 5349 4f4e 2c20 4e4f 524d  MY_VERSION, NORM
+000004f0: 414c 5f54 4142 2c20 4e4f 575f 5449 4d45  AL_TAB, NOW_TIME
+00000500: 2c20 466f 726d 6174 4c69 6e65 0a0a 0a23  , FormatLine...#
+00000510: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
 00000520: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00000530: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00000540: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00000550: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000560: 2323 2323 2323 2323 2323 230a 2320 4164  ###########.# Ad
-00000570: 6420 7468 6520 6865 6164 696e 6720 6d61  d the heading ma
-00000580: 7474 6572 2074 6f20 7468 6520 6f75 7470  tter to the outp
-00000590: 7574 3a20 6865 6164 696e 672c 2073 6f75  ut: heading, sou
-000005a0: 7263 652c 2073 6372 6565 6e20 7369 7a65  rce, screen size
-000005b0: 2c20 6574 632e 0a23 2023 2323 2323 2323  , etc..# #######
+00000560: 2323 230a 2320 4164 6420 7468 6520 6865  ###.# Add the he
+00000570: 6164 696e 6720 6d61 7474 6572 2074 6f20  ading matter to 
+00000580: 7468 6520 6f75 7470 7574 3a20 6865 6164  the output: head
+00000590: 696e 672c 2073 6f75 7263 652c 2073 6372  ing, source, scr
+000005a0: 6565 6e20 7369 7a65 2c20 6574 632e 0a23  een size, etc..#
+000005b0: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
 000005c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000005d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000005e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000005f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000600: 2323 2323 2323 2323 2323 230a 6465 6620  ###########.def 
-00000610: 6f75 7470 7574 5f74 6865 5f68 6561 6469  output_the_headi
-00000620: 6e67 2829 202d 3e20 4e6f 6e65 3a0a 2020  ng() -> None:.  
-00000630: 2020 2222 220a 2020 2020 4469 7370 6c61    """.    Displa
-00000640: 7920 7468 6520 6865 6164 696e 6720 616e  y the heading an
-00000650: 6420 736f 7572 6365 2066 696c 6520 6465  d source file de
-00000660: 7461 696c 730a 2020 2020 2222 220a 0a20  tails.    """.. 
-00000670: 2020 2023 2053 7461 7274 206f 7574 2062     # Start out b
-00000680: 7920 6f75 7470 7574 7469 6e67 206f 7572  y outputting our
-00000690: 2063 6f6c 6f72 7320 616e 6420 666f 6e74   colors and font
-000006a0: 2043 5353 0a20 2020 2061 6464 5f63 7373   CSS.    add_css
-000006b0: 2829 0a0a 2020 2020 7461 736b 6572 5f6d  ()..    tasker_m
-000006c0: 6170 7069 6e67 203d 2022 5461 736b 6572  apping = "Tasker
-000006d0: 204d 6170 7069 6e67 2e2e 2e2e 2e2e 2e2e   Mapping........
-000006e0: 2e2e 2e2e 2e2e 2e2e 2054 6173 6b65 7220  ........ Tasker 
-000006f0: 7665 7273 696f 6e3a 220a 0a20 2020 2023  version:"..    #
-00000700: 2047 6574 2074 6865 2073 6372 6565 6e20   Get the screen 
-00000710: 6469 6d65 6e73 696f 6e73 2066 726f 6d20  dimensions from 
-00000720: 3c64 6d65 7472 6963 3e20 786d 6c0a 2020  <dmetric> xml.  
-00000730: 2020 7363 7265 656e 5f65 6c65 6d65 6e74    screen_element
-00000740: 203d 2050 7269 6d65 4974 656d 732e 786d   = PrimeItems.xm
-00000750: 6c5f 726f 6f74 2e66 696e 6428 2264 6d65  l_root.find("dme
-00000760: 7472 6963 2229 0a20 2020 2073 6372 6565  tric").    scree
-00000770: 6e5f 7369 7a65 203d 2028 0a20 2020 2020  n_size = (.     
-00000780: 2020 2066 2726 6e62 7370 3b26 6e62 7370     f'&nbsp;&nbsp
-00000790: 3b44 6576 6963 6520 7363 7265 656e 2073  ;Device screen s
-000007a0: 697a 653a 207b 7363 7265 656e 5f65 6c65  ize: {screen_ele
-000007b0: 6d65 6e74 2e74 6578 742e 7265 706c 6163  ment.text.replac
-000007c0: 6528 222c 222c 2022 2058 2022 297d 270a  e(",", " X ")}'.
-000007d0: 2020 2020 2020 2020 6966 2073 6372 6565          if scree
-000007e0: 6e5f 656c 656d 656e 7420 6973 206e 6f74  n_element is not
-000007f0: 204e 6f6e 650a 2020 2020 2020 2020 656c   None.        el
-00000800: 7365 2022 220a 2020 2020 290a 0a20 2020  se "".    )..   
-00000810: 2023 2053 6574 2075 7020 6869 6768 6c69   # Set up highli
-00000820: 6768 7420 6261 636b 6772 6f75 6e64 2063  ght background c
-00000830: 6f6c 6f72 2069 6620 6e65 6564 6564 0a20  olor if needed. 
-00000840: 2020 2069 6620 5072 696d 6549 7465 6d73     if PrimeItems
-00000850: 2e70 726f 6772 616d 5f61 7267 756d 656e  .program_argumen
-00000860: 7473 5b22 6869 6768 6c69 6768 7422 5d3a  ts["highlight"]:
-00000870: 0a20 2020 2020 2020 2062 6163 6b67 726f  .        backgro
-00000880: 756e 645f 636f 6c6f 725f 6874 6d6c 203d  und_color_html =
-00000890: 2028 0a20 2020 2020 2020 2020 2020 2022   (.            "
-000008a0: 3c73 7479 6c65 3e5c 6e6d 6172 6b20 7b20  <style>\nmark { 
-000008b0: 5c6e 6261 636b 6772 6f75 6e64 2d63 6f6c  \nbackground-col
-000008c0: 6f72 3a20 2220 2b20 5072 696d 6549 7465  or: " + PrimeIte
-000008d0: 6d73 2e63 6f6c 6f72 735f 746f 5f75 7365  ms.colors_to_use
-000008e0: 5b22 6869 6768 6c69 6768 745f 636f 6c6f  ["highlight_colo
-000008f0: 7222 5d20 2b20 223b 5c6e 7d5c 6e3c 2f73  r"] + ";\n}\n</s
-00000900: 7479 6c65 3e5c 6e22 0a20 2020 2020 2020  tyle>\n".       
-00000910: 2029 0a20 2020 2065 6c73 653a 0a20 2020   ).    else:.   
-00000920: 2020 2020 2062 6163 6b67 726f 756e 645f       background_
-00000930: 636f 6c6f 725f 6874 6d6c 203d 2022 220a  color_html = "".
-00000940: 0a20 2020 2023 204f 7574 7075 7420 6461  .    # Output da
-00000950: 7465 2061 6e64 2074 696d 6520 6966 2069  te and time if i
-00000960: 6e20 6465 6275 6720 6d6f 6465 0a20 2020  n debug mode.   
-00000970: 2069 6620 5072 696d 6549 7465 6d73 2e70   if PrimeItems.p
-00000980: 726f 6772 616d 5f61 7267 756d 656e 7473  rogram_arguments
-00000990: 5b22 6465 6275 6722 5d3a 0a20 2020 2020  ["debug"]:.     
-000009a0: 2020 206e 6f77 203d 2064 6174 6574 696d     now = datetim
-000009b0: 652e 6e6f 7728 290a 2020 2020 2020 2020  e.now().        
-000009c0: 6e6f 775f 666f 725f 6f75 7470 7574 203d  now_for_output =
-000009d0: 206e 6f77 2e73 7472 6674 696d 6528 2225   now.strftime("%
-000009e0: 6d2f 2564 2f25 7920 2548 3a25 4d3a 2553  m/%d/%y %H:%M:%S
-000009f0: 2229 0a20 2020 2065 6c73 653a 0a20 2020  ").    else:.   
-00000a00: 2020 2020 206e 6f77 5f66 6f72 5f6f 7574       now_for_out
-00000a10: 7075 7420 3d20 2222 0a0a 2020 2020 2320  put = ""..    # 
-00000a20: 466f 726d 6174 2074 6865 206f 7574 7075  Format the outpu
-00000a30: 7420 6865 6164 696e 670a 2020 2020 6865  t heading.    he
-00000a40: 6164 696e 675f 636f 6c6f 7220 3d20 2268  ading_color = "h
-00000a50: 6561 6469 6e67 5f63 6f6c 6f72 220a 2020  eading_color".  
-00000a60: 2020 5072 696d 6549 7465 6d73 2e68 6561    PrimeItems.hea
-00000a70: 6469 6e67 203d 2028 0a20 2020 2020 2020  ding = (.       
-00000a80: 2066 223c 2164 6f63 7479 7065 2068 746d   f"<!doctype htm
-00000a90: 6c3e 5c6e 3c68 746d 6c20 6c61 6e67 3de2  l>\n<html lang=.
-00000aa0: 809d 656e e280 9d3e 5c6e 3c68 6561 643e  ..en...>\n<head>
-00000ab0: 5c6e 7b62 6163 6b67 726f 756e 645f 636f  \n{background_co
-00000ac0: 6c6f 725f 6874 6d6c 7d3c 7469 746c 653e  lor_html}<title>
-00000ad0: 4d61 7054 6173 6b65 723c 2f74 6974 6c65  MapTasker</title
-00000ae0: 3e5c 6e3c 626f 6479 220a 2020 2020 2020  >\n<body".      
-00000af0: 2020 6622 2073 7479 6c65 3d5c 2262 6163    f" style=\"bac
-00000b00: 6b67 726f 756e 642d 636f 6c6f 723a 7b50  kground-color:{P
-00000b10: 7269 6d65 4974 656d 732e 636f 6c6f 7273  rimeItems.colors
-00000b20: 5f74 6f5f 7573 655b 2762 6163 6b67 726f  _to_use['backgro
-00000b30: 756e 645f 636f 6c6f 7227 5d7d 5c22 3e5c  und_color']}\">\
-00000b40: 6e22 0a20 2020 2020 2020 202b 2066 6f72  n".        + for
-00000b50: 6d61 745f 6874 6d6c 280a 2020 2020 2020  mat_html(.      
-00000b60: 2020 2020 2020 6865 6164 696e 675f 636f        heading_co
-00000b70: 6c6f 722c 0a20 2020 2020 2020 2020 2020  lor,.           
-00000b80: 2022 222c 0a20 2020 2020 2020 2020 2020   "",.           
-00000b90: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-00000ba0: 2020 2066 223c 6832 3e4d 6170 5461 736b     f"<h2>MapTask
-00000bb0: 6572 3c2f 6832 3e3c 6272 3e20 7b74 6173  er</h2><br> {tas
-00000bc0: 6b65 725f 6d61 7070 696e 677d 220a 2020  ker_mapping}".  
-00000bd0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-00000be0: 207b 5072 696d 6549 7465 6d73 2e78 6d6c   {PrimeItems.xml
-00000bf0: 5f72 6f6f 742e 6174 7472 6962 5b27 7476  _root.attrib['tv
-00000c00: 275d 7d26 6e62 7370 3b26 6e62 7370 3b26  ']}&nbsp;&nbsp;&
-00000c10: 6e62 7370 3b26 6e62 7370 3b22 0a20 2020  nbsp;&nbsp;".   
-00000c20: 2020 2020 2020 2020 2020 2020 2066 227b               f"{
-00000c30: 4d59 5f56 4552 5349 4f4e 7d7b 7363 7265  MY_VERSION}{scre
-00000c40: 656e 5f73 697a 657d 266e 6273 703b 266e  en_size}&nbsp;&n
-00000c50: 6273 703b 266e 6273 703b 266e 6273 703b  bsp;&nbsp;&nbsp;
-00000c60: 7b6e 6f77 5f66 6f72 5f6f 7574 7075 747d  {now_for_output}
-00000c70: 220a 2020 2020 2020 2020 2020 2020 292c  ".            ),
-00000c80: 0a20 2020 2020 2020 2020 2020 2054 7275  .            Tru
-00000c90: 652c 0a20 2020 2020 2020 2029 0a20 2020  e,.        ).   
-00000ca0: 2029 0a0a 2020 2020 5072 696d 6549 7465   )..    PrimeIte
-00000cb0: 6d73 2e6f 7574 7075 745f 6c69 6e65 732e  ms.output_lines.
-00000cc0: 6164 645f 6c69 6e65 5f74 6f5f 6f75 7470  add_line_to_outp
-00000cd0: 7574 280a 2020 2020 2020 2020 302c 0a20  ut(.        0,. 
-00000ce0: 2020 2020 2020 2050 7269 6d65 4974 656d         PrimeItem
-00000cf0: 732e 6865 6164 696e 672c 0a20 2020 2020  s.heading,.     
-00000d00: 2020 2046 6f72 6d61 744c 696e 652e 646f     FormatLine.do
-00000d10: 6e74 5f66 6f72 6d61 745f 6c69 6e65 2c0a  nt_format_line,.
-00000d20: 2020 2020 290a 0a20 2020 2023 2044 6973      )..    # Dis
-00000d30: 706c 6179 2077 6865 7265 2074 6865 2073  play where the s
-00000d40: 6f75 7263 6520 6669 6c65 2063 616d 6520  ource file came 
-00000d50: 6672 6f6d 0a20 2020 2023 2044 6964 2077  from.    # Did w
-00000d60: 6520 7265 7374 6f72 6520 7468 6520 6261  e restore the ba
-00000d70: 636b 7570 2066 726f 6d20 416e 6472 6f69  ckup from Androi
-00000d80: 643f 0a20 2020 2069 6620 5072 696d 6549  d?.    if PrimeI
-00000d90: 7465 6d73 2e70 726f 6772 616d 5f61 7267  tems.program_arg
-00000da0: 756d 656e 7473 5b22 6665 7463 6865 645f  uments["fetched_
-00000db0: 6261 636b 7570 5f66 726f 6d5f 616e 6472  backup_from_andr
-00000dc0: 6f69 6422 5d3a 0a20 2020 2020 2020 2073  oid"]:.        s
-00000dd0: 6f75 7263 655f 6669 6c65 203d 2028 0a20  ource_file = (. 
-00000de0: 2020 2020 2020 2020 2020 2022 4672 6f6d             "From
-00000df0: 2041 6e64 726f 6964 2064 6576 6963 6522   Android device"
-00000e00: 0a20 2020 2020 2020 2020 2020 2066 2720  .            f' 
-00000e10: 5443 5020 4950 2061 6464 7265 7373 3a7b  TCP IP address:{
-00000e20: 5072 696d 6549 7465 6d73 2e70 726f 6772  PrimeItems.progr
-00000e30: 616d 5f61 7267 756d 656e 7473 5b22 616e  am_arguments["an
-00000e40: 6472 6f69 645f 6970 6164 6472 225d 7d27  droid_ipaddr"]}'
-00000e50: 0a20 2020 2020 2020 2020 2020 2066 2720  .            f' 
-00000e60: 6f6e 2070 6f72 743a 7b50 7269 6d65 4974  on port:{PrimeIt
-00000e70: 656d 732e 7072 6f67 7261 6d5f 6172 6775  ems.program_argu
-00000e80: 6d65 6e74 735b 2261 6e64 726f 6964 5f70  ments["android_p
-00000e90: 6f72 7422 5d7d 270a 2020 2020 2020 2020  ort"]}'.        
-00000ea0: 2020 2020 6627 2077 6974 6820 6669 6c65      f' with file
-00000eb0: 206c 6f63 6174 696f 6e3a 207b 5072 696d   location: {Prim
-00000ec0: 6549 7465 6d73 2e70 726f 6772 616d 5f61  eItems.program_a
-00000ed0: 7267 756d 656e 7473 5b22 616e 6472 6f69  rguments["androi
-00000ee0: 645f 6669 6c65 225d 7d27 0a20 2020 2020  d_file"]}'.     
-00000ef0: 2020 2029 0a20 2020 2065 6c69 6620 5072     ).    elif Pr
-00000f00: 696d 6549 7465 6d73 2e70 726f 6772 616d  imeItems.program
-00000f10: 5f61 7267 756d 656e 7473 5b22 6465 6275  _arguments["debu
-00000f20: 6722 5d20 6f72 206e 6f74 2050 7269 6d65  g"] or not Prime
-00000f30: 4974 656d 732e 7072 6f67 7261 6d5f 6172  Items.program_ar
-00000f40: 6775 6d65 6e74 735b 2266 696c 6522 5d3a  guments["file"]:
-00000f50: 0a20 2020 2020 2020 2066 696c 656e 616d  .        filenam
-00000f60: 6520 3d20 6973 696e 7374 616e 6365 2850  e = isinstance(P
-00000f70: 7269 6d65 4974 656d 732e 6669 6c65 5f74  rimeItems.file_t
-00000f80: 6f5f 6765 742c 2073 7472 290a 2020 2020  o_get, str).    
-00000f90: 2020 2020 6669 6c65 6e61 6d65 203d 2050      filename = P
-00000fa0: 7269 6d65 4974 656d 732e 6669 6c65 5f74  rimeItems.file_t
-00000fb0: 6f5f 6765 742e 6e61 6d65 2069 6620 6e6f  o_get.name if no
-00000fc0: 7420 6669 6c65 6e61 6d65 2065 6c73 6520  t filename else 
-00000fd0: 5072 696d 6549 7465 6d73 2e66 696c 655f  PrimeItems.file_
-00000fe0: 746f 5f67 6574 0a20 2020 2020 2020 2073  to_get.        s
-00000ff0: 6f75 7263 655f 6669 6c65 203d 2066 696c  ource_file = fil
-00001000: 656e 616d 650a 2020 2020 656c 7365 3a0a  ename.    else:.
-00001010: 2020 2020 2020 2020 736f 7572 6365 5f66          source_f
-00001020: 696c 6520 3d20 5072 696d 6549 7465 6d73  ile = PrimeItems
-00001030: 2e70 726f 6772 616d 5f61 7267 756d 656e  .program_argumen
-00001040: 7473 5b22 6669 6c65 225d 0a20 2020 2023  ts["file"].    #
-00001050: 2041 6464 2073 6f75 7263 6520 746f 206f   Add source to o
-00001060: 7574 7075 740a 2020 2020 5072 696d 6549  utput.    PrimeI
-00001070: 7465 6d73 2e6f 7574 7075 745f 6c69 6e65  tems.output_line
-00001080: 732e 6164 645f 6c69 6e65 5f74 6f5f 6f75  s.add_line_to_ou
-00001090: 7470 7574 280a 2020 2020 2020 2020 302c  tput(.        0,
-000010a0: 0a20 2020 2020 2020 2066 223c 6272 3e3c  .        f"<br><
-000010b0: 6272 3e53 6f75 7263 6520 6261 636b 7570  br>Source backup
-000010c0: 2066 696c 653a 207b 736f 7572 6365 5f66   file: {source_f
-000010d0: 696c 657d 222c 0a20 2020 2020 2020 205b  ile}",.        [
-000010e0: 2222 2c20 2268 6561 6469 6e67 5f63 6f6c  "", "heading_col
-000010f0: 6f72 222c 2046 6f72 6d61 744c 696e 652e  or", FormatLine.
-00001100: 6164 645f 656e 645f 7370 616e 5d2c 0a20  add_end_span],. 
-00001110: 2020 2029 0a0a 0a23 2023 2323 2323 2323     )...# #######
-00001120: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001130: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001140: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001150: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001160: 2323 2323 2323 2323 2323 230a 2320 4f75  ###########.# Ou
-00001170: 7470 7574 2074 6865 2068 6561 6469 6e67  tput the heading
-00001180: 2065 7463 2e20 6173 2074 6865 2066 726f   etc. as the fro
-00001190: 6e74 206d 6174 7465 722e 0a23 2023 2323  nt matter..# ###
-000011a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000011b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000011c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000011d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000011e0: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
-000011f0: 6465 6620 6f75 7470 7574 5f74 6865 5f66  def output_the_f
-00001200: 726f 6e74 5f6d 6174 7465 7228 2920 2d3e  ront_matter() ->
-00001210: 204e 6f6e 653a 0a20 2020 2022 2222 0a20   None:.    """. 
-00001220: 2020 2047 656e 6572 6174 6573 2074 6865     Generates the
-00001230: 2066 726f 6e74 206d 6174 7465 7220 666f   front matter fo
-00001240: 7220 7468 6520 6f75 7470 7574 2066 696c  r the output fil
-00001250: 653a 2068 6561 6469 6e67 2c20 7275 6e74  e: heading, runt
-00001260: 696d 6520 7365 7474 696e 6773 2c0a 2020  ime settings,.  
-00001270: 2020 6469 7265 6374 6f72 792c 2054 6173    directory, Tas
-00001280: 6b65 7220 7072 6566 6572 656e 6365 732e  ker preferences.
-00001290: 0a20 2020 2022 2222 0a0a 2020 2020 2320  .    """..    # 
-000012a0: 4865 6164 696e 6720 696e 666f 726d 6174  Heading informat
-000012b0: 696f 6e0a 2020 2020 6f75 7470 7574 5f74  ion.    output_t
-000012c0: 6865 5f68 6561 6469 6e67 2829 0a0a 2020  he_heading()..  
-000012d0: 2020 2320 4966 2077 6520 6172 6520 6465    # If we are de
-000012e0: 6275 6767 696e 672c 206f 7574 7075 7420  bugging, output 
-000012f0: 7468 6520 7275 6e74 696d 6520 6172 6775  the runtime argu
-00001300: 6d65 6e74 7320 616e 6420 636f 6c6f 7273  ments and colors
-00001310: 0a20 2020 2069 6620 5072 696d 6549 7465  .    if PrimeIte
-00001320: 6d73 2e70 726f 6772 616d 5f61 7267 756d  ms.program_argum
-00001330: 656e 7473 5b22 6465 6275 6722 5d20 6f72  ents["debug"] or
-00001340: 2050 7269 6d65 4974 656d 732e 7072 6f67   PrimeItems.prog
-00001350: 7261 6d5f 6172 6775 6d65 6e74 735b 2272  ram_arguments["r
-00001360: 756e 7469 6d65 225d 3a0a 2020 2020 2020  untime"]:.      
-00001370: 2020 6469 7370 6c61 795f 6465 6275 675f    display_debug_
-00001380: 696e 666f 2829 0a0a 2020 2020 2320 5374  info()..    # St
-00001390: 6172 7420 6120 6c69 7374 2028 3c75 6c3e  art a list (<ul>
-000013a0: 2920 746f 2066 6f72 6365 2065 7665 7279  ) to force every
-000013b0: 7468 696e 6720 746f 2074 6162 206f 7665  thing to tab ove
-000013c0: 720a 2020 2020 2320 5072 696d 6549 7465  r.    # PrimeIte
-000013d0: 6d73 2e75 6e6f 7264 6572 6564 5f6c 6973  ms.unordered_lis
-000013e0: 745f 636f 756e 7422 5d20 3d20 300a 2020  t_count"] = 0.  
-000013f0: 2020 5072 696d 6549 7465 6d73 2e6f 7574    PrimeItems.out
-00001400: 7075 745f 6c69 6e65 732e 6164 645f 6c69  put_lines.add_li
-00001410: 6e65 5f74 6f5f 6f75 7470 7574 2831 2c20  ne_to_output(1, 
-00001420: 2222 2c20 466f 726d 6174 4c69 6e65 2e64  "", FormatLine.d
-00001430: 6f6e 745f 666f 726d 6174 5f6c 696e 6529  ont_format_line)
-00001440: 0a0a 2020 2020 2320 4f75 7470 7574 2061  ..    # Output a
-00001450: 2066 6c61 6720 746f 2069 6e64 6963 6174   flag to indicat
-00001460: 6520 7468 6973 2069 7320 7768 6572 6520  e this is where 
-00001470: 7468 6520 6469 7265 6374 6f72 7920 676f  the directory go
-00001480: 6573 0a20 2020 2050 7269 6d65 4974 656d  es.    PrimeItem
-00001490: 732e 6f75 7470 7574 5f6c 696e 6573 2e61  s.output_lines.a
-000014a0: 6464 5f6c 696e 655f 746f 5f6f 7574 7075  dd_line_to_outpu
-000014b0: 7428 352c 2022 6d61 7074 6173 6b65 725f  t(5, "maptasker_
-000014c0: 6469 7265 6374 6f72 7922 2c20 466f 726d  directory", Form
-000014d0: 6174 4c69 6e65 2e64 6f6e 745f 666f 726d  atLine.dont_form
-000014e0: 6174 5f6c 696e 6529 0a0a 2020 2020 2320  at_line)..    # 
-000014f0: 4966 2064 6f69 6e67 2054 6173 6b65 7220  If doing Tasker 
-00001500: 7072 6566 6572 656e 6365 732c 2067 6574  preferences, get
-00001510: 2074 6865 6d0a 2020 2020 6966 2050 7269   them.    if Pri
-00001520: 6d65 4974 656d 732e 7072 6f67 7261 6d5f  meItems.program_
-00001530: 6172 6775 6d65 6e74 735b 2270 7265 6665  arguments["prefe
-00001540: 7265 6e63 6573 225d 3a0a 2020 2020 2020  rences"]:.      
-00001550: 2020 6765 745f 7072 6566 6572 656e 6365    get_preference
-00001560: 7328 290a                                s().
+00000600: 2323 230a 6465 6620 6f75 7470 7574 5f74  ###.def output_t
+00000610: 6865 5f68 6561 6469 6e67 2829 202d 3e20  he_heading() -> 
+00000620: 4e6f 6e65 3a0a 2020 2020 2222 220a 2020  None:.    """.  
+00000630: 2020 4469 7370 6c61 7920 7468 6520 6865    Display the he
+00000640: 6164 696e 6720 616e 6420 736f 7572 6365  ading and source
+00000650: 2066 696c 6520 6465 7461 696c 730a 2020   file details.  
+00000660: 2020 2222 220a 2320 2020 2077 696e 646f    """.#    windo
+00000670: 775f 6469 6d65 6e73 696f 6e73 203d 2022  w_dimensions = "
+00000680: 2222 0a23 3c70 2069 643d 226d 7977 696e  "".#<p id="mywin
+00000690: 223e 3c2f 703e 0a23 3c73 6372 6970 743e  "></p>.#<script>
+000006a0: 0a23 7661 7220 7720 3d20 7769 6e64 6f77  .#var w = window
+000006b0: 2e69 6e6e 6572 5769 6474 683b 0a23 7661  .innerWidth;.#va
+000006c0: 7220 6820 3d20 7769 6e64 6f77 2e69 6e6e  r h = window.inn
+000006d0: 6572 4865 6967 6874 3b0a 2376 6172 2078  erHeight;.#var x
+000006e0: 203d 2064 6f63 756d 656e 742e 6765 7445   = document.getE
+000006f0: 6c65 6d65 6e74 4279 4964 2822 6d79 7769  lementById("mywi
+00000700: 6e22 293b 0a23 782e 696e 6e65 7248 544d  n");.#x.innerHTM
+00000710: 4c20 3d20 2242 726f 7773 6572 2077 6964  L = "Browser wid
+00000720: 7468 3a20 2220 2b20 7720 2b20 222c 2068  th: " + w + ", h
+00000730: 6569 6768 743a 2022 202b 2068 202b 2022  eight: " + h + "
+00000740: 2e22 3b0a 233c 2f73 6372 6970 743e 2222  .";.#</script>""
+00000750: 220a 0a20 2020 2023 2053 7461 7274 206f  "..    # Start o
+00000760: 7574 2062 7920 6f75 7470 7574 7469 6e67  ut by outputting
+00000770: 206f 7572 2063 6f6c 6f72 7320 616e 6420   our colors and 
+00000780: 666f 6e74 2043 5353 0a20 2020 2061 6464  font CSS.    add
+00000790: 5f63 7373 2829 0a0a 2020 2020 7461 736b  _css()..    task
+000007a0: 6572 5f6d 6170 7069 6e67 203d 2022 5461  er_mapping = "Ta
+000007b0: 736b 6572 204d 6170 7069 6e67 2e2e 2e2e  sker Mapping....
+000007c0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2054 6173  ............ Tas
+000007d0: 6b65 7220 584d 4c20 7665 7273 696f 6e3a  ker XML version:
+000007e0: 220a 0a20 2020 2023 2047 6574 2074 6865  "..    # Get the
+000007f0: 2073 6372 6565 6e20 6469 6d65 6e73 696f   screen dimensio
+00000800: 6e73 2066 726f 6d20 3c64 6d65 7472 6963  ns from <dmetric
+00000810: 3e20 786d 6c0a 2020 2020 7363 7265 656e  > xml.    screen
+00000820: 5f65 6c65 6d65 6e74 203d 2050 7269 6d65  _element = Prime
+00000830: 4974 656d 732e 786d 6c5f 726f 6f74 2e66  Items.xml_root.f
+00000840: 696e 6428 2264 6d65 7472 6963 2229 0a20  ind("dmetric"). 
+00000850: 2020 2073 6372 6565 6e5f 7369 7a65 203d     screen_size =
+00000860: 2028 0a20 2020 2020 2020 2066 2726 6e62   (.        f'&nb
+00000870: 7370 3b26 6e62 7370 3b44 6576 6963 6520  sp;&nbsp;Device 
+00000880: 7363 7265 656e 2073 697a 653a 207b 7363  screen size: {sc
+00000890: 7265 656e 5f65 6c65 6d65 6e74 2e74 6578  reen_element.tex
+000008a0: 742e 7265 706c 6163 6528 222c 222c 2022  t.replace(",", "
+000008b0: 2058 2022 297d 270a 2020 2020 2020 2020   X ")}'.        
+000008c0: 6966 2073 6372 6565 6e5f 656c 656d 656e  if screen_elemen
+000008d0: 7420 6973 206e 6f74 204e 6f6e 650a 2020  t is not None.  
+000008e0: 2020 2020 2020 656c 7365 2022 220a 2020        else "".  
+000008f0: 2020 290a 0a20 2020 2023 2053 6574 2075    )..    # Set u
+00000900: 7020 6869 6768 6c69 6768 7420 6261 636b  p highlight back
+00000910: 6772 6f75 6e64 2063 6f6c 6f72 2069 6620  ground color if 
+00000920: 6e65 6564 6564 0a20 2020 2069 6620 5072  needed.    if Pr
+00000930: 696d 6549 7465 6d73 2e70 726f 6772 616d  imeItems.program
+00000940: 5f61 7267 756d 656e 7473 5b22 6869 6768  _arguments["high
+00000950: 6c69 6768 7422 5d3a 0a20 2020 2020 2020  light"]:.       
+00000960: 2062 6163 6b67 726f 756e 645f 636f 6c6f   background_colo
+00000970: 725f 6874 6d6c 203d 2028 0a20 2020 2020  r_html = (.     
+00000980: 2020 2020 2020 2022 3c73 7479 6c65 3e5c         "<style>\
+00000990: 6e6d 6172 6b20 7b20 5c6e 6261 636b 6772  nmark { \nbackgr
+000009a0: 6f75 6e64 2d63 6f6c 6f72 3a20 2220 2b20  ound-color: " + 
+000009b0: 5072 696d 6549 7465 6d73 2e63 6f6c 6f72  PrimeItems.color
+000009c0: 735f 746f 5f75 7365 5b22 6869 6768 6c69  s_to_use["highli
+000009d0: 6768 745f 636f 6c6f 7222 5d20 2b20 223b  ght_color"] + ";
+000009e0: 5c6e 7d5c 6e3c 2f73 7479 6c65 3e5c 6e22  \n}\n</style>\n"
+000009f0: 0a20 2020 2020 2020 2029 0a20 2020 2065  .        ).    e
+00000a00: 6c73 653a 0a20 2020 2020 2020 2062 6163  lse:.        bac
+00000a10: 6b67 726f 756e 645f 636f 6c6f 725f 6874  kground_color_ht
+00000a20: 6d6c 203d 2022 220a 0a20 2020 2023 204f  ml = ""..    # O
+00000a30: 7574 7075 7420 6461 7465 2061 6e64 2074  utput date and t
+00000a40: 696d 6520 6966 2069 6e20 6465 6275 6720  ime if in debug 
+00000a50: 6d6f 6465 0a20 2020 206e 6f77 5f66 6f72  mode.    now_for
+00000a60: 5f6f 7574 7075 7420 3d20 4e4f 575f 5449  _output = NOW_TI
+00000a70: 4d45 2e73 7472 6674 696d 6528 2225 642d  ME.strftime("%d-
+00000a80: 2542 2d25 5920 2548 3a25 4d3a 2553 2229  %B-%Y %H:%M:%S")
+00000a90: 0a0a 2020 2020 2320 466f 726d 6174 2074  ..    # Format t
+00000aa0: 6865 206f 7574 7075 7420 6865 6164 696e  he output headin
+00000ab0: 670a 2020 2020 6865 6164 696e 675f 636f  g.    heading_co
+00000ac0: 6c6f 7220 3d20 2268 6561 6469 6e67 5f63  lor = "heading_c
+00000ad0: 6f6c 6f72 220a 2020 2020 5072 696d 6549  olor".    PrimeI
+00000ae0: 7465 6d73 2e68 6561 6469 6e67 203d 2028  tems.heading = (
+00000af0: 0a20 2020 2020 2020 2066 273c 2164 6f63  .        f'<!doc
+00000b00: 7479 7065 2068 746d 6c3e 5c6e 3c68 746d  type html>\n<htm
+00000b10: 6c20 6c61 6e67 3de2 809d 656e e280 9d3e  l lang=...en...>
+00000b20: 5c6e 3c68 6561 643e 5c6e 3c6d 6574 6120  \n<head>\n<meta 
+00000b30: 6368 6172 7365 743d 2255 5446 2d38 223e  charset="UTF-8">
+00000b40: 7b62 6163 6b67 726f 756e 645f 636f 6c6f  {background_colo
+00000b50: 725f 6874 6d6c 7d3c 7469 746c 653e 4d61  r_html}<title>Ma
+00000b60: 7054 6173 6b65 723c 2f74 6974 6c65 3e5c  pTasker</title>\
+00000b70: 6e3c 626f 6479 270a 2020 2020 2020 2020  n<body'.        
+00000b80: 6622 2073 7479 6c65 3d5c 2262 6163 6b67  f" style=\"backg
+00000b90: 726f 756e 642d 636f 6c6f 723a 7b50 7269  round-color:{Pri
+00000ba0: 6d65 4974 656d 732e 636f 6c6f 7273 5f74  meItems.colors_t
+00000bb0: 6f5f 7573 655b 2762 6163 6b67 726f 756e  o_use['backgroun
+00000bc0: 645f 636f 6c6f 7227 5d7d 5c22 3e5c 6e22  d_color']}\">\n"
+00000bd0: 0a20 2020 2020 2020 202b 2066 6f72 6d61  .        + forma
+00000be0: 745f 6874 6d6c 280a 2020 2020 2020 2020  t_html(.        
+00000bf0: 2020 2020 6865 6164 696e 675f 636f 6c6f      heading_colo
+00000c00: 722c 0a20 2020 2020 2020 2020 2020 2022  r,.            "
+00000c10: 222c 0a20 2020 2020 2020 2020 2020 2028  ",.            (
+00000c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000c30: 2066 223c 6832 3e7b 4e4f 524d 414c 5f54   f"<h2>{NORMAL_T
+00000c40: 4142 7d4d 6170 5461 736b 6572 3c2f 6832  AB}MapTasker</h2
+00000c50: 3e3c 6272 3e7b 4e4f 524d 414c 5f54 4142  ><br>{NORMAL_TAB
+00000c60: 7d7b 7461 736b 6572 5f6d 6170 7069 6e67  }{tasker_mapping
+00000c70: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+00000c80: 2020 2066 2220 7b50 7269 6d65 4974 656d     f" {PrimeItem
+00000c90: 732e 786d 6c5f 726f 6f74 2e61 7474 7269  s.xml_root.attri
+00000ca0: 625b 2774 7627 5d7d 266e 6273 703b 266e  b['tv']}&nbsp;&n
+00000cb0: 6273 703b 266e 6273 703b 266e 6273 703b  bsp;&nbsp;&nbsp;
+00000cc0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00000cd0: 2020 6622 7b4d 595f 5645 5253 494f 4e7d    f"{MY_VERSION}
+00000ce0: 7b73 6372 6565 6e5f 7369 7a65 7d26 6e62  {screen_size}&nb
+00000cf0: 7370 3b26 6e62 7370 3b26 6e62 7370 3b26  sp;&nbsp;&nbsp;&
+00000d00: 6e62 7370 3b7b 6e6f 775f 666f 725f 6f75  nbsp;{now_for_ou
+00000d10: 7470 7574 7d22 0a20 2020 2020 2020 2020  tput}".         
+00000d20: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
+00000d30: 2020 5472 7565 2c0a 2020 2020 2020 2020    True,.        
+00000d40: 290a 2020 2020 290a 0a20 2020 2023 2041  ).    )..    # A
+00000d50: 6464 2073 6372 6970 7420 746f 2067 6574  dd script to get
+00000d60: 2077 696e 646f 7720 6469 6d65 6e73 696f   window dimensio
+00000d70: 6e73 0a20 2020 2023 5072 696d 6549 7465  ns.    #PrimeIte
+00000d80: 6d73 2e6f 7574 7075 745f 6c69 6e65 732e  ms.output_lines.
+00000d90: 6164 645f 6c69 6e65 5f74 6f5f 6f75 7470  add_line_to_outp
+00000da0: 7574 280a 2020 2020 2320 2020 2030 2c0a  ut(.    #    0,.
+00000db0: 2020 2020 2320 2020 2077 696e 646f 775f      #    window_
+00000dc0: 6469 6d65 6e73 696f 6e73 2c0a 2020 2020  dimensions,.    
+00000dd0: 2320 2020 2046 6f72 6d61 744c 696e 652e  #    FormatLine.
+00000de0: 646f 6e74 5f66 6f72 6d61 745f 6c69 6e65  dont_format_line
+00000df0: 2c0a 2020 2020 2329 0a0a 2020 2020 2320  ,.    #)..    # 
+00000e00: 4164 6420 6120 626c 616e 6b20 6c69 6e65  Add a blank line
+00000e10: 0a20 2020 2050 7269 6d65 4974 656d 732e  .    PrimeItems.
+00000e20: 6f75 7470 7574 5f6c 696e 6573 2e61 6464  output_lines.add
+00000e30: 5f6c 696e 655f 746f 5f6f 7574 7075 7428  _line_to_output(
+00000e40: 0a20 2020 2020 2020 2030 2c0a 2020 2020  .        0,.    
+00000e50: 2020 2020 5072 696d 6549 7465 6d73 2e68      PrimeItems.h
+00000e60: 6561 6469 6e67 2c0a 2020 2020 2020 2020  eading,.        
+00000e70: 466f 726d 6174 4c69 6e65 2e64 6f6e 745f  FormatLine.dont_
+00000e80: 666f 726d 6174 5f6c 696e 652c 0a20 2020  format_line,.   
+00000e90: 2029 0a0a 2020 2020 2320 4469 7370 6c61   )..    # Displa
+00000ea0: 7920 7768 6572 6520 7468 6520 736f 7572  y where the sour
+00000eb0: 6365 2066 696c 6520 6361 6d65 2066 726f  ce file came fro
+00000ec0: 6d0a 2020 2020 2320 4469 6420 7765 2072  m.    # Did we r
+00000ed0: 6573 746f 7265 2074 6865 2062 6163 6b75  estore the backu
+00000ee0: 7020 6672 6f6d 2041 6e64 726f 6964 3f0a  p from Android?.
+00000ef0: 2020 2020 6966 2050 7269 6d65 4974 656d      if PrimeItem
+00000f00: 732e 7072 6f67 7261 6d5f 6172 6775 6d65  s.program_argume
+00000f10: 6e74 735b 2266 6574 6368 6564 5f62 6163  nts["fetched_bac
+00000f20: 6b75 705f 6672 6f6d 5f61 6e64 726f 6964  kup_from_android
+00000f30: 225d 3a0a 2020 2020 2020 2020 736f 7572  "]:.        sour
+00000f40: 6365 5f66 696c 6520 3d20 280a 2020 2020  ce_file = (.    
+00000f50: 2020 2020 2020 2020 2246 726f 6d20 416e          "From An
+00000f60: 6472 6f69 6420 6465 7669 6365 220a 2020  droid device".  
+00000f70: 2020 2020 2020 2020 2020 6627 2054 4350            f' TCP
+00000f80: 2049 5020 6164 6472 6573 733a 7b50 7269   IP address:{Pri
+00000f90: 6d65 4974 656d 732e 7072 6f67 7261 6d5f  meItems.program_
+00000fa0: 6172 6775 6d65 6e74 735b 2261 6e64 726f  arguments["andro
+00000fb0: 6964 5f69 7061 6464 7222 5d7d 270a 2020  id_ipaddr"]}'.  
+00000fc0: 2020 2020 2020 2020 2020 6627 206f 6e20            f' on 
+00000fd0: 706f 7274 3a7b 5072 696d 6549 7465 6d73  port:{PrimeItems
+00000fe0: 2e70 726f 6772 616d 5f61 7267 756d 656e  .program_argumen
+00000ff0: 7473 5b22 616e 6472 6f69 645f 706f 7274  ts["android_port
+00001000: 225d 7d27 0a20 2020 2020 2020 2020 2020  "]}'.           
+00001010: 2066 2720 7769 7468 2066 696c 6520 6c6f   f' with file lo
+00001020: 6361 7469 6f6e 3a20 7b50 7269 6d65 4974  cation: {PrimeIt
+00001030: 656d 732e 7072 6f67 7261 6d5f 6172 6775  ems.program_argu
+00001040: 6d65 6e74 735b 2261 6e64 726f 6964 5f66  ments["android_f
+00001050: 696c 6522 5d7d 270a 2020 2020 2020 2020  ile"]}'.        
+00001060: 290a 2020 2020 656c 6966 2050 7269 6d65  ).    elif Prime
+00001070: 4974 656d 732e 7072 6f67 7261 6d5f 6172  Items.program_ar
+00001080: 6775 6d65 6e74 735b 2264 6562 7567 225d  guments["debug"]
+00001090: 206f 7220 6e6f 7420 5072 696d 6549 7465   or not PrimeIte
+000010a0: 6d73 2e70 726f 6772 616d 5f61 7267 756d  ms.program_argum
+000010b0: 656e 7473 5b22 6669 6c65 225d 3a0a 2020  ents["file"]:.  
+000010c0: 2020 2020 2020 6669 6c65 6e61 6d65 203d        filename =
+000010d0: 2069 7369 6e73 7461 6e63 6528 5072 696d   isinstance(Prim
+000010e0: 6549 7465 6d73 2e66 696c 655f 746f 5f67  eItems.file_to_g
+000010f0: 6574 2c20 7374 7229 0a20 2020 2020 2020  et, str).       
+00001100: 2066 696c 656e 616d 6520 3d20 5072 696d   filename = Prim
+00001110: 6549 7465 6d73 2e66 696c 655f 746f 5f67  eItems.file_to_g
+00001120: 6574 2e6e 616d 6520 6966 206e 6f74 2066  et.name if not f
+00001130: 696c 656e 616d 6520 656c 7365 2050 7269  ilename else Pri
+00001140: 6d65 4974 656d 732e 6669 6c65 5f74 6f5f  meItems.file_to_
+00001150: 6765 740a 2020 2020 2020 2020 736f 7572  get.        sour
+00001160: 6365 5f66 696c 6520 3d20 6669 6c65 6e61  ce_file = filena
+00001170: 6d65 0a20 2020 2065 6c73 653a 0a20 2020  me.    else:.   
+00001180: 2020 2020 2073 6f75 7263 655f 6669 6c65       source_file
+00001190: 203d 2050 7269 6d65 4974 656d 732e 7072   = PrimeItems.pr
+000011a0: 6f67 7261 6d5f 6172 6775 6d65 6e74 735b  ogram_arguments[
+000011b0: 2266 696c 6522 5d0a 2020 2020 2320 4164  "file"].    # Ad
+000011c0: 6420 736f 7572 6365 2074 6f20 6f75 7470  d source to outp
+000011d0: 7574 0a20 2020 2050 7269 6d65 4974 656d  ut.    PrimeItem
+000011e0: 732e 6f75 7470 7574 5f6c 696e 6573 2e61  s.output_lines.a
+000011f0: 6464 5f6c 696e 655f 746f 5f6f 7574 7075  dd_line_to_outpu
+00001200: 7428 0a20 2020 2020 2020 2030 2c0a 2020  t(.        0,.  
+00001210: 2020 2020 2020 6622 3c62 723e 3c62 723e        f"<br><br>
+00001220: 7b4e 4f52 4d41 4c5f 5441 427d 536f 7572  {NORMAL_TAB}Sour
+00001230: 6365 2062 6163 6b75 7020 6669 6c65 3a20  ce backup file: 
+00001240: 7b73 6f75 7263 655f 6669 6c65 7d22 2c0a  {source_file}",.
+00001250: 2020 2020 2020 2020 5b22 222c 2022 6865          ["", "he
+00001260: 6164 696e 675f 636f 6c6f 7222 2c20 466f  ading_color", Fo
+00001270: 726d 6174 4c69 6e65 2e61 6464 5f65 6e64  rmatLine.add_end
+00001280: 5f73 7061 6e5d 2c0a 2020 2020 290a 0a0a  _span],.    )...
+00001290: 2320 2323 2323 2323 2323 2323 2323 2323  # ##############
+000012a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000012b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000012c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000012d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000012e0: 2323 2323 0a23 204f 7574 7075 7420 7468  ####.# Output th
+000012f0: 6520 6865 6164 696e 6720 6574 632e 2061  e heading etc. a
+00001300: 7320 7468 6520 6672 6f6e 7420 6d61 7474  s the front matt
+00001310: 6572 2e0a 2320 2323 2323 2323 2323 2323  er..# ##########
+00001320: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001330: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001340: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001350: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001360: 2323 2323 2323 2323 0a64 6566 206f 7574  ########.def out
+00001370: 7075 745f 7468 655f 6672 6f6e 745f 6d61  put_the_front_ma
+00001380: 7474 6572 2829 202d 3e20 4e6f 6e65 3a0a  tter() -> None:.
+00001390: 2020 2020 2222 220a 2020 2020 4765 6e65      """.    Gene
+000013a0: 7261 7465 7320 7468 6520 6672 6f6e 7420  rates the front 
+000013b0: 6d61 7474 6572 2066 6f72 2074 6865 206f  matter for the o
+000013c0: 7574 7075 7420 6669 6c65 3a20 6865 6164  utput file: head
+000013d0: 696e 672c 2072 756e 7469 6d65 2073 6574  ing, runtime set
+000013e0: 7469 6e67 732c 0a20 2020 2064 6972 6563  tings,.    direc
+000013f0: 746f 7279 2c20 5461 736b 6572 2070 7265  tory, Tasker pre
+00001400: 6665 7265 6e63 6573 2e0a 2020 2020 2222  ferences..    ""
+00001410: 220a 0a20 2020 2023 2048 6561 6469 6e67  "..    # Heading
+00001420: 2069 6e66 6f72 6d61 7469 6f6e 0a20 2020   information.   
+00001430: 206f 7574 7075 745f 7468 655f 6865 6164   output_the_head
+00001440: 696e 6728 290a 0a20 2020 2023 2049 6620  ing()..    # If 
+00001450: 7765 2061 7265 2064 6562 7567 6769 6e67  we are debugging
+00001460: 2c20 6f75 7470 7574 2074 6865 2072 756e  , output the run
+00001470: 7469 6d65 2061 7267 756d 656e 7473 2061  time arguments a
+00001480: 6e64 2063 6f6c 6f72 730a 2020 2020 6966  nd colors.    if
+00001490: 2050 7269 6d65 4974 656d 732e 7072 6f67   PrimeItems.prog
+000014a0: 7261 6d5f 6172 6775 6d65 6e74 735b 2264  ram_arguments["d
+000014b0: 6562 7567 225d 206f 7220 5072 696d 6549  ebug"] or PrimeI
+000014c0: 7465 6d73 2e70 726f 6772 616d 5f61 7267  tems.program_arg
+000014d0: 756d 656e 7473 5b22 7275 6e74 696d 6522  uments["runtime"
+000014e0: 5d3a 0a20 2020 2020 2020 2064 6973 706c  ]:.        displ
+000014f0: 6179 5f64 6562 7567 5f69 6e66 6f28 290a  ay_debug_info().
+00001500: 0a20 2020 2023 204f 7574 7075 7420 6120  .    # Output a 
+00001510: 666c 6167 2074 6f20 696e 6469 6361 7465  flag to indicate
+00001520: 2074 6869 7320 6973 2077 6865 7265 2074   this is where t
+00001530: 6865 2064 6972 6563 746f 7279 2067 6f65  he directory goe
+00001540: 730a 2020 2020 5072 696d 6549 7465 6d73  s.    PrimeItems
+00001550: 2e6f 7574 7075 745f 6c69 6e65 732e 6164  .output_lines.ad
+00001560: 645f 6c69 6e65 5f74 6f5f 6f75 7470 7574  d_line_to_output
+00001570: 2835 2c20 226d 6170 7461 736b 6572 5f64  (5, "maptasker_d
+00001580: 6972 6563 746f 7279 222c 2046 6f72 6d61  irectory", Forma
+00001590: 744c 696e 652e 646f 6e74 5f66 6f72 6d61  tLine.dont_forma
+000015a0: 745f 6c69 6e65 290a 0a20 2020 2023 2049  t_line)..    # I
+000015b0: 6620 646f 696e 6720 5461 736b 6572 2070  f doing Tasker p
+000015c0: 7265 6665 7265 6e63 6573 2c20 6765 7420  references, get 
+000015d0: 7468 656d 0a20 2020 2069 6620 5072 696d  them.    if Prim
+000015e0: 6549 7465 6d73 2e70 726f 6772 616d 5f61  eItems.program_a
+000015f0: 7267 756d 656e 7473 5b22 7072 6566 6572  rguments["prefer
+00001600: 656e 6365 7322 5d3a 0a20 2020 2020 2020  ences"]:.       
+00001610: 2067 6574 5f70 7265 6665 7265 6e63 6573   get_preferences
+00001620: 2829 0a                                  ().
```

### Comparing `maptasker-2.6.3/maptasker/src/getbakup.py` & `maptasker-3.2.2/maptasker/src/getbakup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,21 +7,19 @@
 # GNU General Public License v3.0                                                      #
 # Permissions of this strong copyleft license are conditioned on making available      #
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
+from __future__ import annotations
 
 import os.path
 from os import getcwd
 
-import requests
-from requests.exceptions import ConnectionError, ConnectTimeout, InvalidSchema
-
 from maptasker.src.error import error_handler
 from maptasker.src.primitem import PrimeItems
 from maptasker.src.sysconst import logger
 
 
 # ##################################################################################
 # We've read in the xml backup file.  Now save it for processing.
@@ -37,17 +35,18 @@
     my_output_dir = getcwd()
     if my_output_dir is None:
         error_handler(
             "MapTasker cancelled.  An error occurred in getbakup.  Program cancelled.",
             2,
         )
 
-    # We are going to save the file as...
+    # We must get just the file name and type since we will be using this to save it to our local path.
+    # This is the file we will do all of our processing against...the local file fetched from the Android device.
     # Get position of the last "/" in path/file
-    name_location = PrimeItems.program_arguments["android_file"].rfind("/") + 1
+    name_location = PrimeItems.program_arguments["android_file"].rfind(PrimeItems.slash) + 1
     # Get the name of the file
     my_file_name = PrimeItems.program_arguments["android_file"][name_location:]
 
     # Convert the binary code to string
     output_lines = file_contents.decode("utf-8")
 
     # Set up the backup file full path
@@ -67,65 +66,14 @@
             out_file.write(item)
 
     # Set flag to identify that backup file was fetched from Android device
     PrimeItems.program_arguments["fetched_backup_from_android"] = True
 
 
 # ##################################################################################
-# Issue HTTP Request to get the backup xml file from the Android device.
-# ##################################################################################
-def request_file(ip_addr: str, port_number: str, file_location: str) -> tuple[int, object]:
-    """
-    Issue HTTP Request to get the backup xml file from the Android device.
-    Tasker's HTTP Server Example must be installed for this to work:
-    https://taskernet.com/shares/?user=AS35m8ne7oO4s%2BaDx%2FwlzjdFTfVMWstg1ay5AkpiNdrLoSXEZdFfw1IpXiyJCVLNW0yn&id=Project%3AHttp+Server+Example
-        :param backup_file_http: the port to use for the Android device's Tasker server
-        :param backup_file_location: location of
-        :return: return code, response: eitherr text string with error message or the
-        contents of the backup file
-    """
-    # Create the URL to request the backup xml file from the Android device running the
-    # Tasker server.
-    # Something like: 192.168.0.210:1821/file/path/to/backup.xml?download=1
-    http = "http://" if "http://" not in ip_addr else ""
-    url = f"{http}{ip_addr}:{port_number}/file{file_location}?download=1"
-
-    # Make the request.
-    try:
-        response = requests.get(url, timeout=10)
-    except InvalidSchema:
-        return (
-            8,
-            f"Request failed for url: {url} .  Invalid url!",
-        )
-    except ConnectionError:
-        return (
-            8,
-            f"Request failed for url: {url} .  Connection error!",
-        )
-    except ConnectTimeout:
-        return (
-            8,
-            f"Request failed for url: {url} .  Timeout error!",
-        )
-
-    # Check the response status code.
-    if response.status_code == 200:
-        # Return the contents of the file.
-        return 0, response.content
-    elif response.status_code == 404:
-        return 6, f"File '{file_location}' not found."
-    else:
-        return (
-            8,
-            f"Request failed for url: {url} ...with status code {response.status_code}",
-        )
-
-
-# ##################################################################################
 # Return the substring after the last occurance of a specific character in a string
 # ##################################################################################
 def substring_after_last(string: str, char: chr) -> str:
     """
     Return the substring after the last occurance of a specific character in a string
         Args:
             string (str): The string to search for the substring
@@ -144,19 +92,27 @@
 def get_backup_file() -> str:
     """
     Set up to fetch the Tasker backup xml file from the Android device running
     the Tasker server
 
         :return: The name of the backup file (e.g. backup.xml)
     """
-    # Get the contents of the file.
-    return_code, file_contents = request_file(
+    from maptasker.src.maputils import http_request
+
+    # If ruinning from the GUI, then we have already gotten the file. Just return the name on the local drive.add
+    if PrimeItems.program_arguments["gui"]:
+        return substring_after_last(PrimeItems.program_arguments["android_file"], "/")
+
+    # Get the contents of the file from the Android device.
+    return_code, file_contents = http_request(
         PrimeItems.program_arguments["android_ipaddr"],
         PrimeItems.program_arguments["android_port"],
         PrimeItems.program_arguments["android_file"],
+        "file",
+        "?download=1",
     )
 
     if return_code != 0:
         if PrimeItems.program_arguments["gui"]:
             PrimeItems.error_code = return_code
             return None
         error_handler(str(file_contents), 8)
```

### Comparing `maptasker-2.6.3/maptasker/src/getids.py` & `maptasker-3.2.2/maptasker/src/getids.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
 
 import defusedxml.ElementTree  # Need for type hints
-from maptasker.src.primitem import PrimeItems
-from maptasker.src.sysconst import FormatLine
 
 
 def get_ids(
     doing_head_xml_element: bool,
     head_xml_element: defusedxml.ElementTree.XML,
     head_xml_element_name: str,
     head_xml_elements_without_profiles: list,
@@ -29,22 +27,18 @@
     :param head_xml_element: head_xml_element xml element
     :param head_xml_element_name: name of head_xml_element
     :param head_xml_elements_without_profiles: list of elements without ids
     :return: list of found IDs, or empty list if none found
     """
 
     found_ids = ""
-    # Get Profiles by searching for <pids> element
-    if doing_head_xml_element:
-        ids_to_find = "pids"
-        # Start Profile list
-        PrimeItems.output_lines.add_line_to_output(1, "", FormatLine.dont_format_line)
-    else:
-        # If not Profile IDs, just get Task IDs via <tids> xml element.
-        ids_to_find = "tids"
+    # Get Profiles by searching for <pids> element.  If not Profile IDs, just get Task IDs via <tids> xml element.
+    ids_to_find = "pids" if doing_head_xml_element else "tids"
+
+    # Get the IDs.
     try:
         # Get a list of the Profiles for this head_xml_element
         found_ids = head_xml_element.find(ids_to_find).text
     except AttributeError:  # head_xml_element has no Profile/Task IDs
         if head_xml_element_name not in head_xml_elements_without_profiles:
             head_xml_elements_without_profiles.append(head_xml_element_name)
```

### Comparing `maptasker-2.6.3/maptasker/src/globalvr.py` & `maptasker-3.2.2/maptasker/src/globalvr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
+"""Display global variables in output HTML"""
+
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
 # variables: process Tasker variables.                                                 #
 #                                                                                      #
 # GNU General Public License v3.0                                                      #
 # Permissions of this strong copyleft license are conditioned on making available      #
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
+import darkdetect
 import defusedxml.ElementTree  # Need for type hints
 
-from maptasker.src.sysconst import FormatLine
 from maptasker.src.primitem import PrimeItems
+from maptasker.src.sysconst import NORMAL_TAB, TABLE_BACKGROUND_COLOR, TABLE_BORDER, FormatLine
 
 # List of Tasker global variables
 tasker_global_variables = [
     "%AIR",
     "%AIRR",
     "%BATT",
     "%BLUE",
@@ -156,41 +159,54 @@
         }
 
 
 # ##################################################################################
 # Print the variables (Project's or Unreferenced)
 # ##################################################################################
 def print_the_variables(color_to_use: str, project: defusedxml.ElementTree) -> None:
-    """
-    Print the variables (Project's or Unreferenced)
-        Args:
-            color_to_use (str): Colot to use in the output.
-            project (xml element): xml element of the Project.
-        Return: list of output lines to be added to output queue.
-    """
+    """Parameters:
+        - color_to_use (str): The color to use for the table definition.
+        - project (defusedxml.ElementTree): The project to use, if applicable.
+    Returns:
+        - None: This function does not return anything.
+    Processing Logic:
+        - Create table definition.
+        - Create empty list for variable output lines.
+        - Sort the Tasker global variables.
+        - If the key is a Tasker global variable, change the value to "global".
+        - If project is not None or an empty string, find the Project.
+        - If the variable has a list of Projects, extend the variable output lines with the key and value.
+        - If the variable is a verified "tasker variable" and not a Project global variable, append the key and value to the variable output lines.
+        - Return the variable output lines."""
     table_definition = f'<td style="height:16px; color:{color_to_use}; text-align:left">'
     variable_output_lines = []
 
     # Go through all of the Tasker global variables.
     for key, value in sorted(PrimeItems.variables.items()):
         # If this is a Tasker global variable, change the value to "global"
         if key in tasker_global_variables:
             value["value"] = "<em>Tasker Global</em>"
 
         # If doing the Project variables, first find the Project
-        if project:
+        if project is not None and project != "":
             # Does this variable have a list of Projects?
             if PrimeItems.variables[key]["project"]:
-                variable_output_lines.extend(
-                    f'<tr>{table_definition}{key}</td>{table_definition}{value["value"]}</td></tr>'
-                    for variable_project in PrimeItems.variables[key]["project"]
-                    if variable_project["xml"] == project
-                )
+                for variable_project in PrimeItems.variables[key]["project"]:
+                    if variable_project["xml"] == project:
+                        variable_output_lines.append(
+                            f"<tr>{table_definition}{key}</td>{table_definition}{value['value']}</td></tr>"
+                        )
+                # variable_output_lines.extend(
+                #     f'<tr>{table_definition}{key}</td>{table_definition}{value["value"]}</td></tr>'
+                #     for variable_project in PrimeItems.variables[key]["project"]
+                #     if variable_project["xml"] == project
+                # )
         # If this is a verified "tasker variable", and not a Project global var?
         elif PrimeItems.variables[key]["verified"] and not PrimeItems.variables[key]["project"]:
+            # It is an unrefereenced variable.
             variable_output_lines.append(f"<tr>{table_definition}{key}</td>{table_definition}{value}</td></tr>")
 
     return variable_output_lines
 
 
 # ##################################################################################
 # Print variables by adding them to the output.
@@ -202,23 +218,24 @@
 
             heading (str): Heading to print.
             project (xml.etree.ElementTree): Project to print.
     """
     if not PrimeItems.variables:
         return
     # Add a directory entry for variables.
-    if not project and PrimeItems.program_arguments["directory"]:
+    if (project is None or project == "") and PrimeItems.program_arguments["directory"]:
         PrimeItems.output_lines.add_line_to_output(
             5,
             '<a id="unreferenced_variables"></a>',
             FormatLine.dont_format_line,
         )
 
+    # Output unreferenced global variables.  The Project will be "".
     # Force an indentation and set color to use in output.
-    if not project:
+    if project is None or project == "":
         color_to_use = PrimeItems.colors_to_use["trailing_comments_color"]
         color_name = "trailing_comments_color"
         PrimeItems.output_lines.add_line_to_output(
             1,
             "",
             ["", "trailing_comments_color", FormatLine.add_end_span],
         )
@@ -228,23 +245,24 @@
             "<br><hr>",
             FormatLine.dont_format_line,
         )
     else:
         color_to_use = PrimeItems.colors_to_use["project_color"]
         color_name = "project_color"
 
+    # Print the heading if we have global variables.
     if variable_output_lines := print_the_variables(color_to_use, project):
         PrimeItems.output_lines.add_line_to_output(
             5,
-            heading,
+            f"<br>{NORMAL_TAB}{heading}",
             ["", color_name, FormatLine.add_end_span],
         )
 
         # Define table
-        table_definition = f'<table cellspacing="1" cellpadding="2" border="1" style="height:16px; color:{color_to_use}; text-align:left">\n<tr>\n<th>Name</th>\n<th>Value</th>\n</tr>'
+        table_definition = f'{TABLE_BORDER}<table cellspacing="1" cellpadding="2" border="1" style="height:16px; margin-left: 20;color:{color_to_use};background-color:{TABLE_BACKGROUND_COLOR};font-family:{PrimeItems.program_arguments["font"]};text-align:left">\n<tr>\n<th>Name</th>\n<th>Value</th>\n</tr>'
         PrimeItems.output_lines.add_line_to_output(
             5,
             table_definition,
             FormatLine.dont_format_line,
         )
 
         # Now go through our dictionary outputing the (sorted) variables
@@ -259,13 +277,13 @@
         # End table
         PrimeItems.output_lines.add_line_to_output(
             5,
             "</table><br>",
             FormatLine.dont_format_line,
         )
         # Un-indent the output only if doing unreferenced variables.
-        if not project:
+        if project is None or project == "":
             PrimeItems.output_lines.add_line_to_output(
                 3,
                 "",
                 FormatLine.dont_format_line,
             )
```

### Comparing `maptasker-2.6.3/maptasker/src/initparg.py` & `maptasker-3.2.2/maptasker/src/initparg.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Intialize command line interface/runtime arguments for MapTasker"""
+
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
 # initparg: intialize command line interface/runtime arguments for MapTasker           #
 #                                                                                      #
 # GNU General Public License v3.0                                                      #
 # Permissions of this strong copyleft license are conditioned on making available      #
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
-from maptasker.src.config import ANDROID_IPADDR, ANDROID_PORT, ANDROID_FILE, OUTPUT_FONT
+from maptasker.src.config import ANDROID_FILE, ANDROID_IPADDR, ANDROID_PORT, OUTPUT_FONT
 
 
 #######################################################################################
 # Initialize Program runtime arguments to default values
 # ##################################################################################
 # Command line parameters
 def initialize_runtime_arguments() -> dict:
@@ -42,17 +43,16 @@
         "font": OUTPUT_FONT,  # Font to use in the output
         "gui": False,  # Use the GUI to get the runtime and color options
         "highlight": False,  # Highlight Project/Profile?Task/Scene names
         "indent": 4,  # Backup file was fetched from Android device
         "italicize": False,  # Italicise Project/Profile?Task/Scene names
         "outline": False,  # Outline Project/Profile?Task/Scene names
         "rerun": False,  # Is this a GUI re-run?
-        "restore": False,  # Restore settings from a previous run
+        "reset": False,  # Reset settings to default values
         "runtime": False,  # Display the runtime arguments/settings
-        "save": False,  # Save settings for reuse
         "single_profile_name": "",  # Display single Profile name only
         "single_project_name": "",  # Display single Project name only
         "single_task_name": "",  # Display single Task name only
         "twisty": False,  # Add Task twisty "▶︎" clickable icons for Task details
         "underline": False,  # Underline Project/Profile?Task/Scene names
-        "reset": False,  # Reset settings to default values
+        "pretty": False,  # Pretty up the output (takes many more output lines)
     }
```

### Comparing `maptasker-2.6.3/maptasker/src/kidapp.py` & `maptasker-3.2.2/maptasker/src/kidapp.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,21 +9,24 @@
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
 import defusedxml.ElementTree  # Need for type hints
 
+from maptasker.src.primitem import PrimeItems
+
 
 def get_kid_app(element: defusedxml.ElementTree) -> str:
     """
     Get any associated Kid Application info and return it
         :param element: root element to search for <Kid>
         :return: the Kid App info
     """
+    blank = "&nbsp;"
     kid_features = kid_plugins = ""
     four_spaces = "&nbsp;&nbsp;&nbsp;&nbsp;"
     kid_element = element.find("Kid")
     if kid_element is None:
         return ""
 
     kid_package = kid_element.find("pkg").text
@@ -39,12 +42,18 @@
             kid_plugins = f" {kid_plugins}{num_plugin+1}={item.text}, "
             num_plugin += 1
     if kid_features:
         kid_features = f"<br>{four_spaces}Features:{kid_features[:len(kid_features)-2]}"
     if kid_plugins:
         kid_plugins = f"<br>{four_spaces}Plugins:{kid_plugins[:len(kid_plugins)-2]}"
 
-    return (
+    kid_app_info = (
         f"<br>&nbsp;&nbsp;&nbsp;[Kid App Package:{kid_package}, Version"
         f" Name:{kid_version}, Target Android"
         f" Version:{kid_target} {kid_features} {kid_plugins}]"
     )
+
+    if PrimeItems.program_arguments["pretty"]:
+        number_of_blanks = kid_app_info.find("Package:") - 4
+        kid_app_info = kid_app_info.replace(",", f"<br>{blank*number_of_blanks}")
+
+    return kid_app_info
```

### Comparing `maptasker-2.6.3/maptasker/src/lineout.py` & `maptasker-3.2.2/maptasker/src/lineout.py`

 * *Files 22% similar despite different names*

```diff
@@ -41,31 +41,50 @@
 
 # ##################################################################################
 # Class definition for our output lines
 # ##################################################################################
 class LineOut:
     """Class definition for our output lines"""
 
-    def __init__(self) -> None:  # noqa: ANN101
+    def __init__(self) -> None:
         """
         Initialize an object
         Args:
             self: The object being initialized
         Returns:
             None: Nothing is returned
         - Initialize an empty list to store output lines
         - The list will be used to store lines of text as the object is used"""
         self.output_lines = []
 
     def refresh_our_output(
-        self,  # noqa: ANN101
+        self,
         include_the_profile: bool,
         project_name: str,
         profile_name: str,
     ) -> None:
+        """self.add_line_to_output(
+                2,
+                f"Project: {project_name}",
+                ["", "project_color", FormatLine.add_end_span],
+            )
+        Refreshes the output by clearing existing output and starting anew.
+        Parameters:
+            include_the_profile (bool): Flag to indicate whether this is a Profile to be included.
+            project_name (str): Name of the Project, if any.
+            profile_name (str): Name of the Profile, if any.
+        Returns:
+            - None: No return value.
+        Processing Logic:
+            - Clears existing output and starts anew.
+            - Adds directory item.
+            - Starts Project list.
+            - Checks if Profile is to be included.
+            - Starts Profile list.
+            - Starts Project list."""
         """
         For whatever reason, we need to clear out the existing output and start anew.
 
                 :param include_the_profile: Boolean flag to indicate whether this is
                     a Profile to be included
                 :param project_name: name of the Project, if any
                 :param profile_name: name of the Profile, if any
@@ -78,22 +97,14 @@
             "current_item": "",
             "projects": [],
             "profiles": [],
             "tasks": [],
             "scenes": [],
         }
 
-        PrimeItems.scene_countgrand_totals = {
-            "projects": 0,
-            "profiles": 0,
-            "unnamed_tasks": 0,
-            "named_tasks": 0,
-            "scenes": 0,
-        }
-
         PrimeItems.grand_totals = {
             "projects": 0,
             "profiles": 0,
             "unnamed_tasks": 0,
             "named_tasks": 0,
             "scenes": 0,
         }
@@ -123,58 +134,116 @@
             )
             # Start Project list
             self.add_line_to_output(1, "", FormatLine.dont_format_line)
 
     # ##################################################################################
     # Generate an updated output line with HTML style details
     # Input is a dictionary containing the requirements:
-    #  color1 - color to user
-    #  color2 - optional 2nd color to use
-    #  color3 - optional third color to tack onto end of string
-    #  is_list - boolean: True= is a list HTML element
-    #  span - boolean: True= requires a <span> element
-    #  font - font to use
+    #  color - color to user
+    #  tab - CSS tab to use
+    #  font - the m,onospace font to use
+    #  element - the actual output line
     # ##################################################################################
     def add_style(self, style_details: dict) -> str:
         """
         Add appropriate HTML style tags based on parameters in dictionary passed in
             :param style_details: True if we are to output a list (<li>), False if not
             :return: updated output line with style details added
         """
 
         line_with_style = ""
-        if style_details["is_list"]:
-            line_with_style = f'<li "<span class="{style_details["color"]}">{style_details["element"]}</span></li>\n'
+        if style_details["tab"]:
+            # Note: add <div> to force a divisional block so any text wraparound stays within the block of text.
+            line_with_style = f'<div><span class="{style_details["color"]} {style_details["tab"]}">{style_details["element"]}</span></div>\n'
 
         elif style_details["is_taskernet"]:
-            line_with_style = f'<p class="{style_details["color"]}{style_details["element"]}</p>\n'
+            line_with_style = (
+                f'<p class="{style_details["tab"]} {style_details["color"]}>{style_details["element"]}</p><br>\n'
+            )
             line_with_style = line_with_style.replace("<span></span>", "")
 
         return line_with_style
 
     # ##################################################################################
+    #  Adds a directory link to the provided string.
+    # ##################################################################################
+    def add_directory_link(self, arg1: str, element: str, arg3: str) -> str:
+        """
+        Adds a directory link to the provided string.
+        Args:
+            self: The class instance
+            arg1: First part of the string
+            element: Middle part of the string
+            arg3: Last part of the string
+        Returns:
+            String: The full string with directory link added if applicable
+        Processes the function:
+            - Checks if a directory is specified in arguments
+            - Gets the current directory item if set
+            - Generates the directory link HTML
+            - Concatenates all parts and returns the full string
+        """
+        directory = ""
+
+        if PrimeItems.program_arguments["directory"] and PrimeItems.directory_items["current_item"]:
+            directory_item = f'"{PrimeItems.directory_items["current_item"]}"'
+            directory = f"<a id={directory_item}></a>\n"
+        return f"{directory}{arg1}{element}{arg3}"
+
+    # ##################################################################################
+    # Find the color attribute/class and add the tab attribute to it.
+    # ##################################################################################
+    def add_tab(self, tab: str, element: str) -> str:
+        r"""
+
+        This function adds a tab before the substring "_color" in a given element string.
+
+        Parameters:
+        - tab (str): The tab to be added before the "_color" substring.
+        - element (str): The element string in which the tab should be added before "_color".
+
+        Returns:
+        - str: The modified element string with the tab added before "_color".
+
+        Processing Logic:
+        - Find the position of the "_color" substring in the element string.
+        - Insert a tab before the "_color" substring using string slicing and concatenation.
+        - Return the modified element string.
+
+        Examples:
+        - Example usage of the function:
+
+            # Calling the function with tab = "\t" and element = 'background_color:"red"'
+            add_tab("\t", 'background_color:"red"')
+            # Output: '\tbackground_color "red"'
+
+        """
+        color_pos = element.find('_color"')
+        return f'{element[0:color_pos]}_color {tab}"{element[(color_pos+7):]}'
+
+    # ##################################################################################
     # Given a text string to output, format it based on it's contents:
     #   Project/Profile/Task/Actrion/Scene
     # ##################################################################################
-    def format_line_list_item(self, element: str) -> str:  # noqa: ANN101
+    def format_line_list_item(self, element: str) -> str:
         """
         Generate the output list (<li>) string based on the input XML <code> passed in
 
         :param element: text string to be added to output
         :return: the formatted text to add to the output queue
         """
 
         font = PrimeItems.program_arguments["font"]
         if "Project:" in element or "Project has no Profiles" in element:
             return self.handle_project(element)
 
         if "Profile:" in element:
             return self.handle_profile(element)
 
-        if element.startswith("Task:") or "&#45;&#45;Task:" in element:
+        if element.startswith("Task:") or "&#45;&#45;Task:" in element or "Task: Properties" in element:
             return self.handle_task(element, font)
 
         if element.startswith("Scene:"):
             return self.handle_scene(element, font)
 
         if "Action:" in element:
             return self.handle_action(element)
@@ -184,182 +253,228 @@
 
         # Must be additional item
         return self.handle_additional(element)
 
     # ##################################################################################
     # Insert the hyperlink target if doing a the directory
     # ##################################################################################
-    def handle_project(self, element: str) -> str:  # noqa: ANN101
+    def handle_project(self, element: str) -> str:
         """
         Insert the hyperlink target if doing a the directory
                 Args:
 
                     element (str): text to incorporate after the target
 
                 Returns:
                     _type_: output text with hyperlink target embedded
         """
-        return self.add_directory_link("<li ", element, "</li>\n")
+        element = self.add_tab("projtab", element)
+        return self.add_directory_link("<br>", element, "\n")
 
-    def handle_profile(self, element: str) -> None:  # noqa: ANN101
+    # ##################################################################################
+    # Handles profile element by adding directory link
+    # ##################################################################################
+    def handle_profile(self, element: str) -> None:
         """Handles profile element by adding directory link
         Args:
             element: Profile element to handle
         Returns:
             str: Formatted profile element with directory link
         - Adds opening and closing tags for list item
         - Calls method to add directory link
         - Returns formatted string"""
-        return self.add_directory_link("<br><li ", element, "</span></li>\n")
+        element = self.add_tab("proftab", element)
+        # Add the directory link to the Profile line.
+        # Add <div </div> to ensure line wrap breaks at proftab (Profile spacing)
+        return self.add_directory_link("<br><div ", element, "</div><br>\n")
 
     # ##################################################################################
-    #  Adds a directory link to the provided string.
+    # Handle styling for a task element
     # ##################################################################################
-    def add_directory_link(self, arg1: str, element: str, arg3: str) -> str:  # noqa: ANN101
-        """
-        Adds a directory link to the provided string.
-        Args:
-            self: The class instance
-            arg1: First part of the string
-            element: Middle part of the string
-            arg3: Last part of the string
-        Returns:
-            String: The full string with directory link added if applicable
-        Processes the function:
-            - Checks if a directory is specified in arguments
-            - Gets the current directory item if set
-            - Generates the directory link HTML
-            - Concatenates all parts and returns the full string
-        """
-        directory = ""
-
-        if PrimeItems.program_arguments["directory"] and PrimeItems.directory_items["current_item"]:
-            directory_item = f'"{PrimeItems.directory_items["current_item"]}"'
-            directory = f"<a id={directory_item}></a>\n"
-        return f"{directory}{arg1}{element}{arg3}"
-
-    def handle_task(self, element: str, font: str) -> str:  # noqa: ANN101
+    def handle_task(self, element: str, font: str) -> str:
         """Handle styling for a task element
         Args:
             element: Element name in one line
             font: Font name in one line
         Returns:
             style_details: Styled element details in one line
         Processing Logic:
             - Check if element name contains UNKNOWN_TASK_NAME
             - Set color to "unknown_task_color" if true else "task_color"
             - Add font and element details to style
             - Return styled element from add_style method"""
         style_details = {
-            "is_list": True,
+            "tab": "tasktab",
             "font": font,
             "element": element,
             "color": ("unknown_task_color" if UNKNOWN_TASK_NAME in element else "task_color"),
         }
+
+        # Note: add <div> to force a divisional block so any text wraparound stays within the block of text.
         return self.add_style(style_details)
 
-    def handle_scene(self, element, font):
+    # ##################################################################################
+    # Handle Scene
+    # ##################################################################################
+    def handle_scene(self, element: str, font: str) -> str:
+        r"""
+        This function handles a scene element by generating a string with HTML tags and style details. The function takes two parameters: element and font.
+
+        Parameters:
+        - element (str): The scene element that needs to be processed.
+        - font (str): The font to use for the scene element.
+
+        Returns:
+        - str: The processed string with HTML tags and style details.
+
+        Processing Logic:
+        - If the program_arguments "directory" and the directory_items "current_item" are both true, the function extracts the scene name from the element and assigns it to the variable scene_name.
+        - It then checks if any of the program_arguments "bold", "italicize", "highlight", or "underline" are true. If any of them are true, it calls the remove_html_tags() function to remove any name attributions from the scene name.
+        - The function assigns an empty string to the variable directory if the program_arguments "directory" and the directory_items "current_item" are both false.
+        - The function then creates a dictionary called style_details with details about the style of the scene element.
+        - It finally returns a formatted string with the directory and the result of calling the add_style() function with the style_details dictionary.
+
+        Examples:
+        - Example usage of the function:
+            handle_scene('Scene:&nbsp;1', 'Arial')
+            # Returns: '<a id="scenes_1"></a>\n<style=color:scene_color;font:Arial;element:Scene:&nbsp;1;>'
+        """
         directory = ""
         if PrimeItems.program_arguments["directory"] and PrimeItems.directory_items["current_item"]:
             scene_name = f'scenes_{element.split("Scene:&nbsp;")[1]}'
             # Get rid of any name attributions
             if (
                 PrimeItems.program_arguments["bold"]
                 or PrimeItems.program_arguments["italicize"]
                 or PrimeItems.program_arguments["highlight"]
                 or PrimeItems.program_arguments["underline"]
             ):
                 scene_name = remove_html_tags(scene_name, "")
-                # scene_name = self.remove_attributes(scene_name)
+
             directory = f'<a id="{scene_name.replace(" ","_")}"></a>\n'
         style_details = {
-            "is_list": True,
+            "tab": "scenetab",
             "color": "scene_color",
             "font": font,
             "element": element,
         }
-        return f"{directory}{self.add_style(style_details)}"
+
+        # Note: add <div> to force a divisional block so any text wraparound stays within the block of text.
+        return f"{directory}<br><div>{self.add_style(style_details)}</div>"
 
     # def remove_attributes(self, scene_name):
     #     scene_name = scene_name.replace("<em>", "")
     #     scene_name = scene_name.replace("</em>", "")
     #     scene_name = scene_name.replace("<b>", "")
     #     scene_name = scene_name.replace("</b>", "")
     #     scene_name = scene_name.replace("<mark>", "")
     #     scene_name = scene_name.replace("</mark>", "")
     #     scene_name = scene_name.replace("<u>", "")
     #     scene_name = scene_name.replace("</u>", "")
     #     return scene_name
 
-    def handle_action(self, element):
+    # ##################################################################################
+    # Handles the action element.
+    # ##################################################################################
+    def handle_action(self, element: str) -> str:
         """
-        Handles the action element.
+        This function handles an action element by processing its contents and formatting it into HTML code.
 
-        Args:
-            element: The action element to be handled.
+        Parameters:
+        - self: The object reference to the class instance.
+        - element (str): The action element that needs to be processed.
 
         Returns:
-            The formatted HTML list item element.
+        - str: The formatted HTML code for the action element.
+
+        Processing Logic:
+        - First, the function generates the necessary number of whitespace characters for indentation.
+        - If the action element starts with "Action: ...", it checks for a continuation line.
+        - If there is a continuation line, it splits the element into the indentation level and the remaining part of the line.
+        - If the indentation level is 0, it sets an indentation of 5 spaces.
+        - Otherwise, it sets the indentation based on the specified level.
+        - It then replaces the "Action: ..." part of the line with the indentation and the continuation indicator.
+        - Finally, it formats the element into HTML code by adding a class and line break.
 
         Examples:
-            >>> handle_action(self, "Action: ...indent=2item=Attribute")
-            '<li ...">continued >>> Attribute</span></li>\n'
-        """
+        - Usage of the function:
 
-        blanks = f'{"&nbsp;"*PrimeItems.program_arguments["indent"]}&nbsp;&nbsp;&nbsp;'
+            handler = ActionHandler()
+            element = "Action: ...indent=2item=Attribute"
+            formatted_element = handler.handle_action(element)
+            print(formatted_element)
+
+            Output:
+            <span class="actiontab"></span><span class="indentation">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;continued >>> Attribute</span><br>
+        """
+        blank = "&nbsp;"
+        # Is this a continuation line?
         if "Action: ..." in element:
-            if element[11:] == "":
+            if element[11:] == "":  # This catches valid lines that have "Action: ..." in them
                 return ""
             # We have a continuation line: Action: ...indent=nitem=remaindertheline
             # Example:
             # '<span ...">Action: ...indent=2item=Attribute</span><span ...</span>>'
             start1 = element.split("indent=")
-            start2 = start1[1].split("item=")
+            start2 = start1[1].split("item=")  # Indentation amount
             # Force an indent of at least 1
-            if start2[0] == "0":
-                indentation = f'{"&nbsp;"*5}'
-            else:
-                indentation = f'{blanks*int(start2[0])}{"&nbsp;"*int(start2[0])}&nbsp;'
+            indentation = f"{'&nbsp;' * 5}" if start2[0] == "0" else f"{blank * (int(start2[0]) + 8)}"
             # Add indentation for contination line
             tmp = start1[0].replace("Action: ...", f"{indentation}continued >>> {start2[1]}")
-            # tmp = action_evaluate.cleanup_the_result(
-            #     start1[0].replace(
-            #         "Action: ...", f"{indentation}continued >>> {start2[1]}"
-            #     )
-            # )
+
             element = tmp
-        return f"<li {element}</span></li>\n"
 
-    def handle_taskernet(self, element):
+        # Add action tab to existing class.
+        element = self.add_tab("actiontab", element)
+
+        # Note: add <div> to force a divisional block so any text wraparound stays within the block of text.
+        return f"<div {element}</span></div><br>\n"
+
+    # ##################################################################################
+    # Handle taskernet
+    # ##################################################################################
+    def handle_taskernet(self, element: str) -> str:
+        r"""
+        This function handles a taskernet by appending a given element to a new line.
+
+        Parameters:
+        - element (str): The element to be added to the taskernet.
+
+        Returns:
+        - str: The taskernet with the given element appended to a new line.
+
+        Processing Logic:
+        - The function takes in a string representing an element.
+        - It appends the element to a new line using the '\n' character.
+        - The modified taskernet is then returned.
+
+        Examples:
+        - Example usage of the function:
+
+            handle_taskernet("Task 1")
+            Output: "Task 1\n"
+            Explanation: The function appends the element "Task 1" to a new line and returns it as a taskernet.
+        """
         return f"{element}\n"
 
-    def handle_additional(self, element):
-        return f"<li {element}" + "</span></li>\n"
+    # ##################################################################################
+    # Handle additional elements and return a formatted list item string.
+    # ##################################################################################
+    def handle_additional(self, element: str) -> str:
+        """
+        Handle additional elements and return a formatted list item string.
 
-    def end_unordered_list(self):
-        if PrimeItems.unordered_list_count > 0:
-            PrimeItems.unordered_list_count -= 1
-        return "</ul>" if PrimeItems.unordered_list_count >= 0 else ""
-
-    def delete_last_line(self):
-        # self.my_traceback("3", f"delete last element:{self.output_lines[-1]}")
-        if PrimeItems.unordered_list_count > 0:
-            if self.output_lines[-1] == "</ul>":
-                PrimeItems.unordered_list_count += 1
-            else:
-                PrimeItems.unordered_list_count -= 1
-        self.output_lines[-1] = ""
-
-    def my_traceback(self, key, element):
-        import sys
-        import traceback
-
-        print(f"--------------------------- Traceback:{key}", file=sys.stderr)
-        print(element, file=sys.stderr)
-        traceback.print_stack()
+        Parameters:
+            self: The instance of the class.
+            element: The element to be added to the list item string.
+
+        Returns:
+            A formatted list item string with the provided element.
+        """
+        return element
 
     # ##################################################################################
     # Generate the output string based on the input XML <code> passed in
     # Returns a formatted string for output based on the input codes
     # ##################################################################################
     def format_line_out(self, element: str, lvl: int) -> str:
         """
@@ -369,33 +484,37 @@
                     1=start list, 2= list item, 3= end list, 4= plain text
                 :return: modified output line
 
         """
 
         if lvl == 0:
             # Heading / break
-            return f"{element}<br>"
+
+            return f'<span class="normtab"></span>{element}<br>'
+
+            # return f'<div <span class="normtab"></span>{element}</div><br>'
 
         if lvl == 1:
             # Start list
-            return f"<ul>{element}\n"
+            return f"{element}\n"
 
         if lvl == 2:
             # List item
             if PrimeItems.program_arguments["twisty"] and "Scene:" in element:
-                return f"<ul>{self.format_line_list_item(element)}"
+                return f"{self.format_line_list_item(element)}"
             return self.format_line_list_item(element)
 
         if lvl == 3:
             # End list
-            return PrimeItems.output_lines.end_unordered_list()
+            return ""
 
         if lvl == 5:
             # Plain text
             return f"{element}\n"
+        return element
 
     # ##################################################################################
     # Write line of output
     # ##################################################################################
     def add_line_to_output(
         self,
         list_level: int,
@@ -411,35 +530,33 @@
                 adding HTML to it. Empty if we are not to first format the line.
                 format_line[0] = text_before: The text to add before out_string.
                 format_line[1] = color_to_use: The color to use if formatting line
                 format_line[2] = add_span: Boolean to determine if a <span> tag
                     should be added if formatting the line.
             :return: none
         """
-
         # Format the output line by adding appropriate HTML.
         if format_line != FormatLine.dont_format_line:
             out_string = format_html(
-                format_line[1],
-                format_line[0],
-                out_string,
-                format_line[2],
+                format_line[1],  # Color code
+                format_line[0],  # Text before.
+                out_string,  # Text after.
+                format_line[2],  # End span True or False
             )
 
         # Drop ID: nnn since we don't need it anymore
         if "Task ID:" in out_string and PrimeItems.program_arguments["debug"] is False:
             temp_element = out_string.split("Task ID:")
             out_string = temp_element[0]
 
         # Go configure the output based on the contents of the element and the
         #   list level. Call format_line before appending it.
         self.output_lines.append(
             self.format_line_out(
                 out_string,
                 list_level,
-            )
+            ),
         )
         # Log the generated output if in special debug mode
         if debug_out:
             debug_msg = f"out_string: {self.output_lines[-1]}"
             logger.debug(debug_msg)
-        return
```

### Comparing `maptasker-2.6.3/maptasker/src/mapit.py` & `maptasker-3.2.2/maptasker/src/mapit.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 #  $$ | \_/ $$ |\$$$$$$$ |$$$$$$$  |         $$ |\$$$$$$$ |$$$$$$$  |$$ | \$$\ \$$$$$$$\ $$ |
 #  \__|     \__| \_______|$$  ____/          \__| \_______|\_______/ \__|  \__| \_______|\__|
 #                         $$ |
 #                         $$ |
 #                         \__|
 
 """
-    This is the main coordinator module that imports all the other components and
-    executes the key steps to take the Tasker backup and produce the visual map output.
+This is the main coordinator module that imports all the other components and
+executes the key steps to take the Tasker backup and produce the visual map output.
 """
 
 # #################################################################################### #
 #                                                                                      #
 # mapit: Main Program                                                                  #
 #            Read the Tasker backup file to build a visual map of its configuration:   #
 #            Projects, Profiles, Tasks, Scenes                                         #
@@ -39,14 +39,16 @@
 # Reference: https://github.com/Taskomater/Tasker-XML-Info                             #
 #                                                                                      #
 # #################################################################################### #
 
 import contextlib
 import gc
 import os
+import platform
+import subprocess
 import sys
 import webbrowser
 from subprocess import run
 
 import maptasker.src.proginit as initialize
 import maptasker.src.taskuniq as special_tasks
 from maptasker.src import projects
@@ -57,16 +59,17 @@
 from maptasker.src.getputer import save_restore_args
 from maptasker.src.globalvr import get_variables, output_variables
 from maptasker.src.initparg import initialize_runtime_arguments
 from maptasker.src.lineout import LineOut
 from maptasker.src.outline import outline_the_configuration
 from maptasker.src.primitem import PrimeItems, PrimeItemsReset
 from maptasker.src.sysconst import (
+    NORMAL_TAB,
     Colors,
-    DISPLAY_DETAIL_LEVEL_everything,
+    DISPLAY_DETAIL_LEVEL_all_variables,
     FormatLine,
     debug_file,
     debug_out,
     logger,
 )
 
 # print('Path:', os.getcwd())
@@ -105,27 +108,27 @@
         - Write detailed crash report to debug log file
         - Redirect print/stderr to log for detailed crash information
     """
     if crash_debug:
         # sys.__excepthook__ is the default excepthook that prints the stack trace
         # So we use it directly if we want to see it
         sys.__excepthook__(exctype, value, traceback)
-        print("MapTasker encountered a runtime error!  Error can be found in maptasker_debug.log")  # noqa: T201
-        print("]\nGo to https://github.com/mctinker/Map-Tasker/issues to report the problem.\n")  # noqa: T201
+        print("MapTasker encountered a runtime error!  Error can be found in maptasker_debug.log")
+        print("]\nGo to https://github.com/mctinker/Map-Tasker/issues to report the problem.\n")
     # Give the user a more graceful error message.
     else:
         # Instead of the stack trace, we print an error message to stderr
-        print("\nMapTasker encountered a runtime error!", file=sys.stderr)  # noqa: T201
+        print("\nMapTasker encountered a runtime error!", file=sys.stderr)
         # print("Exception type:", exctype, " value:", value)
-        print(f"The error log can be found in {debug_file}.")  # noqa: T201
-        print(  # noqa: T201
+        print(f"The error log can be found in {debug_file}.")
+        print(
             "Go to https://github.com/mctinker/Map-Tasker/issues to report the problem.\n",
             file=sys.stderr,
         )
-        print("\a", end="", flush=True)  # noqa: T201
+        print("\a", end="", flush=True)
         # Redirect print to a debug log
         with open(debug_file, "w") as log:
             # sys.stdout = log
             sys.stderr = log
             sys.__excepthook__(exctype, value, traceback)
 
 
@@ -173,17 +176,17 @@
     write_out_the_file: we have a list of output lines.  Write them out.
         :param my_output_dir: directory to output to
         :param my_file_name: name of file to use
         :return: nothing
     """
     logger.info(f"Function Entry: write_out_the_file dir:{my_output_dir}")
     output_file = f"{my_output_dir}{my_file_name}"
-    with open(output_file, "w") as out_file:
+    with open(output_file, "w", encoding="utf-8") as out_file:
         # Output the rest that is in our output queue
-        for num, item in enumerate(PrimeItems.output_lines.output_lines):
+        for item in PrimeItems.output_lines.output_lines:
             # Check to see if this is where the directory is to go in the
             # Output directory. if so, output_directory will create it's own list of
             # output lines.
             if "maptasker_directory" in item:
                 # Temporarily save our output lines
                 temp_lines_out = PrimeItems.output_lines.output_lines
                 PrimeItems.output_lines.output_lines = []  # Create a new output queue
@@ -196,15 +199,15 @@
                     out_file.write(output_line)
                 # Restore our regular output
                 PrimeItems.output_lines.output_lines = temp_lines_out
                 continue
 
             # Format the output line
             # logger.info(item)
-            output_line = format_line(PrimeItems.output_lines, num, item)
+            output_line = format_line(item)
             # Continue if we are to ignore this output line.
             if not output_line:
                 continue
 
             # Parse twisty <details>...yield result
             with contextlib.suppress(ValueError):
                 details_position = output_line.index("<details>")
@@ -216,14 +219,16 @@
             if output_line.strip():  # Write out if not blank
                 logger.info(f"Writing: {output_line}")
                 out_file.write(output_line)
             if debug_out:
                 logger.debug(f"mapit output line:{output_line}")
                 logger.info("Function Exit: write_out_the_file")
 
+        os.fsync(out_file)  # Force write to disk
+
 
 # ##################################################################################
 # Cleanup memory and let user know there was no match found for Task/Profile
 # ##################################################################################
 def clean_up_and_exit(
     name: str,
     profile_or_task_name: str,
@@ -248,33 +253,39 @@
 # Output grand totals
 # ##################################################################################
 def output_grand_totals() -> None:
     """
     Output the grand totals of Projects/Profiles/Tasks/Scenes
     """
     grand_total_projects = PrimeItems.grand_totals["projects"]
+    if PrimeItems.program_arguments["single_project_name"] or PrimeItems.program_arguments["single_profile_name"]:
+        grand_total_projects = 1
     grand_total_profiles = PrimeItems.grand_totals["profiles"]
+    if PrimeItems.program_arguments["single_profile_name"]:
+        grand_total_profiles = 1
     grand_total_unnamed_tasks = PrimeItems.grand_totals["unnamed_tasks"]
     grand_total_named_tasks = PrimeItems.grand_totals["named_tasks"]
+    if PrimeItems.program_arguments["single_task_name"]:
+        grand_total_named_tasks = 1
     grand_total_scenes = PrimeItems.grand_totals["scenes"]
     # If doing a directory, then add id to hyperlink to.
     if PrimeItems.program_arguments["directory"]:
         PrimeItems.output_lines.add_line_to_output(
             5,
             '<a id="grand_totals"></a>',
             FormatLine.dont_format_line,
         )
 
     total_number = "Total number of "
     PrimeItems.output_lines.add_line_to_output(
         1,
         (
-            f"<br><hr>Tasker Totals...<br>{total_number}Projects: {grand_total_projects}<br>{total_number}Profiles:  {grand_total_profiles}<br>{total_number}Tasks:"
+            f"<br><hr>{NORMAL_TAB}Tasker Displayed Totals...<br>{NORMAL_TAB}{total_number}Projects: {grand_total_projects}<br>{NORMAL_TAB}{total_number}Profiles:  {grand_total_profiles}<br>{NORMAL_TAB}{total_number}Tasks:"
             f" {grand_total_unnamed_tasks + grand_total_named_tasks} ({grand_total_unnamed_tasks} unnamed,"
-            f" {grand_total_named_tasks} named)<br>{total_number}Scenes:"
+            f" {grand_total_named_tasks} named)<br>{NORMAL_TAB}{total_number}Scenes:"
             f" {grand_total_scenes}<br><br>"
         ),
         ["", "trailing_comments_color", FormatLine.add_end_span],
     )
     PrimeItems.output_lines.add_line_to_output(3, "", FormatLine.dont_format_line)
 
 
@@ -283,14 +294,19 @@
 # ##################################################################################
 def initialize_everything() -> dict:
     """
     Set up all the variables and logic in case program craps out
         :return: dictionary of primary items used throughout project, and empty staring
     """
 
+    # Check to see if we might be coming from another program (e.g. run_test.py).
+    # If so, re-initialize PrimeItems since it is still carrying the values from the last test/run.
+    if PrimeItems.colors_to_use:
+        PrimeItemsReset()
+
     # We have to initialize output_lines here. Otherwise, we'll lose the output class
     # with the upcoming call to start_up.
     PrimeItems.output_lines = LineOut()
 
     # Get colors to use, runtime arguments etc...all of our primary items we need
     # throughout
     initialize.start_up()
@@ -363,26 +379,26 @@
     Display the output in the default web browser,
     Args:
         my_output_dir (str): The directory to our current file path.
         my_file_name (str): The name of the file to open.
     """
     logger.debug("MapTasker program ended normally")
     try:
-        webbrowser.open(f"file://{my_output_dir}{my_file_name}", new=2)
+        webbrowser.open(f"file:{PrimeItems.slash*2}{my_output_dir}{my_file_name}", new=2)
     except webbrowser.Error:
         error_handler("Error: Failed to open output in browser: your browser is not supported.", 1)
-    print("")  # noqa: T201
+    print("")
 
     # If doing the outline, let 'em know about the map file.
     map_text = (
         "The Configuration Map was saved as MapTasker_Map.txt.  " if PrimeItems.program_arguments["outline"] else ""
     )
 
-    print(f"{Colors.Green}You can find 'MapTasker.html' in the current folder.  {map_text}Program end.")  # noqa: T201
-    print("")  # noqa: T201
+    print(f"{Colors.Green}You can find 'MapTasker.html' in the current folder.  {map_text}Program end.")
+    print("")
 
 
 # ##################################################################################
 # Output the configuration outline and map
 # ##################################################################################
 def process_outline() -> None:
     """
@@ -401,17 +417,22 @@
     Output the configuration outline and map
         Args:
             my_output_dir (str): Our current directory for output.
     """
     # Do the configuration outline and generate the map
     outline_the_configuration()
 
-    # Display the map in the first available text editor
+    # Display the diagram in the default text editor.
     with contextlib.suppress(FileNotFoundError):
-        run(["open", "MapTasker_map.txt"], check=False)  # noqa: S607, S603
+        # Asterisk before sys.argv breaks it into separate arguments
+        if platform.system() == "Windows":
+            directory = os.getcwd()
+            os.startfile(f"{directory}{PrimeItems.slash}MapTasker_map.txt")
+        else:
+            run(["open", "MapTasker_map.txt"], check=False)  # noqa: S607, S603
 
 
 # ##################################################################################
 # Check if doing a single item and if not found, then clean up and exit
 # ##################################################################################
 def check_single_item(
     single_project_name: str,
@@ -475,15 +496,15 @@
         - Clean up and exit if single item not found
         - Display program caveats
         - Finalize HTML
         - Write output file
         - Clean up memory
         - Display output file in browser
     """
-    if program_arguments["display_detail_level"] == DISPLAY_DETAIL_LEVEL_everything:
+    if program_arguments["display_detail_level"] >= DISPLAY_DETAIL_LEVEL_all_variables:
         output_variables("Unreferenced Global Variables", "")
 
     # Get the output directory/folder path
     my_output_dir = os.getcwd()
 
     # Output the Configuration Outline
     if program_arguments["outline"]:
@@ -514,36 +535,53 @@
             f"{Colors.Yellow}MapTasker cancelled.  An error occurred.  Program cancelled.",
             0,
         )
         clean_up_memory()
         sys.exit(2)
 
     # Finally, write out all of the output that is queued up.
-    my_file_name = "/MapTasker.html"
+    my_file_name = f"{PrimeItems.slash}MapTasker.html"
     write_out_the_file(my_output_dir, my_file_name)
 
     # Display the final results in the default web browser
     display_output(my_output_dir, my_file_name)
 
 
 # ##################################################################################
 # Re-launch our program via the "rerun" feature.
 # ##################################################################################
 def restart_program() -> None:
-    """Restarts the current program, with file objects and descriptors
-    cleanup
-    """
-    # Get the path of the python interpreter and use it to execute ourselves again.
-    python = sys.executable
-
-    # Restart our program (sys.argv[0])
+    # Restart our program
+    # sys.executable = the path of the python interpreter and use it to execute ourselves again.
+    """Restarts the program.
+    Parameters:
+        - None
+    Returns:
+        - None
+    Processing Logic:
+        - Use sys.executable to execute ourselves again.
+        - Use contextlib.suppress to ignore OSError.
+        - Use platform.system to check the system: Windows or Linux/UNix base.
+        - Use subprocess.run to run the program if Windows.
+        - Use os.execl to execute the program if not Windows.
+        - Use sys.exit to exit the program."""
+    # NOTE: execl is the preferred method to launch a new program, but it doesn't work on Windows.
+    #       So for Windows, we use subprocess.run.
+    #       'subprocess' does not immediately return from the call whereas 'execl' does return immediate control.
+    #
+    # sys.executable points to location of python: ../../python runtime
+    # Asterisk before sys.argv breaks it into separate arguments
     with contextlib.suppress(OSError):
-        # Asterisk before sys.argv breaks it into separate arguments
-        os.execl(python, python, *sys.argv)
-    sys.exit(0)
+        if platform.system() == "Windows":
+            subprocess.run([sys.executable, *sys.argv], check=False)  # noqa: S603
+        else:
+            # Start a new process which replaces our current process (it does not return).
+            os.execl(sys.executable, "python", *sys.argv)
+
+    sys.exit(0)  # This should never be called.
 
 
 # ##################################################################################
 # Handle "rerun" request
 # ##################################################################################
 def do_rerun() -> None:
     """
@@ -564,112 +602,38 @@
 
     # Now do it!  Rerun the program.
     with contextlib.suppress(KeyError):
         restart_program()
         # mapit_all(filename)
 
 
-########################################################################################
-#                                                                                      #
-#   Main Program Starts Here                                                           #
-#                                                                                      #
-########################################################################################
-"""
--The function 'mapit_all' is the main function of the MapTasker program, which maps the
-Tasker environment and generates an HTML output file.
-
-
-
-- The function initializes local variables and other necessary stuff.
-
-- It gets colors to use, runtime arguments, found items, and heading by calling the
-'start_up' function from the 'proginit' module.
-
-- It prompts the user to locate the Tasker backup XML file to use to map the Tasker
-environment.
-
-- It opens and reads the file by calling the 'open_and_get_backup_xml_file' function
-from the 'proginit' module.
-
-- It gets all the XML data by calling the 'get_the_xml_data' function from the 'taskerd'
-module.
-
-- It checks for a valid Tasker backup XML file.
-
-- It processes Tasker preferences and displays them if the 'display_preferences'
-argument is True.
-
-- It processes all projects and their profiles by calling the
-'process_projects_and_their_profiles' function from the 'projects' module.
-
-- If a specific project or profile is requested but not found, it exits the program by
-calling the 'clean_up_and_exit' function.
-
-- It looks for tasks that are not referenced by profiles and displays a total count.
-
-- It lists any projects without tasks and projects without profiles.
-
-- If a specific task is requested but not found, it exits the program by calling the
-'clean_up_and_exit' function.
-
-- It outputs caveats if the 'display_detail_level' argument is greater than or equal
-to 3.
-
-- It adds HTML complete code to the output.
-
-- It generates the actual output file and stores it in the current directory.
-
-- It cleans up memory by calling the 'clean_up_memory' function.
-
-- It displays the final output by opening the output file in the default browser.
-
-- It returns the exit code of the program.
-"""
-
-
-def mapit_all(file_to_get: str) -> int:
-    # Initialize variables and get the backup xml file
+# ##################################################################################
+# Do the cleanup stuff: check for single name, do unique situations, and display
+# back matter.
+# ##################################################################################
+def special_handling(found_tasks: list, projects_without_profiles: list, projects_with_no_tasks: list) -> None:
+    # Store single item details in local variables
     """
-    Maps all Projects, Profiles, Tasks and Scenes in a Tasker backup file
+    Processes special handling of found tasks, projects without profiles, and projects with no tasks.
 
     Args:
-        file_to_get (str): The Tasker backup file to process
-
+        found_tasks: list - List of found tasks
+        projects_without_profiles: list - List of projects without profiles
+        projects_with_no_tasks: list - List of projects with no tasks
     Returns:
-        int: 0
+        None
 
-    Processes Projects and their Profiles:
-        - Gets all Project and Profile variables
-        - Processes each Project and its associated Profiles
-        - Stores details of single selected Project, Profile or Task
-    Checks for single selected item and processes accordingly
-    Processes unique situations like Tasks not in Profiles and Projects without Profiles/Tasks
-    Cleans up memory after completing processing
+    Processing Logic:
+        - Store single item details in local variables
+        - Check if only looking for a single Project/Profile/Task
+        - Turn off directory temporarily to avoid duplicates
+        - Get list of tasks not called by profiles and projects without profiles/tasks
+        - Restore original directory setting
+        - Display back matter after processing projects, profiles, tasks, scenes
     """
-    (
-        found_tasks,
-        projects_without_profiles,
-        projects_with_no_tasks,
-    ) = initialize_everything()
-
-    # Set up file to read if it is passed in (via rerun)
-    if file_to_get:
-        PrimeItems.file_to_get = file_to_get
-
-    # Get all Tasker variables
-    if PrimeItems.program_arguments["display_detail_level"] == DISPLAY_DETAIL_LEVEL_everything:
-        get_variables()
-
-    # Process all Projects and their Profiles
-    found_tasks = projects.process_projects_and_their_profiles(
-        found_tasks,
-        projects_without_profiles,
-    )
-
-    # Store single item details in local variables
     program_arguments = PrimeItems.program_arguments
     single_project_name = program_arguments["single_project_name"]
     single_profile_name = program_arguments["single_profile_name"]
     single_task_name = program_arguments["single_task_name"]
     single_project_found = PrimeItems.found_named_items["single_project_found"]
     single_profile_found = PrimeItems.found_named_items["single_profile_found"]
     single_task_found = PrimeItems.found_named_items["single_task_found"]
@@ -707,19 +671,71 @@
         single_profile_name,
         single_task_name,
         single_project_found,
         single_profile_found,
         single_task_found,
     )
 
+
+########################################################################################
+#                                                                                      #
+#   Main Program Starts Here                                                           #
+#                                                                                      #
+########################################################################################
+def mapit_all(file_to_get: str) -> int:
+    # Initialize variables and get the backup xml file
+    """
+    Maps all Projects, Profiles, Tasks and Scenes in a Tasker backup file
+
+    Args:
+        file_to_get (str): The Tasker backup file to process
+
+    Returns:
+        int: 0
+
+    Processes Projects and their Profiles:
+
+
+        - Initialize everything
+
+        - Gets all Project and Profile variables
+        - Processes each Project and its associated Profiles
+        - Stores details of single selected Project, Profile or Task
+    Checks for single selected item and processes accordingly
+    Processes unique situations like Tasks not in Profiles and Projects without Profiles/Tasks
+    Cleans up memory after completing processing
+    """
+    (
+        found_tasks,
+        projects_without_profiles,
+        projects_with_no_tasks,
+    ) = initialize_everything()
+    if PrimeItems.error_code > 0:
+        sys.exit(PrimeItems.error_code)
+
+    # Set up file to read if it is passed in (via rerun)
+    if file_to_get:
+        PrimeItems.file_to_get = file_to_get
+
+    # Get all Tasker variables
+    if PrimeItems.program_arguments["display_detail_level"] >= DISPLAY_DETAIL_LEVEL_all_variables:
+        get_variables()
+
+    # Process all Projects and their Profiles
+    found_tasks = projects.process_projects_and_their_profiles(
+        found_tasks,
+        projects_without_profiles,
+    )
+
+    # Do special handling
+    special_handling(found_tasks, projects_without_profiles, projects_with_no_tasks)
+
     # Save our runtime settings for next time.
     _, _ = save_restore_args(PrimeItems.program_arguments, PrimeItems.colors_to_use, True)
 
     # Rerun this program if "Rerun" was selected from GUI
     # First get the filename as a string.
-    if program_arguments["rerun"]:
+    if PrimeItems.program_arguments["rerun"]:
         do_rerun()
-    # Just a "run".  Clean up and exit.
-    else:
-        clean_up_memory()
+    # Just exit.
 
     return 0
```

### Comparing `maptasker-2.6.3/maptasker/src/nameattr.py` & `maptasker-3.2.2/maptasker/src/nameattr.py`

 * *Files identical despite different names*

### Comparing `maptasker-2.6.3/maptasker/src/outline.py` & `maptasker-3.2.2/maptasker/src/outline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing action runner logic."""
+
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
 # outline: Output the Tasker configuration in outline format                           #
 #                                                                                      #
 # Permissions of this strong copyleft license are conditioned on making available      #
@@ -332,16 +333,15 @@
             project_name (str): name of the Project we are currently outlining
             profile_ids (list): liost of Profiles under this Project
             task_ids (list): liost of Tasks under this Project
             network (dict): Dictionary structure for our network
     """
     all_profiles_tasks = []
 
-    # Delete the <ul> inserted by get_ids for Profile
-    PrimeItems.output_lines.delete_last_line()
+    # Go thru all Profiles
     no_name_counter = 1
     for item in profile_ids:
         # Get the Profile element
         profile = PrimeItems.tasker_root_elements["all_profiles"][item]["xml"]
         # Get the Profile name
         if not (profile_name := PrimeItems.tasker_root_elements["all_profiles"][item]["name"]):
             profile_name = f"Anonymous#{no_name_counter!s}"
@@ -349,15 +349,14 @@
 
         # Doing all Projects or single Project and this is our Project...
         if (
             not PrimeItems.program_arguments["single_profile_name"]
             or PrimeItems.program_arguments["single_profile_name"] == profile_name
         ):
             # Add Profile to our network
-            # network[project_name][profile_name] = []
             profile_line = f"{blank*5}{arrow}{blank*2}Profile: {profile_name}"
             PrimeItems.output_lines.add_line_to_output(
                 0,
                 profile_line,
                 ["", "profile_color", FormatLine.add_end_span],
             )
 
@@ -413,15 +412,14 @@
         if not value["name"]:
             value["name"] = f"Anonymous#{no_name_counter!s}"
             no_name_counter += 1
 
         # From this point on, we only need to find Tasks by Name.  So create a dict of all Tasks by name.
         # PrimeItems.tasks_by_name[value["name"]] = {"id": key, "name": value["name"], "xml": value["xml"]}
         PrimeItems.tasks_by_name[value["name"]] = value
-        ...
 
 
 # ##################################################################################
 # Start outline beginning with the Projects
 # ##################################################################################
 def do_the_outline(network: dict) -> None:
     """
@@ -467,15 +465,15 @@
             # Get the Profile IDs for this Project and process them
             # True if we have Profiles for this Project
             if profile_ids := get_ids(True, project, project_name, []):
                 outline_profiles_tasks_scenes(project_name, profile_ids, task_ids, network)
 
             # No Profiles for Project
             if not profile_ids:
-                # End ordered list since lineout.py added a <ul> for Project
+                # Add blank line since lineout.py added a completion for Project
                 PrimeItems.output_lines.add_line_to_output(3, "", FormatLine.dont_format_line)
 
 
 # ##################################################################################
 # Outline the Tasker Configuration
 # ##################################################################################
 def outline_the_configuration() -> None:
```

### Comparing `maptasker-2.6.3/maptasker/src/parsearg.py` & `maptasker-3.2.2/maptasker/src/parsearg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MapTasker runtime argument parser"""
+
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
 # parsearg: MapTasker runtime argument parser                                          #
 #                                                                                      #
 # GNU General Public License v3.0                                                      #
@@ -19,18 +20,18 @@
 from tkinter import font
 
 from maptasker.src.error import error_handler
 from maptasker.src.maputils import validate_ip_address, validate_port
 from maptasker.src.nameattr import get_tk
 from maptasker.src.sysconst import TYPES_OF_COLORS, logger
 
-# class MutuallyInclusiveArgumentError(Exception):
-#     pass
-
 
+# ##################################################################################
+# Validate mutually inclusive variables
+# ##################################################################################
 def validate_vars(var1: str, var2: int, var3: str) -> None:
     """Validate mutually inclusive arguments
     Args:
         var1: First argument to validate
         var2: Second argument to validate
         var3: Third argument to validate
     Returns:
@@ -133,14 +134,16 @@
     # Get all monospace ("f"=fixed) fonts
     fonts = [font.Font(family=f) for f in font.families()]
     valid_fonts.extend(f.actual("family") for f in fonts if f.metrics("fixed"))
     if x != "help" and x not in valid_fonts:
         msg = f"Invalid or non-monospace font name '{x}'."
         error_handler(msg, 7)
         # raise argparse.ArgumentTypeError(msg)
+    elif x == "help":
+        print("Valid monospace fonts: ", ", ".join(valid_fonts))
     return x
 
 
 ################################################################################
 # Validate file location entered
 ################################################################################
 def file_validation(file: str) -> str:
@@ -284,46 +287,60 @@
             """ \
                         Level of detail to display:
                             0 = display simple Project/Profile/Task/Scene names only with no details
                             1 = display all Task action details for unknown Tasks only
                             2 = display full Task action name on every Task
                             3 = display full Task action details on every Task with action details (default)
                             4 = detail level 3 plus global variables
+                            5 = detail level 4 plus Scene element UI details.
                             Example: '-detail 2' for Task action names only
                             """,
         ),
-        choices=[0, 1, 2, 3, 4],
+        choices=[0, 1, 2, 3, 4, 5],
         required=False,
         type=int,
         nargs=1,
         default=3,
     )
     # Display directory
     parser.add_argument(
         "-directory",
         help="Display a directory of hotlinks for all Projects/Profiles/Tasks/Scenes.",
         action="store_true",
         default=False,
     )
+    # Group everrything and twisty
+    everything_group = parser.add_mutually_exclusive_group()
     # Display everything
-    parser.add_argument(
+    everything_group.add_argument(
         "-e",
         "-everything",
         help=textwrap.dedent(
             """ \
                         Display everything: full detail, Profile/Task conditions,
                         TaskerNet information, directory, etc..
                             """,
         ),
         action="store_true",
         default=False,
     )
+    # File to use for the input (e.g. ~/Downloads/backup.xml)
+    parser.add_argument(
+        "-file",
+        help=textwrap.dedent(
+            """ \
+                        Directory and file name of Tasker XML file to analyze.
+                        Example: -file ~/Downloads/backup.xml
+                            """,
+        ),
+        required=False,
+        nargs=1,
+    )
     # Font to use in output
     parser.add_argument(
-        "-f",
         "-font",
         help=textwrap.dedent(
             """ \
                         Name of monospaced font to use in output (default = 'Courier').
                         Enter font name of 'help' for a list of valid fonts.
                             """,
         ),
@@ -386,62 +403,71 @@
     parser.add_argument(
         "-preferences",
         help="Display Tasker preferences",
         action="store_true",
         default=False,
     )
 
+    # Make the output pretty
+    parser.add_argument(
+        "-pretty",
+        help="Make output prettier (one argument/parameter per line)",
+        action="store_true",
+        default=False,
+    )
+
     # Group project, profile and task = name ... together as exclusive arguments
-    group = parser.add_mutually_exclusive_group()
-    group.add_argument(
+    single_group = parser.add_mutually_exclusive_group()
+    single_group.add_argument(
         "-project",
         nargs=1,
         required=False,
         type=str,
         help="Display the details for a specific Project only.",
     )
-    group.add_argument(
+    single_group.add_argument(
         "-profile",
         nargs=1,
         required=False,
         type=str,
         help="Display the details for a specific Profile only.",
     )
+    single_group.add_argument(
+        "-task",
+        nargs=1,
+        required=False,
+        type=str,
+        help='Display the details for a single Task only (forces minimum of "-detail 3").',
+    )
+
     # Reset arguments
     parser.add_argument(
         "-reset",
         action="store_true",
         default=False,
         help="Reset previously saved arguments...start fresh.",
     )
+    # Rerun indicator (hidden)
+    # parser.add_argument("-rerun", default=False, action="store_true", help=argparse.SUPPRESS)
     # Display runtime arguments/settings
     parser.add_argument(
         "-runtime",
         help="Display all runtime arguments/settings at the top of the output.",
         action="store_true",
         default=False,
     )
     # Display taskerNet info
     parser.add_argument(
         "-taskernet",
         help="Display any TaskerNet information for Projects/Profiles.",
         action="store_true",
         default=False,
     )
-
-    group.add_argument(
-        "-task",
-        nargs=1,
-        required=False,
-        type=str,
-        help='Display the details for a single Task only (forces option "-detail 3").',
-    )
-
     # Display Task details under "hide/twisty"
-    parser.add_argument(
+    everything_group.add_argument(
         "-twisty",
         help=("Hide Task's details under 'twisty' ➤. Click on twisty to display details."),
         action="store_true",
         default=False,
     )
 
     # Version argument
```

### Comparing `maptasker-2.6.3/maptasker/src/prefers.py` & `maptasker-3.2.2/maptasker/src/prefers.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from maptasker.src.servicec import service_codes
 from maptasker.src.sysconst import FormatLine
 
 
 def process_service(
     service_name: str,
     service_value: str,
-    temp_output_lines,
+    temp_output_lines: list,
 ) -> None:
     """
     We have a service xml element that we have mapped as a preference.  Process it.
         :param service_name: name of the preference in <Service xml
         :param service_value: value of the preference in <Service xml
         :param temp_output_lines: list of service/preference output lines
     """
@@ -79,15 +79,15 @@
                     (
                         f"{preferences_html}{blank * 2}{output_service_name}\
                             {blank * 4}{service_value}"
                     ),
                     True,
                 )
             ),
-        ]
+        ],
     )
 
 
 # ##################################################################################
 # Go through all of the <service> xml elements to process the Tasker preferences.
 # ##################################################################################
 def process_preferences(temp_output_lines: list) -> None:
@@ -131,15 +131,15 @@
                             (
                                 f"{blank * 2}Not yet"
                                 f" mapped:{service_name}{blank * 4}type:{service_type}\
                                 {blank * 4}value:{service_value}"
                             ),
                             True,
                         ),
-                    ]
+                    ],
                 )
                 dummy_num += 1
         # Invalid <Setting> xml element
         else:
             error_handler("Error: the backup xml file is corrupt.  Program terminated.", 3)
 
     return
```

### Comparing `maptasker-2.6.3/maptasker/src/primitem.py` & `maptasker-3.2.2/maptasker/src/primitem.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Prime items which are used throughout MapTasker (globals)."""
+
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
 # primitem = intialize PrimeItems which are used throughout MapTasker (globals).       #
 #                                                                                      #
 # GNU General Public License v3.0                                                      #
@@ -30,42 +31,45 @@
 #  task_count_for_profile = number of Tasks in the specific Profile for Project
 #    being processed
 #  named_task_count_total = number of named Tasks for Project being processed
 #  task_count_unnamed = number of unnamed Tasks for Project being processed
 #  task_count_no_profile = number of Profiles in Project being processed.
 #  directory_items = if displaying a directory then this is a dictionary of items
 #    for the directory
-#  ordered_list_count = count of number of <ul> we currently have in output queue
 #  name_list = list of names of Projects/Profiles/Tasks/Scenes found thus far
 #  displaying_named_tasks_not_in_profile = True if we are displaying False if not
 #  mono_fonts = dictionary of monospace fonts from TkInter
 #  grand_totals = used for trcaking number of Projects/Profiles/Tasks/Scenes
 #  tasker_root_elements points to our root xml for Projects/Profiles/Tasks/Scenes
 #  directories = points to our directory items if we are displaying a directory
 #  variables = Tasker variables.
 #  current_project = current Project being processed
 #  tkroot = root for Tkinter (can only get it once)
+#  last_run = date of last run (set by restore_settings)
+#  slash = backslash for Windows or forward slash for OS X and Linux.
 #
 #   return
 from __future__ import annotations
 
 from typing import ClassVar
 
+from maptasker.src.sysconst import NOW_TIME
+
 
 class PrimeItems:
     """PrimeItems class contains global variables used throughout MapTasker"""
 
     xml_tree = None
     xml_root = None
     program_arguments: ClassVar = {}
     colors_to_use: ClassVar = {}
     output_lines = None
     file_to_get = ""
+    file_to_use = ""
     task_count_for_profile = 0
-    unordered_list_count = 0
     displaying_named_tasks_not_in_profile = False
     mono_fonts: ClassVar = {}
     found_named_items: ClassVar = {
         "single_project_found": False,
         "single_profile_found": False,
         "single_task_found": False,
     }
@@ -86,36 +90,31 @@
     tasker_root_elements: ClassVar = {
         "all_projects": [],
         "all_profiles": {},
         "all_scenes": {},
         "all_tasks": {},
         "all_services": [],
     }
-    scene_countgrand_totals: ClassVar = {
-        "projects": 0,
-        "profiles": 0,
-        "unnamed_tasks": 0,
-        "named_tasks": 0,
-        "scenes": 0,
-    }
     directories: ClassVar = []
     variables: ClassVar = {}
     current_project = ""
     error_code = 0
     error_msg = ""
     tkroot = None
+    last_run = NOW_TIME
+    slash = "/"
 
 
 # ##################################################################################
 # Reset all values
 # ##################################################################################
 class PrimeItemsReset:
     """Re-initialize all values in PrimeItems class"""
 
-    def __init__(self) -> None:  # noqa: ANN101
+    def __init__(self) -> None:
         """
         Initialize the PrimeItems class
         Args:
             self: The instance of the class
         Returns:
             None
         Initializes all attributes of the PrimeItems class with empty values or dictionaries:
@@ -146,30 +145,23 @@
         PrimeItems.tasker_root_elements = {
             "all_projects": [],
             "all_profiles": {},
             "all_scenes": {},
             "all_tasks": {},
             "all_services": [],
         }
-        PrimeItems.scene_countgrand_totals = {
-            "projects": 0,
-            "profiles": 0,
-            "unnamed_tasks": 0,
-            "named_tasks": 0,
-            "scenes": 0,
-        }
         PrimeItems.directories = []
         PrimeItems.xml_tree = None
         PrimeItems.xml_root = None
         PrimeItems.program_arguments = {}
         PrimeItems.colors_to_use = {}
         PrimeItems.output_lines = None
         PrimeItems.file_to_get = ""
         PrimeItems.task_count_for_profile = 0
-        PrimeItems.unordered_list_count = 0
         PrimeItems.displaying_named_tasks_not_in_profile = False
         PrimeItems.mono_fonts = {}
         PrimeItems.directories = []
         PrimeItems.variables = {}
         PrimeItems.current_project = ""
         PrimeItems.error_code = 0
         PrimeItems.error_msg = ""
+        PrimeItems.tkroot = None
```

### Comparing `maptasker-2.6.3/maptasker/src/proclist.py` & `maptasker-3.2.2/maptasker/src/proclist.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,18 +62,15 @@
         list_type (list): Either "Task:" or "Scene:"
         the_item (str): text for Task or Scene
 
     Returns:
         tuple[str, str]: Our formatted output line and color to user
     """
     # Format the Task/Scene name as needed: spacing and HTML
-    if list_type in {"Task:", "Scene:"}:
-        the_item_altered = adjust_name(list_type, the_item)
-    else:
-        the_item_altered = the_item
+    the_item_altered = adjust_name(list_type, the_item) if list_type in {"Task:", "Scene:"} else the_item
 
     # Format the output line
     output_line = f"{list_type}&nbsp;{the_item_altered}"
 
     # Set up the correct color for twisty of needed
     color_to_use = "scene_color" if list_type == "Scene:" else "task_color"
 
@@ -98,14 +95,15 @@
             the_task (defusedxml): XML pointer to our Task being procesed
             output_line (str): The etxt satring containing the output
             color_to_use (str): The color to use in the output
 
         Returns:
             tuple[str, str]: Our temporary item and temporary list item
     """
+
     temp_item = temp_list = ""
     if "&#45;&#45;Task:" in list_type:
         temp_item = the_item
         temp_list = list_type
         the_item = ""
         if PrimeItems.program_arguments["debug"]:  # Get the Task ID
             id_loc = list_type.find("ID:")
@@ -117,14 +115,18 @@
         # Get the Task name from the line being formatted
         task_id = the_task.attrib.get("sr")[4:]
         task_name = PrimeItems.tasker_root_elements["all_tasks"][task_id]["name"]
         if task_name != "":
             # Handle directory hyperlink
             add_directory_item("tasks", task_name)
 
+    # Insert directory for Scene
+    elif PrimeItems.program_arguments["directory"] and list_type == "Scene:":
+        add_directory_item("scenes", the_item)
+
     # Insert a hyperlink if this is a Task...it has to go before a twisty
     if (
         PrimeItems.program_arguments["directory"]
         and PrimeItems.directory_items["current_item"]
         and "Task:" in list_type
         and "&#45;&#45;Task:" not in list_type
     ):
@@ -148,29 +150,29 @@
 # Given an item, format it with all of the particulars and add to output.
 # ################################################################################
 def format_item(
     list_type: str,
     the_item: str,
     the_list: list,
     the_task: defusedxml,
-):
+) -> None:
     """
     Given an item, format it with all of the particulars:
         Proper html/color/font, twisty, directory, properties, etc.
         Args:
             list_type (str): Either "Task:" or "Scene:"
             the_item (str): The string for the above type
             the_list (list): List of Tasks or Scenes
             the_task (defusedxml): The Task XML element
     """
     # Log if in debug mode
     if PrimeItems.program_arguments["debug"]:
         logger.debug(
             f"process_list  the_item:{the_item} the_list:{the_list} list_type:\
-            {list_type}"
+            {list_type}",
         )
 
     # Format the Task or Scene
     output_line, color_to_use = format_task_or_scene(list_type, the_item)
 
     # If "--Task:" then this is a Task under a Scene.
     # Need to temporarily save the_item since add_line_to_output changes the_item
@@ -183,23 +185,20 @@
     if temp_item:
         the_item = temp_item
         list_type = temp_list
 
     # Process Task Properties if this is a Task, display level is 3 and
     # we are not at the end dispaying Tasks that are not in any Profile
     if (
-        the_task
+        the_task is not None
         and "Task:" in list_type
         and PrimeItems.program_arguments["display_detail_level"] > 2
         and not PrimeItems.displaying_named_tasks_not_in_profile
     ):
-        get_properties(
-            the_task,
-            "task_color",
-        )
+        get_properties("Task:", the_task)
 
 
 # ##################################################################################
 # Process Given a Task/Scene, process it.
 # ##################################################################################
 def process_item(
     the_item: str,
@@ -230,36 +229,34 @@
     if PrimeItems.program_arguments["display_detail_level"] == 0:
         return
 
     # Output Actions for this Task if Task is unknown
     #   and not part of output for Tasks with no Profile(s)
     # Do we get the Task's Actions?
     if (
-        (the_task and "Task:" in list_type and UNKNOWN_TASK_NAME in the_item) or ("Task:" in list_type)
+        (the_task is not None and "Task:" in list_type and UNKNOWN_TASK_NAME in the_item) or ("Task:" in list_type)
     ) and "<em>No Profile" not in the_item:
         get_task_actions_and_output(
             the_task,
             list_type,
             the_item,
             tasks_found,
         )
 
         # End the twisty hidden lines if not a Task in a Scene
         if PrimeItems.program_arguments["twisty"]:
             remove_twisty()
-        # If not a twisty but is a digit, then this is a Scene's Task...
-        # delete previous </ul>
-        elif the_item.isdigit():
-            PrimeItems.output_lines.delete_last_line()
 
     elif list_type == "Scene:" and PrimeItems.program_arguments["display_detail_level"] > 1:
         # We have a Scene: process its details
         process_scene(
             the_item,
             tasks_found,
+            None,
+            0,
         )
 
     # Remove twisty if not displaying level 0
     elif PrimeItems.program_arguments["twisty"]:
         if PrimeItems.program_arguments["display_detail_level"] > 0:
             remove_twisty()
         else:
@@ -271,26 +268,26 @@
 
 # ##################################################################################
 # Process Task/Scene text/line item: call recursively for Tasks within Scenes
 # ##################################################################################
 def process_list(
     list_type: str,
     the_list: list,
-    the_task: defusedxml.ElementTree.XML,  # type: ignore
+    the_task: defusedxml.ElementTree.XML,
     tasks_found: list,
 ) -> None:
     """
     Process Task/Scene text/line item: call recursively for Tasks within Scenes
 
         :param list_type: Task or Scene
         :param the_list: list of Task names tro process
         :param the_task: Task/Scene xml element
         :param tasks_found: list of Tasks found so far
         :return:
     """
 
     # Go through all Tasks in the list
+    # The list looks like...
+    # 'Battery Full Alert&nbsp;&nbsp;&nbsp;&nbsp;<<< Entry Task&nbsp;&nbsp;Task ID: 18 &nbsp;&nbsp;[Priority: 6]&nbsp;&nbsp;')
     for the_item in the_list:
         # Process the item (list of items)
         process_item(the_item, list_type, the_task, tasks_found)
-
-    return
```

### Comparing `maptasker-2.6.3/maptasker/src/profiles.py` & `maptasker-3.2.2/maptasker/src/profiles.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,38 @@
+"""Handle Profile"""
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
 # profiles: process Profiles for given project                                         #
 #                                                                                      #
 # GNU General Public License v3.0                                                      #
 # Permissions of this strong copyleft license are conditioned on making available      #
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
-import defusedxml.ElementTree  # Need for type hints
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
 
 from maptasker.src import condition, tasks
 from maptasker.src.dirout import add_directory_item
 
 # from maptasker.src.kidapp import get_kid_app
 from maptasker.src.format import format_html
 from maptasker.src.nameattr import add_name_attribute
 from maptasker.src.primitem import PrimeItems
 from maptasker.src.property import get_properties
 from maptasker.src.share import share
-from maptasker.src.sysconst import NO_PROFILE, FormatLine
+from maptasker.src.sysconst import DISABLED, NO_PROFILE, FormatLine
+
+if TYPE_CHECKING:
+    import defusedxml.ElementTree
 
 
 # ##################################################################################
 # Get a specific Profile's Tasks (maximum of two:entry and exit)
 # ##################################################################################
 def get_profile_tasks(
     the_profile: defusedxml.ElementTree.XML,
@@ -69,16 +75,16 @@
                 PrimeItems.task_count_for_profile = PrimeItems.task_count_for_profile + 1
             the_task_element, the_task_name = tasks.get_task_name(
                 task_id,
                 found_tasks_list,
                 task_output_line,
                 task_type,
             )
+            # Add this Task to our list of Tasks processed thus far.
             list_of_tasks.append({"xml": the_task_element, "name": the_task_name})
-            # list_of_tasks.append([the_task_element, the_task_name])
             if (
                 PrimeItems.program_arguments["single_task_name"]
                 and PrimeItems.program_arguments["single_task_name"] == the_task_name
             ):
                 PrimeItems.found_named_items["single_task_found"] = True
                 break
         # If hit Profile's name, we've passed all the Task ids.
@@ -136,95 +142,196 @@
 
         :param project: the Project xml element
         :param profile: the Profile xml element
         :return: Profile name
     """
 
     flags = condition_text = ""
+    blank = "&nbsp;"
 
     # Set up HTML to use
     disabled_profile_html = format_html(
         "disabled_profile_color",
         "",
-        "[DISABLED]",
+        DISABLED,
         True,
     )
     launcher_task_html = format_html(
         "launcher_task_color",
         "",
         "[Launcher Task]",
         True,
     )
 
     # Look for disabled Profile
     limit = profile.find("limit")  # Is the Profile disabled?
-    if limit is not None and limit.text == "true":
-        disabled = disabled_profile_html
-    else:
-        disabled = ""
+    disabled = disabled_profile_html if limit is not None and limit.text == "true" else ""
 
     # Is there a Launcher Task with this Project?
     launcher_xml = project.find("ProfileVariable")
     launcher = launcher_task_html if launcher_xml is not None else ""
 
     # See if there is a Kid app and/or Priority (FOR FUTURE USE)
     # kid_app_info = ''
     # if program_args["display_detail_level"] > 2:
     #     kid_app_info = get_kid_app(profile)
     #     priority = get_priority(profile, False)
 
     # Display flags for debug mode
     if PrimeItems.program_arguments["debug"]:
         flags = profile.find("flags")
-        if flags is not None:
-            flags = format_html(
-                "GreenYellow",
-                "",
-                f" flags: {flags.text}",
-                True,
-            )
-        else:
-            flags = ""
+        flags = format_html("launcher_task_color", "", f" flags: {flags.text}", True) if flags is not None else ""
 
     # Get the Profile name
     profile_name_with_html, profile_name = get_profile_name(profile)
 
     # Handle directory hyperlink
     if PrimeItems.program_arguments["directory"]:
         add_directory_item("profiles", profile_name)
 
     # Get the Profile's conditions
-    if PrimeItems.program_arguments["conditions"] or profile_name == "NO_PROFILE":
-        if profile_conditions := condition.parse_profile_condition(
-            profile,
-        ):
+    if PrimeItems.program_arguments["conditions"] or profile_name == "NO_PROFILE":  # noqa: SIM102
+        if profile_conditions := condition.parse_profile_condition(profile):
             # Strip pre-existing HTML from conditions, since some condition codes
             # may be same as Actions.
             # And the Actions would have plugged in the action_color HTML.
             # profile_conditions = remove_html_tags(profile_conditions, "")
+
+            # Make the conditions pretty
+            if PrimeItems.program_arguments["pretty"]:
+                condition_length = profile_conditions.find(":")
+                # Add spacing for profile name, condition name and "Profile:"
+                profile_conditions = profile_conditions.replace(
+                    ",", f"<br>{blank*(len(profile_name)+condition_length+7)}",
+                )
+
+            # Add the HTML
             condition_text = format_html(
                 "profile_condition_color",
                 "",
                 f" ({profile_conditions})",
                 True,
             )
 
     # Okay, string it all together
     profile_info = f"{profile_name_with_html} {condition_text} {launcher}{disabled} {flags}"
 
+    # Break it up into separate lines if we are doing pretty output
+    if PrimeItems.program_arguments["pretty"]:
+        indentation = len(profile_name) + 4
+        # Break at comma
+        profile_info = profile_info.replace(", ", f"<br>{blank*indentation}")
+        # Break at paren
+        profile_info = profile_info.replace(" (", f"<br>{blank*indentation}  (")
+        # Break at bracket
+        profile_info = profile_info.replace(" [", f"<br>{blank*indentation}  [")
+
     # Output the Profile line
     PrimeItems.output_lines.add_line_to_output(
         2,
         profile_info,
         FormatLine.dont_format_line,
     )
     return profile_name
 
 
 # ##################################################################################
+# Process the Profile passed in.
+# ##################################################################################
+def do_profile(
+    item: defusedxml.ElementTree.XML,
+    project: defusedxml.ElementTree.XML,
+    project_name: str,
+    profile: defusedxml.ElementTree.XML,
+    list_of_found_tasks: list,
+) -> bool:
+    """Function:
+        This function searches for a specific Profile and outputs its Tasks.
+    Parameters:
+        - item (defusedxml.ElementTree.XML): The current item being processed.
+        - project (defusedxml.ElementTree.XML): The current project being processed.
+        - project_name (str): The name of the current project.
+        - profile (defusedxml.ElementTree.XML): The current profile being processed.
+        - list_of_found_tasks (list): A list of all found tasks.
+    Returns:
+        - bool: True if a specific Task is being searched for, False otherwise.
+    Processing Logic:
+        - Checks if a specific Profile is being searched for.
+        - Checks if the current item's name matches the specified Profile name.
+        - If a match is found, sets the appropriate flags and clears the output list.
+        - Gets the list of Tasks for the current Profile.
+        - Outputs the Profile line and its properties.
+        - Processes any <Share> information from TaskerNet.
+        - Outputs the Tasks for the current Profile.
+        - Returns True if a specific Task is being searched for, False otherwise."""
+    # Are we searching for a specific Profile?
+    if PrimeItems.program_arguments["single_profile_name"]:
+        # Make sure this item's name is in our list of profiles.
+        if not (profile_name := PrimeItems.tasker_root_elements["all_profiles"][item]["name"]):
+            return False  # Not our Profile...go to next Profile ID
+
+        if PrimeItems.program_arguments["single_profile_name"] != profile_name:
+            return False  # Not our Profile...go to next Profile ID
+
+            return False  # Not our Profile...go to next Profile ID
+
+        # BINGO! We found the Profile we were looking for!
+        # Identify items found.
+        PrimeItems.found_named_items["single_profile_found"] = True
+        PrimeItems.program_arguments["single_project_name"] = project_name
+        PrimeItems.found_named_items["single_project_found"] = True
+
+        # Clear the output list to prepare for single Profile only
+        PrimeItems.output_lines.refresh_our_output(
+            False,
+            project_name,
+            "",
+        )
+
+        # Start Profile list
+        PrimeItems.output_lines.add_line_to_output(1, "", FormatLine.dont_format_line)
+    # Get Task xml element and name
+    task_output_lines = []  # Profile's Tasks will be filled in here
+    list_of_tasks = get_profile_tasks(
+        profile,
+        list_of_found_tasks,
+        task_output_lines,
+    )
+
+    # Examine Profile attributes and output Profile line
+    profile_name = build_profile_line(
+        project,
+        profile,
+    )
+
+    # Process Profile Properties
+    if PrimeItems.program_arguments["display_detail_level"] > 2:
+        get_properties("Profile:", profile)
+
+    # Process any <Share> information from TaskerNet
+    if PrimeItems.program_arguments["taskernet"]:
+        share(profile, "proftab")
+        # Add a spacer if detail is 0
+        if PrimeItems.program_arguments["display_detail_level"] == 0:
+            PrimeItems.output_lines.add_line_to_output(0, "", FormatLine.dont_format_line)
+
+    # We have the Tasks for this Profile.  Now let's output them.
+    # Return True = we're looking for a specific Task
+    # Return False = this is a normal Task
+    return tasks.output_task_list(
+        list_of_tasks,
+        project_name,
+        profile_name,
+        task_output_lines,
+        list_of_found_tasks,
+        True,
+    )
+
+
+# ##################################################################################
 # Go through all Projects Profiles...and output them
 # ##################################################################################
 def process_profiles(
     project: defusedxml.ElementTree.XML,
     project_name: str,
     profile_ids: list,
     list_of_found_tasks: list,
@@ -240,86 +347,23 @@
     """
 
     # Go through the Profiles found in the Project
     for item in profile_ids:
         profile = PrimeItems.tasker_root_elements["all_profiles"][item]["xml"]
         if profile is None:  # If Project has no profiles, skip
             return None
-
-        # Are we searching for a specific Profile?
-        if PrimeItems.program_arguments["single_profile_name"]:
-            # Make sure this item's name is in our list of profiles.
-            if not (profile_name := PrimeItems.tasker_root_elements["all_profiles"][item]["name"]):
-                continue
-
-            if PrimeItems.program_arguments["single_profile_name"] != profile_name:
-                continue  # Not our Profile...go to next Profile ID
-
-            # BINGO! We found the Profile we were looking for!
-            # Identify items found.
-            PrimeItems.found_named_items["single_profile_found"] = True
-            PrimeItems.program_arguments["single_project_name"] = project_name
-            PrimeItems.found_named_items["single_project_found"] = True
-
-            # Clear the output list to prepare for single Profile only
-            PrimeItems.output_lines.refresh_our_output(
-                False,
-                project_name,
-                "",
-            )
-
-            # Start Profile list
-            PrimeItems.output_lines.add_line_to_output(1, "", FormatLine.dont_format_line)
-        # Get Task xml element and name
-        task_output_lines = []  # Profile's Tasks will be filled in here
-        list_of_tasks = get_profile_tasks(
-            profile,
-            list_of_found_tasks,
-            task_output_lines,
-        )
-
-        # Examine Profile attributes and output Profile line
-        profile_name = build_profile_line(
-            project,
-            profile,
-        )
-
-        # Process Profile Properties
-        if PrimeItems.program_arguments["display_detail_level"] > 2:
-            get_properties(
-                profile,
-                "profile_color",
-            )
-
-        # Process any <Share> information from TaskerNet
-        if PrimeItems.program_arguments["taskernet"]:
-            share(profile)
-            # Add a spacer if detail is 0
-            if PrimeItems.program_arguments["display_detail_level"] == 0:
-                PrimeItems.output_lines.add_line_to_output(0, "", FormatLine.dont_format_line)
-
-        # We have the Tasks for this Profile.  Now let's output them.
-        # True = we're looking for a specific Task
-        # False = this is a normal Task
-        specific_task = tasks.output_task_list(
-            list_of_tasks,
-            project_name,
-            profile_name,
-            task_output_lines,
-            list_of_found_tasks,
-            True,
-        )
+        specific_task = do_profile(item, project, project_name, profile, list_of_found_tasks)
 
         # Get out if doing a specific Task, and it was found, or not specific task but
         # found speficic Profile.  No need to process any more Profiles.
         if (
             specific_task
             and PrimeItems.program_arguments["single_task_name"]
             and PrimeItems.found_named_items["single_task_found"]
         ) or (
             not specific_task and PrimeItems.found_named_items["single_profile_found"]
         ):  # Get out if we've got the Task we're looking for
             break
-        elif not specific_task:
+        if not specific_task:
             continue
 
     return ""
```

### Comparing `maptasker-2.6.3/maptasker/src/progargs.py` & `maptasker-3.2.2/maptasker/src/progargs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Process runtime program arguments"""
+
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
 # progargs: process program runtime arguments for MapTasker                            #
 #                                                                                      #
 # GNU General Public License v3.0                                                      #
```

### Comparing `maptasker-2.6.3/maptasker/src/proginit.py` & `maptasker-3.2.2/maptasker/src/proginit.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
 import atexit
 import contextlib
+import platform
 import sys
-from datetime import datetime
 from json import dumps, loads  # For write and read counter
 from pathlib import Path
 from tkinter import TkVersion, messagebox
 
 # importing askopenfile (from class filedialog) and messagebox functions
 from tkinter.filedialog import askopenfile
 
@@ -30,14 +30,15 @@
 # from maptasker.src.fonts import get_fonts
 from maptasker.src.frontmtr import output_the_front_matter
 from maptasker.src.getbakup import get_backup_file
 from maptasker.src.primitem import PrimeItems
 from maptasker.src.sysconst import (
     COUNTER_FILE,
     MY_VERSION,
+    NOW_TIME,
     TYPES_OF_COLOR_NAMES,
     logger,
     logging,
 )
 from maptasker.src.taskerd import get_the_xml_data
 
 
@@ -71,84 +72,113 @@
 
 
 run_counter = read_counter()
 atexit.register(write_counter)
 
 
 # ##################################################################################
+# Prompt user to select the backup xml file to use.
+# ##################################################################################
+def prompt_for_backup_file(dir_path: str) -> None:
+    """
+    Prompt user to select a backup file
+    Args:
+        dir_path (str): Path to initial directory for file selection dialog
+    Returns:
+        None: No value is returned
+    Processing Logic:
+        - Try to open a file selection dialog to choose an XML backup file
+        - Set a flag if any exception occurs or no file is selected
+        - Check the flag and call an error handler if running without GUI
+        - Set an error code if running with GUI
+    """
+    file_error = False
+    # Tkinter prompt for file selection.
+    try:
+        PrimeItems.file_to_get = askopenfile(
+            parent=PrimeItems.tkroot,
+            mode="r",
+            title="Select Tasker backup xml file",
+            initialdir=dir_path,
+            filetypes=[("XML Files", "*.xml")],
+        )
+        PrimeItems.error_code = 0  # No error.  Clear the code if there is one.
+    except Exception:  # noqa: BLE001
+        file_error = True
+    if PrimeItems.file_to_get is None:
+        file_error = True
+    if file_error and not PrimeItems.program_arguments["gui"]:
+        error_handler("Backup file selection cancelled.  Program ended.", 6)
+    elif file_error:
+        PrimeItems.error_code = 6
+
+
+# ##################################################################################
 # Open and read the Tasker backup XML file
 # Return the file name for use for
 # ##################################################################################
 def open_and_get_backup_xml_file() -> dict:
     """
     Open the Tasker backup file and return the file object
     """
     # Fetch backup xml directly from Android device?
-    if PrimeItems.program_arguments["android_ipaddr"] and PrimeItems.program_arguments["android_file"] and PrimeItems.program_arguments["android_port"]:
+    if (
+        PrimeItems.program_arguments["android_ipaddr"]
+        and PrimeItems.program_arguments["android_file"]
+        and PrimeItems.program_arguments["android_port"]
+    ):
         backup_file_name = get_backup_file()
 
-        # If no backup file and we're coming from the GUI, then rerturn to GUI.
+        # If no backup file and we're coming from the GUI, then return to GUI.
         if backup_file_name is None and PrimeItems.program_arguments["gui"]:
             return None
 
         # Make sure we automatically use the file we just fetched
         PrimeItems.program_arguments["file"] = backup_file_name
 
     logger.info("entry")
-    file_error = False
 
     # Reset the file name
     PrimeItems.file_to_get = None
 
-    # dir_path = path.dirname(path.realpath(__file__))  # Get current directory
+    # Get current directory
     dir_path = Path.cwd()
     logger.info(f"dir_path: {dir_path}")
 
     # If debug and we didn't fetch the backup file from Android device, default to
     # "backup.xml" file as backup to restore
 
-    if PrimeItems.program_arguments["debug"] and PrimeItems.program_arguments["fetched_backup_from_android"] is False:
+    if (
+        PrimeItems.program_arguments["debug"]
+        and PrimeItems.program_arguments["fetched_backup_from_android"] is False
+        and not PrimeItems.program_arguments["file"]
+    ):
         PrimeItems.program_arguments["file"] = ""
         try:
-            PrimeItems.file_to_get = open(f"{dir_path}/backup.xml")
+            PrimeItems.file_to_get = open(f"{dir_path}{PrimeItems.slash}backup.xml")
         except OSError:
             error_handler(
-                (f"Error: The backup.xml file was not found in {dir_path}.  Program terminated!"),
+                (f"Error: Debug is on and the backup.xml file was not found in {dir_path}."),
                 3,
             )
+            prompt_for_backup_file(dir_path)
 
     # See if we already have the file
     elif PrimeItems.program_arguments["file"]:
         filename = isinstance(PrimeItems.program_arguments["file"], str)
         filename = PrimeItems.program_arguments["file"].name if not filename else PrimeItems.program_arguments["file"]
 
         # We already have the file name...open it.
         try:
             PrimeItems.file_to_get = open(filename)
         except FileNotFoundError:
             file_not_found = filename
             error_handler(f"Backup file {file_not_found} not found.  Program ended.", 6)
     else:
-        try:
-            PrimeItems.file_to_get = askopenfile(
-                parent=PrimeItems.tkroot,
-                mode="r",
-                title="Select Tasker backup xml file",
-                initialdir=dir_path,
-                filetypes=[("XML Files", "*.xml")],
-            )
-        except Exception:
-            file_error = True
-        if PrimeItems.file_to_get is None:
-            file_error = True
-        if file_error and not PrimeItems.program_arguments["gui"]:
-            error_handler("Backup file selection cancelled.  Program ended.", 6)
-        elif file_error:
-            PrimeItems.error_code = 6
-            return
+        prompt_for_backup_file(dir_path)
 
     return
 
 
 # ##################################################################################
 # Build color dictionary
 # ##################################################################################
@@ -207,96 +237,113 @@
 # Log the arguments
 # ##################################################################################
 def log_startup_values() -> None:
     """
     Log the runtime arguments and color mappings
     """
     setup_logging()  # Get logging going
-    logger.info(f"{MY_VERSION} {str(datetime.now())}")  # noqa: RUF010, DTZ005
+    logger.info(f"{MY_VERSION} {str(NOW_TIME)}")  # noqa: RUF010
     logger.info(f"sys.argv:{str(sys.argv)}")  # noqa: RUF010
     for key, value in PrimeItems.program_arguments.items():
         logger.info(f"{key}: {value}")
     for key, value in PrimeItems.colors_to_use.items():
         logger.info(f"colormap for {key} set to {value}")
 
 
 # ##################################################################################
 # POpen and read xml and output the introduction/heading matter
 # ##################################################################################
-def get_data_and_output_intro() -> int:
+def get_data_and_output_intro(do_front_matter: bool) -> int:
     """
     Gets data from Tasker backup file and outputs introductory information.
 
     Args:
-        None: None
+        do_front_matter (bool): True = output the front matter, False = don't bother
     Returns:
         int: 0 if okay, non-zero if error (error code)
 
     Processing Logic:
     - Opens and reads the Tasker backup XML file
     - Extracts all the XML data from the file
     - Closes the file after reading
     - Outputs initial information like header and source to the user
     """
-    PrimeItems.program_arguments["file"] = PrimeItems.file_to_get
-
-    # Only display message box if we don't yet have the file name
-    if not PrimeItems.file_to_get and run_counter < 1 and not GUI:
-        msg = "Locate the Tasker backup xml file to use to map your Tasker environment"
-        messagebox.showinfo("MapTasker", msg)
-
-    # Open and read the file...
-    open_and_get_backup_xml_file()
-    if PrimeItems.error_code > 0:
-        return PrimeItems.error_code
-
-    # Go get all the xml data
-    get_the_xml_data()
-
-    # Close the file
-    PrimeItems.file_to_get.close()
+    # Only get the XML if we don't already have it.
+    tasker_root_elements = PrimeItems.tasker_root_elements
+    return_code = 0
+    if (
+        not tasker_root_elements["all_projects"]
+        and not tasker_root_elements["all_profiles"]
+        and not tasker_root_elements["all_tasks"]
+        and not tasker_root_elements["all_scenes"]
+    ):
+
+        # We don't yet have the data.  Let's get it.
+        if not PrimeItems.program_arguments["file"]:
+            PrimeItems.program_arguments["file"] = (
+                PrimeItems.file_to_get if PrimeItems.file_to_use == "" else PrimeItems.file_to_use
+            )
 
-    # Output the inital info: head, source, etc.
-    output_the_front_matter()
+        # Only display message box if we don't yet have the file name,if this is not the first time ever that we have run,
+        # and not running from the GUI.
+        if not PrimeItems.file_to_get and run_counter < 1 and not GUI:
+            msg = "Locate the Tasker backup xml file to use to map your Tasker environment"
+            messagebox.showinfo("MapTasker", msg)
+
+        # Open and read the file...
+        open_and_get_backup_xml_file()
+        if PrimeItems.error_code > 0:
+            return PrimeItems.error_code
+
+        # Go get all the xml data
+        return_code = get_the_xml_data()
+
+        # Close the file
+        PrimeItems.file_to_get.close()
+
+    # Output the inital info: head, source, etc. ...if it hasn't already been output.
+    if return_code == 0 and do_front_matter and not PrimeItems.output_lines.output_lines:
+        output_the_front_matter()
+        return 0
 
-    return 0
+    return return_code
 
 
 # ##################################################################################
 # Make sure we have the appropriate version of Python and Tkinter
 # ##################################################################################
 def check_versions() -> None:
     """
     Checks the Python and Tkinter versions
     Args:
         None: No arguments
     Returns:
         None: Does not return anything
     - It gets the Python version and splits it into major, minor, and patch numbers
-    - It checks if the major version is less than 3 or the major is 3 and minor is less than 10
+    - It checks if the major version is less than 3 or the major is 3 and minor is less than 11
     - It gets the Tkinter version and splits it into major and minor
     - It checks if the major is less than 8 or the major is 8 and minor is less than 6
     - If either check fails, it logs and prints an error message and exits
     """
     msg = ""
     version = sys.version
     version = version.split(" ")
     major, minor, patch = (int(x, 10) for x in version[0].split("."))
-    if major < 3 or (major == 3 and minor < 10):
-        msg = f"Python version {sys.version} is not supported.  Please use Python 3.10 or greater."
+    if major < 3 or (major == 3 and minor < 11):
+        msg = f"Python version {sys.version} is not supported.  Please use Python 3.11 or greater."
     version = str(TkVersion)
     major, minor = version.split(".")
     if int(major) < 8 or (int(major) == 8 and int(minor) < 6):
         msg = (
             f"{msg}  Tcl/tk (Tkinter) version {TkVersion} is not supported.  Please use Tkinter version 8.6 or greater."
         )
         logger.error(msg)
     if msg:
         logger.error("MapTasker", msg)
-        print(msg)  # noqa: T201
+        print(msg)
         exit(0)  # noqa: PLR1722
 
 
 # ##################################################################################
 # Perform maptasker program initialization functions
 # ##################################################################################
 def start_up() -> dict:
@@ -314,28 +361,34 @@
         - Gets the list of available fonts
         - Gets a map of colors to use
         - Gets key program elements and outputs intro text
         - Logs startup values if debug mode is enabled
     """
     logger.info(f"sys.argv{sys.argv!s}")
 
+    # Get the OS so we know which directory slash to use (/ or \)
+    our_platform = platform.system()
+    if our_platform == "Windows":
+        PrimeItems.slash = "\\"
+    else:
+        PrimeItems.slash = "/"
+
     # Validate runtime versions
     check_versions()
 
     # Get runtime arguments (from CLI or GUI)
     get_arguments.get_program_arguments()
 
     # Get our list of fonts
     # _ = get_fonts(True)
 
     # Get our map of colors
     PrimeItems.colors_to_use = setup_colors()
 
-    # get_data_and_output_intro program key elements
-    # PrimeItems.program_arguments["gui"] = False  # Turn off...we don't want this on anymore.
-    _ = get_data_and_output_intro()
+    # Get the XML data and output the front matter
+    _ = get_data_and_output_intro(True)
 
     # If debug mode, log the arguments
     if PrimeItems.program_arguments["debug"]:
         log_startup_values()
 
     return
```

### Comparing `maptasker-2.6.3/maptasker/src/projects.py` & `maptasker-3.2.2/maptasker/src/projects.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,125 @@
+"""Do the Projects"""
+
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
 # project: process the project passed in                                               #
 #                                                                                      #
 # GNU General Public License v3.0                                                      #
 # Permissions of this strong copyleft license are conditioned on making available      #
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
 
-import defusedxml.ElementTree  # Need for type hints
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
 
 from maptasker.src import tasks
 from maptasker.src.dirout import add_directory_item
 from maptasker.src.format import format_html
 from maptasker.src.getids import get_ids
 from maptasker.src.globalvr import output_variables
 from maptasker.src.kidapp import get_kid_app
 from maptasker.src.nameattr import add_name_attribute
 from maptasker.src.primitem import PrimeItems
+from maptasker.src.proclist import process_list
 from maptasker.src.profiles import process_profiles
 from maptasker.src.property import get_properties
 from maptasker.src.scenes import process_project_scenes
 from maptasker.src.share import share
-from maptasker.src.sysconst import FormatLine
+from maptasker.src.sysconst import NORMAL_TAB, FormatLine
 from maptasker.src.taskflag import get_priority
 from maptasker.src.twisty import add_twisty, remove_twisty
 
+if TYPE_CHECKING:
+    import defusedxml.ElementTree
+
 
 # ##################################################################################
 # process_projects: go through all Projects Profiles...and output them
 # ##################################################################################
 def process_projects_and_their_profiles(
     found_tasks: list,
     projects_without_profiles: list,
 ) -> list:
-    """
-    Go through all Projects, process them and their Profiles and Tasks
-    (and add to our output list)
-        :param found_tasks: list of Tasks found thus far
-        :param projects_without_profiles: list of Projects that don't have any Profiles
-        :return: list of Tasks found thus far, with duplicates removed
-    """
+    """Parameters:
+        - found_tasks (list): A list of tasks that have been found.
+        - projects_without_profiles (list): A list of projects that do not have profiles.
+    Returns:
+        - list: A list of tasks found with duplicates removed.
+    Processing Logic:
+        - Process projects if there are any.
+        - If no Projects then process profiles if there are any.
+        - If no Projects and no Scenes the process tasks if there are any.
+        - If no Projects then process scenes if there are any."""
     our_task_element = ""
 
-    process_projects(
-        projects_without_profiles,
-        found_tasks,
-        our_task_element,
-    )
-    PrimeItems.output_lines.add_line_to_output(
-        3,
-        "",
-        FormatLine.dont_format_line,
-    )  # Close Project list
+    # Process Projects only if there are Projects
+    if PrimeItems.tasker_root_elements["all_projects"]:
+        process_projects(
+            projects_without_profiles,
+            found_tasks,
+            our_task_element,
+        )
+
+    # Only Profiles...?
+    elif PrimeItems.tasker_root_elements["all_profiles"]:
+        PrimeItems.task_count_unnamed = 0
+        process_profiles(
+            "",
+            "None",
+            PrimeItems.tasker_root_elements["all_profiles"],
+            found_tasks,
+        )
+        PrimeItems.grand_totals["profiles"] += 1
+
+    # Only Tasks...(and not Scenes too) e.g. only Tasks?
+    elif PrimeItems.tasker_root_elements["all_tasks"] and not PrimeItems.tasker_root_elements["all_scenes"]:
+        # Build a "list" of Tasks consisting of the Tasks off our troot Task list,
+        task_list = []
+        task_output_lines = []
+        for task in PrimeItems.tasker_root_elements["all_tasks"]:
+            task_list.append(
+                {
+                    "xml": PrimeItems.tasker_root_elements["all_tasks"][task]["xml"],
+                    "name": PrimeItems.tasker_root_elements["all_tasks"][task]["name"],
+                },
+            )
+            task_output_lines.append(" ")
+            if PrimeItems.tasker_root_elements["all_tasks"][task]["name"]:
+                PrimeItems.grand_totals["named_tasks"] += 1
+            else:
+                PrimeItems.grand_totals["unnamed_tasks"] += 1
+        tasks.output_task_list(
+            task_list,
+            "Unknown",
+            "None",
+            task_output_lines,
+            [],
+            True,
+        )
+
+    # Only Scene...?
+    elif PrimeItems.tasker_root_elements["all_scenes"]:
+        scene_list = []
+        found_tasks = []
+        for scene in PrimeItems.tasker_root_elements["all_scenes"]:
+            scene_list.append(PrimeItems.tasker_root_elements["all_scenes"][scene]["name"])
+            PrimeItems.grand_totals["scenes"] += 1
+        process_list(
+            "Scene:",
+            scene_list,
+            "",
+            found_tasks,
+        )
 
     # Return a list of Tasks found thus far with duplicates remove
     # Reference: https://www.pythonmorsels.com/deduplicate-lists/
     # return list(dict.fromkeys(found_tasks).keys())
     return list(set(found_tasks))
 
 
@@ -86,23 +145,31 @@
             )
     return launcher_task_info
 
 
 # ##################################################################################
 # Add heading for Tasks that are not in any Profile
 # ##################################################################################
-def task_not_in_profile_heading(project_name: str):
-    """
-    Add heading for Tasks that are not in any Profile
-        Args:
+def task_not_in_profile_heading(project_name: str) -> None:
 
-            project_name (str): Name of the Project we are doing.
-    """
     # Format the output line
-    output_line = "&nbsp;&nbsp;&nbsp;The following Tasks in Project" f" {project_name} are not in any Profile..."
+    """Returns a formatted output line for the tasks that are not in any profile.
+
+    Parameters:
+        - project_name (str): The name of the project.
+    Returns:
+        - None: This function does not return anything, it only formats the output line.
+    Processing Logic:
+        - Formats the output line with the project name.
+        - Adds a line break before the header.
+        - Adds a "twisty" if specified in the program arguments.
+        - If not doing a twisty, adds the output line with a line break.
+        - Starts an unordered list."""
+
+    output_line = f"&nbsp;&nbsp;&nbsp;The following Tasks in Project '{project_name}' are not in any Profile..."
 
     # Force a line break before the header
     PrimeItems.output_lines.add_line_to_output(5, "<br>", FormatLine.dont_format_line)
 
     # Add the "twisty" to hide the Task details
     if PrimeItems.program_arguments["twisty"]:
         add_twisty(
@@ -142,15 +209,16 @@
             found_tasks (list): List of the Tasks found so far
             output_the_heading (bool): True if we need to output the Project heading
             have_tasks_not_in_profile (bool): Trues if there are Tasks not in the current Profile
 
             return: True if we have Tasks not in any Profile
     """
     for the_id in task_ids:
-        PrimeItems.named_task_count_total = len(task_ids)
+        if not PrimeItems.program_arguments["single_profile_name"]:
+            PrimeItems.named_task_count_total = len(task_ids)
         # We have a Task in Project that has yet to be output?
         if the_id not in found_tasks and (
             not PrimeItems.found_named_items["single_profile_found"]
             and not PrimeItems.found_named_items["single_task_found"]
         ):
             # Flag that we have Tasks that are not in any Profile, and bump the count\
             have_tasks_not_in_profile = True
@@ -177,28 +245,32 @@
                 task_not_in_profile_heading(project_name)
 
                 output_the_heading = False
 
             # Format the output line
             task_output_lines = [
                 f"{our_task_name}&nbsp;&nbsp;&nbsp;<em>(Not referenced by any Profile in Project"
-                f" {project_name})</em>",
+                f" '{project_name}')</em>",
             ]
 
             # Output the Task (we don't care about the returned value)
             our_task = PrimeItems.tasker_root_elements["all_tasks"][the_id]
             tasks.output_task_list(
                 [our_task],
                 project_name,
                 "",
                 task_output_lines,
                 found_tasks,
                 True,
             )
 
+        # Determine if we are to count this Task toward our total if doing a single Profile
+        elif PrimeItems.found_named_items["single_profile_found"] and the_id in found_tasks:
+            PrimeItems.named_task_count_total += 1
+
     return have_tasks_not_in_profile
 
 
 # ##################################################################################
 # Process all Tasks in Project that are not referenced by a Profile
 # ##################################################################################
 def tasks_not_in_profiles(
@@ -228,15 +300,14 @@
         have_tasks_not_in_profile,
     )
 
     # End the twisty hidden lines if we have Tasks not in any Profile
     if PrimeItems.program_arguments["twisty"]:
         if have_tasks_not_in_profile:
             remove_twisty()
-        # Add additional </ul> if no Tasks not in any Profile
         else:
             PrimeItems.output_lines.add_line_to_output(3, "", FormatLine.dont_format_line)
 
     # Force a line break
     PrimeItems.output_lines.add_line_to_output(0, "", FormatLine.dont_format_line)
     return have_tasks_not_in_profile
 
@@ -279,39 +350,47 @@
         f"Project: {project_name_altered}",
         True,
     )
 
     # Set up the final Project output line and add a "Go to top" hyperlink
     final_project_line = f"{project_name_details} {launcher_task_info}{priority}{kid_app_info}"
     if len(final_project_line) < 70:
-        final_project_line = f"{final_project_line}{blank * 20}<a href='#'>Go to top</a>"
+        final_project_line = f"{final_project_line}{blank * 20}<a href='#'>Go to top</a><br>"
     else:
-        final_project_line = f"{final_project_line}{blank * 5}<a href='#'>Go to top</a>"
+        final_project_line = f"{final_project_line}{blank * 5}<a href='#'>Go to top</a><br>"
+
+    # Pretty it up?
+    if PrimeItems.program_arguments["pretty"]:
+        indent_amt = len(project_name) + 5
+        # Break at comma
+        final_project_line = final_project_line.replace(", ", f", <br>{blank*indent_amt}")
+        # Break at bracket
+        final_project_line = final_project_line.replace(" [", f"<br>{blank*indent_amt} [")
 
     # Are we looking for a specific Project?
     if PrimeItems.program_arguments["single_project_name"]:
         if project_name != PrimeItems.program_arguments["single_project_name"]:
             return True
         # We found our single Project
         PrimeItems.found_named_items["single_project_found"] = True
         # Clear the output and just put out our Project.
         PrimeItems.output_lines.refresh_our_output(
             False,
             project_name,
             "",
         )
+        # Okay, we've output the Project name.  Get rid of just the Project name (and then add the full Project line).
+        _ = PrimeItems.output_lines.output_lines.pop()
+
+    PrimeItems.output_lines.add_line_to_output(
+        2,
+        final_project_line,
+        FormatLine.dont_format_line,
+    )
 
-    # Not looking for single Project.  Go ahead and output it.
-    else:
-        # Output the final Project text
-        PrimeItems.output_lines.add_line_to_output(
-            2,
-            final_project_line,
-            FormatLine.dont_format_line,
-        )
     return False
 
 
 # ##################################################################################
 # Initialize out grand total counters
 # ##################################################################################
 def setup_summary_counts() -> int:
@@ -348,37 +427,35 @@
     # Accumulate totals for final tally
     PrimeItems.grand_totals["projects"] += 1
     PrimeItems.grand_totals["profiles"] += profile_count
     PrimeItems.grand_totals["unnamed_tasks"] += task_count_unnamed
     PrimeItems.grand_totals["named_tasks"] += named_task_count_total
     PrimeItems.grand_totals["scenes"] += scene_count
 
-    # If doing twisties,  prior line is a <ul> and line before that a </ul>,
-    # delete the <ul> since there are one too many
-    if (
-        PrimeItems.program_arguments["twisty"]
-        and PrimeItems.output_lines.output_lines[-1][:4] == "<ul>"
-        and PrimeItems.output_lines.output_lines[-2][:5] == "</ul>"
-    ):
-        PrimeItems.output_lines.delete_last_line()
-
     # Output the summary line with counts
     PrimeItems.output_lines.add_line_to_output(
         5,
         (
-            f"Project {project_name} has a total of {profile_count} Profiles,"
+            f"<DIV {NORMAL_TAB}<br>Project {project_name} has a total of {profile_count} Profiles,"
             f" {task_count_for_profile}  Tasks called by Profiles,"
             f" {task_count_unnamed} unnamed Tasks, {task_count_no_profile} Tasks"
             f" not in any Profile, {named_task_count_total} named Tasks out of"
             f" {task_count_unnamed + named_task_count_total} total Tasks,"
-            f" and {scene_count} Scenes<br><br>"
+            f" and {scene_count} Scenes</DIV><br><br>"
         ),
         ["", "project_color", FormatLine.add_end_span],
     )
 
+    # Print a ruler
+    PrimeItems.output_lines.add_line_to_output(
+        5,
+        "<hr>",
+        FormatLine.dont_format_line,
+    )
+
 
 # ##################################################################################
 # Output the remaining components related to the Project
 # ##################################################################################
 def finish_up(
     project: defusedxml.ElementTree.XML,
     project_name: str,
@@ -433,57 +510,88 @@
     # If we are not inserting the twisties, then close the unordered list
     # Twisties screw with the indentation, as well as not having Scenes
     if not PrimeItems.program_arguments["twisty"] and (
         PrimeItems.program_arguments["display_detail_level"] > 0 or not have_scenes
     ):
         PrimeItems.output_lines.add_line_to_output(3, "", FormatLine.dont_format_line)  # Close Profile list
 
-    return
-
 
 # ##################################################################################
 # Helper functions to process_projects function, below
 # ##################################################################################
 # Return the flags for single-task-found and single-profile-found
 def is_single_task_or_profile_found() -> bool:
+    """
+    Check if a single task or profile is found and return a boolean value.
+    """
     return PrimeItems.found_named_items["single_task_found"] or PrimeItems.found_named_items["single_profile_found"]
 
 
+# ##################################################################################
+# Retrieves profile IDs for a given project and project name, excluding projects without profiles.
+# ##################################################################################
 def get_profile_ids(
     project: defusedxml.ElementTree.XML,
     project_name: str,
     projects_without_profiles: list,
 ) -> list:
+    """
+    Retrieves profile IDs for a given project and project name, excluding projects without profiles.
+
+    :param project: XML element representing the project
+    :param project_name: string representing the name of the project
+    :param projects_without_profiles: list of projects without profiles
+    :return: list of profile IDs
+    """
     return get_ids(True, project, project_name, projects_without_profiles)
 
 
+# ##################################################################################
+# Check if a single profile is not found based on program arguments and named items.
+# ##################################################################################
 # Return True if we are doing a single Profile and it was not found, False otherwise
 def is_single_profile_not_found() -> bool:
+    """
+    Check if a single profile is not found based on program arguments and named items.
+    Return a boolean indicating whether a single profile is not found.
+    """
     return (
         PrimeItems.program_arguments["single_profile_name"] and not PrimeItems.found_named_items["single_profile_found"]
     )
 
 
-def add_no_profiles_line_to_output():
+# ##################################################################################
+# Add a line to the output with the message "<em>Project has no Profiles</em>" and some formatting.
+# ##################################################################################
+def add_no_profiles_line_to_output() -> None:
+    """
+    Add a line to the output with the message "<em>Project has no Profiles</em>" and some formatting.
+    """
     PrimeItems.output_lines.add_line_to_output(
         5,
-        "<em>Project has no Profiles</em>",
+        f"{NORMAL_TAB}<em>Project has no Profiles</em>",
         ["", "profile_color", FormatLine.add_end_span],
     )
 
 
 def is_single_project_or_profile_or_task_found() -> bool:
+    """
+    Check if a single project, profile, or task is found and return a boolean.
+    """
     return (
         PrimeItems.found_named_items["single_project_found"]
         or PrimeItems.found_named_items["single_profile_found"]
         or PrimeItems.found_named_items["single_task_found"]
     )
 
 
-def add_close_project_list_line_to_output():
+def add_close_project_list_line_to_output() -> None:
+    """
+    Add a close project list line to the output.
+    """
     PrimeItems.output_lines.add_line_to_output(3, "", FormatLine.dont_format_line)
 
 
 # ################################################################################
 # Get this Project's details and output them
 # ################################################################################
 def get_profile_details_and_output(project: str, project_name: str) -> tuple[bool, int, str, bool]:
@@ -512,22 +620,19 @@
 
     # Check for extra details to include.
     # This comes back as True if we have the specific Project we are looking for.
     have_project_wanted = get_extra_and_output_project(project, project_name, launcher_task_info)
 
     # Process Project Properties
     if PrimeItems.program_arguments["display_detail_level"] > 2:
-        get_properties(
-            project,
-            "project_color",
-        )
+        get_properties("Project:", project)
 
     # Process TaskerNet details if requested
     if PrimeItems.program_arguments["taskernet"]:
-        share(project)
+        share(project, "projtab")
 
     return False, profile_count, have_project_wanted
 
 
 # ################################################################################
 # Process all of the Profiles for this Project
 # ################################################################################
```

### Comparing `maptasker-2.6.3/maptasker/src/runcli.py` & `maptasker-3.2.2/maptasker/src/runcli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Process command line interface arguments for MapTasker"""
+
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
 # runcli: process command line interface arguments for MapTasker                       #
 #                                                                                      #
 # Add the following statement (without quotes) to your Terminal Shell config file.     #
@@ -22,14 +23,15 @@
 import sys
 from collections import namedtuple
 
 import darkdetect
 
 from maptasker.src.clip import clip_figure
 from maptasker.src.colors import get_and_set_the_color, validate_color
+from maptasker.src.config import DEFAULT_DISPLAY_DETAIL_LEVEL
 from maptasker.src.error import error_handler
 from maptasker.src.getputer import save_restore_args
 from maptasker.src.initparg import initialize_runtime_arguments
 from maptasker.src.parsearg import runtime_parser
 from maptasker.src.primitem import PrimeItems
 from maptasker.src.rungui import process_gui
 from maptasker.src.sysconst import (
@@ -41,23 +43,23 @@
     logger,
 )
 
 
 # ################################################################################
 # Determine if the argument is a list or string, and return the value as appropriate
 # ################################################################################
-def get_arg_if_in_list(args: namedtuple("ArgNamespace", ["some_arg", "another_arg"]), the_argument: str) -> int:
+def get_arg_if_in_list(args: list, the_argument: str) -> int:
     """
     Determine if the argument is a list or string, and return the value as appropriate
         Args:
             args (Namespace): the args Namespace from either argparse or unit_test
             the_argument (str): the arguemnt to get
 
         Returns:
-            int: the numeric value for the argument that was gotten
+            tuple: boolean True if it is a list and the numeric value for the argument that was gotten
     """
     if the_value := getattr(args, the_argument):
         return int(the_value[0]) if isinstance(the_value, list) else int(the_value)
 
     return the_value
 
 
@@ -80,31 +82,31 @@
         if attribute in valid_attributes:
             PrimeItems.program_arguments[attribute] = True
 
 
 # ##################################################################################
 # Go through all boolean settings, get each and if have it then set value to True
 # ##################################################################################
-def get_and_set_booleans(args: namedtuple("ArgNamespace", ["some_arg", "another_arg"])) -> None:
+def get_and_set_booleans(args: list) -> None:
     """
     Go through all boolean settings, get each and if have it then set value to True
         Args:
             args (namedtuple): runtime arguments namespace
     """
     # Program runtime boolean arguments (long form and short form per argparse.py)
     boolean_arguments = {
         "conditions": "",
         "debug": "",
         "directory": "",
         "everything": "e",
         "outline": "o",
+        "pretty": "",
         "preferences": "",
-        "restore": "",
+        "reset": "",
         "runtime": "",
-        "save": "s",
         "taskernet": "",
         "twisty": "",
     }
 
     # Loop through all possible boolean program arguments and get/set each
     # Check both the long name (key) and the short name (value)
     # NOTE: We can not use an either/or combination if statement to test both the
@@ -119,97 +121,188 @@
                 if value and getattr(args, value):
                     PrimeItems.program_arguments[key] = True
 
 
 # ##################################################################################
 # Get the the other arguments
 # ##################################################################################
-def get_the_other_arguments(args: namedtuple("ArgNamespace", ["some_arg", "another_arg"])) -> None:
+def get_the_other_arguments(args: list) -> None:
     """
     Get the remainder of the arguments
         Args:
             value (str): The attributes to assign to names: (bold, highlight, underline, italicize)
     """
     get_and_set_booleans(args)
 
     # Get display detail level, if provided.
     detail = getattr(args, "detail")
-    if detail is not None and isinstance(detail, int) or (detail := get_arg_if_in_list(args, "detail")):
-        PrimeItems.program_arguments["display_detail_level"] = detail
-
+    if detail is not None:
 
-# ##################################################################################
-# Get our parsed program arguments and save them to PrimeItems.program_args"]
-# ##################################################################################
-def get_runtime_arguments(args: namedtuple("ArgNamespace", ["some_arg", "another_arg"])) -> None:  # noqa: C901
-    """
-    Get our parsed program arguments and save them to PrimeItems.program_args"]
-        Args:
-            args (list): runtime arguments namespace"""
+        if isinstance(detail, int):
+            PrimeItems.program_arguments["display_detail_level"] = detail
+        elif isinstance(detail, list):
+            PrimeItems.program_arguments["display_detail_level"] = detail[0]
 
-    # Color help?
-    if getattr(args, "ch"):
-        validate_color("h")
 
-    # Not GUI.  Get input from command line arguments
-
-    # Get input from command line arguments or unit test defaults.
-    # All booleans and display detail level.
-    get_the_other_arguments(args)
-
-    program_arguments = PrimeItems.program_arguments
-
-    # Everything? Display full detail and set various display optionsm to true.
-    if getattr(args, "e"):
-        program_arguments["display_detail_level"] = 4
-        program_arguments["conditions"] = True
-        program_arguments["preferences"] = True
-        program_arguments["directory"] = True
-        program_arguments["taskernet"] = True
-        program_arguments["outline"] = True
-        program_arguments["runtime"] = True
+def set_everything(program_arguments: dict) -> None:
+    """
+    Establish all of the settings that covers "everything" selection.
+        program_arguments (dict): The program arguments.
 
+    Returns:
+        None
+    """
+    program_arguments["display_detail_level"] = DEFAULT_DISPLAY_DETAIL_LEVEL
+    program_arguments["conditions"] = True
+    program_arguments["preferences"] = True
+    program_arguments["directory"] = True
+    program_arguments["taskernet"] = True
+    program_arguments["outline"] = True
+    program_arguments["runtime"] = True
+    program_arguments["pretty"] = True
+
+
+def get_single_name(program_arguments: dict, args: list) -> None:
+    """
+    A function that extracts single names from the provided arguments and updates the program arguments accordingly.
+    Args:
+        program_arguments (dict): Dictionary to store extracted names.
+        args (list): List of arguments to extract names from.
+    Returns:
+        None
+    """
     the_name = getattr(args, "project")  # Display single Project
     if the_name is not None:
         program_arguments["single_project_name"] = the_name[0]
     the_name = getattr(args, "profile")  # Display single Profile
     if the_name is not None:
         program_arguments["single_profile_name"] = the_name[0]
     the_name = getattr(args, "task")  # Display single task
     if the_name is not None:
         program_arguments["single_task_name"] = the_name[0]
+
+
+def get_android_settings(program_arguments: dict, args: list) -> None:
+    """
+    A function to get Android settings based on the provided arguments.
+    Args:
+        program_arguments (dict): Dictionary to store the extracted Android settings.
+        args (list): List of arguments to extract Android settings from.
+    Returns:
+        None
+    """
+    if value := getattr(args, "android_ipaddr"):
+        if isinstance(value, list):
+            program_arguments["android_ipaddr"] = value[0]
+            program_arguments["android_port"] = getattr(args, "android_port")[0]
+            program_arguments["android_file"] = getattr(args, "android_file")[0]
+        else:
+            program_arguments["android_ipaddr"] = value
+            program_arguments["android_port"] = getattr(args, "android_port")
+            program_arguments["android_file"] = getattr(args, "android_file")
+
+
+def process_extended_arguments(args: list) -> None:
+    """
+    Process extended arguments from the command line.
+
+    Args:
+        args (list): A list of command line arguments.
+
+    Returns:
+        None: This function does not return anything.
+
+    This function processes extended arguments from the command line and updates the program arguments accordingly.
+    It handles special cases and non-binary settings.
+
+    - If the 'e' argument is present, it sets the program arguments to display full detail and sets various display options to true.
+    - If there is a single name (Project/Profile/Task) present in the command line arguments, it gets it.
+    - If the 'v' argument is present, it displays version info.
+    - If the 'names' argument is present, it gets the name attributes.
+    - If the 'appearance' argument is present, it sets the appearance mode in the program arguments.
+    - If the 'i' argument is present, it sets the indentation amount in the program arguments.
+    - If the 'font' argument is present, it sets the font in the program arguments.
+    - If the 'file' argument is present, it sets the file in the program arguments.
+
+    Note:
+        The function assumes that the 'program_arguments' attribute is present in the 'PrimeItems' class.
+    """
+    program_arguments = PrimeItems.program_arguments
+
+    # The rest of this function is to handle special cases and non-binary settings.
+
+    # Everything? Display full detail and set various display options to true.
+    if getattr(args, "e"):
+        set_everything(program_arguments)
+
+    # If there is a single name (Project/Profile/Task), then get it.
+    get_single_name(program_arguments, args)
+
     if getattr(args, "v"):  # Display version info
         display_version()
 
     # Get names (bold, highlight, underline and/or highlight)
     if value := getattr(args, "names"):
         get_name_attributes(value)
 
     # Get Android device info for fetching the backup xml file
-    if value := getattr(args, "android_ipaddr"):
-        program_arguments["android_ipaddr"] = value[0]
-        program_arguments["android_port"] = getattr(args, "android_port")[0]
-        program_arguments["android_file"] = getattr(args, "android_file")[0]
-
+    get_android_settings(program_arguments, args)
 
     # Appearance
     if appearance := getattr(args, "appearance"):
         program_arguments["appearance_mode"] = appearance
 
     # Indentation amount
     if indent := get_arg_if_in_list(args, "i"):
         program_arguments["indent"] = indent
 
     # Font
-    if font := getattr(args, "f"):
+    if font := getattr(args, "font"):
         if isinstance(font, list):
             program_arguments["font"] = font[0]
         else:
             program_arguments["font"] = font
 
+    # File
+    if file := getattr(args, "file"):
+        if isinstance(file, list):
+            program_arguments["file"] = file[0]
+        else:
+            program_arguments["file"] = file
+
+
+# ##################################################################################
+# Get our parsed program arguments and save them to PrimeItems.program_args"]
+# ##################################################################################
+def get_runtime_arguments(args: list) -> None:
+    """
+    Function to get runtime arguments from the command line.
+
+    Parameters:
+        args (list): A list of command line arguments.
+
+    Returns:
+        None: This function does not return anything.
+
+    The code defines a function get_runtime_arguments to retrieve runtime arguments from the command line,
+    process boolean values, display detail level, and non-binary arguments from a list of command line arguments.
+    It does not return any value.
+    """
+    # Color help?
+    if getattr(args, "ch"):
+        validate_color("h")
+
+    # Not GUI.  Get input from command line arguments or unit test defaults.
+
+    # All booleans and display detail level.
+    get_the_other_arguments(args)
+
+    # Get non-binary arguments
+    process_extended_arguments(args)
+
 
 # ##################################################################################
 # Add some pazaazz to the version identiifer
 # ##################################################################################
 def display_version() -> None:
     """
     Display the version of the program.
@@ -233,17 +326,17 @@
 ██╔████╔██║███████║██████╔╝       ██║   ███████║███████╗█████╔╝ █████╗  ██████╔╝
 ██║╚██╔╝██║██╔══██║██╔═══╝        ██║   ██╔══██║╚════██║██╔═██╗ ██╔══╝  ██╔══██╗
 ██║ ╚═╝ ██║██║  ██║██║            ██║   ██║  ██║███████║██║  ██╗███████╗██║  ██║
 ╚═╝     ╚═╝╚═╝  ╚═╝╚═╝            ╚═╝   ╚═╝  ╚═╝╚══════╝╚═╝  ╚═╝╚══════╝╚═╝  ╚═╝
 
 """
     color_to_use = Colors.Yellow if darkdetect.isDark() else Colors.Blue
-    print(header)  # noqa: T201
-    print(f"{color_to_use}{MY_VERSION}, under license {MY_LICENSE}\033[0m")  # noqa: T201
-    print("")  # noqa: T201
+    print(header)
+    print(f"{color_to_use}{MY_VERSION}, under license {MY_LICENSE}\033[0m")
+    print("")
     clip_figure("castles", False)
     sys.exit(0)
 
 
 # ##################################################################################
 # Get arguments from command line and put them to the proper settings
 # ##################################################################################
@@ -275,14 +368,15 @@
 # Get arguments from saved file and restore them to the proper settings
 # ##################################################################################
 def restore_arguments() -> dict:
     """
     Get arguments from saved file and restore them to the proper settings
     """
     temp_arguments = temp_colors = {}
+    # Get the arguments from our saved settings file.
     temp_arguments, temp_colors = save_restore_args(temp_arguments, temp_colors, False)
 
     # We will get a Keyerror if the restore file does not exist
     with contextlib.suppress(KeyError):
         for (
             key,
             value,
@@ -300,17 +394,20 @@
             if key is not None:
                 PrimeItems.colors_to_use[key] = value
 
     return
 
 
 # ##################################################################################
-# We're running a unit test. Get the unit test arguments and create the arg namespace
+# Unit tests...
+# We're running a unit test. Get the unit test arguments and create the arg namespace.
+# We do this so that 1) we can run a unit test without command line arguments, and
+# 2) we can rerun over and over as many times as needed.
 # ##################################################################################
-def unit_test() -> namedtuple("ArgNamespace", ["some_arg", "another_arg"]):
+def unit_test() -> namedtuple:  # noqa: PYI024
     """
     We're running a unit test. Get the unit test arguments and create the arg namespace
             :return: args Namespace with arguments from run_test.py
     """
     single_names = ["project", "profile", "task"]
 
     class Namespace:
@@ -330,15 +427,14 @@
         android_file="",
         android_port="",
         cAction=None,
         cActionCondition=None,
         cActionLabel=None,
         cActionName=None,
         cBackground=None,
-        cBullet=None,
         cDisabledAction=None,
         cDisabledProfile=None,
         ch=False,
         cHeading=None,
         cHighlight=None,
         cLauncherTask=None,
         conditions=False,
@@ -351,33 +447,33 @@
         cTaskerNetInfo=None,
         cTrailingComments=None,
         cUnknownTask=None,
         debug=True,
         detail=3,
         directory=False,
         e=False,
-        f="Courier",
+        file="",
+        font="Courier",
         g=False,
         i=4,
         names=False,
         o=False,
         p=False,
+        pretty=False,
         profile=None,
         project=None,
         reset=False,
-        restore=False,
         runtime=False,
-        s=False,
         task=None,
         taskernet=False,
         twisty=False,
         v=False,
     )
     # Go through each argument from runtest
-    print("Running Unit Test.")  # noqa: T201
+    print("Running Unit Test.")
     for the_argument in sys.argv:
         if the_argument == "-test=yes":  # Remove unit test trigger
             continue
         new_arg = the_argument.split("=")
 
         # Handle boolean (True) values and colors
         if len(new_arg) == 1:
@@ -413,15 +509,15 @@
 
         Returns:
             Nothing"""
     program_arguments = PrimeItems.program_arguments
     # It doesn't make sense to do twisties if notr displaying full detail.
     if program_arguments["display_detail_level"] < 3 and program_arguments["twisty"]:
         message = "Twisty disabled since the display level is not 3 or above."
-        print(f"{Colors.Yellow}{message}")  # noqa: T201
+        print(f"{Colors.Yellow}{message}")
         logger.info(message)
 
 
 # ##################################################################################
 # Get the program arguments from command line or via unit test (e.g. python mapit.py -x)
 # ##################################################################################
 # Command line parameters
@@ -432,37 +528,44 @@
             pi (PrimeItems): Primary Items class object
 
         Returns:
             None
     """
     gui_flag = "g"
     reset_flag = "reset"
+    version_flag = "v"
 
-    # Intialize runtime arguments if we don't yet have them.
-    if not PrimeItems.colors_to_use:
-        PrimeItems.program_arguments = initialize_runtime_arguments()
+    # Intialize runtime arguments.
+    PrimeItems.program_arguments = initialize_runtime_arguments()
 
-    # Process unit tests if "-test" in arguments, else get normal runtime arguments.
+    # Process unit tests if "-test" in arguments, else get normal runtime arguments via Parsearg.
     args = unit_test() if "-test=yes" in sys.argv else runtime_parser()
+
     logger.debug(f"Program arguments: {args}")
 
-    # Restore runtime arguments if we are not doing a reset and not doing the GUI and there is a restore file.
+    # Restore runtime arguments if we are not doing a reset and not doing the GUI and there is a settings file to restore.
     # If doing thew GUI, then the arguments are restored by userintr.py
     PrimeItems.program_arguments["reset"] = getattr(args, reset_flag)
     PrimeItems.program_arguments["gui"] = getattr(args, gui_flag)
+    save_gui = PrimeItems.program_arguments["gui"]
     if (
         not PrimeItems.program_arguments["reset"]
         and not PrimeItems.program_arguments["gui"]
         and os.path.isfile(ARGUMENTS_FILE)
     ):
         restore_arguments()
+
+        # Restore the GUI flag.
+        PrimeItems.program_arguments["gui"] = save_gui  # Restore GUI flag from runtime options,
+
         PrimeItems.program_arguments["rerun"] = False  # Make sure this is off!  Loops otherwise.
 
     # If using the GUI, them process the GUI.
-    if PrimeItems.program_arguments["gui"]:  # GUI for input?
+    do_version = getattr(args, version_flag)
+    if PrimeItems.program_arguments["gui"] and not do_version:  # GUI for input?
         (
             PrimeItems.program_arguments,
             PrimeItems.colors_to_use,
         ) = process_gui(True)
 
     # Not doing the GUI.  Process commands from command line.
     else:
```

### Comparing `maptasker-2.6.3/maptasker/src/rungui.py` & `maptasker-3.2.2/maptasker/src/rungui.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,63 +12,103 @@
 # GNU General Public License v3.0                                                      #
 # Permissions of this strong copyleft license are conditioned on making available      #
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
+from __future__ import annotations
+
 import contextlib
-import tkinter
+import sys
 
 from maptasker.src.colrmode import set_color_mode
 from maptasker.src.error import error_handler
+from maptasker.src.getputer import save_restore_args
 from maptasker.src.initparg import initialize_runtime_arguments
 from maptasker.src.primitem import PrimeItems
-from maptasker.src.getputer import save_restore_args
 from maptasker.src.sysconst import ARGUMENT_NAMES, logger
-import sys
 
 
 # ################################################################################
 # Convert a value to integere, and if not an integer then use default value
 # ################################################################################
 def convert_to_integer(value_to_convert: str, default_value: int) -> int:
     """
     Convert a value to integere, and if not an integer then use default value
         Args:
             value_to_convert (str): The string value to convert to an integer
             where_to_put_it (int): Where to place the converted integer
-            default_value (int):The default to plug in if the value to convert
+            default_value (int): The default to plug in if the value to convert
                 is not an integer
             :return: converted value as integer"""
     try:
         return int(value_to_convert)
     except (ValueError, TypeError):
         return default_value
 
 
 # ##################################################################################
+# Get the colors to use.
+# ##################################################################################
+def do_colors(user_input: dict) -> dict:
+    """Sets color mode and processes colors.
+    Parameters:
+        - user_input (dict): User input dictionary containing appearance mode and color lookup.
+    Returns:
+        - colormap (dict): Dictionary of colors after processing.
+    Processing Logic:
+        - Set color mode based on user input.
+        - Process color lookup if provided.
+        - Set flag for GUI usage."""
+
+    # Appearance change: Dark or Light mode?
+    colormap = set_color_mode(user_input.appearance_mode)
+
+    # Process the colors
+    if user_input.color_lookup:
+        for key, value in user_input.color_lookup.items():
+            colormap[key] = value
+
+    PrimeItems.program_arguments["gui"] = True  # Set flag to indicate we are using GUI
+
+    return colormap
+
+
+# ##################################################################################
 # Get the program arguments from GUI
 # ##################################################################################
 def process_gui(use_gui: bool) -> tuple[dict, dict]:
-    """
-    Present the GUI and get the runtime details
-        :param pi: Primary Items instance
-        :param use_gui: flag if usijng the GUI, make sure we import it
-        :return: program runtime arguments and colors to use in the output
-    """
     # global MyGui
+    """Parameters:
+        - use_gui (bool): Flag to indicate whether to use GUI or not.
+    Returns:
+        - tuple[dict, dict]: Tuple containing program arguments and colors to use.
+    Processing Logic:
+        - Import MyGui if use_gui is True.
+        - Set flag to indicate GUI usage.
+        - Delete previous Tkinter window if it exists.
+        - Display GUI and get user input.
+        - Initialize runtime arguments if not already set.
+        - If user clicks "Exit" button, save settings and exit program.
+        - If user closes window, cancel program.
+        - If user clicks "Run" button, get input from GUI variables.
+        - Set program arguments in dictionary.
+        - Convert display_detail_level and indent to integers.
+        - Get font from GUI.
+        - Return program arguments and colors to use."""
     if use_gui:
         from maptasker.src.userintr import MyGui
 
     PrimeItems.program_arguments["gui"] = True  # Set flag to indicate we are using GUI
 
     # Get rid of any previous Tkinter window
     if PrimeItems.tkroot is not None:
         del PrimeItems.tkroot
+        PrimeItems.tkroot = None
     # Display GUI and get the user input
     user_input = MyGui()
     user_input.mainloop()
 
     # Establish our runtime default values if we don't yet have 'em.
     if not PrimeItems.colors_to_use:
         PrimeItems.program_arguments = initialize_runtime_arguments()
@@ -77,15 +117,15 @@
     if user_input.exit:
         # Save our runtime settings for next time.
         _, _ = save_restore_args(PrimeItems.program_arguments, PrimeItems.colors_to_use, True)
         # Spit out the message and log it.
         error_handler("Program exited. Goodbye.", 0)
         sys.exit(0)
 
-    # User has either closed the window.
+    # Has the user closed the window?
     if not user_input.go_program and not user_input.rerun:
         error_handler("Program cancelled by user (killed GUI)", 99)
 
     # 'Run' button hit.  Get all the input from GUI variables
     PrimeItems.program_arguments["gui"] = True
     # Do we already have the file object?
     if value := user_input.file:
@@ -104,21 +144,9 @@
     )
     # Convert indent to integer
     PrimeItems.program_arguments["indent"] = convert_to_integer(PrimeItems.program_arguments["indent"], 4)
     # Get the font
     if the_font := user_input.font:
         PrimeItems.program_arguments["font"] = the_font
 
-    # Appearance change: Dark or Light mode?
-    colormap = set_color_mode(user_input.appearance_mode)
-
-    # Process the colors
-    if user_input.color_lookup:
-        for key, value in user_input.color_lookup.items():
-            colormap[key] = value
-
-    PrimeItems.program_arguments["gui"] = True  # Set flag to indicate we are using GUI
-
-    return (
-        PrimeItems.program_arguments,
-        colormap,
-    )
+    # Return the program arguments and colors to use.
+    return (PrimeItems.program_arguments, do_colors(user_input))
```

### Comparing `maptasker-2.6.3/maptasker/src/scenes.py` & `maptasker-3.2.2/maptasker/src/xmldata.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,270 +1,254 @@
+"""Module containing action runner logic."""
+
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
-# scenes: Process the Tasker Scene passed as input                                     #
+# xmldata: deal with the xml data                                                      #
 #                                                                                      #
+# GNU General Public License v3.0                                                      #
 # Permissions of this strong copyleft license are conditioned on making available      #
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
-import contextlib
+import os
+import shutil
 
-import defusedxml.ElementTree  # Need for type hints
+import defusedxml.ElementTree
 
-import maptasker.src.tasks as tasks
-from maptasker.src.dirout import add_directory_item
 from maptasker.src.primitem import PrimeItems
-from maptasker.src.proclist import process_list
-from maptasker.src.sysconst import FormatLine
-from maptasker.src.xmldata import tag_in_type
-
-SCENE_TASK_TYPES = {
-    "checkchangeTask": "Check Change",
-    "clickTask": "TAP",
-    "focuschangeTask": "Focus Change",
-    "itemselectedTask": "Item Selected",
-    "keyTask": "Key",
-    "linkclickTask": "Link",
-    "longclickTask": "LONG TAP",
-    "mapclickTask": "Map",
-    "maplongclickTask": "Long Map",
-    "pageloadedTask": "Page Load",
-    "strokeTask": "STROKE",
-    "valueselectedTask": "Value Selected",
-    "videoTask": "Video",
-    "itemclickTask": "ITEM TAP",
-    "itemlongclickTask": "ITEM LONG TAP",
-}
-SCENE_TAGS_TO_IGNORE = [
-    "cdate",
-    "edate",
-    "heightLand",
-    "nme",
-    "widthLand",
-]
+from maptasker.src.sysconst import clean
 
 
 # ##################################################################################
-# Get the Scene's geometry
+# See if the xml tag is one of the predefined types and return result
 # ##################################################################################
-def get_geometry(scene_element: defusedxml.ElementTree.XML) -> tuple[str, str]:
-    """
-    Get the Scene's geometry
-        :param scene_element: xml element of the Scene <Scene sr="scene...
-        :return: width and height
+def tag_in_type(tag: str, flag: bool) -> bool:
     """
-    height = width = "none"
-    height = scene_element.find("heightPort")
-    if height is not None:
-        height = height.text
-    width = scene_element.find("widthPort")
-    if width is not None:
-        width = width.text
-    return width, height
+    Evaluate the xml tag to see if it is one of our predefined types
+
+    Parameters: the tag to evaluate, and whether this is a Scene or not (which
+            determines which list of types to look for)
+
+    Returns: True if tag found, False otherwise
+    """
+    scene_task_element_types = [
+        "ListElementItem",
+        "ListElement",
+        "TextElement",
+        "ImageElement",
+        "ButtonElement",
+        "OvalElement",
+        "EditTextElement",
+        "RectElement",
+        "WebElement",
+        "CheckBoxElement",
+        "DoodleElement",
+        "PickerElement",
+        "SceneElement",
+        "SliderElement",
+        "SpinnerElement",
+        "SwitchElement",
+        "ToggleElement",
+        "VideoElement",
+        "PropertiesElement",  # this element doesn't contain anything of value/import
+    ]
+    scene_task_click_types = [
+        "checkchangeTask",
+        "clickTask",
+        "focuschangeTask",
+        "itemselectedTask",
+        "keyTask",
+        "linkclickTask",
+        "longclickTask",
+        "mapclickTask",
+        "maplongclickTask",
+        "pageloadedTask",
+        "strokeTask",
+        "valueselectedTask",
+        "videoTask",
+        "itemclickTask",
+        "itemlongclickTask",
+    ]
+    # Return a boolean: True if tag found in the appropriate list, False otherwise
+    return flag and tag in scene_task_element_types or not flag and tag in scene_task_click_types  # Boolean
 
 
 # ##################################################################################
-# Get the Scene's elements
-# ##################################################################################
-def get_scene_elements(
-    child: defusedxml.ElementTree,
-) -> None:
-    """
-    Go through Scene's <xxxElement> tags and output them
-        :param child: pointer to '<xxxElement' Scene xml statement
-        :return: nothing
+# We have an integer.  Evaluaate it's value based oon the code's evaluation parameters.
+# ##################################################################################
+def extract_integer(action: defusedxml.ElementTree.XML, arg: str, argeval: str) -> str:
+
+    # Don't move import to avoid cirtcular import
     """
-    element_type = child.tag.split("Element")
-    # First string is the name of the element
-    name_xml_element = child.find("Str")
-    # Get the element's geometry
-    geometry_xml_element = child.find("geom").text
-    geometry = geometry_xml_element.split(",")
-    element_name = name_xml_element.text
-    PrimeItems.output_lines.add_line_to_output(
-        0,
-        (
-            f"&nbsp;&nbsp;&nbsp;Element: {element_type[0]} named"
-            f" {element_name} ...with geometry"
-            f" {geometry[0]}x{geometry[1]} {geometry[2]}x{geometry[3]}"
-        ),
-        ["", "scene_color", FormatLine.add_end_span],
-    )
-
-    # Check to see if this Scene has a layout Scene, and deal with it if so.
-    if sub_scene := child.find("Scene"):
-        sub_scene_element = sub_scene.find("Scene")
-        width, height = get_geometry(sub_scene_element)
-        PrimeItems.output_lines.add_line_to_output(
-            0,
-            (
-                "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Element has an item 'Layout'"
-                f" (Scene) with width/height {width} X {height}"
-            ),
-            ["", "scene_color", FormatLine.add_end_span],
-        )
-    return
+    Extract an integer value from an XML action element
+    Args:
+        action: {XML element}: The XML action element to search
+        arg: {str}: The name of the argument to search for
+        argeval: {str}: The evaluation to perform on the integer
+    Returns:
+        {str}: The result of the integer evaluation
+    {Processes the XML action element to find the integer value associated with the given argument name.
+    If found, performs the specified evaluation on the integer and returns the result. Returns an empty string if no integer is found.}
+    - Searches child elements of the action for an 'Int' element matching the given argument name
+    - Extracts the integer value or variable name if found
+    - Performs the specified evaluation on the integer/variable, joining results into a string if a list
+    - Returns the result of the evaluation or an empty string if no integer was found
+    """
+    from maptasker.src.action import drop_trailing_comma, process_xml_list
+
+    the_int_value = ""
+    result = []
+    # Find the arg we are looking for.
+    for child in action:
+        if child.tag == "Int":
+            the_arg = child.attrib.get("sr")
+            # Is this our arg?
+            if arg == the_arg:
+
+                # We have the arg we are looking for.
+                if child.attrib.get("val") is not None:
+                    the_int_value = child.attrib.get("val")  # There a numeric value as a string?
+                elif child.find("var") is not None:  # There is a variable name?
+                    the_int_value = child.find("var").text
+                if the_int_value:  # If we have an integer or variable name
+                    # List of options for this Int?
+                    if isinstance(argeval, list):
+                        process_xml_list(
+                            [argeval],
+                            0,
+                            the_int_value,
+                            result,
+                            [arg],
+                        )
+                        result = " ".join(result)
+                    else:  # Not a list
+                        result = argeval + the_int_value  # Just grab the integer value
+                        break
+
+                # No integer value or variable name found
+                else:
+                    result = ""
+
+    # If we have a result, get rid of the trailing comma if there is one.
+    if result:
+        return drop_trailing_comma([result])[0]
+
+    return ""  # No Integer value or variable found...return empty
 
 
 # ##################################################################################
-# Pull out the screen widsth and height
-# ##################################################################################
-def get_width_and_height(
-    scene: defusedxml.ElementTree,
-    tasks_found: defusedxml.ElementTree,
-) -> None:
+# Extracts and returns the text from the given argument as a string.
+# ##################################################################################
+def extract_string(action: defusedxml.ElementTree.XML, arg: str, argeval: str) -> str:
     """
-    Go through Scene to obtain it's height and width and output.
-
+    Extracts a string from an XML action element.
     Args:
-        scene (defusedxml.ElementTree): Scene xml element to trundle through.
-        tasks_found (defusedxml.ElementTree): List of Tasks found so far.
-
+        action: XML element to search in one line
+        arg: Name of string argument to search for in one line
+        argeval: Prefix to add to matched string in one line
     Returns:
-        Nothing
+        str: Extracted string with prefix or empty string in one line
+    Processes the XML action element:
+    - Loops through child elements looking for matching "Str" tag
+    - Checks if tag attribute matches arg
+    - Appends child text to list with argeval prefix
+    - Returns first item after processing or empty string
     """
-    for child in scene:
-        if child.tag in SCENE_TAGS_TO_IGNORE:
-            continue
-        # End of "xxxElement"?
-        if child.tag == "PropertiesElement" and PrimeItems.program_arguments["display_detail_level"] != 2:
-            PrimeItems.output_lines.output_lines.append("<br>")
-
-        elif tag_in_type(child.tag, True):  # xxxElement?
-            # Display the Element details
-            if PrimeItems.program_arguments["display_detail_level"] > 2:
-                get_scene_elements(child)
-
-            # Look for Tasks associated with this element
-            for sub_child in child:  # Go through Element sub-items
-                # Task-Click (<xxxClick>, <xxxTask>, etc.) associated with this
-                #  Scene's element?
-                if tag_in_type(sub_child.tag, False):
-                    # Start Scene's Task list
-                    temp_task_list = [sub_child.text]
-                    if "-" in temp_task_list[0]:
-                        break
-                    # Start a list
-                    PrimeItems.output_lines.add_line_to_output(1, "", FormatLine.dont_format_line)
-                    # Get the name of Task
-                    task_element, name_of_task = tasks.get_task_name(
-                        sub_child.text,
-                        tasks_found,
-                        temp_task_list,
-                        "",
-                    )
-
-                    # reset to task name since get_task_name changes its value
-                    temp_task_list = [sub_child.text]
-                    extra = "&nbsp;&nbsp;ID:"
-                    task_type = "&nbsp;&#45;&#45;Task:" f" {SCENE_TASK_TYPES[sub_child.tag]}{extra}"
-                    # process the Scene's Task
-                    process_list(
-                        task_type,
-                        temp_task_list,
-                        task_element,
-                        tasks_found,
-                    )
-
-                elif sub_child.tag == "Str":
-                    break
+    from maptasker.src.action import drop_trailing_comma
+
+    # TODO Optimize this code to find the argn match
+    match_results = []
+    for child in action:
+        if child.tag == "Str":
+            the_arg = child.attrib.get("sr")
+            if arg == the_arg:
+                if child.text is not None:
+                    # Catch the situation in which a newline has been entered for the value (carriage return)
+                    if child.text == "\n":
+                        match_results.append(f"{argeval}(carriage return)")
+                    else:
+                        match_results.append(f"{argeval}{child.text}")
+                else:
+                    match_results.append("")
+                break  # We have what we want.  Go to next child
+    if match_results:
+        return drop_trailing_comma(match_results)[0]
+    return ""
 
 
 # ##################################################################################
-# Process the Scene
-# ##################################################################################
-def process_scene(
-    my_scene: str,
-    tasks_found: list[str],
-) -> None:
+# Given a string, remove all HTML (anything between < >) tags from it
+# ##################################################################################
+def remove_html_tags(text: str, replacement: str) -> str:
     """
-    Process the Project's Scene(s), one at a time
-
-        :param my_scene: name of Scene to process
-        :param tasks_found: list of Tasks found so far
-        :return:
+    Remove html tags from a string
+    :param text: text from which HTML is to be removed
+    :param replacement: text to replace HTML with, if any
+    :return: the text with HTML removed
     """
+    import re
 
-    scene = PrimeItems.tasker_root_elements["all_scenes"][my_scene]["xml"]
-    # Get the Scene's geometry and display it
-    height, width = get_geometry(scene)
-    PrimeItems.output_lines.add_line_to_output(
-        0,
-        f"&nbsp;Width/Height: {width} X {height}<br>",
-        ["", "scene_color", FormatLine.add_end_span],
-    )
-
-    # Handle directory hyperlink
-    if PrimeItems.program_arguments["directory"]:
-        add_directory_item("scenes", my_scene)
-
-    # Go through all the children of the Scene looking for width/height
-    # and 'click' Tasks
-    get_width_and_height(scene, tasks_found)
-
-    # If we are doing twisties, then we need to close the unordered list.
-    #  (see lineout format_line, where we add a <ul> for this "Scene:" special case)
-    if PrimeItems.program_arguments["twisty"]:
-        PrimeItems.output_lines.add_line_to_output(3, "", FormatLine.dont_format_line)
-
-    return
+    return re.sub(clean, replacement, text)
 
 
 # ##################################################################################
-# Go through all Scenes for Project, get their detail and output it
-# ##################################################################################
-def process_project_scenes(
-    project: defusedxml.ElementTree.XML,
-    our_task_element: defusedxml.ElementTree.XML,
-    found_tasks: list,
-) -> bool:
+# Find Task by name in PrimeItems.tasker_root_elements["all_tasks"]
+# ##################################################################################
+def find_task_by_name(task_name: str) -> defusedxml.ElementTree.XML:
     """
-    Go through all Scenes for Project, get their detail and output it
-        :param project: xml element of Project we are processing
-        :param our_task_element: xml element pointing to our Task
-        :param found_tasks: list of Tasks found so far
-        :return: True if a Scene was output, False if not
+    Find a task by name in the tasker_root_elements["all_tasks"] list
+    :param task_name: name of task to find
+    :return: the task's (root) dictionary pointer, else None
     """
-    scene_names = None
-    PrimeItems.scene_count = 0
-    with contextlib.suppress(Exception):
-        scene_names = project.find("scenes").text
-    if scene_names is not None:
-        scene_list = scene_names.split(",")
-
-        # If 2nd and 3rd last output lines are </ul>, then there is one too many.
-        # Counter by adding a new line for the Scene.
-        if (
-            PrimeItems.output_lines.output_lines[-2][:5] == "</ul>"
-            and PrimeItems.output_lines.output_lines[-3][:5] == "</ul>"
-        ):
-            PrimeItems.output_lines.add_line_to_output(1, "", FormatLine.dont_format_line)
-
-        # If last line in output has an end-ordered-list, then it must have been
-        # for the list of Tasks not found in any Profile...and it has to be removed
-        # to avoid a double end underline causing mis-alignment of Scene:
-        #   statements in output
-        if PrimeItems.output_lines.output_lines[-1] == "</ul>":
-            PrimeItems.output_lines.delete_last_line()
-
-        # If we have at least one Scene, process it
-        if scene_list[0]:
-            PrimeItems.scene_count = len(scene_list)
-            process_list(
-                "Scene:",
-                scene_list,
-                our_task_element,
-                found_tasks,
-            )
-
-            # Force a line break
-            PrimeItems.output_lines.add_line_to_output(0, "", FormatLine.dont_format_line)
-
-            if PrimeItems.program_arguments["display_detail_level"] == 0:
-                # End list if displaying level 0
-                PrimeItems.output_lines.add_line_to_output(3, "", FormatLine.dont_format_line)
+    for task in PrimeItems.tasker_root_elements["all_tasks"]:
+        if PrimeItems.tasker_root_elements["all_tasks"][task]["name"] == task_name:
+            return task
+    return None
+
 
-    return bool(scene_names)
+# ##################################################################################
+# Append file1 to file2
+# ##################################################################################
+def append_files(file1_path: str, file2_path: str) -> None:
+    """Appends the contents of file1 to file2.
+    Parameters:
+        - file1_path (str): Path to file1.
+        - file2_path (str): Path to file2.
+    Returns:
+        - None: No return value.
+    Processing Logic:
+        - Open file1 in read mode.
+        - Open file2 in append mode.
+        - Copy contents of file1 to file2."""
+    with open(file1_path, "r") as file1, open(file2_path, "a") as file2:
+        shutil.copyfileobj(file1, file2)
+
+
+# ##################################################################################
+# The XML file hs incorrect encoding.  Let's read it in and rewrite it correctly.
+# ##################################################################################
+def rewrite_xml(file_to_parse: str) -> None:
+    """Rewrite XML file with UTF-8 encoding.
+    Parameters:
+        - file_to_parse (str): Name of the file to be parsed.
+    Returns:
+        - None: No return value.
+    Processing Logic:
+        - Create new file with UTF-8 encoding.
+        - Append, rename, and remove files.
+        - Remove temporary file."""
+    utf_xml = '<?xml version = "1.0" encoding = "UTF-8" standalone = "no" ?>\n'
+
+    # Create the XML file with the encoding we want
+    with open(".maptasker_tmp.xml", "w") as new_file:
+        new_file.write(utf_xml)
+        new_file.close()
+
+    # Append, rename and remove.
+    append_files(file_to_parse, ".maptasker_tmp.xml")
+    os.remove(file_to_parse)
+    os.rename(".maptasker_tmp.xml", file_to_parse)
+    os.remove(".maptasker_tmp.xml")
```

### Comparing `maptasker-2.6.3/maptasker/src/servicec.py` & `maptasker-3.2.2/maptasker/src/servicec.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     "lcD": {
         "display": "Lock Code",
         "section": 2,
         "num": 19,
     },
     "lae": {
         "display": "Lock On Startup",
-        "section": 1,
+        "section": 2,
         "num": 20,
     },
     "lang": {
         "display": "Language",
         "section": 3,
         "num": 21,
     },
@@ -198,14 +198,19 @@
         },
     },
     "nfcda": {
         "display": "NFC Detection Enabled",
         "section": 4,
         "num": 30,
     },
+    "PREF_START_MONITOR_ON_APP_OPEN": {
+        "display": "Start Monitor On App Open",
+        "section": 4,
+        "num": 30.5,
+    },
     "PREF_KEEP_ACCESSIBILITY_SERVICES_RUNNING": {
         "display": "KEEP ACCESSIBILITY RUNNING",
         "section": 4,
         "num": 31,
     },
     "appcheckMethod": {
         "display": "App Check Method",
@@ -452,15 +457,15 @@
         "num": 66,
     },
     "csnipD": {
         "display": "Camera Delay",
         "section": 9,
         "num": 67,
     },
-    "????????": {
+    "mFn": {
         "display": "Flash Problems",
         "section": 9,
         "num": 68,
     },
     "PREF_ALLOW_INSECURE_TASK_RUN_REQUESTS": {
         "display": "Allow Running Tasks From Insecure Sources",
         "section": 9,
@@ -548,15 +553,15 @@
         "num": 83,
     },
     "fExtCache": {
         "display": "Debug To Internal Storage",
         "section": 12,
         "num": 84,
     },
-    "?????????": {
+    "lEnable": {
         "display": "Popup Errors/Warnings",
         "section": 12,
         "num": 85,
     },
     "PREF_IS_USING_TEST_SERVER": {
         "display": "Use Test Server For Shares",
         "section": 12,
```

### Comparing `maptasker-2.6.3/maptasker/src/share.py` & `maptasker-3.2.2/maptasker/src/share.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Handle TaskerNet "Share" information"""
+
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
 # share: process TaskerNet "Share" information                                         #
 #                                                                                      #
 # GNU General Public License v3.0                                                      #
@@ -10,117 +12,121 @@
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
 import defusedxml.ElementTree  # Need for type hints
 
 from maptasker.src.format import format_html
-from maptasker.src.sysconst import FONT_FAMILY, FormatLine
 from maptasker.src.primitem import PrimeItems
+from maptasker.src.sysconst import FormatLine
 
 
 # ##################################################################################
 # Go through xml <Share> elements to grab and output TaskerNet description and
 # search-on lines.
 # ##################################################################################
 def share(
     root_element: defusedxml.ElementTree.XML,
+    tab: str,
 ) -> None:
     """
     Go through xml <Share> elements to grab and output TaskerNet description and search-on lines
         :param root_element: beginning xml element (e.g. Project or Task)
+        :param tab: "projtab", "proftab" or "tasktab"
     """
     # Get the <share> element, if any
     share_element: defusedxml.ElementTree = root_element.find("Share")
     if share_element is not None:
         #  We have a <Share> .  Find the description
         description_element = share_element.find("d")
         # Process the description
         if description_element is not None:
             description_element_output(
                 description_element,
+                tab,
             )
 
         # Look for TaskerNet search parameters
         search_element = share_element.find("g")
         if search_element is not None and search_element.text:
             # Found search...format and output
             out_string = format_html(
                 "taskernet_color",
                 "",
                 f"\n<br><br>TaskerNet search on: {search_element.text}",
                 True,
             )
+            # Add the tab CSS call to the color.
+            out_string = PrimeItems.output_lines.add_tab(tab, out_string)
             PrimeItems.output_lines.add_line_to_output(2, out_string, FormatLine.dont_format_line)
 
+        # Force a break when done with last Share element, only if there isn't one there already.
+        break_html = "" if PrimeItems.output_lines.output_lines[-1] == "<br>" else "<br>"
+        PrimeItems.output_lines.add_line_to_output(0, f"{break_html}", FormatLine.dont_format_line)
+
+        # Now get rid of the last duplicate <br> lines at the bottom of the output.
+        for num, item in reversed(list(enumerate(PrimeItems.output_lines.output_lines))):
+            if "TaskerNet description:" in item:
+                break
+            if item == "<br>" and PrimeItems.output_lines.output_lines[num - 1] == "<br>":
+                PrimeItems.output_lines.output_lines.remove(num)
+                break
+            if tab != "proftab" and item.endswith("<br><br>"):
+                PrimeItems.output_lines.output_lines[-1] = item.replace("<br><br>", "<br>")
+                break
+
 
 # ################################################################################
 # Process the description <d> element
 # ################################################################################
 def description_element_output(
     description_element: defusedxml.ElementTree,
+    tab: str,
 ) -> None:
     """
-    We have a Taskernet description (<Share>).  Clean it uip and add it to
-    the output list.
+    We have a Taskernet description (<Share>).  Clean it up and add it to the output list.
 
-        :param description_element: xml element <d> TaskerNet description
+        :param description_element: xml element <d> TaskerNet description.
+        :param tab: CSS tab class name to apply to the color HTML.
     """
     # We need to properly format this since it has embedded stuff that screws it up
     out_string = format_html(
         "taskernet_color",
         "",
         f"TaskerNet description: {description_element.text}",
         True,
     )
-    indent_html = (
-        "</p><p"
-        f' style="margin-left:20px;margin-right:50px;color:'
-        f'{PrimeItems.colors_to_use["taskernet_color"]}'
-        f'{FONT_FAMILY}{PrimeItems.program_arguments["font"]}">'
-    )
+
+    # Replace all of the Taskernet imbedded HTML with our HTML.
+    indent_html = f'<div <span class="{PrimeItems.colors_to_use["taskernet_color"]} {tab}"></span"></div>'
 
     # Indent the description and override various embedded HTML attributes
     out_string = out_string.replace("<p>", indent_html)
     out_string = out_string.replace("<P>", indent_html)
     out_string = out_string.replace("</p>", "")
     out_string = out_string.replace("</P>", "")
     out_string = out_string.replace("<b>", "")
     out_string = out_string.replace("<br>", indent_html)
     out_string = out_string.replace("<h1>", indent_html)
     out_string = out_string.replace("\r", indent_html)
     out_string = out_string.replace("<li>", indent_html)
     out_string = out_string.replace("</li>", "")
     out_string = out_string.replace("<strong>", "")
-    out_string = out_string.replace("\n", indent_html)
+    out_string = out_string.replace("\n\n", "<br><br>")  # N
+    out_string = out_string.replace("\n", "<br>")  # New line break.
+    out_string = out_string.replace("  ", "<br>")  # Break after two blanks.
+    out_string = out_string.replace("- ", "<br>")  # Break after dash blank.
 
     out_string = out_string.replace(
         "<table>",
         (
             "\n<style>\n.myTable2 {\n color:"
             + PrimeItems.colors_to_use["taskernet_color"]
-            + ';}\n</style>\n<table class="myTable2">'
+            + ';}\n</style>\n<table class="myTable2 {tab}">'
         ),
     )
 
-    # Look for double blanks = line break
-    new_line = ""
-    if indent_html not in out_string:  # Only if we have not already formatted
-        for position, character_index in enumerate(out_string):
-            new_line = (
-                f'{new_line}<p style="margin-left:20px;'
-                f"margin-right:50px;color:"
-                f'{PrimeItems.colors_to_use["taskernet_color"]}'
-                f'{FONT_FAMILY}{PrimeItems.program_arguments["font"]}">'
-                if (character_index == " " and out_string[position + 1] == " ")
-                or (character_index == "-" and out_string[position + 1] == " ")
-                else new_line + character_index
-            )
-
-        # Make certain we have proper html in front of string
-        if "<span " not in out_string:
-            out_string = format_html("taskernet_color", "", new_line, True)
-        else:
-            out_string = new_line
+    # Add the tab CSS call to the color.
+    out_string = PrimeItems.output_lines.add_tab(tab, out_string)
 
     # Output the description line.
     PrimeItems.output_lines.add_line_to_output(2, f"{out_string}", FormatLine.dont_format_line)
```

### Comparing `maptasker-2.6.3/maptasker/src/shelsort.py` & `maptasker-3.2.2/maptasker/src/shelsort.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,15 +14,29 @@
 
 from maptasker.src.sysconst import logger
 
 
 # ##################################################################################
 # Shell sort for Action list (Actions are not necessarily in numeric order in XML backup file).
 # ##################################################################################
-def shell_sort(arr, do_arguments, by_numeric):
+def shell_sort(arr: list, do_arguments: bool, by_numeric: bool) -> None:
+    """
+    Shell sort the list in-place
+    Args:
+        arr: The list to sort
+        do_arguments: Whether to treat elements as arguments
+        by_numeric: Whether to sort numerically
+    Returns:
+        None
+    Processing Logic:
+        1. Set the gap size initially as half of list size
+        2. Keep reducing gap size by half until it reaches 1
+        3. For current gap size, check all pairs of elements gap positions apart and swap if out of order
+        4. Repeat step 3 for all elements in list with current gap
+    """
     n = len(arr)
     gap = n // 2
     while gap > 0:
         j = gap
         # Check the array in from left to right
         # Till the last possible index of j
         while j < n:
@@ -30,16 +44,14 @@
             while i >= 0:
                 if do_arguments:
                     # Get the n from <Action sr='actn' ve='7'> as a number for comparison purposes
                     attr1 = arr[i]
                     attr2 = arr[i + gap]
                     val1 = attr1.attrib.get("sr", "")
                     val2 = attr2.attrib.get("sr", "")
-                    # val1 = attr1.attrib["sr"]
-                    # val2 = attr2.attrib["sr"]
                     if val1[3:] == "" or val2[3:] == "":  # 'if' argument...skip
                         break
                     comp1 = val1[3:]
                     comp2 = val2[3:]
                 else:
                     # General list sort
                     comp1 = arr[i]
@@ -47,18 +59,16 @@
                 # Sort by value or numeric(value)?
                 if by_numeric:
                     comp1 = int(comp1)
                     comp2 = int(comp2)
                 # If value on right side is already greater than left side value
                 # We don't do swap else we swap
                 if not comp1.isdigit() or not comp2.isdigit():
-                    logger.debug("MapTasker.py:shell_sort:" f" comp1:{str(comp1)} comp2:{str(comp2)}")
+                    logger.debug(f"MapTasker.py:shell_sort: comp1:{comp1!s} comp2:{comp2!s}")
                 if do_arguments and int(comp2) > int(comp1) or not do_arguments and comp2 > comp1:
                     break
-                else:
-                    arr[i + gap], arr[i] = arr[i], arr[i + gap]
+                arr[i + gap], arr[i] = arr[i], arr[i + gap]
                 i = i - gap  # To check left side also
             # If the element present is greater than current element
             j += 1
         gap = gap // 2
     # We are done
-    return
```

### Comparing `maptasker-2.6.3/maptasker/src/sysconst.py` & `maptasker-3.2.2/maptasker/src/sysconst.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing action runner logic."""
+
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
 # sysconst: System constants                                                           #
 #                                                                                      #
 # GNU General Public License v3.0                                                      #
@@ -12,26 +13,34 @@
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
 from __future__ import annotations
 
 import logging
 import re
+from datetime import datetime
 from enum import Enum
 from typing import ClassVar
 
+import darkdetect
+
 # Global constants
 UNKNOWN_TASK_NAME = "Unnamed/Anonymous."
-MY_VERSION = "MapTasker version 2.6.3"
-MY_LICENSE = "GNU GENERAL PUBLIC LICENSE (Version 3, 29 June 2007)"
+
+VERSION = "3.2.2"
+MY_VERSION = f"MapTasker version {VERSION}"
+
+MY_LICENSE = "MIT License"
 NO_PROJECT = "-none found."
 COUNTER_FILE = ".MapTasker_RunCount.txt"
-ARGUMENTS_FILE = ".MapTasker_arguments.json"
+OLD_ARGUMENTS_FILE = ".MapTasker_arguments.json"
+ARGUMENTS_FILE = "MapTasker_Settings.toml"
 FONT_FAMILY = ";font-family:"
 NO_PROFILE = "None or unnamed!"
+CHANGELOG_FILE = ".maptasker_changelog.txt"
 
 #  List of color arguments and their names
 #  Two different key/value structures in one:
 #    1- Used as lookup for color selection in GUI.  E.g. key=Disabled Profiles
 #    2- Used as color lookup from runtime parameters.  E.g. DisabledProfile (must follow #1)
 #       Only needed for keys that are different between case #1 and case #2
 TYPES_OF_COLOR_NAMES = {
@@ -52,16 +61,14 @@
     "Profile Conditions": "profile_condition_color",
     "ProfileCondition": "profile_condition_color",
     "Launcher Task": "launcher_task_color",
     "LauncherTask": "launcher_task_color",
     "Background": "background_color",
     "Scenes": "scene_color",
     "Scene": "scene_color",
-    "Bullets": "bullet_color",
-    "Bullet": "bullet_color",
     "Action Labels": "action_label_color",
     "ActionLabel": "action_label_color",
     "Action Names": "action_name_color",
     "ActionName": "action_name_color",
     "TaskerNet Information": "taskernet_color",
     "TaskerNetInfo": "taskernet_color",
     "Tasker Preferences": "preferences_color",
@@ -82,15 +89,14 @@
     "UnknownTask": "'unknown' Tasks",
     "DisabledAction": "disabled Task 'actions'",
     "ActionCondition": "Task action 'conditions'",
     "ProfileCondition": "Profile 'conditions'",
     "LauncherTask": "Project's 'launcher' Task",
     "Background": "output background",
     "Scene": "Scenes",
-    "Bullet": "list bullets",
     "ActionLabel": "Task action 'labels'",
     "ActionName": "Task action 'names'",
     "TaskerNetInfo": "TaskerNet 'information'",
     "Preferences": "Tasker 'preferences'",
     "TrailingComments": "Trailing Comments",
     "Highlight": "Highlight",
     "Heading": "Heading",
@@ -113,18 +119,17 @@
     "file": "Get backup file named",
     "font": "Font To Use",
     "gui": "GUI Mode",
     "highlight": "Highlight Names",
     "indent": "Indentation Amount",
     "italicize": "Italicize Names",
     "outline": "Display Configuration Outline",
+    "pretty": "Display Prettier Output",
     "rerun": "ReRun Program",
-    "restore": "Restore Settings",
     "runtime": "Display Runtime Arguments/Settings",
-    "save": "Save Settings",
     "single_profile_name": "Single Profile Name",
     "single_project_name": "Single Project Name",
     "single_task_name": "Single Task Name",
     "twisty": "Hide Task Details under Twisty",
     "underline": "Underline Names",
 }
 
@@ -137,22 +142,20 @@
 # Compiled match patterns reused throughout
 pattern0 = re.compile(",,")
 pattern1 = re.compile(",  ,")
 pattern2 = re.compile(" ,")
 pattern3 = re.compile("<")
 pattern4 = re.compile(">")
 
-pattern5 = re.compile("<ul>")
-pattern6 = re.compile("</ul>")
-pattern7 = re.compile("<li")
 pattern8 = re.compile("<br>")
 pattern9 = re.compile("</span></span>")
 pattern10 = re.compile("</p></p>")
 pattern11 = re.compile(".*[A-Z].*")
-pattern12 = re.compile("[%]\w+")  # matches any word-constituent character.   # noqa: W605
+pattern12 = re.compile(r"[%]\w+")  # matches any word-constituent character.
+pattern13 = r",(?=\S)"  # matches any comma folowed by a nonblank charatcer.  e.g. now is,the time, for (catches is,the)
 RE_FONT = re.compile(r"</font>")
 
 clean = re.compile("<.*?>")
 
 
 # ASCII Color Definitions
 class Colors:
@@ -178,8 +181,35 @@
     """Definitions for defining the output display level."""
 
 
 DISPLAY_DETAIL_LEVEL_summary: int = 0
 DISPLAY_DETAIL_LEVEL_anon_tasks_only: int = 1
 DISPLAY_DETAIL_LEVEL_all_tasks: int = 2
 DISPLAY_DETAIL_LEVEL_all_parameters: int = 3
-DISPLAY_DETAIL_LEVEL_everything: int = 4
+DISPLAY_DETAIL_LEVEL_all_variables: int = 4
+DISPLAY_DETAIL_LEVEL_everything: int = 5
+
+# Use the normal tab in output.
+NORMAL_TAB = '<span class="normtab"></span>'
+
+# Disabled Profile and Task indicator
+DISABLED = " [&#9940;&nbsp;DISABLED]"  # &#9940 = "⛔"
+
+# Set up background color and border for tables
+TABLE_BACKGROUND_COLOR = "LightSteelBlue" if darkdetect.isDark() else "DarkTurquoise"
+TABLE_BORDER = (
+    "\n"
+    "<style> \
+        table, \
+        td, \
+        th { \
+        padding: 5px; \
+        border: 2px solid #1c87c9; \
+        border-radius: 3px; \
+        background-color: #128198; \
+        text-align: center; \
+        } \
+    </style>"
+)
+
+
+NOW_TIME = datetime.now()  # noqa: DTZ005
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `maptasker-2.6.3/maptasker/src/taskactn.py` & `maptasker-3.2.2/maptasker/src/taskactn.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,21 +7,26 @@
 # GNU General Public License v3.0                                                      #
 # Permissions of this strong copyleft license are conditioned on making available      #
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
-import defusedxml.ElementTree  # Need for type hints
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
 
 import maptasker.src.tasks as tasks
 from maptasker.src.error import error_handler
 from maptasker.src.primitem import PrimeItems
 from maptasker.src.sysconst import UNKNOWN_TASK_NAME, FormatLine
 
+if TYPE_CHECKING:
+    import defusedxml.ElementTree
+
 
 # ##################################################################################
 # Go through list of actions and output them
 # ##################################################################################
 def output_list_of_actions(
     action_count: int,
     alist: list,
@@ -45,46 +50,63 @@
             if taction[:3] == "...":
                 PrimeItems.output_lines.add_line_to_output(
                     2,
                     f"Action: {taction}",
                     ["", "action_color", FormatLine.dont_add_end_span],
                 )
             else:
+                # First remove one blank if line number is > 99 and < 1000
+                temp_action = taction.replace("&nbsp;", "", 1) if action_count > 99 and action_count < 1000 else taction
                 #  Output the Action count = line number of action (fill to 2 leading zeros)
                 PrimeItems.output_lines.add_line_to_output(
                     2,
-                    f"Action: {str(action_count).zfill(2)}</span> {taction}",
+                    f"Action: {str(action_count).zfill(2)}</span> {temp_action}",
                     ["", "action_color", FormatLine.dont_add_end_span],
                 )
                 action_count += 1
             if (
                 action_count == 2
                 and PrimeItems.program_arguments["display_detail_level"] == 0
                 and UNKNOWN_TASK_NAME in the_item
             ):  # Just show first Task if unknown Task
                 break
-            elif PrimeItems.program_arguments["display_detail_level"] == 1 and UNKNOWN_TASK_NAME not in the_item:
+            if PrimeItems.program_arguments["display_detail_level"] == 1 and UNKNOWN_TASK_NAME not in the_item:
                 break
 
     # Close Action list if doing straight print, no twisties
     if not PrimeItems.program_arguments["twisty"]:
         PrimeItems.output_lines.add_line_to_output(3, "", FormatLine.dont_format_line)
-    return
 
 
 # ##################################################################################
 # For this specific Task, get its Actions and output the Task and Actions
 # ##################################################################################
 def get_task_actions_and_output(
     the_task: defusedxml.ElementTree.XML,
     list_type: str,
     the_item: str,
     tasks_found: list[str],
 ) -> None:
     # If Unknown task or displaying more detail, then 'the_task' is not valid, and we have to find it.
+    """
+    Get task actions and output.
+    Args:
+        the_task: {Task xml element}: Task xml element
+        list_type: {str}: Type of list
+        the_item: {str}: Item being displayed
+        tasks_found: {list[str]}: Tasks found so far
+    Returns:
+        None: No return value
+    {Processing Logic}:
+    1. Check if task is unknown or detail level is high, find task ID
+    2. Get task xml element from ID
+    3. Get task actions from xml element
+    4. Output actions list with formatting
+    5. Handle errors if no task found
+    """
     if UNKNOWN_TASK_NAME in the_item or PrimeItems.program_arguments["display_detail_level"] > 0:
         # Get the Task ID so that we can get the Task xml element
         # "--Task:" denotes a Task in a Scene
         temp_id = "x" if "&#45;&#45;Task:" in list_type else the_item.split("Task ID: ")
 
         # Get the Task xml element
         if len(temp_id) > 1:
@@ -93,26 +115,24 @@
                 temp_id[1],  # Task ID
                 tasks_found,  # Tasks found so far
                 [temp_id[1]],  # Task's output line
                 "",  # Task type
             )
 
         # Get Task actions
-        if the_task:
-            # If we have Task Actions, then output them
+        if the_task is not None:
+            # If we have Task Actions, then output them.  The action list is a list of the Action output lines already
+            # formatted.
             if alist := tasks.get_actions(the_task):
                 # Start a list of Actions
                 PrimeItems.output_lines.add_line_to_output(1, "", FormatLine.dont_format_line)
                 action_count = 1
                 output_list_of_actions(action_count, alist, the_item)
                 # End list if Scene Task
                 if "&#45;&#45;Task:" in list_type:
                     PrimeItems.output_lines.add_line_to_output(3, "", FormatLine.dont_format_line)
-                    # Add an extra </ul> if doing twisties
                     if PrimeItems.program_arguments["twisty"]:
                         PrimeItems.output_lines.add_line_to_output(3, "", FormatLine.dont_format_line)
                 # End the list of Actions
                 PrimeItems.output_lines.add_line_to_output(3, "", FormatLine.dont_format_line)
         else:
             error_handler("No Task found!!!", 0)
-
-    return
```

### Comparing `maptasker-2.6.3/maptasker/src/taskflag.py` & `maptasker-3.2.2/maptasker/src/taskflag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
-# taskflag: Get Profile/Task fags: priority, collision, stay awake                           #
+# taskflag: Get Profile/Task fags: priority, collision, stay awake                     #
 #                                                                                      #
 # GNU General Public License v3.0                                                      #
 # Permissions of this strong copyleft license are conditioned on making available      #
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
@@ -21,18 +21,17 @@
         :param event: True if this is for an 'Event' condition, False if not
         :return: the priority or none
     """
 
     priority_element = element.find("pri")
     if priority_element is None:
         return ""
-    elif event:
+    if event:
         return f" Priority:{priority_element.text}"
-    else:
-        return f"&nbsp;&nbsp;[Priority: {priority_element.text}]"
+    return f"&nbsp;&nbsp;[Priority: {priority_element.text}]"
 
 
 def get_collision(element: defusedxml.ElementTree.XML) -> str:
     """
     Get any Task collision setting
         :param element: root element to search for
         :return: the collision setting as text or blank
```

### Comparing `maptasker-2.6.3/maptasker/src/tasks.py` & `maptasker-3.2.2/maptasker/src/tasks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Process Tasks"""
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
 # tasks: Process Tasks                                                                 #
 #                                                                                      #
 # GNU General Public License v3.0                                                      #
@@ -18,15 +19,14 @@
 import maptasker.src.actione as action_evaluate
 import maptasker.src.taskflag as task_flags
 from maptasker.src.error import error_handler
 from maptasker.src.format import format_html
 from maptasker.src.getids import get_ids
 from maptasker.src.kidapp import get_kid_app
 from maptasker.src.primitem import PrimeItems
-from maptasker.src.proclist import process_list
 from maptasker.src.shelsort import shell_sort
 from maptasker.src.sysconst import UNKNOWN_TASK_NAME, DISPLAY_DETAIL_LEVEL_all_tasks, FormatLine, logger
 from maptasker.src.xmldata import tag_in_type
 
 blank = "&nbsp;"
 
 
@@ -34,17 +34,25 @@
 # Navigate through Task's Actions and identify each
 # Return a list of Task's actions for the given Task
 # ##################################################################################
 def get_actions(
     current_task: defusedxml.ElementTree.XML,
 ) -> list:
     """
-    Return a list of Task's actions for the given Task
-        :param current_task: xml element of the Task we are getting actions for
-        :return: list of Task 'action' output lines
+    Get the actions for a task
+    Args:
+        current_task: defusedxml.ElementTree.XML - The XML element of the current task
+    Returns:
+        list - The list of actions for the task
+    Processing Logic:
+        1. Get all <Action> elements from the current task
+        2. Sort the actions by their "sr" attribute to get them in proper order
+        3. Iterate through each action and get its code
+        4. Build the action and add indentation if it is a conditional statement
+        5. Return the list of actions
     """
     tasklist = []
     blanks = f'{"&nbsp;" * PrimeItems.program_arguments["indent"]}'
 
     # Get the Task's Actions (<Action> elements)
     try:
         task_actions = current_task.findall("Action")
@@ -60,18 +68,18 @@
         # Task's Action statements can be out-of-order, and we need them in
         # proper-order/sequence.
         # sort the Task's Actions by attrib sr (e.g. sr='act0', act1, act2, etc.)
         # to get them in true order.
         if len(task_actions) > 0:
             shell_sort(task_actions, True, False)
 
-        # Now go through each Action to start processing it.
+        # Now go through each Action to start processing it.  They are in "argn" "n" order.
         for action in task_actions:
             child = action.find("code")  # Get the <code> element
-            # Get the Action code ( <code> )
+            # Get the Action code ( <code> ).  task_code will be returned with the formatted task action output line.
             task_code = action_evaluate.get_action_code(
                 child,
                 action,
                 True,
                 "t",
             )
             # Log the Task action.
@@ -82,21 +90,31 @@
             # Calculate the amount of indention required
             if ">End If" in task_code or ">Else" in task_code or ">End For" in task_code:  # Do we un-indent?
                 indentation -= 1
                 length_indent = len(indentation_amount)
                 # Total indentation = 6 characters (&nbsp;) times the indent argument
                 total_indentation = int(f'{PrimeItems.program_arguments["indent"]*6}')
                 indentation_amount = indentation_amount[total_indentation:length_indent]
+
+            # Make it pretty
+            if "Configuration Parameter(s):" in task_code and PrimeItems.program_arguments["pretty"]:
+                number_of_blanks = task_code.find(":")
+                task_code = task_code.replace(",", f"<br>{blank*(number_of_blanks-70)}")  # Back out the "<span..."
+                if "Configuration Parameter(s):\n," in task_code:
+                    task_code = task_code.replace("Configuration Parameter(s):\n,", "Configuration Parameter(s):\n")
+
+            # Build the output line.
             tasklist = action_evaluate.build_action(
                 tasklist,
                 task_code,
                 child,
                 indentation,
                 indentation_amount,
             )
+
             #  Indent the line if this is a condition
             if ">If" in task_code or ">Else" in task_code or ">For<" in task_code:  # Do we indent?
                 indentation += 1
                 indentation_amount = f"{indentation_amount}{blanks}"
 
     return tasklist
 
@@ -120,39 +138,40 @@
             task_type (str): Type of this Task: Entry or Exit
             extra (str): Extra text to add to the end of the Task's output line
             duplicate_task (bool): Is this a duplicate Task? True if it is.
 
         Returns:
             tuple: task_output_lines and task_name
     """
+    line_left_arrow = "&#11013;"
     # Determine if this is an "Entry" or "Exit" Task
     if task_name:
         # Don't add the entry/exit text if display level = 0
         if PrimeItems.program_arguments["display_detail_level"] > 0:
             if task_type == "Exit":
-                task_output_lines.append(f"{task_name}{blank*4}<<< Exit Task{extra}")
+                task_output_lines.append(f"{task_name}{blank*4}{line_left_arrow} Exit Task{extra}")
 
             else:
-                task_output_lines.append(f"{task_name}{blank*4}<<< Entry Task{extra}")
+                task_output_lines.append(f"{task_name}{blank*4}{line_left_arrow} Entry Task{extra}")
         else:
             task_output_lines.append(f"{task_name}{blank*4}")
     else:
         task_name = UNKNOWN_TASK_NAME
         # Count this as an unnamed Task if it hasn't yet been counted and it
         # is a normal Task
         if not duplicate_task and task_type in {"Entry", "Exit"}:
             PrimeItems.task_count_unnamed = PrimeItems.task_count_unnamed + 1
         blanks = f'{blank * PrimeItems.program_arguments["indent"]}'
         # Don't add the entry/exit text if display level = 0
         if PrimeItems.program_arguments["display_detail_level"] > 0:
             if task_type == "Exit":
-                task_output_lines.append(f"{UNKNOWN_TASK_NAME}{blanks}<<< Exit Task{extra}")
+                task_output_lines.append(f"{UNKNOWN_TASK_NAME}{blanks}{line_left_arrow} Exit Task{extra}")
 
             else:
-                task_output_lines.append(f"{UNKNOWN_TASK_NAME}{blanks}<<< Entry Task{extra}")
+                task_output_lines.append(f"{UNKNOWN_TASK_NAME}{blanks}{line_left_arrow} Entry Task{extra}")
         else:
             task_output_lines.append(f"{UNKNOWN_TASK_NAME}{blanks}")
 
     return task_output_lines, task_name
 
 
 # ##################################################################################
@@ -211,15 +230,15 @@
 ) -> tuple[str, defusedxml.ElementTree.XML]:
     """
     Find the Project belonging to the Task id passed in
     :param the_task_id: the ID of the Task
     :param projects_with_no_tasks: list of Projects that do not have any Tasks
     :return: name of the Project that belongs to this task and the Project xml element
     """
-    NO_PROJECT = "No Project"
+    NO_PROJECT = "No Project"  # noqa: N806
     project_name = NO_PROJECT
     project_element = None
 
     all_projects = PrimeItems.tasker_root_elements["all_projects"]
     if all_projects is not None:
         for project in all_projects:
             project_element = PrimeItems.tasker_root_elements["all_projects"][project]["xml"]
@@ -268,37 +287,65 @@
     project_name: str,
     profile_name: str,
     task_list: list,
     our_task_element: defusedxml.ElementTree.XML,
     list_of_found_tasks: list,
 ) -> None:
     """
+    Process a single Task only.
+
+    Args:
+        our_task_name (str): The name of the Task to be processed.
+        project_name (str): The name of the Project the Task belongs to.
+        profile_name (str): The name of the Profile the Task belongs to.
+        task_list (list): A list of Tasks.
+        our_task_element (defusedxml.ElementTree.XML): The XML element for this Task.
+        list_of_found_tasks (list): A list of all Tasks processed so far.
+
+    Returns:
+        None
+
+    This function processes a single Task only. It first checks if the Task name matches
+    the single Task name specified in the program arguments. If it does, it sets the
+    "single_task_found", "single_project_found", and "single_profile_found" flags to True,
+    and updates the program arguments with the project and profile names. It then clears
+    the output list. If a Task list is provided, it filters the list to include only the
+    Tasks that start with the same name as the single Task. If the Task list is empty, it
+    sets the temporary task list to an empty list. It then processes the Task/Task list by
+    calling the process_list function. If multiple Tasks are present in the Profile, it
+    adds a line to the output, filters the Task list to include only the single Task, and
+    processes the Task by calling the process_list function.
+    """
+    # This import must reside here to avoid circular error.
+    from maptasker.src.proclist import process_list
+
+    """
     Process a single Task only
 
         :param our_task_name: name of Task we are to process
         :param project_name: name of the Project Task belongs to
         :param profile_name: name of the Profile the Task belongs to
         :param task_list: list of Tasks
         :param our_task_element: the xml element for this Task
         :param list_of_found_tasks: all Tasks processed so far
     """
 
     logger.debug(
         "tasks single task"
         f' name:{PrimeItems.program_arguments["single_task_name"]} our Task'
-        f" name:{our_task_name}"
+        f" name:{our_task_name}",
     )
 
     # Doing a specific Task...
     if (
         PrimeItems.program_arguments["single_task_name"]
         and PrimeItems.program_arguments["single_task_name"] == our_task_name
     ):
         # We have the single Task we are looking for
-        # Set all the "found" items
+        # Set all the "found" items so that everyone bails out of their loops.
         PrimeItems.found_named_items["single_task_found"] = True
         PrimeItems.found_named_items["single_project_found"] = True
         PrimeItems.found_named_items["single_profile_found"] = True
         PrimeItems.program_arguments["single_project_name"] = project_name
         PrimeItems.program_arguments["single_profile_name"] = profile_name
 
         # Clear output list
@@ -312,40 +359,63 @@
         #  Note: we need to save the task_list since process_list will alter it.
         temporary_task_list = []
         if task_list:
             the_task_name_length = len(our_task_name)
             temporary_task_list = [item for item in task_list if our_task_name == item[:the_task_name_length]]
         else:
             temporary_task_list = task_list
+
+        # Make the line pretty
+        if PrimeItems.program_arguments["pretty"]:
+            temporary_task_list[0] = temporary_task_list[0].replace("[", "<br>[")
+
         # Go process the Task/Task list
         process_list(
             "Task:",
             temporary_task_list,
             our_task_element,
             list_of_found_tasks,
         )
 
     # If multiple Tasks in this Profile, just get the one we want
     else:
         PrimeItems.output_lines.add_line_to_output(1, "", FormatLine.dont_format_line)
+
+        # Make the line pretty
+        if PrimeItems.program_arguments["pretty"]:
+            blanks = f'{"&nbsp;" * len(our_task_name)}'
+            task_list[0] = task_list[0].replace("[", f"<br>{blanks}[")
+
         # Process the task(s)
         process_list(
             "Task:",
             task_list,
             our_task_element,
             list_of_found_tasks,
         )
         # End Task list
         PrimeItems.output_lines.add_line_to_output(3, "", FormatLine.dont_format_line)
 
 
 # ##################################################################################
 # Search image xml element for key and return title=value
 # ##################################################################################
-def get_image(image, title, key):
+def get_image(image: defusedxml.ElementTree, title: str, key: str) -> str:
+    """Returns:
+        - str: Returns a string.
+    Parameters:
+        - image (defusedxml.ElementTree): An XML element tree.
+        - title (str): The title of the image.
+        - key (str): The key to search for in the XML element tree.
+    Processing Logic:
+        - Finds the element with the given key.
+        - If the element is not found, returns an empty string.
+        - If the element's text contains a period, splits the text at the last period and returns the second part.
+        - If the text is empty, returns an empty string.
+        - Otherwise, returns a string containing the title and text."""
     element = image.find(key)
     if element is None:
         return ""
     text = element.text
     if "." in text:
         text = text.rsplit(".", 1)[1]
     return f"{title}={text} " if text else ""
@@ -424,44 +494,51 @@
 def output_task_list(
     list_of_tasks: list,
     project_name: str,
     profile_name: str,
     task_output_lines: str,
     list_of_found_tasks: list,
     do_extra: bool,
-) -> None:
+) -> bool:
     """
     Given a list of tasks, output them.  The list of tasks is a list of tuples.
         The first element is the Task name, the second is the Task element.
         Args:
 
             list_of_tasks (list): list of Tasks to output.
             project_name (str): name of the owning Projeect
             profile_name (str): name of the owning Profile
             task_output_lines (str): the output lines for the Tasks
             list_of_found_tasks (list): list of Tasks found so far
-            do_extra (bool): True to output extra info."""
+            do_extra (bool): True to output extra info.
+        Returns:
+            bool: True if we found a Task"""
     for count, task_item in enumerate(list_of_tasks):
+        # If we are coming in without a Task name, then we are only doing a single Task and we need to plug in
+        # the Task name.
+        if task_output_lines[count] == " ":
+            task_output_lines[count] = f'{task_item["name"]}&nbsp;&nbsp;'
+
         # Doing extra details?
         if do_extra and PrimeItems.program_arguments["display_detail_level"] > DISPLAY_DETAIL_LEVEL_all_tasks:
             # Get the extra details for this Task
             (
                 kid_app_info,
                 priority,
                 collision,
                 stay_awake,
                 icon_info,
             ) = get_extra_details(
                 task_item["xml"],
                 [task_output_lines[count]],
             )
-            # Tack on the extra info since [task_output_lines[count]] is immutable
-            task_output_lines[
-                count
-            ] = f"{task_output_lines[count]} {kid_app_info}{priority}{collision}{stay_awake}{blank*2}{icon_info}"
+            # Tack on the extra info since [task_output_lines[count]] it is immutable
+            task_output_lines[count] = (
+                f"{task_output_lines[count]} {kid_app_info}{priority}{collision}{stay_awake}{blank*2}{icon_info}"
+            )
 
         do_single_task(
             task_item["name"],
             project_name,
             profile_name,
             [task_output_lines[count]],
             task_item["xml"],
@@ -469,10 +546,11 @@
         )
 
         # If only doing a single Task and we found/did it, then we are done
         if (
             PrimeItems.program_arguments["single_task_name"]
             and PrimeItems.program_arguments["single_task_name"] == task_item["name"]
         ):
+            PrimeItems.found_named_items["single_task_found"] = True
             return True
 
     return False
```

### Comparing `maptasker-2.6.3/maptasker/src/taskuniq.py` & `maptasker-3.2.2/maptasker/src/taskuniq.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,48 @@
+"""Process Unique Task Situations"""
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
 # taskuniq: deal with unique Tasks                                                     #
 #                                                                                      #
 # GNU General Public License v3.0                                                      #
 # Permissions of this strong copyleft license are conditioned on making available      #
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
-from typing import List, Union
 
-import defusedxml.ElementTree
-
-import maptasker.src.tasks as tasks
 from maptasker.src.primitem import PrimeItems
-from maptasker.src.sysconst import NO_PROJECT, UNKNOWN_TASK_NAME, FormatLine
+from maptasker.src.sysconst import NO_PROJECT, NORMAL_TAB, UNKNOWN_TASK_NAME, FormatLine
+from maptasker.src.tasks import get_project_for_solo_task, get_task_name, output_task_list, task_in_scene
 from maptasker.src.twisty import add_twisty, remove_twisty
 
 
 # ##################################################################################
 # Output Projects Without Tasks and Projects Without Profiles
 # ##################################################################################
 def process_missing_tasks_and_profiles(
-    projects_with_no_tasks: Union[List[str], List],
-    projects_without_profiles: List[str],
+    projects_with_no_tasks: list,
+    projects_without_profiles: list,
 ) -> None:
     """
     Output Projects Without Tasks and Projects Without Profiles
         all Tasker xml root elements, and a list of all output lines.
         :param projects_with_no_tasks: root xml entry for list of Projects with no Tasks
         :param projects_without_profiles: root xml entry for list of Projects with no Profiles
         :return: nothing
     """
 
     # List Projects with no Tasks
     if len(projects_with_no_tasks) > 0 and not PrimeItems.found_named_items["single_task_found"]:
         PrimeItems.output_lines.add_line_to_output(
             1,
-            "<hr><em>Projects Without Tasks...</em><br>",
+            f"{NORMAL_TAB}<hr>{NORMAL_TAB}<em>Projects Without Tasks...</em><br>",
             ["", "trailing_comments_color", FormatLine.add_end_span],
         )
 
         for item in projects_with_no_tasks:
             PrimeItems.output_lines.add_line_to_output(
                 0,
                 f"Project {item} has no <em>Named</em> Tasks",
@@ -54,21 +52,21 @@
         PrimeItems.output_lines.add_line_to_output(3, "<br>", FormatLine.dont_format_line)
 
     # List all Projects without Profiles
     if projects_without_profiles:
         # Add heading
         PrimeItems.output_lines.add_line_to_output(
             1,
-            "<em>Projects Without Profiles...</em><br>",
+            f"{NORMAL_TAB}<em>Projects Without Profiles...</em><br>",
             ["<br>", "trailing_comments_color", FormatLine.add_end_span],
         )
         for item in projects_without_profiles:
             PrimeItems.output_lines.add_line_to_output(
                 0,
-                f"- Project {item} has no Profiles",
+                f"- Project '{item}' has no Profiles",
                 ["", "trailing_comments_color", FormatLine.add_end_span],
             )
         # End list
         PrimeItems.output_lines.add_line_to_output(3, "<br>", FormatLine.dont_format_line)
 
 
 # ##################################################################################
@@ -80,15 +78,15 @@
 
         :param save_twisty: flag to indicate whether or not we are doing the twisty/hidden Tasks
         :return: True...flag that the heading has been created/output
     """
 
     # Start a list and add a ruler-line across page
     PrimeItems.output_lines.add_line_to_output(1, "<hr>", FormatLine.dont_format_line)
-    text_line = "Named Tasks that are not called by any Profile..."
+    text_line = f"{NORMAL_TAB}Named Tasks that are not called by any Profile...<br>"
 
     # Add a twisty, if doing twisties, to hide the line
     if save_twisty:
         add_twisty("trailing_comments_color", text_line)
 
     # Add the header
     PrimeItems.output_lines.add_line_to_output(
@@ -108,68 +106,66 @@
 def process_solo_task_with_no_profile(
     task_id: str,
     found_tasks: list,
     task_count: int,
     have_heading: bool,
     projects_with_no_tasks: list,
     save_twisty: bool,
-) -> tuple[int, defusedxml.ElementTree.XML, int]:
+) -> tuple:
     """
     Process a single Task that does not belong to any Profile
 
         :param task_id: the ID of the Task being displayed
         :param found_tasks: list of Tasks that we have found
         :param task_count: count of the unnamed Tasks
         :param have_heading: whether we have the heading
         :param projects_with_no_tasks: list of Projects without Tasks
         :param save_twisty: whether we are displaying twisty to Hide Task details
         :return: heading flag, xml element for this Task, and total count of unnamed Tasks
     """
     unknown_task, specific_task = False, False
 
     # Get the Project this Task is under.
-    project_name, the_project = tasks.get_project_for_solo_task(
+    project_name, the_project = get_project_for_solo_task(
         task_id,
         projects_with_no_tasks,
     )
 
     # Get the Task's name
-    task_element, task_name = tasks.get_task_name(task_id, found_tasks, [], "")
+    task_element, task_name = get_task_name(task_id, found_tasks, [], "")
     if task_name == UNKNOWN_TASK_NAME:
         task_name = f"{UNKNOWN_TASK_NAME}&nbsp;&nbsp;Task ID: {task_id}"
         # Ignore it if it is in a Scene
-        if tasks.task_in_scene(task_id, PrimeItems.tasker_root_elements["all_scenes"]):
+        if task_in_scene(task_id, PrimeItems.tasker_root_elements["all_scenes"]):
             return have_heading, specific_task, task_count
         unknown_task = True
     # else:
     #     the_task_name = task_name
     task_count += 1
 
     # At this point, we've found the Project this Task belongs to,
     # or it doesn't belong to any Profile
     if not have_heading and PrimeItems.program_arguments["display_detail_level"] > 2:
         # Add the heading to the output
-        have_heading = add_heading(
-            save_twisty,
-        )
+        have_heading = add_heading(save_twisty)
     if not unknown_task and project_name != NO_PROJECT:
         if PrimeItems.program_arguments["debug"]:
-            task_name += f" with Task ID: {task_id} ...in Project {project_name}&nbsp;&nbsp;> <em>No" " Profile</em>"
+            task_name += f" with Task ID: {task_id} ...in Project '{project_name}'&nbsp;&nbsp;> <em>No Profile</em>"
         else:
-            task_name += f" ...in Project {project_name}&nbsp;&nbsp;> <em>No Profile</em>"
+            task_name += f" ...in Project '{project_name}'&nbsp;&nbsp;> <em>No Profile</em>"
 
     # Output the Task's details
     if (not unknown_task) and (
         PrimeItems.program_arguments["display_detail_level"] > 2
-    ):  # Only list named Tasks or if details are wanted
-        task_output_lines = [task_name]
+    ):  # Only list named Tasks or if details are wanted.
+        task_output_lines = [task_name]  # Return as a list.
 
         # We have the Tasks.  Now let's output them.
         our_task = PrimeItems.tasker_root_elements["all_tasks"][task_id]
-        specific_task = tasks.output_task_list(
+        specific_task = output_task_list(
             [our_task],
             project_name,
             "",
             task_output_lines,
             found_tasks,
             False,
         )
@@ -177,16 +173,16 @@
     return have_heading, specific_task, task_count
 
 
 # ##################################################################################
 # process_tasks: go through all tasks and output them
 # ##################################################################################
 def process_tasks_not_called_by_profile(
-    projects_with_no_tasks: List,
-    found_tasks_list: List[str],
+    projects_with_no_tasks: list,
+    found_tasks_list: list,
 ) -> None:
     """
     Go through all tasks and output them
         :param projects_with_no_tasks: list of Project xml roots for which there are no Tasks
         :param found_tasks_list: list of all Tasks found so far
         :return: nothing
     """
@@ -212,17 +208,18 @@
                 have_heading,
                 projects_with_no_tasks,
                 save_twisty,
             )
             if specific_task:
                 break
 
-    # End the twisty hidden Task list
+    # End the twisty hidden Task list.  Remove it and restore the setting.
     if save_twisty:
         remove_twisty()
+        PrimeItems.program_arguments["twisty"] = save_twisty
 
     # Provide spacing and end list if we have Tasks
     if task_count > 0:
         if PrimeItems.program_arguments["display_detail_level"] > 0:
             PrimeItems.output_lines.add_line_to_output(0, "", FormatLine.dont_format_line)  # blank line
         PrimeItems.output_lines.add_line_to_output(3, "", FormatLine.dont_format_line)  # Close Task list
```

### Comparing `maptasker-2.6.3/maptasker/src/twisty.py` & `maptasker-3.2.2/maptasker/src/twisty.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,49 +8,34 @@
 # Permissions of this strong copyleft license are conditioned on making available      #
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
 from maptasker.src.primitem import PrimeItems
-from maptasker.src.sysconst import logger, FormatLine
+from maptasker.src.sysconst import FormatLine
 
 
 def add_twisty(output_color_name: str, line_to_output: str) -> None:
     """
     Add the necessary html to hide the follow-on text under a twisty ►
 
         :param output_color_name: name of the color to insert into the html
         :param line_to_output: text line to output into the html
         :return: nothing.  Add formatted html with the twisty magic
     """
     # Add the "twisty" to hide the Task details
     PrimeItems.output_lines.add_line_to_output(
         5,
-        f"\n<details><summary>{line_to_output}</summary>\r",
+        f"\n<span class='tasktab'><details><summary>{line_to_output}</summary>\r",
+        # f"\n<details><summary><span class='tasktab'>{line_to_output}</span></summary>\r",
         ["", output_color_name, FormatLine.add_end_span],
     )
-    return
 
 
 def remove_twisty() -> None:
     """
     Add the html element to stop the hidden items..so the follow-up stuff is not hidden
 
         :return: nothing.  The output line is modified to include "</details>"
     """
-    # Replace the last line (</ul>) with </ul></details> to end the twisty/hidden items
-    # If our unordered list counter is zero, then only insert the </details>
-    if PrimeItems.unordered_list_count == 0:
-        PrimeItems.output_lines.output_lines[-1] = "</details>\n"
-    elif PrimeItems.unordered_list_count > 0:
-        PrimeItems.unordered_list_count -= 1
-        PrimeItems.output_lines.output_lines[-1] = "</ul></details>\n"
-        logger.info(f"linout twisty counter deducted: {PrimeItems.unordered_list_count}")
-    else:
-        print("Rutroh!")
-        import traceback
-
-        traceback.print_tb()
-        exit()
-
-    return
+    PrimeItems.output_lines.output_lines[-1] = "</details></span><br>\n"
```

### Comparing `maptasker-2.6.3/maptasker/src/userintr.py` & `maptasker-3.2.2/maptasker/src/userintr.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,663 +1,260 @@
 """Code to manage the graphical user interface."""
+
 #! /usr/bin/env python3
 
 # #################################################################################### #
 #                                                                                      #
 # userintr: provide GUI and process input for program arguments                        #
 #                                                                                      #
 # GNU General Public License v3.0                                                      #
 # Permissions of this strong copyleft license are conditioned on making available      #
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
 import contextlib
-import os
+import webbrowser
 from pathlib import Path
 
 import customtkinter
 from CTkColorPicker.ctk_color_picker import AskColor
-from PIL import Image
 
-from maptasker.src.config import OUTPUT_FONT
-from maptasker.src.getbakup import request_file
+from maptasker.src.colrmode import set_color_mode
+from maptasker.src.config import DEFAULT_DISPLAY_DETAIL_LEVEL, OUTPUT_FONT
+from maptasker.src.getids import get_ids
 from maptasker.src.getputer import save_restore_args
-from maptasker.src.guiutils import clear_android_buttons, get_monospace_fonts, ping_android_device, valid_item
+from maptasker.src.guiutils import (
+    CHANGELOG,
+    CTkTreeview,
+    TreeviewWindow,
+    add_button,
+    add_label,
+    check_for_changelog,
+    clear_android_buttons,
+    create_changelog,
+    get_xml,
+    initialize_gui,
+    initialize_screen,
+    is_new_version,
+    ping_android_device,
+    valid_item,
+    validate_or_filelist_xml,
+)
+from maptasker.src.initparg import initialize_runtime_arguments
+from maptasker.src.lineout import LineOut
+from maptasker.src.mapit import clean_up_memory, do_rerun
+from maptasker.src.maputils import update, validate_xml_file
 from maptasker.src.primitem import PrimeItems
+from maptasker.src.profiles import get_profile_tasks
 from maptasker.src.sysconst import (
     ARGUMENT_NAMES,
     TYPES_OF_COLOR_NAMES,
+    VERSION,
     DISPLAY_DETAIL_LEVEL_all_parameters,
 )
+from maptasker.src.taskerd import get_the_xml_data
 
 # Color Modes: "System" (standard), "Dark", "Light"
 customtkinter.set_appearance_mode("System")
 # Themes: "blue" (standard), "green", "dark-blue"
 customtkinter.set_default_color_theme("blue")
 
+# NOTE: The textbox is used for help information via new_message_box, normal one-liner messages via display_message_box
+#       and multi-line messages via display_multiple_message.
 # Help Text
 INFO_TEXT = (
-    "MapTasker displays your Android Tasker "
-    "configuration based on your uploaded Tasker backup "
-    "file (e.g. 'backup.xml'). The display will "
-    "optionally include all Projects, Profiles, Tasks "
-    "and their actions, Profile/Task conditions and "
-    "other Profile/Task related information.\n\n"
+    "MapTasker displays your Android Tasker configuration based on your uploaded Tasker XML "
+    "file (e.g. 'backup.xml'). The display will optionally include all Projects, Profiles, Tasks "
+    "and their actions, Profile/Task conditions and other Profile/Task related information.\n\n"
     "* Display options are:\n"
-    "    Level 0: display first Task action only, for "
-    "unnamed Tasks only (silent).\n"
-    "    Level 1 = display all Task action details for "
-    "unknown Tasks only (default).\n"
-    "    Level 2 = display full Task action name on "
-    "every Task.\n"
-    "    Level 3 = display full Task action details on "
-    "every Task with action details.\n"
+    "    Level 0: display first Task action only, for unnamed Tasks only (silent).\n"
+    "    Level 1 = display all Task action details for unknown Tasks only (default).\n"
+    "    Level 2 = display full Task action name on every Task.\n"
+    "    Level 3 = display full Task action details on every Task with action details.\n"
     "    Level 4 = display level of 3 plus Project's global variables.\n\n"
     "* Just Display Everything: Turns on the display of "
-    "conditions, TaskerNet information, preferences, twisties, directory, "
-    "and configuration outline.\n\n"
-    "* Display Conditions: Turn on the display of "
-    "Profile and Task conditions.\n\n"
-    "* Display TaskerNet Info - If available, display "
-    "TaskerNet publishing information.\n\n"
-    "* Display Tasker Preferences - display Tasker's "
-    "system Preferences.\n\n"
-    "* Hide Task Details under Twisty: hide Task "
-    "information within ► and click to display.\n\n"
-    "* Display Directory of hyperlinks at beginning."
-    "\n\n"
-    "* Display Configuration Outline and Map of your Projects/Profiles/Tasks/Scenes."
-    "\n\n"
-    "* Project/Profile/Task/Scene Names options to "
-    "italicize, bold, underline and/or highlight their "
-    "names.\n\n"
+    "conditions, TaskerNet information, preferences, pretty output, directory, and configuration outline.\n\n"
+    "* Display Conditions: Turn on the display of Profile and Task conditions.\n\n"
+    "* Display TaskerNet Info - If available, display TaskerNet publishing information.\n\n"
+    "* Display Tasker Preferences - display Tasker's system Preferences.\n\n"
+    "* Hide Task Details under Twisty: hide Task information within ► and click to display.\n\n"
+    "* Display Directory of hyperlinks at beginning.\n\n"
+    "* Display Configuration Outline and Map of your Projects/Profiles/Tasks/Scenes.\n\n"
+    "* Display Prettier Output: Make the output more human-readable by adding newlines and indentation for all arguments.\n\n"
+    "* Project/Profile/Task/Scene Names options to italicize, bold, underline and/or highlight their names.\n\n"
     "* Indentation amount for If/Then/Else Task Actions.\n\n"
-    "* Save Settings - Save these settings for later "
-    "use.\n\n"
-    "* Restore Settings - Restore the settings from a "
-    "previously saved session.\n\n"
-    "* Appearance Mode: Dark, Light, or System "
-    "default.\n\n"
-    "* Reset Options: Clear everything and start "
-    "anew.\n\n"
+    "* Save Settings - Save these settings for later use.\n\n"
+    "* Restore Settings - Restore the settings from a previously saved session.\n\n"
+    "* Report Issue - This will bring up your browser to the issue reporting site, and you can use this to "
+    "either report a bug or request a new feature ( [Feature Request] )\n\n"
+    "* Appearance Mode: Dark, Light, or System default.\n\n"
+    "* Tree View: Display a tree of your Projects/Profiles/Tasks.\n\n"
+    "* Reset Options: Clear everything and start anew.\n\n"
+    "* Clear Messages: Clear any messages in the textbox.\n\n"
     "* Font To Use: Change the monospace font used for the output.\n\n"
     "* Display Outline: Display Projects/Profiles/Tasks/Scenes configuration outline.\n\n"
-    "* Get Backup from Android Device: fetch the backup "
-    "xml file from device.  You will be asked for the IP address and port number for your"
+    "* Get XML from Android Device: fetch the backup/exported "
+    "XML file from Androiddevice.  You will be asked for the IP address and port number for your"
     " Android device, as well as the file location on the device.\n\n"
-    "* Run: Run the program with the settings "
-    "provided and then exit.\n"
-    "* ReRun: Run multiple times (each time with "
-    "new settings) without exiting.\n\n"
-    "* Specific Name tab: enter a single, specific "
-    "named item to display...\n"
-    "   - Project Name: enter a specific Project to "
-    "display.\n"
-    "   - Profile Name: enter a specific Profile to "
-    "display.\n"
-    "   - Task Name: enter a specific Task to "
-    "display.\n"
-    "   (These three are exclusive: enter one "
-    "only)\n\n"
-    "* Colors tab: select colors for various elements "
-    "of the display.\n"
-    "              (e.g. color for Projects, Profiles, "
-    "Tasks, etc.).\n\n"
-    "* Debug tab: Display Runtime Settings option and "
-    "turn on Debug mode.\n\n"
+    "* Run and Exit: Run the program with the settings provided and then exit.\n"
+    "* ReRun: Run multiple times (each time with new settings) without exiting.\n\n"
+    "* Specific Name tab: enter a single, specific named item to display...\n"
+    "   - Project Name: enter a specific Project to display.\n"
+    "   - Profile Name: enter a specific Profile to display.\n"
+    "   - Task Name: enter a specific Task to display.\n"
+    "   (These three are exclusive: enter one only)\n\n"
+    "* Colors tab: select colors for various elements of the display.\n"
+    "              (e.g. color for Projects, Profiles, Tasks, etc.).\n\n"
+    "* Debug tab: Display Runtime Settings option and turn on Debug mode.\n\n"
     "* Exit: Exit the program (quit).\n\n"
-    "Note: You will be prompted to identify your Tasker "
-    "backup file once you hit the 'Run' button."
+    "Notes:\n\n"
+    "- You will be prompted to identify your Tasker XML file once you hit the 'Run and Exit' or 'ReRun' button if you have not yet done so.\n\n"
+    "- If running on OS X Ventura, you may receive the runtime error: +[CATransaction synchronize] called within transaction. This can be ignored and the program will still run correctly.\n\n"
+    "- The 'Rerun' button will spit out the message 'Task policy set failed: 4 ((os/kern) invalid argument)' which can be ignored.\n\n"
 )
 BACKUP_HELP_TEXT = (
-    "The following steps are required in order to fetch a Tasker backup file directly"
+    "The following steps are required in order to fetch a Tasker XML file directly"
     " from your Android device.\n\n"
     "1- Both this device and the Android device must be on the same named network.\n\n"
     "2- The Tasker Project 'HTTP Server Example' or identical function must be"
     " installed and active on the Android device (the server must be running):\n\n"
     "    https://shorturl.at/bwCD4\n\n"
+    "3- If you want to use the 'List XML Files' option, then you must also import the following profile "
+    "into the Android device and make sure the imported profile 'MapTasker List' is enabled:\n\n"
+    "    https://shorturl.at/buvK6\n\n"
     "You will be asked for the IP address, the port number for your Android device,"
     " as well as the file location on the Android device.  Default values are supplied, where...\n\n"
     "'192.168.0.210' is the default IP address,\n\n'1821' is the default port number for the Tasker HTTP"
-    " Server Example running on your Android device\n\n'/Tasker/configs/user/backup.xml' is the default file location.\n\n"
+    " Server Example running on your Android device\n\n'/Tasker/configs/user/backup.xml' is the default file location.  "
+    "If you don't know the file location and have already entered your IP address and port, then you can select "
+    "the 'List XML Files' button to get a list of available XML files on your Android device for selection.\n\n"
     "Usage Notes:\n\n"
     "The IP address and port can be obtained by installing the 'HTTP Server Example' project from the above URL "
     "on your Android device. Then run the task named 'Update GD HTTP Info' to get the Android notification:\n\n"
     "HTTP Server Info\n"
     'Server info updated {"device name":"http://192.168.0.49:1821"}\n\n'
-    "- To fetch the backup file, click on the button\n\n 'Get Backup from Android Device'\n\n"
+    "- To fetch the XML file, click on the button\n\n 'Get XML from Android Device'\n\n"
     "Then modify the default values presented in the input fields below this button, and then"
-    " click on the button\n\n'Finally, enter and Click Here to Set Baclup Details'.\n\n"
-    "- the Fetch backup settings are only used once the 'Run' button is pressed, but"
-    " this program will try to ping your Android device to see if it is available"
-    " once your enter the TCP IP Address, Port Number and File Location values.  The ping will timeout after"
+    " click on the button 'Enter and Click Here to Set XML Details' or 'List XML Files'.\n\n"
+    "- Hitting either button will ping the Android device to see if it is available.  The ping will timeout after"
     " 10 seconds if the device is not reachable.  Make sure that the IP address is correct.\n\n"
+    "Click on the 'Cancel Entry' button to back out of this fetch process.\n\n"
+)
+LISTFILES_HELP_TEXT = (
+    "Clicking this button will result in the following actions:\n\n"
+    "- The IP Address will be used to ping the Android device.\n\n"
+    "- The IP Address and port number will be used to query the Android device and get a list of available XML files "
+    "found in the Tasker folder.\n\n"
+    "- The list of found XML files will be presented in a pulldown menu from which you can select the one you want "
+    "to use.\n\n"
+    "- Once you have selected the XML file, it will be fetched and verified as valid XML which is then used as "
+    "input to the program once you subsequently click on the 'Run' or 'ReRun' button.\n\n"
+    "In order for this to work, you MUST have already imported the 'MapTasker List' profile into Tasker running "
+    "on your Android device.  This profile can be found at the following URL:\n\n"
+    "    https://shorturl.at/buvK6\n\n"
 )
 
+TREEVIEW_HELP_TEXT = (
+    "The Treeview has the following limitations/behavior:\n\n"
+    "- Huge configurations that scroll beyond the bottom of the screen are not viewable in their entirety yet.\n\n"
+    "- Only Projects can be displayed. XML consisting of only a single Profile or Task will not be displayed.\n\n"
+    "- If the XML has already been fetched, it will be used as input to the treeview.  Hitting the 'Reset' button will clear the treeview data."
+    " In otherwords, the treeview will remain the same until either the 'Reset' button is hit, or a new XML file is fetched from the"
+    " Android device or the program is run with the '-reset' option."
+)
+
+HELP = f"MapTasker {VERSION} Help\n\n{INFO_TEXT}{CHANGELOG}"
+
 
 # ##################################################################################
 # Class to define the GUI configuration
 # ##################################################################################
 class MyGui(customtkinter.CTk):
     """
     Main class for GUI.
         Args:
             customtkinter (_type_): GUI class from customtkinter library.
     """
 
-    def __init__(self) -> None:  # noqa: ANN101, PLR0915
-        """Initializes the GUI window for the MapTasker runtime options
-
-        Args:
-            self: The class instance
-
-        Returns:
-            None: Initializes and configures the GUI window
-
-        Processing Logic:
-        - Configures the window layout using grid geometry manager
-        - Creates frames and widgets for sidebar, tabs, buttons etc
-        - Sets default values for options
-        - Binds widget events to callback methods
+    def __init__(self) -> None:
         """
+        Initializes the GUI, adds menu elements, and sets default values.
+        If not resetting, restores settings and updates fields.
+        Checks for single item to be displayed. Checks for newer version of code on Pypi every 24 hours.
+        Displays upgrade button if new version is available.
+        Checks for changelog and displays message box if applicable."""
         super().__init__()
 
-        # configure window
-        self.android_ipaddr = ""
-        self.android_port = ""
-        self.android_file = ""
-        self.appearance_mode = None
-        self.bold = None
-        self.color_labels = None
-        self.color_lookup = None
-        self.color_text_row = None
-        self.debug = None
-        self.display_detail_level = None
-        self.preferences = None
-        self.conditions = None
-        self.everything = None
-        self.taskernet = None
-        self.exit = None
-        self.fetched_backup_from_android = False
-        self.file = None
-        self.font = None
-        self.go_program = None
-        self.gui = True
-        self.highlight = None
-        self.indent = None
-        self.italicize = None
-        self.named_item = None
-        self.rerun = None
-        self.reset = None
-        self.restore = False
-        self.runtime = False
-        self.save = False
-        self.single_profile_name = None
-        self.single_project_name = None
-        self.single_task_name = None
-        self.twisty = None
-        self.underline = None
-        self.outline = False
-        PrimeItems.program_arguments["gui"] = True
-
-        self.title("MapTasker Runtime Options")
-        # Overall window dimensions
-        self.geometry("1100x800")
-        self.width = 1100
-        self.height = 800
-
-        # configure grid layout (4x4)
-        self.grid_columnconfigure(1, weight=1)
-        self.grid_columnconfigure((2, 3), weight=0)
-        self.grid_rowconfigure(0, weight=1)
-
-        # load and create background image
-
-        # create sidebar frame with widgets
-        self.sidebar_frame = customtkinter.CTkFrame(self, width=140, corner_radius=0)
-        # self.sidebar_frame.configure(height=self._apply_window_scaling(800))
-        self.sidebar_frame.grid(row=0, column=0, rowspan=13, sticky="nsew")
-        # Define sidebar background frame with 14 rows
-        self.sidebar_frame.grid_rowconfigure(14, weight=1)
-
-        # Add our logo
-        # Get the path to our logos:
-        # current_dir = directory from which we are running.
-        # abspath = path of this source code (userintr.py).
-        # cwd = directory from which the main program is (main.py)
-        # dname = directory of src
-        current_dir = os.getcwd()
-        abspath = os.path.abspath(__file__)
-        # cwd = os.path.abspath(os.path.dirname(sys.argv[0]))
-        dname = os.path.dirname(abspath)
-        temp_dir = dname.replace("src", "assets")
-        # Switch to our temp directory (assets)
-        os.chdir(temp_dir)
-
-        # Create a CTkImage object to display the logo
-        my_image = customtkinter.CTkImage(
-            light_image=Image.open("maptasker_logo_light.png"),
-            dark_image=Image.open("maptasker_logo_dark.png"),
-            size=(190, 50),
-        )
-        self.logo_label = customtkinter.CTkLabel(
-            self.sidebar_frame,
-            image=my_image,
-            text="",
-            compound="left",
-            font=customtkinter.CTkFont(size=1, weight="bold"),
-        )  # display image with a CTkLabel
-        self.logo_label.grid(row=0, column=0, padx=0, pady=0, sticky="n")
-        # del my_image  # Done with image...get rid of it.
-
-        # # Add the background image.
-        # bg_image = customtkinter.CTkImage(
-        #     Image.open("bg_gradient.jpg"),
-        #     size=(self.width, self.height),
-        # )
-        # self.bg_image_label = customtkinter.CTkLabel(self, image=bg_image)
-        # self.bg_image_label.grid(row=0, column=0)
-
-        # Switch back to proper directory
-        os.chdir(current_dir)
-
-        # Add grid title
-        self.logo_label = customtkinter.CTkLabel(
-            self.sidebar_frame,
-            text="Display Options",
-            font=customtkinter.CTkFont(size=20, weight="bold"),
-        )
-        self.logo_label.grid(row=0, column=0, padx=20, pady=(60, 10), sticky="s")
-
-        # Start first grid / column definitions
-
-        # Display Detail Level
-        self.detail_label = customtkinter.CTkLabel(self.sidebar_frame, text="Display Detail Level:", anchor="w")
-        self.detail_label.grid(row=1, column=0, padx=20, pady=(10, 0))
-        self.sidebar_detail_option = customtkinter.CTkOptionMenu(
-            self.sidebar_frame,
-            values=["0", "1", "2", "3", "4"],
-            command=self.detail_selected_event,
-        )
-        self.sidebar_detail_option.grid(row=2, column=0, padx=20, pady=(10, 10))
-
-        # Everything
-        self.everything_checkbox = customtkinter.CTkCheckBox(
-            self.sidebar_frame,
-            command=self.everything_event,
-            text="Just Display Everything!",
-            onvalue=True,
-            offvalue=False,
-        )
-        self.everything_checkbox.grid(row=3, column=0, padx=20, pady=10, sticky="w")
-
-        # Display 'Condition' checkbox
-        self.condition_checkbox = customtkinter.CTkCheckBox(
-            self.sidebar_frame,
-            command=self.condition_event,
-            text="Display Profile and Task Action Conditions",
-            onvalue=True,
-            offvalue=False,
-        )
-        self.condition_checkbox.grid(row=4, column=0, padx=20, pady=10, sticky="w")
-
-        # Display 'TaskerNet' checkbox
-        self.taskernet_checkbox = customtkinter.CTkCheckBox(
-            self.sidebar_frame,
-            command=self.taskernet_event,
-            text="Display TaskerNet Info",
-            onvalue=True,
-            offvalue=False,
-        )
-        self.taskernet_checkbox.grid(row=5, column=0, padx=20, pady=10, sticky="w")
-
-        # Display 'Tasker Preferences' checkbox
-        self.preferences_checkbox = customtkinter.CTkCheckBox(
-            self.sidebar_frame,
-            command=self.preferences_event,
-            text="Display Tasker Preferences",
-            onvalue=True,
-            offvalue=False,
-        )
-        self.preferences_checkbox.grid(row=6, column=0, padx=20, pady=10, sticky="w")
-
-        # Display 'Twisty' checkbox
-        self.twisty_checkbox = customtkinter.CTkCheckBox(
-            self.sidebar_frame,
-            command=self.twisty_event,
-            text="Hide Task Details Under Twisty",
-            onvalue=True,
-            offvalue=False,
-        )
-        self.twisty_checkbox.grid(row=7, column=0, padx=20, pady=10, sticky="w")
-
-        # Display 'directory' checkbox
-        self.directory_checkbox = customtkinter.CTkCheckBox(
-            self.sidebar_frame,
-            command=self.directory_event,
-            text="Display Directory",
-            onvalue=True,
-            offvalue=False,
-        )
-        self.directory_checkbox.grid(row=8, column=0, padx=20, pady=10, sticky="w")
-
-        # Outline
-        self.outline_checkbox = customtkinter.CTkCheckBox(
-            self.sidebar_frame,
-            command=self.outline_event,
-            text="Display Configuration Outline",
-            onvalue=True,
-            offvalue=False,
-        )
-        self.outline_checkbox.grid(row=9, column=0, padx=20, pady=10, sticky="w")
-
-        # Names: Bold / Highlight / Italicise
-        self.display_names_label = customtkinter.CTkLabel(
-            self.sidebar_frame,
-            text="Project/Profile/Task/Scene Names:",
-            anchor="s",
-        )
-        self.display_names_label.grid(row=10, column=0, padx=20, pady=10)
-        # Bold
-        self.bold_checkbox = customtkinter.CTkCheckBox(
-            self.sidebar_frame,
-            command=self.names_bold_event,
-            text="Bold",
-            onvalue=True,
-            offvalue=False,
-        )
-        self.bold_checkbox.grid(row=11, column=0, padx=20, pady=0, sticky="ne")
-        # Italicize
-        self.italicize_checkbox = customtkinter.CTkCheckBox(
-            self.sidebar_frame,
-            command=self.names_italicize_event,
-            text="Italicize",
-            onvalue=True,
-            offvalue=False,
-        )
-        self.italicize_checkbox.grid(row=11, column=0, padx=20, pady=0, sticky="nw")
-        # Highlight
-        self.highlight_checkbox = customtkinter.CTkCheckBox(
-            self.sidebar_frame,
-            command=self.names_highlight_event,
-            text="Highlight",
-            onvalue=True,
-            offvalue=False,
-        )
-        self.highlight_checkbox.grid(row=12, column=0, padx=20, pady=5, sticky="ne")
-        # Underline
-        self.underline_checkbox = customtkinter.CTkCheckBox(
-            self.sidebar_frame,
-            command=self.names_underline_event,
-            text="Underline",
-            onvalue=True,
-            offvalue=False,
-        )
-        self.underline_checkbox.grid(row=12, column=0, padx=20, pady=5, sticky="nw")
-
-        # Indentation
-        self.indent_label = customtkinter.CTkLabel(
-            self.sidebar_frame,
-            text="If/Then/Else Indentation Amount:",
-            anchor="s",
-        )
-        self.indent_label.grid(row=13, column=0, padx=20, pady=(10, 0))
-        # Indentation Amount
-        self.indent_option = customtkinter.CTkOptionMenu(
-            self.sidebar_frame,
-            values=[
-                "0",
-                "1",
-                "2",
-                "3",
-                "4",
-                "5",
-                "6",
-                "7",
-                "8",
-                "9",
-                "10",
-            ],
-            command=self.indent_selected_event,
-        )
-        self.indent_option.grid(row=14, column=0, padx=20, pady=(10, 10))
-
-        # Screen Appearance: Light / Dark / System
-        self.appearance_mode_label = customtkinter.CTkLabel(self.sidebar_frame, text="Appearance Mode:", anchor="sw")
-        self.appearance_mode_label.grid(row=15, column=0, padx=20, pady=10)
-        self.appearance_mode_optionemenu = customtkinter.CTkOptionMenu(
-            self.sidebar_frame,
-            values=["Light", "Dark", "System"],
-            command=self.change_appearance_mode_event,
-        )
-        self.appearance_mode_optionemenu.grid(row=16, column=0, padx=0, sticky="n")
-
-        # 'Reset Settings' button definition
-        self.reset_button = customtkinter.CTkButton(
-            # master=self,
-            self.sidebar_frame,
-            fg_color="#246FB6",
-            border_width=2,
-            text="Reset Options",
-            command=self.reset_settings_event,
-        )
-        self.reset_button.grid(row=17, column=0, padx=20, pady=20, sticky="")
-
-        # Start second grid / column definitions
-
-        # Font to use
-        self.font_label = customtkinter.CTkLabel(master=self, text="Font To Use In Output:", anchor="sw")
-        self.font_label.grid(row=6, column=1, padx=20, pady=10, sticky="sw")
-        # Get fonts from TkInter
-        font_items, res = get_monospace_fonts()
-        # Delete the tkroot obtained by get_monospace_fonts
-        if PrimeItems.tkroot:
-            del PrimeItems.tkroot
-            PrimeItems.tkroot = None
-        self.font_optionemenu = customtkinter.CTkOptionMenu(
-            master=self,
-            values=font_items,
-            command=self.font_event,
-        )
-        self.font_optionemenu.set(res[0])
-        self.font_optionemenu.grid(row=7, column=1, padx=20, sticky="nw")
-
-        # Save settings button
-        self.save_settings_button = customtkinter.CTkButton(
-            master=self,
-            border_color="#6563ff",
-            border_width=2,
-            text="Save Settings",
-            command=self.save_settings_event,
-        )
-        self.save_settings_button.grid(row=8, column=1, padx=20, sticky="sw")
-
-        # Restore settings button
-        self.restore_settings_button = customtkinter.CTkButton(
-            master=self,
-            border_color="#6563ff",
-            border_width=2,
-            text="Restore Settings",
-            command=self.restore_settings_event,
-        )
-        self.restore_settings_button.grid(row=9, column=1, padx=20, pady=10, sticky="nw")
-
-        # 'Get Backup Settings' button definition
-        self.display_backup_button("Get Backup from Android Device", "#246FB6", "#6563ff", self.get_backup_event)
-
-        # 'Display Help' button definition
-        self.help_button = customtkinter.CTkButton(
-            master=self,
-            fg_color="#246FB6",
-            border_width=2,
-            text="Display Help",
-            command=self.help_event,
-            text_color=("#0BF075", "#ffd941"),
-        )
-        self.help_button.grid(row=6, column=2, padx=(20, 20), pady=(20, 20), sticky="ne")
-
-        # 'Backup Help' button definition
-        self.backup_help_button = customtkinter.CTkButton(
-            master=self,
-            fg_color="#246FB6",
-            border_width=2,
-            text="Get Backup Help",
-            command=self.backup_help_event,
-            text_color=("#0BF075", "#ffd941"),
-        )
-        self.backup_help_button.grid(row=7, column=2, padx=(20, 20), pady=(20, 20), sticky="ne")
-
-        # 'Run' button definition
-        self.run_button = customtkinter.CTkButton(
-            master=self,
-            fg_color="#246FB6",
-            border_width=2,
-            text="Run",
-            command=self.run_program,
-            text_color=("#0BF075", "#1AD63D"),
-        )
-        self.run_button.grid(row=8, column=2, padx=(20, 20), pady=(20, 20), sticky="e")
-
-        # 'ReRun' button definition
-        self.rerun_button = customtkinter.CTkButton(
-            master=self,
-            fg_color="#246FB6",
-            border_width=2,
-            text="ReRun",
-            command=self.rerun_the_program,
-            text_color=("#0BF075", "#1AD63D"),
-        )
-        self.rerun_button.grid(row=9, column=2, padx=(20, 20), pady=(20, 20), sticky="e")
-
-        # 'Exit' button definition
-        self.exit_button = customtkinter.CTkButton(
-            master=self,
-            fg_color="#246FB6",
-            border_width=2,
-            text="Exit",
-            command=self.exit_program,
-            text_color="Red",
-        )
-        self.exit_button.grid(row=10, column=2, padx=(20, 20), pady=(20, 20), sticky="e")
-
-        # Create textbox for Help information
-        self.textbox = customtkinter.CTkTextbox(self, height=600, width=250)
-        self.textbox.configure(scrollbar_button_color="#6563ff", wrap="word")
-        self.textbox.grid(row=0, column=1, padx=(20, 0), pady=(20, 0), sticky="ew")
-
-        # Start third grid / column definitions
-        # create tabview for Name, Color, and Debug
-        self.tabview = customtkinter.CTkTabview(self, width=250, segmented_button_fg_color="#6563ff")
-        self.tabview.grid(row=0, column=2, padx=(20, 0), pady=(20, 0), sticky="nsew")
-        self.tabview.add("Specific Name")
-        self.tabview.add("Colors")
-        self.tabview.add("Debug")
-
-        self.tabview.tab("Specific Name").grid_columnconfigure(0, weight=1)  # configure grid of individual tabs
-        self.tabview.tab("Colors").grid_columnconfigure(0, weight=1)
-
-        # Project Name
-        self.string_input_button1 = customtkinter.CTkRadioButton(
-            self.tabview.tab("Specific Name"),
-            text="Project Name",
-            command=self.single_project_name_event,
-            fg_color="#6563ff",
-            border_color="#1bc9ff",
-        )
-        self.string_input_button1.grid(row=1, column=0, padx=20, pady=(10, 10), sticky="nsew")
-
-        # Profile Name
-        self.string_input_button2 = customtkinter.CTkRadioButton(
-            self.tabview.tab("Specific Name"),
-            text="Profile Name",
-            command=self.single_profile_name_event,
-            fg_color="#6563ff",
-            border_color="#1bc9ff",
-        )
-        self.string_input_button2.grid(row=2, column=0, padx=20, pady=(10, 10), sticky="nsew")
-
-        # Task Name
-        self.string_input_button3 = customtkinter.CTkRadioButton(
-            self.tabview.tab("Specific Name"),
-            text="Task Name",
-            command=self.single_task_name_event,
-            fg_color="#6563ff",
-            border_color="#1bc9ff",
-        )
-        self.string_input_button3.grid(row=3, column=0, padx=20, pady=(10, 10), sticky="nsew")
-
-        # Prompt for the name
-        self.name_label = customtkinter.CTkLabel(self.tabview.tab("Specific Name"), text="(Pick ONLY One)", anchor="w")
-        self.name_label.grid(row=4, column=0, padx=20, pady=(10, 10))
-
-        # Setup to get various display colors
-        self.label_tab_2 = customtkinter.CTkLabel(self.tabview.tab("Colors"), text="Set Various Display Colors Here")
-        self.label_tab_2.grid(row=0, column=0, padx=0, pady=0)
-        self.colors_optionemenu = customtkinter.CTkOptionMenu(
-            self.tabview.tab("Colors"),
-            values=[
-                "Projects",
-                "Profiles",
-                "Disabled Profiles",
-                "Launcher Task",
-                "Profile Conditions",
-                "Tasks",
-                "(Task) Actions",
-                "Action Conditions",
-                "Action Labels",
-                "Action Names",
-                "Scenes",
-                "Background",
-                "Bullets",
-                "TaskerNet Information",
-                "Tasker Preferences",
-                "Highlight",
-                "Heading",
-            ],
-            command=self.colors_event,
-        )
-        self.colors_optionemenu.grid(row=1, column=0, padx=20, pady=(10, 10))
+        # Initialize GUI
+        initialize_gui(self)
 
-        # Debug Mode checkbox
-        self.debug_checkbox = customtkinter.CTkCheckBox(
-            self.tabview.tab("Debug"),
-            text="Debug Mode",
-            command=self.debug_checkbox_event,
-            onvalue=True,
-            offvalue=False,
-        )
-        self.debug_checkbox.configure(border_color="#6563ff")
-        self.debug_checkbox.grid(row=4, column=3, padx=20, pady=10, sticky="w")
-
-        # Runtime
-        self.runtime_checkbox = customtkinter.CTkCheckBox(
-            self.tabview.tab("Debug"),
-            text="Display Runtime Settings",
-            command=self.runtime_checkbox_event,
-            onvalue=True,
-            offvalue=False,
-        )
-        self.runtime_checkbox.configure(border_color="#6563ff")
-        self.runtime_checkbox.grid(row=3, column=3, padx=20, pady=10, sticky="w")
+        # Add menu elements
+        initialize_screen(self)
 
         # set default values
         self.set_defaults(True)
 
         # Now restore the settings and update the fields if not resetting.
         if not PrimeItems.program_arguments["reset"]:
             self.restore_settings_event()
-            self.textbox.destroy()  # Clear any prior error message
-            self.display_message_box("Settings restored.", True)
+        else:
+            self.display_message_box("GUI started with the '-reset' option.\n", True)
+
+        if self.android_ipaddr:
+            # Display backup details as a label
+            self.display_backup_details()
+
+        # Check for single item only to be displayed
+        if self.single_project_name:
+            self.single_name_status(f"Display only Project '{self.single_project_name}'.", "#3f99ff")
+        if self.single_profile_name:
+            self.single_name_status(f"Display only Profile '{self.single_profile_name}'.", "#3f99ff")
+        if self.single_task_name:
+            self.single_name_status(f"Display only Task '{self.single_task_name}'.", "#3f99ff")
+
+        # Check if newer version of our code is available on Pypi (only check every 24 hours).
+        # If so, add a button to enable user to update.
+        # TODO For testing only = True.  False for production
+        test_button = False
+        if is_new_version() or test_button:
+            self.new_version = True
+            # We have a new version.  Let user upgrade.
+            self.upgrade_button = add_button(
+                self,
+                self,
+                "",
+                "#79ff94",
+                "#6563ff",
+                self.upgrade_event,
+                1,
+                "Upgrade to Latest Version",
+                "1",
+                6,
+                2,
+                (0, 170),
+                (0, 20),
+                "sw",
+            )
+
+            self.message = self.message + "\n\nA new version of MapTasker is available."
+        else:
+            self.new_version = False
+
+        # See if we have a changelog, and get it if we do.
+        check_for_changelog(self)
+
+        if self.message:
+            self.display_message_box(self.message, True)
 
     # ##################################################################################
     # Establish all of the default values used
     # ##################################################################################
-    def set_defaults(self, first_time: bool) -> None:  # noqa: ANN101
+    def set_defaults(self, first_time: bool) -> None:
         # Item names must be the same as their value in
         #  PrimeItems.program_arguments
         """
         Sets default values for attributes.
         Args:
             first_time: {bool}: Indicates if it is the first time running the program.
         Returns:
@@ -666,143 +263,134 @@
         - Sets default values for attributes like sidebar detail level, conditions flags etc.
         - Sets appearance mode, indent etc.
         - Inserts help text if first_time is True
         - Initializes empty dictionaries and default font
         - Handles initialization of backup file attributes if not already defined
         - Displays single name status message
         }"""
-        self.sidebar_detail_option.configure(values=["0", "1", "2", "3", "4"])
-        self.sidebar_detail_option.set("4")
-        self.display_detail_level = 4
-        self.conditions = (
-            self.preferences
-        ) = (
-            self.taskernet
-        ) = (
-            self.debug
-        ) = (
-            self.everything
-        ) = (
-            self.clear_settings
-        ) = (
+        self.sidebar_detail_option.configure(values=["0", "1", "2", "3", "4", "5"])
+        self.sidebar_detail_option.set(str(DEFAULT_DISPLAY_DETAIL_LEVEL))
+        self.display_detail_level = DEFAULT_DISPLAY_DETAIL_LEVEL
+        self.conditions = self.preferences = self.taskernet = self.debug = self.everything = self.clear_settings = (
             self.reset
-        ) = (
-            self.restore
-        ) = (
-            self.exit
-        ) = (
-            self.bold
-        ) = (
-            self.highlight
-        ) = (
-            self.italicize
-        ) = (
-            self.underline
-        ) = (
+        ) = self.restore = self.exit = self.bold = self.highlight = self.italicize = self.underline = (
             self.go_program
-        ) = (
-            self.outline
-        ) = (
-            self.rerun
-        ) = self.runtime = self.save = self.twisty = self.directory = self.fetched_backup_from_android = False
+        ) = self.outline = self.rerun = self.list_files = self.runtime = self.save = self.twisty = self.directory = (
+            self.pretty
+        ) = self.fetched_backup_from_android = False
         self.single_project_name = self.single_profile_name = self.single_task_name = self.file = ""
         self.color_text_row = 2
         self.appearance_mode_optionemenu.set("System")
         self.appearance_mode = "system"
-        self.indent_option.set("4")
+        self.indent_option.set(DEFAULT_DISPLAY_DETAIL_LEVEL)
         self.indent = 4
         self.color_labels = []
         self.android_ipaddr = ""
         self.android_port = ""
         self.android_file = ""
         if first_time:
-            self.textbox.insert("0.0", "MapTasker Help\n\n" + INFO_TEXT)
-            self.all_messages = ""
+            # self.textbox.insert("0.0", HELP)
+            self.all_messages = {}
         self.color_lookup = {}  # Setup default dictionary as empty list
         self.font = OUTPUT_FONT
         self.gui = True
         self.color_row = 4
+        self.message = ""
 
         # Display current Items setting.
         self.single_name_status("Display all Projects, Profiles, and Tasks.", "#3f99ff")
 
     # ##################################################################################
     # Display the Backup button
     # ##################################################################################
-    def display_backup_button(self, the_text: str, color1: str, color2: str, routine: object) -> None:  # noqa: ANN101
-        # 'Get Backup Settings' button definition
+    def display_backup_button(self, the_text: str, color1: str, color2: str, routine: object) -> None:
         """
         Displays a backup button on the GUI.
         Args:
             the_text: The text to display on the button in one line
             color1: The foreground color of the button in one line
             color2: The border color of the button in one line
         Returns:
-            None: Does not return anything
+            self.get_backup_button: the button object
         Processing Logic:
             - Creates a CTkButton object with the given text, colors and command
             - Places the button on row 7, column 1 spanning 2 columns with padding
             - Configures the button to be stuck to the northwest side of its cell
         """
-        self.get_backup_button = customtkinter.CTkButton(
-            master=self,
-            fg_color=color1,
-            border_color=color2,
-            border_width=2,
-            text=the_text,
-            command=routine,
-            text_color=("#0BF075", "#1AD63D"),
+        # 'Get Backup Settings' button definition
+        self.get_backup_button = add_button(
+            self,
+            self,
+            color1,
+            ("#0BF075", "#1AD63D"),
+            color2,
+            routine,
+            1,
+            the_text,
+            2,
+            7,
+            1,
+            (200, 200),
+            (0, 10),
+            "nw",
         )
-        self.get_backup_button.grid(row=7, column=1, columnspan=2, padx=(200, 10), pady=(0, 10), sticky="nw")
+        return self.get_backup_button
 
     # ##################################################################################
     # Display Message Box
     # ##################################################################################
-    def display_message_box(self, message: str, good: bool) -> None:  # noqa: ANN101
-        # If "good", display in green.  Otherwise, must be bad and display in red.
-        r"""
-        Displays a message box with the given message and color.
-
+    def display_message_box(self, message: str, good: bool) -> None:
+        """Display Message Box
         Args:
-            message: The message to display in one line.
-            good: Whether the message is good or bad in one line.
-        Returns:
-            None: No return value in one line.
-
-        - Deletes prior textbox contents
-        - Recreates the textbox
-        - Sets the color based on good/bad
-        - Inserts the accumulated messages
-        - Configures textbox properties
+            message (str): The text to display in the textbox.
+            good (bool): True = No Problem = Green, False = Error = Red
         """
-        color = "Green" if good else "Red"
+
+        # If "good", display in green.  Otherwise, must be bad and display in red.
+        # color = "Green" if good else "Red"
+        bad_color = "red"
+        good_color = "green"
         # Delete prior contents
         self.textbox.destroy()
 
         # Recreate text box
         self.textbox = customtkinter.CTkTextbox(self, height=500, width=600)
         self.textbox.grid(row=0, column=1, padx=20, pady=40, sticky="nsew")
 
-        # Display some colored text
-        # self.textbox.insert('end', 'This is some colored text.\n')
-        # self.textbox.tag_add('color', '1.5', '1.11')  # '1.5' means first line, 5th character; '1.11' means first line, 11th character
-        # self.textbox.tag_config('color', foreground='red')
+        line_num = 0
+
+        # Go through our messages and add each to the text box.
+        for num, key in enumerate(self.all_messages):
+            line_num = num + 1
+            line_num_str = str(line_num)
+            line_detail = self.all_messages[key]
+            # fmt: off
+            self.textbox.insert(f"{line_num_str}.0", line_detail["text"], (line_num_str))
+            self.textbox.tag_add(line_num_str, f"{line_num_str}.0", f"{line_num_str}.{len(line_detail['text'])!s}") # fmt: skip
+            # fmt: on
+            self.textbox.tag_config(line_num_str, foreground=line_detail["color"])
+
+        # Insert the text with our new message into the text box.
+        line_num += 1
+        line_num_str = str(line_num)
+        # Add this message to our dictionary of messages.
+        self.all_messages[line_num] = {"text": f"{message}\n", "color": good_color if good else bad_color}
+        # Add the test and color to the text box.
+        # fmt: off
+        self.textbox.insert(f"{line_num_str}.0", f"{message}\n", (line_num_str))
+        self.textbox.tag_add(line_num_str, f"{line_num_str}.0", f"{line_num_str}.{len(message)!s}")
+        # fmt: on
+        self.textbox.tag_config(line_num_str, foreground=self.all_messages[line_num]["color"])
 
-        # self.all_messages = f"{self.all_messages}{message}\n"
-        self.all_messages = f"{message}\n"
-        # insert at line 0 character 0
-        self.textbox.insert("0.0", self.all_messages)
-        # Set read-only, color, wrap around and font
-        self.textbox.configure(state="disabled", text_color=color, wrap="word", font=(self.font, 14))
         self.textbox.focus_set()
 
     # ##################################################################################
     # Validate name entered
     # ##################################################################################
-    def check_name(self, the_name: str, element_name: str) -> bool:  # noqa: ANN101
+    def check_name(self, the_name: str, element_name: str) -> bool:
         """
         Checks name validity
         Args:
             the_name: str - Name to check
             element_name: str - Element type being named
         Returns:
             bool - Whether name is valid
@@ -812,84 +400,98 @@
             3. Check that named item exists in valid items
             4. If error, display message and clear individual names
             5. If valid, display confirmation message and return True
         """
         error_message = ""
         # Check for missing name
         if not the_name:
-            error_message = (
-                f"\n\nEither the name entered for the {element_name} is blank or the"
-                f" 'Cancel' button was clicked.\n\nAll {element_name}s will be"
-                " displayed."
-            )
+            error_message = [
+                f"Either the name entered for the {element_name} is blank or the 'Cancel' button was clicked.\n",
+                "All Projects, Profiles, and Tasks will be displayed.\n",
+            ]
+
             self.named_item = False
         # Check to make sure only one named item has been entered
         elif self.single_project_name and self.single_profile_name:
-            error_message = (
-                "Error:\n\nYou have entered both a Project and a Profile name!\n\nTry again and only select one."
-            )
+            error_message = [
+                "Error:\n\n",
+                "You have entered both a Project and a Profile name!\n",
+                "Try again and only select one.",
+            ]
         elif self.single_project_name and self.single_task_name:
-            error_message = (
-                "Error:\n\nYou have entered both a Project and a Task name!\n\nTry again and only select one."
-            )
+            error_message = [
+                "Error:\n\n",
+                "You have entered both a Project and a Task name!\n",
+                "Try again and only select one.",
+            ]
         elif self.single_profile_name and self.single_task_name:
-            error_message = (
-                "Error:\n\nYou have entered both a Profile and a Task name!\n\nTry again and only select one."
-            )
+            error_message = [
+                "Error:\n\n",
+                "You have entered both a Profile and a Task name!\n",
+                "Try again and only select one.",
+            ]
         # Make sure the named item exists
         elif not valid_item(the_name, element_name, self.debug, self.appearance_mode):
-            error_message = f'Error: "{the_name}" {element_name} not found!!  Try again.\n{PrimeItems.error_msg}'
+            error_message = [f'Error: "{the_name}" {element_name} not found!  Try again.\n']
 
         # If we have an error, display it and blank out the various individual names
         if error_message:
-            # Delete prior contents
-            self.all_messages = ""
-
-            self.display_message_box(error_message, False)
+            self.display_multiple_messages(error_message, False)
             (
                 self.single_project_name,
                 self.single_profile_name,
                 self.single_task_name,
             ) = ("", "", "")
             return False
 
+        # No error.
         self.display_message_box(
             f"Display only the '{the_name}' {element_name} (overrides any previous set name).",
             True,
         )
         return True
 
     # ##################################################################################
     # Display single item status.
     # ##################################################################################
-    def single_name_status(self, status_message: str, color_to_use: str) -> None:  # noqa: ANN101
+    def single_name_status(self, status_message: str, color_to_use: str) -> None:
         # Display The selection
         """
         Display a status message with a given color.
         Args:
             status_message: The status message to display in one line.
             color_to_use: The color to use for the text in one line.
         Returns:
             None: No value is returned.
         - The status message and color are passed to a CTkLabel widget.
         - The label is placed in a grid layout on the "Specific Name" tab.
         - Text color is set using the passed color."""
-        self.single_label = customtkinter.CTkLabel(
+        # Clear out any previous label
+        with contextlib.suppress(AttributeError):
+            self.single_label.destroy()
+        # Display the label.
+        self.single_label = add_label(
+            self,
             self.tabview.tab("Specific Name"),
-            text=status_message,
-            anchor="w",
-            text_color=("#0BF075", color_to_use),
+            status_message,
+            ("#0BF075", f"{color_to_use}"),
+            0,
+            "normal",
+            5,
+            0,
+            20,
+            (10, 10),
+            "w",
         )
-        self.single_label.grid(row=5, column=0, padx=20, pady=(10, 10), sticky="nsew")
 
     # ##################################################################################
     # Process single name selection/event
     # ##################################################################################
     def process_name_event(
-        self,  # noqa: ANN101
+        self,
         my_name: str,
         checkbox1: customtkinter.CHECKBUTTON,
         checkbox2: customtkinter.CHECKBUTTON,
         checkbox3: customtkinter.CHECKBUTTON,
     ) -> None:
         #  Clear any prior error message.
         """
@@ -933,47 +535,46 @@
 
                 case "Profile":
                     self.single_profile_name = name_entered
 
                 case "Task":
                     self.single_task_name = name_entered
 
-                case _:
-                    pass
-
             # Let the user know...
             self.single_name_status(f"Display only {my_name} '{name_entered}'.", "#3f99ff")
 
         else:
             self.single_name_status("Display all Projects, Profiles, and Tasks.", "#3f99ff")
 
         # Deselect the check box just selected
         checkbox3.deselect()
 
     # ##################################################################################
     # Process single name restore
     # ##################################################################################
     def process_single_name_restore(
-        self,  # noqa: ANN101
+        self,
         my_name: str,
         name_entered: str,
     ) -> None:
-        # Name sure it is a valid name
         """
         Restores a single name based on the provided name type.
         Args:
             my_name: Name of the type to restore (Project, Profile, Task)
             name_entered: Name entered by the user
         Returns:
             None: No value is returned
         Processing Logic:
             - Check if the entered name is valid
             - Clear existing single name values
             - Match the name type and assign the entered name to the correct single name attribute
             - Do nothing if an invalid name type is provided"""
+        # Make sure it is a valid name
+        if self.file:
+            PrimeItems.file_to_get = self.file  # Load file for def get_xml
         if name_entered and self.check_name(name_entered, my_name):
             self.single_project_name = self.single_profile_name = self.single_task_name = ""
 
             match my_name:
                 case "Project":
                     self.single_project_name = name_entered
                 case "Profile":
@@ -982,15 +583,15 @@
                     self.single_task_name = name_entered
                 case _:
                     pass
 
     # ##################################################################################
     # Process the Project Name entry
     # ##################################################################################
-    def single_project_name_event(self) -> None:  # noqa: ANN101
+    def single_project_name_event(self) -> None:
         """Generates a single project name event from button inputs
         Args:
             self: The class instance
         Returns:
             None: No value is returned
         - Gets the project name from the second button
         - Gets the event type from the third button
@@ -1002,15 +603,15 @@
             self.string_input_button3,
             self.string_input_button1,
         )
 
     # ##################################################################################
     # Process the Profile Name entry
     # ##################################################################################
-    def single_profile_name_event(self) -> None:  # noqa: ANN101
+    def single_profile_name_event(self) -> None:
         """Generates a single profile name event from button inputs
         Args:
             self: The class instance
         Returns:
             None: No value is returned
         - Gets name from button1 input
         - Gets category from button3 input
@@ -1022,15 +623,15 @@
             self.string_input_button3,
             self.string_input_button2,
         )
 
     # ##################################################################################
     # Process the Task Name entry
     # ##################################################################################
-    def single_task_name_event(self) -> None:  # noqa: ANN101
+    def single_task_name_event(self) -> None:
         """Processes a single task name event.
         Args:
             self: The class instance.
         Returns:
             None: Does not return anything.
         - Gets the task name from the first string input button
         - Gets additional details from the other string input buttons
@@ -1041,30 +642,30 @@
             self.string_input_button2,
             self.string_input_button3,
         )
 
     # ##################################################################################
     # Process the screen mode: dark, light, system
     # ##################################################################################
-    def change_appearance_mode_event(self, new_appearance_mode: str) -> None:  # noqa: ANN101
+    def change_appearance_mode_event(self, new_appearance_mode: str) -> None:
         """
         Change the appearance mode of the GUI
         Args:
             new_appearance_mode: The new appearance mode as a string
         Returns:
             None: Does not return anything
         - Set the global appearance mode to the new mode
         - Update the local appearance mode attribute to the new lowercased mode"""
         customtkinter.set_appearance_mode(new_appearance_mode)
         self.appearance_mode = new_appearance_mode.lower()
 
     # ##################################################################################
     # Process the screen mode: dark, light, system
     # ##################################################################################
-    def font_event(self, font_selected: str) -> None:  # noqa: ANN101
+    def font_event(self, font_selected: str) -> None:
         """
         Sets the font for the GUI
         Args:
             font_selected: The font name selected by the user
         Returns:
             None: No value is returned
         Processing Logic:
@@ -1083,17 +684,33 @@
             anchor="sw",
             font=(font_selected, 14),
         )
         self.font_out_label.grid(row=6, column=1, padx=10, pady=10, sticky="sw")
         self.display_message_box(f"Font To Use set to {font_selected}", True)
 
     # ##################################################################################
+    # Clear the message text box.
+    # ##################################################################################
+    def clear_messages_event(self) -> None:
+        """
+        Clears the message box
+        Args:
+            None
+        Returns:
+            None
+        Processing Logic:
+            - Destroys the message box
+        """
+        self.all_messages = {}
+        self.textbox.destroy()
+
+    # ##################################################################################
     # Process the Display Detail Level selection
     # ##################################################################################
-    def detail_selected_event(self, display_detail: str) -> None:  # noqa: ANN101
+    def detail_selected_event(self, display_detail: str) -> None:
         """
         Set display detail level and update UI
         Args:
             display_detail (str): The selected display detail level
         Returns:
             None
         Processing Logic:
@@ -1113,15 +730,15 @@
             )
             self.twisty = False
             self.twisty_checkbox.deselect()
 
     # ################################################################################
     # Select or deselect a checkbox based on the value passed in
     # ################################################################################
-    def get_input_and_put_message(self, checkbox: customtkinter.CHECKBUTTON, title: str) -> bool:  # noqa: ANN101
+    def get_input_and_put_message(self, checkbox: customtkinter.CHECKBUTTON, title: str) -> bool:
         """
         Get checkbox value and display message
         Args:
             checkbox: Customtkinter checkbox object
             title: Title of message box
         Returns:
             checkbox_value: Value of checkbox
@@ -1131,15 +748,15 @@
         checkbox_value = checkbox.get()
         self.inform_message(title, checkbox_value, "")
         return checkbox_value
 
     # ##################################################################################
     # Process the Identation Amount selection
     # ##################################################################################
-    def indent_selected_event(self, ident_amount: str) -> None:  # noqa: ANN101
+    def indent_selected_event(self, ident_amount: str) -> None:
         """Indent selected text or code block
         Args:
             ident_amount: The amount of indentation to apply as a string
         Returns:
             None: No value is returned
         - Set the indent attribute to the passed ident_amount
         - Update the indent option dropdown to the selected amount
@@ -1147,15 +764,15 @@
         self.indent = ident_amount
         self.indent_option.set(ident_amount)
         self.inform_message("Indentation Amount", True, ident_amount)
 
     # ##################################################################################
     # Process color selection
     # ##################################################################################
-    def colors_event(self, color_selected_item: str) -> None:  # noqa: ANN101
+    def colors_event(self, color_selected_item: str) -> None:
         """
         Changes the color for a selected item
         Args:
             color_selected_item (str): The item whose color is to be changed
         Returns:
             None
         - Checks if the associated display flag for the selected item is True
@@ -1210,33 +827,33 @@
             self.color_row += 1
             if self.color_row > max_row:
                 self.color_row = 4
 
     # ##################################################################################
     # Color selected...process it.
     # ##################################################################################
-    def extract_color_from_event(self, color: str, color_selected_item: str) -> None:  # noqa: ANN101
+    def extract_color_from_event(self, color: str, color_selected_item: str) -> None:
         """Maps a color name to a selected item
         Args:
             color: str - The color name
             color_selected_item: str - The name of the selected item
         Returns:
             None - No return value
         Maps a color name to a selected item:
             - Looks up the color name in a dictionary of color types
             - Adds the color as a value to the color lookup dictionary using the looked up color type as the key
             - This associates the given color with the given selected item"""
-        self.color_lookup[
-            TYPES_OF_COLOR_NAMES[color_selected_item]
-        ] = color  # Add color for the selected item to our dictionary
+        self.color_lookup[TYPES_OF_COLOR_NAMES[color_selected_item]] = (
+            color  # Add color for the selected item to our dictionary
+        )
 
     # ##################################################################################
     # Process the 'conditions' checkbox
     # ##################################################################################
-    def condition_event(self) -> None:  # noqa: ANN101
+    def condition_event(self) -> None:
         """
         Get input and put message for condition checkbox
         Args:
             self: The class instance
             condition_checkbox: Condition checkbox input
             message: Message to display
         Returns:
@@ -1246,33 +863,49 @@
         - Store input value in self.conditions"""
         self.conditions = self.get_input_and_put_message(
             self.condition_checkbox,
             "Display Profile and Task Action Conditions",
         )
 
     # ##################################################################################
-    # Process the 'conditions' checkbox
+    # Process the 'Outline' checkbox
     # ##################################################################################
-    def outline_event(self) -> None:  # noqa: ANN101
+    def outline_event(self) -> None:
         """
         Display Configuration Outline
         Args:
             self: The class instance
         Returns:
             None: Does not return anything
         - Get the input value of the outline_checkbox attribute
         - Call the get_input_and_put_message method to get user input and display a message
         - Assign the return value to the outline attribute
         """
         self.outline = self.get_input_and_put_message(self.outline_checkbox, "Display Configuration Outline")
 
     # ##################################################################################
+    # Process the 'Prettier' checkbox
+    # ##################################################################################
+    def pretty_event(self) -> None:
+        """
+        Display Configuration Outline
+        Args:
+            self: The class instance
+        Returns:
+            None: Does not return anything
+        - Get the input value of the outline_checkbox attribute
+        - Call the get_input_and_put_message method to get user input and display a message
+        - Assign the return value to the outline attribute
+        """
+        self.pretty = self.get_input_and_put_message(self.pretty_checkbox, "Display Pretty Output")
+
+    # ##################################################################################
     # Process the 'everything' checkbox
     # ##################################################################################
-    def everything_event(self) -> None:  # noqa: ANN101
+    def everything_event(self) -> None:
         # Dictionary of program arguments and function to run for each upon restoration.
         """
         Handles toggling all options in the Everything event
         Args:
             self: The class instance
         Returns:
             None: Does not return anything
@@ -1297,64 +930,69 @@
                 "Display Configuration Outline",
             ),
             "preferences": lambda: self.select_deselect_checkbox(
                 self.preferences_checkbox,
                 value,
                 "Display Tasker Preferences",
             ),
+            "pretty": lambda: self.select_deselect_checkbox(
+                self.pretty_checkbox,
+                value,
+                "Display Prettier Output",
+            ),
             "runtime": lambda: self.select_deselect_checkbox(self.runtime_checkbox, value, "Display Runtime Settings"),
             "taskernet": lambda: self.select_deselect_checkbox(
                 self.taskernet_checkbox,
                 value,
                 "Display TaskerNet Information",
             ),
-            "twisty": lambda: self.select_deselect_checkbox(
-                self.twisty_checkbox,
-                value,
-                "Hide Task Details Under Twisty",
-            ),
-            "display_detail_level": lambda: self.detail_selected_event("4"),
+            # "twisty": lambda: self.select_deselect_checkbox(
+            #    self.twisty_checkbox,
+            #    value,
+            #    "Hide Task Details Under Twisty",
+            # ),
+            "display_detail_level": lambda: self.detail_selected_event(DEFAULT_DISPLAY_DETAIL_LEVEL),
         }
 
         self.everything = self.everything_checkbox.get()
         value = self.everything
 
-        new_message = all_messages = ""
+        # new_message = all_messages = ""
         for key in message_map:
             if message_func := message_map.get(key):
-                new_message = f"{message_func()}"
-                all_messages = f"{all_messages}{new_message}"
+
+                # Handle toggle: select/deselect checkbox and set/unset setting.
+                self.display_message_box(f"{message_func()}", True)
+
             # Check if key is an attribute on self before setting
             if hasattr(self, key) and key != "display_detail_level":
                 setattr(self, key, value)
 
         # Handle Display Detail Level
-        self.display_detail_level = 4
-
-        self.display_message_box(all_messages, True)
+        self.display_detail_level = DEFAULT_DISPLAY_DETAIL_LEVEL
 
     # ##################################################################################
     # Process the 'Tasker Preferences' checkbox
     # ##################################################################################
-    def preferences_event(self) -> None:  # noqa: ANN101
+    def preferences_event(self) -> None:
         """
         Get user input on whether to display tasker preferences
         Args:
             self: The class instance
         Returns:
             None: Does not return anything
         - Get user input from preferences_checkbox checkbox
         - Store input in self.preferences
         - Display message based on input to confirm action"""
         self.preferences = self.get_input_and_put_message(self.preferences_checkbox, "Display Tasker Preferences")
 
     # ##################################################################################
     # Process the 'Twisty' checkbox
     # ##################################################################################
-    def twisty_event(self) -> None:  # noqa: ANN101
+    def twisty_event(self) -> None:
         """
         Toggle display of task details under a twisty
         Args:
             self: The class instance
         Returns:
             None: No value is returned
         - Get the state of the twisty checkbox and put a message
@@ -1366,18 +1004,24 @@
             self.display_message_box(
                 "This has no effect with Display Detail Level less than 3.  Display Detail Level set to 3!",
                 False,
             )
             self.sidebar_detail_option.set("3")  # display detail level
             self.display_detail_level = "3"
 
+        # Check to see if we are doing everything (they are mutually exclusive)
+        if self.twisty and self.everything:
+            self.display_message_box("Twisty and Everything are mutually exclusive. Unchecking Twisty.", False)
+            self.twisty = False
+            self.twisty_checkbox.deselect()
+
     # ##################################################################################
     # Process the 'Display Directory' checkbox
     # ##################################################################################
-    def directory_event(self) -> None:  # noqa: ANN101
+    def directory_event(self) -> None:
         """
         Get input and put message for directory checkbox
         Args:
             self: The class instance
             directory_checkbox: The directory checkbox
             "Display Directory": The message to display
         Returns:
@@ -1386,30 +1030,30 @@
         - If checked, put message "Display Directory"
         - Does not return anything, just updates class attribute"""
         self.directory = self.get_input_and_put_message(self.directory_checkbox, "Display Directory")
 
     # ##################################################################################
     # Process the 'Bold Names' checkbox
     # ##################################################################################
-    def names_bold_event(self) -> None:  # noqa: ANN101
+    def names_bold_event(self) -> None:
         """
         Get input to display names in bold and put message
         Args:
             self: The class instance
         Returns:
             None: No value is returned
         - Get input value from bold_checkbox attribute
         - Put message "Display Names in Bold" based on input
         - No return value, function updates attribute on class instance"""
         self.bold = self.get_input_and_put_message(self.bold_checkbox, "Display Names in Bold")
 
     # ##################################################################################
     # Process the 'Highlight Names' checkbox
     # ##################################################################################
-    def names_highlight_event(self) -> None:  # noqa: ANN101
+    def names_highlight_event(self) -> None:
         """
         Get input and put message for names highlight checkbox
         Args:
             self: The class instance
             highlight_checkbox: The checkbox input element
             "Display Names Highlighted": The message to display
         Returns:
@@ -1419,15 +1063,15 @@
         - If not checked, do not put any message
         """
         self.highlight = self.get_input_and_put_message(self.highlight_checkbox, "Display Names Highlighted")
 
     # ##################################################################################
     # Process the 'Italicize Names' checkbox
     # ##################################################################################
-    def names_italicize_event(self) -> None:  # noqa: ANN101
+    def names_italicize_event(self) -> None:
         """
         Italicize names based on checkbox input
         Args:
             self: The class instance
         Returns:
             None: No value is returned
         - Get input value from italicize_checkbox checkbox
@@ -1435,15 +1079,15 @@
         - No return value, function updates UI state directly
         """
         self.italicize = self.get_input_and_put_message(self.italicize_checkbox, "Display Names Italicized")
 
     # ##################################################################################
     # Process the 'Underline Names' checkbox
     # ##################################################################################
-    def names_underline_event(self) -> None:  # noqa: ANN101
+    def names_underline_event(self) -> None:
         """
                 Gets user input to display names underlined or not
                 Args:
                     self: The class instance
                 Returns:
                     None: No value is returned
                 - Gets user input from the underline_checkbox checkbox
@@ -1451,15 +1095,15 @@
         #Loading.
         """
         self.underline = self.get_input_and_put_message(self.underline_checkbox, "Display Names Underlined")
 
     # ##################################################################################
     # Process the 'Taskernet' checkbox
     # ##################################################################################
-    def taskernet_event(self) -> None:  # noqa: ANN101
+    def taskernet_event(self) -> None:
         """
         Display TaskerNet Information
         Args:
             self: The TaskerNet object
         Returns:
             None: Does not return anything
         - Check if TaskerNet checkbox is checked
@@ -1467,30 +1111,30 @@
         - Put message dialog to display TaskerNet information
         """
         self.taskernet = self.get_input_and_put_message(self.taskernet_checkbox, "Display TaskerNet Information")
 
     # ##################################################################################
     # Process the 'Runtime' checkbox
     # ##################################################################################
-    def runtime_checkbox_event(self) -> None:  # noqa: ANN101
+    def runtime_checkbox_event(self) -> None:
         """
         Get input and put message for runtime checkbox
         Args:
             self: The class instance
         Returns:
             None: No return value
         - Get value of runtime_checkbox input
         - If checked, put message "Display Runtime Settings"
         - No return value, function modifies instance attributes"""
         self.runtime = self.get_input_and_put_message(self.runtime_checkbox, "Display Runtime Settings")
 
     # ##################################################################################
-    # Rebuilld message box with new text.
+    # Rebuilld message box with new text (e.g. for Help).
     # ##################################################################################
-    def new_message_box(self, message: str) -> None:  # noqa: ANN101
+    def new_message_box(self, message: str) -> None:
         # Clear any prior error message
         """
         Displays a message in a textbox widget.
         Args:
             message (str): The message to display
         Returns:
             None
@@ -1507,57 +1151,87 @@
         self.textbox = customtkinter.CTkTextbox(self, height=600, width=250)
         self.textbox.configure(scrollbar_button_color="#6563ff", wrap="word")
         self.textbox.grid(row=0, column=1, padx=(20, 0), pady=(20, 0), sticky="ew")
         # Insert the text.
         self.textbox.insert("0.0", message)
         # Set read-only, color, wrap around and font
         self.textbox.configure(state="disabled", font=(self.font, 14), wrap="word")
-        # Display some colored text
+        # Display some colored text: the heading
         # self.textbox.insert('end', 'This is some colored text.\n')
         self.textbox.tag_add(
             "color",
             "1.0",
             f"1.{len(message)}",
         )  # '1.5' means first line, 5th character; '1.11' means first line, 11th character
         self.textbox.tag_config("color", foreground="green")
-        self.all_messages = ""
+        self.all_messages = {}
 
     # ##################################################################################
-    # Process the 'Display Help' checkbox
+    # Process the 'Display Help' button
     # ##################################################################################
-    def help_event(self) -> None:  # noqa: ANN101
+    def help_event(self) -> None:
         """Displays help information in a message box.
         Args:
             self: The class instance.
         Returns:
             None: Does not return anything.
         - Constructs a message with help text information
         - Opens a new message box window
         - Displays the help message text in the message box"""
-        self.new_message_box("MapTasker Help\n\n" + INFO_TEXT)
+        self.new_message_box(HELP)
 
     # ##################################################################################
-    # Process the 'Display Help' checkbox
+    # Process the 'Get Backup Help' button
     # ##################################################################################
-    def backup_help_event(self) -> None:  # noqa: ANN101
+    def backup_help_event(self) -> None:
         """Backs up help text and displays it in a message box
         Args:
             self: The class instance
         Returns:
             None: Does not return anything
         Processes:
             - Fetches the backup help text from a constant
             - Creates a new message box window
             - Displays the backup help text in the message box"""
         self.new_message_box("Fetch Backup Help\n\n" + BACKUP_HELP_TEXT)
 
+    # ##################################################################################
+    # Process the '?' List XML Files query button
+    # ##################################################################################
+    def listfile_query_event(self) -> None:
+        """Function to display help text for the listfile_query_event method.
+        Parameters:
+            - self (object): The object that the method is being called on.
+        Returns:
+            - None: This method does not return anything.
+        Processing Logic:
+            - Displays help text for listfile_query_event method.
+            - Uses new_message_box method.
+            - Help text is stored in LISTFILES_HELP_TEXT variable."""
+        self.new_message_box("List XML Files Help\n\n" + LISTFILES_HELP_TEXT)
+
+    # ##################################################################################
+    # Process the '?' Tree View query button
+    # ##################################################################################
+    def treeview_query_event(self) -> None:
+        """Function to display help text for the listfile_query_event method.
+        Parameters:
+            - self (object): The object that the method is being called on.
+        Returns:
+            - None: This method does not return anything.
+        Processing Logic:
+            - Displays help text for treeview_query_event method.
+            - Uses new_message_box method.
+            - Help text is stored in LISTFILES_HELP_TEXT variable."""
+        self.new_message_box("Tree View Help\n\n" + TREEVIEW_HELP_TEXT)
+
     # ################################################################################
     # Inform user of toggle selection
     # ################################################################################
-    def inform_message(self, toggle_name: str, toggle_value: str, number_value: str) -> None:  # noqa: ANN101
+    def inform_message(self, toggle_name: str, toggle_value: str, number_value: str) -> None:
         """
         Set a toggle and display a message box
         Args:
             toggle_name: Name of the toggle being set
             toggle_value: Value of the toggle
             number_value: Optional number value
         Returns:
@@ -1576,15 +1250,15 @@
         else:
             response = "Off"
         self.display_message_box(f"{toggle_name} set{extra}{response}", True)
 
     # ##################################################################################
     # Process the 'Save Settings' checkbox
     # ##################################################################################
-    def save_settings_event(self) -> None:  # noqa: ANN101
+    def save_settings_event(self) -> None:
         # Get program arguments from GUI and store in a temporary dictionary
         """
         Saves program settings from GUI to file.
         Args:
             self: The class instance.
         Returns:
             None
@@ -1607,15 +1281,15 @@
         temp_args, self.color_lookup = save_restore_args(temp_args, self.color_lookup, True)
         self.display_message_box("Settings saved.", True)
 
     # ################################################################################
     # Select or deselect a checkbox based on the value passed in
     # ################################################################################
     def select_deselect_checkbox(
-        self,  # noqa: ANN101
+        self,
         checkbox: customtkinter.CHECKBUTTON,
         checked: bool,
         argument_name: str,
     ) -> str:
         """Select or deselect a checkbox widget
         Args:
             checkbox: The checkbox widget to select or deselect
@@ -1628,15 +1302,15 @@
         - Return a string with the argument name and checked status"""
         checkbox.select() if checked else checkbox.deselect()
         return f"{argument_name} set to {checked}.\n"
 
     # ##################################################################################
     # Restore displays setting from restored value!
     # ##################################################################################
-    def restore_display(self, key: str, value: str) -> str:  # noqa: ANN101
+    def restore_display(self, key: str, value: str) -> str:
         # Dictionary of program arguments and function to run for each upon restoration.
         """
         Restores display settings
         Args:
             key: str - Setting name
             value: str - Setting value
         Returns:
@@ -1645,29 +1319,29 @@
             - Maps setting names to lambda functions for processing
             - Checks for special case settings and sets attribute directly
             - Looks up and runs corresponding lambda function
             - Returns message generated by lambda function
         """
         message = ""
         message_map = {
-            "android_ipaddrt": lambda: f"Get Backup TCP IP Address set to {value}\n",
-            "android_port": lambda: f"Get Backup Port Number set to {value}\n",
-            "android_file": lambda: f"Get Backup File Location set to {value}\n",
+            "android_ipaddr": lambda: f"Get XML TCP IP Address set to {value}\n",
+            "android_port": lambda: f"Get XML Port Number set to {value}\n",
+            "android_file": lambda: f"Get XML File Location set to {value}\n",
             "appearance_mode": lambda: f"Appearance mode set to {value}.\n",
             "bold": lambda: self.select_deselect_checkbox(self.bold_checkbox, value, "Display Names in Bold"),
             "conditions": lambda: self.select_deselect_checkbox(
                 self.condition_checkbox,
                 value,
                 "Display Profile/Task Conditions",
             ),
             "debug": lambda: self.select_deselect_checkbox(self.debug_checkbox, value, "Debug Mode"),
             "directory": lambda: self.select_deselect_checkbox(self.directory_checkbox, value, "Display Directory"),
             "display_detail_level": lambda: self.detail_selected_event(value),
-            "fetched_backup_from_android": lambda: f"Fetched Backup From Android:{value}.\n",
-            "file": lambda: f"Get backup file named '{value}'.\n",
+            "fetched_backup_from_android": lambda: f"Fetched XML From Android:{value}.\n",
+            "file": lambda: f"Get XML file named '{value}'.\n",
             "font": lambda: f"Font set to {value}.\n",
             "highlight": lambda: self.select_deselect_checkbox(
                 self.highlight_checkbox,
                 value,
                 "Display Names Highlighted",
             ),
             "indent": lambda: self.indent_selected_event(value),
@@ -1682,14 +1356,19 @@
                 "Display Configuration Outline",
             ),
             "preferences": lambda: self.select_deselect_checkbox(
                 self.preferences_checkbox,
                 value,
                 "Display Tasker Preferences",
             ),
+            "pretty": lambda: self.select_deselect_checkbox(
+                self.pretty_checkbox,
+                value,
+                "Display Prettier",
+            ),
             "runtime": lambda: self.select_deselect_checkbox(self.runtime_checkbox, value, "Display Runtime Settings"),
             "single_profile_name": lambda: self.process_single_name_restore("Profile", value),
             "single_project_name": lambda: self.process_single_name_restore("Project", value),
             "single_task_name": lambda: self.process_single_name_restore("Task", value),
             "taskernet": lambda: self.select_deselect_checkbox(
                 self.taskernet_checkbox,
                 value,
@@ -1704,31 +1383,43 @@
                 self.underline_checkbox,
                 value,
                 "Display Names Underlined",
             ),
         }
 
         # Processs specific items that have no effect on the GUI
-        if key in {"gui", "save", "restore", "rerun"}:
+        if key in {"gui", "save", "restore", "rerun", "reset"}:
             message = ""
             # Check if key is an attribute on self before setting
             if hasattr(self, key):
                 setattr(self, key, value)
         else:
-            # Use dictionary lookup anmd lambda funtion to process key/value
+            # Use dictionary lookup and lambda funtion to process key/value
             message_func = message_map.get(key)
             if message_func:
                 message = message_func()
 
+        # Cleanup the end of the message if it is not set.
+        the_empty_ending = "set to \n"
+        the_empty_ending_length = len(the_empty_ending)
+        named_ending = "named ''.\n"
+        named_ending_length = len(named_ending)
+        if message is None or message == "":
+            return ""
+        if message.endswith(the_empty_ending):
+            message = f"{message[:-the_empty_ending_length]} is not set.\n"
+        elif message.endswith(named_ending):
+            message = f"{message[:-named_ending_length]} is not named.\n"
+
         return message
 
     # ##################################################################################
     # Process the 'Restore Settings' checkbox
     # ##################################################################################
-    def restore_settings_event(self) -> None:  # noqa: ANN101
+    def restore_settings_event(self) -> None:
         """
         Resets settings to defaults and restores from saved settings file
         Args:
             self: The class instance
         Returns:
             None: No value is returned
         Processing Logic:
@@ -1744,78 +1435,84 @@
         temp_args, self.color_lookup = save_restore_args(temp_args, self.color_lookup, False)
         # Check for errors
         with contextlib.suppress(KeyError):
             if temp_args["msg"]:
                 self.display_message_box(temp_args["msg"], False)
                 temp_args["msg"] = ""
                 return
+
+        # If no colors restored, let user know.
+        if not self.color_lookup:
+            self.display_message_box("Colors set to defaults.", True)
         # Restore progargs values
         if temp_args or self.color_lookup:
             self.extract_settings(temp_args)
             self.restore = True
+
         else:  # Empty?
             self.display_message_box("No settings file found.", False)
-        # Empty message queue so we don't fill it up (causes as display text problem)
-        self.all_messages = ""
 
     # ##################################################################################
     # We have read colors and runtime args from backup file.  Now extract them for use.
     # ##################################################################################
-    def extract_settings(self, temp_args: dict) -> None:  # noqa: ANN101
+    def extract_settings(self, temp_args: dict) -> None:
         """
         Extract settings from arguments dictionary
         Args:
             temp_args: Dictionary of settings
         Returns:
             None: Does not return anything
         - Loops through dictionary and sets attributes on object
         - Calls restore_display to get message for setting change
         - Loops through color lookup and builds message of color changes
         - Displays message box with all setting changes
         """
-        all_messages, new_message = "", ""
-        self.all_messages = ""
         for key, value in temp_args.items():
             if key is not None:
                 setattr(self, key, value)
                 if new_message := self.restore_display(key, value):
-                    all_messages = f"{all_messages}{new_message}"
+                    self.display_message_box(f"{new_message}\n", True)
         # Display the restored color changes, using the reverse dictionary of
         #   TYPES_OF_COLOR_NAMES (found in sysconst.py)
         inv_color_names = {v: k for k, v in TYPES_OF_COLOR_NAMES.items()}
         for key, value in self.color_lookup.items():
             if key is not None:
                 if key == "msg":
                     inv_color_names[key] = ""
                 else:
-                    all_messages = f"{all_messages} {inv_color_names[key]} color set to {value}\n"
+                    with contextlib.suppress(KeyError):
+                        self.display_message_box(f"{inv_color_names[key]} color set to {value}\n", True)
 
         # Display the queue of messages
-        self.display_message_box(f"{all_messages}\nSettings restored.", True)
+        self.display_message_box("Settings restored.\n", True)
 
     # ##################################################################################
     # Display an input field and a label for the user to input a value
     # ##################################################################################
     def display_label_and_input(
-        self,  # noqa: ANN101
+        self,
         label: str,
         default_value: str,
         starting_row: int,
-        indentation_label: int,
+        indentation_x_label: int,
+        indentation_y_label: int,
         input_name: customtkinter.CTkButton,
         label_name: customtkinter.CTkLabel,
+        do_input: bool,
     ) -> None:
         """
         Display an input field and a label for the user to input a value
         Args:
             label: The label to display
             default_value: The default value to display
             starting_row: The grid row that the label starts on
-            indentation_label: the x indentation amount for the label
+            indentation_x_label: the x indentation amount for the label
+            indentation_y_label: the y indentation amount for the label
             input_name: the name of the input field
+            do_input: whether to display the input field (True) or not (False)
         Returns:
             The value entered by the user
         Processing Logic:
             - Creates an entry field
             - Adds a label above the entry field
             - Inserts the default value into the entry field
             - Returns the value entered by the user
@@ -1826,108 +1523,197 @@
             text=label,
             anchor="sw",
         )
         label_name.grid(
             row=starting_row,
             column=1,
             columnspan=1,
-            padx=(0, indentation_label),
-            pady=(30, 0),
+            padx=(0, indentation_x_label),
+            pady=(indentation_y_label, 5),
             sticky="ne",
         )
 
-        # Display prompt/input field
-        input_name = customtkinter.CTkEntry(
-            self,
-            placeholder_text=default_value,
-        )
-        input_name.configure(
-            # width=320,
-            fg_color="#246FB6",
-            border_color="#1bc9ff",
-            text_color=("#0BF075", "#1AD63D"),
-        )
-        input_name.insert(0, default_value)
-        input_name.grid(
-            row=starting_row + 1,
-            column=1,
-            columnspan=1,
-            padx=(0, 100),
-            pady=(0, 0),
-            sticky="ne",
-        )
+        if do_input:
+            # Display prompt/input field
+            input_name = customtkinter.CTkEntry(
+                self,
+                placeholder_text=default_value,
+            )
+            input_name.configure(
+                # width=320,
+                fg_color="#246FB6",
+                border_color="#1bc9ff",
+                text_color=("#0BF075", "#1AD63D"),
+            )
+            input_name.insert(0, default_value)
+            next_row = starting_row + 1
+            # If file location, we have to push line up by 1 for some reason.
+            if next_row == 10:
+                next_row = 9
+                sticky = "se"
+            else:
+                sticky = "ne"
+            input_name.grid(
+                row=next_row,
+                column=1,
+                columnspan=1,
+                padx=(0, 80),
+                pady=(0, 0),
+                sticky=sticky,
+            )
         return input_name, label_name
 
     # ##################################################################################
-    # Process the 'Backup' IP Address
+    # Process the 'Backup' IP Address/port/file location
     # ##################################################################################
-    def get_backup_event(self) -> None:  # noqa: ANN101
+    def get_backup_event(self) -> None:
         # Set up default values
         """
         Gets backup event details from user.
         Args:
             self: The class instance.
         Returns:
             None: No value is returned.
         Processing Logic:
         - Sets default backup file HTTP address and location if not provided
         - Creates an entry field to input backup details
         - Adds a label above the entry field
         - Inserts the default backup info into the entry field
         - Replaces the backup button to fetch input details on click
         """
+        # First clear out any entries we may already have filled in.
+        clear_android_buttons(self)
         ###  TCP/IP Address ###
         if self.android_ipaddr == "" or self.android_ipaddr is None:
             self.android_ipaddr = "192.168.0.210"
         self.ip_entry = self.ip_label = None
         self.ip_entry, self.ip_label = self.display_label_and_input(
-            "TCP/IP Address:", self.android_ipaddr, 7, 140, self.ip_entry, self.ip_label,
+            "1-TCP/IP Address:",
+            self.android_ipaddr,
+            7,
+            100,
+            30,
+            self.ip_entry,
+            self.ip_label,
+            True,
         )
 
         ### Port Number ###
         if self.android_port == "" or self.android_port is None:
             self.android_port = "1821"
         self.port_entry = self.port_label = None
         self.port_entry, self.port_label = self.display_label_and_input(
-            "Port Number:", self.android_port, 8, 157, self.port_entry, self.port_label,
+            "2-Port Number:",
+            self.android_port,
+            8,
+            117,
+            30,
+            self.port_entry,
+            self.port_label,
+            True,
         )
 
         ###  File Location ###
         if self.android_file == "" or self.android_file is None:
-            self.android_file = "/Tasker/configs/user/backup.xml"
+            self.android_file = "/Tasker/configs/user/backup.xml".replace("/", PrimeItems.slash)
         self.file_entry = self.file_label = None
         self.file_entry, self.file_label = self.display_label_and_input(
-            "File Location:", self.android_file, 9, 159, self.file_entry, self.file_label,
+            "3-File Location:",
+            self.android_file,
+            9,
+            119,
+            40,
+            self.file_entry,
+            self.file_label,
+            True,
         )
 
         # Add Cancel button
-        self.cancel_entry_button = customtkinter.CTkButton(
+        self.cancel_entry_button = add_button(
+            self,
+            self,
+            "#246FB6",
+            "",
+            "#1bc9ff",
+            self.backup_cancel_event,
+            2,
+            "Cancel Entry",
+            2,
+            8,
+            1,
+            (80, 220),
+            (0, 0),
+            "ne",
+        )
+
+        # Add 'List XML Files' button
+        self.list_files_button = add_button(
+            self,
             self,
-            fg_color="#246FB6",
-            border_width=2,
-            text="Cancel Entry",
-            command=self.backup_cancel_event,
-        )
-        self.cancel_entry_button.configure(
-            # width=320,
-            fg_color="#246FB6",
-            border_color="#1bc9ff",
-            # text_color=("#0BF075", "#1AD63D"),
+            "#246FB6",
+            ("#0BF075", "#1AD63D"),
+            "#1bc9ff",
+            self.list_files_event,
+            2,
+            "List XML Files",
+            2,
+            9,
+            1,
+            (80, 220),
+            (0, 0),
+            "se",
         )
-        self.cancel_entry_button.grid(row=10, column=1, columnspan=1, padx=(370, 0), pady=(0, 0), sticky="ne")
+
+        # Add ...or... label.
+        self.label_or = customtkinter.CTkLabel(
+            master=self,
+            text="...or...",
+            anchor="sw",
+        )
+        self.label_or.grid(
+            row=9,
+            column=1,
+            columnspan=1,
+            padx=(0, 38),
+            pady=(0, 0),
+            sticky="se",
+        )
+
+        #  Query ? button
+        self.list_files_query_button = add_button(
+            self,
+            self,
+            "#246FB6",
+            ("#0BF075", "#ffd941"),
+            "#1bc9ff",
+            self.listfile_query_event,
+            1,
+            "?",
+            2,
+            9,
+            1,
+            (0, 180),
+            (0, 0),
+            "se",
+        )
+        self.list_files_query_button.configure(width=20)
 
         # Replace backup button.
-        self.display_backup_button(
-            "Enter and Click Here to Set Backup Details", "#D62CFF", "#6563ff", self.fetch_backup_event,
+        self.get_backup_button = self.display_backup_button(
+            "Enter 1-3 and Click Here to Set XML Details",
+            "#D62CFF",
+            "#6563ff",
+            self.fetch_backup_event,
         )
+        self.get_backup_button.configure(anchor="center", width=600)
 
     # ##################################################################################
     # Fetch Backup info error...process it.
     # ##################################################################################
-    def backup_error(self, error_message: str) -> None:  # noqa: ANN101
+    def backup_error(self, error_message: str) -> None:
         # Setup error message
         """
         Displays an error message and resets the UI.
 
         Args:
             error_message (str): The error message to display.
         Returns:
@@ -1941,17 +1727,35 @@
         if error_message:
             self.display_message_box(
                 error_message,
                 False,
             )
 
     # ##################################################################################
+    # Get list of lines and output them.
+    # ##################################################################################
+    def display_multiple_messages(self, details: list, good_or_bad: bool) -> None:
+        """
+        Display Android settings based on the given details list.
+
+        :param self: The instance of the class.
+        :param details: A list containing the details to be displayed.
+        :param good_or_bad: True = good (green), False = bad (red).
+        :return: None
+        """
+        for line in details:
+            self.display_message_box(line, good_or_bad)
+
+    # ##################################################################################
     # Fetch the backup ip and file details, and validate.
+    # This function can be entered through two paths:
+    # 1- User clicked on the 'Get Backup Settings' button
+    # 2- User clicked on the 'List XML Files' button
     # ##################################################################################
-    def fetch_backup_event(self) -> None:  # noqa: ANN101
+    def fetch_backup_event(self) -> None:
         """Fetches backup event details from user input
 
         Args:
             self: The class instance
         Returns:
             None: No value is returned
 
@@ -1959,96 +1763,221 @@
         - Splits input into IP address, port and file location
         - Validates IP address format and checks reachability via ping
         - Validates port number format
         - Validates file location is provided
         - Sets backup IP and file location attributes if valid
         - Displays message with backup details
         """
+
         # Get the input entered by the user.
         android_ipaddr = self.ip_entry.get()
         android_port = self.port_entry.get()
-        android_file = self.file_entry.get()
+        # Only get the file if we are not doing a file list.
+        android_file = "" if self.list_files else self.file_entry.get()
 
         # Make sure something was entered into each field.
         error_msg = ""
         if android_ipaddr == "" or android_ipaddr is None:
             error_msg = "Please enter an IP address."
         if android_port == "" or android_port is None:
             error_msg = "Please enter a port number."
-        if android_file == "" or android_file is None:
-            error_msg = "Please enter a file location."
         if error_msg:
             self.display_message_box(error_msg, False)
             return
 
         # Validate each field entered and ping the Android device to make sure it is reachible.
-        failure = ping_android_device(
+        if not ping_android_device(
             self,
             android_ipaddr,
             android_port,
-            android_file,
-        )
-        if failure:
+        ):
             return
 
-        # Get the contents of the file to confirm it is really there.
-        return_code, file_contents = request_file(android_ipaddr, android_port,  android_file)
+        # Either validate the file provided or provide a filelist.  Return code = 2 if list is good.
+        return_code, android_ipaddr, android_port, android_file = validate_or_filelist_xml(
+            self,
+            android_ipaddr,
+            android_port,
+            android_file,
+        )
 
-        if return_code != 0:
+        # Drop here if bad file location or XML file not found.
+        if return_code not in (0, 2):
             self.backup_error("File not found.  Return code: " + str(return_code))
             return
 
-        # All is well.  Dave the info, restore the button and get rid of the input fields.
+        # If we got a good return from getting ther XML filelist, then return to process it.
+        if return_code == 2:
+            return
+
+        # All is well.  Save the info, restore the button and get rid of the input fields.
         self.android_ipaddr = android_ipaddr
         self.android_port = android_port
-        self.android_file = android_file
+        if not self.list_files:
+            self.android_file = android_file
         clear_android_buttons(self)
-        self.display_message_box(
-            (
-                f"\n\nGet Backup IP Address set to: {self.android_ipaddr}\n\nPort"
-                f" Number set to: {self.android_port}\n\nGet"
-                f" Location set to: {self.android_file}"
-                f"\n\nBackup file will be fetched when 'Run' is selected."
-            ),
+
+        # Set our file to get
+        filename_location = self.android_file.rfind(PrimeItems.slash) + 1
+        PrimeItems.file_to_use = self.android_file[filename_location:]
+
+        self.display_multiple_messages(
+            [
+                f"Get XML IP Address set to: {self.android_ipaddr}\n",
+                f"Port Number set to: {self.android_port}\n",
+                f"Get Location set to: {self.android_file}\n",
+                "XML file acquired.\n",
+            ],
             True,
         )
 
+        # Display backup details as a label again.
+        self.display_backup_details()
+
+    # ##################################################################################
+    # Fetching backup from Android.  Let the user know the specific details.
+    # ##################################################################################
+    def display_backup_details(self) -> None:
+        """
+        Displays backup details from Android device.
+        Args:
+            self: The class instance.
+        Returns:
+            None: Does not return anything.
+        Processing Logic:
+            - Displays label and input for getting backup.xml file from Android device
+            - Displays label and input for TCP/IP Address and Port of Android device
+            - Displays label and input for location of backup file on Android device
+        """
+        self.ip_label = add_label(
+            self,
+            self,
+            "Getting XML file from Android device:",
+            "",
+            12,
+            "normal",
+            7,
+            1,
+            (30, 0),
+            (50, 0),
+            "ne",
+        )
+
+        # IP address and port
+        self.port_label = add_label(
+            self,
+            self,
+            f"TCP/IP Address: {self.android_ipaddr}   Port: {self.android_port}",
+            "",
+            12,
+            "normal",
+            8,
+            1,
+            (60, 0),
+            (0, 50),
+            "ne",
+        )
+
+        # Location of backup file on Android device...on same row as IP address and port.
+        self.file_label = add_label(
+            self,
+            self,
+            f"Location: {self.android_file}",
+            "",
+            13,
+            "normal",
+            8,
+            1,
+            (60, 0),
+            (0, 50),
+            "ne",
+        )
+
     # ##################################################################################
     # Cancel the entry of backup parameters
     # ##################################################################################
-    def backup_cancel_event(self) -> None:  # noqa: ANN101
+    def backup_cancel_event(self) -> None:
         """
         Closes the backup details window.
         Args:
             self: The class instance
         Returns:
             None
         """
         clear_android_buttons(self)
-        self.display_message_box("Get Backup Details Cancelled.", True)
+        self.fetched_backup_from_android = False
+        self.android_file = ""
+        self.android_ipaddr = ""
+        self.android_port = ""
+        self.display_message_box("Get XML Details Cancelled.", False)
+
+    # ##################################################################################
+    # List files event
+    # ##################################################################################
+    def list_files_event(self) -> None:
+        """
+        Closes the backup details window.
+        Args:
+            self: The class instance
+        Returns:
+            None
+        """
+        self.list_files = True
+        self.list_files_button.configure(text="List Files Selected")
+        self.fetch_backup_event()
+
+    # ##################################################################################
+    # User has selected a specific XML file from pulldown menu.
+    # ##################################################################################
+    def file_selected_event(self, android_file: str) -> None:
+        """User has selected a specific XML file from pulldown menu.
+        Returns:
+            - None: Adds android_file to file_list."""
+        self.android_file = android_file
+        clear_android_buttons(self)
+        self.display_multiple_messages(
+            [
+                f"Get XML IP Address set to: {self.android_ipaddr}\n",
+                f"Port Number set to: {self.android_port}\n",
+                f"Get Location set to: {self.android_file}\n",
+                "XML file acquired.\n",
+            ],
+            True,
+        )
+
+        # Validate XML file.
+        PrimeItems.program_arguments["gui"] = True
+        return_code, error_message = validate_xml_file(self.android_ipaddr, self.android_port, android_file)
+        if return_code > 0:
+            self.display_message_box(error_message, False)  # Error out and exit
+            return
+
+        # Display backup details as a label again.
+        self.display_backup_details()
 
     # ##################################################################################
     # Process the 'Reset Settings' button
     # ##################################################################################
-    def reset_settings_event(self) -> None:  # noqa: ANN101
+    def reset_settings_event(self) -> None:
         """
         Resets all class settings to default values.
         Args:
             self: The class instance.
         Returns:
             None
         """
         clear_android_buttons(self)
         self.android_ipaddr = ""
         self.android_port = ""
         self.android_file = ""
-        self.sidebar_detail_option.set("3")  # display detail level
+        self.sidebar_detail_option.set(DEFAULT_DISPLAY_DETAIL_LEVEL)  # display detail level
         self.indent_option.set("4")  # Indentation amount
         self.condition_checkbox.deselect()  # Conditions
         self.preferences_checkbox.deselect()  # Tasker Preferences
+        self.pretty_checkbox.deselect()  # Pretty output
         self.taskernet_checkbox.deselect()  # TaskerNet
         self.appearance_mode_optionemenu.set("System")  # Appearance
         customtkinter.set_appearance_mode("System")  # Enforce appearance
         self.debug_checkbox.deselect()  # Debug
         self.display_message_box("Settings reset.", True)
         self.twisty_checkbox.deselect()  # Twisty
         self.directory_checkbox.deselect()  # directory
@@ -2060,18 +1989,27 @@
         self.outline_checkbox.deselect()  # Display outline
         self.everything_checkbox.deselect()  # Display everything
         if self.color_labels:  # is there any color text?
             for label in self.color_labels:
                 label.configure(text="")
         self.set_defaults(False)  # Reset all defaults
 
+        # Cleanup the inline data.
+        clean_up_memory()
+
+        # Setup a temporary PrimeItems since the clean_up_memory cleared it all out.
+        PrimeItems.colors_to_use = set_color_mode(self.appearance_mode)
+        PrimeItems.output_lines = LineOut()
+        PrimeItems.program_arguments = initialize_runtime_arguments()
+        PrimeItems.program_arguments["debug"] = self.debug
+
     # ##################################################################################
     # Process Debug Mode checkbox
     # ##################################################################################
-    def debug_checkbox_event(self) -> None:  # noqa: ANN101
+    def debug_checkbox_event(self) -> None:
         """
         Handle debug checkbox event
         Args:
             self: The class instance
         Returns:
             None
         Processing Logic:
@@ -2085,67 +2023,393 @@
         """
         self.debug = self.debug_checkbox.get()
         if self.debug:
             if Path("backup.xml").is_file():
                 self.display_message_box("Debug mode enabled.", True)
             else:
                 self.display_message_box(
-                    ("Debug mode requires Tasker backup file to be named: 'backup.xml', which is missing!"),
+                    ("Debug mode requires Tasker XML file to be named: 'backup.xml', which is missing.  No change."),
                     False,
                 )
                 self.debug = False
         else:
             self.display_message_box("Debug mode disabled.", True)
 
     # ##################################################################################
+    # User has requested that the colors be result to their defaults.
+    # ##################################################################################
+    def color_reset_event(self) -> None:
+        """Resets the color mode for Tasker items.
+        Parameters:
+            self (object): The current instance of the class.
+        Returns:
+            None: This function does not return anything.
+        Processing Logic:
+            - Resets color mode for Tasker items.
+            - Sets color mode to default.
+            - Displays message box to confirm reset.
+            - Destroys color change window."""
+
+        PrimeItems.colors_to_use = set_color_mode(self.appearance_mode)
+        self.color_lookup = {}
+        self.display_message_box("Tasker items set back to their default colors.", True)
+        with contextlib.suppress(Exception):
+            self.color_change.destroy()
+
+    # ##################################################################################
+    # Close the GUI.
+    # ##################################################################################
+    def cleanup(self, run_only: bool) -> None:
+        """Function:
+        Closes the application.
+        Parameters:
+            run_only (bool): If True, only closes the application. If False, closes the application and withdraws the funds.
+        Returns:
+            None: Does not return anything.
+        Processing Logic:
+            - Closes the application.
+            - If run_only is True, only closes the application.
+            - If run_only is False, withdraws the funds before closing the application."""
+        if run_only:
+            self.quit()
+        else:
+            self.withdraw()
+            self.quit()
+            self.quit()
+            self.sidebar_frame.destroy()
+
+    # ##################################################################################
+    # Validate XML and close the GUI.
+    # ##################################################################################
+    def cleanup_and_run(self, run_only: bool) -> None:
+        """Function: cleanup_and_run
+        Parameters:
+            run_only (bool): Flag to determine if program should only run and not display GUI.
+        Returns:
+            None: Does not return any value.
+        Processing Logic:
+            - Display "Program running..." message.
+            - If XML is not valid, return to GUI.
+            - If XML is valid, exit and return to process_gui.
+            - If XML is not valid, return to GUI."""
+        self.display_message_box("Program running...", True)
+
+        # If XML is not valid, simply return to GUI.  Otherwise, exit and return to process_gui.
+        if PrimeItems.xml_tree is None:
+            PrimeItems.program_arguments["gui"] = True
+            # Get and validate the XML.
+            if self.load_xml():  # If true, the XML is valid.  Signal exit.
+                self.cleanup(run_only)
+
+            # XML error.  Just return to the GUI.
+            else:
+                return
+
+        # We already have the XML.  Just exit.
+        self.cleanup(run_only)
+
+    # ##################################################################################
     # The 'Run' program button has been pressed.  Set the run flag and close the GUI
     # ##################################################################################
-    def run_program(self) -> None:  # noqa: ANN101
+    def run_program(self) -> None:
         """
         Starts a program and displays a message box.
         Args:
             self: The class instance.
         Returns:
             None: Does not return anything.
         - Sets the go_program attribute to True to start the program
         - Displays a message box with the text "Program running..." and blocks user interaction
         - Calls the quit() method to exit the program"""
         self.go_program = True
         self.rerun = False
-        self.display_message_box("Program running...", True)
-        self.quit()
+
+        # Validate the XML and cleanup
+        self.cleanup_and_run(run_only=True)
 
     # ##################################################################################
     # The 'ReRun' program button has been pressed.  Set the run flag and close the GUI
     # ##################################################################################
-    def rerun_the_program(self) -> None:  # noqa: ANN101
+    def rerun_the_program(self) -> None:
         """
         Resets the program state and exits.
         Args:
             self: The class instance.
         Returns:
             None: Does not return anything.
         - Sets the rerun flag to True to restart the program on next run
         - Calls withdraw() to reset the program state
         - Calls quit() twice to ensure program exits"""
         self.rerun = True
-        self.withdraw()
-        self.quit()
-        self.quit()
+        self.cleanup_and_run(run_only=False)
+
+    # ##################################################################################
+    # The Upgrade Version button has been pressed.
+    # ##################################################################################
+    def upgrade_event(self) -> None:
+        """ "Runs an update and reruns the program."
+        Parameters:
+            - self (object): Instance of the class.
+        Returns:
+            - None: No return value.
+        Processing Logic:
+            - Calls the update function.
+            - Reruns the program to pick up the update."""
+        update()
+        self.display_message_box("Program updated.  Restarting...", True)
+        # Create the Change Log file to be read and displayed after a program update.
+        create_changelog()
+        do_rerun()
+
+    # ##################################################################################
+    # The Upgrade Version button has been pressed.
+    # ##################################################################################
+    def report_issue_event(self) -> None:
+        """Opens a web browser and directs the user to create a new issue on GitHub for the Map-Tasker project.
+        Parameters:
+            - self (object): The instance of the class calling the function.
+        Returns:
+            - None: This function does not return any values.
+        Processing Logic:
+            - Opens a web browser using the webbrowser module.
+            - Uses the url variable to direct the user to the correct page on GitHub.
+            - If the web browser is not supported, a message box is displayed.
+            - If the web browser is supported, a message box is displayed with instructions for creating a new issue."""
+        url = "//github.com/mctinker/Map-Tasker/issues"
+        issue_text = (
+            "Go to your browser and create a new issue or feature request, providing as much detail as possible."
+        )
+        try:
+            webbrowser.open(f"https:{PrimeItems.slash*2}{url}", new=2)
+        except webbrowser.Error:
+            self.display_message_box("Error: Failed to open output in browser: your browser is not supported.", False)
+            return
+        self.new_message_box("Report an Issue or Request a Feature\n\n" + issue_text)
 
     # ##################################################################################
     # The 'Exit' program button has been pressed.  Call it quits
     # ##################################################################################
-    def exit_program(self) -> None:  # noqa: ANN101
+    def exit_program(self) -> None:
         """
         Exits the program by setting exit flag and calling quit twice
         Args:
             self: The object instance
         Returns:
             None: Does not return anything
         - Sets the exit flag to True to indicate program exit
         - Calls quit() twice to ensure program exits cleanly
         - Calling quit() twice is done as a precaution in case one call fails to exit for some reason
         """
         self.exit = True
         self.quit()
         self.quit()
+
+    # ##################################################################################
+    # Load the XML if not already loaded.
+    # ##################################################################################
+    def load_xml(self) -> bool:
+        """Load XML from a file or URL.
+        Parameters:
+            self (Tasker): Instance of Tasker class.
+        Returns:
+            - bool: True if successful, False otherwise.
+        Processing Logic:
+            - Check if file is specified.
+            - If file is specified, read it.
+            - If file is not specified, get from URL.
+            - If file is not found, display error.
+            - If error reading file, display error.
+            - If successful, return True."""
+        if (
+            not PrimeItems.tasker_root_elements["all_projects"]
+            and not PrimeItems.tasker_root_elements["all_profiles"]
+            and not PrimeItems.tasker_root_elements["all_tasks"]
+            or self.android_ipaddr
+        ):
+            if self.android_ipaddr == "":
+                return_code = get_xml(self.debug, self.appearance_mode)
+                # Did we get an error reading the backup file?
+                if return_code > 0:
+                    if return_code == 6:
+                        self.display_message_box("Cancel button pressed.\n", False)
+                    else:
+                        self.display_multiple_messages(
+                            [f"{PrimeItems.error_msg}\n", "Click 'Reset Options' to try a different XML file."],
+                            False,
+                        )
+                    return False
+
+            # We have a file identified.  We now have to read it in.
+            else:
+                filename_location = self.android_file.rfind(PrimeItems.slash) + 1
+                file_to_use = PrimeItems.program_arguments["android_file"][filename_location:]
+                if not file_to_use:
+                    file_to_use = self.android_file[filename_location:]
+                try:
+                    PrimeItems.file_to_get = open(file_to_use)
+                except FileNotFoundError:
+                    self.display_message_box(f"XML file {file_to_use} not found.", False)
+                    return False
+
+                # Get the XML
+                PrimeItems.program_arguments["gui"] = True
+                return_code = get_the_xml_data()
+                if return_code != 0:
+                    return False
+
+        return True
+
+    # ##################################################################################
+    # Display a treeview of the XML.
+    # ##################################################################################
+    def treeview_event(self) -> None:
+        """Handles the event of clicking on the treeview.
+        Parameters:
+            - self (object): The object calling the function.
+        Returns:
+            - None: This function does not return anything.
+        Processing Logic:
+            - Checks if the XML file has already been retrieved.
+            - If not, calls the get_xml function.
+            - If there is an error reading the backup file, displays an error message.
+            - If the file has been identified, attempts to open it.
+            - If the file is not found, displays an error message.
+            - Calls the build_the_tree function to build the tree.
+            - Calls the display_tree function to display the tree."""
+        PrimeItems.error_code = 0  # Clear any previous error.
+
+        # Do we already have the XML?
+        # If we don't have any data, get it.
+        if self.load_xml():
+            # Ok, we have our root Tasker elements.  Build the tree
+            self.toplevel_window = None
+
+            # Build our tree from XML data
+            tree_data = self.build_the_tree()
+
+            # Display the tree
+            self.display_tree(tree_data)
+
+    # ##################################################################################
+    # Build a hierarchical list of all of the Tasker elements.
+    # ##################################################################################
+    def build_the_tree(self) -> list:
+        """Builds the hierarchical list of all of the Tasker elements.
+        Parameters:
+            self (object): The object calling the function.
+        Returns:
+            tree_data (list): The hierarchical list of all of the Tasker elements.
+        Processing Logic:
+            - Checks if the XML file has already been retrieved.
+            - If not, calls the get_xml function.
+            - If there is an error reading the backup file, displays an error message.
+            - If the file has been identified, attempts to open it.
+            - If the file is not found, displays an error message.
+            - Gets all of the Tasker elements.
+        """
+
+        tree_data = []
+        root = PrimeItems.tasker_root_elements
+        # Start with Projects
+        projects = root["all_projects"]
+        if projects:
+            for project in projects:
+                project_name = projects[project]["name"]
+
+                # Retrieves profile IDs for a given project and project name, excluding projects without profiles.
+                if profile_ids := get_ids(True, projects[project]["xml"], project_name, []):
+                    # Build our list of Profiles in this Project.
+                    profile_list = build_profiles(root, profile_ids)
+
+                # Project has no Profiles
+                else:
+                    profile_list = ["No Profiles Found"]
+
+                # Process Scenes
+                scene_names = None
+                with contextlib.suppress(Exception):
+                    scene_names = projects[project]["xml"].find("scenes").text
+                if scene_names is not None:
+                    scene_list = scene_names.split(",")
+                    for scene in scene_list:
+                        profile_list.append(f"Scene: {scene}")
+
+                # Put it all together: Project, Profiles, and Tasks
+                tree_data.append({"name": f"Project: {project_name}", "children": profile_list})
+
+        # Return our data tree
+        return tree_data
+
+    # ##################################################################################
+    # Display the tree view.
+    # ##################################################################################
+    def display_tree(self, tree_data: list) -> None:
+        """Displays a treeview window with given data.
+        Parameters:
+            tree_data (list): List of data to be displayed in the treeview.
+        Returns:
+            None: This function does not return anything.
+        Processing Logic:
+            - Creates a new window if one does not exist.
+            - Focuses on the window if it already exists.
+            - Displays the given data in a treeview format.
+            - Packs the treeview in the window with specified padding and filling."""
+        if tree_data:
+            if self.toplevel_window is None or not self.toplevel_window.winfo_exists():
+                self.toplevel_window = TreeviewWindow(self)  # create window if its None or destroyed
+            else:
+                self.toplevel_window.focus()  # if window exists focus it
+
+            # Display the tree in the toplevel window.
+            tree_view = CTkTreeview(master=self.toplevel_window, items=tree_data)
+            tree_view.pack(padx=10, pady=10, fill="both", expand=True)
+        else:
+            self.display_message_box("No Project(s) Found in XML!", False)
+
+
+# ##################################################################################
+# Build a list of Profiles that are under the given project
+# ##################################################################################
+def build_profiles(root: dict, profile_ids: list) -> list:
+    """Parameters:
+        - root (dict): Dictionary containing all profiles and their tasks.
+        - profile_ids (list): List of profile IDs to be processed.
+    Returns:
+        - list: List of dictionaries containing profile names and their corresponding tasks.
+    Processing Logic:
+        - Get all profiles from root dictionary.
+        - Create an empty list to store profile names and tasks.
+        - Loop through each profile ID in the provided list.
+        - Get the tasks for the current profile.
+        - If tasks are found, create a list to store task names.
+        - Loop through each task and add its name to the task list.
+        - If no tasks are found, add a default message to the task list.
+        - Get the name of the current profile.
+        - If no name is found, add a default message to the profile name.
+        - Combine the profile name and task list into a dictionary and add it to the profile list.
+        - Return the profile list."""
+    profiles = root["all_profiles"]
+    profile_list = []
+    for profile in profile_ids:
+        # Get the Profile's Tasks
+        PrimeItems.task_count_unnamed = 0  # Avoid an error in get_profile_tasks
+        if the_tasks := get_profile_tasks(profiles[profile]["xml"], [], []):
+            task_list = []
+            # Process each Task.  Tasks are simply a flat list of names.
+            for task in the_tasks:
+                if task["name"] == "":
+                    task_list.append("Task: Unnamed Task")
+                else:
+                    task_list.append(f'Task: {task["name"]}')
+        else:
+            task_list = ["No Profile Tasks Found"]
+
+        # Get the Profile name.
+        if profiles[profile]["name"] == "":
+            profile_name = "Profile: Unnamed/Anonymous"
+        else:
+            profile_name = f'Profile: {profiles[profile]["name"]}'
+
+        # Combine the Profile with it's Tasks
+        profile_list.append({"name": profile_name, "children": task_list})
+
+    return profile_list
```

### Comparing `maptasker-2.6.3/pyproject.toml` & `maptasker-3.2.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 [tool.poetry]
 name = "maptasker"
-version = "2.6.3"
+
+version = "3.2.2"
+
 description = "Utility to display your entire Android 'Tasker' configuration on your MAC."
 authors = ["Michael Rubin <mikrubin@gmail.com>"]
 readme = "README_PyPl.md"
-license = "GPL-3.0-or-later"
+license = "MIT License (MIT)"
 repository = "https://github.com/mctinker/Map-Tasker"
+# changelog = "https://github.com/mctinker/Map-Tasker/blob/Master/Changelog.md"
 keywords = ["tasker", "Tasker", "map tasker"]
 packages = [
     { include = "maptasker"}
 ]
 include = ["**/maptasker/**/*.py", "**/maptasker/assets/*.*"]
 # How to include a data directory...
 # include = ["**/maptasker/**/*.py", {path="**/clip/castles/ascii/**", format="sdist"}]
 exclude = ["run_test.py", "**/maptasker/**/backup.xml", "**/maptasker/maptasker.log", "**/maptasker/MapTasker.html", "**/maptasker/.MapTasker_RunCount.txt", "**/maptasker/.arguments.txt", "**/maptasker/**/__pycache__", "**/maptasker/**/.dep-tree.yml"]
 
 [tool.poetry.dependencies]
-python = "^3.10.13"
-customtkinter = "^5.2.1"
-ctkcolorpicker = "^0.8.0"
-pillow = "^10.1.0"
-darkdetect = "^0.8.0"
-defusedxml = "^0.7.1"
-requests = "^2.31.0"
-packaging = "^23.2"  # Needed due to bug in customtkinter
+python = "<=3.13,>=3.11"
+customtkinter = "^5.2.2"  # GUI
+ctkcolorpicker = "^0.9.0"  # Color picker in GUI
+pillow = "^10.3.0"  # Image support in GUI
+darkdetect = "^0.8.0"  # Appearance mode detection
+defusedxml = "^0.7.1"  # More secure xml parser
+requests = "^2.31.0"  # HTTP Server function request
+tomli_w = "^1.0.0"  # Write toml file
 
 [tool.poetry.scripts]
 maptasker = "maptasker.main:main"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/mctinker/Map-Tasker/issues"
 "Change Log" = "https://github.com/mctinker/Map-Tasker/CHANGELOG.md"
@@ -40,14 +43,15 @@
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "primary"
 
 [tool.ruff]
 line-length = 120
 respect-gitignore = true
+# editor.formatOnSaveMode = "modificationsIfAvailable"
 select = [
     'A',    # Builtins
     'ANN',  # Annotations
     'ARG',  # Unused arguments
     'B',    # Bugbear
     'BLE',  # Blind except
     'C4',   # Comprehensions
@@ -120,14 +124,16 @@
     "README.md",
 ]
 ignore = [
     "PLR2004",  # Constant value comparison
     "SIM115",   # Missing "with" on oepn file
     "S606",     # No shell
     "B009",     # Do not perform function calls in argument defaults
+    "T201",     # Print found
+    "ANN101",   # Missing type annotation for self
     ]
 show-fixes = true
 src = ['src',]
 
 [tool.ruff.pycodestyle]
 ignore-overlong-task-comments = true
 
@@ -156,20 +162,27 @@
 [tool.ruff.format]
 quote-style = "double"
 # indent-style = "tab"
 docstring-code-format = true
 
 [tool.black]
 --line-length = 120
+line-length = 120
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 pythonpath = [
   "."
 ]
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.2"
 pytest-mock = "*"
+
+# Bump version identifiers.  Repeat this chunk for each file.
+[[tool.poetry_bumpversion.replacements]]
+files = ["maptasker/src/sysconst.py"]
+search = 'VERSION = "{current_version}"'
+replace = 'VERSION = "{new_version}"'
```

### Comparing `maptasker-2.6.3/PKG-INFO` & `maptasker-3.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: maptasker
-Version: 2.6.3
+Version: 3.2.2
 Summary: Utility to display your entire Android 'Tasker' configuration on your MAC.
 Home-page: https://github.com/mctinker/Map-Tasker
-License: GPL-3.0-or-later
+License: MIT License (MIT)
 Keywords: tasker,Tasker,map tasker
 Author: Michael Rubin
 Author-email: mikrubin@gmail.com
-Requires-Python: >=3.10.13,<4.0.0
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Requires-Python: >=3.11,<=3.13
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: ctkcolorpicker (>=0.8.0,<0.9.0)
-Requires-Dist: customtkinter (>=5.2.1,<6.0.0)
+Requires-Dist: ctkcolorpicker (>=0.9.0,<0.10.0)
+Requires-Dist: customtkinter (>=5.2.2,<6.0.0)
 Requires-Dist: darkdetect (>=0.8.0,<0.9.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
-Requires-Dist: packaging (>=23.2,<24.0)
-Requires-Dist: pillow (>=10.1.0,<11.0.0)
+Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: tomli_w (>=1.0.0,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/mctinker/Map-Tasker/issues
 Project-URL: Change Log, https://github.com/mctinker/Map-Tasker/CHANGELOG.md
 Project-URL: Repository, https://github.com/mctinker/Map-Tasker
 Description-Content-Type: text/markdown
 
 # MapTasker
-## Display the Tasker Project/Profile/Task/Scene hierarchy on a MAC based on Tasker's backup file (backup.xml)
 
-This is an application in support of [Tasker](https://tasker.joaoapps.com/) that is intended to run on a MAC.
- 
-For further details: https://github.com/mctinker/Map-Tasker
+## Display the Tasker Project/Profile/Task/Scene hierarchy on a MAC/PC/Linux desktop based on Tasker's backup or exported XML file (e.g. backup.xml)
+
+This is an application in support of [Tasker](https://tasker.joaoapps.com/) that is intended to run on a MAC/PC/Linux desktop.
+
+An older version, which requires Python version 3.10 rather than 3.11 or higher, is available as version 2.6.3...
+    `pip install maptasker==2.6.3`
+
+For further details, refer to [the project on Github.](https://github.com/mctinker/Map-Tasker)
```


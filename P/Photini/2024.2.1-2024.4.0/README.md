# Comparing `tmp/Photini-2024.2.1.tar.gz` & `tmp/Photini-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jim/Documents/projects/Photini/main/dist/tmp9yyaajc_/Photini-2024.2.1.tar", last modified: Sat Feb 17 12:11:39 2024, max compression
+gzip compressed data, was "/home/jim/Documents/projects/Photini/main/dist/tmp8t4cthkf/Photini-2024.4.0.tar", last modified: Thu Apr 25 08:47:45 2024, max compression
```

## Comparing `Photini-2024.2.1.tar` & `Photini-2024.4.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-02-17 12:11:39.000000 Photini-2024.2.1/
--rw-r--r--   0 jim       (1026) users      (100)    16867 2024-02-17 12:07:53.000000 Photini-2024.2.1/CHANGELOG.txt
--rw-r--r--   0 jim       (1026) users      (100)    35147 2023-09-11 09:27:18.000000 Photini-2024.2.1/LICENSE.txt
--rw-r--r--   0 jim       (1026) users      (100)      529 2023-09-11 09:27:18.000000 Photini-2024.2.1/MANIFEST.in
--rw-r--r--   0 jim       (1026) users      (100)     8853 2024-02-17 12:11:39.000000 Photini-2024.2.1/PKG-INFO
--rw-r--r--   0 jim       (1026) users      (100)     7756 2024-02-01 09:20:49.000000 Photini-2024.2.1/README.rst
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-02-17 12:11:39.000000 Photini-2024.2.1/custom_build/
--rw-r--r--   0 jim       (1026) users      (100)     2294 2023-09-11 09:27:18.000000 Photini-2024.2.1/custom_build/backend.py
--rw-r--r--   0 jim       (1026) users      (100)     3662 2024-02-17 12:07:53.000000 Photini-2024.2.1/pyproject.toml
--rw-r--r--   0 jim       (1026) users      (100)       38 2024-02-17 12:11:39.000000 Photini-2024.2.1/setup.cfg
--rw-r--r--   0 jim       (1026) users      (100)     2562 2024-02-01 09:20:49.000000 Photini-2024.2.1/setup.py
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-02-17 12:11:39.000000 Photini-2024.2.1/src/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-02-17 12:11:39.000000 Photini-2024.2.1/src/Photini.egg-info/
--rw-r--r--   0 jim       (1026) users      (100)     1746 2024-02-17 12:11:39.000000 Photini-2024.2.1/src/Photini.egg-info/SOURCES.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-02-17 12:11:39.000000 Photini-2024.2.1/src/photini/
--rw-r--r--   0 jim       (1026) users      (100)     1048 2024-02-01 09:20:49.000000 Photini-2024.2.1/src/photini/__init__.py
--rw-r--r--   0 jim       (1026) users      (100)      917 2023-09-11 09:27:18.000000 Photini-2024.2.1/src/photini/__main__.py
--rw-r--r--   0 jim       (1026) users      (100)      148 2024-02-17 12:11:38.000000 Photini-2024.2.1/src/photini/_version.py
--rw-r--r--   0 jim       (1026) users      (100)    19671 2024-02-17 12:07:53.000000 Photini-2024.2.1/src/photini/address.py
--rw-r--r--   0 jim       (1026) users      (100)     4704 2024-02-01 09:20:49.000000 Photini-2024.2.1/src/photini/bingmap.py
--rw-r--r--   0 jim       (1026) users      (100)     5060 2024-02-01 09:20:49.000000 Photini-2024.2.1/src/photini/configstore.py
--rw-r--r--   0 jim       (1026) users      (100)     6890 2023-09-11 09:27:18.000000 Photini-2024.2.1/src/photini/cv.py
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-02-17 12:11:39.000000 Photini-2024.2.1/src/photini/data/
--rw-r--r--   0 jim       (1026) users      (100)    35147 2023-09-11 09:27:18.000000 Photini-2024.2.1/src/photini/data/LICENSE.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-02-17 12:11:39.000000 Photini-2024.2.1/src/photini/data/icons/
--rw-r--r--   0 jim       (1026) users      (100)    14554 2023-09-11 09:27:18.000000 Photini-2024.2.1/src/photini/data/icons/photini_128.png
--rw-r--r--   0 jim       (1026) users      (100)     3262 2023-09-11 09:27:18.000000 Photini-2024.2.1/src/photini/data/icons/photini_48.png
--rw-r--r--   0 jim       (1026) users      (100)    86598 2023-09-11 09:27:18.000000 Photini-2024.2.1/src/photini/data/icons/photini_win.ico
--rw-r--r--   0 jim       (1026) users      (100)     2205 2023-09-11 09:44:02.000000 Photini-2024.2.1/src/photini/data/keys.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-02-17 12:11:39.000000 Photini-2024.2.1/src/photini/data/lang/
--rw-r--r--   0 jim       (1026) users      (100)    22126 2024-02-17 12:11:38.000000 Photini-2024.2.1/src/photini/data/lang/photini.ca.qm
--rw-r--r--   0 jim       (1026) users      (100)    32936 2024-02-17 12:11:38.000000 Photini-2024.2.1/src/photini/data/lang/photini.cs.qm
--rw-r--r--   0 jim       (1026) users      (100)    47788 2024-02-17 12:11:38.000000 Photini-2024.2.1/src/photini/data/lang/photini.de.qm
--rw-r--r--   0 jim       (1026) users      (100)    29055 2024-02-17 12:11:38.000000 Photini-2024.2.1/src/photini/data/lang/photini.en.qm
--rw-r--r--   0 jim       (1026) users      (100)    55444 2024-02-17 12:11:38.000000 Photini-2024.2.1/src/photini/data/lang/photini.es.qm
--rw-r--r--   0 jim       (1026) users      (100)    43003 2024-02-17 12:11:38.000000 Photini-2024.2.1/src/photini/data/lang/photini.fr.qm
--rw-r--r--   0 jim       (1026) users      (100)    55640 2024-02-17 12:11:38.000000 Photini-2024.2.1/src/photini/data/lang/photini.it.qm
--rw-r--r--   0 jim       (1026) users      (100)     2026 2024-02-17 12:11:38.000000 Photini-2024.2.1/src/photini/data/lang/photini.ko.qm
--rw-r--r--   0 jim       (1026) users      (100)    21271 2024-02-17 12:11:38.000000 Photini-2024.2.1/src/photini/data/lang/photini.nb.qm
--rw-r--r--   0 jim       (1026) users      (100)    14017 2024-02-17 12:11:38.000000 Photini-2024.2.1/src/photini/data/lang/photini.pl.qm
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-02-17 12:11:39.000000 Photini-2024.2.1/src/photini/data/linux/
--rw-r--r--   0 jim       (1026) users      (100)      321 2023-09-11 09:27:18.000000 Photini-2024.2.1/src/photini/data/linux/photini.desktop
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-02-17 12:11:39.000000 Photini-2024.2.1/src/photini/data/map/
--rw-r--r--   0 jim       (1026) users      (100)     7400 2024-02-01 09:20:49.000000 Photini-2024.2.1/src/photini/data/map/bingmap.js
--rw-r--r--   0 jim       (1026) users      (100)      209 2023-09-11 09:27:18.000000 Photini-2024.2.1/src/photini/data/map/circle_blue.png
--rw-r--r--   0 jim       (1026) users      (100)      207 2023-09-11 09:27:18.000000 Photini-2024.2.1/src/photini/data/map/circle_red.png
--rw-r--r--   0 jim       (1026) users      (100)     6212 2024-02-01 09:20:49.000000 Photini-2024.2.1/src/photini/data/map/googlemap.js
--rw-r--r--   0 jim       (1026) users      (100)     5687 2024-02-01 09:20:49.000000 Photini-2024.2.1/src/photini/data/map/mapboxmap.js
--rw-r--r--   0 jim       (1026) users      (100)     1867 2023-09-11 09:27:18.000000 Photini-2024.2.1/src/photini/data/map/pin_grey.png
--rw-r--r--   0 jim       (1026) users      (100)     2016 2023-09-11 09:27:18.000000 Photini-2024.2.1/src/photini/data/map/pin_red.png
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-02-17 12:11:39.000000 Photini-2024.2.1/src/photini/data/windows/
--rw-r--r--   0 jim       (1026) users      (100)     2638 2023-09-11 09:27:18.000000 Photini-2024.2.1/src/photini/data/windows/install_shortcuts.vbs
--rw-r--r--   0 jim       (1026) users      (100)    13496 2023-09-11 09:44:02.000000 Photini-2024.2.1/src/photini/descriptive.py
--rw-r--r--   0 jim       (1026) users      (100)    23113 2024-02-01 09:20:49.000000 Photini-2024.2.1/src/photini/editor.py
--rw-r--r--   0 jim       (1026) users      (100)     8435 2023-09-11 09:27:18.000000 Photini-2024.2.1/src/photini/editsettings.py
--rw-r--r--   0 jim       (1026) users      (100)    34091 2024-02-01 09:20:49.000000 Photini-2024.2.1/src/photini/exiv2.py
--rw-r--r--   0 jim       (1026) users      (100)     3287 2023-09-11 09:27:18.000000 Photini-2024.2.1/src/photini/ffmpeg.py
--rw-r--r--   0 jim       (1026) users      (100)    33323 2023-09-11 09:44:02.000000 Photini-2024.2.1/src/photini/flickr.py
--rw-r--r--   0 jim       (1026) users      (100)     4177 2024-02-01 09:20:49.000000 Photini-2024.2.1/src/photini/googlemap.py
--rw-r--r--   0 jim       (1026) users      (100)    13099 2023-09-11 09:27:18.000000 Photini-2024.2.1/src/photini/googlephotos.py
--rw-r--r--   0 jim       (1026) users      (100)     4504 2023-09-11 09:44:02.000000 Photini-2024.2.1/src/photini/gpximporter.py
--rw-r--r--   0 jim       (1026) users      (100)    40641 2023-09-11 09:44:02.000000 Photini-2024.2.1/src/photini/imagelist.py
--rw-r--r--   0 jim       (1026) users      (100)    27950 2023-09-11 09:44:02.000000 Photini-2024.2.1/src/photini/importer.py
--rw-r--r--   0 jim       (1026) users      (100)    27318 2024-02-01 09:20:49.000000 Photini-2024.2.1/src/photini/ipernity.py
--rw-r--r--   0 jim       (1026) users      (100)     5404 2024-02-01 09:20:49.000000 Photini-2024.2.1/src/photini/loggerwindow.py
--rw-r--r--   0 jim       (1026) users      (100)     4228 2024-02-01 09:20:49.000000 Photini-2024.2.1/src/photini/mapboxmap.py
--rw-r--r--   0 jim       (1026) users      (100)    38889 2024-02-01 09:20:49.000000 Photini-2024.2.1/src/photini/metadata.py
--rw-r--r--   0 jim       (1026) users      (100)    21920 2023-09-11 09:27:18.000000 Photini-2024.2.1/src/photini/ownership.py
--rw-r--r--   0 jim       (1026) users      (100)    25878 2024-02-01 09:20:49.000000 Photini-2024.2.1/src/photini/photinimap.py
--rw-r--r--   0 jim       (1026) users      (100)    37798 2023-09-11 09:44:02.000000 Photini-2024.2.1/src/photini/pixelfed.py
--rw-r--r--   0 jim       (1026) users      (100)    10708 2023-09-11 09:27:18.000000 Photini-2024.2.1/src/photini/pyqt.py
--rw-r--r--   0 jim       (1026) users      (100)    37814 2024-02-01 09:20:49.000000 Photini-2024.2.1/src/photini/regions.py
--rw-r--r--   0 jim       (1026) users      (100)     7756 2024-02-01 09:20:49.000000 Photini-2024.2.1/src/photini/scripts.py
--rw-r--r--   0 jim       (1026) users      (100)     3687 2023-09-11 09:27:18.000000 Photini-2024.2.1/src/photini/spelling.py
--rw-r--r--   0 jim       (1026) users      (100)    40941 2024-02-01 09:20:49.000000 Photini-2024.2.1/src/photini/technical.py
--rw-r--r--   0 jim       (1026) users      (100)    72730 2024-02-17 12:07:53.000000 Photini-2024.2.1/src/photini/types.py
--rw-r--r--   0 jim       (1026) users      (100)    47570 2024-02-01 09:20:49.000000 Photini-2024.2.1/src/photini/uploader.py
--rw-r--r--   0 jim       (1026) users      (100)    36486 2024-02-01 09:20:49.000000 Photini-2024.2.1/src/photini/widgets.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/
+-rw-r--r--   0 jim       (1026) users      (100)    17042 2024-04-25 08:46:39.000000 Photini-2024.4.0/CHANGELOG.txt
+-rw-r--r--   0 jim       (1026) users      (100)    35147 2023-09-11 09:27:18.000000 Photini-2024.4.0/LICENSE.txt
+-rw-r--r--   0 jim       (1026) users      (100)      529 2023-09-11 09:27:18.000000 Photini-2024.4.0/MANIFEST.in
+-rw-r--r--   0 jim       (1026) users      (100)     9342 2024-04-25 08:47:45.000000 Photini-2024.4.0/PKG-INFO
+-rw-r--r--   0 jim       (1026) users      (100)     8245 2024-04-25 08:46:39.000000 Photini-2024.4.0/README.rst
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/custom_build/
+-rw-r--r--   0 jim       (1026) users      (100)     2294 2023-09-11 09:27:18.000000 Photini-2024.4.0/custom_build/backend.py
+-rw-r--r--   0 jim       (1026) users      (100)     3659 2024-04-25 08:46:39.000000 Photini-2024.4.0/pyproject.toml
+-rw-r--r--   0 jim       (1026) users      (100)       38 2024-04-25 08:47:45.000000 Photini-2024.4.0/setup.cfg
+-rw-r--r--   0 jim       (1026) users      (100)     2562 2024-02-01 09:20:49.000000 Photini-2024.4.0/setup.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/src/
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/src/Photini.egg-info/
+-rw-r--r--   0 jim       (1026) users      (100)     1746 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/Photini.egg-info/SOURCES.txt
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/src/photini/
+-rw-r--r--   0 jim       (1026) users      (100)     1048 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/__init__.py
+-rw-r--r--   0 jim       (1026) users      (100)      917 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/__main__.py
+-rw-r--r--   0 jim       (1026) users      (100)      148 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/_version.py
+-rw-r--r--   0 jim       (1026) users      (100)    19671 2024-02-17 12:07:53.000000 Photini-2024.4.0/src/photini/address.py
+-rw-r--r--   0 jim       (1026) users      (100)     4704 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/bingmap.py
+-rw-r--r--   0 jim       (1026) users      (100)     5060 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/configstore.py
+-rw-r--r--   0 jim       (1026) users      (100)     6890 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/cv.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/src/photini/data/
+-rw-r--r--   0 jim       (1026) users      (100)    35147 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/data/LICENSE.txt
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/src/photini/data/icons/
+-rw-r--r--   0 jim       (1026) users      (100)    14554 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/data/icons/photini_128.png
+-rw-r--r--   0 jim       (1026) users      (100)     3262 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/data/icons/photini_48.png
+-rw-r--r--   0 jim       (1026) users      (100)    86598 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/data/icons/photini_win.ico
+-rw-r--r--   0 jim       (1026) users      (100)     2205 2024-04-25 08:46:39.000000 Photini-2024.4.0/src/photini/data/keys.txt
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/src/photini/data/lang/
+-rw-r--r--   0 jim       (1026) users      (100)    22126 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/data/lang/photini.ca.qm
+-rw-r--r--   0 jim       (1026) users      (100)    32936 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/data/lang/photini.cs.qm
+-rw-r--r--   0 jim       (1026) users      (100)    47788 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/data/lang/photini.de.qm
+-rw-r--r--   0 jim       (1026) users      (100)    51535 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/data/lang/photini.en.qm
+-rw-r--r--   0 jim       (1026) users      (100)    55444 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/data/lang/photini.es.qm
+-rw-r--r--   0 jim       (1026) users      (100)    43003 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/data/lang/photini.fr.qm
+-rw-r--r--   0 jim       (1026) users      (100)    55640 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/data/lang/photini.it.qm
+-rw-r--r--   0 jim       (1026) users      (100)     2026 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/data/lang/photini.ko.qm
+-rw-r--r--   0 jim       (1026) users      (100)    21271 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/data/lang/photini.nb.qm
+-rw-r--r--   0 jim       (1026) users      (100)    14017 2024-04-25 08:47:44.000000 Photini-2024.4.0/src/photini/data/lang/photini.pl.qm
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/src/photini/data/linux/
+-rw-r--r--   0 jim       (1026) users      (100)      321 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/data/linux/photini.desktop
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/src/photini/data/map/
+-rw-r--r--   0 jim       (1026) users      (100)     7400 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/data/map/bingmap.js
+-rw-r--r--   0 jim       (1026) users      (100)      209 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/data/map/circle_blue.png
+-rw-r--r--   0 jim       (1026) users      (100)      207 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/data/map/circle_red.png
+-rw-r--r--   0 jim       (1026) users      (100)     6186 2024-04-25 08:46:39.000000 Photini-2024.4.0/src/photini/data/map/googlemap.js
+-rw-r--r--   0 jim       (1026) users      (100)     5687 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/data/map/mapboxmap.js
+-rw-r--r--   0 jim       (1026) users      (100)     1867 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/data/map/pin_grey.png
+-rw-r--r--   0 jim       (1026) users      (100)     2016 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/data/map/pin_red.png
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2024-04-25 08:47:45.000000 Photini-2024.4.0/src/photini/data/windows/
+-rw-r--r--   0 jim       (1026) users      (100)     2638 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/data/windows/install_shortcuts.vbs
+-rw-r--r--   0 jim       (1026) users      (100)    13496 2023-09-11 09:44:02.000000 Photini-2024.4.0/src/photini/descriptive.py
+-rw-r--r--   0 jim       (1026) users      (100)    23113 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/editor.py
+-rw-r--r--   0 jim       (1026) users      (100)     8435 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/editsettings.py
+-rw-r--r--   0 jim       (1026) users      (100)    34091 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/exiv2.py
+-rw-r--r--   0 jim       (1026) users      (100)     3287 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/ffmpeg.py
+-rw-r--r--   0 jim       (1026) users      (100)    33323 2023-09-11 09:44:02.000000 Photini-2024.4.0/src/photini/flickr.py
+-rw-r--r--   0 jim       (1026) users      (100)     4264 2024-04-25 08:46:39.000000 Photini-2024.4.0/src/photini/googlemap.py
+-rw-r--r--   0 jim       (1026) users      (100)    13099 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/googlephotos.py
+-rw-r--r--   0 jim       (1026) users      (100)     4504 2023-09-11 09:44:02.000000 Photini-2024.4.0/src/photini/gpximporter.py
+-rw-r--r--   0 jim       (1026) users      (100)    40589 2024-04-25 08:46:39.000000 Photini-2024.4.0/src/photini/imagelist.py
+-rw-r--r--   0 jim       (1026) users      (100)    27950 2023-09-11 09:44:02.000000 Photini-2024.4.0/src/photini/importer.py
+-rw-r--r--   0 jim       (1026) users      (100)    27318 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/ipernity.py
+-rw-r--r--   0 jim       (1026) users      (100)     5491 2024-04-25 08:46:39.000000 Photini-2024.4.0/src/photini/loggerwindow.py
+-rw-r--r--   0 jim       (1026) users      (100)     4228 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/mapboxmap.py
+-rw-r--r--   0 jim       (1026) users      (100)    38967 2024-04-25 08:46:39.000000 Photini-2024.4.0/src/photini/metadata.py
+-rw-r--r--   0 jim       (1026) users      (100)    21920 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/ownership.py
+-rw-r--r--   0 jim       (1026) users      (100)    25878 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/photinimap.py
+-rw-r--r--   0 jim       (1026) users      (100)    37798 2023-09-11 09:44:02.000000 Photini-2024.4.0/src/photini/pixelfed.py
+-rw-r--r--   0 jim       (1026) users      (100)    10708 2023-09-11 09:27:18.000000 Photini-2024.4.0/src/photini/pyqt.py
+-rw-r--r--   0 jim       (1026) users      (100)    37963 2024-04-25 08:46:39.000000 Photini-2024.4.0/src/photini/regions.py
+-rw-r--r--   0 jim       (1026) users      (100)     7689 2024-04-25 08:46:39.000000 Photini-2024.4.0/src/photini/scripts.py
+-rw-r--r--   0 jim       (1026) users      (100)     3869 2024-04-25 08:46:39.000000 Photini-2024.4.0/src/photini/spelling.py
+-rw-r--r--   0 jim       (1026) users      (100)    40941 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/technical.py
+-rw-r--r--   0 jim       (1026) users      (100)    72730 2024-02-17 12:07:53.000000 Photini-2024.4.0/src/photini/types.py
+-rw-r--r--   0 jim       (1026) users      (100)    46234 2024-04-25 08:46:39.000000 Photini-2024.4.0/src/photini/uploader.py
+-rw-r--r--   0 jim       (1026) users      (100)    36486 2024-02-01 09:20:49.000000 Photini-2024.4.0/src/photini/widgets.py
```

### Comparing `Photini-2024.2.1/CHANGELOG.txt` & `Photini-2024.4.0/CHANGELOG.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see
 <http://www.gnu.org/licenses/>.
 
+Changes in v2024.4.0:
+  1/ Google Map no longer used deprecated marker.
+  2/ Improved handling of multiple language configurations.
+  3/ Pillow is now a required dependency.
+
 Changes in v2024.2.1:
   1/ Fix bug in LangAlt values without a default language.
   2/ Possibly fix NSRangeException on MacOS ARM computers.
   3/ Ignore '_normalized_city' address component.
 
 Changes in v2024.2.0:
   1/ Improved lens model recognition.
```

### Comparing `Photini-2024.2.1/LICENSE.txt` & `Photini-2024.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/MANIFEST.in` & `Photini-2024.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/PKG-INFO` & `Photini-2024.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Photini
-Version: 2024.2.1
+Version: 2024.4.0
 Summary: Simple photo metadata editor
 Home-page: https://github.com/jim-easterbrook/Photini
 Author: Jim Easterbrook
 Author-email: jim@jim-easterbrook.me.uk
 License: GPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -106,14 +106,19 @@
 Getting help
 ------------
 
 If you encounter any problems installing or running Photini, please email jim@jim-easterbrook.me.uk and I'll respond as soon as I can.
 There is also an email list or forum for discussions about Photini at https://groups.google.com/forum/#!forum/photini.
 If you discover a bug and have a GitHub account then please file a bug report on the GitHub `"issues" page`_.
 
+If you find a problem with a particular image file then it would be useful for me to have a copy of its metadata.
+You can use the exiv2_ command line program to extract the raw metadata so you don't need to send me the entire image file.
+For example, the command ``exiv2 ex problem_file.jpg`` can reduce a 3 MByte image file to a 20 kByte file called ``problem_file.exv``.
+I promise not to publish or redistribute any file you send me.
+
 Localisation
 ------------
 
 Work has begun on providing Photini in multiple languages.
 I rely on users to do the translation, as I am not fluent in any language other than English.
 The project uses an online translation service called Weblate_.
 If you'd like to help translate Photini, please join the `Photini team on Hosted Weblate`_.
@@ -177,14 +182,15 @@
 ^^^^^^^^^^^^^^^^^^^^^
 
 Permission is granted to copy, distribute and/or modify the Photini documentation under the terms of the GNU Free Documentation License, Version 1.3 or any later version published by the Free Software Foundation; with no Invariant Sections, no Front-Cover Texts, and no Back-Cover Texts.
 A copy of the license is included in the documentation section entitled "GNU Free Documentation License".
 
 .. _blog post:
       https://www.jim-easterbrook.me.uk/2012/10/photini-whats-in-a-name/
+.. _exiv2:         https://exiv2.org/manpage.html
 .. _Flickr:        http://www.flickr.com/
 .. _Google Photos: https://photos.google.com/
 .. _Google Maps Terms of Use:
       http://www.google.com/help/terms_maps.html
 .. _Google Privacy Policy:
       http://www.google.com/policies/privacy/
 .. _installation documentation:
```

### Comparing `Photini-2024.2.1/README.rst` & `Photini-2024.4.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -71,14 +71,19 @@
 Getting help
 ------------
 
 If you encounter any problems installing or running Photini, please email jim@jim-easterbrook.me.uk and I'll respond as soon as I can.
 There is also an email list or forum for discussions about Photini at https://groups.google.com/forum/#!forum/photini.
 If you discover a bug and have a GitHub account then please file a bug report on the GitHub `"issues" page`_.
 
+If you find a problem with a particular image file then it would be useful for me to have a copy of its metadata.
+You can use the exiv2_ command line program to extract the raw metadata so you don't need to send me the entire image file.
+For example, the command ``exiv2 ex problem_file.jpg`` can reduce a 3 MByte image file to a 20 kByte file called ``problem_file.exv``.
+I promise not to publish or redistribute any file you send me.
+
 Localisation
 ------------
 
 Work has begun on providing Photini in multiple languages.
 I rely on users to do the translation, as I am not fluent in any language other than English.
 The project uses an online translation service called Weblate_.
 If you'd like to help translate Photini, please join the `Photini team on Hosted Weblate`_.
@@ -142,14 +147,15 @@
 ^^^^^^^^^^^^^^^^^^^^^
 
 Permission is granted to copy, distribute and/or modify the Photini documentation under the terms of the GNU Free Documentation License, Version 1.3 or any later version published by the Free Software Foundation; with no Invariant Sections, no Front-Cover Texts, and no Back-Cover Texts.
 A copy of the license is included in the documentation section entitled "GNU Free Documentation License".
 
 .. _blog post:
       https://www.jim-easterbrook.me.uk/2012/10/photini-whats-in-a-name/
+.. _exiv2:         https://exiv2.org/manpage.html
 .. _Flickr:        http://www.flickr.com/
 .. _Google Photos: https://photos.google.com/
 .. _Google Maps Terms of Use:
       http://www.google.com/help/terms_maps.html
 .. _Google Privacy Policy:
       http://www.google.com/policies/privacy/
 .. _installation documentation:
```

### Comparing `Photini-2024.2.1/custom_build/backend.py` & `Photini-2024.4.0/custom_build/backend.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/pyproject.toml` & `Photini-2024.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -41,28 +41,29 @@
 ]
 dependencies = [
   "appdirs >= 1.3",
   "cachetools >= 3.0",
   "chardet >= 3.0",
   "exiv2 >= 0.16",
   "filetype >= 1.0",
+  "Pillow >= 2.0",
   "requests >= 2.4",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 flickr = ["photini[keyring,requests-oauthlib,requests-toolbelt]"]
 google = ["photini[keyring,requests-oauthlib]"]
 importer = ["gphoto2 >= 1.8; platform_system != 'Windows'"]
 ipernity = ["photini[keyring,requests-toolbelt]"]
 pixelfed = ["photini[keyring,requests-oauthlib,requests-toolbelt]"]
 spelling = ["pyenchant >= 2.0"]
 # install everything except the Qt package
 all = ["""photini[keyring,requests-oauthlib,requests-toolbelt,\
-importer,spelling,gpxpy,Pillow]"""]
+importer,spelling,gpxpy]"""]
 # set versions of common packages
 keyring = ["keyring >= 7.0"]
 requests-oauthlib = ["requests-oauthlib >= 1.0"]
 requests-toolbelt = ["requests-toolbelt >= 0.9"]
 # the following are intended for use by the photini-configure script
 PyQt5 = ["PyQt5 >= 5.9", "PyQtWebEngine >= 5.12"]
 PyQt6 = ["PyQt6 >= 6.2", "PyQt6-WebEngine >= 6.2",
@@ -72,15 +73,15 @@
   "PyQt6-WebEngine-Qt6 != 6.6.1; sys_platform == 'darwin'"
 ]
 PySide2 = ["PySide2 >= 5.11"]
 PySide6 = ["PySide6 >= 6.2",
   "PySide6 != 6.6.1; sys_platform == 'darwin'"
 ]
 gpxpy = ["gpxpy >= 1.3.5, != 1.6.0"]
-Pillow = ["Pillow >= 2.0"]
+Pillow = []
 
 [project.urls]
 homepage = "https://github.com/jim-easterbrook/Photini"
 documentation = "https://photini.readthedocs.io/"
 repository = "https://github.com/jim-easterbrook/Photini"
 changelog = "https://github.com/jim-easterbrook/Photini/blob/main/CHANGELOG.txt"
```

### Comparing `Photini-2024.2.1/setup.py` & `Photini-2024.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/Photini.egg-info/SOURCES.txt` & `Photini-2024.4.0/src/Photini.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/__init__.py` & `Photini-2024.4.0/src/photini/__init__.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/__main__.py` & `Photini-2024.4.0/src/photini/__main__.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/address.py` & `Photini-2024.4.0/src/photini/address.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/bingmap.py` & `Photini-2024.4.0/src/photini/bingmap.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/configstore.py` & `Photini-2024.4.0/src/photini/configstore.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/cv.py` & `Photini-2024.4.0/src/photini/cv.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/data/LICENSE.txt` & `Photini-2024.4.0/src/photini/data/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/data/icons/photini_128.png` & `Photini-2024.4.0/src/photini/data/icons/photini_128.png`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/data/icons/photini_48.png` & `Photini-2024.4.0/src/photini/data/icons/photini_48.png`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/data/icons/photini_win.ico` & `Photini-2024.4.0/src/photini/data/icons/photini_win.ico`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/data/keys.txt` & `Photini-2024.4.0/src/photini/data/keys.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  Photini - a simple photo metadata editor.
 #  http://github.com/jim-easterbrook/Photini
-#  Copyright (C) 2015-23  Jim Easterbrook  jim@jim-easterbrook.me.uk
+#  Copyright (C) 2015-24  Jim Easterbrook  jim@jim-easterbrook.me.uk
 #
 #  This program is free software: you can redistribute it and/or
 #  modify it under the terms of the GNU General Public License as
 #  published by the Free Software Foundation, either version 3 of the
 #  License, or (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
@@ -25,24 +25,24 @@
 api_secret = ZGU2NmVlYWEwZDdjODY4Nw==
 
 [googlephotos]
 client_id = OTkxMTQ2MzkyMzc1LWdyOXRjcTc1NWZvbXRqNGUxazQ5NzNmM2FjbWlvN29tLmFwcHMuZ29vZ2xldXNlcmNvbnRlbnQuY29t
 client_secret = dnkwV3UtYWVmMmlYeTJXZ2lVaUZDOFlB
 
 [googlemap]
-api_key = QUl6YVN5RFlfLW5OWnVTOWlYaF81cFJmd2s0QnhRQnZQbU1xUGVB
+api_key = QUl6YVN5Q0NCQkVBenhmS0pwSjJGaTNwNFZ0TzA0OS14S0FkeGk4
 
 [bingmap]
-api_key = QXJrdkh0eHhrU29kVnRndzdiV2ZlYUh0ZXVUNzZObHRpZ2d6cS1Ba3RiQm04b0prLWxxTE9sZTZMQUJlY09YXw==
+api_key = QXFMRjRjcDc3N3IzZVVPNFFQT28zWU9mMV9Ta2hHWEV5ajdlWmZBOEtBclBlaEJLZFlJNHlWQWR5cC1pTXV1bg==
 
 [opencage]
 api_key = YWE3YjIwMTE3ZTBkNGE4NDk4NzQzMTc3MTI0NmY1NjU=
 
 [mapboxmap]
-api_key = cGsuZXlKMUlqb2lhbWx0TFdWaGMzUmxjbUp5YjI5cklpd2lZU0k2SW1Oc2JHOTFabTFwT1RBd2VEQXpabkEwT1hweGNIazBlVEVpZlEuSWxhZTdQWnVaQ2E2OG5TTjBUTHdRdw==
+api_key = cGsuZXlKMUlqb2lhbWx0TFdWaGMzUmxjbUp5YjI5cklpd2lZU0k2SW1Oc2RUbHJlV001TmpCaVl6SXliWEZyT1RkdVpXcDBiSG9pZlEuWXgxc1RtVmtKWHlDTzlONkZzc2pCdw==
 
 [pixelfed pixelfed.de]
 client_id = NDIyNjQ=
 client_secret = NWI0a0tLMGRmTm9YYUtKdUw2QWJPNFZmeG5Qd1FJeU9nclhjZlpweQ==
 
 [pixelfed pxlmo.com]
 client_id = MTY1MQ==
```

### Comparing `Photini-2024.2.1/src/photini/data/lang/photini.ca.qm` & `Photini-2024.4.0/src/photini/data/lang/photini.ca.qm`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/data/lang/photini.cs.qm` & `Photini-2024.4.0/src/photini/data/lang/photini.cs.qm`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/data/lang/photini.de.qm` & `Photini-2024.4.0/src/photini/data/lang/photini.de.qm`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/data/lang/photini.es.qm` & `Photini-2024.4.0/src/photini/data/lang/photini.es.qm`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/data/lang/photini.fr.qm` & `Photini-2024.4.0/src/photini/data/lang/photini.fr.qm`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/data/lang/photini.it.qm` & `Photini-2024.4.0/src/photini/data/lang/photini.it.qm`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/data/lang/photini.ko.qm` & `Photini-2024.4.0/src/photini/data/lang/photini.ko.qm`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/data/lang/photini.nb.qm` & `Photini-2024.4.0/src/photini/data/lang/photini.nb.qm`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/data/lang/photini.pl.qm` & `Photini-2024.4.0/src/photini/data/lang/photini.pl.qm`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/data/map/bingmap.js` & `Photini-2024.4.0/src/photini/data/map/bingmap.js`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/data/map/googlemap.js` & `Photini-2024.4.0/src/photini/data/map/mapboxmap.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 //  Photini - a simple photo metadata editor.
 //  http://github.com/jim-easterbrook/Photini
-//  Copyright (C) 2012-24  Jim Easterbrook  jim@jim-easterbrook.me.uk
+//  Copyright (C) 2018-24  Jim Easterbrook  jim@jim-easterbrook.me.uk
 //
 //  This program is free software: you can redistribute it and/or
 //  modify it under the terms of the GNU General Public License as
 //  published by the Free Software Foundation, either version 3 of the
 //  License, or (at your option) any later version.
 //
 //  This program is distributed in the hope that it will be useful,
@@ -12,219 +12,215 @@
 //  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 //  General Public License for more details.
 //
 //  You should have received a copy of the GNU General Public License
 //  along with this program.  If not, see
 //  <http://www.gnu.org/licenses/>.
 
-// See https://developers.google.com/maps/documentation/javascript/overview
+// See https://docs.mapbox.com/mapbox.js/api/v3.3.1/
+// and https://leafletjs.com/reference-1.7.1.html
 
+var drag_id = -1;
 var map;
 var markers = {};
 var gpsMarkers = {};
 var icon_on;
 var icon_off;
 var gpsBlueCircle;
-var gpsRedCircle;
+var gpsRedCircle
+
+window.addEventListener('load', initialize);
 
 function loadMap(lat, lng, zoom) {
-    var mapOptions = {
-        center: new google.maps.LatLng(lat, lng),
-        fullscreenControl: false,
-        scaleControl: true,
-        streetViewControl: false,
-        tilt: 0,
-        zoom: zoom,
-        maxZoom: 20,
-        mapTypeId: google.maps.MapTypeId.ROADMAP,
-        mapTypeControl: true,
-        mapTypeControlOptions: {
-            style: google.maps.MapTypeControlStyle.DROPDOWN_MENU,
-        },
-    };
-    map = new google.maps.Map(document.getElementById("mapDiv"), mapOptions);
-    google.maps.event.addListener(map, 'idle', newBounds);
-    var anchor = new google.maps.Point(11, 35);
-    icon_on = {
-        anchor: anchor,
-        url: 'pin_red.png'
-    };
-    icon_off = {
-        anchor: anchor,
-        url: 'pin_grey.png'
-    };
-    anchor = new google.maps.Point(5, 5);
-    gpsBlueCircle = {
-        anchor: anchor,
-        url: 'circle_blue.png'
-    };
-    gpsRedCircle = {
-        anchor: anchor,
-        url: 'circle_red.png'
+    var streets = L.mapbox.styleLayer(
+        'mapbox://styles/mapbox/streets-v11', {
+            tileSize: 512,
+            zoomOffset: -1
+        });
+    var outdoors = L.mapbox.styleLayer(
+        'mapbox://styles/mapbox/outdoors-v11', {
+            tileSize: 512,
+            zoomOffset: -1
+        });
+    var satellite = L.mapbox.styleLayer(
+        'mapbox://styles/mapbox/satellite-v9', {
+            tileSize: 512,
+            zoomOffset: -1
+        });
+    map = L.mapbox.map(document.getElementById("mapDiv"))
+    map.setView([lat, lng], zoom);
+    var baseMaps = {
+        "Street": streets,
+        "Outdoors": outdoors,
+        "Aerial": satellite,
     };
+    outdoors.addTo(map);
+    L.control.layers(baseMaps).addTo(map);
+    L.control.scale().addTo(map);
+    map.on('contextmenu', ignoreEvent);
+    map.on('moveend zoomend', newBounds);
+    icon_on = new L.Icon({
+        iconUrl: 'pin_red.png',
+        iconSize: [25, 35],
+        iconAnchor: [11, 35]
+    });
+    icon_off = new L.Icon({
+        iconUrl: 'pin_grey.png',
+        iconSize: [25, 35],
+        iconAnchor: [11, 35]
+    });
+    gpsBlueCircle = new L.Icon({
+        iconUrl: 'circle_blue.png',
+        iconSize: [11, 11],
+        iconAnchor: [5, 5]
+    });
+    gpsRedCircle = new L.Icon({
+        iconUrl: 'circle_red.png',
+        iconSize: [11, 11],
+        iconAnchor: [5, 5]
+    });
+    python.new_status({
+        version: L.version
+    });
     python.initialize_finished();
+    newBounds();
 }
 
-function newBounds() {
+function ignoreEvent(event) {}
+
+function newBounds(event) {
     var centre = map.getCenter();
     var bounds = map.getBounds();
     var sw = bounds.getSouthWest();
     var ne = bounds.getNorthEast();
     python.new_status({
-        centre: [centre.lat(), centre.lng()],
-        bounds: [ne.lat(), ne.lng(), sw.lat(), sw.lng()],
+        centre: [centre.lat, centre.lng],
+        bounds: [ne.lat, ne.lng, sw.lat, sw.lng],
         zoom: map.getZoom(),
     });
 }
 
 function setView(lat, lng, zoom) {
-    map.setZoom(zoom)
-    map.panTo(new google.maps.LatLng(lat, lng));
+    map.setView([lat, lng], zoom, {
+        animate: true
+    });
 }
 
 function adjustBounds(north, east, south, west) {
-    map.fitBounds({
-        north: north,
-        east: east,
-        south: south,
-        west: west
+    map.fitBounds([
+        [north, east],
+        [south, west]
+    ], {
+        animate: true
     });
 }
 
 function fitPoints(points) {
-    var bounds = new google.maps.LatLngBounds();
-    for (var i = 0; i < points.length; i++) {
-        bounds.extend({
-            lat: points[i][0],
-            lng: points[i][1]
-        });
-    }
-    var mapBounds = map.getBounds();
-    var mapSpan = mapBounds.toSpan();
-    var ne = bounds.getNorthEast();
-    var sw = bounds.getSouthWest();
-    bounds.extend({
-        lat: ne.lat() + (mapSpan.lat() * 0.13),
-        lng: ne.lng() + (mapSpan.lng() * 0.04)
-    });
-    bounds.extend({
-        lat: sw.lat() - (mapSpan.lat() * 0.04),
-        lng: sw.lng() - (mapSpan.lng() * 0.04)
-    });
-    ne = bounds.getNorthEast();
-    sw = bounds.getSouthWest();
-    if (mapBounds.contains(ne) && mapBounds.contains(sw))
+    var bounds = L.latLngBounds(points);
+    if (map.getBounds().contains(bounds))
         return;
-    var span = bounds.toSpan();
-    if (span.lat() > mapSpan.lat() || span.lng() > mapSpan.lng())
-        map.fitBounds(bounds);
-    else if (mapBounds.intersects(bounds))
-        map.panToBounds(bounds);
-    else
-        map.panTo(bounds.getCenter());
+    map.fitBounds(bounds, {
+        paddingTopLeft: [15, 50],
+        paddingBottomRight: [15, 10],
+        maxZoom: map.getZoom(),
+        animate: true
+    });
 }
 
 function plotGPS(points) {
     for (var i = 0; i < points.length; i++) {
-        var latlng = new google.maps.LatLng(points[i][0], points[i][1]);
+        var latlng = L.latLng(points[i][0], points[i][1]);
         var id = points[i][2];
-        gpsMarkers[id] = new google.maps.Marker({
-            map: map,
-            position: latlng,
+        gpsMarkers[id] = L.marker(latlng, {
             icon: gpsBlueCircle,
-            zIndex: 2,
-            clickable: false
+            interactive: false,
+            zIndexOffset: 1001
         });
+        gpsMarkers[id].addTo(map);
     }
 }
 
 function enableGPS(ids) {
-    for (var id in gpsMarkers)
-        if (ids.includes(id))
-            gpsMarkers[id].setOptions({
-                icon: gpsRedCircle,
-                zIndex: 3
-            });
-        else
-            gpsMarkers[id].setOptions({
-                icon: gpsBlueCircle,
-                zIndex: 2
-            });
+    for (var id in gpsMarkers) {
+        var marker = gpsMarkers[id];
+        if (ids.includes(id)) {
+            marker.setZIndexOffset(1002);
+            marker.setIcon(gpsRedCircle);
+        } else {
+            marker.setZIndexOffset(1001);
+            marker.setIcon(gpsBlueCircle);
+        }
+    }
 }
 
 function clearGPS() {
     for (var id in gpsMarkers)
-        gpsMarkers[id].setMap(null);
+        gpsMarkers[id].remove();
     gpsMarkers = {};
 }
 
 function enableMarker(id, active) {
     var marker = markers[id];
-    if (active)
-        marker.setOptions({
-            icon: icon_on,
-            zIndex: 1
-        });
-    else
-        marker.setOptions({
-            icon: icon_off,
-            zIndex: 0
-        });
+    if (active) {
+        marker.setZIndexOffset(1000);
+        if (id != drag_id)
+            marker.setIcon(icon_on);
+    } else {
+        marker.setZIndexOffset(0);
+        marker.setIcon(icon_off);
+    }
 }
 
 function addMarker(id, lat, lng, active) {
-    var marker = new google.maps.Marker({
-        icon: icon_off,
-        position: new google.maps.LatLng(lat, lng),
-        map: map,
+    var marker = L.marker([lat, lng], {
         draggable: true,
-        crossOnDrag: false,
+        autoPan: true
     });
+    marker.addTo(map);
     markers[id] = marker;
-    google.maps.event.addListener(marker, 'click', markerClick);
-    google.maps.event.addListener(marker, 'dragstart', markerClick);
-    google.maps.event.addListener(marker, 'drag', markerDrag);
-    google.maps.event.addListener(marker, 'dragend', markerDragEnd);
+    marker.on('click', markerClick);
+    marker.on('dragstart', markerDragStart);
+    marker.on('drag', markerDrag);
+    marker.on('dragend', markerDragEnd);
     enableMarker(id, active)
 }
 
 function markerToId(marker) {
     for (var id in markers)
         if (markers[id] == marker)
             return id;
 }
 
 function markerClick(event) {
     python.marker_click(markerToId(this));
 }
 
+function markerDragStart(event) {
+    // workaround for Leaflet bug #4484 - don't change marker image until end
+    // of drag. https://github.com/Leaflet/Leaflet/issues/4484
+    var id = markerToId(this);
+    drag_id = id;
+    python.marker_click(id);
+}
+
 function markerDrag(event) {
-    var loc = event.latLng;
-    python.marker_drag(loc.lat(), loc.lng());
+    var loc = this.getLatLng();
+    python.marker_drag(loc.lat, loc.lng);
 }
 
 function markerDragEnd(event) {
-    var loc = event.latLng;
-    python.marker_drag_end(loc.lat(), loc.lng(), markerToId(this));
+    var loc = this.getLatLng();
+    var id = markerToId(this);
+    this.setIcon(icon_on);
+    python.marker_drag_end(loc.lat, loc.lng, id);
+    drag_id = -1;
 }
 
 function markerDrop(x, y) {
-    // convert x, y to world coordinates
-    var scale = Math.pow(2, map.getZoom());
-    var nw = new google.maps.LatLng(
-        map.getBounds().getNorthEast().lat(),
-        map.getBounds().getSouthWest().lng()
-    );
-    var worldCoordinateNW = map.getProjection().fromLatLngToPoint(nw);
-    var worldX = worldCoordinateNW.x + (x / scale);
-    var worldY = worldCoordinateNW.y + (y / scale);
-    // convert world coordinates to lat & lng
-    var position = map.getProjection().fromPointToLatLng(
-        new google.maps.Point(worldX, worldY));
-    python.marker_drop(position.lat(), position.lng());
+    var position = map.containerPointToLatLng([x, y]);
+    python.marker_drop(position.lat, position.lng);
 }
 
 function delMarker(id) {
-    google.maps.event.clearInstanceListeners(markers[id]);
-    markers[id].setMap(null);
+    map.removeLayer(markers[id]);
     delete markers[id];
 }
```

### Comparing `Photini-2024.2.1/src/photini/data/map/pin_grey.png` & `Photini-2024.4.0/src/photini/data/map/pin_grey.png`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/data/map/pin_red.png` & `Photini-2024.4.0/src/photini/data/map/pin_red.png`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/data/windows/install_shortcuts.vbs` & `Photini-2024.4.0/src/photini/data/windows/install_shortcuts.vbs`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/descriptive.py` & `Photini-2024.4.0/src/photini/descriptive.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/editor.py` & `Photini-2024.4.0/src/photini/editor.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/editsettings.py` & `Photini-2024.4.0/src/photini/editsettings.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/exiv2.py` & `Photini-2024.4.0/src/photini/exiv2.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/ffmpeg.py` & `Photini-2024.4.0/src/photini/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/flickr.py` & `Photini-2024.4.0/src/photini/flickr.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/googlemap.py` & `Photini-2024.4.0/src/photini/googlemap.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,18 @@
     def tab_name():
         return translate('MapTabGoogle', 'Map (&Google)')
 
     def get_geocoder(self):
         return GoogleGeocoder(parent=self)
 
     def get_head(self):
-        url = 'http://maps.googleapis.com/maps/api/js?callback=initialize'
+        url = ('http://maps.googleapis.com/maps/api/js'
+               '?callback=initialize'
+               '&loading=async'
+               '&libraries=marker')
         if self.app.options.test:
             url += '&v=beta'
         url += '&key=' + self.api_key
         lang, encoding = locale.getlocale()
         if lang:
             language, sep, region = lang.replace('_', '-').partition('-')
             url += '&language=' + language
```

### Comparing `Photini-2024.2.1/src/photini/googlephotos.py` & `Photini-2024.4.0/src/photini/googlephotos.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/gpximporter.py` & `Photini-2024.4.0/src/photini/gpximporter.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/imagelist.py` & `Photini-2024.4.0/src/photini/imagelist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##  Photini - a simple photo metadata editor.
 ##  http://github.com/jim-easterbrook/Photini
-##  Copyright (C) 2012-23  Jim Easterbrook  jim@jim-easterbrook.me.uk
+##  Copyright (C) 2012-24  Jim Easterbrook  jim@jim-easterbrook.me.uk
 ##
 ##  This program is free software: you can redistribute it and/or
 ##  modify it under the terms of the GNU General Public License as
 ##  published by the Free Software Foundation, either version 3 of the
 ##  License, or (at your option) any later version.
 ##
 ##  This program is distributed in the hope that it will be useful,
@@ -18,18 +18,15 @@
 
 from datetime import datetime
 import io
 import logging
 import os
 import time
 
-try:
-    import PIL.Image as PIL
-except ImportError:
-    PIL = None
+import PIL.Image as PIL
 
 from photini.ffmpeg import FFmpeg
 from photini.metadata import Metadata
 from photini.pyqt import *
 from photini.pyqt import (image_types, image_types_lower, qt_version_info,
                           set_symbol_font, video_types, video_types_lower)
 
@@ -94,15 +91,15 @@
         return pixmap.transformed(transform)
 
     def regenerate_thumbnail(self):
         # DCF spec says thumbnail must be 160 x 120, so other aspect
         # ratios are padded with black
         # try using PIL first, good quality and quick
         qt_im = self.get_qt_image()
-        if qt_im and PIL:
+        if qt_im:
             data = self.make_thumb_PIL(qt_im)
             if data:
                 self.metadata.thumbnail = {'data': data}
                 return True
         # next try using FFmpeg, good quality but slower
         data = self.make_thumb_ffmpeg()
         if data:
```

### Comparing `Photini-2024.2.1/src/photini/importer.py` & `Photini-2024.4.0/src/photini/importer.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/ipernity.py` & `Photini-2024.4.0/src/photini/ipernity.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/loggerwindow.py` & `Photini-2024.4.0/src/photini/loggerwindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,20 +33,22 @@
 
 
 def full_version_info():
     version = 'Photini ' + photini_version
     version += '\n  Python ' + sys.version
     version += '\n  ' + exiv2_version
     version += '\n  ' + qt_version
-    version += ', locale ' + QtCore.QLocale.system().bcp47Name()
+    version += '\n  system locale ' + QtCore.QLocale.system().bcp47Name()
+    version += ', locales: ' + ' '.join(
+        QtCore.QLocale.system().uiLanguages())
     if spelling_version:
         version += '\n  ' + spelling_version
     if ffmpeg_version:
         version += '\n  ' + ffmpeg_version
-    version += '\n  available styles: {}'.format(
+    version += '\n  styles: {}'.format(
         ', '.join(QtWidgets.QStyleFactory.keys()))
     version += '\n  using style: {}'.format(
         QtWidgets.QApplication.style().objectName())
     return version
 
 
 class StreamProxy(QtCore.QObject):
```

### Comparing `Photini-2024.2.1/src/photini/mapboxmap.py` & `Photini-2024.4.0/src/photini/mapboxmap.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/metadata.py` & `Photini-2024.4.0/src/photini/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -824,14 +824,16 @@
                     'FocalPlaneResolutionUnit'):
             key = '.'.join((family, group, tag))
             if key not in resolution:
                 return None
             resolution[tag] = resolution[key]
         resolution['x'] = safe_fraction(resolution['FocalPlaneXResolution'])
         resolution['y'] = safe_fraction(resolution['FocalPlaneYResolution'])
+        if not (resolution['x'] and resolution['y']):
+            return None
         resolution['unit'] = int(resolution['FocalPlaneResolutionUnit'])
         # find largest image dimensions
         w = image_size['width'] / resolution['x']
         h = image_size['height'] / resolution['y']
         d = math.sqrt((h ** 2) + (w ** 2))
         if resolution['unit'] == 3:
             # unit is cm
```

### Comparing `Photini-2024.2.1/src/photini/ownership.py` & `Photini-2024.4.0/src/photini/ownership.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/photinimap.py` & `Photini-2024.4.0/src/photini/photinimap.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/pixelfed.py` & `Photini-2024.4.0/src/photini/pixelfed.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/pyqt.py` & `Photini-2024.4.0/src/photini/pyqt.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/regions.py` & `Photini-2024.4.0/src/photini/regions.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import logging
 import math
 import os
 import re
 
 from photini.cv import image_region_types, image_region_roles
 from photini.pyqt import *
-from photini.pyqt import set_symbol_font
+from photini.pyqt import set_symbol_font, using_pyside
 from photini.types import ImageRegionItem, MD_LangAlt
 from photini.widgets import LangAltWidget, MultiStringEdit, SingleLineEdit
 
 logger = logging.getLogger(__name__)
 translate = QtCore.QCoreApplication.translate
 
 
@@ -400,15 +400,18 @@
             if pixmap.isNull():
                 w, h = 0, 0
             else:
                 w, h = pixmap.width(), pixmap.height()
             # try image previews
             for data in image.metadata.get_previews():
                 buf = QtCore.QBuffer()
-                buf.setData(bytes(data))
+                # PySide insists on bytes, can't use buffer interface
+                if using_pyside:
+                    data = bytes(data)
+                buf.setData(data)
                 reader = QtGui.QImageReader(buf)
                 reader.setAutoTransform(False)
                 preview = QtGui.QPixmap.fromImageReader(reader)
                 if preview.isNull():
                     continue
                 if preview.width() > w:
                     pixmap = preview
```

### Comparing `Photini-2024.2.1/src/photini/scripts.py` & `Photini-2024.4.0/src/photini/scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,16 +89,15 @@
     options = [('flickr', 'photini.flickr', 'upload pictures to Flickr'),
                ('google', 'photini.googlephotos',
                 'upload pictures to Google Photos'),
                ('ipernity', 'photini.ipernity', 'upload pictures to Ipernity'),
                ('pixelfed', 'photini.pixelfed',
                 'upload pictures to Pixelfed or Mastodon'),
                ('spelling', None, 'check spelling of metadata'),
-               ('gpxpy', None, 'import GPS track data'),
-               ('Pillow', None, 'make higher quality thumbnails')]
+               ('gpxpy', None, 'import GPS track data')]
     if sys.platform != 'win32':
         options.append(
             ('importer', 'photini.importer', 'import pictures from a camera'))
     for name, module, description in options:
         msg = 'Would you like to {}? (y/n)'.format(description)
         if module:
             default = config.get('tabs', module)
```

### Comparing `Photini-2024.2.1/src/photini/spelling.py` & `Photini-2024.4.0/src/photini/spelling.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##  Photini - a simple photo metadata editor.
 ##  http://github.com/jim-easterbrook/Photini
-##  Copyright (C) 2012-22  Jim Easterbrook  jim@jim-easterbrook.me.uk
+##  Copyright (C) 2012-24  Jim Easterbrook  jim@jim-easterbrook.me.uk
 ##
 ##  This program is free software: you can redistribute it and/or
 ##  modify it under the terms of the GNU General Public License as
 ##  published by the Free Software Foundation, either version 3 of the
 ##  License, or (at your option) any later version.
 ##
 ##  This program is distributed in the hope that it will be useful,
@@ -23,15 +23,16 @@
 
 try:
     import enchant
 except ImportError as ex:
     enchant = None
     print(str(ex))
 
-from photini.pyqt import catch_all, QtCore, QtSignal, QtSlot, QtWidgets
+from photini.pyqt import (
+    catch_all, QtCore, QtSignal, QtSlot, QtWidgets, qt_version_info)
 
 logger = logging.getLogger(__name__)
 
 if enchant:
     spelling_version = 'PyEnchant ' + enchant.__version__
 else:
     spelling_version = None
@@ -50,15 +51,18 @@
     def available_languages():
         result = defaultdict(list)
         if enchant:
             for code in enchant.list_languages():
                 locale = QtCore.QLocale(code)
                 language = locale.languageToString(locale.language())
                 if '_' in code and '_ANY' not in code:
-                    country = locale.countryToString(locale.country())
+                    if qt_version_info < (6, 2):
+                        country = locale.countryToString(locale.country())
+                    else:
+                        country = locale.territoryToString(locale.territory())
                 else:
                     country = ''
                 result[language].append((country, code))
         else:
             return None
         for value in result.values():
             value.sort()
```

### Comparing `Photini-2024.2.1/src/photini/technical.py` & `Photini-2024.4.0/src/photini/technical.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/types.py` & `Photini-2024.4.0/src/photini/types.py`

 * *Files identical despite different names*

### Comparing `Photini-2024.2.1/src/photini/uploader.py` & `Photini-2024.4.0/src/photini/uploader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 ##  Photini - a simple photo metadata editor.
 ##  http://github.com/jim-easterbrook/Photini
-##  Copyright (C) 2012-23  Jim Easterbrook  jim@jim-easterbrook.me.uk
+##  Copyright (C) 2012-24  Jim Easterbrook  jim@jim-easterbrook.me.uk
 ##
 ##  This program is free software: you can redistribute it and/or
 ##  modify it under the terms of the GNU General Public License as
 ##  published by the Free Software Foundation, either version 3 of the
 ##  License, or (at your option) any later version.
 ##
 ##  This program is distributed in the hope that it will be useful,
@@ -24,24 +24,22 @@
 import logging
 import os
 import re
 import time
 import urllib
 
 import keyring
-try:
-    import PIL.Image as PIL
-except ImportError:
-    PIL = None
+import PIL.Image as PIL
 import requests
 
 from photini import __version__
 from photini.configstore import key_store
 from photini.metadata import Metadata
 from photini.pyqt import *
+from photini.pyqt import using_pyside
 from photini.widgets import Label, StartStopButton
 
 logger = logging.getLogger(__name__)
 translate = QtCore.QCoreApplication.translate
 
 
 class UploadAborted(Exception):
@@ -569,30 +567,16 @@
                 }
 
     def data_to_image(self, src):
         dst = dict(src)
         if dst['image']:
             return dst
         exiv_io = dst['data'].io()
-        if PIL:
-            # use Pillow for good quality
-            dst['image'] = PIL.open(io.BytesIO(exiv_io))
-            dst['width'], dst['height'] = dst['image'].size
-        else:
-            # use Qt, lower quality but available
-            buf = QtCore.QBuffer()
-            buf.setData(exiv_io)
-            reader = QtGui.QImageReader(buf)
-            reader.setAutoTransform(False)
-            im = reader.read()
-            if im.isNull():
-                raise RuntimeError(reader.errorString())
-            dst['image'] = im
-            dst['width'] = dst['image'].width()
-            dst['height'] = dst['image'].height()
+        dst['image'] = PIL.open(io.BytesIO(exiv_io))
+        dst['width'], dst['height'] = dst['image'].size
         return dst
 
     def image_to_data(self, src, mime_type=None, max_size=None):
         dst_mime_type = mime_type or src['mime_type']
         if src['data'] and src['mime_type'] == dst_mime_type and not (
                             max_size and src['data'].io().size() > max_size):
             return src
@@ -608,46 +592,29 @@
             dst_mime_type = mime_type or dst['mime_type']
             fmt = dst_mime_type.split('/')[1].upper()
             if dst_mime_type == 'image/jpeg':
                 options = [{'quality': 95}, {'quality': 85}, {'quality': 75}]
             else:
                 options = [{}]
             for option in options:
-                if PIL:
-                    dest_buf = io.BytesIO()
-                    dst['image'].save(dest_buf, format=fmt, **option)
-                    data = dest_buf.getbuffer()
-                else:
-                    dest_buf = QtCore.QBuffer()
-                    dest_buf.open(dest_buf.OpenModeFlag.WriteOnly)
-                    writer = QtGui.QImageWriter(dest_buf, fmt.encode('ascii'))
-                    writer.setQuality(option['quality'])
-                    if not writer.write(dst['image']):
-                        raise RuntimeError(writer.errorString())
-                    data = dest_buf.data().data()
+                dest_buf = io.BytesIO()
+                dst['image'].save(dest_buf, format=fmt, **option)
+                data = dest_buf.getbuffer()
                 dst['data'] = src['metadata'].clone(data)
                 dst['mime_type'] = dst_mime_type
                 if not (max_size and dst['data'].io().size() > max_size):
                     logger.info('Converted %s from %dx%d to %dx%d JPEG',
                                 src['name'], w_src, h_src, w_dst, h_dst)
                     return dst
         return None
 
     def resize_image(self, src, w, h):
         dst = self.data_to_image(src)
-        if PIL:
-            dst['image'] = dst['image'].resize(
-                (w, h), resample=PIL.BICUBIC)
-            dst['width'], dst['height'] = dst['image'].size
-        else:
-            dst['image'] = dst['image'].scaled(
-                w, h, Qt.AspectRatioMode.IgnoreAspectRatio,
-                Qt.TransformationMode.SmoothTransformation)
-            dst['width'] = dst['image'].width()
-            dst['height'] = dst['image'].height()
+        dst['image'] = dst['image'].resize((w, h), resample=PIL.BICUBIC)
+        dst['width'], dst['height'] = dst['image'].size
         dst['data'] = None
         dst['mime_type'] = 'image/jpeg'
         return dst
 
     def process_image(self, image):
         image = self.read_image(image)
         image = self.image_to_data(
```

### Comparing `Photini-2024.2.1/src/photini/widgets.py` & `Photini-2024.4.0/src/photini/widgets.py`

 * *Files identical despite different names*


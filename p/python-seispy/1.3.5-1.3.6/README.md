# Comparing `tmp/python-seispy-1.3.5.tar.gz` & `tmp/python_seispy-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-seispy-1.3.5.tar", last modified: Thu Feb 29 02:28:45 2024, max compression
+gzip compressed data, was "python_seispy-1.3.6.tar", last modified: Thu Apr 25 01:36:58 2024, max compression
```

## Comparing `python-seispy-1.3.5.tar` & `python_seispy-1.3.6.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:28:45.441604 python-seispy-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-02-29 02:28:36.000000 python-seispy-1.3.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-02-29 02:28:45.441604 python-seispy-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-02-29 02:28:36.000000 python-seispy-1.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:28:45.441604 python-seispy-1.3.5/python_seispy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-02-29 02:28:45.000000 python-seispy-1.3.5/python_seispy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-02-29 02:28:45.000000 python-seispy-1.3.5/python_seispy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 02:28:45.000000 python-seispy-1.3.5/python_seispy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-02-29 02:28:45.000000 python-seispy-1.3.5/python_seispy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 02:28:45.000000 python-seispy-1.3.5/python_seispy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-29 02:28:45.000000 python-seispy-1.3.5/python_seispy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-29 02:28:45.000000 python-seispy-1.3.5/python_seispy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:28:45.433603 python-seispy-1.3.5/seispy/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    15653 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/ccp3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/ccppara.py
--rw-r--r--   0 runner    (1001) docker     (127)    15478 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/ccpprofile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:28:45.433603 python-seispy-1.3.5/seispy/core/
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/core/RFStation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17643 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/core/depmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/core/pertmod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:28:45.437603 python-seispy-1.3.5/seispy/data/
--rwxr-xr-x   0 runner    (1001) docker     (127)  2645806 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/data/EventCMT.dat
--rwxr-xr-x   0 runner    (1001) docker     (127)      458 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/data/ak135.vel
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/data/cmpVsVp.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      978 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/data/cyan.mat
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/data/iasp91.vel
--rwxr-xr-x   0 runner    (1001) docker     (127)      875 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/data/mtna.vel
--rwxr-xr-x   0 runner    (1001) docker     (127)     3696 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/data/prem.vel
--rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/data/saveicon.png
--rw-r--r--   0 runner    (1001) docker     (127)    58484 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/data/seispy.png
--rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/decon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/distaz.py
--rw-r--r--   0 runner    (1001) docker     (127)    24961 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/eq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11384 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/geo.py
--rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/get_cpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/harmonics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/hk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/hkpara.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/mccc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/modcreator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/para.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:28:45.437603 python-seispy-1.3.5/seispy/pickdepth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/pickdepth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/pickdepth/get_depth.py
--rw-r--r--   0 runner    (1001) docker     (127)    12208 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/pickdepth/pickdepthui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:28:45.437603 python-seispy-1.3.5/seispy/pickrf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/pickrf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/pickrf/pickfigure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/pickrf/pickui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/pickrf/rpickfigure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:28:45.441604 python-seispy-1.3.5/seispy/pickseis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/pickseis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/pickseis/sviewerui.py
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/plotR.py
--rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/plotRT.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/psrayp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/recalrf.py
--rw-r--r--   0 runner    (1001) docker     (127)    25722 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/rf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/rf2depth_makedata.py
--rw-r--r--   0 runner    (1001) docker     (127)    14869 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/rfani.py
--rw-r--r--   0 runner    (1001) docker     (127)    40383 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/rfcorrect.py
--rw-r--r--   0 runner    (1001) docker     (127)    20224 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/seisfwd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/setuplog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/slantstack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-02-29 02:28:36.000000 python-seispy-1.3.5/seispy/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 02:28:45.441604 python-seispy-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-02-29 02:28:36.000000 python-seispy-1.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:28:45.441604 python-seispy-1.3.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-02-29 02:28:36.000000 python-seispy-1.3.5/test/test_case01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-02-29 02:28:36.000000 python-seispy-1.3.5/test/test_case02.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-02-29 02:28:36.000000 python-seispy-1.3.5/test/test_case03.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-02-29 02:28:36.000000 python-seispy-1.3.5/test/test_case04.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-02-29 02:28:36.000000 python-seispy-1.3.5/test/test_case05.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:58.453385 python_seispy-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-25 01:36:50.000000 python_seispy-1.3.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-04-25 01:36:58.453385 python_seispy-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-04-25 01:36:50.000000 python_seispy-1.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:58.453385 python_seispy-1.3.6/python_seispy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-04-25 01:36:58.000000 python_seispy-1.3.6/python_seispy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-25 01:36:58.000000 python_seispy-1.3.6/python_seispy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 01:36:58.000000 python_seispy-1.3.6/python_seispy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-25 01:36:58.000000 python_seispy-1.3.6/python_seispy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 01:36:58.000000 python_seispy-1.3.6/python_seispy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-25 01:36:58.000000 python_seispy-1.3.6/python_seispy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 01:36:58.000000 python_seispy-1.3.6/python_seispy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:58.445385 python_seispy-1.3.6/seispy/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15653 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/ccp3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/ccppara.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15619 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/ccpprofile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:58.445385 python_seispy-1.3.6/seispy/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/core/RFStation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19047 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/core/depmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/core/pertmod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:58.449385 python_seispy-1.3.6/seispy/data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)  2645806 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/data/EventCMT.dat
+-rwxr-xr-x   0 runner    (1001) docker     (127)      458 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/data/ak135.vel
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/data/cmpVsVp.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      978 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/data/cyan.mat
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/data/iasp91.vel
+-rwxr-xr-x   0 runner    (1001) docker     (127)      875 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/data/mtna.vel
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3696 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/data/prem.vel
+-rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/data/saveicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    58484 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/data/seispy.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/decon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/distaz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/eq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11448 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/get_cpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/harmonics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/hk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/hkpara.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/mccc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/modcreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11085 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/para.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:58.453385 python_seispy-1.3.6/seispy/pickdepth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/pickdepth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/pickdepth/get_depth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12208 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/pickdepth/pickdepthui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:58.453385 python_seispy-1.3.6/seispy/pickrf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/pickrf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/pickrf/pickfigure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/pickrf/pickui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/pickrf/rpickfigure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:58.453385 python_seispy-1.3.6/seispy/pickseis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/pickseis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/pickseis/sviewerui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/plotR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/plotRT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/psrayp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/recalrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29212 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/rf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10200 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/rf2depth_makedata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16742 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/rfani.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43094 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/rfcorrect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20224 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/seisfwd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/setuplog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/slantstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-25 01:36:50.000000 python_seispy-1.3.6/seispy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 01:36:58.453385 python_seispy-1.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-25 01:36:50.000000 python_seispy-1.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:36:58.453385 python_seispy-1.3.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-25 01:36:50.000000 python_seispy-1.3.6/test/test_case01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-25 01:36:50.000000 python_seispy-1.3.6/test/test_case02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-25 01:36:50.000000 python_seispy-1.3.6/test/test_case03.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-25 01:36:50.000000 python_seispy-1.3.6/test/test_case04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-25 01:36:50.000000 python_seispy-1.3.6/test/test_case05.py
```

### Comparing `python-seispy-1.3.5/LICENSE.txt` & `python_seispy-1.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/PKG-INFO` & `python_seispy-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-seispy
-Version: 1.3.5
+Version: 1.3.6
 Author: Mijian Xu
 Author-email: gomijianxu@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-seispy Version: 1.3.5 Author: Mijian Xu
+Metadata-Version: 2.1 Name: python-seispy Version: 1.3.6 Author: Mijian Xu
 Author-email: gomijianxu@gmail.com License: GPLv3 Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Description-Content-Type: text/markdown License-
 File: LICENSE.txt Requires-Dist: numpy>=1.19.0 Requires-Dist: scipy>=1.9.1
 Requires-Dist: matplotlib>=3.5.0 Requires-Dist: pandas>=1.0.0 Requires-Dist:
 obspy>=1.2.1 Requires-Dist: pyside6>=6.2.0 Requires-Dist:
```

### Comparing `python-seispy-1.3.5/README.md` & `python_seispy-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/python_seispy.egg-info/PKG-INFO` & `python_seispy-1.3.6/python_seispy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-seispy
-Version: 1.3.5
+Version: 1.3.6
 Author: Mijian Xu
 Author-email: gomijianxu@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-seispy Version: 1.3.5 Author: Mijian Xu
+Metadata-Version: 2.1 Name: python-seispy Version: 1.3.6 Author: Mijian Xu
 Author-email: gomijianxu@gmail.com License: GPLv3 Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Description-Content-Type: text/markdown License-
 File: LICENSE.txt Requires-Dist: numpy>=1.19.0 Requires-Dist: scipy>=1.9.1
 Requires-Dist: matplotlib>=3.5.0 Requires-Dist: pandas>=1.0.0 Requires-Dist:
 obspy>=1.2.1 Requires-Dist: pyside6>=6.2.0 Requires-Dist:
```

### Comparing `python-seispy-1.3.5/python_seispy.egg-info/SOURCES.txt` & `python_seispy-1.3.6/python_seispy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/python_seispy.egg-info/entry_points.txt` & `python_seispy-1.3.6/python_seispy.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/catalog.py` & `python_seispy-1.3.6/seispy/catalog.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/ccp3d.py` & `python_seispy-1.3.6/seispy/ccp3d.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/ccppara.py` & `python_seispy-1.3.6/seispy/ccppara.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/ccpprofile.py` & `python_seispy-1.3.6/seispy/ccpprofile.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     for i in range(lat.size-1):
         dis.append(distaz(lat[i], lon[i], lat[i+1], lon[i+1]).degreesToKilometers())
     return np.cumsum(dis)
 
 
 def create_center_bin_profile(stations, val=5, method='linear'):
     """Create bins along a profile with given stations
+
     :param stations: Stations along a profile
     :type stations: :class:`seispy.rf2depth_makedata.Station`
     :param val: The interval between two points in km
     :type val: float
     :param method: Method for interpolation
     :type method: str
     :return: The location of bins (bin_loca), and length between each bin and the start point (profile_range)
@@ -105,29 +106,30 @@
     bin_loca = np.vstack((lat_loca, lon_loca)).T
     return bin_loca, profile_range
 
 
 class CCPProfile():
     def __init__(self, cfg_file=None, log:SetupLog=SetupLog()):
         """CCPProfile class for CCP stacking along a profile
+
         :param cfg_file: Configure file for CCP stacking
         :type cfg_file: str
         :param log: Log class for logging
         :type log: :class:`seispy.setuplog.SetupLog`
         """
         self.logger = log
         if cfg_file is None:
             self.cpara = CCPPara()
         elif isinstance(cfg_file, str):
-            self.load_para(cfg_file)
+            self._load_para(cfg_file)
         else:
             raise ValueError('cfg_file must be str format.')
         self.stack_data = []
 
-    def load_para(self, cfg_file):
+    def _load_para(self, cfg_file):
         try:
             self.cpara = ccppara(cfg_file)
         except Exception as e:
             self.logger.CCPlog.error('Cannot open configure file {}'.format(cfg_file))
             raise FileNotFoundError('{}'.format(e))
         try:
             self.stack_mul = check_stack_val(self.cpara.stack_val, self.cpara.dep_val)
@@ -273,20 +275,27 @@
             boot_stack['profile_dis'] = self.profile_range[i]
             boot_stack['mu'] = bin_mu
             boot_stack['ci'] = bin_ci
             boot_stack['count'] = bin_count
             self.stack_data.append(boot_stack)   
 
     def save_stack_data(self, format='npz'):
-        """If format is \'npz\', saving stacked data and parameters to local as a npz file. To load the file, please use data = np.load(fname, allow_pickle=True).
-        data['cpara'] is the parameters when CCP stacking.
-        data['stack_data'] is the result of stacked data.
-
-        If format is \'dat\' the stacked data will be save into a txt file with 8 columns, including bin_lat, bin_lon, profile_dis, depth, amp, ci_low, ci_high and count.
-        where bin_lat and bin_lon represent the position of each bin; profile_dis represents the distance in km between each bin and the start point of the profile; depth represents depth of each bin; amp means the stacked amplitude; ci_low and ci_high mean confidence interval with bootstrap method; count represents stacking number of each bin.
+        """If format is ``npz``, saving stacked data and parameters to local as a npz file. To load the file, please use data = np.load(fname, allow_pickle=True).
+        ``data['cpara']`` is the parameters when CCP stacking.
+        ``data['stack_data']`` is the result of stacked data.
+
+        If format is ``dat`` the stacked data will be save into a txt file with 8 columns,
+        including ``bin_lat``, ``bin_lon``, ``profile_dis``, ``depth``, ``amp``, ``ci_low``, ``ci_high`` and ``count``.
+        
+        - ``bin_lat`` and ``bin_lon`` represent the position of each bin; 
+        - ``profile_dis`` represents the distance in km between each bin and the start point of the profile;
+        - ``depth`` represents depth of each bin;
+        - ``amp`` means the stacked amplitude; 
+        - ``ci_low`` and ``ci_high`` mean confidence interval with bootstrap method;
+        - ``count`` represents stacking number of each bin.
 
         :param format: Format for stacked data
         :type format: str
         """
         self.cpara.stackfile = _fix_filename(self.cpara.stackfile, format)
         self.logger.CCPlog.info('Saving stacked data to {}'.format(self.cpara.stackfile))
         if not isinstance(self.cpara.stackfile, str):
```

### Comparing `python-seispy-1.3.5/seispy/core/RFStation.py` & `python_seispy-1.3.6/seispy/core/RFStation.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 from obspy.io.sac import SACTrace
 from obspy.core import Stream
 
 
 class Trace_Clust(UserList):
     """
     user can accese traces from self.data or like a default list
+
+    .. rubric:: Example
+    
     >>> st= obspy.read();tt=Trace_Clust()
     >>> for _i in st:
     ...   _i.stats.sac ={};
     ...   _i.stats.sac["stla"]=10.0
     ...   _i.stats.sac["stlo"]=20.0
     >>> st = [SACTrace.from_obspy_trace(_i) for _i in st]
     >>> len(st)
```

### Comparing `python-seispy-1.3.5/seispy/core/depmodel.py` & `python_seispy-1.3.6/seispy/core/depmodel.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,22 +39,22 @@
 
     try:
         raw_model = np.loadtxt(filename)
     except:
         raise IOError
     # check cols of file
     if raw_model.shape[1] < 3 or raw_model.shape[1] > 4:
-        raise ValueError
+        raise ValueError('The file should contain 3 or 4 columns')
 
     # cal rho if rho is not given in vel files.
     if raw_model.shape[1] == 3:
         model = np.zeros((raw_model.shape[0], 4))
-        model[:3, :] = raw_model[:, :]
+        model[:, :3] = raw_model[:, :]
         _p, rho = vs2vprho(raw_model[:, 2])
-        model[3, :] = rho
+        model[:, 3] = rho
         return model
     else:
         return raw_model
 
 
 def _layer2grid(dep_range, model):
     """
@@ -113,40 +113,39 @@
         if dep > dep_range[-1]:
             break
     return np.vstack((dep_range, vp_dep, vs_dep, rho_dep)).T
 
 
 class DepModel(object):
     """
-    radiu_s is used to call piercing point
-    tps,tpsps or so are used to cal displacement
+    Class for constructing 1D velocity model and computing delay time of Ps, PpPs and PsPs Rays.
+
+    .. rubric:: Examples
 
-    examples:
     >>> model = DepModel(np.array([0, 20.1, 35.1, 100]))
     >>> print(model.dz)
     [ 0.  20.1 15.  64.9]
     >>> print(model.vp)
     [5.8        6.5        8.04001059 8.04764706]
     >>> print(model.vs)
     [3.36       3.75       4.47003177 4.49294118]
     """
 
     def __init__(self, dep_range, velmod='iasp91', elevation=0., layer_mod=False):
-        """Class for computing back projection of Ps Ray paths.
-
-        Parameters
-        ----------
-        dep_range : numpy.ndarray
-            Depth range for conversion
-            Depth for each layer, not thickness
-        velmod : str, optional
-            Text file of 1D velocity model with first 3 columns of depth/thickness, Vp and Vs,
-            by default 'iasp91'
-        elevation : float, optional Elevation in km, by default 0.0
-        layer_mod: True for search, and False for interp1d
+        """ Initialize DepModel object
+        
+        :type dep_range: numpy.ndarray
+        :param dep_range: Depth range for conversion
+        :type velmod: str, optional
+        :param velmod: Text file of 1D velocity model with first 3 columns of depth/thickness, Vp and Vs, by default 'iasp91'
+        :type elevation: float, optional
+        :param elevation: Elevation in km, by default 0.0
+        :type layer_mod: bool, optional
+        :param layer_mod: True for search, and False for interp1d, by default False
+        
         """
         self.isrho = False
         self.elevation = elevation
         self.layer_mod = layer_mod
         # dep layer for CCP or other purpose, relative to sea level, dont contain any depth infomation
         self.depths = dep_range.astype(float)
         self.dep_val = np.average(np.diff(self.depths))
@@ -162,14 +161,39 @@
                     _layer2grid(self.depths, self.model_array)
             else:
                 self.vp, self.vs, self.rho = \
                     _intep_mod(self.model_array, self.depths_elev)
 
     @classmethod
     def read_layer_model(cls, dep_range, h, vp, vs, rho=None, elevation=0):
+        """ Read layer model from given parameters
+
+        :type dep_range: numpy.ndarray
+        :param dep_range: Depth range for conversion
+        :type h: numpy.ndarray
+        :param h: Thickness of each layer
+        :type vp: numpy.ndarray
+        :param vp: P-wave velocity of each layer
+        :type vs: numpy.ndarray
+        :param vs: S-wave velocity of each layer
+        :type rho: numpy.ndarray
+        :param rho: Density of each layer, by default None
+        :type elevation: float
+        :param elevation: Elevation in km, by default 0
+        :rtype: DepModel
+        :return: DepModel object
+
+        .. rubric:: Examples
+        
+        >>> dep_range = np.arange(100)
+        >>> h = np.array([20, 15., 0])
+        >>> vp = np.array([5.8, 6.5, 8.04])
+        >>> vs = np.array([3.36, 3.75, 4.47])
+        >>> model = DepModel.read_layer_model(dep_range, h, vp, vs)
+        """
         mod = cls(dep_range, velmod=None, layer_mod=True, elevation=elevation)
         if rho is not None:
             mod.isrho = True
         mod._elevation()
         mod.model_array = _from_layer_model(mod.depths, h, vp, vs, rho=rho)
         mod.vp, mod.vs, mod.rho = _layer2grid(mod.depths, mod.model_array)
         return mod
@@ -178,14 +202,18 @@
         """
         set all depth related values:
         1. depths_elev: depth array contains layer above sea level(represent by value lower than 0
         2. depths_extend: depth array contains layer above sea level( evaluate from 0 to original depth
         3. dz: 0, thick_1, thick_2....
         4. thickness: thick_1, thick_2, ... , 0
         requires elevation, depths_range or other component
+
+        .. rubric:: Examples
+
+
         >>> model = DepModel(np.array([0, 20.1, 35.1, 100]))
         >>> model.depths_elev
         array([  0. ,  20.1,  35.1, 100. ])
         >>> model.depths_extend
         array([  0. ,  20.1,  35.1, 100. ])
         >>> model.dz
         array([ 0. , 20.1, 15. , 64.9])
@@ -215,18 +243,16 @@
         self.thickness = np.append(np.diff(self.depths_extend), 0.)
         self.R = 6371.0 - self.depths_elev
 
     def plot_model(self, show=True):
         """
         plot model with matplotlib
         
-        Parameters
-        ----------
-        show : bool, optional
-        whether to show the plot, by default True
+        :type show: bool, optional
+        :param show: whether to show the plot, by default True
         """        
         plt.style.use('bmh')
         if self.isrho:
             self.model_fig = plt.figure(figsize=(6, 6))
             fignum = 2
         else:
             self.model_fig = plt.figure(figsize=(4, 6))
@@ -249,26 +275,23 @@
         if show:
             plt.show()
 
     def tpds(self, rayps, raypp, sphere=True):
         # generate docstring
         """
         calculate travel time of Pds
-        Parameters
-        ----------
-        rayps : float or numpy.ndarray
-            ray parameter of Ps wave
-        raypp : float or numpy.ndarray
-            ray parameter of P wave
-        sphere : bool, optional
-            whether to use sphere earth, by default True
-        
-        Returns
-        -------
-        travel time of Pds
+
+        :type rayps: float or numpy.ndarray
+        :param rayps: ray parameter of Ps wave
+        :type raypp: float or numpy.ndarray
+        :param raypp: ray parameter of P wave
+        :type sphere: bool, optional
+        :param sphere: whether to use sphere earth, by default True
+        :rtype: numpy.ndarray
+        :return: travel time of Pds
         """
 
         if sphere:
             radius = self.R
         else:
             radius = 6371.
         tps = np.cumsum((np.sqrt((radius / self.vs) ** 2 - rayps ** 2) -
@@ -276,70 +299,68 @@
                         (self.dz / radius))
         return tps
 
     def tpppds(self, rayps, raypp, sphere=True):
         """
         calculate travel time of Ppds
 
-        Parameters
-        ----------
-        rayps : float or numpy.ndarray
-            ray parameter of Ps wave
-        raypp : float or numpy.ndarray
-            ray parameter of P wave
-        sphere : bool, optional
-            whether to use sphere earth, by default True
-        
-        Returns
-        -------
-        travel time of Ppds
+        :type rayps: float or numpy.ndarray
+        :param rayps: ray parameter of Ps wave
+        :type raypp: float or numpy.ndarray
+        :param raypp: ray parameter of P wave
+        :type sphere: bool, optional
+        :param sphere: whether to use sphere earth, by default True
+        :rtype: numpy.ndarray
+        :return: travel time of Ppds
         """
         if sphere:
             radius = self.R
         else:
             radius = 6371.
         tps = np.cumsum((np.sqrt((radius / self.vs) ** 2 - rayps ** 2) +
                          np.sqrt((radius / self.vp) ** 2 - raypp ** 2)) *
                         (self.dz / radius))
         return tps
 
     def tpspds(self, rayps, sphere=True):
         """
         calculate travel time of Ppsds
         
-        Parameters
-        ----------
-        rayps : float or numpy.ndarray
-            ray parameter of Ps wave
-        sphere : bool, optional
-            whether to use sphere earth, by default True
-        
-        Returns
-        -------
-        travel time of Ppsds
+        :type rayps: float or numpy.ndarray
+        :param rayps: ray parameter of Ps wave
+        :type sphere: bool, optional
+        :param sphere: whether to use sphere earth, by default True
+        :rtype: numpy.ndarray
+        :return: travel time of Ppsds
         """
         if sphere:
             radius = self.R
         else:
             radius = 6371.
         tps = np.cumsum(2 * np.sqrt((radius / self.vs) ** 2 - rayps ** 2) *
                         (self.dz / radius))
         return tps
 
     def radius_s(self, rayp, phase='P', sphere=True):
         """
-        calculate piercing point, P for Sp and S for Ps
-        Parameters
-        ----------
-        rayp
-        phase
-        sphere
+        calculate horizontal radius from piercing point to station postion.
+        
+        P for Sp and S for Ps.
+
+        :type rayp: float or numpy.ndarray
+        :param rayp: ray parameter
+        :type phase: str, optional
+        :param phase: phase name, by default 'P'
+        :type sphere: bool, optional
+        :param sphere: whether to use sphere earth, by default True
+        :rtype: numpy.ndarray
+        :return: horizontal radius
+        
+        .. rubric:: Examples
 
-        Returns
-        -------
         >>> model = DepModel(np.array([0, 20.1, 35.1, 100]))
         >>> model.dz
         array([ 0. , 20.1, 15. , 64.9])
         >>> model.R
         array([6371. , 6350.9, 6335.9, 6271. ])
         >>> model.radius_s(1.2,phase="S", sphere=False)*111.2
         array([0.        , 0.0002478 , 0.00046823, 0.00142685])
@@ -355,14 +376,20 @@
         hor_dis = np.cumsum((self.dz / radius) / np.sqrt((1. / (rayp ** 2. * (radius / vel) ** -2)) - 1))
         #hor_dis = np.sqrt((1. / (rayp ** 2. * (radius / vel) ** -2)) - 1)
         return hor_dis
 
     def save_tvel(self, filename):
         """
         save vel mod in tvel format for taup
+
+        :type filename: str
+        :param filename: output file name
+
+        .. rubric:: Examples
+
         >>> model = DepModel(np.array([0, 20.1, 35.1, 100]))
         >>> model.save_tvel("test")
             0.00     5.80     3.36     2.72
            20.10    5.800     3.36     2.72
            20.10     6.50     3.75     2.92
            35.10    6.500     3.75     2.92
            35.10     8.04     4.47     3.32
@@ -395,26 +422,22 @@
                 raise IOError('cannot write to {}'.format(filename))
 
 
     def raylength(self, rayp, phase='P', sphere=True):
         """
         calculate ray length, P for Sp and S for Ps
         
-        Parameters
-        ----------
-        rayp: float or numpy.ndarray
-            ray parameter
-        phase: str, optional
-            phase name, by default 'P'
-        sphere: bool, optional
-            whether to use sphere earth, by default True
-        
-        Returns
-        -------
-        ray length
+        :type rayp: float or numpy.ndarray
+        :param rayp: ray parameter
+        :type phase: str, optional
+        :param phase: phase name, by default 'P'
+        :type sphere: bool, optional
+        :param sphere: whether to use sphere earth, by default True
+        :rtype: numpy.ndarray
+        :return: ray length
         """
 
         if phase == 'P':
             vel = self.vp
         else:
             vel = self.vs
         if sphere:
@@ -428,16 +451,19 @@
     def ccp_model(cls, dep_range = np.array([0, 20.1, 35.1, 100]),
                   elevation = 0, layerd = False, **kwargs):
         """
         import ccp configure and init DepModel object for time2depth convertion
         if any parameters given is wrong, return a default DepModel object
 
         there's 3 types of input is allowed:
+
         1. mod3d, stla, stlo: for 3d model( need modification
+
         2. modfolder, staname: for dir
+
         3. mod: for single file
         """
         if kwargs.get("mod3d", None):
             stla = kwargs.pop("stla",None)
             stlo = kwargs.pop("stlo", None)
             # if stla and stlo is not given return iasp91 model
             if not stla or not stlo:
@@ -477,31 +503,25 @@
         raise ValueError('More then 1 file were found as the expresion: {}'.format(expresion))
     else:
         return modfiles[0]
 
 def interp_depth_model(model, lat, lon, new_dep):
     """ Interpolate Vp and Vs from 3D velocity with a specified depth range.
 
-    Parameters
-    ----------
-    mod3d : :meth:`np.lib.npyio.NpzFile`
-        3D velocity loaded from a ``.npz`` file
-    lat : float
-        Latitude of position in 3D velocity model
-    lon : float
-        Longitude of position in 3D velocity model
-    new_dep : :meth:`np.ndarray`
-        1D array of depths in km
-
-    Returns
-    -------
-    Vp : :meth:`np.ndarray`
-        Vp in ``new_dep``
-    Vs : :meth:`np.ndarray`
-        Vs in ``new_dep``
+    :param mod3d: 3D velocity loaded from a ``.npz`` file
+    :type mod3d: :meth:`np.lib.npyio.NpzFile`
+    :param lat: Latitude of position in 3D velocity model
+    :type lat: float
+    :param lon: Longitude of position in 3D velocity model
+    :type lon: float
+    :param new_dep: 1D array of depths in km
+    :type new_dep: :meth:`np.ndarray`
+    :rtype: :meth:`np.ndarray`
+    :return: Vp and Vs in ``new_dep``
+    
     """
     #  model = np.load(modpath)
     points = [[depth, lat, lon] for depth in new_dep]
     vp = interpn((model['dep'], model['lat'], model['lon']), model['vp'], points, bounds_error=False, fill_value=None)
     vs = interpn((model['dep'], model['lat'], model['lon']), model['vs'], points, bounds_error=False, fill_value=None)
     return vp, vs
```

### Comparing `python-seispy-1.3.5/seispy/core/pertmod.py` & `python_seispy-1.3.6/seispy/core/pertmod.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/data/EventCMT.dat` & `python_seispy-1.3.6/seispy/data/EventCMT.dat`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/data/cmpVsVp.txt` & `python_seispy-1.3.6/seispy/data/cmpVsVp.txt`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/data/cyan.mat` & `python_seispy-1.3.6/seispy/data/cyan.mat`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/data/iasp91.vel` & `python_seispy-1.3.6/seispy/data/iasp91.vel`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/data/mtna.vel` & `python_seispy-1.3.6/seispy/data/mtna.vel`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/data/prem.vel` & `python_seispy-1.3.6/seispy/data/prem.vel`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/data/saveicon.png` & `python_seispy-1.3.6/seispy/data/saveicon.png`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/data/seispy.png` & `python_seispy-1.3.6/seispy/data/seispy.png`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/decon.py` & `python_seispy-1.3.6/seispy/decon.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/distaz.py` & `python_seispy-1.3.6/seispy/distaz.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,20 @@
 import math
 import numpy as np
 
 
-def sind(deg):
-    rad = math.radians(deg)
-    return math.sin(rad)
-
-
-def cosd(deg):
-    rad = math.radians(deg)
-    return math.cos(rad)
-
-
-def tand(deg):
-    rad = math.radians(deg)
-    return math.tan(rad)
-
-
-def cotd(deg):
-    rad = math.radians(deg)
-    return math.cos(rad) / math.sin(rad)
-
-
-def asind(x):
-    rad = math.asin(x)
-    return math.degrees(rad)
-
-
-def acosd(x):
-    rad = math.acos(x)
-    return math.degrees(rad)
-
-
-def atand(x):
-    rad = math.atan(x)
-    return math.degrees(rad)
-
-
-def km2deg(kilometers):
-    return kilometers / 111.19
-
-
-def deg2km(degree):
-    return degree * 111.19
-
-
 class distaz:
     """
-    c Subroutine to calculate the Great Circle Arc distance
-    c    between two sets of geographic coordinates
-    c
-    c Equations take from Bullen, pages 154, 155
-    c
-    c T. Owens, September 19, 1991
-    c           Sept. 25 -- fixed az and baz calculations
-    c
+    Subroutine to calculate the Great Circle Arc distance
+        between two sets of geographic coordinates
+    
+    Equations take from Bullen, pages 154, 155
+    
+    T. Owens, September 19, 1991
+              Sept. 25 -- fixed az and baz calculations
     P. Crotwell, Setember 27, 1995
     Converted to c to fix annoying problem of fortran giving wrong
     answers if the input doesn't contain a decimal point.
     
     H. P. Crotwell, September 18, 1997
     Java version for direct use in java programs.
     *
```

### Comparing `python-seispy-1.3.5/seispy/eq.py` & `python_seispy-1.3.6/seispy/eq.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 class TooMoreComponents(Exception):
     def __init__(self, matchkey):
         self.matchkey = matchkey
     def __str__(self):
         return '{}'.format(self.matchkey)
 
 def rotateZNE(st):
+    """Rotate Z, N, E components to Z, N, E components
+    """
     try:
         zne = rotate2zne(
             st[0], st[0].stats.sac.cmpaz, st[0].stats.sac.cmpinc,
             st[1], st[1].stats.sac.cmpaz, st[1].stats.sac.cmpinc,
             st[2], st[2].stats.sac.cmpaz, st[2].stats.sac.cmpinc)
     except Exception as e:
         raise ValueError('No specified cmpaz or cmpinc. {}'.format(e))
@@ -88,14 +90,15 @@
     def _cleanstream(self):
         self.st = None
         self.rf = None
 
     @classmethod
     def from_stream(cls, stream):
         """Create EQ object from obspy stream
+
         :param stream: obspy stream
         :type stream: obspy.Stream
         :return: EQ object
         :rtype: EQ
         """
         eq = cls('', '')
         eq.st = stream
@@ -134,14 +137,21 @@
         if switchEN:
             chE = self.st.select(channel='*[E2]')[0].stats.channel
             chN = self.st.select(channel='*[N1]')[0].stats.channel
             self.st.select(channel='*[E2]')[0].stats.channel = chN
             self.st.select(channel='*[N1]')[0].stats.channel = chE
 
     def write(self, path, evt_datetime):
+        """Write raw stream to SAC files
+
+        :param path: path to save SAC files
+        :type path: str
+        :param evt_datetime: event datetime
+        :type evt_datetime: obspy.core.utcdatetime.UTCDateTime
+        """
         for tr in self.st:
             sac = SACTrace.from_obspy_trace(tr)
             sac.b = 0
             sac.o = evt_datetime - tr.stats.starttime
             fname = join(path, '{}.{}.{}.{}.SAC'.format(
                 tr.stats.network, tr.stats.station,
                 tr.stats.starttime.strftime('%Y.%j.%H%M%S'),
@@ -154,25 +164,27 @@
         """
         self.st.detrend(type='linear')
         self.st.detrend(type='constant')
         self.fix_channel_name()
 
     def filter(self, freqmin=0.05, freqmax=1, order=4):
         """Bandpass filter
+
         :param freqmin: minimum frequency, defaults to 0.05
         :type freqmin: float, optional
         :param freqmax: maximum frequency, defaults to 1
         :type freqmax: float, optional
         :param order: filter order, defaults to 4
         :type order: int, optional
         """
         self.st.filter('bandpass', freqmin=freqmin, freqmax=freqmax, corners=order, zerophase=True)
 
     def get_arrival(self, model, evdp, dis, phase='P'):
         """Get arrival time, ray parameter and incident angle from TauP model
+
         :param model: TauP model
         :type model: TauPyModel
         :param evdp: focal depth
         :type evdp: float
         :param dis: epicentral distance
         :type dis: float
         :param phase: phase name, defaults to 'P'
@@ -188,14 +200,15 @@
             self.arr_time = arrivals[0].time
             self.rayp = arrivals[0].ray_param
             self.inc = arrivals[0].incident_angle
             self.phase = phase
 
     def search_inc(self, bazi):
         """Search incident angle for S wave
+
         :param bazi: back azimuth
         :type bazi: float
         :return: incident angle
         :rtype: float
         """
         inc_range = np.arange(0.1, 90, 0.1)
         s_range = self.trim(20, 20, isreturn=True)
@@ -207,14 +220,15 @@
         real_inc_idx = np.argmin(power)
         real_inc = inc_range[real_inc_idx]
         self.inc_correction = real_inc - self.inc
         self.inc = real_inc
 
     def search_baz(self, bazi, time_b=10, time_e=20, offset=90):
         """Search back azimuth for P wave
+
         :param bazi: back azimuth
         :type bazi: float
         :param time_b: time before P arrival, defaults to 10
         :type time_b: int, optional
         :param time_e: time after P arrival, defaults to 20
         :type time_e: int, optional
         :param offset: offset for searching, defaults to 90
@@ -257,14 +271,15 @@
             self.st.select(channel='*3')[0].stats.channel = 'E'
             self.st.sort(['channel'])
         else:
             pass
 
     def rotate(self, baz, inc=None, method='NE->RT', search_inc=False, baz_shift=0):
         """Rotate to radial and transverse components
+
         :param baz: back azimuth
         :type baz: float
         :param inc: incident angle, defaults to None
         :type inc: float, optional
         :param method: method for rotation, defaults to 'NE->RT'
         :type method: str, optional
         :param search_inc: whether search incident angle, defaults to False
@@ -290,14 +305,15 @@
         elif method == 'LQT->ZNE':
             self.st.rotate('LQT->ZNE', back_azimuth=bazi, inclination=self.inc)
         else:
             pass
 
     def snr(self, length=50):
         """Calculate SNR
+
         :param length: length for noise, defaults to 50
         :type length: int, optional
         :return: SNR of E, N, Z components
         :rtype: (float, float, float)
         """
         st_noise = self.trim(length, 0, isreturn=True)
         st_signal = self.trim(0, length, isreturn=True)
@@ -313,14 +329,15 @@
             snr_Z = snr(st_signal[2].data, st_noise[2].data)
         except IndexError:
             snr_Z = 0
         return snr_E, snr_N, snr_Z
     
     def get_time_offset(self, event_time=None):
         """Get time offset from SAC header
+
         :param event_time: event time, defaults to None
         :type event_time: obspy.core.utcdatetime.UTCDateTime, optional
         """
         if event_time is not None and not isinstance(event_time, obspy.core.utcdatetime.UTCDateTime):
             raise TypeError('Event time should be UTCDateTime type in obspy')
         elif event_time is None:
             self.timeoffset = self.st[2].stats.sac.b - self.st[2].stats.sac.o
@@ -343,14 +360,15 @@
         arr = self.arr_correct(write_to_sac=False)
         t1 = self.st[2].stats.starttime + (arr + self.trigger_shift - time_before)
         t2 = self.st[2].stats.starttime + (arr + self.trigger_shift + time_after)
         return t1, t2
 
     def phase_trigger(self, time_before, time_after, prepick=True, stl=5, ltl=10):
         """ Trigger P or S phase
+
         :param time_before: time before P or S arrival
         :type time_before: float
         :param time_after: time after P or S arrival
         :type time_after: float
         :param prepick: whether use prepick, defaults to True
         :type prepick: bool, optional
         :param stl: short time length for STA/LTA, defaults to 5
@@ -441,14 +459,15 @@
                 for tr in self.rf:
                     if tr.stats.delta != target_dt:
                         tr.data = resample(tr.data, int((shift + time_after)/target_dt+1))
                         tr.stats.delta = target_dt
     
     def decon_p(self, tshift, tcomp=False, **kwargs):
         """Deconvolution for P wave
+
         :param tshift: Time shift before P arrival
         :type tshift: float
         :param tcomp: Whether calculate transverse component, defaults to False
         :type tcomp: bool, optional
         """
         if self.comp == 'lqt':
             win = self.st.select(channel='*L')[0]
@@ -464,14 +483,15 @@
             else:
                 uin = self.st.select(channel='*R')[0]
         uout = RFTrace.deconvolute(uin, win, phase='P', tshift=tshift, **kwargs)
         self.rf.append(uout)
 
     def decon_s(self, tshift, **kwargs):
         """Deconvolution for S wave
+
         :param tshift: Time shift before P arrival
         :type tshift: float
         """
         if self.comp == 'lqt':
             win = self.st.select(channel='*Q')[0]
             uin = self.st.select(channel='*L')[0]
         else:
@@ -483,14 +503,15 @@
         uout.data = np.flip(uout.data)
         self.rf.append(uout)
 
     def saverf(self, path, evtstr=None, shift=0, evla=-12345., 
                evlo=-12345., evdp=-12345., mag=-12345.,
                gauss=0, baz=-12345., gcarc=-12345., only_r=False, **kwargs):
         """Save receiver function to SAC file
+
         :param path: path to save SAC file
         :type path: str
         :param evtstr: event string, defaults to None
         :type evtstr: str, optional
         :param shift: time shift before P arrival, defaults to 0
         :type shift: int, optional
         :param evla: event latitude, defaults to -12345.
@@ -556,14 +577,15 @@
         if rssq(trrf.data[nt0:nt25]) > rssq(trrf.data[nt25:]):
             return True
         else:
             return False
 
     def judge_rf(self, gauss, shift, npts, criterion='crust', rmsgate=None):
         """Judge whether receiver function is valid
+        
         :param gauss: Gaussian factor
         :type gauss: float
         :param shift: time shift before P arrival
         :type shift: float
         :param npts: number of points for RF
         :type npts: int
         :param criterion: criterion for judging, defaults to 'crust'
```

### Comparing `python-seispy-1.3.5/seispy/geo.py` & `python_seispy-1.3.6/seispy/geo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,178 +1,195 @@
 import numpy as np
 from seispy import distaz
 from pyproj import Geod
 from seispy.utils import scalar_instance, array_instance
 
 def sind(deg):
     """ Sine function with degree as input
+
     :param deg: Degree
     :type deg: float
     :return: Sine value
     :rtype: float
     """
     rad = np.radians(deg)
     return np.sin(rad)
 
 
 def cosd(deg):
     """ Cosine function with degree as input
+
     :param deg: Degree
     :type deg: float
     :return: Cosine value
     :rtype: float
     """
     rad = np.radians(deg)
     return np.cos(rad)
 
 
 def tand(deg):
     """ Tangent function with degree as input
+
     :param deg: Degree
     :type deg: float
     :return: Tangent value
     :rtype: float
     """
     rad = np.radians(deg)
     return np.tan(rad)
 
 
 def cotd(deg):
     """ Cotangent function with degree as input
+
     :param deg: Degree
     :type deg: float
     :return: Cotangent value
     :rtype: float
     """
     rad = np.radians(deg)
     return np.cos(rad) / np.sin(rad)
 
 
 def asind(x):
     """ Inverse sine function with degree as output
+
     :param x: Sine value
     :type x: float
     :return: Degree
     :rtype: float
     """
     rad = np.arcsin(x)
     return np.degrees(rad)
 
 
 def acosd(x):
     """ Inverse cosine function with degree as output
+
     :param x: Cosine value
     :type x: float
     :return: Degree 
     :rtype: float
     """
     rad = np.arccos(x)
     return np.degrees(rad)
 
 
 def atand(x):
     """ Inverse tangent function with degree as output
+
     :param x: Tangent value
     :type x: float
     :return: Degree
     :rtype: float
     """
     rad = np.arctan(x)
     return np.degrees(rad)
 
 
 def km2deg(km):
     """ Convert km to degree
+
     :param km: Distance in km
     :type km: float
     :return: Distance in degree
     :rtype: float
     """
     radius = 6371
     circum = 2*np.pi*radius
     conv = circum / 360
     deg = km / conv
     return deg
 
 
 def deg2km(deg):
     """ Convert degree to km
+
     :param deg: Distance in degree
     :type deg: float
     :return: Distance in km
     :rtype: float
     """
     radius = 6371
     circum = 2*np.pi*radius
     conv = circum / 360
     km = deg * conv
     return km
 
 
 def rad2deg(rad):
     """ Convert radian to degree
+
     :param rad: Radian
     :type rad: float
     :return: Degree
     :rtype: float
     """
     deg = rad*(360/(2*np.pi))
     return deg
 
 
 def skm2sdeg(skm):
     """ Convert s/km to s/degree
+
     :param skm: s/km
     :type skm: float
     :return: s/degree
     :rtype: float
     """
     sdeg = skm * deg2km(1)
     return sdeg
 
 
 def sdeg2skm(sdeg):
     """ Convert s/degree to s/km
+
     :param sdeg: s/degree
     :type sdeg: float
     :return: s/km
     :rtype: float
     """
     skm = sdeg / deg2km(1)
     return skm
 
 
 def srad2skm(srad):
     """ Convert s/rad to s/km
+
     :param srad: s/rad
     :type srad: float
     :return: s/km
     :rtype: float
     """
     sdeg = srad * ((2*np.pi)/360)
     return sdeg / deg2km(1)
 
 
 def skm2srad(skm):
     """ Convert s/km to s/rad
+
     :param skm: s/km
     :type skm: float
     :return: s/rad
     :rtype: float
     """
     sdeg = skm * deg2km(1)
     return rad2deg(sdeg)
 
 
 def rot3D(bazi, inc):
     """
     Rotate components from ZRT to LQT
-    M = [cos(inc)     -sin(inc)*sin(bazi)    -sin(inc)*cos(bazi);
-        sin(inc)      cos(inc)*sin(bazi)     cos(inc)*cos(bazi);
-        0              -cos(bazi)             sin(bazi)];
+    
+    .. code-block:: python
+
+    M = [[cos(inc)     -sin(inc)*sin(bazi)    -sin(inc)*cos(bazi)],
+         [sin(inc)      cos(inc)*sin(bazi)     cos(inc)*cos(bazi)],
+         [0              -cos(bazi)             sin(bazi)]]
     
     :param bazi: back-azimuth of station-event pair
     :param inc: Incidence angle
     :return: Coefficient matrix m
     :rtype: np.ndarray
     """
 
@@ -190,14 +207,15 @@
                   [np.sin(inc), np.cos(inc)*np.sin(bazi), np.cos(inc)*np.cos(bazi)],
                   [value31, -np.cos(bazi), np.sin(bazi)]])
     return m
 
 
 def rotateSeisZENtoLQT(z, e, n, bazi, inc):
     """ Rotate ZEN to LQT
+
     :param z: Vertical component
     :type z: np.ndarray
     :param e: East component
     :type e: np.ndarray
     :param n: North component
     :type n: np.ndarray
     :param bazi: Back-azimuth
@@ -211,14 +229,15 @@
     zen = np.array([z, e, n])
     lqt = np.dot(m, zen)
     return lqt[0, :], lqt[1, :], lqt[2, :]
 
 
 def spherical2cartesian(lon, lat, dep):
     """ Convert spherical coordinates to cartesian coordinates
+
     :param lon: Longitude
     :type lon: float
     :param lat: Latitude
     :type lat: float
     :param dep: Depth
     :type dep: float
     :return: Cartesian coordinates
@@ -230,14 +249,15 @@
     y = r * sind(cola) * sind(lon)
     z = r * cosd(cola)
     return x, y, z
 
 
 def rotateSeisENtoTR(e, n, baz):
     """ Rotate EN to TR
+
     :param e: East component
     :type e: np.ndarray
     :param n: North component
     :type n: np.ndarray
     :param baz: Back-azimuth
     :type baz: float
     :return: T and R components
@@ -257,14 +277,15 @@
     :rtype: float
     """
     return np.sqrt(np.sum(x**2)/len(x))
 
 
 def snr(x, y):
     """ Signal-to-noise ratio
+    
     :param x: Signal
     :type x: np.ndarray
     :param y: Noise
     :type y: np.ndarray
     :return: SNR
     :rtype: float
     """
@@ -354,14 +375,15 @@
     g = Geod(ellps=ellps)
     lon, lat, _ = g.fwd(lon0, lat0, azimuth, deg2km(gcarc_dist)*1000)
     return lat, lon
 
 
 def geoproject(lat_p, lon_p, lat1, lon1, lat2, lon2):
     """ Project a point to a line
+
     :param lat_p: Latitude of the point
     :type lat_p: float
     :param lon_p: Longitude of the point
     :type lon_p: float
     :param lat1: Latitude of the first point of the line
     :type lat1: float
     :param lon1: Longitude of the first point of the line
@@ -407,14 +429,15 @@
     phi = np.radians(lon)
     r = 6371 - dep
     return r, theta, phi
 
 def sph2geo(r, theta, phi):
     """
     Convert spherical coordinates to geographic coordinates.
+
     :param float r: radial distance from coordinate system origin
                     {**Units**: km, **Range**: [0, inf)}
     :param float theta: polar angle {**Units**: radians, **Range**: [0,
                         π]}
     :param float phi: azimuthal angle {**Units**: radians, **Range**:
                       [-π, π]}
     :returns: geographic coordinate conversion *(lat, lon, depth)* of
```

### Comparing `python-seispy-1.3.5/seispy/get_cpt.py` & `python_seispy-1.3.6/seispy/get_cpt.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/harmonics.py` & `python_seispy-1.3.6/seispy/harmonics.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/hk.py` & `python_seispy-1.3.6/seispy/hk.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,14 +132,15 @@
         f.savefig(path, format='png', dpi=400, bbox_inches='tight')
 
 
 def ci(allstack, h, kappa, ev_num):
     """
     Search best H and kappa from stacked matrix.
     Calculate error for H and kappa
+
     :param allstack: stacked HK matrix
     :param h: 1-D array of H
     :param kappa: 1-D array of kappa
     :param ev_num: event number
     :return:
     """
     [i, j] = np.unravel_index(allstack.argmax(), allstack.shape)
```

### Comparing `python-seispy-1.3.5/seispy/hkpara.py` & `python_seispy-1.3.6/seispy/hkpara.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/io.py` & `python_seispy-1.3.6/seispy/io.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/mccc.py` & `python_seispy-1.3.6/seispy/mccc.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/modcreator.py` & `python_seispy-1.3.6/seispy/modcreator.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/para.py` & `python_seispy-1.3.6/seispy/para.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,17 +49,31 @@
         """
         try:
             self.query = Query(server, user=user, password=password)
         except Exception as e:
             raise ConnectionError('Cannot connect with {} server'.format(server))
 
     def get_stainfo(self):
+        """Get station information
+
+        :return: Station information
+        :rtype: dict
+        """
         return self.__dict__
 
     def load_stainfo(self, pathname, ref_comp, suffix):
+        """Load station information from SAC file
+
+        :param pathname: Path to SAC file
+        :type pathname: str
+        :param ref_comp: Reference component
+        :type ref_comp: str
+        :param suffix: Suffix of SAC file
+        :type suffix: str
+        """
         (self.network, self.station, self.stla, self.stlo, self.stel) = _load_station_info(pathname, ref_comp, suffix)
 
     def get_station_from_ws(self, **kwargs):
         """Get station information from web-service with given network and station or other optional condition.
 
         
         """
```

### Comparing `python-seispy-1.3.5/seispy/pickdepth/get_depth.py` & `python_seispy-1.3.6/seispy/pickdepth/get_depth.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/pickdepth/pickdepthui.py` & `python_seispy-1.3.6/seispy/pickdepth/pickdepthui.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/pickrf/pickfigure.py` & `python_seispy-1.3.6/seispy/pickrf/pickfigure.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/pickrf/pickui.py` & `python_seispy-1.3.6/seispy/pickrf/pickui.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/pickrf/rpickfigure.py` & `python_seispy-1.3.6/seispy/pickrf/rpickfigure.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/pickseis/sviewerui.py` & `python_seispy-1.3.6/seispy/pickseis/sviewerui.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/plotR.py` & `python_seispy-1.3.6/seispy/plotR.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/plotRT.py` & `python_seispy-1.3.6/seispy/plotRT.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/psrayp.py` & `python_seispy-1.3.6/seispy/psrayp.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/recalrf.py` & `python_seispy-1.3.6/seispy/recalrf.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/rf.py` & `python_seispy-1.3.6/seispy/rf.py`

 * *Files 14% similar despite different names*

```diff
@@ -106,14 +106,27 @@
                     (eq_lst['mag']>=magmin) & (eq_lst['mag']<=magmax) & \
                     (eq_lst['evdp']>=depthmin) & (eq_lst['evdp']<=depthmax) & \
                     (dis>=dismin) & (dis<=dismax)]
     return eq_lst
 
 
 def fetch_waveform(eq_lst, para, model, logger):
+    """Fetch waveforms from remote data server
+
+    :param eq_lst: Earthquake list
+    :type eq_lst: pandas.DataFrame
+    :param para: RFPara object
+    :type para: seispy.para.RFPara
+    :param model: TauPyModel object
+    :type model: obspy.taup.TauPyModel
+    :param logger: Logger
+    :type logger: seispy.setuplog.SetupLog
+    :return: Earthquake list with fetched waveforms
+    :rtype: pandas.DataFrame
+    """
     tb = np.max([2*para.noiselen, 2*para.time_before])
     te = np.max([2*para.noiselen, 2*para.time_after])
     try:
         query = para.stainfo.query
     except:
         logger.RFlog.error('Please load station information and search earthquake before fetch waveform')
     new_col = ['dis', 'bazi', 'data', 'datestr']
@@ -240,14 +253,21 @@
         raise FileNotFoundError('Cannot open configure file %s' % cfg_file)
     cf.set(session, key, value)
     cf.write(open(cfg_file, 'w'))
 
 
 class RF(object):
     def __init__(self, cfg_file=None, log=None):
+        """Procedure of Receiver function analysis
+
+        :param cfg_file: Path to configure file, defaults to None
+        :type cfg_file: str, optional
+        :param log: Logger, defaults to None
+        :type log: seispy.setuplog.SetupLog, optional
+        """
         if log is None:
             self.logger = SetupLog()
         else:
             self.logger = log
         if cfg_file is None:
             self.para = RFPara()
         elif isinstance(cfg_file, str):
@@ -278,14 +298,19 @@
         return self.para.date_end
 
     @date_end.setter
     def date_end(self, value):
         self.para.date_end = value
 
     def load_stainfo(self, use_date_range=True):
+        """Load station information from local file or remote web-service
+        
+        :param use_date_range: Use date range to search station information, defaults to True
+        :type use_date_range: bool, optional
+        """
         try:
             if self.para.use_remote_data:
                 self.logger.RFlog.info('Load station info of {}.{} from {} web-service'.format(
                     self.para.stainfo.network, self.para.stainfo.station, self.para.data_server))
                 self.para.stainfo.link_server(
                     self.para.data_server,
                     self.para.data_server_user,
@@ -309,14 +334,21 @@
             self.logger.RFlog.info('{}.{}, latitude: {:.3f}, longitude: {:.3f}'.format(
                 self.para.stainfo.network, self.para.stainfo.station, self.stainfo.stla, self.stainfo.stlo))
         except Exception as e:
             self.logger.RFlog.error('Error in loading station info: {0}'.format(e))
             sys.exit(1)
 
     def search_eq(self, local=False, catalog=None):
+        """Search earthquakes from local or online data server
+
+        :param local: Search from local data, defaults to False
+        :type local: bool, optional
+        :param catalog: Catalog type, defaults to None
+        :type catalog: str, optional
+        """
         if not local:
             try:
                 self.logger.RFlog.info('Searching earthquakes from {}'.format(self.para.cata_server))
                 if self.para.date_end > UTCDateTime():
                     self.para.date_end = UTCDateTime()
                 query = Query(self.para.cata_server)
                 query.get_events(starttime=self.para.date_begin, endtime=self.para.date_end,
@@ -363,33 +395,44 @@
         if self.eqs.shape[0] == 0:
             self.logger.RFlog.warning('No earthquakes associated, please check configurations.'.format(self.eqs.shape[0]))
             sys.exit(1)
         else:
             self.logger.RFlog.info('{0} earthquakes are associated'.format(self.eqs.shape[0]))
 
     def save_raw_data(self):
+        """Save raw data to local disk
+        """
         if not exists(self.para.datapath):
             makedirs(self.para.datapath)
         for i, row in self.eqs.iterrows():
             row['data'].write(self.para.datapath, row['date'])
 
     def savepjt(self):
+        """Save project to local disk
+        """
         eqs = self.eqs.copy()
         for _, row in eqs.iterrows():
             row['data'].cleanstream()
         try:
             self.logger.RFlog.info('Saving project to {0}'.format(self.para.pjtpath))
             with open(self.para.pjtpath, 'wb') as f:
                 pickle.dump({'para': self.para, 'eqs': eqs}, f, -1)
         except Exception as e:
             self.logger.RFlog.error('{0}'.format(e))
             raise IOError(e)
  
     @classmethod
     def loadpjt(cls, path):
+        """Load project from local disk
+
+        :param path: Path to project file
+        :type path: str
+        :return: Project object
+        :rtype: seispy.rf.RF
+        """
         with open(path, 'rb') as f:
             rfdata = pickle.load(f)
         pjt = cls(phase=rfdata['para'].phase)
         pjt.para = rfdata['para']
         if not exists(pjt.para.datapath):
             pjt.logger.RFlog.error('Data path {} was not found'.format(pjt.para.datapath))
             sys.exit(1)
@@ -400,46 +443,72 @@
                 row['data'].readstream()
             except Exception as e:
                 pjt.logger.RFlog.warning('Cannot read {}, skipping'.format(row['data'].filestr))
                 continue
         return pjt
 
     def channel_correct(self):
+        """Correct channel components
+        """
         if self.para.switchEN or self.para.reverseN or self.para.reverseE:
             self.logger.RFlog.info('Correct components with switchEN: {}, reverseE: {}, reverseN: {}'.format(
                                     self.para.switchEN, self.para.reverseE, self.para.reverseN))
             for _, row in self.eqs.iterrows():
                 row['data'].channel_correct(self.para.switchEN, self.para.reverseE, self.para.reverseN)
         
     def detrend(self):
+        """Detrend all data
+        """
         self.logger.RFlog.info('Detrend all data')
         drop_idx = []
         for i, row in self.eqs.iterrows():
             try:
                 row['data'].detrend()
             except:
                 self.logger.RFlog.error('Data error in {}'.format(row['date'].strftime('%Y.%j.%H.%M.%S')))
                 drop_idx.append(i)
         self.eqs.drop(drop_idx, inplace=True)
 
     def filter(self, freqmin=None, freqmax=None, order=4):
+        """Filter all data
+
+        :param freqmin: Minimum frequency, defaults to self.para.freqmin
+        :type freqmin: float, optional
+        :param freqmax: Maximum frequency, defaults to self.para.freqmax
+        :type freqmax: float, optional
+        :param order: Order of filter, defaults to 4
+        :type order: int, optional
+        """
         if freqmin is None:
             freqmin = self.para.freqmin
         if freqmax is None:
             freqmax = self.para.freqmax
         self.logger.RFlog.info('Filter all data from {0} to {1}'.format(freqmin, freqmax))
         for _, row in self.eqs.iterrows():
             row['data'].filter(freqmin=freqmin, freqmax=freqmax, order=order)
 
     def cal_phase(self):
+        """Calculate arrivals and ray parameters for all data
+        """
         self.logger.RFlog.info('Calculate {} arrivals and ray parameters for all data'.format(self.para.phase))
         for _, row in self.eqs.iterrows():
             row['data'].get_arrival(self.model, row['evdp'], row['dis'], phase=self.para.phase)
 
     def baz_correct(self, time_b=10, time_e=20, offset=90, correct_angle=None):
+        """Correct back-azimuth for all data
+
+        :param time_b: Begin time of searching, defaults to 10
+        :type time_b: int, optional
+        :param time_e: End time of searching, defaults to 20
+        :type time_e: int, optional
+        :param offset: Offset of searching, defaults to 90
+        :type offset: int, optional
+        :param correct_angle: Correct angle, defaults to None
+        :type correct_angle: float, optional
+        """
         if correct_angle is not None:
             self.logger.RFlog.info('correct back-azimuth with {} deg.'.format(correct_angle))
             self.eqs['bazi'] = np.mod(self.eqs['bazi'] + correct_angle, 360)
         else:
             self.logger.RFlog.info('correct back-azimuth with T energy minimization')
             y = np.arange(self.eqs.shape[0])
             shift_all = np.array([])
@@ -452,14 +521,19 @@
             if None in shift_all:
                 self.logger.RFlog.error('Range of searching bazi is too small.')
                 sys.exit(1)
             self.baz_shift = np.mean(shift_all[np.where(np.logical_not(np.isnan(shift_all)))])
             self.logger.RFlog.info('Average {:.1f} deg offset in back-azimuth'.format(self.baz_shift))
 
     def rotate(self, search_inc=False):
+        """Rotate all data to ZNE or RTZ
+
+        :param search_inc: Search incidence angle, defaults to False
+        :type search_inc: bool, optional
+        """
         targ_comp = ''.join(sorted(self.para.comp.upper()))
         if targ_comp == 'RTZ':
             method='NE->RT'
         elif targ_comp == 'LQT':
             method='ZNE->LQT'
         else:
             raise ValueError('comp must be in RTZ or LQT.')
@@ -474,14 +548,21 @@
                 continue
             if search_inc:
                 self.logger.RFlog.info('The incidence angle of {} was corrected by {:.1f} deg'.format(
                                        row['data'].datestr, row['data'].inc_correction))
         self.eqs.drop(drop_idx, inplace=True)
 
     def drop_eq_snr(self, length=None, z_only=False):
+        """Drop earthquakes with low SNR
+
+        :param length: Length of data, defaults to None
+        :type length: int, optional
+        :param z_only: Use Z component only, defaults to False
+        :type z_only: bool, optional
+        """
         if length is None:
             length = self.para.noiselen
         self.logger.RFlog.info('Reject data record with SNR less than {0}'.format(self.para.noisegate))
         drop_lst = []
         for i, row in self.eqs.iterrows():
             snr_E, snr_N, snr_Z = row['data'].snr(length=length)
             if z_only:
@@ -490,29 +571,42 @@
                 mean_snr = np.mean([snr_E, snr_N, snr_Z])
             if mean_snr < self.para.noisegate:
                 drop_lst.append(i)
         self.eqs.drop(drop_lst, inplace=True)
         self.logger.RFlog.info('{0} events left after SNR calculation'.format(self.eqs.shape[0]))
 
     def trim(self):
+        """Trim waveforms from start to end
+        """
         self.logger.RFlog.info('Trim waveforms from {0:.2f} before {2} to {1:.2f} after {2}'.format(
                                self.para.time_before, self.para.time_after, self.para.phase))
         for _, row in self.eqs.iterrows():
             row['data'].trim(self.para.time_before, self.para.time_after)
     
     def pick(self, prepick=True, stl=5, ltl=10):
+        """Pick phase arrival
+
+        :param prepick: Use STA/LTA method, defaults to True
+        :type prepick: bool, optional
+        :param stl: Short time length, defaults to 5
+        :type stl: int, optional
+        :param ltl: Long time length, defaults to 10
+        :type ltl: int, optional
+        """
         if prepick:
             self.logger.RFlog.info('Pre-pick {} arrival using STA/LTA method'.format(self.para.phase))
         for _, row in self.eqs.iterrows():
             row['data'].phase_trigger(self.para.time_before, self.para.time_after,
                                       prepick=prepick, stl=stl, ltl=ltl)
         pickphase(self.eqs, self.para, self.logger)
         self.logger.RFlog.info('{0} events left after visual checking'.format(self.eqs.shape[0]))
 
     def deconv(self):
+        """Deconvolution for all data
+        """
         shift = self.para.time_before
         time_after = self.para.time_after
         drop_lst = []
 
         count = 0
         for i, row in self.eqs.iterrows():
             count += 1
@@ -529,14 +623,19 @@
                         row['data'].datestr, count, self.eqs.shape[0], row['data'].rf[0].stats.rms))
             except Exception as e:
                 self.logger.RFlog.error('{}: {}'.format(row['data'].datestr, e))
                 drop_lst.append(i)
         self.eqs.drop(drop_lst, inplace=True)
 
     def saverf(self, gauss=None):
+        """Save receiver functions to local disk
+        
+        :param gauss: Gaussian width, defaults to self.para.gauss
+        :type gauss: float, optional
+        """
         npts = int((self.para.time_before + self.para.time_after)/self.para.target_dt+1)
         if self.para.phase[-1] == 'P':
             shift = self.para.time_before
         elif self.para.phase[-1] == 'S':
             shift = self.para.time_after
         else:
             pass
@@ -563,14 +662,16 @@
                                    user9=self.baz_shift)
                 good_lst.append(i)
         self.logger.RFlog.info('{} PRFs are saved.'.format(len(good_lst)))
         self.eqs = self.eqs.loc[good_lst]
 
 
 def setpar():
+    """Set parameters to configure file
+    """
     parser = argparse.ArgumentParser(description="Set parameters to configure file")
     parser.add_argument('cfg_file', type=str, help='Path to configure file')
     parser.add_argument('session', type=str, help='session name')
     parser.add_argument('key', type=str, help='key name')
     parser.add_argument('value', type=str, help='value')
     arg = parser.parse_args()
     CfgModify(arg.cfg_file, arg.session, arg.key, arg.value)
```

### Comparing `python-seispy-1.3.5/seispy/rf2depth_makedata.py` & `python_seispy-1.3.6/seispy/rf2depth_makedata.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,16 @@
 
 class RFDepth():
     """Convert receiver function to depth axis
     """
     def __init__(self, cpara:CCPPara, log:Logger=SetupLog().RF2depthlog,
                  raytracing3d=False, velmod3d=None, modfolder1d=None) -> None:
         """
+        Convert receiver function to depth axis
+        
         :param cpara: CCPPara object
         :type cpara: CCPPara
         :param log: Log object
         :type log: logging.Logger
         :param raytracing3d: If True, use 3D ray tracing to calculate the travel time
         :type raytracing3d: bool
         :param velmod3d: Path to 3D velocity model in npz file
```

### Comparing `python-seispy-1.3.5/seispy/rfani.py` & `python_seispy-1.3.6/seispy/rfani.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import matplotlib.pyplot as plt
 from os.path import join
 from seispy.geo import cosd, sind, extrema
 from scipy.interpolate import griddata
 from seispy.utils import load_cyan_map
 
 
-def joint_stack(energy_r, energy_cc, energy_tc, weight=[0.4, 0.3, 0.3]):
+def _joint_stack(energy_r, energy_cc, energy_tc, weight=[0.4, 0.3, 0.3]):
     energy_r = energy_r / np.max(energy_r)
     energy_cc = energy_cc / np.max(energy_cc)
     energy_tc = energy_tc / np.max(energy_tc)
     return np.exp(np.log(energy_r) * weight[0] + np.log(energy_cc) * weight[1] - np.log(energy_tc) * weight[2])
 
 
-def average_delay(fd, td):
+def _average_delay(fd, td):
     uniq_fd = np.unique(fd)
     if uniq_fd.size > 2:
         raise ValueError('FVD do not converge, {} gotten'.format(uniq_fd))
     uniq_td = []
     for i, fv in enumerate(uniq_fd):
         idx = np.where(fd==fv)[0]
         uniq_td.append(np.mean(td[idx]))
@@ -52,64 +52,80 @@
         self.tlen = tlen
         self.sacdatar = sacdatar
         self.sacdatar.resample(0.1)
         self.nbs = int((self.tb + self.sacdatar.shift) / self.sacdatar.sampling)
         self.nes = int((self.te + self.sacdatar.shift) / self.sacdatar.sampling)
         self.sacdatar.moveoutcorrect(ref_rayp=rayp, velmod=model, replace=True)
         self.baz_stack(val=val)
-        self.search_peak_amp()
-        self.init_ani_para()
+        self._search_peak_amp()
+        self._init_ani_para()
         self.fvd, self.deltat = np.meshgrid(self.fvd_1d, self.deltat_1d)
 
     def baz_stack(self, val=10):
+        """Stack RF data with back-azimuth.
+
+        Parameters
+        ----------
+
+        val : int, optional
+            Interval of back-azimuth, by default 10
+        """
         self.stack_range = np.arange(0, 360, val)
         stacked_data = self.sacdatar.bin_stack(lim=[0, 360], val=val)
         self.rfr_baz = stacked_data['data_prime']
         self.rft_baz = stacked_data['datat']
         self.count_baz = stacked_data['count']
 
-    def search_peak_amp(self):
+    def _search_peak_amp(self):
         mean_rf = np.mean(self.rfr_baz, axis=0)
         nmax = extrema(mean_rf[self.nbs:self.nes])+self.nbs
         if nmax.size > 1:
             nps = nmax[np.nanargmax(mean_rf[nmax])]
         else:
             nps = nmax[0]
         self.nb = int(nps - self.tlen / self.sacdatar.sampling)
         self.ne = int(nps + self.tlen / self.sacdatar.sampling)
 
-    def init_ani_para(self):
+    def _init_ani_para(self):
         self.deltat_1d = np.arange(0, 1.55, 0.05)
         self.fvd_1d = np.arange(0, 365, 5)
 
-    def cut_energy_waveform(self, idx, nb, ne):
+    def _cut_energy_waveform(self, idx, nb, ne):
+        """Cut energy waveform with given index, nb and ne.
+        """
         engr = np.zeros([nb.shape[0], nb.shape[1], self.ne-self.nb])
         for i in range(nb.shape[0]):
             for j in range(nb.shape[1]):
                 engr[i, j, :] = self.rfr_baz[idx, nb[i, j]:ne[i, j]]
         return engr
 
     def radial_energy_max(self):
+        """Calculate the energy of radial component.
+        """
         energy = np.zeros([self.fvd.shape[0], self.fvd.shape[1], self.ne-self.nb])
         # tmp_data = np.zeros(self.ne-self.nb)
         for i, baz in enumerate(self.stack_range):
             t_corr = (self.deltat / 2) * cosd(2 * (self.fvd - baz))
             nt_corr = (t_corr / self.sacdatar.sampling).astype(int)
             new_nb = self.nb - nt_corr
             new_ne = self.ne - nt_corr
-            energy += self.cut_energy_waveform(i, new_nb, new_ne)
+            energy += self._cut_energy_waveform(i, new_nb, new_ne)
         energy = np.max(energy ** 2, axis=2)
         energy /= np.max(np.sum(self.rfr_baz[:, self.nb:self.ne], axis=0)**2)
         return energy
 
     def xyz2grd(self, energy):
+        """Interpolate energy to grid.
+        """
         self.fvd, self.deltat = np.meshgrid(self.fvd_1d, self.deltat_1d)
         return griddata(self.ani_points, energy, (self.fvd, self.deltat))
 
     def rotate_to_fast_slow(self):
+        """Rotate RF data to fast and slow direction.
+        """
         self.ani_points = np.empty([0, 2])
         for f in self.fvd_1d:
             for d in self.deltat_1d:
                 self.ani_points = np.vstack((self.ani_points, np.array([f, d])))
         energy_cc = np.zeros(self.ani_points.shape[0])
         energy_tc = np.zeros(self.ani_points.shape[0])
         raw_energy_r = np.sum(np.sum(self.rfr_baz[:, self.nb:self.ne], axis=0) ** 2 - np.sum(self.rfr_baz[:, self.nb:self.ne] ** 2, axis=0))
@@ -133,14 +149,23 @@
             energy_cc[i] = np.sum(fcr ** 2 - fcr_sq) / raw_energy_r
             energy_tc[i] = fct/ raw_energy_t
         # energy_cc /= np.max(np.abs(energy_cc))
         energy_tc /= np.max(np.abs(energy_tc))
         return self.xyz2grd(energy_cc), self.xyz2grd(energy_tc)
 
     def plot_stack_baz(self, enf=60, outpath='./'):
+        """Plot the stack of RF data with back-azimuth.
+        
+        Parameters
+        ----------
+        enf : int, optional
+            Enlarge factor for back-azimuth, by default 60
+        outpath : str, optional
+            Output path for saving the figure, by default './'
+        """
         ml = MultipleLocator(5)
         bound = np.zeros_like(self.sacdatar.time_axis)
         plt.style.use("bmh")
         plt.rc('grid', color='white', linestyle='-', linewidth=0.7)
         plt.rcParams["axes.grid.axis"] = "x"
         fig = plt.figure(figsize=(15, 8))
         axr = plt.subplot(1, 2, 1)
@@ -187,14 +212,27 @@
         # axt.yaxis.set_minor_locator(ml)
         axr.set_ylabel('Back-azimuth ($^\circ$)',  fontsize=16)
         # axt.set_xlabel('Time after P(s)')
         axt.set_title('T component ({})'.format(self.sacdatar.staname), fontsize=16)
         fig.savefig(join(outpath, '{}_baz_stack.png'.format(self.sacdatar.staname)), dpi=400, bbox_inches='tight')
 
     def plot_correct(self, fvd=0, dt=0.44, enf=80, outpath=None):
+        """Plot the RF data with back-azimuth and time after P corrected.
+
+        Parameters
+        ----------
+        fvd : int, optional
+            Fast velocity direction, by default 0
+        dt : float, optional
+            Time delay for correction, by default 0.44
+        enf : int, optional
+            Enlarge factor for back-azimuth, by default 80
+        outpath : str, optional
+            Output path for saving the figure, by default None
+        """
         nt_corr = int((dt/2 / self.sacdatar.sampling))
         # nt_fast = np.arange(self.nb, self.ne) + nt_corr
         # nt_slow = np.arange(self.nb, self.ne) - nt_corr
         time_axis = np.arange(self.nb, self.ne) * self.sacdatar.sampling - self.sacdatar.shift
         bound = np.zeros_like(time_axis)
         ml = MultipleLocator(5)
         plt.figure(figsize=(8, 6))
@@ -226,41 +264,66 @@
         axr.set_ylabel('Back-azimuth ($^\circ$)', fontsize=16)
         axr.set_title('R component',  fontsize=16)
         axt.set_title('T component',  fontsize=16)
         if outpath is not None and isinstance(outpath, str):
             plt.savefig(join(outpath, 'rf_corrected.png'), dpi=400, bbox_inches='tight')
 
     def search_peak_list(self, energy, opt='max'):
+        """Search the peak of energy.
+
+        Parameters
+        ----------
+        energy : np.ndarray
+            Energy matrix
+        opt : str, optional
+            Option for searching peak, by default 'max'
+        """
         if opt == 'max':
             ind = np.argwhere(energy == np.max(energy))
         elif opt == 'min':
             ind = np.argwhere(energy == np.min(energy))
         else:
             raise ValueError('\'opt\' must be max or min')
         return self.ani_points[ind][:, 0], self.ani_points[ind][:, 1]
 
     def search_peak(self, energy, opt='max'):
+        """Search the peak of energy.
+
+        Parameters
+        ----------
+        energy : np.ndarray
+            Energy matrix
+        opt : str, optional
+            Option for searching peak, by default 'max'
+        """
         if opt == 'max':
             ind = np.argwhere(energy == np.max(energy))
         elif opt == 'min':
             ind = np.argwhere(energy == np.min(energy))
         else:
             raise ValueError('\'opt\' must be max or min')
         best_fvd = []
         best_dt = []
         for i, j in ind:
             best_fvd.append(self.fvd[i, j])
             best_dt.append(self.deltat[i, j])
-        uniq_fd, uniq_td = average_delay(np.array(best_fvd), np.array(best_dt))
+        uniq_fd, uniq_td = _average_delay(np.array(best_fvd), np.array(best_dt))
         return uniq_fd, uniq_td
 
     def joint_ani(self, weight=[0.5, 0.3, 0.2]):
+        """Joint method for crustal anisotropy estimation.
+
+        Parameters
+        ----------
+        weight : list, optional
+            Weight for three energy matrix, by default [0.5, 0.3, 0.2]
+        """
         self.energy_r = self.radial_energy_max()
         self.energy_cc, self.energy_tc = self.rotate_to_fast_slow()
-        self.energy_joint = joint_stack(self.energy_r, self.energy_cc, self.energy_tc, weight)
+        self.energy_joint = _joint_stack(self.energy_r, self.energy_cc, self.energy_tc, weight)
         self.bf, self.bt = self.search_peak(self.energy_joint, opt='max')
         return self.bf, self.bt
 
     def plot_polar(self, cmap=load_cyan_map(), show=False, outpath='./'):
         """Polar map of crustal anisotropy. See Liu and Niu (2012, doi: 10.1111/j.1365-246X.2011.05249.x) in detail.
 
         :param cmap: Colormap of matplotlib, defaults to 'rainbow'
```

### Comparing `python-seispy-1.3.5/seispy/rfcorrect.py` & `python_seispy-1.3.6/seispy/rfcorrect.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             raise ValueError("More than one finallist.dat in the {}".format(data_path))
         else:
             evt_lst = evt_lsts[0]
         self.event, self.phase, self.evla, self.evlo, self.evdp, self.dis, self.bazi, self.rayp, self.mag, self.f0 = \
             np.loadtxt(evt_lst, dtype=self.dtype, unpack=True, ndmin=1)
         self.rayp = skm2srad(self.rayp)
         self.ev_num = self.evla.shape[0]
-        self.read_sample(data_path)
+        self._read_sample(data_path)
         self.data_prime = np.empty([self.ev_num, self.rflength])
         # self.__dict__['data{}'.format(self.comp.lower())] = np.empty([self.ev_num, self.rflength])
         # eval('self.data_prime = self.data{}'.format(self.comp.lower()))
         if not only_r:
             self.datat = np.empty([self.ev_num, self.rflength])
             for _i, evt, ph in zip(range(self.ev_num), self.event, self.phase):
                 sac = SACTrace.read(join(data_path, evt + '_' + ph + '_{}.sac'.format(self.comp)))
@@ -68,15 +68,20 @@
                 self.datat[_i] = sact.data
         else:
             for _i, evt, ph in zip(range(self.ev_num), self.event, self.phase):
                 sac = SACTrace.read(join(data_path, evt + '_' + ph + '_{}.sac'.format(self.comp)))
                 self.data_prime[_i] = sac.data
         exec('self.data{} = self.data_prime'.format(self.comp.lower()))
 
-    def read_sample(self, data_path):
+    def _read_sample(self, data_path):
+        """Read sample SAC file to get station information
+
+        :param data_path: Path to RF data with SAC format
+        :type data_path: str
+        """
         fname = glob.glob(join(data_path, self.event[0] + '_' + self.phase[0] + '_{}.sac'.format(self.comp)))
         if len(fname) == 0:
             raise FileNotFoundError('No such files with comp of {} in {}'.format(self.comp, data_path))
         else:
             sample_sac = SACTrace.read(fname[0])
         self.staname = '{}.{}'.format(sample_sac.knetwk, sample_sac.kstnm)
         self.stla = sample_sac.stla
@@ -86,15 +91,15 @@
         else:
             self.stel = sample_sac.stel
         self.rflength = sample_sac.npts
         self.shift = -sample_sac.b
         self.sampling = sample_sac.delta
         self.time_axis = np.arange(self.rflength) * self.sampling - self.shift
 
-    def init_property(self, ev_num):
+    def _init_property(self, ev_num):
         self.ev_num = ev_num
         self.event = np.array(['']*ev_num)
         self.phase = np.array(['']*ev_num)
         self.evla = np.zeros(ev_num)
         self.evlo = np.zeros(ev_num)
         self.evdp = np.zeros(ev_num)
         self.mag = np.zeros(ev_num)
@@ -114,24 +119,26 @@
         self.datat = np.array([])
         # self.data_prime = eval('self.data{}'.format(self.comp.lower()))
 
     @classmethod
     def read_stream(cls, stream, rayp, baz, prime_comp='R', stream_t=None):
         """Create RFStation instance from ``obspy.Stream``
 
-        Parameters
-        ----------
-        stream : ``obspy.Stream``
-            _description_
-        rayp : ``numpy.ndarray`` or ``float``
-            Ray-parameters in s/km.
-        baz : ``numpy.ndarray`` or ``float``
-            Back-azimuth
-        prime_comp : str, optional
-             Prime component of RF, by default 'R'
+        :param stream: Stream of RFs
+        :type stream: :meth:`obspy.Stream`
+        :param rayp: Ray-parameter of RFs
+        :type rayp: float or :meth:`np.ndarray`
+        :param baz: Back-azimuth of RFs
+        :type baz: float or :meth:`np.ndarray`
+        :param prime_comp: Prime component in RF filename. ``R`` or ``Q`` for PRF and ``L`` or ``Z`` for SRF, defaults to 'R'
+        :type prime_comp: str, optional
+        :param stream_t: Stream of transverse RFs, defaults to None
+        :type stream_t: :meth:`obspy.Stream`, optional
+        :return: RFStation instance
+        :rtype: RFStation
         """
         if len(stream) == 0:
             raise ValueError('No such RFTrace read')
         if stream_t is not None and len(stream) != len(stream_t):
             raise ValueError('Stream and Stream_t must have the same length')
         if stream_t is not None:
             only_r = False
@@ -141,15 +148,15 @@
         ev_num = len(stream)
         if scalar_instance(rayp):
             rayp = np.ones(ev_num)*rayp
         if scalar_instance(baz):
             baz = np.ones(ev_num)*baz
         if ev_num != rayp.size or ev_num != baz.size:
             raise ValueError('Array length of rayp and baz must be the same as stream')
-        rfsta.init_property(ev_num)
+        rfsta._init_property(ev_num)
         try:
             rfsta.staname = '{}.{}'.format(stream[0].stats.sac.knetwk, stream[0].stats.sac.kstnm)
             rfsta.stla = stream[0].stats.sac.stla
             rfsta.stlo = stream[0].stats.sac.stlo
             rfsta.stel = stream[0].stats.sac.stel
         except:
             pass
@@ -222,14 +229,15 @@
         elif self.comp in ['L', 'Z']:
             self.prime_phase = 'S'
         else:
             raise ValueError('prime component should be in \'R\', \'Q\', \'L\' and \'Z\'')
 
     def normalize(self, method='single'):
         """Normalize amplitude of each RFs.
+
         :param method: Method of normalization with ``single`` and ``average`` avaliable.
                      - ``single`` for normalization with max amplitude of current RF.
                      - ``average`` for normalization with average amplitude of current station.
         :type method: str, optional
         """
         if not isinstance(method, str):
             raise TypeError('\'type\' must be string, but {} type got'.format(type(method)))
@@ -245,19 +253,16 @@
             exec('self.data{} = self.data_prime'.format(self.comp.lower()))
             if not self.only_r:
                 self.datat[i] /= maxamp[i]
 
     def resample(self, dt):
         """Resample RFs with specified dt
 
-
-        Parameters
-        ----------
-        dt : ``float``
-            Target sampling interval in sec
+        :param dt: New sampling rate
+        :type dt: float
         """
         npts = int(self.rflength * (self.sampling / dt)) + 1
         self.data_prime = resample(self.data_prime, npts, axis=1)
         exec('self.data{} = self.data_prime'.format(self.comp.lower()))
         if not self.only_r:
             self.datat = resample(self.datat, npts, axis=1)
         self.sampling = dt
@@ -349,24 +354,59 @@
         :rtype: list
         """
         self.dep_range = dep_range
         pplat_s, pplon_s, _ , _, _, _, tps = psrf_1D_raytracing(self, dep_range, **kwargs)
         return pplat_s, pplon_s, tps
 
     def psrf_3D_raytracing(self, mod3dpath, dep_range=np.arange(0, 150), srayp=None):
+        """3D back ray tracing to obtained Ps conversion points at discret depths
+
+        :param mod3dpath: Path to 3D velocity model
+        :type mod3dpath: str
+        :param dep_range: Discret conversion depth, defaults to np.arange(0, 150)
+        :type dep_range: numpy.ndarray, optional
+        :param srayp: Ray-parameter lib for Ps phases, If set up to None the rayp of direct is used, defaults to None
+        :type srayp: numpy.lib.npyio.NpzFile, optional
+        :return pplat_s: Latitude of conversion points
+        :return pplon_s: Longitude of conversion points
+        :return tps: Time difference of Ps at each depth
+        :rtype: list
+        """
         self.dep_range = dep_range
         mod3d = Mod3DPerturbation(mod3dpath, dep_range)
         pplat_s, pplon_s, _, _, tps = psrf_3D_raytracing(self, dep_range, mod3d, srayp=srayp)
         return pplat_s, pplon_s, tps
 
     def psrf_3D_moveoutcorrect(self, mod3dpath, **kwargs):
+        """3D moveout correction with 3D velocity model
+
+        :param mod3dpath: Path to 3D velocity model
+        :type mod3dpath: str
+        :param dep_range: Discret conversion depth, defaults to np.arange(0, 150)
+        :type dep_range: numpy.ndarray, optional
+        :param srayp: Ray-parameter lib for Ps phases, If set up to None the rayp of direct is used, defaults to None
+        :type srayp: numpy.lib.npyio.NpzFile, optional
+        :return: 2D array of RFs in depth
+        :rtype: numpy.ndarray
+        """
         warnings.warn('The fuction will be change to RFStation.psrf_3D_timecorrect in the future')
         self.psrf_3D_timecorrect(mod3dpath, **kwargs)
 
     def psrf_3D_timecorrect(self,  mod3dpath, dep_range=np.arange(0, 150), normalize='single', **kwargs):
+        """3D time-to-depth conversion with 3D velocity model
+        
+        :param mod3dpath: Path to 3D velocity model
+        :type mod3dpath: str
+        :param dep_range: Discret conversion depth, defaults to np.arange(0, 150)
+        :type dep_range: numpy.ndarray, optional
+        :param normalize: Normalization method, defaults to 'single', see RFStation.normalize for detail
+        :type normalize: str, optional
+        :return: 2D array of RFs in depth
+        :rtype: numpy.ndarray
+        """
         self.dep_range = dep_range
         mod3d = Mod3DPerturbation(mod3dpath, dep_range)
         pplat_s, pplon_s, pplat_p, pplon_p, raylength_s, raylength_p, tps = psrf_1D_raytracing(self, dep_range, **kwargs)
         tps = psrf_3D_migration(pplat_s, pplon_s, pplat_p, pplon_p, raylength_s, raylength_p, tps, dep_range, mod3d)
         rfdepth, _ = time2depth(self, dep_range, tps, normalize=normalize)
         return rfdepth
 
@@ -395,46 +435,61 @@
         """
         self.ani = RFAni(self, tb, te, tlen=tlen, rayp=rayp, model=velmodel)
         self.ani.baz_stack(val=stack_baz_val)
         best_f, best_t = self.ani.joint_ani(weight=weight)
         return best_f, best_t
 
     def slantstack(self, ref_dis=None, rayp_range=None, tau_range=None):
+        """Slant stack for receiver function
+
+        :param ref_dis: reference distance, by default None
+        :type ref_dis: int or float, optional
+        :param rayp_range: range of ray parameter, by default None
+        :type rayp_range: numpy.ndarray, optional
+        :param tau_range: range of tau, by default None
+        :type tau_range: numpy.ndarray, optional
+        """
         self.slant = SlantStack(self.data_prime, self.time_axis, self.dis)
         self.slant.stack(ref_dis, rayp_range, tau_range)
         return self.slant.stack_amp
 
     def harmonic(self, tb=-5, te=10, is_stack=True):
         """Harmonic decomposition for extracting anisotropic and isotropic features from the radial and transverse RFs
 
         :param tb: Start time relative to P, defaults to -5
         :type tb: ``float``, optional
         :param te: End time relative to P, defaults to 10
         :type te: ``float``, optional
-
-        Returns
-        -------
-        harmonic_trans: numpy.ndarray, float
-                Harmonic components with shape of ``(5, nsamp)``, ``nsamp = (te-tb)/RFStation.sampling``
-
-        unmodel_trans: numpy.ndarray, float
-                Unmodel components with same shape as harmonic_trans.
+        :param is_stack: Wether stack the result, defaults to True
+        :type is_stack: bool, optional
+        :return: Harmonic components and unmodel components
+        :rtype: ``numpy.ndarray``, ``numpy.ndarray``
         """
         if self.only_r:
             raise ValueError('Transverse RFs are nessary for harmonic decomposition')
         self.harmo = Harmonics(self, tb, te, bin_stack=is_stack)
         self.harmo.harmo_trans()
         return self.harmo.harmonic_trans, self.harmo.unmodel_trans
 
     def plotrt(self, outformat=None, **kwargs):
+        """Plot radial and transverse RFs
+
+        :param outformat: Output format for plot, defaults to None
+        :type outformat: str, optional
+        """
         if self.only_r:
             raise ValueError('Transverse RFs are nessary or use RFStation.plotr instead.')
         return _plotrt(self, outformat=outformat, **kwargs)
 
     def plotr(self, outformat=None, **kwargs):
+        """Plot radial RFs
+
+        :param outformat: Output format for plot, defaults to None
+        :type outformat: str, optional
+        """
         return _plotr(self, outformat=outformat, **kwargs)
 
 
 class SACStation(RFStation):
     def __init__(self, data_path, only_r=False):
         """Class for derivative process of RFs.
```

### Comparing `python-seispy-1.3.5/seispy/scripts.py` & `python_seispy-1.3.6/seispy/scripts.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/seisfwd.py` & `python_seispy-1.3.6/seispy/seisfwd.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/setuplog.py` & `python_seispy-1.3.6/seispy/setuplog.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/signal.py` & `python_seispy-1.3.6/seispy/signal.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/seispy/slantstack.py` & `python_seispy-1.3.6/seispy/slantstack.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,23 @@
         self.ref_dis = 65
         self.rayp_range = np.arange(-0.35, 0.35, 0.01)
         self.tau_range = np.arange(0, 100, 0.1)
         self.syn_tau = np.array([])
         self.syn_drayp = np.array([])
 
     def stack(self, ref_dis=None, rayp_range=None, tau_range=None):
+        """Slant stack for receiver function
+
+        :param ref_dis: reference distance, by default None
+        :type ref_dis: int or float, optional
+        :param rayp_range: range of ray parameter, by default None
+        :type rayp_range: numpy.ndarray, optional
+        :param tau_range: range of tau, by default None
+        :type tau_range: numpy.ndarray, optional
+        """
         if ref_dis is not None and scalar_instance(ref_dis):
             self.ref_dis = ref_dis
         elif ref_dis is None:
             pass
         else:
             raise TypeError('{} should be in int or float type.'.format(ref_dis))
         if rayp_range is not None and array_instance(rayp_range):
@@ -49,14 +58,23 @@
         self.stack_amp = np.zeros([self.rayp_range.shape[0], self.tau_range.shape[0]])
         for i in range(ev_num):
             tps = taus - rayps * (self.dis[i] - self.ref_dis)
             self.stack_amp += interp1d(self.time_axis, self.datar[i, :], fill_value='extrapolate')(tps)
         self.stack_amp /= ev_num
 
     def syn_tps(self, phase_list, velmodel='iasp91', focal_dep=10):
+        """Calculate the theoretical tau and reference rayp for the given phase list
+
+        :param phase_list: phase list for theoretical arrival time
+        :type phase_list: list
+        :param velmodel: velocity model, by default 'iasp91'
+        :type velmodel: str, optional
+        :param focal_dep: focal depth, by default 10
+        :type focal_dep: int or float, optional
+        """
         model = TauPyModel(model=velmodel)
         phase_list.insert(0, 'P')
         arrs = model.get_travel_times(focal_dep, self.ref_dis, phase_list=phase_list)
         p_arr = arrs[0].time
         p_rayp = skm2sdeg(srad2skm(arrs[0].ray_param))
         self.syn_tau = [arr.time - p_arr for arr in arrs[1:]]
         self.syn_drayp = [p_rayp - skm2sdeg(srad2skm(arr.ray_param))for arr in arrs[1:]]
```

### Comparing `python-seispy-1.3.5/seispy/utils.py` & `python_seispy-1.3.6/seispy/utils.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/setup.py` & `python_seispy-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 packages = find_packages()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
-VERSION = "1.3.5"
+VERSION = "1.3.6"
 setup(name='python-seispy',
       version=VERSION,
       author='Mijian Xu',
       long_description=long_description,
       long_description_content_type="text/markdown",
       author_email='gomijianxu@gmail.com',
       license='GPLv3',
```

### Comparing `python-seispy-1.3.5/test/test_case01.py` & `python_seispy-1.3.6/test/test_case01.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/test/test_case02.py` & `python_seispy-1.3.6/test/test_case02.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/test/test_case03.py` & `python_seispy-1.3.6/test/test_case03.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/test/test_case04.py` & `python_seispy-1.3.6/test/test_case04.py`

 * *Files identical despite different names*

### Comparing `python-seispy-1.3.5/test/test_case05.py` & `python_seispy-1.3.6/test/test_case05.py`

 * *Files identical despite different names*


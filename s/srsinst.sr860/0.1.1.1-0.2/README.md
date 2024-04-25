# Comparing `tmp/srsinst.sr860-0.1.1.1.tar.gz` & `tmp/srsinst_sr860-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\instrument_library\sr860\dist\.tmp-68z_f7va\srsinst.sr860-0.1.1.1.tar", last modified: Thu Aug 10 17:40:18 2023, max compression
+gzip compressed data, was "C:\PyPI\instrument drivers to GIT\sr860\dist\.tmp-te_kz69v\srsinst_sr860-0.2.tar", last modified: Thu Apr 25 19:16:59 2024, max compression
```

## Comparing `srsinst.sr860-0.1.1.1.tar` & `srsinst_sr860-0.2.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-08-10 17:40:18.161059 srsinst.sr860-0.1.1.1/
--rw-rw-rw-   0        0        0     1107 2023-01-03 17:25:41.000000 srsinst.sr860-0.1.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     8622 2023-08-10 17:40:18.161059 srsinst.sr860-0.1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     7684 2023-07-05 22:15:49.000000 srsinst.sr860-0.1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-10 17:40:18.111093 srsinst.sr860-0.1.1.1/docs/
-drwxrwxrwx   0        0        0        0 2023-08-10 17:40:18.111093 srsinst.sr860-0.1.1.1/docs/_static/
-drwxrwxrwx   0        0        0        0 2023-08-10 17:40:18.118620 srsinst.sr860-0.1.1.1/docs/_static/image/
--rw-rw-rw-   0        0        0   102698 2023-02-10 20:16:01.000000 srsinst.sr860-0.1.1.1/docs/_static/image/SR860_screenshot.png
--rw-rw-rw-   0        0        0     1375 2023-08-10 16:28:38.000000 srsinst.sr860-0.1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-10 17:40:18.161059 srsinst.sr860-0.1.1.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsinst.sr860-0.1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-10 17:40:18.111093 srsinst.sr860-0.1.1.1/srsinst/
-drwxrwxrwx   0        0        0        0 2023-08-10 17:40:18.128667 srsinst.sr860-0.1.1.1/srsinst/sr860/
--rw-rw-rw-   0        0        0      269 2023-08-10 17:39:36.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/__init__.py
--rw-rw-rw-   0        0        0      485 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/__main__.py
-drwxrwxrwx   0        0        0        0 2023-08-10 17:40:18.128667 srsinst.sr860-0.1.1.1/srsinst/sr860/instruments/
--rw-rw-rw-   0        0        0        0 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/instruments/__init__.py
--rw-rw-rw-   0        0        0    29231 2023-08-10 17:32:25.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/instruments/components.py
--rw-rw-rw-   0        0        0      815 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/instruments/get_instruments.py
--rw-rw-rw-   0        0        0     4134 2023-08-10 17:33:22.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/instruments/keys.py
--rw-rw-rw-   0        0        0     4221 2023-08-10 00:43:04.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/instruments/sr860.py
--rw-rw-rw-   0        0        0     3778 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/instruments/visainterface.py
--rw-rw-rw-   0        0        0     3145 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/instruments/vxi11interface.py
-drwxrwxrwx   0        0        0        0 2023-08-10 17:40:18.138612 srsinst.sr860-0.1.1.1/srsinst/sr860/plots/
--rw-rw-rw-   0        0        0        0 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/plots/__init__.py
--rw-rw-rw-   0        0        0     8576 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/plots/timeplot.py
--rw-rw-rw-   0        0        0     4379 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/plots/twobytwosharexplot.py
--rw-rw-rw-   0        0        0     2021 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/sr860 with sr542.taskconfig
--rw-rw-rw-   0        0        0     3723 2023-08-10 16:32:39.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/sr860.taskconfig
-drwxrwxrwx   0        0        0        0 2023-08-10 17:40:18.151019 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/
--rw-rw-rw-   0        0        0        0 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/__init__.py
--rw-rw-rw-   0        0        0     1142 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/assignparametertochannel.py
--rw-rw-rw-   0        0        0     1477 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/autofunctiontask.py
--rw-rw-rw-   0        0        0     1335 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/auxoutputtask.py
--rw-rw-rw-   0        0        0     2430 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/configurereferencetask.py
--rw-rw-rw-   0        0        0     1539 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/configuresineoutputtask.py
--rw-rw-rw-   0        0        0     2751 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/datatransferfromdatachannelstask.py
--rw-rw-rw-   0        0        0     1321 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/scanauxout1task.py
--rw-rw-rw-   0        0        0     1321 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/scanauxout2task.py
--rw-rw-rw-   0        0        0     1757 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/scanfrequencytask.py
--rw-rw-rw-   0        0        0     1667 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/scanrefamplitudetask.py
--rw-rw-rw-   0        0        0     1539 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/scanrefoffsettask.py
--rw-rw-rw-   0        0        0     1756 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/selecttimebasetask.py
--rw-rw-rw-   0        0        0     2425 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/setreferencetochoptask.py
--rw-rw-rw-   0        0        0     2343 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/setreferencetodualtask.py
--rw-rw-rw-   0        0        0     2186 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/setreferencetoexternaltask.py
--rw-rw-rw-   0        0        0     7552 2023-07-19 23:45:23.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/setreferencetoexternalwithsr542task.py
--rw-rw-rw-   0        0        0     1907 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/setreferencetointernaltask.py
--rw-rw-rw-   0        0        0     1195 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/sidntesttask.py
--rw-rw-rw-   0        0        0     1740 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/signaltocurrentmodetask.py
--rw-rw-rw-   0        0        0     2112 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/signaltovoltagemodetask.py
--rw-rw-rw-   0        0        0     1458 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/simulatedplot.py
--rw-rw-rw-   0        0        0     3427 2023-07-14 21:17:42.000000 srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/streamingtask.py
-drwxrwxrwx   0        0        0        0 2023-08-10 17:40:18.118620 srsinst.sr860-0.1.1.1/srsinst.sr860.egg-info/
--rw-rw-rw-   0        0        0     8622 2023-08-10 17:40:17.000000 srsinst.sr860-0.1.1.1/srsinst.sr860.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1856 2023-08-10 17:40:18.000000 srsinst.sr860-0.1.1.1/srsinst.sr860.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-10 17:40:17.000000 srsinst.sr860-0.1.1.1/srsinst.sr860.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-08-10 17:40:17.000000 srsinst.sr860-0.1.1.1/srsinst.sr860.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       67 2023-08-10 17:40:17.000000 srsinst.sr860-0.1.1.1/srsinst.sr860.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-10 17:40:17.000000 srsinst.sr860-0.1.1.1/srsinst.sr860.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-10 17:40:18.151019 srsinst.sr860-0.1.1.1/tests/
--rw-rw-rw-   0        0        0     3368 2023-03-06 17:34:08.000000 srsinst.sr860-0.1.1.1/tests/test_sr860.py
+drwxrwxrwx   0        0        0        0 2024-04-25 19:16:59.552269 srsinst_sr860-0.2/
+-rw-rw-rw-   0        0        0     1968 2023-02-10 18:32:29.000000 srsinst_sr860-0.2/.gitignore
+-rw-rw-rw-   0        0        0     1107 2023-01-03 17:25:41.000000 srsinst_sr860-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     8925 2024-04-25 19:16:59.552269 srsinst_sr860-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7818 2024-04-25 18:55:20.000000 srsinst_sr860-0.2/README.md
+-rw-rw-rw-   0        0        0   102698 2023-02-10 20:16:01.000000 srsinst_sr860-0.2/SR860_screenshot.png
+drwxrwxrwx   0        0        0        0 2024-04-25 19:16:59.493195 srsinst_sr860-0.2/docs/
+drwxrwxrwx   0        0        0        0 2024-04-25 19:16:59.493195 srsinst_sr860-0.2/docs/_static/
+drwxrwxrwx   0        0        0        0 2024-04-25 19:16:59.512318 srsinst_sr860-0.2/docs/_static/image/
+-rw-rw-rw-   0        0        0   102698 2023-02-10 20:16:01.000000 srsinst_sr860-0.2/docs/_static/image/SR860_screenshot.png
+-rw-rw-rw-   0        0        0    55539 2024-04-25 19:09:37.000000 srsinst_sr860-0.2/getting_started.ipynb
+-rw-rw-rw-   0        0        0     1375 2023-08-10 16:28:38.000000 srsinst_sr860-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 19:16:59.552269 srsinst_sr860-0.2/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsinst_sr860-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 19:16:59.493195 srsinst_sr860-0.2/srsinst/
+drwxrwxrwx   0        0        0        0 2024-04-25 19:16:59.522285 srsinst_sr860-0.2/srsinst/sr860/
+-rw-rw-rw-   0        0        0      337 2024-04-23 18:09:53.000000 srsinst_sr860-0.2/srsinst/sr860/__init__.py
+-rw-rw-rw-   0        0        0      485 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 19:16:59.532280 srsinst_sr860-0.2/srsinst/sr860/instruments/
+-rw-rw-rw-   0        0        0        0 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/instruments/__init__.py
+-rw-rw-rw-   0        0        0    29231 2023-11-13 17:14:22.000000 srsinst_sr860-0.2/srsinst/sr860/instruments/components.py
+-rw-rw-rw-   0        0        0      815 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/instruments/get_instruments.py
+-rw-rw-rw-   0        0        0     4134 2023-08-10 17:33:22.000000 srsinst_sr860-0.2/srsinst/sr860/instruments/keys.py
+-rw-rw-rw-   0        0        0     4221 2023-08-10 00:43:04.000000 srsinst_sr860-0.2/srsinst/sr860/instruments/sr860.py
+-rw-rw-rw-   0        0        0     3778 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/instruments/visainterface.py
+-rw-rw-rw-   0        0        0     3145 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/instruments/vxi11interface.py
+drwxrwxrwx   0        0        0        0 2024-04-25 19:16:59.532280 srsinst_sr860-0.2/srsinst/sr860/plots/
+-rw-rw-rw-   0        0        0        0 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/plots/__init__.py
+-rw-rw-rw-   0        0        0     8576 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/plots/timeplot.py
+-rw-rw-rw-   0        0        0     4379 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/plots/twobytwosharexplot.py
+-rw-rw-rw-   0        0        0     2021 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/sr860 with sr542.taskconfig
+-rw-rw-rw-   0        0        0     3723 2023-08-10 16:32:39.000000 srsinst_sr860-0.2/srsinst/sr860/sr860.taskconfig
+drwxrwxrwx   0        0        0        0 2024-04-25 19:16:59.552269 srsinst_sr860-0.2/srsinst/sr860/tasks/
+-rw-rw-rw-   0        0        0        0 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/__init__.py
+-rw-rw-rw-   0        0        0     1142 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/assignparametertochannel.py
+-rw-rw-rw-   0        0        0     1477 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/autofunctiontask.py
+-rw-rw-rw-   0        0        0     1335 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/auxoutputtask.py
+-rw-rw-rw-   0        0        0     2385 2023-08-11 22:07:44.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/configurereferencetask.py
+-rw-rw-rw-   0        0        0     1539 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/configuresineoutputtask.py
+-rw-rw-rw-   0        0        0     2751 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/datatransferfromdatachannelstask.py
+-rw-rw-rw-   0        0        0     1321 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/scanauxout1task.py
+-rw-rw-rw-   0        0        0     1321 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/scanauxout2task.py
+-rw-rw-rw-   0        0        0     1757 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/scanfrequencytask.py
+-rw-rw-rw-   0        0        0     1667 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/scanrefamplitudetask.py
+-rw-rw-rw-   0        0        0     1539 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/scanrefoffsettask.py
+-rw-rw-rw-   0        0        0     1756 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/selecttimebasetask.py
+-rw-rw-rw-   0        0        0     2425 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/setreferencetochoptask.py
+-rw-rw-rw-   0        0        0     2343 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/setreferencetodualtask.py
+-rw-rw-rw-   0        0        0     2186 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/setreferencetoexternaltask.py
+-rw-rw-rw-   0        0        0     7552 2023-07-19 23:45:23.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/setreferencetoexternalwithsr542task.py
+-rw-rw-rw-   0        0        0     1907 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/setreferencetointernaltask.py
+-rw-rw-rw-   0        0        0     1195 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/sidntesttask.py
+-rw-rw-rw-   0        0        0     1740 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/signaltocurrentmodetask.py
+-rw-rw-rw-   0        0        0     2112 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/signaltovoltagemodetask.py
+-rw-rw-rw-   0        0        0     1458 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/simulatedplot.py
+-rw-rw-rw-   0        0        0     3427 2023-07-14 21:17:42.000000 srsinst_sr860-0.2/srsinst/sr860/tasks/streamingtask.py
+drwxrwxrwx   0        0        0        0 2024-04-25 19:16:59.552269 srsinst_sr860-0.2/srsinst.sr860.egg-info/
+-rw-rw-rw-   0        0        0     8925 2024-04-25 19:16:59.000000 srsinst_sr860-0.2/srsinst.sr860.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1880 2024-04-25 19:16:59.000000 srsinst_sr860-0.2/srsinst.sr860.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 19:16:59.000000 srsinst_sr860-0.2/srsinst.sr860.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-25 19:16:59.000000 srsinst_sr860-0.2/srsinst.sr860.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       67 2024-04-25 19:16:59.000000 srsinst_sr860-0.2/srsinst.sr860.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 19:16:59.000000 srsinst_sr860-0.2/srsinst.sr860.egg-info/top_level.txt
```

### Comparing `srsinst.sr860-0.1.1.1/LICENSE.txt` & `srsinst_sr860-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/PKG-INFO` & `srsinst_sr860-0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,15 @@
-Metadata-Version: 2.1
-Name: srsinst.sr860
-Version: 0.1.1.1
-Summary: Instrument driver package for the Lock-In Amplifiers, SR860 series from Stanford Research Systems
-Author: Chulhoon Kim
-License: MIT license
-Project-URL: homepage, https://github.com/thinkSRS/srsinst.sr860
-Project-URL: repository, https://github.com/thinkSRS/srsinst.sr860.git
-Keywords: SR860,SR865A,SRS,Stanford Research Systems,lock-in amplifier
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: full
-License-File: LICENSE.txt
-
 # Srsinst.sr860
 
 `srsinst.sr860` is a Python package to control and acquire data from  
 [Stanford Research Systems (SRS) SR860 series Lock-In Amplifiers](https://thinksrs.com/products/sr865a.html):
- SR860, SR865 and SR865A.
+SR860, SR865 and SR865A. If you prefer instructional videos, 
+watch [these videos](https://www.youtube.com/playlist?list=PLnZT3yqji4iXZsnPbufkaAGROhm99UvKP).
 
-![screenshot](https://github.com/thinkSRS/srsinst.sr860/blob/main/docs/_static/image/SR860_screenshot.png?raw=true " ")
+![screenshot](https://github.com/thinkSRS/srsinst.sr860/blob/main/docs/_static/image/SR860_screenshot.png?raw=true " ").
 
 ## Installation
 You need a working Python 3.7 or later with `pip` (Python package installer) 
 installed. If you don't, [install Python](https://www.python.org/) to your system.
 
 To install `srsinst.sr860` as an instrument driver , use Python package installer `pip` from the command line.
```

### Comparing `srsinst.sr860-0.1.1.1/README.md` & `srsinst_sr860-0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,42 @@
+Metadata-Version: 2.1
+Name: srsinst.sr860
+Version: 0.2
+Summary: Instrument driver package for the Lock-In Amplifiers, SR860 series from Stanford Research Systems
+Author: Chulhoon Kim
+License: MIT license
+Project-URL: homepage, https://github.com/thinkSRS/srsinst.sr860
+Project-URL: repository, https://github.com/thinkSRS/srsinst.sr860.git
+Keywords: SR860,SR865A,SRS,Stanford Research Systems,lock-in amplifier
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: python-vxi11
+Requires-Dist: srsgui>=0.4.3
+Provides-Extra: full
+Requires-Dist: matplotlib>=3.6.2; extra == "full"
+Requires-Dist: pyside6; extra == "full"
+
 # Srsinst.sr860
 
 `srsinst.sr860` is a Python package to control and acquire data from  
 [Stanford Research Systems (SRS) SR860 series Lock-In Amplifiers](https://thinksrs.com/products/sr865a.html):
- SR860, SR865 and SR865A.
+SR860, SR865 and SR865A. If you prefer instructional videos, 
+watch [these videos](https://www.youtube.com/playlist?list=PLnZT3yqji4iXZsnPbufkaAGROhm99UvKP).
 
-![screenshot](https://github.com/thinkSRS/srsinst.sr860/blob/main/docs/_static/image/SR860_screenshot.png?raw=true " ")
+![screenshot](https://github.com/thinkSRS/srsinst.sr860/blob/main/docs/_static/image/SR860_screenshot.png?raw=true " ").
 
 ## Installation
 You need a working Python 3.7 or later with `pip` (Python package installer) 
 installed. If you don't, [install Python](https://www.python.org/) to your system.
 
 To install `srsinst.sr860` as an instrument driver , use Python package installer `pip` from the command line.
```

### Comparing `srsinst.sr860-0.1.1.1/docs/_static/image/SR860_screenshot.png` & `srsinst_sr860-0.2/SR860_screenshot.png`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/pyproject.toml` & `srsinst_sr860-0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/instruments/components.py` & `srsinst_sr860-0.2/srsinst/sr860/instruments/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,16 +71,16 @@
 
     timebase_mode = DictCommand('TBMODE', TimebaseModeDict)
     timebase_source = DictCommand('TBSTAT', TimebaseSourceDict)
 
     blade_slots = DictCommand('BLADESLOTS', BladeSlotsDict, None, 'slots')
     blade_phase = FloatCommand('BLADEPHASE', '°')
     
-    sine_out_amplitude = FloatCommand('SLVL', ' V', 0, 2.0, 1e-9, 4, 0.0)
-    sine_out_offset = FloatCommand('SOFF', 'V', -5.0, 5.0, 1e-4, 4, 0.0)
+    sine_out_amplitude = FloatCommand('SLVL', ' V', 0, 2.0, 1e-9, 3, 0.0)
+    sine_out_offset = FloatCommand('SOFF', 'V', -5.0, 5.0, 1e-4, 3, 0.0)
     sine_out_dc_mode = DictCommand('REFM', SineOutDCModeDict)
     reference_source = DictCommand('RSRC', ReferenceSourceDict)
     
     trigger_mode = DictCommand('RTRG', TriggerModeDict)
     trigger_input = DictCommand('REFZ', TriggerInputDict)
 
     def __init__(self, parent):
```

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/instruments/get_instruments.py` & `srsinst_sr860-0.2/srsinst/sr860/instruments/get_instruments.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/instruments/keys.py` & `srsinst_sr860-0.2/srsinst/sr860/instruments/keys.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/instruments/sr860.py` & `srsinst_sr860-0.2/srsinst/sr860/instruments/sr860.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/instruments/visainterface.py` & `srsinst_sr860-0.2/srsinst/sr860/instruments/visainterface.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/instruments/vxi11interface.py` & `srsinst_sr860-0.2/srsinst/sr860/instruments/vxi11interface.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/plots/timeplot.py` & `srsinst_sr860-0.2/srsinst/sr860/plots/timeplot.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/plots/twobytwosharexplot.py` & `srsinst_sr860-0.2/srsinst/sr860/plots/twobytwosharexplot.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/sr860 with sr542.taskconfig` & `srsinst_sr860-0.2/srsinst/sr860/sr860 with sr542.taskconfig`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/sr860.taskconfig` & `srsinst_sr860-0.2/srsinst/sr860/sr860.taskconfig`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/assignparametertochannel.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/assignparametertochannel.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/autofunctiontask.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/autofunctiontask.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/auxoutputtask.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/auxoutputtask.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/configurereferencetask.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/configurereferencetask.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ##! Copyright(c) 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import time
 
 from srsgui import Task
-from srsgui import BoolInput, IntegerListInput, FloatListInput, InstrumentInput, CommandInput
+from srsgui import InstrumentInput, CommandInput
 from srsinst.sr860 import SR860, get_sr860
 
 from srsinst.sr860.instruments.components import Signal, Reference
 from srsinst.sr860.instruments.keys import Keys
 
 
 class ConfigureReferenceTask(Task):
```

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/configuresineoutputtask.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/configuresineoutputtask.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/datatransferfromdatachannelstask.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/datatransferfromdatachannelstask.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/scanauxout1task.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/scanauxout1task.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/scanauxout2task.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/scanauxout2task.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/scanfrequencytask.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/scanfrequencytask.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/scanrefamplitudetask.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/scanrefamplitudetask.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/scanrefoffsettask.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/scanrefoffsettask.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/selecttimebasetask.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/selecttimebasetask.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/setreferencetochoptask.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/setreferencetochoptask.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/setreferencetodualtask.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/setreferencetodualtask.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/setreferencetoexternaltask.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/setreferencetoexternaltask.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/setreferencetoexternalwithsr542task.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/setreferencetoexternalwithsr542task.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/setreferencetointernaltask.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/setreferencetointernaltask.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/sidntesttask.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/sidntesttask.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/signaltocurrentmodetask.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/signaltocurrentmodetask.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/signaltovoltagemodetask.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/signaltovoltagemodetask.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/simulatedplot.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/simulatedplot.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst/sr860/tasks/streamingtask.py` & `srsinst_sr860-0.2/srsinst/sr860/tasks/streamingtask.py`

 * *Files identical despite different names*

### Comparing `srsinst.sr860-0.1.1.1/srsinst.sr860.egg-info/PKG-INFO` & `srsinst_sr860-0.2/srsinst.sr860.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsinst.sr860
-Version: 0.1.1.1
+Version: 0.2
 Summary: Instrument driver package for the Lock-In Amplifiers, SR860 series from Stanford Research Systems
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsinst.sr860
 Project-URL: repository, https://github.com/thinkSRS/srsinst.sr860.git
 Keywords: SR860,SR865A,SRS,Stanford Research Systems,lock-in amplifier
 Classifier: Development Status :: 3 - Alpha
@@ -13,24 +13,30 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: full
 License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: python-vxi11
+Requires-Dist: srsgui>=0.4.3
+Provides-Extra: full
+Requires-Dist: matplotlib>=3.6.2; extra == "full"
+Requires-Dist: pyside6; extra == "full"
 
 # Srsinst.sr860
 
 `srsinst.sr860` is a Python package to control and acquire data from  
 [Stanford Research Systems (SRS) SR860 series Lock-In Amplifiers](https://thinksrs.com/products/sr865a.html):
- SR860, SR865 and SR865A.
+SR860, SR865 and SR865A. If you prefer instructional videos, 
+watch [these videos](https://www.youtube.com/playlist?list=PLnZT3yqji4iXZsnPbufkaAGROhm99UvKP).
 
-![screenshot](https://github.com/thinkSRS/srsinst.sr860/blob/main/docs/_static/image/SR860_screenshot.png?raw=true " ")
+![screenshot](https://github.com/thinkSRS/srsinst.sr860/blob/main/docs/_static/image/SR860_screenshot.png?raw=true " ").
 
 ## Installation
 You need a working Python 3.7 or later with `pip` (Python package installer) 
 installed. If you don't, [install Python](https://www.python.org/) to your system.
 
 To install `srsinst.sr860` as an instrument driver , use Python package installer `pip` from the command line.
```

### Comparing `srsinst.sr860-0.1.1.1/srsinst.sr860.egg-info/SOURCES.txt` & `srsinst_sr860-0.2/srsinst.sr860.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+.gitignore
 LICENSE.txt
 README.md
+SR860_screenshot.png
+getting_started.ipynb
 pyproject.toml
-readme.md
 setup.py
 docs/_static/image/SR860_screenshot.png
 srsinst.sr860.egg-info/PKG-INFO
 srsinst.sr860.egg-info/SOURCES.txt
 srsinst.sr860.egg-info/dependency_links.txt
 srsinst.sr860.egg-info/entry_points.txt
 srsinst.sr860.egg-info/requires.txt
@@ -42,9 +44,8 @@
 srsinst/sr860/tasks/setreferencetoexternaltask.py
 srsinst/sr860/tasks/setreferencetoexternalwithsr542task.py
 srsinst/sr860/tasks/setreferencetointernaltask.py
 srsinst/sr860/tasks/sidntesttask.py
 srsinst/sr860/tasks/signaltocurrentmodetask.py
 srsinst/sr860/tasks/signaltovoltagemodetask.py
 srsinst/sr860/tasks/simulatedplot.py
-srsinst/sr860/tasks/streamingtask.py
-tests/test_sr860.py
+srsinst/sr860/tasks/streamingtask.py
```

